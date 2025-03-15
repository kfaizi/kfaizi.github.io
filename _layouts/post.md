---
layout: wrap
---

<h1>{{ page.title }}</h1>

{% if page.edited != None %}
<p class="post-metadata">published {{ page.date | date: "%Y-%m-%d" }}; edited {{ page.edited }}. <a href="/writing.html">back to posts</a></p>
{% else %}
<p class="post-metadata">published {{ page.date | date: "%Y-%m-%d" }}. <a href="/writing.html">back to posts</a></p>
{% endif %}

<div class="post-content">
{{ content }}
</div>


