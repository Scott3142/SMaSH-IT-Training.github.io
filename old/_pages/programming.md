---
title: Programming
layout: subpage
permalink: /programming/
description: Course page for programming. This course will enable you and your students to get an insight into a programming language. We offer courses in Python, Scratch, Matlab and Fortran
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
