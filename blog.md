---
title: Blog | Kian Faizi
layout: default
---
<header>
    <nav>
        <ul>
            <li><a href="/" title="home">Kian Faizi</a></li>
            <li><a href="/contact.html" title="contact">Contact</a></li>
            <li><a href="/blog.html" title="blog" class="active">Blog</a></li>
            <li><a href="/cv.html" title="cv">CV</a></li>
            <li><a href="/projects.html" title="projects">Projects</a></li>
        </ul>
    </nav>
</header>

<h1> Posts </h1>

<ul class="posts">
    {% for post in site.posts %}
        <li>
            <a href="{{ post.url }}" title="{{ post.title | handleize }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
        </li>
    {% endfor %}
</ul>
