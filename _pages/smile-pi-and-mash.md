---
title: SMILE Pi &amp; Mash
layout: subpage
permalink: /smile-pi-and-mash/
---

<!-- Main -->
{% for content in site.data.outreach.events %}{% if content.title == page.title %}
  {% include outreach.html %}
{% endif %}{% endfor %}
