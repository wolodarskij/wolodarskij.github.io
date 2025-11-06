---
layout: default
title: Home
permalink: /
---

<section class="hero">
  <p class="eyebrow">Alexandr Wolodarkij • Full-stack, DevOps & Product Engineering</p>
  <h1>Building calm, resilient products that ship continuously.</h1>
  <p class="lead">I work with funded startups and product teams that need to scale delivery without losing quality. Together we tighten feedback loops, harden infrastructure, and craft human-centered experiences.</p>
  <div class="hero-actions">
    <a class="button" href="#contact">Start a project</a>
    <a class="link-arrow" href="{{ '/projects' | relative_url }}">Explore recent work</a>
  </div>
</section>

<section class="section" id="focus">
  <h2>Where I make the biggest impact</h2>
  <div class="pill-grid">
    <article>
      <h3>Delivery acceleration</h3>
      <p>CI/CD pipelines, progressive delivery practices, and developer tooling that help teams ship on demand.</p>
    </article>
    <article>
      <h3>Cloud-native architecture</h3>
      <p>Designing secure, observable systems on AWS and GCP with sensible guardrails and layered resilience.</p>
    </article>
    <article>
      <h3>Product discovery</h3>
      <p>Structured discovery sprints that translate customer insight into backlog clarity and measurable outcomes.</p>
    </article>
  </div>
</section>

<section class="section" id="projects">
  <div class="section-heading">
    <h2>Selected projects</h2>
    <a class="link-arrow" href="{{ '/projects' | relative_url }}">See all work</a>
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

<section class="section" id="process">
  <h2>A playbook tuned for momentum</h2>
  <ol class="process">
    <li>
      <strong>Frame the problem.</strong>
      <span>Discovery workshops surface constraints, define success metrics, and align stakeholders.</span>
    </li>
    <li>
      <strong>Shape & prototype.</strong>
      <span>Collaborative architecture and product shaping keeps scope realistic while maximizing learning.</span>
    </li>
    <li>
      <strong>Deliver & harden.</strong>
      <span>Lean builds, rigorous automation, and observability deliver reliable software that is simple to run.</span>
    </li>
  </ol>
</section>

<section class="section testimonials" id="testimonials">
  <h2>What partners say</h2>
  <blockquote>
    “Alexandr helped us move from weekly outages to four nines of uptime in a single quarter, all while tripling iteration speed.”
    <cite>— Nastya Petrenko, CTO at FlowLedger</cite>
  </blockquote>
  <blockquote>
    “He combines strategic product sense with deep technical chops. We now ship experiments weekly and measure impact confidently.”
    <cite>— David Patel, Head of Product at Navigator AI</cite>
  </blockquote>
</section>

<section class="section" id="contact">
  <h2>Ready to collaborate?</h2>
  <p>Tell me a little about your team, product, and the outcomes you are aiming for. I respond within two business days.</p>
  <form class="contact-form" name="contact" method="post" data-netlify="true">
    <input type="hidden" name="form-name" value="contact">
    <div class="field-group">
      <label for="name">Name</label>
      <input id="name" name="name" type="text" required>
    </div>
    <div class="field-group">
      <label for="email">Email</label>
      <input id="email" name="email" type="email" required>
    </div>
    <div class="field-group">
      <label for="company">Company</label>
      <input id="company" name="company" type="text">
    </div>
    <div class="field-group">
      <label for="message">What would you like to build?</label>
      <textarea id="message" name="message" rows="4" required></textarea>
    </div>
    <button type="submit" class="button">Send message</button>
  </form>
</section>
