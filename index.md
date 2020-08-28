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

{:fancylink: class="front"}

# Hi there! I'm Kian.

![aoraki-headshot](/assets/headshot_web.jpg){: id="headshot"}

I’m a fourth year undergraduate at UC San Diego studying molecular biology, with a minor in applied math. I intend to apply to PhD programs this fall, during the 2020-21 cycle.

### Research interests:

Systems, synthetic, and quantitative biology /
bioinformatics /
genome editing / 
data science.

See my [projects page]{: fancylink} for more information.

I also have a keen interest in environmental conservation, technology/data ethics, and science communication.

Sometimes I write about science, programming, and my thoughts on the world. Check out my most recent posts below, or [view the archive]{: fancylink}:

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
    </li>
  {% endfor %}
</ul>

[projects page]: /projects.html
[view the archive]: /blog.html
