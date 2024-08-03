---
layout: page
title: "Poems"
permalink: /poems/
---

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "poems" %}
      <li>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
