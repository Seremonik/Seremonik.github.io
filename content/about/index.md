---
title: "About"
draft: false
type: "simple"
showDate: false
showAuthor: false
showReadingTime: false
showTableOfContents: false
showPagination: false
showComments: false
showRelatedContent: false
showTaxonomies: false
showHero: false
sharingLinks: false
showBreadcrumbs: false
showWordCount: false
showViews: false
showLikes: false
showEdit: false
showHeadingAnchors: false
---

<div class="about-page">

  <!-- Hero -->
  <div class="about-hero">
    <img src="/profile_pic.png" alt="Michał Duziak" class="about-avatar" />
    <div class="about-hero-text">
      <h1>Michał Duziak</h1>
      <p class="about-headline">Senior Unity Developer & Tech Lead</p>
      <p class="about-tagline">10+ years shipping games across PC, console, mobile, and XR.</p>
      <div class="about-badges">
        <span class="about-badge">Unity Certified Expert</span>
        <span class="about-badge">Tech Lead</span>
        <span class="about-badge">MMO</span>
        <span class="about-badge">XR</span>
      </div>
    </div>
  </div>

  <!-- Bio -->
  <div class="about-section">
    <h2 class="about-section-title">About Me</h2>
    <p>I'm a Senior Unity Developer and Tech Lead with over a decade of experience building games and interactive applications. I hold the <strong>Unity Certified Expert Programmer</strong> credential and have spent the last several years leading teams and owning architecture on production-scale projects.</p>
    <p>Most recently I served as Tech Lead on a live MMO with 50+ engineers. I care about scalable systems, clean code, and shipping things that actually work.</p>
  </div>

  <!-- Projects -->
  <div class="about-section">
    <h2 class="about-section-title">Featured Projects</h2>
    <div class="about-project-card">
      <div class="about-project-info">
        <h3>Live MMO Gameplay UI — The Sandbox</h3>
        <p>Tech Lead for the gameplay UI layer of a live MMO. Designed scalable input, state, and navigation architecture used across the entire game by a team of 50+ engineers. Translated complex game design requirements into robust, extensible runtime systems built with Unity UI Toolkit.</p>
      </div>
      <div class="about-video-wrapper">
        <video autoplay loop muted playsinline preload="auto">
          <source src="/sandbox_trailer.mp4" type="video/mp4">
        </video>
      </div>
    </div>
  </div>

  <div class="about-project-card about-project-card--image">
    <div class="about-project-info">
      <h3>Magic Leap — XR Application</h3>
      <p>Developed an XR application for Magic Leap, building immersive spatial computing experiences. Leveraged Unity's XR toolkit to create interactive mixed reality environments targeting the Magic Leap headset platform.</p>
    </div>
    <img src="/magicleap.jpg" alt="Magic Leap" class="about-project-image" />
  </div>

</div>

<style>
.about-page {
  max-width: 860px;
  margin: 0 auto;
  padding: 2rem 0;
}

/* Hero */
.about-hero {
  display: flex;
  align-items: center;
  gap: 2.5rem;
  margin-bottom: 3rem;
  flex-wrap: wrap;
}

.about-avatar {
  width: 160px;
  height: 160px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid rgb(var(--color-primary-400));
  flex-shrink: 0;
  box-shadow: 0 0 24px rgba(var(--color-primary-500), 0.3);
}

.about-hero-text h1 {
  margin: 0 0 0.25rem 0;
  font-size: 2rem;
  font-weight: 800;
}

.about-headline {
  color: rgb(var(--color-primary-400));
  font-weight: 600;
  margin: 0 0 0.5rem 0;
  font-size: 1.1rem;
}

.about-tagline {
  margin: 0 0 1rem 0;
  opacity: 0.75;
}

.about-badges {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.about-badge {
  background: rgba(var(--color-primary-500), 0.15);
  color: rgb(var(--color-primary-400));
  border: 1px solid rgba(var(--color-primary-400), 0.3);
  border-radius: 999px;
  padding: 0.2rem 0.75rem;
  font-size: 0.8rem;
  font-weight: 600;
}

/* Sections */
.about-section {
  margin-bottom: 3rem;
}

.about-section-title {
  font-size: 1.3rem;
  font-weight: 700;
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 1px solid rgba(var(--color-primary-400), 0.3);
  color: rgb(var(--color-primary-400));
}

.about-section p {
  margin-bottom: 0.75rem;
  line-height: 1.7;
}

/* Project card */
.about-project-card {
  background: rgba(var(--color-neutral-800), 0.4);
  border: 1px solid rgba(var(--color-neutral-600), 0.4);
  border-radius: 1rem;
  overflow: hidden;
}

.about-project-info {
  padding: 1.5rem;
}

.about-project-info h3 {
  margin: 0 0 0.75rem 0;
  font-size: 1.1rem;
  font-weight: 700;
}

.about-project-info p {
  margin: 0;
  opacity: 0.85;
  line-height: 1.7;
}

/* Project image */
.about-project-card--image {
  margin-top: 1.5rem;
}

.about-project-image {
  width: 100%;
  display: block;
  max-height: 400px;
  object-fit: cover;
}

/* Video */
.about-video-wrapper {
  width: 100%;
  background: #000;
}

.about-video-wrapper video {
  width: 100%;
  display: block;
  max-height: 400px;
}
</style>
