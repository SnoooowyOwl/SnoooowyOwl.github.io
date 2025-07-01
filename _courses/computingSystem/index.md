---
title: "计算系统建模、分析与优化"
collection: courses
date: 2025-07-02
excerpt: "介绍图算法、BDD、SAT、命题逻辑、时序逻辑等内容"
layout: single
author_profile: true
classes: wide
---

## 课程简介
本课程介绍用于建模与分析复杂计算系统的核心方法。涵盖图论、布尔逻辑、SAT 求解器、BDD、LTL/CTL 等内容，是从事形式验证、EDA、复杂系统建模有关方向的入门课程

---

## 章节目录

<ul>
  {% assign course_pages = site.courses | where: "parent", "computation-modeling" | sort: "date" %}
  {% for page in course_pages %}
    <li><a href="{{ page.url }}">{{ page.title }}</a></li>
  {% endfor %}
</ul>