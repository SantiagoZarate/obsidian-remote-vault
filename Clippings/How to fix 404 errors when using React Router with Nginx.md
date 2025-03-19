---
title: "How to fix 404 errors when using React Router with Nginx"
source: "https://www.frontendundefined.com/posts/tutorials/nginx-react-router-404/"
author:
  - "[[Frontend undefined]]"
created: 2024-11-13
published: 2023-06-07
description: "This post describes how you can fix 404 errors that occur when using Nginx with React router"
tags:
  - "clippings"
---
If you are using Nginx to host a React app with React Router, you might come across a 404 error when you directly load a React Router Route. For example, if you have a route with the path `/about-us`, it might work when you load the root route `/` and navigate to `/about-us` by clicking on a link but it will return a 404 when you try to load `/about-us` directly

![Nginx 404 not found error screen](https://www.frontendundefined.com/posts/tutorials/nginx-react-router-404/nginx-404-not-found-720w.jpeg "404 Not Found")

## Why doesn't this work?

This error occurs because React Router uses client-side routing. Client-side routing is where routes or paths are emulated in the browser using JavaScript and the [History API](https://developer.mozilla.org/en-US/docs/Web/API/History_API). Those routes don't exist on the disk as web pages and web servers like Nginx, attempt to serve web pages from the disk by default. So in our example, Nginx will attempt to serve `about-us/index.html` from the disk when `/about-us` is requested and will fail since it doesn't exist.

Single page applications (SPAs) like the ones built with React run within a single web page that is loaded from the server. Even though a React app might have several screens implemented as different Routes within React Router, all of those screens are displayed using JavaScript by overwriting the contents of a single web page. So when we build a React app, a single `index.html` file is outputted along with the JavaScript and CSS files necessary to run it. When these files are placed in the root folder of a web server, navigating to the root route `/` will load `index.html` which will cause React to start.

## How to fix it

To get React Router's routes to work with Nginx, we need to configure Nginx to serve `index.html` for all non-existent paths that are requested from it. To do this, we can use the following Nginx configuration.

```nginx
server {
	listen       80;
	listen  [::]:80;
	
	location / {
		root   /usr/share/nginx/html;
		try_files $uri $uri/ /index.html;
	}
}
```

On most Linux systems, this configuration should be saved in a `.conf` file in the `/etc/nginx/conf.d/` folder. All the configuration files in that folder are added within the `http` section of the primary nginx configuration file in `/etc/nginx/nginx.conf`. You can name the `.conf` file whatever you choose (e.g.: `default.conf`). You can use the following commands to create and edit the configuration file and restart nginx on most Linux servers.

```shell-session
$ sudo nano /etc/nginx/conf.d/default.conf$ sudo systemctl restart nginx
```

The key part of this configuration is the `try_files` directive which configures nginx to try and serve a file from the disk if it exists and to serve index.html if it doesn't. We need to instruct nginx to try and serve the file from the disk first so that it can properly serve the `.css` and `.js` files that are also output when a React app is built for production.

Note that with this configuration, nginx will never return a 404 and will always serve index.html regardless of the path that is requested from it. So you need to [set up a 404 route with React router](https://reactrouter.com/en/main/start/faq#how-do-i-add-a-no-match-404-route-in-react-router-v6) to show a meaningful message to the user in the case of an invalid URL.