---
layout: single
permalink: /blog/
title: "Blog"
author_profile: true
---

Welcome to my blog. Here you can find my latest posts.

<hr>

{% for post in site.posts %}
  <article class="archive__item">
    <h2 class="archive__item-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>
    <p class="page__meta"><i class="far fa-clock" aria-hidden="true"></i> {{ post.date | date: "%B %-d, %Y" }}</p>
    <div class="archive__item-excerpt">
      {{ post.excerpt }}
    </div>
  </article>
{% endfor %}