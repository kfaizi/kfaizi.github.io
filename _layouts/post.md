---
layout: default
---
<header>
    <nav>
        <ul>
            <li><a href="/">Kian Faizi</a></li>
            <li><a href="/contact.html">Contact</a></li>
            <li><a href="/blog.html" class="active">Blog</a></li>
            <li><a href="/cv.html">CV</a></li>
            <li><a href="/projects.html">Projects</a></li>
        </ul>
    </nav>
</header>

<h1>{{ page.title }}</h1>

<p id="post-metadata">Published {{ page.date | date:"%B %-d, %Y" }}. <a href="/blog.html">Back to posts</a></p>

{{ content }}


