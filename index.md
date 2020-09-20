---
title: Kian Faizi
layout: default
---
<header>
    <nav>
        <ul>
            <li><a href="/" class="active">Kian Faizi</a></li>
            <li><a href="/contact.html">Contact</a></li>
            <li><a href="/blog.html">Blog</a></li>
            <li><a href="/cv.html">CV</a></li>
            <li><a href="/projects.html">Projects</a></li>
        </ul>
    </nav>
</header>

# Hi there! I'm Kian.

![aoraki-headshot](/assets/headshot_web.jpg){: id="headshot"}

I’m a final year undergraduate at UC San Diego studying molecular biology and math. **I'm currently applying to PhD programs!**

### Research interests:
<pre>
synthetic biology / the non-coding genome / cellular models /
network interactions and dynamical systems / climate change.
</pre>
Sometimes I write about science, programming, and my thoughts on the world.  Check out my most recent posts below, or [view the archive]:

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
    </li>
  {% endfor %}
</ul>

[projects page]: /projects.html
[view the archive]: /blog.html
