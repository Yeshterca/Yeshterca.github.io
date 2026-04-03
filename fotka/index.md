---
layout: category
title: / fotka
category: fotka
permalink: /fotka/
---
<h1>/ fotka</h1>

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "poezie" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="date">{{ post.date | date: "%b %d, %Y" }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>