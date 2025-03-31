---
title: Designing Data-Intensive Applications
subtitle: The Big Ideas Behind Reliable, Scalable, and Maintainable Systems
author:
  - Martin Kleppmann
tags:
  - 📚Book
status: Reading
totalPages: "613"
currentPages: "11"
---

Intro

## Chapter 1 - Reliable, Scalable, and Maintainable Applications

> When you combine several tools in order to provide a service, the service’s interface or application programming interface (API) usually hides those implementation details from clients. Now you have essentially created a new, special-purpose data system from smaller, general-purpose components.

[[ddia.pdf#page=27&selection=3,0,6,48|ddia, p.5]]

**Reliability**: The system should continue to work correctly (performing the correct function at the desired level of performance) even in the face of adversity

**Scalability**: As the system grows (in data volume, traffic volume, or complexity), there should be reasonable ways of dealing with that growth.

**Maintainability**: Over time, many different people will work on the system (engineering and operations, both maintaining current behavior and adapting the system to new use cases), and they should all be able to work on it productively.

> The things that can go wrong are called faults, and systems that anticipate faults and can cope with them are called fault-tolerant or resilient

[[ddia.pdf#page=28&selection=57,0,68,0|ddia, p.6]]

> There are situations in which we may choose to sacrifice reliability in order to reduce development cost (e.g., when developing a prototype product for an unproven mar‐ ket) or operational cost (e.g., for a service with a very narrow profit margin)—but we should be very conscious of when we are cutting corners

[[ddia.pdf#page=32&selection=30,0,33,55|ddia, p.10]]

> scalability means considering questions like “If the system grows in a particular way, what are our options for coping with the growth?” and “How can we add computing resources to handle the additional load?”

[[ddia.pdf#page=33&selection=5,0,7,41|ddia, p.11]]

> For example, a system that is designed to handle 100,000 requests per second, each 1 kB in size, looks very different from a system that is designed for 3 requests per minute, each 2 GB in size—even though the two systems have the same data through‐ put.

[[ddia.pdf#page=40&selection=20,0,23,4|ddia, p.18]]

> Reliability means making systems work correctly, even when faults occur. Faults can be in hardware (typically random and uncorrelated), software (bugs are typically sys‐ tematic and hard to deal with), and humans (who inevitably make mistakes from time to time). Fault-tolerance techniques can hide certain types of faults from the end user.

[[ddia.pdf#page=44&selection=45,0,51,5|ddia, p.22]]

## Chapter 2 - Data Models and Query Languages
