---
title: Web Development
layout: subpage
permalink: /web-development/
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
