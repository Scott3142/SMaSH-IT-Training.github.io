---
title: Maths &amp; Computing
layout: subpage
permalink: /maths-and-computing/
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
