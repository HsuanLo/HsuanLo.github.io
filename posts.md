---
layout: default
title: Posts
permalink: /posts/
---

<section class="page-intro">
  <h1>Posts</h1>
  <p>Notes, research thoughts, and short writing.</p>
</section>

<section class="section">
  <div class="stack">
    {% for post in site.posts %}
      <div class="item">
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        <p class="date">{{ post.date | date: "%B %d, %Y" }}</p>
      </div>
    {% endfor %}
  </div>
</section>
