---
layout: post
title: "A Gift from Knowledge Distillation"
categories: [blog ]
tags: [CNN, ]
description: 这是一篇关于知识迁移学习的文章
---
声明：本博客欢迎转发，但请保留原作者信息!                            
作者: [曹文龙]                                                                 
博客： <https://cwlseu.github.io/>

## 来源

[CVPR2017](https://cgv.kaist.ac.kr/sigmi/data/CVPR2017.pdf)
## 名词解释
1. 迁移学习

迁移学习的效果与知识的表示是很相关的。
     Because
a DNN uses many layers sequentially to map from the input
space to the output space, the flow of solving a problem can
be defined as the relationship between features from two
layers.

2. FSP matrix

    The extracted feature maps from two layers are used to generate the flow of solution procedure (FSP) matrix. The student DNN is trained to make its FSP matrix similar to that of the teacher DNN

## Model
![本文中的迁移学习方法示意图](../images/cvpr2017/kd/method.JPG)

![DenseNet的组成结构](../images/cvpr2017/kd/arch.JPG)

## 三个任务中使用Distilling the Knowledge方法
### Fast Optimization
### Network Minimization
### Transfer Learning

## 评测标准
Recognition rates
收敛速度
## 小结
本文利用使用两层featuremap 之间的关系表示为FSP。利用这种学习过程知识表示方法，在DNN加速方面有很的表现。并且这个方法还可以应用到迁移学习中。