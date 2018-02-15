---
title: Computing for Mathematics
layout: subpage
permalink: /computing-for-mathematics/
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
