---
layout: page
title: Projects
permalink: /projects/
---

## Game experiments

Short, strange, usually unstable. These are the builds I keep prodding until they bleed right.

<div class="project-list">
  {% for project in site.projects %}
  <article class="project-card">
    <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
    <p class="project-meta">{{ project.role }} • {{ project.platforms }}</p>
    {% if project.status %}
    <p class="project-status">{{ project.status }}</p>
    {% endif %}
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

Want in on a playtest? [Email me](mailto:wolodarskij@octobernight.games).
