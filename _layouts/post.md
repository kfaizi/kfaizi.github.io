---
layout: wrap
---

<h1 style="margin-bottom:0;">{{ page.title }}</h1>

{% if page.edited != None %}
<p class="post-metadata">published {{ page.date | date: "%Y-%m-%d" }}; edited {{ page.edited }}</p>
{% else %}
<p class="post-metadata">published {{ page.date | date: "%Y-%m-%d" }}</p>
{% endif %}

<div class="post-content">
{{ content }}
</div>


