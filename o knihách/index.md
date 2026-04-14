---
layout: category
title:  / o literatuře
category: o literatuře
permalink: /oliterature/
---
<h1>/ o knihách</h1>

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "oliterature" %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="date">{{ post.date | date: "%b %d, %Y" }}</span>
      </li>
    {% endif %}
  {% endfor %}
</ul>
