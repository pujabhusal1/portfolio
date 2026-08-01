---
layout: default
title: Puja Bhusal | Portfolio
---

<section class="hero">
  <img src="{{ '/assets/images/photo-placeholder.svg' | relative_url }}" alt="Placeholder portrait of Puja Bhusal" />
  <div class="intro">
    <h1>Puja Bhusal</h1>
    <p>Creative developer building meaningful digital experiences with thoughtful design and clean code.</p>
    <p><strong>Photo description:</strong> A soft, natural-light portrait placeholder with a calm and welcoming presence.</p>
  </div>
</section>

<section class="projects">
  <h2>Projects</h2>
  <ul>
    {% for project in site.data.projects %}
    <li>
      <h3>{{ project.name }}</h3>
      <p>{{ project.description }}</p>
    </li>
    {% endfor %}
  </ul>
</section>
