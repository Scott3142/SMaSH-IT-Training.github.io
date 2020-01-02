---
title: Software Development
layout: subpage
permalink: /software-development/
description: Course page for software development. This course will introduce the concept of open-source, and other commonly used licensing and copyright practises. 
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
