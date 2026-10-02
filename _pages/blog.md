---
layout: default
title: Blog
permalink: /blog/
nav: true
nav_order: 4
description: Writing and notes from Aravind Seshadri.
---

<div class="folio-editorial folio-journal">
  <div class="folio-masthead"><span>04 / Blog</span><span>Field notes · An open notebook</span></div>
  <header class="folio-journal-cover">
    <div class="folio-journal-cover-copy"><p class="folio-overline">Writing &amp; collaborations</p><h1>Ideas in<br><em>motion.</em></h1><p>Notes on machine learning, perception, robotics, and the questions that connect them.</p></div>
    <div class="folio-journal-mark" aria-hidden="true"><span>FIELD<br>NOTES</span><span>№ 02</span></div>
  </header>

  <section class="folio-journal-entries" aria-labelledby="journal-contributions-heading">
    <div class="folio-section-title"><span class="folio-overline">Writing with others</span><h2 id="journal-contributions-heading">Co-authored articles<span class="folio-period">.</span></h2></div>
    {% for article in site.data.writing %}
    <article class="folio-journal-entry"><time datetime="{{ article.date | date: '%Y-%m-%d' }}">{{ article.date | date: '%B %d, %Y' }}<span class="folio-journal-source">Medium · {{ article.authors }}</span></time><div><h3><a href="{{ article.url }}" target="_blank" rel="noopener noreferrer">{{ article.title }} ↗</a></h3><p>{{ article.description }}</p></div></article>
    {% endfor %}
  </section>

{% if site.posts.size > 0 %}

  <section class="folio-journal-entries" aria-label="Articles">
    <div class="folio-section-title"><span class="folio-overline">The archive</span><h2>More notes<span class="folio-period">.</span></h2></div>
    {% for post in site.posts %}
    <article class="folio-journal-entry"><time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: '%B %d, %Y' }}</time><div><h3><a href="{{ post.url | relative_url }}">{{ post.title }} ↗</a></h3><p>{{ post.description | default: post.excerpt | strip_html | truncatewords: 30 }}</p></div></article>
    {% endfor %}
  </section>
  {% endif %}
  <div class="folio-journal-footer"><span>Perception</span><span>Learning</span><span>Control</span><span>More to come ↗</span></div>
</div>
