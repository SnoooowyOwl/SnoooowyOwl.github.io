---
title: "计算系统建模与优化"
slug: computing-system
collection: courses
date: 2025-07-02
excerpt: "介绍图算法、BDD、SAT、命题逻辑、时序逻辑等内容"
layout: single
author_profile: true
classes: wide
parent: null
weight: 2
---
22.06
## 📚 章节目录

<ul>
  {% assign course_pages = site.courses | where: "parent", page.slug | sort: "weight" %}
  {% for page in course_pages %}
    <li><a href="{{ page.url }}">{{ page.title }}</a></li>
  {% endfor %}
</ul>
