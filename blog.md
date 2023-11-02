---
layout: default
title: blog
---
{% include header.html %}

<h1>posts</h1>

<ul class="posts">
    {% for post in site.posts %}
        <li>
        {% if post.external_url %}
            <a href="{{ post.external_url }}">↗ {{ post.title }}</a>, <span id="post-metadata">published by <i>{{post.external_host}}</i> on</span> <span id="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
        {% else %}
            <a href="{{ post.url }}">{{ post.title }}</a>, <span id="post-metadata">published on</span> <span id="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
        {% endif %}    
        </li>
    {% endfor %}
</ul>