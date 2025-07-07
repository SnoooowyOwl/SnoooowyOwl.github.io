---
title: "章节 1：图基础"
collection: courses
parent: computing-system
layout: single
weight: 1
---

章节内容写这里...

{% comment %} 章节页跳转 {% endcomment %}
{% assign siblings = site.courses | where: "parent", page.parent | sort: "weight" %}
{% assign current_index = -1 %}
{% for item in siblings %}
  {% if item.url == page.url %}
    {% assign current_index = forloop.index0 %}
  {% endif %}
{% endfor %}

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
