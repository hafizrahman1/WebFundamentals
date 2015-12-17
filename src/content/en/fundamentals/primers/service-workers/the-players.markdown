---
layout: shared/narrow
published: false
title: "The Players"
description: "A basic service worker implementation has two types of players."
published_on: 2015-10-01
updated_on: 2015-10-01
order: 3
translation_priority: 0
authors:
- josephmedley
---

<p class="intro">
  A basic service worker implementation has two types of players.
</p>

 
### Clients

A client is a web page that uses a service worker.

### Service worker script

This player is a background script that acts as a network proxy for one or
more clients. Though its name implies activity, you can almost think of a
service worker as a passive player, one that only runs when one of its
event handlders is fired. It can't even manipulate  its clients' DOMs.

### Clients don't need service workers

If you follow the principles of progressive enhancement, you'll be happy to know 
that clients should function without service workers. This sounds like a 
contradiction, but it's key to the service worker's design. 

First and foremost, it allows for user engagement to occur while the service 
worker is loading and installing. It also allows the page to function on 
browsers that don't support service workers and simplifies adding service 
workers to existing pages. 
