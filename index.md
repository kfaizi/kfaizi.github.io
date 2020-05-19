---
title: Kian Faizi
layout: home
---
{:fancylink: class="front"}
{:tbd: class="under-construction"}

# Hi there! I'm Kian.

I’m a third year undergraduate at UC San Diego studying molecular biology, with a minor in math (emphasis on statistics). I intend to apply to PhD programs during the 2020-21 cycle. More [about me]{: fancylink}.

**Research interests:** quantitative systems biology, bioinformatics, synthetic biology, genome editing. I currently work in a plant genetics lab, where we're interested in how roots sense and respond to environmental stimuli. For more on my work so far, see [my projects]{: tbd}.

Part of this site is a blog — mostly on science, programming, and academia. Check out my most recent posts below, or view the archive of [all my writing]{: fancylink}:

<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}" title="{{ post.title | handleize }}">{{ post.title }}</a> <span id="post-date">({{ post.date | date: "%-m/%-d/%y" }})</span>
    </li>
  {% endfor %}
</ul>

[about me]: /about.html "about"
[all my writing]: /blog.html "blog"
[my projects]: /projects.html "projects"
