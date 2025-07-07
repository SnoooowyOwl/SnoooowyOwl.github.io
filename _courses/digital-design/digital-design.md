---
title: "数字系统原理与设计"
slug: digital-design
collection: courses
date: 2025-07-02
excerpt: "介绍组合逻辑、时序逻辑、Verilog 设计、FPGA 实践等内容"
layout: single
author_profile: true
classes: wide
weight: 1
---

## 📚 章节目录

<ul>
  {% assign course_pages = site.courses | where: "parent", page.slug | sort: "weight" %}
  {% for page in course_pages %}
    <li><a href="{{ page.url }}">{{ page.title }}</a></li>
  {% endfor %}
</ul>

{% comment %} 课程主页跳转 {% endcomment %}
{% assign siblings = site.courses | where_exp: "item", "item.parent == nil" | sort: "weight" %}
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
