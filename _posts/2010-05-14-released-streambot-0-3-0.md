--- 
layout: post
title: released streambot 0.3.0
tags: 
- Internal
- streambot
---
Yesterday I released <a href="http://github.com/gr4y/streambot/tree/v0.3.0">version 0.3.0 of streambot</a>. It is also available on <a href="http://rubygems.org/gems/streambot">rubygems.org</a>. If you want to contribute, then just fork the project, add your changes and send me a pull request. 

I think it is time to explain it a little bit and show you a little example. So, streambot is a gem for ruby that provides a retweet bot. I completely rewrote my retweet bot and published it to github. The philosophy is: keep it simple.

I started an twitter-account with the idea to retweet all tweets that are related to the local public transport in leipzig. <a href="http://twitter.com/oepnv_leipzig">@oepnv_leipzig</a> is the account where it is running on. So here is my script:
<script src="http://gist.github.com/401046.js"></script>

My server is running the whole day and everytime I reboot the system I need to run the script again. Actually I am searching for an init.d-script to start it when the server is started. If you have some tipps then please drop a comment below this article! Thanks!
