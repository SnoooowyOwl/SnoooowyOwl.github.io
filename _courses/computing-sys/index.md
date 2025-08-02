---
title: "数字系统设计"
layout: course
collection: courses
slug: computing-sys
position: 2
permalink: /courses/computing-sys/
---

本课程介绍基本的图算法，以及数字系统建模仿真的内容

- 图基础
- 图算法
- 树覆盖
- BDD
- SAT
- 命题逻辑
- 一阶逻辑
- 时序逻辑

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
