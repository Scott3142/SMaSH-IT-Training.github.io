---
title: SMILE Pi &amp; Mash
layout: subpage
permalink: /smile-pi-and-mash/
description: Page for SMILE Pi and Mash. The Pi and Mash event was the follow up to the SMILE Technology Workshops and featured Year 5 and 6 children from 4 local primary schools - St. Mary & St. Patrick, Litchard, Croesty and Brynmenyn. 
---

<!-- Main -->
{% for content in site.data.outreach.events %}{% if content.title == page.title %}
  {% include outreach.html %}
{% endif %}{% endfor %}
