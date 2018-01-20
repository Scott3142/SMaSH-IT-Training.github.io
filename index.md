---
title: Test
layout: homepage
permalink: /index.html

banner-header: Professional Development and Training

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

banner-foter: <a href="#" class="button">Find out more</a>    

about-image: <img src="images/author_small.jpg" alt="Scott Morgan - Company Director" />
about-header: Director
about-description: |

  I am a <strong>PhD Student in Mathematics</strong>, with <br/> extensive teaching and training experience in <br/> <strong>schools, colleges and universities.</strong><br/><br/>

  I am passionate about <strong>improving science education</strong><br/> and I am particularly interested in mapping<br/> <strong>fun</strong> and <strong>creative</strong> ideas into <strong>existing curricula</strong>.
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

      <a href="/what-we-do/" class="button">See available courses...</a>

      <footer>
        {{ page.banner-footer }}
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
          <p>
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
            <a href="learn-more.html#testimonials" class="button">See more</a>
          </footer>
        </article>
      </div>
    </div>
  </section>
