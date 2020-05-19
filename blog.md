---
title: Blog | Kian Faizi
layout: default
---

<h1> Posts </h1>

<ul class="posts">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}" title="{{ post.title | handleize }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
    </li>
  {% endfor %}
</ul>
