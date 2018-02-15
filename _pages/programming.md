---
title: Programming
layout: subpage
permalink: /programming/
---

<!-- Main -->
{% for course in site.data.courses %}{% if course.banner-title == "Physical Computing" %}
  <section id="main" class="wrapper">
    <div class="inner">
      <header class="align-center">
        <h2>{{ course.banner-title }}</h2>
        <p>{{ course.banner-text }}</p>
      </header>

      <!-- Intro -->
        <div class="row">
          <section class="6u 12u$(medium)">
            <p>{{ course.main-text }}</p>
            <dl>
              <div class="row">
                {% for content in course.details %}
                    <div class="box" style="margin-left:2%;">
                      <dt>{{ content.level }}</dt>
                      <p class="more">{{ content.text }}</p>
                    </div>
                {% endfor %}
              </div>
            </dl>
          </section>
        </div>
    </div>
  </section>
{% endif %}{% endfor %}
