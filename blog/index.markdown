---
layout: page
title: Blog
permalink: /blog/
---

<p>All posts from kynetic intelligence.</p>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%B %-d, %Y" }}</span>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
