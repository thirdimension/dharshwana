---
layout: page
title: "Book Blurbs"
permalink: /book-blurbs/
---

<ul>
  {% for post in site.posts %}
    {% if post.categories contains "book-blurbs" %}
      <li>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
