---
title: Blog | Kian Faizi
layout: default
---
<header>
    <nav>
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/blog.html" class="active">Blog</a></li>
            <li><a href="/cv.html">CV</a></li>
        </ul>
    </nav>
</header>

<h1> Posts </h1>

<ul class="posts">
    {% for post in site.posts %}
        <li>
            <a href="{{ post.url }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
        </li>
    {% endfor %}
</ul>
