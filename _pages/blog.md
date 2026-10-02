---
layout: default
title: Blog
permalink: /blog/
nav: true
nav_order: 4
description: Writing and notes from Aravind Seshadri.
---

<style>
  body:has(.folio-journal) {
    --global-bg-color: #fbf7f0;
    --global-text-color: #322b2b;
    --global-text-color-light: #685c5a;
    --global-theme-color: #a34d5a;
    --global-hover-color: #803c48;
    --global-hover-text-color: #fffaf5;
    --global-card-bg-color: #fffaf5;
    --global-divider-color: #dcccc7;
    --global-footer-bg-color: #30262a;
    --global-footer-text-color: #f6eee9;
    --global-footer-link-color: #fffaf5;
    font-family: "Trebuchet MS", "Segoe UI", sans-serif;
  }
  html[data-theme="dark"] body:has(.folio-journal) {
    --global-bg-color: #211d20;
    --global-text-color: #f7ede7;
    --global-text-color-light: #cebdb8;
    --global-theme-color: #f2ab9c;
    --global-hover-color: #ffd0be;
    --global-hover-text-color: #211d20;
    --global-card-bg-color: #30282d;
    --global-divider-color: #58474b;
    --global-footer-bg-color: #191518;
    --global-footer-text-color: #f7ede7;
    --global-footer-link-color: #fffaf5;
  }
  .folio-journal .folio-journal-cover {
    display: block;
    min-height: 0;
    margin-top: 2rem;
    border-left: 4px solid var(--global-theme-color);
    background: var(--global-card-bg-color);
    color: var(--global-text-color);
  }
  .folio-journal .folio-journal-cover-copy { padding: clamp(1.6rem, 4vw, 3rem); }
  .folio-journal .folio-journal-cover h1 {
    color: var(--global-text-color);
    font-family: "Iowan Old Style", "Palatino Linotype", "Book Antiqua", Georgia, serif;
    font-size: clamp(2.8rem, 5vw, 4.6rem);
    letter-spacing: -0.06em;
  }
  .folio-journal .folio-journal-cover-copy > p:last-child {
    margin-top: 0.75rem;
    color: var(--global-text-color-light);
  }
  .folio-journal .folio-journal-entries { margin-top: 1.5rem; }
</style>

<div class="folio-editorial folio-journal">
  <header class="folio-journal-cover">
    <div class="folio-journal-cover-copy"><h1 id="blog-title">Ideas worth sharing.</h1><p>A few pieces I’ve worked on with others.</p></div>
  </header>

  <section class="folio-journal-entries" aria-labelledby="blog-title">
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
</div>
<script>
  // Keep the site's theme switch to one click in either direction.
  if (typeof toggleThemeSetting === "function" && typeof setThemeSetting === "function") {
    toggleThemeSetting = function () {
      const activeTheme = document.documentElement.getAttribute("data-theme");
      setThemeSetting(activeTheme === "dark" ? "light" : "dark");
    };
  }
</script>
