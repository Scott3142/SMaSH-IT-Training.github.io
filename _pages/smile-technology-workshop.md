---
title: SMILE Technology Workshop
layout: subpage
permalink: /smile-technology-workshop/
---

<!-- Main -->
{% for content in site.data.outreach.events %}{% if content.title == page.title %}
  {% include outreach.html %}
{% endif %}{% endfor %}
