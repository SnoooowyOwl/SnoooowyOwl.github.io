---
title: "数字系统设计"
layout: course
collection: courses
slug: digital-sys
position: 1
permalink: /courses/digital-sys/
---

本课程介绍数字逻辑设计的基础

- CMOS 电路
- 组合逻辑与最小化
- 时序逻辑与状态机
- Verilog 编程基础

---

## 章节目录

{% assign chapters = site.courses | where: "parent", page.slug | sort: "position" %}

<div style="background: #f9f9f9; padding: 1.5rem; border-radius: 12px;">

  {% for chapter in chapters %}
    <div style="margin-bottom: 1.5rem;">
      <h3 style="margin-top: 0; margin-bottom: 0.5rem;">
        <a href="{{ chapter.url | relative_url }}" style="text-decoration: none; color: #0056b3;">
          {{ chapter.title }}
        </a>
      </h3>
      {% if chapter.excerpt %}
        <p style="margin: 0;">{{ chapter.excerpt }}</p>
      {% else %}
        <p style="margin: 0; color: #888;">章节简介待添加。</p>
      {% endif %}
    </div>
  {% endfor %}

</div>
