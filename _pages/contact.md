---
title: Contact Us
layout: contact
permalink: /contact/

banner-header: Contact Details
---

<section id="main" class="wrapper">
  <div class="inner">
    <header class="align-center">
      <h2>{{ page.banner-header }}</h2>
    </header>

    <div class="row">
    {% for content in site.data.contact %}
      <p style="margin-left:1.25%;"><a class="button small" href="{{ content.url }}" target="_blank">{{ content.title }} : {{ content.text }}</a></p>
    {% endfor %}</div>
  </div>
</section>