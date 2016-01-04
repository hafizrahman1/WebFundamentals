---
layout: shared/narrow
published: false
title: "What do they do?"
description: "Service workers provide web pages with capabilities that make them more like native apps. Here are a list of characteristics and apps or sites that demonstrate their use."
authors:
- josephmedley
published_on: 2015-10-01
updated_on: 2015-10-01
order: 2
---

<p class="intro">
  Service workers provide web pages with capabilities that make them more like 
  native apps. Here are a list of characteristics and apps or sites that 
  demonstrate their use.
</p>

To achieve some of these goals you'll eventually need know more than this primer
provides. Links are provided where appropriate. Fortunately, this primer doesn't
assume you know any of that information.

### Responsiveness

What if you could build a web page that took voice 
recordings? [Voice Memos](https://voice-memos.appspot.com/) by Paul Lewis
does exactly that. For a web-based memo app a slow network would mean slow 
playback. Voice Memos solves this by caching memos on the device. The code is 
[available on GitHub](https://github.com/GoogleChrome/voice-memos). A best 
practice for responsiveness is to use an [application shell architecture](/web/updates/2015/11/app-shell).

### Offline access

The [Guitar Tuner app](https://guitar-tuner.appspot.com/) by Paul Lewis
only needs one interaction with a server. After the first download a 
service worker stores the app's resources so that reopening doesn't require
communicating with a server. The code is also 
[available on GitHub](https://github.com/GoogleChrome/guitar-tuner).


### Engagement

Service workers also allow you to engage users by provideing content outside of
the context of a web page. They do this using [push and notifications](/web/fundamentals/engage-and-retain/push-notifications), 
which are separate API's that allow you to send updates to a service worker and
display messages to a user. Neither feature requires that your web page be open.
The details of this are beyond the scope of this primer. But, you can see it in
action with our [push messaging and notifications](https://github.com/GoogleChrome/samples/tree/gh-pages/push-messaging-and-notifications) 
sample.

{% comment %}https://github.com/google/WebFundamentals/issues/1985{% endcomment %}
