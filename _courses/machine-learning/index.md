---
title: "机器学习"
layout: course
collection: courses
slug: machine-learning
position: 1
permalink: /courses/machine-learning/
---

本课程介绍机器学习的基本内容

- 各类模型结构(CNN,RNN,ResNet,Transformer...)
- 生成式模型(VAE,GAN)
- 强化学习基础

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
