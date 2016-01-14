---
layout: shared/narrow
published: false
title: "Where does the code live?"
description: "A basic service worker implementation requires code in two places."
published_on: 2015-10-01
updated_on: 2015-10-01
order: 3
translation_priority: 0
authors:
- josephmedley
---

<p class="intro">
  A basic service worker implementation requires code in two places.
</p>

 
### Clients

A client is a web page that uses a service worker. One or more clients 
can use the same service worker. All they need do is implement the 
registration code, which we'll look at in the next section.

### Service worker script

This is a background script that acts as a network proxy for one or
more clients. Though its name implies activity, you can almost think of a
service worker as a passive player, one that only runs when one of its
event handlders are fired. It can't even manipulate its clients' DOMs.

### Clients don't need service workers

If you follow the principles of progressive enhancement, you'll be happy to know 
that clients should function without service workers. This is the key to the 
service worker's design. 

First and foremost, it allows for user engagement to occur while the service 
worker is loading and installing. This is because the service worker life cycle 
is independent of a client page's life cycle. Hence, the service worker 
doesn't block the page. It also allows the page to function on browsers that 
don't support service workers and simplifies adding service workers to existing 
pages. 
