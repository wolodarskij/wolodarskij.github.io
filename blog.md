---
layout: page
title: Dev Log
permalink: /blog/
---

## Short dev notes

Scraps from the build process, AI experiments, and design rabbit holes.

<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <span class="post-date">{{ post.date | date: "%b %d, %Y" }}</span>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
  </li>
  {% endfor %}
</ul>

Want updates in your inbox? [Subscribe to the RSS feed]({{ '/feed.xml' | relative_url }}).
