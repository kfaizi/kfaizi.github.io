<!DOCTYPE html>
<html lang="en-US">
    <head>
        <!-- if you're reading this i love you -->
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>{% if page.title %}{{ page.title | append: " - Kian Faizi"}}{% else %}{{ site.title }}{% endif %}</title>
        <meta name="author" content="Kian Faizi">
        <!-- custom css -->
        <link rel="stylesheet" type="text/css" href="/assets/styles.css">
        <!-- load inter font -->
        <link rel="preconnect" href="https://rsms.me/">
        <link rel="stylesheet" href="https://rsms.me/inter/inter.css">
        <!-- and others -->
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link href="https://fonts.googleapis.com/css2?family=Geist+Mono:wght@100..900&display=swap" rel="stylesheet">
        <!-- open graph -->
        <meta name="title" property="og:title" content="{{ page.title }}">
        <meta property="og:type" content="website">
        <meta property="og:url" content="{{ page.url | prepend: site.url }}">
        <!-- twitter cards -->
        <meta name="twitter:site" content="@kianfaizi">
        <meta name="twitter:creator" content="@kianfaizi">
        <meta name="twitter:title" content="{{ page.title }}">
        <!-- descriptions -->
        {% if page.summary %}
        <meta name="description" property="og:description" content="{{ page.summary }}">
        <meta name="twitter:description" content="{{ page.summary }}">
        {% else %}
        <meta name="description" property="og:description" content="{{ site.description }}">
        <meta name="twitter:description" content="{{ site.description }}">
        {% endif %}
        <!-- favicon, etc -->
        <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
        <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
        <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
        <link rel="manifest" href="/site.webmanifest">
        <link rel="mask-icon" href="/safari-pinned-tab.svg" color="#575757">
        <meta name="msapplication-TileColor" content="#2b5797">
        <meta name="theme-color" content="#ffffff">
        <!-- privacy-conscious analytics -->
        <script data-goatcounter="https://kian.goatcounter.com/count" async src="//gc.zgo.at/count.js"></script>
        <!-- mathjax for LaTeX support -->
        {% if page.math %}
        {% include mathjax.html %}
        {% endif %}
    </head>
    <body>
        <div class="centered-box">
            {{ content }}
        </div>
    </body>
</html>
