---
layout: default
title: Blog
permalink: /blog/
nav: true
nav_order: 4
description: Writing and notes from Aravind S.
---

<div class="folio-page-intro"><p class="folio-eyebrow">04 / Blog</p><h1>Notes & ideas<span class="folio-period">.</span></h1><p class="folio-lede">Thoughts, lessons, and observations worth writing down.</p></div>

{% if site.posts.size > 0 %}

<div class="folio-stack">
  {% for post in site.posts %}
  <article class="folio-card folio-post"><div><span class="folio-card-number">{{ post.date | date: '%B %d, %Y' }}</span><h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2><p>{{ post.description | default: post.excerpt | strip_html | truncatewords: 30 }}</p></div><a class="folio-read-link" href="{{ post.url | relative_url }}" aria-label="Read {{ post.title | escape }}">Read article ↗</a></article>
  {% endfor %}
</div>
{% else %}
<div class="folio-card folio-empty"><span class="folio-empty-symbol" aria-hidden="true">✳</span><span class="folio-card-number">Coming soon</span><h2>The first post is on its way.</h2><p>This space is ready for writing. Articles will appear here as they are published.</p></div>
{% endif %}
