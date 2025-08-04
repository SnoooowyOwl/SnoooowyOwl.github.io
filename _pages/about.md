---
permalink: /
title: "Hi ~"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


这个站点主要用来记录一下dz上过的课的有关资料，有关代码部分都是自己一点一点完成的，由于本人能力有限，同一个项目网上可能会有优秀得多的解答。(尤其是[**Arthals**](https://arthals.ink/)写的有关[**CSAPP**](https://github.com/zhuozhiyongde/Introduction-To-Computer-System-2023Fall-PKU)和[**编译原理**](https://github.com/zhuozhiyongde/Compiler-Principles-2024Fall-PKU)的博客,我觉得这两个博客的完善程度绝对是所有教程&解答类博客之中的巅峰，难以想象[**Arthals**](https://arthals.ink/)本人是怎么边上课边写出来这些东西的...本站相比之下就逊色得多...不过记录的意义也不止于此...所以我还是做了这么个东西...记录一下上学的过程)

## News

1.3

---

<div style="
  position: fixed;
  bottom: 10px;
  right: 10px;
  background: rgba(255,255,255,0.9);
  border: 1px solid #ccc;
  padding: 10px 15px;
  border-radius: 8px;
  font-size: 14px;
  max-width: 300px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
  z-index: 9999;
">
  {% assign poems = "床前明月光，疑是地上霜。|举头望明月，低头思故乡。|春眠不觉晓，处处闻啼鸟。|锄禾日当午，汗滴禾下土。|海内存知己，天涯若比邻。|会当凌绝顶，一览众山小。|人生得意须尽欢，莫使金樽空对月。|清明时节雨纷纷，路上行人欲断魂。" | split: "|" %}

  {% assign day_of_year = site.time | date: "%j" | plus: 0 %}
  {% assign index = day_of_year | modulo: poems.size %}

  {{ poems[index] }}
</div>
