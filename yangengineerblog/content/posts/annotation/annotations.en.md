---
weight: 1
title: "Spring Boot Annotaions"
date: 2019-12-01T21:57:40+08:00
lastmod: 2020-01-01T16:45:40+08:00
draft: false
author: "Yang"
authorLink: ""
description: "Spring Boot Annotaions"
images: []
resources:
- name: "featured-image"
  src: "featured-image.png"
tags: ["jvm", "machine"]
categories: ["Java"]

lightgallery: true
---

## 如何使用spring-boot 进行注解装配

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
