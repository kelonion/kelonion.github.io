---
title: "学习Google如何用DL改变世界"
date: 2019-06-01
categories:
  - Tech
tags:
  - Machine Learning
  - Tutorial
toc: true
toc_label: 文章目录
---

在前不久刚举行完毕的一年一度Google开发者大会 I/O'19 上, Google AI的负责人Jeff Dean在一个小型讨论会上介绍了Google是如何用深度学习技术来解决世界上最具挑战性的问题的（[油管链接](https://www.youtube.com/watch?v=rP8CGyDbxBY&list=WL&index=14&t=0s)）。这个演讲目的其实主要是为了介绍Google在各种具有挑战性的工程问题上作出的努力，但Google作为科技特别是深度学习技术的领头羊，他们的成果也在一定程度上代表了这个领域的最新进展，所以这个演讲的内容对于我们了解人工智能发展进展能起到一定帮助。

## 深度学习在近几年的进展
尽管深度学习算法在几十年前已经被提出来了，但直到近几年才真正展示出它的潜力。甚至到2011年的图像识别竞赛中，最好的成绩也只能做到26%的错误率，也就是每识别四张图中的物体就有一张识别错误。而到了2016年，机器已经能达到3%的错误率了，而人类的错误率是5%，这意味着机器在这个领域上的能力已经超过了人类普通水平。

![](/assets/images/2019-06-01/01_imagenet.png)

而纵观近几年在这个领域上的文献数量也已经超过了[摩尔定律](https://zh.wikipedia.org/wiki/%E6%91%A9%E5%B0%94%E5%AE%9A%E5%BE%8B)了。


![](/assets/images/2019-06-01/02_paper.png)

2008年美国工程院发表了21世纪最具挑战的工程问题清单，而Google也在致力于利用技术去解决这些问题。红色字部分为他们正在着手解决的问题，而粗体部分则是这次演讲重点介绍的部分，这些问题包括：
- 修复及改善城市基建设施
- 推进医疗信息化
- 制造出更好的药物
- 制造更好的科研工具

![](/assets/images/2019-06-01/03_problems.png)

## 修复及改善城市基建设施
这一部分介绍的更多的还是智能化和机械化让人们对城市基建设计有了新的理解。

1. 自动驾驶汽车Waymo
已经有超过100辆Google的自动驾驶汽车Waymo行驶在美国亚利桑那州的凤凰城的路上了。依靠深度学习技术，电脑可以将收集到的图像、雷达、声音等信息经过处理生成一个真实世界的信息化模拟，从而能让车辆顺利完成从A点到达B点的任务。

![](/assets/images/2019-06-01/04_selfdriving.png)

1. 能识别物体的机械臂


![](/assets/images/2019-06-01/05_robot.png)
![](/assets/images/2019-06-01/06_robot.png)
![](/assets/images/2019-06-01/07_robot.png)

1. 自模仿学习

## 推进医疗信息化

![](/assets/images/2019-06-01/08_diabetic.png)
![](/assets/images/2019-06-01/10_retina.png)
![](/assets/images/2019-06-01/11_retina.png)
![](/assets/images/2019-06-01/12_retina.png)
![](/assets/images/2019-06-01/13_retina.png)

## 制造出更好的药物
![](/assets/images/2019-06-01/14_molecules.png)

## 制造更好的科研工具
![](/assets/images/2019-06-01/24_TensorFlow.png)
![](/assets/images/2019-06-01/25_TensorFlow.png)

## 科研上的进展
1. Sparsely gated mixture of experts layer
![](/assets/images/2019-06-01/15_expert.png)
![](/assets/images/2019-06-01/16_expert.png)

2. AutoML
![](/assets/images/2019-06-01/17_automl.png)
![](/assets/images/2019-06-01/18_automl.png)
![](/assets/images/2019-06-01/19_automl.png)
![](/assets/images/2019-06-01/20_automl.png)

3. Single Large Model
![](/assets/images/2019-06-01/21_large_model.png)

5. TPU
![](/assets/images/2019-06-01/22_TPU.png)


## 结论
![](/assets/images/2019-06-01/23_conclusion.png)