--- 
layout: post
title: final streambot 1.0.0 released
tags: 
- Gems
- Ruby
- streambot
---
Last Sunday, I finally released the version 1.0.0 of streambot. But since then I had no time to announce it here, but now my weekend has officially started and I have some minutes to drop a notice. ;-)

So, the new streambot release is a huge milestone for me. When I look back at the 0.5 releases, I have the desire to bash my head against a wall. Now it has working filters and an nice callback / eventing mechanism.

If you are upgrading from an earlier version of streambot I highly encourage you to read the <a href="https://github.com/gr4y/streambot/blob/master/README.rdoc">README</a>, cause there is an elementary change in passing the params into the tracker. Instead of passing four arguments like it was back in 0.5 and previous versions, you now pass one hash into the tracker.

Maybe there are some problems with the threading of ruby running on an ubuntu machine. More about this in another post.

(I should write more posts here, mh?)
