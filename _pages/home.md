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
    align-items: stretch;
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
  .folio-home-scroll {
    display: inline-flex;
    align-items: center;
    gap: 0.85rem;
    margin-top: clamp(2.4rem, 5vw, 4rem);
    padding: 0.3rem 0;
    border: 0;
    background: transparent;
    color: var(--global-text-color-light);
    cursor: pointer;
    font-family: "Trebuchet MS", "Segoe UI", sans-serif;
    font-size: 0.95rem;
    font-weight: 600;
  }
  .folio-home-scroll-arrow {
    display: grid;
    place-items: center;
    width: 2.5rem;
    height: 2.5rem;
    border: 1px solid var(--global-theme-color);
    border-radius: 50%;
    color: var(--global-theme-color);
    font-size: 1.25rem;
    transition: transform 180ms ease, background-color 180ms ease;
  }
  .folio-home-scroll:hover { color: var(--global-text-color); }
  .folio-home-scroll:hover .folio-home-scroll-arrow {
    background: var(--folio-soft);
    transform: translateY(3px);
  }
  .folio-home-scroll:focus-visible { outline: 3px solid var(--global-theme-color); outline-offset: 5px; }
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
  @media (prefers-reduced-motion: reduce) {
    .folio-home-scroll-arrow { transition: none; }
  }
</style>

<div class="folio-editorial folio-home">
  <div class="folio-home-layout">
    <section class="folio-home-welcome" aria-labelledby="home-title">
      <div class="folio-home-copy">
        <h1 id="home-title">Hi, I’m<br><em>Aravind.</em></h1>
        <p class="folio-home-intro">Looks like you’ve stumbled onto my page.<br>Curious about my existence?</p>

        <button class="folio-home-scroll" type="button" aria-controls="about"><span>Scroll down</span><span class="folio-home-scroll-arrow" aria-hidden="true">↓</span></button>
      </div>
    </section>

    <figure class="folio-home-portrait">
      <img class="folio-home-portrait-image" src="{{ '/assets/img/aravind-portrait.jpg' | relative_url }}" alt="Portrait of Aravind Seshadri">
    </figure>

    <section id="about" class="folio-home-about" aria-labelledby="about-title">
      <h2 id="about-title">A little <em>about me.</em></h2>
      <p>I’m a machine learning engineer at Adobe, working on AI safety guardrails and on-device computation. I completed my B.Tech. in Electrical Engineering at the Indian Institute of Technology Kanpur in 2025. I enjoy problems that bring mathematical reasoning into the real world, especially where machine learning meets vision, robotics, and communication.</p>

      <p>Outside work, I love swimming, reading fiction (especially thrillers, mysteries, and sci-fi), and watching movies. I recently started playing the guitar, and most of all, I enjoy exploring new places on my bike.</p>

    </section>

  </div>
</div>
<script>
  document.querySelector(".folio-home-scroll").addEventListener("click", function () {
    const about = document.getElementById("about");
    about.scrollIntoView({
      behavior: window.matchMedia("(prefers-reduced-motion: reduce)").matches ? "auto" : "smooth",
      block: "start"
    });
  });
</script>
<script>
  // Keep the site's theme switch to one click in either direction.
  if (typeof toggleThemeSetting === "function" && typeof setThemeSetting === "function") {
    toggleThemeSetting = function () {
      const activeTheme = document.documentElement.getAttribute("data-theme");
      setThemeSetting(activeTheme === "dark" ? "light" : "dark");
    };
  }
</script>
