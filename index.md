---
layout: default
title: Home
---

<section class="hero">
  <p class="eyebrow">MIT Physcis PhD Candidates</p>
  <h1>Lo Hsuan</h1>
  <p class="intro">
    I am 
  </p>

  <div class="links">
    <a href="mailto:your@email.com">Email</a>
    <a href="https://github.com/your-username">GitHub</a>
    <a href="#">Google Scholar</a>
    <a href="#">CV</a>
  </div>
</section>

<section class="section">
  <h2>Selected work</h2>
  <div class="stack">
    <div class="item">
      <h3>On-chip spectrometer via inverse design</h3>
      <p>Compact infrared spectrometer design for integrated photonics.</p>
    </div>
    <div class="item">
      <h3>Optical neural network architecture</h3>
      <p>Exploring FFT and diagonal mixing layers for efficient physical matrix operations.</p>
    </div>
  </div>
</section>

<section class="section">
  <h2>Latest post</h2>
  <div class="stack">
    {% assign latest_post = site.posts.first %}
    {% if latest_post %}
      <div class="item">
        <h3><a href="{{ latest_post.url | relative_url }}">{{ latest_post.title }}</a></h3>
        <p class="date">{{ latest_post.date | date: "%B %d, %Y" }}</p>
      </div>
    {% else %}
      <div class="item">
        <p>No posts yet.</p>
      </div>
    {% endif %}
  </div>
</section>
