---
layout: default
title: Home
permalink: /
---

<section class="hero">
  <p class="eyebrow">Alexandr Wolodarkij • Indie game dev • AI optimist</p>
  <h1>I make games where hidden rules twist your compass.</h1>
  <p class="lead">Mechanical hooks first, moral hangover after.</p>
  <div class="hero-actions">
    <a class="link-arrow" href="{{ '/projects' | relative_url }}">See the latest builds</a>
    <a class="link-arrow" href="mailto:wolodarskij@octobernight.games">Contact</a>
  </div>
</section>

<section class="section" id="pulse">
  <h2>Current obsessions</h2>
  <div class="pill-grid">
    <article>
      <h3>AI conspirators</h3>
      <p>Small models nudging player choices, never stealing agency.</p>
    </article>
    <article>
      <h3>Hidden systems</h3>
      <p>Rules that stay opaque so curiosity has teeth.</p>
    </article>
    <article>
      <h3>Moral clarity</h3>
      <p>No gray sludge. There is right, there is wrong, and you’ll feel the slide.</p>
    </article>
  </div>
</section>

<section class="section" id="projects">
  <div class="section-heading">
    <h2>Playtests in motion</h2>
    <a class="link-arrow" href="{{ '/projects' | relative_url }}">All projects</a>
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
  <h2>Say hi</h2>
  <p>Drop a line at <a href="mailto:wolodarskij@octobernight.games">wolodarskij@octobernight.games</a>. Bring weird ideas, unfinished prototypes, or AI creatures that need a home.</p>
</section>
