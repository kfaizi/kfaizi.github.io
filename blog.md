---
layout: default
title: Blog
---
<header>
    <nav>
        <ul>
            <li><a href="/">home</a></li>
            <li><a href="/blog.html" class="active">blog</a></li>
            <li><a href="/assets/kian-faizi-cv.pdf">cv</a></li>
        </ul>
    </nav>
</header>

<h1>posts</h1>

<ul class="posts">
    {% for post in site.posts %}
        <li>
        {% if post.external_url %}
            <a href="{{ post.external_url }}">↗ {{ post.title }}</a> (published at {{post.external_host}}) <span id="post-date">({{ post.date | date: "%Y-%m-%d" }})</span>
        {% else %}
            <a href="{{ post.url }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%Y-%m-%d" }})</span>
        {% endif %}    
        </li>
    {% endfor %}
</ul>