---
layout: default
title: Resume
permalink: /resume/
nav: true
nav_order: 5
description: View Aravind Seshadri's CV and get in touch.
---

<style>
  body:has(.folio-resume-finale) {
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
  html[data-theme="dark"] body:has(.folio-resume-finale) {
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
  .folio-resume-finale {
    display: flex;
    flex-direction: column;
    justify-content: center;
    box-sizing: border-box;
    min-height: calc(100svh - 175px);
    padding: clamp(2.5rem, 6vh, 5rem) 0;
  }
  .folio-resume-finale .folio-eyebrow {
    margin-bottom: 1.5rem;
    color: var(--global-theme-color);
  }
  .folio-resume-finale h1 {
    margin: 0;
    color: var(--global-text-color);
    font-family: "Iowan Old Style", "Palatino Linotype", "Book Antiqua", Georgia, serif;
    font-size: clamp(3.5rem, 8vw, 7.5rem);
    font-weight: 400;
    letter-spacing: -0.07em;
    line-height: 1.05;
  }
  .folio-resume-finale h1 em { color: var(--global-theme-color); font-weight: 400; }
  .folio-resume-finale > p:not(.folio-eyebrow) {
    margin: 1.4rem 0 2.2rem;
    color: var(--global-text-color-light);
    font-size: clamp(1.08rem, 1.7vw, 1.3rem);
  }
  .folio-resume-finale .folio-editorial-cta { align-self: flex-start; }
  .folio-resume-connect {
    display: flex;
    flex-wrap: wrap;
    align-items: baseline;
    gap: 0.8rem 1.7rem;
    margin-top: clamp(3rem, 8vh, 6rem);
    padding-top: 1.5rem;
    border-top: 1px solid var(--global-divider-color);
  }
  .folio-resume-connect p { width: 100%; margin: 0; color: var(--global-text-color-light); }
  .folio-resume-connect a {
    color: var(--global-text-color);
    font-weight: 600;
    text-decoration: none;
  }
  .folio-resume-connect a:hover { color: var(--global-theme-color); text-decoration: underline; }
  .folio-resume-connect a:focus-visible { outline: 3px solid var(--global-theme-color); outline-offset: 4px; }
</style>

<div class="folio-editorial folio-resume-finale">
  <p class="folio-eyebrow">05 / Resume</p>
  <h1>That's all, <em>folks.</em></h1>
  <p>You can view my full CV below.</p>
  <a class="folio-editorial-cta" href="https://drive.google.com/file/d/1deZBfhtYXiNd2hw8zdjlO4vfKKAMVy32/view?usp=sharing" target="_blank" rel="noopener noreferrer">View full CV <span aria-hidden="true">↗</span></a>
  <div class="folio-resume-connect">
    <p>Want to get in touch?</p>
    <a href="https://www.linkedin.com/in/{{ site.data.socials.linkedin_username }}/" target="_blank" rel="noopener noreferrer">LinkedIn ↗</a>
    <a href="https://github.com/{{ site.data.socials.github_username }}" target="_blank" rel="noopener noreferrer">GitHub ↗</a>
    <a href="mailto:{{ site.data.socials.email }}">Email ↗</a>
  </div>
</div>
