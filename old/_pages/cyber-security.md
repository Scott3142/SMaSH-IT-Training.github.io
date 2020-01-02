---
title: Cyber Security (Beta)
layout: subpage
permalink: /cyber-security/
description: Course page for cyber security. Currently in beta, this course explores some basic ideas about cyber security, including the mathematics of RSA encryption and some common hacking techniques.
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
