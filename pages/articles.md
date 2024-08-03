---
layout: page
title: "Articles"
permalink: /articles/
---

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "articles" %}
      <li>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
