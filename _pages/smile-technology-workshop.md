---
title: SMILE Technology Workshop
layout: subpage
permalink: /smile-technology-workshop/
description: Page for the SMILE Technology Workshop. Between January 17th and 20th, I was involved in the long-running SMILE Technology Workshops at Bridgend College. The format of the week was to split Year 5 and 6 children from 4 local primary schools; St. Mary & St. Patrick, Litchard, Croesty and Brynmenyn into several groups and run parallel sessions with interesting technology. 
---

<!-- Main -->
{% for content in site.data.outreach.events %}{% if content.title == page.title %}
  {% include outreach.html %}
{% endif %}{% endfor %}
