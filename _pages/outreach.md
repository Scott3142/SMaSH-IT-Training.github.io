---
title: Outreach
layout: subpage
permalink: /outreach/

banner-header: Outreach
banner-text: Community and Educational Projects

intro-header: Activities
intro-text: We, either as a company or as individuals, have been involved in many projects and initiatives in the past, and are always interested in how we can help local schools and communities who may not otherwise have access to high-quality educational resources or opportunities. Working with our partners and in keeping with our philosophy and mission, we offer several <strong>free opportunities</strong> for students. A selection of the events we've been involved in are below.

---

<section id="main" class="wrapper">
  <div class="inner">
    <header class="align-center">
      <h2>{{ page.banner-header }}</h2>
      <p>{{ page.banner-text }}</p>
    </header>

  <!-- Intro -->
    <section>
      <h2>{{ page.intro-header }}</h2>
      <p>{{ page.intro-text }}</p>
    </section>
    <div class="row">
      {% for content in site.data.outreach.events %}
        <section class="6u 12u$(medium) box">
          <h2 class="align-center">{{ content.title }} | <em>{{ content.author }}</em></h2>
          <div class="more">{{ content.text }}</div>
          <p><a href="{{ content.url }}">Find out more...</a></p>
        </section>
      {% endfor %}
    </div>
  </div>
</section>
