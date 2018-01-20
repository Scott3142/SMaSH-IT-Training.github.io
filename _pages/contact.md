---
title: Test
layout: subpage
permalink: /contact/

banner-header: Contact Us
---

<section id="main" class="wrapper">
  <div class="inner">
    <header class="align-center">
      <h2>{{ page.banner-header }}</h2>
    </header>

    {% for content in site.data.contact %}
      <p>{{ content.title }} : <a href="{{ content.url }}" target="_blank">{{ content.text }}</a></p>
    {% endfor %}
  </div>
</section>
