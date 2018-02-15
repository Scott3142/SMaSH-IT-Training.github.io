---
title: Physical Computing
layout: subpage
permalink: /physical-computing/
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
