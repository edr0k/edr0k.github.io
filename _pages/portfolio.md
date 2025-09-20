---
layout: single
permalink: /portfolio/
title: "Data Science Portfolio"
author_profile: true
---

Here are selected projects that demonstrate my skills in data analysis, statistical modeling, and machine learning.

<hr>

{% for project in site.portfolio %}
  <article class="archive__item">
    <h2 class="archive__item-title">
      <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
    </h2>
    <div class="archive__item-excerpt">
      <p>{{ project.excerpt }}</p>
    </div>
  </article>
{% endfor %}