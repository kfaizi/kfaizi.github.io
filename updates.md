---
layout: wrap
title: updates
---

# // updates

<ul>
{% for item in site.data.news %}
  <li>{{ item.date }}: {{ item.text }}</li>
{% endfor %}
</ul>