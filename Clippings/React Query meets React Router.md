---
title: "React Query meets React Router"
source: "https://tkdodo.eu/blog/react-query-meets-react-router"
author:
  - "[[TkDodo]]"
created: 2024-11-13
published: 28.08.2022
description: "React Query and React Router are a match made in heaven."
tags:
  - "clippings"
---
28.08.2022 — [ReactJs](https://tkdodo.eu/blog/tags/react-js), [React Query](https://tkdodo.eu/blog/tags/react-query), [React Router](https://tkdodo.eu/blog/tags/react-router), [TypeScript](https://tkdodo.eu/blog/tags/type-script), [JavaScript](https://tkdodo.eu/blog/tags/java-script) — 6 min read

## A router that fetches data

To recap: React Router will allow you to define [loaders](https://reactrouter.com/en/6.4.0/route/loader) on each route, which will be called when the route is visited. In the route component itself, you can `useLoaderData()` to get access to that data. Updating data is as simple as submitting a `Form`, which will call an [action](https://reactrouter.com/en/6.4.0/route/action) function. Actions invalidate all active loaders, so you'll automagically see updated data on your screen.

If this sounds very similar to `queries` and `mutations` - you are right, it does. So the questions that have been popping up after the announcement of [Remixing React Router](https://remix.run/blog/remixing-react-router) are:

- Would we still want React Query now that we can fetch in the route?
- If we already use React Query, do we want to (and how can we) leverage the new React Router features?

### It's not a cache

To me, the answers to both questions are clearly: YES. As [Ryan Florence](https://twitter.com/ryanflorence) from the remix team has put it: "React Router is not a cache":

[

![](https://tkdodo.eu/blog/www.w3.org/2000/svg'%20version='1.1'%3E%3C/svg%3E)

![](https://tkdodo.eu/blog/2wBDABALDA4MChAODQ4SERATGCgaGBYWGDEjJR0oOjM9PDkzODdASFxOQERXRTc4UG1RV19iZ2hnPk1xeXBkeFxlZ2P/2wBDARESEhgVGC8aGi9jQjhCY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2NjY2P/wgARCAAUABQDASIAAhEBAxEB/8QAGAABAQEBAQAAAAAAAAAAAAAAAAUEAQP/xAAXAQADAQAAAAAAAAAAAAAAAAAAAQMC/9oADAMBAAIQAxAAAAHXMozJ0rspHfAboAz/AP/EABsQAAICAwEAAAAAAAAAAAAAAAECAAMREjEy/9oACAEBAAEFAiVEDvnZZbxCxmxErGyjlfj/xAAXEQEAAwAAAAAAAAAAAAAAAAAQAREx/9oACAEDAQE/AaJ0/8QAFREBAQAAAAAAAAAAAAAAAAAAESD/2gAIAQIBAT8BY//EABsQAAMAAgMAAAAAAAAAAAAAAAABEQIxECIy/9oACAEBAAY/AnlHSrZ22OEPNHef/8QAGxABAAMBAQEBAAAAAAAAAAAAAQAhMRFBUYH/2gAIAQEAAT8hYBj8ZqnGv2FvFoqOctizh9Zjq8WC/RUqn9j4J//aAAwDAQACAAMAAAAQY8g//8QAGBEAAgMAAAAAAAAAAAAAAAAAABEBEEH/2gAIAQMBAT8QXRRZ/8QAGBEBAQADAAAAAAAAAAAAAAAAAQAQETH/2gAIAQIBAT8QEW2OY//EABwQAQEAAgMBAQAAAAAAAAAAAAERACExQWGBkf/aAAgBAQABPxAldLQ2z3rHml+zt3m+USsqfMUWAgpGpqfm81VRjPG9zAFjmA8YzKhD59xJDdipaxxwHBxn/9k=)![Avatar for ryanflorence](https://tkdodo.eu/blog/static/39f03fb56a95b14d9441ba73908ecc8a/47930/ryanflorence.jpg)

![Avatar for ryanflorence](/blog/static/39f03fb56a95b14d9441ba73908ecc8a/47930/ryanflorence.jpg)

Ryan Florence

@ryanflorence

Nah, React Router is not a cache.

Browsers have this built in with HTTP and libraries like React Query have this job nailed down.

React Router is about \*when\*, data caching libs are about \*what\*.

\- Aug 21, 2022

](https://twitter.com/ryanflorence/status/1561731634419773447)

Fetching "as early as possible" is an important concept to provide the best possible user experience. Full Stack frameworks like [NextJs](https://nextjs.org/) or Remix move this step to the server, because that is the earliest entry point. With client rendered applications, we have no such luxury.

### Fetching early

What we are usually doing is fetching on component mount - when data is first needed. That is not great, as it will lead to a loading spinner visible to the user for as long as we are initially fetching. [Prefetching](https://tanstack.com/query/v4/docs/guides/prefetching) can help, but only for subsequent navigations, and you need to manually set it up for every way to navigate to a route.

The router however is the first component that always knows which page you are trying to visit, and because it now has loaders, it can know which data those pages need to render. This is great for the first page visit - but loaders are called on *every* page visit. And as the router has no cache, it will hit the server again, unless we do something about it.

As an example (yes, this is from the tutorial mentioned before. Credits go to Ryan Florence), suppose you have a list of contacts. If you click on one of them, you show the contact details:

```jsx
1import { useLoaderData } from 'react-router-dom'2import { getContact } from '../contacts'3
4// ⬇️ this is the loader for the detail route5export async function loader({ params }) {6  return getContact(params.contactId)7}8
9export default function Contact() {10  // ⬇️ this gives you data from the loader11  const contact = useLoaderData()12  // render some jsx13}
```

```jsx
1import Contact, { loader as contactLoader } from './routes/contact'2
3const router = createBrowserRouter([4  {5    path: '/',6    element: <Root />,7    children: [8      {9        path: 'contacts',10        element: <Contacts />,11        children: [12          {13            path: 'contacts/:contactId',14            element: <Contact />,15            // ⬇️ this is the loader for the detail route16            loader: contactLoader,17          },18        ],19      },20    ],21  },22])
```

If you navigate to `contacts/1`, data for that contact will be fetched *before* the component is rendered. By the time we want to show the Contact, `useLoaderData` will have data readily available. This is awesome as it not only improves the user experience, but look at that developer experience of co-located data fetching and rendering! I love it. 🥰

### Fetching too often

The big drawback of not having a cache shows when you go to Contact 2 and then back to Contact 1 again. If you are used to React Query, you will know that data for Contact 1 is cached already, so we can show it instantly and kick of a background refetch if data is considered stale. With the loader approach, we will have to fetch that data again (and wait for it to finish fetching!), even though we have already fetched it before.

And that is exactly where React Query comes in.

What if we can use the loader to pre-fill the React Query Cache, but still `useQuery` in the component to get all the React Query goodies like `refetchOnWindowFocus` and showing stale data instantly? To me, this sounds like the best of both worlds. The router is responsible for fetching data early (if we don't have it), and React Query is responsible for caching and keeping the data fresh.

## Querifying the example

Let's try to move the example in that direction:

There are a couple of things going on here, so let's break it down:

### The loader needs access to the QueryClient.

The loader is not a hook, so we can't `useQueryClient`. Importing the QueryClient directly is something that [I'm not recommending](https://tkdodo.eu/blog/react-query-fa-qs#why-should-i-usequeryclient), so passing it explicitly seems like the best alternative.

### getQueryData ?? fetchQuery

We want the loader to wait for our data to be ready and return it to get a good experience on the first loads. We also want errors to be thrown to the [errorElement](https://reactrouter.com/en/6.4.0/route/error-element), so `fetchQuery` is the best option. Note that `prefetchQuery` doesn't return anything and catches errors internally (otherwise, they are equivalent).

`getQueryData` does the trick for returning any data we have in the cache, even if it's stale. This ensures that recurring visits to a page will show data immediately. Only if `getQueryData` returns `undefined` (meaning nothing is in the cache), we'll actually do the fetch.

An alternative approach would be to set a `staleTime` for `fetchQuery`:

```jsx
1export const loader =2  (queryClient) =>3  ({ params }) =>4    queryClient.fetchQuery({5      ...contactDetailQuery(params.contactId),6      staleTime: 1000 * 60 * 2,7    })
```

Setting the `staleTime` to two minutes tells `fetchQuery` to resolve data immediately if it's available and not older than two minutes, otherwise, it will go and fetch it. If you are fine with stale data *not* being shown in the component, this is a good alternative.

Setting `staleTime` to `Infinity` is almost equivalent to the `getQueryData` approach, except that manual query invalidation takes precedence over `staleTime`. So I like the `getQueryData` approach a bit better, even if it is slightly more code.

​Update: As of [v4.18.0](https://github.com/TanStack/query/releases/tag/v4.18.0), you can use the built-in [queryClient.ensureQueryData](https://tanstack.com/query/v4/docs/reference/QueryClient#queryclientensurequerydata) method to achieve the same thing. It is literally implemented with `getQueryData ?? fetchQuery`, but it's a common enough use-case for the library to have it out of the box.

## Summary

I'm very excited about the new React Router release. It's a great step forward to enable all applications to trigger fetches as early as possible. However, it is not a replacement for caching - so go ahead and combine React Router with React Query to get the best of both worlds. 🚀