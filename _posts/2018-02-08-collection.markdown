---
layout:     post
title:      "jdk8中的集合框架(一)"
subtitle:   " \"jdk8中集合框架汇总\""
date:       2018-02-08 11:15:00
author:     "FengZzz"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - java
---



## 前言

最近看书复习基础知识，看到集合框架，做个笔记记录一下。 

##正文

先看整个集合框架。
![img](/img/collection-1.png)

Iterable接口：Collection接口继承的父接口，主要方法为Iterator()方法，返回值类型为Iterator接口，由每个Collection实现类内部自己定义的内部类，实现Iterator接口，确保不同实现类，不同数据结构由自定义的迭代器遍历集合(多态的使用)。
```html
public interface Iterable<T> {
        Iterator<T> iterator();
```
之前一直想着可以有一个自己的博客，也查了很多，无奈都半途而废，这几天在家终于弄出来自己的博客了。

目前完全是按照Hux的github.io模板来做得(其实就是fork+copy人家的github)，目前自己还属于菜鸡阶段，所以很多前端内容都没有深入了解过，所以之后会慢慢搞懂前端部分，不过主要还是更新java吧，写些自己在学习过程之中遇到的各种java语法糖等等，因为自己还属于初级阶段，所以会可能内容不会涉及编译器、虚拟机部分等等，相对基础(其实就是简单)，但是与我而言，也是积累吧，给予自己学习的动力和反馈。
