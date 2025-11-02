---
layout: category
title: / poezie
category: / poezie
permalink: /poezie/
---
<h1>/ poezie</h1>

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "oknihach" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="date">{{ post.date | date: "%b %d, %Y" }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>
