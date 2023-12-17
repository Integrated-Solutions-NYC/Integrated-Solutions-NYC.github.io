---
title: About
layout: default
---

{% assign about = site.posts | where: 'title', 'About' | first %}
{{ about.content }}