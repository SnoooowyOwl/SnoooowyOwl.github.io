---
title: "章节 1：图基础"
collection: courses
parent: computing-system
layout: single
weight: 1
---

章节内容写这里...

{% comment %}
章节页的上一页下一页跳转（只在同一课程章节页之间）
{% endcomment %}
{% assign siblings = site.courses | where: "parent", page.parent | sort: "weight" %}
{% assign current_index = siblings | index_of: page %}

<nav class="pagination">
  {% if current_index > 0 %}
    {% assign prev = siblings[current_index | minus: 1] %}
    <a class="prev" href="{{ prev.url }}">&larr; {{ prev.title }}</a>
  {% endif %}
  {% if current_index < siblings.size | minus: 1 %}
    {% assign next = siblings[current_index | plus: 1] %}
    <a class="next" href="{{ next.url }}">{{ next.title }} &rarr;</a>
  {% endif %}
</nav>
