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

### Responsiveness

What if you could build a web page that took voice 
recordings? [Voice Memos](https://voice-memos.appspot.com/) by Paul Lewis
does exactly that. For a web-based memo app a slow network would mean slow 
playback. Voice Memos solves this by caching memos on the device. The code is 
[available on GitHub](https://github.com/GoogleChrome/voice-memos).

### Offline access

The [Guitar Tuner app](https://guitar-tuner.appspot.com/) by Paul Lewis
only needs one interaction with a server. After the first download a 
service worker stores the app's resources so that reopening doesn't require
communicating with a server. The code is also [available on GitHub](https://github.com/GoogleChrome/guitar-tuner).


### Engagement

{% comment %}https://github.com/google/WebFundamentals/issues/1985{% endcomment %}
