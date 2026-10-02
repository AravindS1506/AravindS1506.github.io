---
layout: default
title: Home
permalink: /
description: A little introduction to Aravind Seshadri.
---

<style>
  /* Home needs this spacing even when a previous main.css is cached. */
  body:has(.folio-home) { padding-bottom: 35px; }
  body:has(.folio-home) > .container.mt-5 { margin-top: 0 !important; }
  .folio-home { padding-bottom: 0; }
  .folio-home-welcome { min-height: calc(100svh - 103px); padding: clamp(1.5rem, 3vh, 3rem) 0; }
</style>

<div class="folio-editorial folio-home">
  <section class="folio-home-welcome" aria-labelledby="home-title">
    <div class="folio-home-copy">
      <h1 id="home-title">Hi, I’m<br><em>Aravind.</em></h1>
      <p class="folio-home-intro">Looks like you’ve stumbled onto my page.<br>Curious about my existence?</p>

      <nav class="folio-home-socials" aria-label="Find me online">
        <a href="https://github.com/{{ site.data.socials.github_username }}" target="_blank" rel="noopener noreferrer">GitHub <span aria-hidden="true">↗</span></a>
        <a href="https://www.linkedin.com/in/{{ site.data.socials.linkedin_username }}/" target="_blank" rel="noopener noreferrer">LinkedIn <span aria-hidden="true">↗</span></a>
      </nav>

      <a class="folio-home-invite" href="{{ '/about/' | relative_url }}"><span>Let’s dig around</span><span class="folio-home-invite-arrow" aria-hidden="true">→</span></a>
    </div>

    <figure class="folio-home-portrait">
      <!-- Replace this image path and alt text when the portrait is uploaded. -->
      <img class="folio-home-portrait-image" src="{{ '/assets/img/portrait-placeholder.svg' | relative_url }}" alt="Placeholder for Aravind’s portrait">
      <figcaption>Portrait coming soon</figcaption>
    </figure>

  </section>
</div>
