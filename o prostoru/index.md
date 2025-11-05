---
layout: category
title:  / o prostoru
category: o prostoru
permalink: /oprostoru/
---
<h1>/ o knihách</h1>

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "oprostoru" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="date">{{ post.date | date: "%b %d, %Y" }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>