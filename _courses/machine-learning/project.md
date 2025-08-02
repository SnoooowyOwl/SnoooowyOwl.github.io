---
title: "课程大作业：CircuitNet"
layout: course
collection: courses
parent: machine-learning
position: 1
permalink: /courses/machine-learning/project/
---

林亦波老师课题组曾发布了机器学习方法辅助集成电路后端设计的的数据集[**CircuitNet**](https://circuitnet.github.io/)。大作业的任务是首先跑通这个模型，原始模型是一个简单的U-Net。其次按照参考论文或自行搜索论文，探究改进模型的方法。

大作业的主要问题是，假如在本地训练模型，并且没有GPU，20000个epoch就需要约
8小时，模型还没充分收敛！因此本地训练在有限的时间里基本上收敛不了，能看出来的效果也就有限

---