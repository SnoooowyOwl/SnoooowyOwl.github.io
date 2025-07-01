---
title: "计算系统建模、分析与优化"
collection: courses
date: 2025-07-02
excerpt: "介绍图算法、BDD、SAT、命题逻辑、时序逻辑等内容"
layout: single
author_profile: true
classes: wide
toc: true
---


本课程介绍用于建模与分析复杂计算系统的核心方法。涵盖图论、布尔逻辑、SAT 求解器、BDD、LTL/CTL 等内容，是从事形式验证、EDA、复杂系统建模有关方向的入门课程

---

## 📑 章节导航

- [📑 章节导航](#-章节导航)
- [Graph Basic      图基础](#graph-basic------图基础)
  - [⚙️ 图基本概念](#️-图基本概念)
- [Graph Algorithm      图算法](#graph-algorithm------图算法)
- [Max-flow and Min-cut 最大流与最小割](#max-flow-and-min-cut-最大流与最小割)
- [Tree covering 树覆盖](#tree-covering-树覆盖)
- [Linear Programming 线性规划与整数线性规划](#linear-programming-线性规划与整数线性规划)
- [BDD 布尔决策图](#bdd-布尔决策图)
- [SAT 可满足性问题](#sat-可满足性问题)
- [建模与模型检查](#建模与模型检查)
- [Project](#project)


---

## Graph Basic      图基础

<details open>
<summary><strong>🔍 展开</strong></summary>

### ⚙️ 图基本概念

- 图的类型：有向图、无向图、加权图
- 表示方法：邻接矩阵 / 邻接表
- 路径、圈、连通分量、度数、拓扑排序

## Graph Algorithm      图算法

- 深度优先搜索 DFS / 广度优先搜索 BFS
- 最短路径：Dijkstra、Floyd、Bellman-Ford
- 最小生成树：Kruskal / Prim 算法

</details>

---

## Max-flow and Min-cut 最大流与最小割

<details>
<summary><strong>🔍 展开</strong></summary>

- 网络流建模
- Ford-Fulkerson 算法
- Edmonds-Karp 实现与复杂度
- Max-flow / Min-cut 定理及证明
- 图像分割、作业调度等实际应用

</details>

---

## Tree covering 树覆盖

<details>
<summary><strong>🔍 展开</strong></summary>
</details>

## Linear Programming 线性规划与整数线性规划

<details>
<summary><strong>🔍 展开</strong></summary>
</details>

## BDD 布尔决策图

<details>
<summary><strong>🔍 展开</strong></summary>

- 布尔函数的图表示
- ROBDD 及其唯一性
- BDD 运算规则（合取、析取、非）
- 变量排序策略对 BDD 大小的影响
- BDD 在电路等价性验证中的应用

</details>

---

## SAT 可满足性问题

<details>
<summary><strong>🔍 展开</strong></summary>

- 命题逻辑语法与可满足性问题（SAT）
- 3-SAT 归约与 NP 完全性
- DPLL/CDCL 算法原理
- Minisat / Z3 等求解器简介
- SAT 在验证、测试向量生成中的应用

</details>

---

## 建模与模型检查

<details>
<summary><strong>🔍 展开</strong></summary>

- LTL：线性时序逻辑
- CTL：计算树逻辑
- Kripke 结构建模系统状态空间
- NuSMV/SPIN 实验工具介绍
- 安规验证、硬件时序分析案例

</details>

---

## Project

<details>
<summary><strong>🔍 展开</strong></summary>
满足约束的随机解生成器

</details>