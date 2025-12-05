---
layout: default
title: "Blog"
permalink: /blog/
---

# Blog

Stay current on why agent-based Tier-1 SOC is reshaping operations. Latest posts:

<div class="row g-4">
  {% for post in site.posts %}
  <div class="col-md-6 col-lg-4">
    <div class="card h-100 border-0 shadow-sm">
      <div class="card-body py-4">
        <p class="text-uppercase text-muted small mb-2">{{ post.date | date: "%b %d, %Y" }}</p>
        <h5 class="card-title"><a class="text-dark" href="{{ post.url }}">{{ post.title }}</a></h5>
        <p class="card-text text-muted">{{ post.excerpt | strip_html | truncate: 140 }}</p>
        <a class="text-primary small" href="{{ post.url }}">Read more →</a>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
