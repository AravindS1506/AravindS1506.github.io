---
layout: default
title: Projects
permalink: /projects/
nav: true
nav_order: 3
description: Machine learning, robotics, and algorithms projects by Aravind Seshadri.
---

<style>
  body:has(.folio-projects) {
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
    --folio-warm: #a34d5a;
    font-family: "Trebuchet MS", "Segoe UI", sans-serif;
  }
  html[data-theme="dark"] body:has(.folio-projects) {
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
    --folio-warm: #f2ab9c;
  }
  .folio-projects .folio-page-intro { padding-bottom: 1.3rem; }
  .folio-projects .folio-page-intro h1,
  .folio-projects .folio-more-title,
  .folio-projects .folio-project h2 {
    font-family: "Iowan Old Style", "Palatino Linotype", "Book Antiqua", Georgia, serif;
    font-weight: 400;
    letter-spacing: -0.05em;
  }
  .folio-projects .folio-more-title {
    margin: 4rem 0 1.7rem;
    font-size: clamp(2.3rem, 4vw, 3.5rem);
  }
  .folio-projects .folio-project h2 { font-size: 1.6rem; }
  .folio-paper-list { margin: 0; padding: 0; list-style: none; }
  .folio-paper-list li {
    display: grid;
    grid-template-columns: 9rem minmax(0, 1fr);
    gap: 1.5rem;
    align-items: baseline;
    padding: 1.1rem 0;
    border-top: 1px solid var(--global-divider-color);
  }
  .folio-paper-list li:last-child { border-bottom: 1px solid var(--global-divider-color); }
  .folio-paper-meta {
    color: var(--global-theme-color);
    font-size: 0.78rem;
    font-weight: 700;
    line-height: 1.45;
  }
  .folio-paper-list a,
  .folio-paper-title {
    color: var(--global-text-color);
    font-size: 1.08rem;
    line-height: 1.5;
    text-decoration: none;
  }
  .folio-paper-list a:hover { color: var(--global-theme-color); text-decoration: underline; }
  .folio-paper-list a:focus-visible { outline: 3px solid var(--global-theme-color); outline-offset: 4px; }
  .folio-paper-list a span { color: var(--global-theme-color); white-space: nowrap; }
  @media (max-width: 600px) {
    .folio-paper-list li { grid-template-columns: 1fr; gap: 0.35rem; }
  }
</style>

<div class="folio-projects">
<div class="folio-page-intro"><p class="folio-eyebrow">03 / Projects</p><h1 id="publications-title">Publications<span class="folio-period">.</span></h1></div>

<section aria-labelledby="publications-title">
  <ol class="folio-paper-list">
    <li><span class="folio-paper-meta">2026 · IEEE Wireless Communications Letters</span><a href="https://doi.org/10.1109/LWC.2026.3677126" target="_blank" rel="noopener noreferrer">Reduced RF Chains Using Fixed Phase Shifters for Over-the-Air Computation <span aria-hidden="true">↗</span></a></li>
    <li><span class="folio-paper-meta">2026 · Research paper</span><span class="folio-paper-title">Influence Enhancement in Opinion Dynamics Using Edge Modification: A Kron Reduction-Based Approach</span></li>
  </ol>
</section>

<section aria-labelledby="more-title">
<h2 id="more-title" class="folio-more-title">Some more<span class="folio-period">...</span></h2>

<div class="folio-grid folio-grid--two">
  <article class="folio-card folio-project"><div class="folio-project-visual folio-project-visual--a" aria-hidden="true"><span>01</span></div><span class="folio-card-number">Oct – Nov 2024 / Computer vision</span><h2>CrowdDiffKDE</h2><p>Enhanced diffusion-based crowd density estimation with KDE to reduce latency.</p><span class="folio-tag">Diffusion · KDE</span><p class="folio-project-link"><a href="https://github.com/AravindS1506/crowddiff">View code ↗</a></p></article>
  <article class="folio-card folio-project"><div class="folio-project-visual folio-project-visual--b" aria-hidden="true"><span>02</span></div><span class="folio-card-number">Jan – Apr 2025 / Probabilistic ML</span><h2>VI-NAM</h2><p>Used a mean-field variational posterior for uncertainty estimation in Neural Additive Models.</p><span class="folio-tag">Variational inference</span><p class="folio-project-link"><a href="https://github.com/AravindS1506/Vi-NAM">View code ↗</a></p></article>
  <article class="folio-card folio-project"><div class="folio-project-visual folio-project-visual--a" aria-hidden="true"><span>03</span></div><span class="folio-card-number">Aug – Nov 2024 / Cyber-physical systems</span><h2>Resilient control execution</h2><p>Worked on a dynamic programming algorithm for control skips during false data injection attacks and trained models to predict attack behavior.</p><span class="folio-tag">Control · GRU · Dynamic programming</span><p class="folio-project-link"><a href="https://github.com/kn-joshua/Design-and-Deployment-of-Resilient-Control-Execution-Patterns">View code ↗</a></p></article>
  <article class="folio-card folio-project"><div class="folio-project-visual folio-project-visual--b" aria-hidden="true"><span>04</span></div><span class="folio-card-number">Jan – Apr 2025 / Algorithms</span><h2>Randomized Quick Sort: A Complete Analysis</h2><p>Derived a strong concentration bound for the number of comparisons in randomized quicksort.</p><span class="folio-tag">Randomized algorithms</span><p class="folio-project-link"><a href="https://github.com/kn-joshua/CS648-Randomized-QuickSort/tree/main">View code ↗</a></p></article>
  <article class="folio-card folio-project"><div class="folio-project-visual folio-project-visual--a" aria-hidden="true"><span>05</span></div><span class="folio-card-number">2022 – 2023 / Aerial robotics</span><h2>FPV drone navigation</h2><p>As part of Team Aerial Robotics, learned to work with ROS and Gazebo while simulating first-person-view drone racing scenarios.</p><span class="folio-tag">ROS · Gazebo · Computer vision</span></article>
</div>
</section>
</div>
