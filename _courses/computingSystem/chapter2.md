---
title: "Graph Algorithm 图算法"
collection: courses
parent: computation-modeling  
layout: single
---


{% assign siblings = site.courses | where:"parent", page.parent | sort:"date" %}
{% assign current_index = siblings | index_of: page %}

<nav class="pagination">
  {% if current_index > 0 %}
    {% assign prev = siblings[current_index | minus:1] %}
    <a class="prev" href="{{ prev.url }}">&larr; {{ prev.title }}</a>
  {% endif %}
  {% if current_index < siblings.size | minus:1 %}
    {% assign next = siblings[current_index | plus:1] %}
    <a class="next" href="{{ next.url }}">{{ next.title }} &rarr;</a>
  {% endif %}
</nav>
