---
title: 动态布局
group:
  path: /layout
  title: 布局方案
  order: 9
nav:
  title: 使用文档
  path: /graphin
  order: 1
---

## 动态布局

`动态布局`是指 布局的过程是动态，可以根据`数据的变化而变化`。因此我们也称之为数据响应布局，比如在 画布分析过程中，需要对数据进行 添加，删除，修改。如果此时对应的布局也需要改变，则我们称之为`动态布局`。

在 Graphin 中，将动态布局分为两类：

- 第一类为普通布局算法的动态布局，比如`circular`,`grid`等，数据的变化后，重新执行该布局函数，通过计算两次布局后节点的最终位置，加以补间动画完成布局响应，因此也称之为`数据响应布局`
- 第二类为力导布局的动态布局。比如`d3-force`,`graphin-force`等。数据变化后，并不能通过再次执行该布局函数就能得到理想的布局，需要对力导的前置布局做预处理，对力的施加处理策略，是一个渐进的过程，因此也称之为`力导渐进布局`

## 【普通布局】动态布局（数据响应布局）

<code src='./demos/normal-layout.tsx'>

## 【力导布局】动态布局（力导渐进布局）

<code src='./demos/graphin-force.tsx'>
