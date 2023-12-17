---
title: Integrated Solutions
layout: default
post_titles:
    - Top Slider
    - About
    - Services
    - Stats
    - Frequently Asked Questions
    - Welcome
    - Team
---

{% for title in page.post_titles %}
  {% assign post = site.posts | where: 'title', title | first %}
  <!-- <h2>{{ post.title }}</h2> -->
  {{ post.content }}
{% endfor %}