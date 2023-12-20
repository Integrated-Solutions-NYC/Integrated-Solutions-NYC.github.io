---
title: Integrated Solutions
layout: default # home
post_titles:
    - About
    - Services
    # - Stats
    # - Frequently Asked Questions
    # - Welcome
    - Team
navigation:
  - text: About
    link: '#about'
  #- text: Team
  #  link: '#team'
  # - text: FAQ
  #   link: '#faq'
  - text: Services
    link: '#services'
---
{% for title in page.post_titles %}
  {% assign post = site.posts | where: 'title', title | first %}
  {{ post }}
{% endfor %}