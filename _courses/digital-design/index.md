---
title: "数字系统设计"
layout: course
collection: courses
slug: digital-sys
position: 1
permalink: /courses/digital-sys/
---

## 本课程介绍数字逻辑设计的基础，包括：

- CMOS 电路
- 组合逻辑与最小化
- 时序逻辑与状态机
- Verilog 编程基础

---

## 章节目录

{% assign chapters = site.courses | where: "parent", page.slug | sort: "position" %}

<div class="cards cards--three">
  {% for chapter in chapters %}
    <div class="card" style="box-shadow: 0 2px 8px rgba(0,0,0,0.08); border-radius: 8px; padding: 1.2rem; margin-bottom: 1rem; background-color: var(--global-bg); transition: transform 0.2s;">
      <h3 style="margin-top: 0;">
        <a href="{{ chapter.url | relative_url }}" style="text-decoration: none; color: inherit;">
          {{ chapter.title }}
        </a>
      </h3>
      {% if chapter.excerpt %}
        <p style="margin-bottom: 0;">{{ chapter.excerpt }}</p>
      {% else %}
        <p style="margin-bottom: 0; color: #888;">章节简介待添加。</p>
      {% endif %}
    </div>
  {% endfor %}
</div>
