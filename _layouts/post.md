---
layout: default
---
{% include header.html %}

<h1>{{ page.title }}</h1>

<p id="post-metadata">published {{ page.date | date:"%B %-d, %Y" }}. <a href="/blog.html">back to posts</a></p>

{{ content }}


