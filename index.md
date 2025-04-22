---
title: Integrated Solutions
layout: default #home # default # home
page_titles:
    - About
    - Services
#    - Stats
    - Frequently Asked Questions
#    - Welcome
    - Team
navigation:
  - text: About
    link: '#about'
  - text: Team
    link: '#team'
  - text: FAQ
    link: '#faq'
  - text: Services
    link: '#services'
  - text: Quick Links
    dropdown:
    - text: Buy Time
      link: 'https://link.waveapps.com/rn8j9w-jh4qyj'
    - text: Buy PBX Onboarding
      link: 'https://link.waveapps.com/5uv7c7-yftq6g'
    - text: Buy Domain Name, eMail, and Website
      link: 'https://sdxdomains.com'

---
{% for title in page.page_titles %}
  {% assign post = site.pages | where: 'title', title | first %}
  {{ post }}
{% endfor %}
