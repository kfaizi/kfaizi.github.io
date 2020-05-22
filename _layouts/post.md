---
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

<h1>{{ page.title }}</h1>

<p id="post-metadata">Published {{ page.date | date:"%B %-d, %Y" }}. <a href="/blog.html" title="blog">Back to posts</a></p>

{{ content }}


