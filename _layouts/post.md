---
layout: default
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

<h1>{{ page.title }}</h1>

<p id="post-metadata">published {{ page.date | date:"%B %-d, %Y" }}. <a href="/blog.html">back to posts</a></p>

{{ content }}


