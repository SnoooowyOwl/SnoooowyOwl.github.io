---
title: "课程大作业:满足约束的样例生成器"
layout: course
collection: courses
parent: computing-sys
position: 1
permalink: /courses/computing-sys/project/
---

假设我们用Verilog写好了一个复杂的组合逻辑模块，现在需要写一些测试用例验证其功能。该怎么办呢，手写吗？还是纯随机生成？一般来说模块的合法输入并非是完全毫无关联的，随机生成的输入很可能现实中根本不会出现。所以，我们面临的问题是：已知一个模块的输入之间有一些关系，现在要尽可能均匀地生成一些测试用例，覆盖到合法输入空间的每一个角落。


你的程序将接收一个json格式的约束，里面会告诉你有几个变量，以及变量之间必须满足的关系；你的程序需要给出一个json格式的输出，包含若干组解，每一组解指明了每个变量的值。详细说明见：[大作业框架](https://github.com/pku-liang/sv-sampler-lab)

---


