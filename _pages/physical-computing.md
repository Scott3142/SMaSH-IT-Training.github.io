---
title: Test
layout: subpage
permalink: /physical-computing/

banner-header: Physical Computing
banner-text: Raspberry Pi, Micro:bit, Arduino, Lego

main-text: Lorem ipsum dolor vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.

details:
  - level: KS2
    text: |
      Lorem ipsum dolor vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.
  - level: KS3
    text: |
      Lorem ipsum dolor vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.
  - level: KS4
    text: |
      Lorem ipsum dolor vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.
  - level: A-Level &amp; BTEC
    text: |
      Lorem ipsum dolor vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan eu faucibus. Integer ac pellentesque praesent.

---

<!-- Main -->
  <section id="main" class="wrapper">
    <div class="inner">
      <header class="align-center">
        <h2>{{ page.banner-header }}</h2>
        <p>{{ page.banner-text }}</p>
      </header>

      <!-- Intro -->
        <section class="6u 12u$(medium)">
          <p>{{ page.main-text }}</p>
          <dl>
            {% for content in page.details %}
              <dt>{{ content.level }}</dt>
              <dd>
                <p>{{ content.text }}</p>
              </dd>
            {% endfor %}
          </dl>
        </section>
    </div>
  </section>
