---
title: Mobile App Development
layout: subpage
permalink: /mobile-apps/
description: Course page for Android mobile app development. This course investigates the characteristics and uses of mobile apps, enabling you to learn how mobile apps are developed.
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
