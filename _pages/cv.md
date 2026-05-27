---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<h2>Education</h2>
<hr />

<div class="list__item">
  <article class="archive__item cv-entry">
    <h3 class="archive__item-title">Ph.D in Physics</h3>
    <p class="archive__item-meta">Massachusetts Institute of Technology <span aria-hidden="true">&middot;</span> 2030 (expected)</p>
  </article>
</div>

<div class="list__item">
  <article class="archive__item cv-entry">
    <h3 class="archive__item-title">B.S. in Physics</h3>
    <p class="archive__item-meta">Nanyang Technological University <span aria-hidden="true">&middot;</span> 2024</p>
  </article>
</div>

<h2>Work Experience</h2>
<hr />

<div class="list__item">
  <article class="archive__item cv-entry">
    <h3 class="archive__item-title">Project Officer</h3>
    <p class="archive__item-meta">Nanyang Technological University <span aria-hidden="true">&middot;</span> 2024-2025</p>
    <p class="archive__item-excerpt">Supervisor: Chong Yidong</p>
  </article>
</div>

<h2>Publications</h2>
<hr />

{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}
