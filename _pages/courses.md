---
title: Courses
layout: subpage
permalink: /courses/
description: Page for description of teacher training and development courses offered by SMaSH-IT Training in the Cardiff, Bridgend and South Wales regions.

banner-header: What We Do
banner-text: Training Courses and CPD

intro-header: Courses
intro-text: Our courses are flexible and tailored to your needs, but for guidance we have provided some example ideas below. The availability of each course in terms of appropriate level is listed inside the course description.

second-header: Student Workshops
second-text: As part of any course you book with us, we offer a <strong>free</strong> workshop to your students. All of the above courses are available in a workshop version which we will deliver directly to your class. <br><br> Alternatively, we offer a standalone package if you would just like a workshop or demonstration without a course. If you are interested, please <strong><a href="/contact/">get in touch</a></strong>!
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
            {% if course.show != 0 %}
              <a href="{{ course.link }}">Find out more...</a>
            {% endif %}
          </div>
        </section>
      {% endfor %}

    </div><br>

    <section><a name="student"></a>
      <h2>{{ page.second-header }}</h2>
      <p>{{ page.second-text }}</p>
    </section>

  </div>
</section>
