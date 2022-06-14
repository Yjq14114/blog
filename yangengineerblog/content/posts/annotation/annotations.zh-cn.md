---
weight: 1
title: "SpringBoot 如何编写注解"
date: 2021-12-01T21:57:40+08:00
lastmod: 2022-01-01T16:45:40+08:00
draft: false
author: "Yang"
authorLink: ""
description: "SpringBoot 如何编写注解"
images: []
tags: ["java", "grpc", "springboot"]
categories: ["Java"]
lightgallery: true
---

## 首先定义一个注解

```java
@Target({ElementType.FIELD})
@Retention(RetentionPolicy.RUNTIME)
@Documented
@Inherited
public @interface GRpcClient {

    String value() default "localhost";

    Class<? extends ClientInterceptor>[] interceptors() default {};
}
```
