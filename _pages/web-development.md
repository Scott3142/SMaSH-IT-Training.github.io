---
title: Web Development | Professional Development &amp; Training for Computing &amp; Emerging Technologies 
layout: subpage
permalink: /web-development/
description: Course page for web development. This course introduces several aspects of web design and development, including the underpinning services required to host, manage and access a secure website.
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
