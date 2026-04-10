---
layout: default
title: Home
---

<section class="hero">
  <span class="eyebrow">Physics PhD · Photonics · Optical Neural Networks</span>
  <h1>Lo Hsuan</h1>
  <p>
    I work on photonics, inverse design, and optical computation.
    This site collects my research interests, selected projects, writings, and publications.
  </p>

  <div class="button-row">
    <a class="button button-primary" href="/research/">View Research</a>
    <a class="button button-secondary" href="/publications/">Publications</a>
  </div>
</section>

<section class="section">
  <h2 class="section-title">Selected Projects</h2>
  <div class="grid grid-2">
    <div class="card">
      <h3>On-chip spectrometer</h3>
      <p>Inverse-designed compact infrared spectrometer for integrated photonics.</p>
    </div>
    <div class="card">
      <h3>Optical neural network architecture</h3>
      <p>Exploring FFT and diagonal mixing layers for efficient physical matrix operations.</p>
    </div>
  </div>
</section>

<section class="section">
  <h2 class="section-title">Recent Writing</h2>
  <div class="card">
    <ul class="post-list">
      {% for post in site.posts limit:5 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
      </li>
      {% endfor %}
    </ul>
  </div>
</section>