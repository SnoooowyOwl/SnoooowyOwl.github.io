---
title: "数字系统原理与设计"
collection: courses
date: 2025-7-2
excerpt: "介绍组合逻辑、时序逻辑、Verilog 设计、FPGA 实践等内容"
layout: single
author_profile: true
classes: wide
weight: 1
---

## 课程大作业：大矩阵乘法单元的设计

---

## 📚 参考资料

- [verilator使用教程](#)
- [示例代码](#)


{% assign top_courses = site.courses | where_exp:"item","item.parent == nil" | sort:"weight" %}
{% assign current_index = top_courses | index_of: page %}

<nav class="pagination">
  {% if current_index > 0 %}
    {% assign prev = top_courses[current_index | minus: 1] %}
    <a class="prev" href="{{ prev.url }}">&larr; {{ prev.title }}</a>
  {% endif %}
  {% if current_index < top_courses.size | minus: 1 %}
    {% assign next = top_courses[current_index | plus: 1] %}
    <a class="next" href="{{ next.url }}">{{ next.title }} &rarr;</a>
  {% endif %}
</nav>
