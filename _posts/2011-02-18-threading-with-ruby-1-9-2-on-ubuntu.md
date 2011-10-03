--- 
layout: post
title: threading with ruby 1.9.2 on ubuntu
tags: 
- Gems
- issues
- mac
- Ruby
- ruby 1.9.2
- snow leopard
- streambot
- threading
- threads
- Ubuntu
---
Since October I am developing on an mac with OS X Snow Leopard instead of my old notebook with Ubuntu. While the release candidate phase I was testing the streambot gem on my ubuntu server.

The Tracker was starting and stopping immediately on the server, but on the mac all was working as I expected it. After fixing this issues with some calling of the join method on the thread it worked on Ubuntu, but actually after one hour the running thread is dead, but there is no Exception either.

I had no time this week to take a look into this weird issue, but I promise that I will look into it this weekend. I even installed ubuntu and rvm on the old notebook for better testing of my gems.
