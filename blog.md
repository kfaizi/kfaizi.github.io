---
layout: default
title: Blog
---
<header>
    <nav>
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/blog.html" class="active">Blog</a></li>
            <li><a href="/assets/kian-faizi-cv.pdf">CV</a></li>
        </ul>
    </nav>
</header>

<h1> Posts </h1>

<ul class="posts">
    {% for post in site.posts %}
        <li>
        {% if post.external_url %}
            <a href="{{ post.external_url }}">{{ post.title }} ↗</a> (published at {{post.external_host}}) <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
        {% else %}
            <a href="{{ post.url }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
        {% endif %}    
        </li>
    {% endfor %}
</ul>