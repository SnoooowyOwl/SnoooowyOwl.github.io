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

---

## 📚 章节目录

{% assign chapters = site.courses | where: "parent", page.slug | sort: "position" %}

<div class="feature__wrapper">
  {% for chapter in chapters %}
    <div class="feature__item" style="border: 1px solid #ccc; padding: 1rem; border-radius: 0.5rem; margin-bottom: 1rem;">
      <h3 style="margin-top: 0;"><a href="{{ chapter.url | relative_url }}">{{ chapter.title }}</a></h3>
      {% if chapter.excerpt %}
        <p>{{ chapter.excerpt }}</p>
      {% else %}
        <p>章节简介待添加。</p>
      {% endif %}
      <a href="{{ chapter.url | relative_url }}" class="btn btn--primary">阅读章节</a>
    </div>
  {% endfor %}
</div>
