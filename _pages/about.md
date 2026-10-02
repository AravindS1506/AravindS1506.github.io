---
layout: default
title: About
permalink: /about/
nav: true
nav_order: 1
description: A little about Aravind Seshadri, his work, interests, and life outside work.
---

<style>
  /* Keep About's palette in step with Home, including cached stylesheet visits. */
  body:has(.folio-about) {
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
    --folio-soft: #efdcd8;
    font-family: "Trebuchet MS", "Segoe UI", sans-serif;
    padding-bottom: 35px;
  }
  html[data-theme="dark"] body:has(.folio-about) {
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
    --folio-soft: #49343c;
  }
  .folio-about { padding-bottom: 0; }
  .folio-about-lead { padding: clamp(2.5rem, 4vw, 3.5rem) 0 2rem; }
  .folio-about-lead h1 {
    margin: 0;
    font-family: "Iowan Old Style", "Palatino Linotype", "Book Antiqua", Georgia, serif;
    font-size: clamp(3.7rem, 7vw, 6.8rem);
    font-weight: 400;
    letter-spacing: -0.075em;
    line-height: 1;
  }
  .folio-about-lead h1 em { color: var(--global-theme-color); font-weight: 400; }
  .folio-about-grid {
    display: grid;
    grid-template-columns: minmax(0, 1.15fr) minmax(280px, 0.85fr);
    align-items: start;
    gap: clamp(2.5rem, 7vw, 7rem);
  }
  .folio-about-copy { padding-top: 0.35rem; }
  .folio-about-copy p {
    max-width: 57ch;
    margin: 0;
    font-size: clamp(1.07rem, 1.5vw, 1.25rem);
    line-height: 1.75;
  }
  .folio-about-copy p + p {
    margin-top: 1.6rem;
    padding-top: 1.5rem;
    border-top: 1px solid var(--global-divider-color);
  }
  .folio-about-portrait {
    position: sticky;
    top: 6.25rem;
    width: min(100%, 390px);
    margin: 0;
    justify-self: end;
  }
  .folio-about-portrait-frame {
    padding: 0.85rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 48% 48% 5px 5px;
    background: var(--folio-soft);
    transform: rotate(2deg);
  }
  .folio-about-portrait img {
    display: block;
    width: 100%;
    aspect-ratio: 4 / 4.5;
    border: 1px dashed var(--global-theme-color);
    border-radius: 48% 48% 2px 2px;
    background: var(--global-card-bg-color);
    object-fit: cover;
  }
  .folio-about-portrait figcaption {
    margin-top: 1.2rem;
    color: var(--global-text-color-light);
    font-family: "Iowan Old Style", "Palatino Linotype", Georgia, serif;
    font-size: 0.95rem;
    font-style: italic;
    text-align: right;
  }
  .folio-about-next {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 1.5rem;
    max-width: 390px;
    margin-top: 2.2rem;
    padding: 1.1rem 1.2rem 1.1rem 1.45rem;
    border: 1px solid var(--global-theme-color);
    border-radius: 4px 26px 4px 26px;
    background: var(--global-card-bg-color);
    box-shadow: 7px 7px 0 var(--folio-soft);
    color: var(--global-text-color);
    font-family: "Iowan Old Style", "Palatino Linotype", Georgia, serif;
    font-size: clamp(1.35rem, 2vw, 1.7rem);
    text-decoration: none !important;
    transition: transform 180ms ease, box-shadow 180ms ease;
  }
  .folio-about-next:hover {
    color: var(--global-text-color);
    box-shadow: 10px 10px 0 var(--folio-soft);
    transform: translate(-3px, -3px);
  }
  .folio-about-next-arrow {
    display: grid;
    flex: none;
    place-items: center;
    width: 2.1rem;
    height: 2.1rem;
    border-radius: 50%;
    background: var(--global-theme-color);
    color: var(--global-hover-text-color);
    font-family: "Trebuchet MS", "Segoe UI", sans-serif;
    font-size: 1.2rem;
  }
  .folio-about-next:focus-visible { outline: 3px solid var(--global-theme-color); outline-offset: 8px; }
  @media (max-width: 900px) {
    .folio-about-grid { grid-template-columns: 1fr; }
    .folio-about-portrait { position: static; width: min(65vw, 310px); justify-self: center; grid-row: 1; }
  }
  @media (max-width: 680px) {
    .folio-about-lead { padding: 2.5rem 0 2rem; }
    .folio-about-lead h1 { font-size: clamp(3.5rem, 12vw, 5.5rem); }
    .folio-about-grid { gap: 2.5rem; }
    .folio-about-portrait { width: min(70vw, 280px); }
  }
  @media (prefers-reduced-motion: reduce) {
    .folio-about-next { transition: none; }
  }
</style>

<div class="folio-editorial folio-about">
  <div class="folio-masthead"><span>01 / About</span><span>Aravind Seshadri</span></div>
  <header class="folio-about-lead"><h1>A little <em>about me.</em></h1></header>

  <div class="folio-about-grid">
    <div class="folio-about-copy">
      <p>I’m a machine learning engineer at Adobe, working on AI safety guardrails and on-device computation. I completed my B.Tech. in Electrical Engineering at the Indian Institute of Technology Kanpur in 2025. I enjoy problems that bring mathematical reasoning into the real world, especially where machine learning meets vision, robotics, and communication.</p>

      <p>Outside work, I love swimming, reading fiction (especially thrillers, mysteries, and sci-fi), and watching movies. I recently started playing the guitar, and most of all, I enjoy exploring new places on my bike.</p>

      <a class="folio-about-next" href="{{ '/experience/' | relative_url }}"><span>The journey so far</span><span class="folio-about-next-arrow" aria-hidden="true">→</span></a>
    </div>

    <figure class="folio-about-portrait">
      <div class="folio-about-portrait-frame">
        <!-- Replace this image path and alt text when the portrait is uploaded. -->
        <img src="{{ '/assets/img/portrait-placeholder.svg' | relative_url }}" alt="Placeholder for Aravind’s portrait">
      </div>
      <figcaption>Portrait coming soon</figcaption>
    </figure>

  </div>
</div>
