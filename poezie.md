---
layout: default
title: / poezie 
permalink: /poezie/
---

<section class="post-list">
  {% for post in site.categories.poetry %}
    <article class="post-preview">
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p class="date">{{ post.date | date: "%B %-d, %Y" }}</p>
      <p class="excerpt">{{ post.excerpt | strip_html | truncate: 150 }}</p>
    </article>
  {% endfor %}
</section>
