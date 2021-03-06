---
layout: post
read_time: true
show_date: true
title: "pytorch的初步知识 "
date: 2021-10-10
img: posts/20211009/pytorch_brand.png
tags: [machine learning, copyright, artificial intelligence, pytorch]
category: machine learning
author: HU YANG
description: "use with pytorch"
---
### CONCEPT

| 0维  | 1维  | 2维  | 3维      | 4维  | 5维  |
| :--- | :--- | :--- | :------- | :--- | :--- |
| 数字 | 向量 | 矩阵 | 时间序列 | 图像 | 视频 |

几何代数中的张量代表什么含义？



### 利用`pytorch`构建不同类型的张量

`torch.rand(4,3)`    构建随机数

` torch.zeros() `

`x=torch.Tensor([5,5,5])` 根据已有数据构建

`x1=x.new_ones([5,5,5],dtype=torch.double)`  利用现有的数据构建，其实构建方法都一样，不过可以显示联系

> pytorch 和 numpy 的联系
>
> | pytorch | `torch.Tensor()`             | `torch.ones(3,4)` | `torch.zeros(3,4)`       | `torch.rand(3,4)`        |      |
> | ------- | ---------------------------- | ----------------- | ------------------------ | ------------------------ | ---- |
> | numpy   | `np.array()`                 | `np.ones((3,4))`  | `np.zeros((3,4))`        | `np.rand(3,4)`           |      |
> | pytorch | `torch.eye()`                | `torch.arange()`  | `torch.linspace(1,4,10)` | `torch.normal(mean,std)` |      |
> | numpy   | `np.eye()`                   | `np.arange()`     | `np.linspace(1,4,10)`    | `np.random.normal(3,4)`  |      |
> | pytorch | `torch.uniform(from,to)`     |                   |                          |                          |      |
> | numpy   | `np.random.uniform(from,to)` |                   |                          |                          |      |



### pytorch 的运算法则

- 加法

  `y.add_(x)` 或者  `torch.add(x,y)`

- 索引

  ![map](/home/huyang/huyanghalo.github.io/_posts/assets/img/posts/20211010/suoyin.png)

  `x[a,b]` a 代表行,b代表列

- 改变size

  `x.view(16)`

  `x.view(-1,8)`

  类似于 `np.reshape()`

- 广播机制













