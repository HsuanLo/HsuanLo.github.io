---
layout: default
title: Home
---

<section class="hero">
  <div class="hero-copy">
    <p class="eyebrow">Personal Academic Website</p>
    <h1>Lo Hsuan</h1>
    <p class="intro">
      I am currently a physics PhD candidate in MIT under the condensed matter theory group. I solve problems with theory and computational methods. My current research interest is to study artificial intelligence for physics problems.
    </p>

    <div class="links">
      <a href="mailto:lohsuan@mit.edu">Email</a>
      <a href="https://github.com/hsuanlo">GitHub</a>
      <a href="https://scholar.google.com/citations?user=wek1XTgAAAAJ&hl=en">Google Scholar</a>
      <!-- <a href="#">CV</a> -->
    </div>
  </div>

  <img
    class="profile-photo"
    src="https://github.com/hsuanlo.png"
    alt="Lo Hsuan profile photo"
  >
</section>

<section class="section">
  <h2 class="section-title">Background</h2>
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-date">2025-Present</div>
      <div class="timeline-content">
        <h3>MIT Physics PhD</h3>
        <p>
          Working on photonics, optical computation, and inverse design.
        </p>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-date">2024-2025</div>
      <div class="timeline-content">
        <h3>Project Manager, Nanyang Technological University</h3>
        <p>
          Supervisor: Prof. Chong Yidong
        </p>
      </div>
    </div>

    <div class="timeline-item">
      <div class="timeline-date">2020–2024</div>
      <div class="timeline-content">
        <h3>Bsc in Physics</h3>
        <p>
          Thesis advisor: Prof. Chong Yidong
        </p>
      </div>
    </div>
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
