--- 
layout: post
title: "snippet: action specific link rendering"
tags: 
- action
- dry
- Helper
- link
- rails
- render
- Ruby
- Snippet
- view
---
<strong>Update on 06/05/10</strong>
Today I noticed the ActionView::UrlHelper method <strong><a href="http://api.rubyonrails.org/classes/ActionView/Helpers/UrlHelper.html#M002144">link_to_unless_current</a></strong>. It is very similar to my snippet below, but as documented in the rdoc, it renders the specified link text but not the link when the the current request URI is the same as the one it links to.
<p style="text-align: center;">---------------------------------------------------------------------------------------------------------------------------</p>
Renders a link in the specified action/actions. I needed it in an partial because I DRYed up my views a little bit.

<script src="http://gist.github.com/395373.js"></script>
