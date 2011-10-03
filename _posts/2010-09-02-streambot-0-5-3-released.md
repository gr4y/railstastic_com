--- 
layout: post
title: streambot 0.5.3 released
tags: 
- gems
- Gems
- Internal
- Ruby
- streambot
---
Last weekend I released streambot 0.5.0 with the two new features. First the detailed filtering by language of the profile, timezone of the tweeting user or content of the status itself. The second feature is an very simple callback mechanism, which allows you to do implement own processing of status.

A day later I found a bug in filtering which broke it completely and released version 0.5.1 with the fix of that issue. 

Today I noticed on my development machine that Twitter removed the http basic authentication for the rest API, so I removed the http class and released version 0.5.2, which again was not working because of my stupidity. So I finally released version 0.5.3.

The documentation and an example how to implement the callback methods is available on <a href="http://rubydoc.info/github/gr4y/streambot/master/frames">rubydoc.info</a>
