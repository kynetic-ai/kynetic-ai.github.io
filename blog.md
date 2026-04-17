---
layout: page
title: Blog
permalink: /blog/
---

{% for post in site.posts %}
  <article class="post-preview">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</p>
    {% if post.excerpt %}
      <p>{{ post.excerpt | strip_html | truncatewords: 40 }}</p>
    {% endif %}
  </article>
{% endfor %}
