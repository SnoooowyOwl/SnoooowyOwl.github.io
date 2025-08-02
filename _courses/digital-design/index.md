---
title: "数字系统设计"
layout: course
collection: courses
slug: digital-sys
position: 1
permalink: /courses/digital-sys/
---

本课程介绍数字逻辑设计的基础，包括：

- CMOS 电路
- 组合逻辑与最小化
- 时序逻辑与状态机
- Verilog 编程基础

欢迎阅读本课程的各个章节！


{% assign chapters = site.courses | where: "parent", page.slug | sort: "position" %}
<ul>
  {% for chapter in chapters %}
    <li><a href="{{ chapter.url | relative_url }}">{{ chapter.title }}</a></li>
  {% endfor %}
</ul>