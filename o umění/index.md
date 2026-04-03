---
layout: category
title: / o umění
category: o umění
permalink: /oumeni/
---
<h1>/ o umění</h1>

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "ohudbe" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="date">{{ post.date | date: "%b %d, %Y" }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>
