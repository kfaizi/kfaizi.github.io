---
layout: default
---


<div style="width: 100%; margin: auto; overflow: hidden;">

<h1 style="text-align: center">Kian Faizi</h1>

<a  href="/assets/images/headshot.jpg">
<img src="/assets/images/headshot-square.jpg" height="250em" id="headshot">
</a>

<p>
I'm a PhD student at <span style="color: #FF6C0C">Caltech</span> with <a href="http://www.rpgroup.caltech.edu/">Rob Phillips</a>, where I think about how matter and energy move through biological systems, from the molecular to the planetary scale.
</p>

<p>
I like being outside. You can find me in the <span style="color: #005838">Angeles National Forest</span>, where I sometimes volunteer as a <a href="http://nhlr.org/lookouts/us/ca/vetter-mountain-lookout">fire lookout</a> and trail maintainer.
</p>

<p>
Major prior iterations of me have been an inaugural <a href="https://www.newscience.org">New Science</a> fellow at Harvard, a lab tech at the Salk Institute, an undergrad at UCSD, a high school student in Malaysia, and a gastrulating embryo in San Diego.
</p>

</div>

<b>// updates</b> 
<div class="newsbox">
<ul>
{% for item in site.data.news limit:4 %}
  <li>{{ item.date }}: {{ item.text }}</li>
{% endfor %}
  <li>[<a href="/updates.html">+ {{ site.data.news.size | minus:4 }} more</a>]</li>
</ul>

</div>

<hr>

<p id="linkbar">
[internal:
    <a href="/contact.html">say hi!</a> / 
    <a href="/listlist.html">list-of-lists</a> /
    <a href="/writing.html">writing</a>]
[external:
    <a href="https://twitter.com/kianfaizi">twitter</a> /
    <a href="https://scholar.google.com/citations?user=frNmiZkAAAAJ&hl=en">scholar</a> /
    <a href="https://github.com/kfaizi">github</a>]
[files:
    <a href="/assets/images/headshot.jpg">headshot.jpg</a> /
    <a href="/assets/kian_faizi_resume.pdf">resume.pdf</a>]
</p>
