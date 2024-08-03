---
layout: page
title: "Book Reviews"
permalink: /book-reviews/
---

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "book-reviews" %}
      <li>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
