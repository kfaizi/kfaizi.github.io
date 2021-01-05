---
layout: default
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

<h1>{{ page.title }}</h1>

<p id="post-metadata">Published {{ page.date | date:"%B %-d, %Y" }}. <a href="/blog.html">Back to posts</a></p>

{{ content }}


