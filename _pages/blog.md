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
    <div class="folio-journal-cover-copy"><p class="folio-overline">A place for thinking out loud</p><h1>Ideas in<br><em>progress.</em></h1><p>Notes on machine learning, perception, robotics, and the questions that connect them.</p></div>
    <div class="folio-journal-mark" aria-hidden="true"><span>FIELD<br>NOTES</span><span>№ 00</span></div>
  </header>

{% if site.posts.size > 0 %}

  <section class="folio-journal-entries" aria-label="Articles">
    <div class="folio-section-title"><span class="folio-overline">The archive</span><h2>Published notes<span class="folio-period">.</span></h2></div>
    {% for post in site.posts %}
    <article class="folio-journal-entry"><time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: '%B %d, %Y' }}</time><div><h3><a href="{{ post.url | relative_url }}">{{ post.title }} ↗</a></h3><p>{{ post.description | default: post.excerpt | strip_html | truncatewords: 30 }}</p></div></article>
    {% endfor %}
  </section>
  {% else %}
  <section class="folio-journal-waiting" aria-labelledby="journal-waiting-heading">
    <div class="folio-journal-waiting-no">00 / THE FIRST PAGE</div>
    <div><h2 id="journal-waiting-heading">The notebook is open.<br>The first entry is still being written.</h2><p>There are no articles here yet. In the meantime, you can explore the work and research behind the ideas.</p><div class="folio-journal-links"><a href="{{ '/projects/' | relative_url }}">Explore projects ↗</a><a href="{{ '/about/#publications-heading' | relative_url }}">Read about the research ↗</a></div></div>
  </section>
  {% endif %}
  <div class="folio-journal-footer"><span>Perception</span><span>Learning</span><span>Control</span><span>More to come ↗</span></div>
</div>
