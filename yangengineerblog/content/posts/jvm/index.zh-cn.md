---
weight: 1
title: "JVM"
date: 2019-12-01T21:57:40+08:00
lastmod: 2020-01-01T16:45:40+08:00
draft: false
author: "Yang"
authorLink: ""
description: "JVM入门"
images: []
resources:
- name: "featured-image"
  src: "featured-image.png"
tags: ["jvm", "machine"]
categories: ["JVM"]

lightgallery: true
---

# JVM 包含三个不同的组件

1. Class Loader
1. Loading
2. Linking 
3. Initialization

4. Runtime Memory/Data Area
5. . Method Area
	1. Heap Area
	2. Stack Area
	3. PC Register
	4. Native Method Stack
6. Execution Engine
	5.  Interpreter
	6.  JIT Compiler
	7.  Garbage Collector

## Class Loader
## Garbage Collector
GC是用来管理java的堆内存

1. Mark 识别未使用的对象
2. Sweep 清理上一步识别的对象

GC  Types
1. Serial GC

```
-XX:+UseSerialGC
```
2. Parallel GC
```
-XX:+UseParallelG
```
3. Garbage First(G1)GC - G1GC
```
-XX:+UseG1GC

