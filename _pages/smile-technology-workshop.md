---
title: SMILE Technology Workshop
layout: subpage
permalink: /smile-technology-workshop.html
---

<!-- Main -->
{% for content in site.data.outreach.events %}{% if content.title == page.title %}
  {% include outreach.html %}
{% endif %}{% endfor %}
