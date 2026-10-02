---
layout: default
title: Home
permalink: /
description: Meet Aravind Seshadri and learn a little about his work and interests.
---

<style>
  /* Home needs this spacing even when a previous main.css is cached. */
  body:has(.folio-home) { padding-bottom: 35px; }
  .folio-home { padding-bottom: 0; }
  .folio-home-layout {
    display: grid;
    grid-template-columns: minmax(0, 1.15fr) minmax(300px, 0.85fr);
    grid-template-areas: "welcome portrait" "about portrait";
    align-items: start;
    column-gap: clamp(2rem, 5vw, 6rem);
  }
  .folio-home-welcome {
    grid-area: welcome;
    display: flex;
    flex-direction: column;
    justify-content: center;
    min-height: calc(100svh - 151px);
    padding: clamp(1.5rem, 3vh, 3rem) 0;
  }
  .folio-home-portrait {
    grid-area: portrait;
    position: sticky;
    top: 6.25rem;
    align-self: start;
    margin-top: clamp(4rem, 9vh, 7rem);
  }
  .folio-home-about {
    grid-area: about;
    scroll-margin-top: 6rem;
    padding: 3rem 0 6rem;
    border-top: 1px solid var(--global-divider-color);
  }
  .folio-home-about h2 {
    margin: 0 0 2rem;
    font-family: "Iowan Old Style", "Palatino Linotype", "Book Antiqua", Georgia, serif;
    font-size: clamp(3.1rem, 5vw, 4.8rem);
    font-weight: 400;
    letter-spacing: -0.07em;
    line-height: 1.08;
  }
  .folio-home-about h2 em { color: var(--global-theme-color); font-weight: 400; }
  .folio-home-about p {
    max-width: 57ch;
    margin: 0;
    font-size: clamp(1.07rem, 1.5vw, 1.25rem);
    line-height: 1.75;
  }
  .folio-home-about p + p {
    margin-top: 1.8rem;
    padding-top: 1.5rem;
    border-top: 1px solid var(--global-divider-color);
  }
  .folio-home-about .folio-home-invite { margin-top: 2.5rem; }
  @media (max-width: 900px) {
    .folio-home-layout {
      grid-template-columns: 1fr;
      grid-template-areas: "welcome" "portrait" "about";
    }
    .folio-home-welcome { min-height: 0; }
    .folio-home-portrait {
      position: static;
      width: min(78vw, 370px);
      margin: 2rem auto 0;
      justify-self: center;
    }
    .folio-home-about { margin-top: 3rem; padding-bottom: 4rem; }
  }
  @media (max-width: 680px) {
    .folio-home-welcome { padding: 3.5rem 0 0; }
    .folio-home-portrait { width: min(74vw, 310px); }
    .folio-home-about { padding-top: 2.5rem; }
  }
</style>

<div class="folio-editorial folio-home">
  <div class="folio-home-layout">
    <section class="folio-home-welcome" aria-labelledby="home-title">
      <div class="folio-home-copy">
        <h1 id="home-title">Hi, I’m<br><em>Aravind.</em></h1>
        <p class="folio-home-intro">Looks like you’ve stumbled onto my page.<br>Curious about my existence?</p>

        <nav class="folio-home-socials" aria-label="Find me online">
          <a href="https://github.com/{{ site.data.socials.github_username }}" target="_blank" rel="noopener noreferrer">GitHub <span aria-hidden="true">↗</span></a>
          <a href="https://www.linkedin.com/in/{{ site.data.socials.linkedin_username }}/" target="_blank" rel="noopener noreferrer">LinkedIn <span aria-hidden="true">↗</span></a>
        </nav>

        <a class="folio-home-invite" href="#about"><span>Let’s dig around</span><span class="folio-home-invite-arrow" aria-hidden="true">↓</span></a>
      </div>
    </section>

    <figure class="folio-home-portrait">
      <!-- Replace this image path and alt text when the portrait is uploaded. -->
      <img class="folio-home-portrait-image" src="{{ '/assets/img/portrait-placeholder.svg' | relative_url }}" alt="Placeholder for Aravind’s portrait">
      <figcaption>Portrait coming soon</figcaption>
    </figure>

    <section id="about" class="folio-home-about" aria-labelledby="about-title">
      <h2 id="about-title">A little <em>about me.</em></h2>
      <p>I’m a machine learning engineer at Adobe, working on AI safety guardrails and on-device computation. I completed my B.Tech. in Electrical Engineering at the Indian Institute of Technology Kanpur in 2025. I enjoy problems that bring mathematical reasoning into the real world, especially where machine learning meets vision, robotics, and communication.</p>

      <p>Outside work, I love swimming, reading fiction (especially thrillers, mysteries, and sci-fi), and watching movies. I recently started playing the guitar, and most of all, I enjoy exploring new places on my bike.</p>

      <a class="folio-home-invite" href="{{ '/experience/' | relative_url }}"><span>The journey so far</span><span class="folio-home-invite-arrow" aria-hidden="true">→</span></a>
    </section>

  </div>
</div>
