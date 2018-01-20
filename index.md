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
    description: Advice on getting creative with the curriculum

banner-foter: <a href="#" class="button">Find out more</a>    
---

<!-- Banner -->
  <section id="banner">
    <div class="inner">
      <header>
        <h1>{% page.banner-header %}</h1>
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
    </div>
  </section>


<!-- Three -->
  <section id="three" class="wrapper align-center">
    <div class="inner">
      <div class="flex flex-2">
        <article>
          <div class="image round">
            <img src="images/author_small.jpg" alt="Pic 01" />
          </div>
          <header>
            <br />
            <h3>Director</h3>
          </header>
          <p>
            I am a <strong>PhD Student in Mathematics</strong>, with <br/> extensive teaching and training experience in <br/> <strong>schools, colleges and universities.</strong><br /><br />

            I am passionate about <strong>improving science education</strong><br/> and I am particularly interested in mapping<br/> <strong>fun</strong> and <strong>creative</strong> ideas into <strong>existing curricula</strong>.
          </p>
          <footer>
            <a href="http://scott3142.com" class="button">Personal Site</a>
            <a href="http://scott3142.com/cv/cv.pdf" class="button">CV</a>
          </footer>
        </article>
        <article>
          <header>
            <br />
            <h3>Testimonials</h3>
          </header>
          <!-- Blockquote -->
            <h4>Bridgend College</h4>
            <blockquote>Fringilla nisl. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan faucibus. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis.</blockquote>
            <h3>Croesty Primary School</h3>
            <blockquote>Fringilla nisl. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan faucibus. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis.</blockquote>
            <h3>Olveston Primary School</h3>
            <blockquote>Fringilla nisl. Donec accumsan interdum nisi, quis tincidunt felis sagittis eget tempus euismod. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis iaculis volutpat ac adipiscing accumsan faucibus. Vestibulum ante ipsum primis in faucibus vestibulum. Blandit adipiscing eu felis.</blockquote>
          <footer>
            <a href="learn-more.html#testimonials" class="button">See more</a>
          </footer>
        </article>
      </div>
    </div>
  </section>
