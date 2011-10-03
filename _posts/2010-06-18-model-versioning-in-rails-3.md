--- 
layout: post
title: Model Versioning in Rails 3
tags: 
- activerecord
- Gems
- Model
- model versioning
- rails
- rails 3
- Ruby
---
Some months ago I saw the <a href="http://railscasts.com/episodes/177-model-versioning">Episode #177 of railscasts</a> about Model Versioning. Two weeks ago I started to build an own wiki application. So I watched this episode again and started to add it to my wiki application. The vestal_versions gem worked properly, but after upgrading to rails 3 beta 4 it stopped working. The issue is already <a href="http://github.com/laserlemon/vestal_versions/issues#issue/34">filed</a> so I thought I should try fixing it, but I don't got it working. 

Today I discovered paper_trail on github and added it to my application. And woooohooo: It worked and it just needs a migration file in your application. No initializer like in vestal_versions. If you are searching for an nice and small solution for model versioning in rails 3, then you should take a look at <a href="http://github.com/airblade/paper_trail">airblades's paper_trail</a>
