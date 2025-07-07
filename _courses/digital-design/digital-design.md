---
title: "数字系统原理与设计"
slug: digital-design
collection: courses
date: 2025-07-02
excerpt: "介绍组合逻辑、时序逻辑、Verilog 设计、FPGA 实践等内容"
layout: single
author_profile: true
classes: wide
parent: null
weight: 1
---
22.17
## 📚 章节目录

<ul>
  {% assign course_pages = site.courses | where: "parent", page.slug | sort: "weight" %}
  {% for page in course_pages %}
    <li><a href="{{ page.url }}">{{ page.title }}</a></li>
  {% endfor %}
</ul>
