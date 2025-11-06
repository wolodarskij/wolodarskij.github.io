---
layout: page
title: Projects
permalink: /projects/
---

## Recent work

Here is a snapshot of engagements where I partnered with teams to unlock growth, improve reliability, and elevate user experience.

<div class="project-list">
  {% for project in site.projects %}
  <article class="project-card">
    <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
    <p class="project-meta">{{ project.role }} • {{ project.industry }}</p>
    <p>{{ project.summary }}</p>
    {% if project.outcome %}
    <p class="project-outcome"><strong>Outcome:</strong> {{ project.outcome }}</p>
    {% endif %}
    {% if project.highlights %}
    <ul>
      {% for highlight in project.highlights %}
      <li>{{ highlight }}</li>
      {% endfor %}
    </ul>
    {% endif %}
    {% if project.tags %}
    <ul class="tag-list">
      {% for tag in project.tags %}
      <li>{{ tag }}</li>
      {% endfor %}
    </ul>
    {% endif %}
  </article>
  {% endfor %}
</div>

Looking for something specific? [Reach out](#contact) and I will share a tailored case study.
