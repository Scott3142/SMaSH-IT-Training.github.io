---
title: Full STEAM Ahead
layout: subpage
permalink: /full-steam-ahead/
description: Page for the Full STEAM Ahead event. On June 28th 2017, I was involved in the Cardiff SIAM-IMA Student Chapter ‘Full STEAM Ahead’ event, open to secondary school and FE College students, PhD students and staff. The event consisted of three workshops aimed at inspiring students to engage in STEM subjects.
---

<!-- Main -->
{% for content in site.data.outreach.events %}{% if content.title == page.title %}
  {% include outreach.html %}
{% endif %}{% endfor %}
