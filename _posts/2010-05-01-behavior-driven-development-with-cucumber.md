--- 
layout: post
title: behavior driven development with cucumber
tags: 
- bdd
- behavior driven development
- cucumber
- rails
- Ruby
- testing
---
The last weeks I had no time for rails. But I released some minor patches for <a href="http://rubygems.org/gems/streambot">streambot</a>. So I started to playing with rails . Actually I discovered <a href="http://www.cukes.info">cucumber</a>. Ryan Bates from railscasts.com published a nice screencast about <a href="http://railscasts.com/episodes/155-beginning-with-cucumber">beginning with cucumber</a>.

Actually I am running ubuntu linux and it seems there happend some changes in the last few months on this gem. Actually you need to define <strong>cucumber-rails</strong> instead of <strong>cucumber</strong> in your <strong>environments/test.rb</strong>. And then you should follow the steps from Ryans screencast.

So lets take a look on my example:
<script src="http://gist.github.com/386465.js"></script>
