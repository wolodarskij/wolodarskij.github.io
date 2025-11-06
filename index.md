---
layout: default
title: Home
permalink: /
---

<section class="hero">
  <p class="eyebrow">Alexandr Wolodarkij • indie game dev / AI optimist</p>
  <h1>Games that hook fast and leave you uneasy.</h1>
  <p class="lead">Hidden rules, moral whiplash.</p>
  <div class="hero-actions">
    <a class="link-arrow" href="{{ '/projects' | relative_url }}">Latest builds</a>
    <a class="link-arrow" href="mailto:wolodarskij@octobernight.games">Email</a>
  </div>
</section>

<section class="section" id="pulse">
  <h2>Now</h2>
  <div class="pill-grid">
    <article>
      <h3>AI trouble</h3>
      <p>Tiny models that meddle without stealing control.</p>
    </article>
    <article>
      <h3>Opaque systems</h3>
      <p>Players learn by breaking rules, not tutorials.</p>
    </article>
    <article>
      <h3>Hard lines</h3>
      <p>Right and wrong exist. Feeling the slide is the point.</p>
    </article>
  </div>
</section>

<section class="section" id="projects">
  <div class="section-heading">
    <h2>In playtest</h2>
    <a class="link-arrow" href="{{ '/projects' | relative_url }}">All builds</a>
  </div>
  <ul class="project-grid">
    {% assign featured = site.projects | where: "featured", true | slice: 0, 3 %}
    {% for project in featured %}
    <li>
      <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
      <p>{{ project.summary }}</p>
      {% if project.tags %}
      <ul class="tag-list">
        {% for tag in project.tags %}
        <li>{{ tag }}</li>
        {% endfor %}
      </ul>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</section>

<section class="section" id="ping">
  <h2>Ping me</h2>
  <p><a href="mailto:wolodarskij@octobernight.games">wolodarskij@octobernight.games</a>. Send ideas, builds, or bugs.</p>
</section>
