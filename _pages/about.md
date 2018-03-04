---
title: About Us
layout: subpage
permalink: /about/

banner-header: Why We Do This
banner-text: Philosophy and Interests

philosophy-header: Philosophy
philosophy-row1:
  - header: Students First
    text: |
      <p>Students are at the heart of what we do. Professional development for staff does not work without carefully considering the needs of each individual learner. A technique that might work for one school or one age group might not work at all for another.

      <br/><br/>

      As part of any staff training we deliver, we offer a <strong>free workshop</strong> for your students. It is critical for us to understand the class needs, and put these at the heart of our delivery.</p>

      <span class="image fit"><img src="/images/pi_workshop.jpg"/></span>

  - header: Thoughts on Science
    text: |
      <p>We believe that the common subject divides are counter-productive, and endeavour to demonstrate the applicability of computing and mathematics to all science subjects.

      <br/><br/>

      Traditionally, when we think about ‘science’, we think of labs, dissections, experiments; biology, chemistry and physics and often miss the the other letters in STEAM. In reality, mathematics, computing and digital competency are central to science, and teaching science subjects in isolation can often be counter-productive. If we artificially pigeon-hole the subjects, and erect walls around our disciplines, do we stifle innovation, creativity and critical thinking? <br><br>

      We believe that it is increasingly important to equip the new generation in this Information Age with the necessary skills to thrive in a world where automation is growing, and talk of jobs being replaced by robots is common in mainstream media. We are keen to develop transferable skills through the sciences, enabling students to stay ahead of the automation curve, and shifting curricula from ​using ​towards ​developing technologies.

      Several of our lesson plans focus on all areas of science, and we welcome enquiries from educators outside of computing.</p>

      <span class="image fit" style="margin-top:6%;"><img src="/images/steam.png"/></span>

philosophy-row2:
  - header: Widening Access
    text: |
      <p>The fact that the income of a student's parents is still a deciding factor in that student's progression to higher education is shocking. We are passionate about closing this attainment gap, and work with students and schools from all socio-economic areas and backgrounds.

      <br/><br/>

      </p>

  - header: Commitment to Open Source
    text: |
      <p>We are committed to transparent, open source resources and everything we create is published under the MIT license. This allows anyone to use, distribute and benefit from our resources.

      <br/><br/>

      Every training resource is available to download from <a href="https://github.com/SMaSH-IT-Training/" target="_blank">GitHub</a> and will remain that way indefinitely.</p>

director:
  header: Director's Note
  text: |
    <blockquote>I am passionate about education and I firmly believe that teaching is one of the world's most important professions. I am very interested in new and innovative teaching methods and practises, and will do everything I can to ensure all students have access to excellent resources, regardless of their background.

    <br/><br/>

    I am particularly interested in learners from disadvantaged backgrounds, and those who might not necessarily be able to get the help and support they deserve for reasons outside of their control. I welcome any thoughts, advice and comments at any time and I am always looking for ways to improve the design and delivery of these courses. <br/><br/> <strong>Scott Morgan</strong></blockquote>

testimonials-header: Testimonials

partners-header: Partners

partners:
  - image: <div class="3u"><span class="image fit"><img src="/images/bcoll.png"/></span></div>
    text:  <h2 class="align-center">Bridgend College</h2>
  - image: <div class="1u"><span class="image fit"><img src="/images/culogo.png"/></span></div>
  - image: <div class="1u"><span class="image fit"><img src="/images/picademy.png"/></span></div>
  - image: <div class="1u"><span class="image fit"><img src="/images/siamlogo.png"/></span></div><br>
  - image: <div class="1u"><span class="image fit"><img src="/images/ima_logo.png"/></span></div>
  - image: <div class="1u"><span class="image fit"><img src="/images/emotion.jpg"/></span></div>
  - image: <div class="1u"><span class="image fit"><img src="/images/stem.jpg"/></span></div>

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
        {% for content in page.philosophy-row1 %}
          <section class="6u 12u$(medium) box">
            <h2 class="align-center">{{ content.header }}</h2>
            {{ content.text }}
          </section>
        {% endfor %}
      </div>
      <div class="row">
        {% for content in page.philosophy-row2 %}
          <section class="6u 12u$(medium) box">
            <h2 class="align-center">{{ content.header }}</h2>
            {{ content.text }}
          </section>
        {% endfor %}
      </div>

      <h2 class="align-center" style="margin-top:5%;">{{ page.director.header }}</h2>
      {{ page.director.text }}

      <h2 class="align-center" style="margin-top:5%;">{{ page.testimonials-header }}</h2>
      <div class="row">
        <!-- Blockquote -->
        {% for content in site.data.testimonials %}
          {% if content.fullshow contains "yes" %}
            <section class="6u 12u$(medium)"><a name="testimonials"></a>
              <strong>{{ content.company }} | {{ content.date }}</strong><br/><br/>
              <blockquote>{{ content.text }}</blockquote>
            </section>
          {% endif %}
        {% endfor %}
      </div>

      <!--<h2 class="align-center" style="margin-top:5%;">{{ page.partners-header }}</h2><br>
      <div class="row">
        {% for content in page.partners %}
          <section class="6u 12u$(medium) box">
            {{ content.text }}
          </section>
          <section class="6u 12u$(medium) box">
            {{ content.image }}
          </section>
        {% endfor %}
      </div>-->

    </div>
  </section>
