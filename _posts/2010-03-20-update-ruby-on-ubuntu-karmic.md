--- 
layout: post
title: update ruby on ubuntu karmic
tags: 
- compile
- gems
- karmic
- Ruby
- rubygems
- Ubuntu
- update
---
On Ubuntu Karmic aka Ubuntu 9.10 by default ruby is an ruby 1.8.7 and a little old in my opinion. In my environment some gems doesn't work properly, so I switched to ruby 1.9 and now I want to show you how I updated ruby. I admit it is the sledgehammer method but i wanted to suppress disturbing side-effects! ;-)

First I removed all ruby 1.8 packages with apt-get

<pre>sudo apt-get purge ruby1.8* rubygems1.8</pre>

<strong><em>!!! Be careful at this point !!!</em></strong><em>
On my environment I had <strong>texlive</strong> installed and it depends on ruby1.8, but I don't needed it so I removed it with:</em>

<pre>sudo apt-get autoremove</pre>

I created a directory for compiling stuff like ruby

<pre>mkdir ~/src; cd ~/src</pre>

Now I downloaded the latest stable package of ruby 1.9 and extracted it

<pre> wget ftp://ftp.ruby-lang.org/pub/ruby/ruby-1.9-stable.tar.gz; tar xzfv ruby-1.9-stable.tar.gz</pre>

Change into the extracted directory. I my case it was <strong>ruby-1.9.1-p378</strong>. Then I ran the configure script and compiled it all with make.

<pre>cd ruby-1.9*; ./configure --prefix=/usr/local; sudo make &amp;&amp; sudo make install</pre>

I checked the version of ruby:

<pre>ruby -v
ruby 1.9.1p378 (2010-01-10 revision 26273) [x86_64-linux]</pre>

Finally I updated all my system gems with:

<pre>sudo gem update --system</pre>

and installed rails, rake and mysql with

<pre>sudo gem install rails rake mysql</pre>

And then I was ready to go!
