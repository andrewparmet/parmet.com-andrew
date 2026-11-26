---
layout: page
title: Blog
permalink: /blog/
description: Writing on software and music by Andrew Parmet.
---

Writing on software and music.

<ul class="posts">
{% for post in site.posts %}
  <li><article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h2>
    <p class="date"><time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: '%B %-d, %Y' }}</time></p>
    <p>{{ post.description | escape }}</p>
  </article></li>
{% endfor %}
</ul>
