---
title: "软件设计实践"
layout: course
collection: courses
slug: software-designPractice
position: 1
permalink: /courses/software-designPractice/
---

本课程介绍面向对象编程和软件设计方法

- c++ 类，继承，封装，多态
- 软件jiegou
- 必要的工具
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
    </div>
  {% endfor %}

</div>
