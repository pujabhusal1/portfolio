---
layout: default
title: Puja Bhusal | Portfolio
---

<section class="hero">
  <img src="{{ '/assets/images/photo_of_puja.jpg' | relative_url }}" alt="Portrait of Puja Bhusal" />
  <div class="intro">
    <h1>Puja Bhusal</h1>
    <p>Hello, my name is Puja Bhusal. I am from Nepal. I have completed my Bachelor's degree (BCA). I am currently learning Python programming and improving my technical skills. I am interested in technology, UI/UX design, and continuous learning. My goal is to build a successful career in the IT field and keep developing my knowledge through practice and real-world projects. </p>
  </div>
</section>

<section class="projects">
  <h2>Projects</h2>
  <ul>
    {% for project in site.data.projects %}
      <li>
        <h3>{{ project.name }}</h3>
        <p>{{ project.description }}</p>

        {% if project.url %}
          <p>
            <a href="{{ project.url }}" target="_blank" rel="noopener">
              Visit Project
            </a>
          </p>
        {% endif %}
      </li>
    {% endfor %}
     
  </ul>
</section>

<section class="education">
  <h2>Education</h2>
  <ul>
    {% for education_info in site.data.education %}
      <li>
        <h3>{{ education_info.name }}</h3>
        <p>{{ education_info.description }}</p>
        <p>{{education_info.date}}</p>

        {% if education_info.url %}
          <p>
            <a href="{{ education_info.url }}" target="_blank" rel="noopener">
              Visit Education
            </a>
          </p>
        {% endif %}
      </li>
    {% endfor %}
     
  </ul>
</section>

