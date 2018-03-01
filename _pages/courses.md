---
title: Courses
layout: subpage
permalink: /courses/

banner-header: What We Do
banner-text: Training Courses and CPD

intro-header: Courses
intro-text: Our courses are flexible and tailored to your needs, but for guidance we have provided some example ideas below. The availability of each course in terms of appropriate level is listed inside the course description.
---

<!-- Main -->
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

      {% for course in site.data.courses %}
        <section class="3u 6u(medium) 12u$(small)">
          <a href="{{ course.link }}"><h3 class="button special fit">{{ course.banner-title }}</h3></a>
          <div class="box">
            <p class="more">{{ course.main-text }}</p>
            <a href="{{ course.link }}">Find out more...</a>
          </div>
        </section>
      {% endfor %}

    </div>

  </div>
</section>
