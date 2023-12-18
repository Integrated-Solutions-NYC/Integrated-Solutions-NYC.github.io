---
title: Integrated Solutions
layout: knight
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
  {{ post.content }}
{% endfor %}