---
layout: wrap
title: updates
---

# Updates

<ul>
{% for item in site.data.news %}
  <li>{{ item.date }}: {{ item.text }}</li>
{% endfor %}
</ul>