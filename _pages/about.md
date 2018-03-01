---
title: About Us
layout: subpage
permalink: /about/

banner-header: Why We Do This
banner-text: Philosophy and Interests

philosophy-header: Philosophy
philosophy:
  - header: Students First
    text: |
      <p>Students are at the heart of what we do. Professional development for staff does not work without carefully conisdering the needs of each individual learner. A technique that might work for one school or one age group might not work at all for another.

      <br/><br/>

      As part of any staff training we deliver, we offer a <strong>free workshop</strong> for your students. It is critical for us to understand the class needs, and put these at the heart of our delivery.</p>

  - header: Commitment to Open Source
    text: |
      <p>We are commited to transparent, open source resources and everything we create is published under the MIT license. This allows anyone to use, distribute and benefit from our resources.

      <br/><br/>

      Every training resource is available to download from <a href="github.com/scott3142">Github</a> and will remain that way indefinitely.</p>

  - header: Thoughts on Science
    text: |
      <p>We believe that the common subject divides are counter-productive, and endeavour to demonstrate the applicability of computing and mathematics to all science subjects.

      <br/><br/>

      Several of our lesson plans focus on other areas of science in a coherent way, and we welcome enquiries from educators outside of computing.</p>

  - header: Director's Note
    text: |
      <blockquote>I am passionate about education and I firmly believe that teaching is one of the world's most important professions. I am very interested in new and innovative teaching methods and practises, and will do everything I can to ensure all students have access to excellent resources, regardless of their background.

      <br/><br/>

      I am particulary interested in learners from disadvantaged backgrounds, and those who might not necessarily be able to get the help and support they deserve for reasons outside of their control. I welcome any thoughts, advice and comments at any time and I am always looking for ways to improve the design and delivery of these courses. <br/><br/> <strong>Scott Morgan</strong></blockquote>

testimonials-header: Testimonials
---

<!-- Main -->
  <section id="main" class="wrapper">
    <div class="inner">
      <header class="align-center">
        <h2>{{ page.banner-header }}</h2>
        <p>{{ page.banner-text }}</p>
      </header>

    <!-- Intro -->
      <div class="row">
        <section class="6u 12u$(medium)">
          <h2>{{ page.philosophy-header }}</h2>
          {% for content in page.philosophy %}
            <strong>{{ content.header }}</strong><br/><br/>
            {{ content.text }}
          {% endfor %}
          {{ page.philosophy-text }}
        </section>

        <section class="6u 12u$(medium)">
            <img class="image fit" src="/images/si_chemistry.jpg"/>
            <br>
            <img class="image fit" src="/images/pi_workshop.jpg"/>
        </section>
      </div>

      <h2 class="align-center" style="margin-top:5%;">{{ page.testimonials-header }}</h2>
      <div class="row">
        <!-- Blockquote -->
        {% for content in site.data.testimonials %}
          <section class="6u 12u$(medium)">
            <strong>{{ content.company }} | {{ content.date }}</strong><br/><br/>
            <blockquote>{{ content.text }}</blockquote>
          </section>
        {% endfor %}
      </div>

    </div>
  </section>
