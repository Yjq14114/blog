---
weight: 1
title: "CQRS 模式"
date: 2020-12-01T21:57:40+08:00
lastmod: 2021-01-01T16:45:40+08:00
draft: false
author: "Yang"
authorLink: ""
description: "CQRS 模式"
images: []
resources:
- name: "featured-image"
  src: "featured-image.png"
tags: ["cqrs", "design pattern"]
categories: ["design pattern"]

lightgallery: true
---

## 意图

CQRS 是一种将查询和命令分离的模式.

## 适用性

- 当查询和命令需要分离的时候
- 当你想要使用诸如event sourcing 或者 task based UI 这类架构的时候
- 当你想要使用不同的数据模型,在处理复杂领域的时候是很有用的

CQRS 通常要结合event-driven模式一起来使用, 下图是CQRS的一个基本架构
![CQRS_Arch](./CQRS_Arch.png)

## 使用AxonFrameWork 实现CQRS

![Command](CQRS_Command_API.png)

上图为AxonFrmework 的一个Command工作流, 首先用户请求