---
title: Integrated Solutions
layout: home
post_titles:
    - About
    - Services
    - Stats
    - Frequently Asked Questions
    - Welcome
    - Team
---
{% for title in page.post_titles %}
  {% assign post = site.posts | where: 'title', title | first %}
  {% include post.layout %}
  {{ post.content }}
{% endfor %}