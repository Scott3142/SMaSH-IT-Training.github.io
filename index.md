---
title: Home
layout: homepage
permalink: /index.html

banner-header: Training and Development for Computing

banner-content:
  - icon: <span class="icon fa-file-code-o"></span>
    title: One-to-one Training
    description: Tailored training delivered to your needs

  - icon: <span class="icon fa-code-fork"></span>
    title: Group Workshops
    description: Opportunities for team development

  - icon: <span class="icon fa-file-code-o"></span>
    title: Curriculum Support
    description: Advice to get creative with the curriculum

banner-footer: <a href="/courses/" class="button">See available courses...</a>

lower-banner-content:
  - icon: <span class="icon fa-graduation-cap"></span>
    title: Student workshops
    description: Activities for students of all ages

lower-banner-footer: <a href="/courses#student" class="button">Find out more...</a>

about-image: <img src="images/author_small.jpg" alt="Scott Morgan - Company Director" />
about-header: Director
about-description: |
  I am currently finishing up my <strong>Mathematics PhD</strong> and have extensive teaching and training experience in all sectors of education, including <strong>schools, colleges and universities.</strong><br/><br/>

  I am passionate about education and I firmly believe that teaching is one of the world's <strong>most important</strong> professions. I am very interested in <strong>new and innovative teaching methods and practises</strong>, and will do everything I can to ensure all students have access to excellent resources, <strong>regardless of their background</strong>. <br/><br/>

  To read more about our <strong>motivations as a company</strong>, read <strong><a href="/about/">our philosophy</a></strong>.<br/><br/>

  To read more about my <strong>background and experiences</strong>, visit my <strong><a href="http://scott3142.com">personal site</a></strong>.
about-footer:
   - url: http://scott3142.com
     text: Personal Site

   - url: http://scott3142.com/cv/cv.pdf
     text: CV

testimonials-header: Testimonials
---

<!-- Banner -->
  <section id="banner">
    <div class="inner">
      <header>
        <h1>{{ page.banner-header }}</h1>
      </header>

      <div class="flex ">

        {% for content in page.banner-content %}
          <div>
            {{ content.icon }}
            <h3>{{ content.title }}</h3>
            <p>{{ content.description }}</p>
          </div>
        {% endfor %}

      </div>

      <footer>
        {{ page.banner-footer }}
      </footer>

      <br><br>
    </div>

    <div class="inner">
      <div class="flex" style="margin-top:-6%;">
        {% for content in page.lower-banner-content %}
          <div>
            {{ content.icon }}
            <h3>{{ content.title }}</h3>
            <p>{{ content.description }}</p>
          </div>
        {% endfor %}
      </div>

      <footer style="margin-bottom:-6%;">
        {{ page.lower-banner-footer }}
      </footer>
    </div>
  </section>

<!-- Three -->
  <section id="three" class="wrapper align-center">
    <div class="inner">
      <div class="flex flex-2">
        <article>
          <div class="image round">
            {{ page.about-image }}
          </div>
          <header>
            <br/>
            <h3>{{ page.about-header }}</h3>
          </header>
          <p style="padding-left:3%; padding-right:3%;">
            {{ page.about-description }}
          </p>
          <footer>
            {% for link in page.about-footer %}
              <a href="{{ link.url }}" class="button" target="_blank">{{ link.text }}</a>
            {% endfor %}
          </footer>
        </article>

        <article>
          <header>
            <br/>
            <h3>{{ page.testimonials-header }}</h3>
          </header>
          <!-- Blockquote -->
            {% for content in site.data.testimonials %}
              {% if content.homeshow contains "yes" %}
                <h4>{{ content.company }} | {{ content.date }}</h4>
                <blockquote>{{ content.text }}</blockquote>
              {% endif %}
            {% endfor %}
          <footer>
            <a href="/about#testimonials" class="button">See more...</a>
          </footer>
        </article>
      </div>
    </div>
  </section>
