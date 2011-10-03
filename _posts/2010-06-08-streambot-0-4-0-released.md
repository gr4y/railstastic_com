--- 
layout: post
title: streambot 0.4.0 released
tags: 
- bot
- gem
- gems
- Gems
- Internal
- Ruby
- streambot
---
The last days I was to busy to write this post, but now I have some free time. Last Saturday I had enough power to release <a href="http://github.com/gr4y/streambot/tree/v0.4.0">streambot 0.4.0</a>. I planned to release it earlier but I was sick and I had no power to work on this project. But back to topic: With streambot 0.4.0 I added oauth for the communication with the twitter api because twitter shuts down the http basic authentication on June 30th. I needed to change the params you pass into the tracker class.

So I encourage you to switch to oauth as soon as possible! But we still need the http basic authentication because the streaming api recently doesn't support oauth and requires the http basic authentication.

Your code needs to look like this:
<script src="http://gist.github.com/430539.js?file=bot.rb"></script>



<strong>rdoc </strong>
From now on the documentation for streambot is available on <a href="http://rdoc.info/projects/gr4y/streambot">rdoc.info</a>

<strong>Future Ideas/Todos</strong>
- a finer grained filtering of tweets.
- removal of http basic auth 

<strong>Bug reports</strong>
If you notice some bugs then don't be shy and file an issue on <a href="http://github.com/gr4y/streambot/issues">github</a>!
