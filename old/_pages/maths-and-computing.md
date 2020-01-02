---
title: Maths &amp; Computing
layout: subpage
permalink: /maths-and-computing/
description: Course page for maths and computing. Mathematics and computing are inexorably linked through the application of logic and number theory. This course introduces the mathematical principles and theory that underpin the computing curriculum.
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == page.title %}
  {% include courses.html %}
{% endif %}{% endfor %}
