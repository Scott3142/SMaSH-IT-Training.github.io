---
title: Physical Computing
layout: subpage
permalink: /physical-computing/
description: Course page for physical computing. This course will enable you and your students to get hands-on with computing. Using affordable emerging technologies such as the Raspberry Pi, BBC Micro:bit, Lego EV3 and Arduino, we offer training and curriculum support for all aspects of physical computing across all key stages.
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
