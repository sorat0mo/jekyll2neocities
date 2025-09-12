---
title: Blog
layout: default
permalink: /blog
---
{% if site.blog_as_home %}
<meta http-equiv="refresh" content="0; url={{ site.url }}{{ site.baseurl }}">
{% else %}
{% include blog.html %}
{% endif %}
