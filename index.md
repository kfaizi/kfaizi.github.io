---
title: Kian Faizi
layout: default
---
<header>
    <nav>
        <ul>
            <li><a href="/" title="home" class="active">Kian Faizi</a></li>
            <li><a href="/contact.html" title="contact">Contact</a></li>
            <li><a href="/blog.html" title="blog">Blog</a></li>
            <li><a href="/cv.html" title="cv">CV</a></li>
            <li><a href="/projects.html" title="projects">Projects</a></li>
        </ul>
    </nav>
</header>

{:fancylink: class="front"}

# Hi there! I'm Kian.

![headshot](/assets/headshot_web.jpg){: title="aoraki" id="headshot"}

I’m a third year undergraduate at UC San Diego studying molecular biology, with a minor in math (emphasis on statistics). I intend to apply to PhD programs this fall, during the 2020-21 cycle.

<em>**Research interests:** quantitative systems biology, bioinformatics, synthetic biology, genome editing, plant-environment interactions.</em> See my [projects page]{: fancylink} for more information.

I also have a keen interest in issues of environmental conservation, technology/data ethics, and science communication.

[Sometimes I write]{: fancylink} about science, programming, and academia. Check out my most recent posts below:

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}" title="{{ post.title | handleize }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
    </li>
  {% endfor %}
</ul>

[about me]: /about.html "about"
[Sometimes I write]: /blog.html "blog"
[projects page]: /projects.html "projects"
