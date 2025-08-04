---
permalink: /
title: "Hi ~"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


这个站点主要用来记录一下dz上过的课的有关资料，有关代码部分都是自己一点一点完成的，由于本人能力有限，同一个项目网上可能会有优秀得多的解答。(尤其是[**Arthals**](https://arthals.ink/)写的有关[**CSAPP**](https://github.com/zhuozhiyongde/Introduction-To-Computer-System-2023Fall-PKU)和[**编译原理**](https://github.com/zhuozhiyongde/Compiler-Principles-2024Fall-PKU)的博客,我觉得这两个博客的完善程度绝对是所有教程&解答类博客之中的巅峰，难以想象[**Arthals**](https://arthals.ink/)本人是怎么边上课边写出来这些东西的...本站相比之下就逊色得多...不过记录的意义也不止于此...所以我还是做了这么个东西...记录一下上学的过程)

<div id="floating-poem-box" style="
    position: fixed;
    bottom: 20px;
    right: 20px;
    width: 300px;
    background-color: #f9f9f9cc;
    color: #333;
    border: 1px solid #ccc;
    border-radius: 10px;
    padding: 15px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    z-index: 9999;
    font-size: 14px;
    font-family: 'Georgia', serif;
">
  <strong>今日诗句：</strong>
  <p id="poem-line" style="margin: 8px 0 0;"></p>
</div>

<script>
  const poems = [
    "人生若只如初见，何事秋风悲画扇。",
    "路漫漫其修远兮，吾将上下而求索。",
    "天生我材必有用，千金散尽还复来。"
  ];

  // 简易随机种子函数（基于当天日期）
  function seededRandom(seed) {
    const x = Math.sin(seed) * 10000;
    return x - Math.floor(x);
  }

  const today = new Date();
  const seed = today.getFullYear() * 10000 + (today.getMonth() + 1) * 100 + today.getDate();
  const index = Math.floor(seededRandom(seed) * poems.length);
  document.getElementById("poem-line").textContent = poems[index];
</script>
