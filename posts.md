---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
title: Posts and Blog by Vince Arter, Jr.
permalink: /posts/
numFeaturedPostsToShow: 5
---
# Posts

## Featured Posts
<ul class="posts">
{% for post in site.tags.featured limit: page.numFeaturedPostsToShow %}
  <div class="post_info">
    <li>
         <a href="{{ post.url }}">{{ post.title }}</a>
         <span>({{ post.date | date:"%Y-%m-%d" }})</span>
    </li>
    </div>
  {% endfor %}
</ul>

## All Posts
<ul class="posts">
{% for post in site.posts %}
  <div class="post_info">
    <li>
         <a href="{{ post.url }}">{{ post.title }}</a>
         <span>({{ post.date | date:"%Y-%m-%d" }})</span>
    </li>
    </div>
  {% endfor %}
</ul>

## Vince's Legacy Medium Blog

<script async src="https://static.medium.com/embed.js"></script><a class="m-profile"
    href="https://medium.com/@VinnieDaArm" data-width="100%">Vince Arter, Jr.</a>
    