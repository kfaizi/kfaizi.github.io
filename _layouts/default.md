<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>{{ page.title }}</title>
    <link rel="stylesheet" type="text/css" href="/assets/styles.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,700;1,400;1,700&display=swap">
    <meta name="author" content="Kian Faizi">
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
  </head>
  <body>
    <div id="wrap">
      {{ content }}
      {% include footer.html %}
    </div>
  </body>
</html>
