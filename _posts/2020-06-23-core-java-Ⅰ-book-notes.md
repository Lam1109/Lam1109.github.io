---
date: 2020-06-23 14:22:40
layout: post
title: Core Java™, Volume I–Fundamentals
subtitle: (Eleventh Edition) Book Notes
description: The book notes of Core Java™, Volume I–Fundamentals.
image: /assets/img/post_img/corejava1.png
optimized_image: /assets/img/post_img/java1.png
category: java
tags:
  - java
  - fundamentals
author: Lam
---
* [第1章 Java程序设计概述](#%E7%AC%AC1%E7%AB%A0-java%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1%E6%A6%82%E8%BF%B0)
  * [1\.1 程序设计平台](#11-%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1%E5%B9%B3%E5%8F%B0)
  * [1\.2 Java“白皮书”的关键术语](#12-java%E7%99%BD%E7%9A%AE%E4%B9%A6%E7%9A%84%E5%85%B3%E9%94%AE%E6%9C%AF%E8%AF%AD)
    * [1\.2\.1 简单性](#121-%E7%AE%80%E5%8D%95%E6%80%A7)
    * [1\.2\.2 面向对象](#122-%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1)
    * [1\.2\.3 分布式](#123-%E5%88%86%E5%B8%83%E5%BC%8F)
    * [1\.2\.4 健壮性](#124-%E5%81%A5%E5%A3%AE%E6%80%A7)
    * [1\.2\.5 安全性](#125-%E5%AE%89%E5%85%A8%E6%80%A7)
    * [1\.2\.6 体系结构中立](#126-%E4%BD%93%E7%B3%BB%E7%BB%93%E6%9E%84%E4%B8%AD%E7%AB%8B)
    * [1\.2\.7 可移植性](#127-%E5%8F%AF%E7%A7%BB%E6%A4%8D%E6%80%A7)
    * [1\.2\.8 解释型](#128-%E8%A7%A3%E9%87%8A%E5%9E%8B)
    * [1\.2\.9 高性能](#129-%E9%AB%98%E6%80%A7%E8%83%BD)
    * [1\.2\.10 多线程](#1210-%E5%A4%9A%E7%BA%BF%E7%A8%8B)
    * [1\.2\.11 动态性](#1211-%E5%8A%A8%E6%80%81%E6%80%A7)
  * [1\.3 Java applet 与 Internet](#13-java-applet-%E4%B8%8E-internet)
  * [1\.4 Java发展简史](#14-java%E5%8F%91%E5%B1%95%E7%AE%80%E5%8F%B2)
* [第2章 Java程序设计环境](#%E7%AC%AC2%E7%AB%A0-java%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1%E7%8E%AF%E5%A2%83)
* [第3章 Java的基本程序设计结构](#%E7%AC%AC3%E7%AB%A0-java%E7%9A%84%E5%9F%BA%E6%9C%AC%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1%E7%BB%93%E6%9E%84)
  * [3\.1 数据类型](#31-%E6%95%B0%E6%8D%AE%E7%B1%BB%E5%9E%8B)
    * [3\.1\.1 整型](#311-%E6%95%B4%E5%9E%8B)
    * [3\.1\.2 浮点型](#312-%E6%B5%AE%E7%82%B9%E5%9E%8B)
    * [3\.1\.3 char类型](#313-char%E7%B1%BB%E5%9E%8B)
    * [3\.1\.4 boolean类型](#314-boolean%E7%B1%BB%E5%9E%8B)
  * [3\.2 变量与常量](#32-%E5%8F%98%E9%87%8F%E4%B8%8E%E5%B8%B8%E9%87%8F)
    * [3\.2\.1 变量声明与初始化](#321-%E5%8F%98%E9%87%8F%E5%A3%B0%E6%98%8E%E4%B8%8E%E5%88%9D%E5%A7%8B%E5%8C%96)
    * [3\.2\.2 常量](#322-%E5%B8%B8%E9%87%8F)
    * [3\.2\.3 枚举类型](#323-%E6%9E%9A%E4%B8%BE%E7%B1%BB%E5%9E%8B)
  * [3\.3 运算符](#33-%E8%BF%90%E7%AE%97%E7%AC%A6)
    * [3\.3\.1 算术运算符](#331-%E7%AE%97%E6%9C%AF%E8%BF%90%E7%AE%97%E7%AC%A6)
    * [3\.3\.2 数学函数与常量](#332-%E6%95%B0%E5%AD%A6%E5%87%BD%E6%95%B0%E4%B8%8E%E5%B8%B8%E9%87%8F)
    * [3\.3\.3 强制类型转换](#333-%E5%BC%BA%E5%88%B6%E7%B1%BB%E5%9E%8B%E8%BD%AC%E6%8D%A2)
    * [3\.3\.4 位运算符](#334-%E4%BD%8D%E8%BF%90%E7%AE%97%E7%AC%A6)
  * [3\.4 字符串](#34-%E5%AD%97%E7%AC%A6%E4%B8%B2)
    * [3\.4\.1 子串](#341-%E5%AD%90%E4%B8%B2)
    * [3\.4\.2 拼接](#342-%E6%8B%BC%E6%8E%A5)
    * [3\.4\.3 检测字符串是否相等](#343-%E6%A3%80%E6%B5%8B%E5%AD%97%E7%AC%A6%E4%B8%B2%E6%98%AF%E5%90%A6%E7%9B%B8%E7%AD%89)
    * [3\.4\.4 空串与Null串](#344-%E7%A9%BA%E4%B8%B2%E4%B8%8Enull%E4%B8%B2)
    * [3\.4\.5 构建字符串](#345-%E6%9E%84%E5%BB%BA%E5%AD%97%E7%AC%A6%E4%B8%B2)
  * [3\.5 输入与输出](#35-%E8%BE%93%E5%85%A5%E4%B8%8E%E8%BE%93%E5%87%BA)
    * [3\.5\.1 读取输入](#351-%E8%AF%BB%E5%8F%96%E8%BE%93%E5%85%A5)
    * [3\.5\.2 格式化输出](#352-%E6%A0%BC%E5%BC%8F%E5%8C%96%E8%BE%93%E5%87%BA)
    * [3\.5\.3 文件输入与输出](#353-%E6%96%87%E4%BB%B6%E8%BE%93%E5%85%A5%E4%B8%8E%E8%BE%93%E5%87%BA)
    * [3\.5\.4 中断控制流程的语句](#354-%E4%B8%AD%E6%96%AD%E6%8E%A7%E5%88%B6%E6%B5%81%E7%A8%8B%E7%9A%84%E8%AF%AD%E5%8F%A5)
  * [3\.6 大数](#36-%E5%A4%A7%E6%95%B0)
  * [3\.7 数组](#37-%E6%95%B0%E7%BB%84)
    * [3\.7\.1 声明数组](#371-%E5%A3%B0%E6%98%8E%E6%95%B0%E7%BB%84)
    * [3\.7\.2 for each 循环](#372-for-each-%E5%BE%AA%E7%8E%AF)
    * [3\.7\.3 数组拷贝](#373-%E6%95%B0%E7%BB%84%E6%8B%B7%E8%B4%9D)
    * [3\.7\.4 数组排序](#374-%E6%95%B0%E7%BB%84%E6%8E%92%E5%BA%8F)
    * [3\.7\.5 多维数组](#375-%E5%A4%9A%E7%BB%B4%E6%95%B0%E7%BB%84)
* [第4章 对象与类](#%E7%AC%AC4%E7%AB%A0-%E5%AF%B9%E8%B1%A1%E4%B8%8E%E7%B1%BB)
  * [4\.1 面对对象程序设计概述](#41-%E9%9D%A2%E5%AF%B9%E5%AF%B9%E8%B1%A1%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1%E6%A6%82%E8%BF%B0)
    * [4\.1\.1 类](#411-%E7%B1%BB)
    * [4\.1\.2 对象](#412-%E5%AF%B9%E8%B1%A1)
    * [4\.1\.3 识别类](#413-%E8%AF%86%E5%88%AB%E7%B1%BB)
    * [4\.1\.4 类之间的关系](#414-%E7%B1%BB%E4%B9%8B%E9%97%B4%E7%9A%84%E5%85%B3%E7%B3%BB)
  * [4\.2 使用预定义类](#42-%E4%BD%BF%E7%94%A8%E9%A2%84%E5%AE%9A%E4%B9%89%E7%B1%BB)
    * [4\.2\.1 对象与对象变量](#421-%E5%AF%B9%E8%B1%A1%E4%B8%8E%E5%AF%B9%E8%B1%A1%E5%8F%98%E9%87%8F)
  * [4\.3 静态字段与静态方法](#43-%E9%9D%99%E6%80%81%E5%AD%97%E6%AE%B5%E4%B8%8E%E9%9D%99%E6%80%81%E6%96%B9%E6%B3%95)
    * [4\.3\.1 静态字段](#431-%E9%9D%99%E6%80%81%E5%AD%97%E6%AE%B5)
    * [4\.3\.2 静态常量](#432-%E9%9D%99%E6%80%81%E5%B8%B8%E9%87%8F)
    * [4\.3\.3 静态方法](#433-%E9%9D%99%E6%80%81%E6%96%B9%E6%B3%95)
  * [4\.4 方法参数](#44-%E6%96%B9%E6%B3%95%E5%8F%82%E6%95%B0)
  * [4\.5 对象构造](#45-%E5%AF%B9%E8%B1%A1%E6%9E%84%E9%80%A0)
    * [4\.5\.1 重载](#451-%E9%87%8D%E8%BD%BD)
    * [4\.5\.2 默认字段初始化](#452-%E9%BB%98%E8%AE%A4%E5%AD%97%E6%AE%B5%E5%88%9D%E5%A7%8B%E5%8C%96)
    * [4\.5\.3 无参数的构造器](#453-%E6%97%A0%E5%8F%82%E6%95%B0%E7%9A%84%E6%9E%84%E9%80%A0%E5%99%A8)
    * [4\.5\.4 参数名](#454-%E5%8F%82%E6%95%B0%E5%90%8D)
  * [4\.6 包](#46-%E5%8C%85)
  * [4\.7 文档注释](#47-%E6%96%87%E6%A1%A3%E6%B3%A8%E9%87%8A)
    * [4\.7\.1 类注释](#471-%E7%B1%BB%E6%B3%A8%E9%87%8A)
    * [4\.7\.2 方法注释](#472-%E6%96%B9%E6%B3%95%E6%B3%A8%E9%87%8A)
    * [4\.7\.3 通用注释](#473-%E9%80%9A%E7%94%A8%E6%B3%A8%E9%87%8A)
  * [4\.8 类设计技巧](#48-%E7%B1%BB%E8%AE%BE%E8%AE%A1%E6%8A%80%E5%B7%A7)
* [第5章 继承](#%E7%AC%AC5%E7%AB%A0-%E7%BB%A7%E6%89%BF)
  * [5\.1 类、超类和子类](#51-%E7%B1%BB%E8%B6%85%E7%B1%BB%E5%92%8C%E5%AD%90%E7%B1%BB)
    * [5\.1\.1 定义子类](#511-%E5%AE%9A%E4%B9%89%E5%AD%90%E7%B1%BB)
    * [5\.1\.2 子类构造器](#512-%E5%AD%90%E7%B1%BB%E6%9E%84%E9%80%A0%E5%99%A8)
    * [5\.1\.3 继承层次](#513-%E7%BB%A7%E6%89%BF%E5%B1%82%E6%AC%A1)
    * [5\.1\.4 阻止继承：final类和方法](#514-%E9%98%BB%E6%AD%A2%E7%BB%A7%E6%89%BFfinal%E7%B1%BB%E5%92%8C%E6%96%B9%E6%B3%95)
    * [5\.1\.5 抽象类](#515-%E6%8A%BD%E8%B1%A1%E7%B1%BB)
    * [5\.1\.6 受保护的访问](#516-%E5%8F%97%E4%BF%9D%E6%8A%A4%E7%9A%84%E8%AE%BF%E9%97%AE)
  * [5\.2 Object: 所有类的超类](#52-object-%E6%89%80%E6%9C%89%E7%B1%BB%E7%9A%84%E8%B6%85%E7%B1%BB)
    * [5\.2\.1 Object类型的变量](#521-object%E7%B1%BB%E5%9E%8B%E7%9A%84%E5%8F%98%E9%87%8F)
    * [5\.2\.2 equals方法](#522-equals%E6%96%B9%E6%B3%95)
    * [5\.2\.3 相等测试与继承](#523-%E7%9B%B8%E7%AD%89%E6%B5%8B%E8%AF%95%E4%B8%8E%E7%BB%A7%E6%89%BF)
  * [5\.3 泛型数组列表](#53-%E6%B3%9B%E5%9E%8B%E6%95%B0%E7%BB%84%E5%88%97%E8%A1%A8)
    * [5\.3\.1 声明数组列表](#531-%E5%A3%B0%E6%98%8E%E6%95%B0%E7%BB%84%E5%88%97%E8%A1%A8)
    * [5\.3\.2 访问数组列表元素](#532-%E8%AE%BF%E9%97%AE%E6%95%B0%E7%BB%84%E5%88%97%E8%A1%A8%E5%85%83%E7%B4%A0)
  * [5\.4 对象包装器与自动装箱](#54-%E5%AF%B9%E8%B1%A1%E5%8C%85%E8%A3%85%E5%99%A8%E4%B8%8E%E8%87%AA%E5%8A%A8%E8%A3%85%E7%AE%B1)
  * [5\.5 反射](#55-%E5%8F%8D%E5%B0%84)
    * [5\.5\.1 Class类](#551-class%E7%B1%BB)
    * [5\.5\.2 声明异常入门](#552-%E5%A3%B0%E6%98%8E%E5%BC%82%E5%B8%B8%E5%85%A5%E9%97%A8)
  * [5\.6 继承的设计技巧](#56-%E7%BB%A7%E6%89%BF%E7%9A%84%E8%AE%BE%E8%AE%A1%E6%8A%80%E5%B7%A7)
* [第6章 接口、lambda表达式与内部类](#%E7%AC%AC6%E7%AB%A0-%E6%8E%A5%E5%8F%A3lambda%E8%A1%A8%E8%BE%BE%E5%BC%8F%E4%B8%8E%E5%86%85%E9%83%A8%E7%B1%BB)
  * [6\.1 接口](#61-%E6%8E%A5%E5%8F%A3)
    * [6\.1\.1 接口的概念](#611-%E6%8E%A5%E5%8F%A3%E7%9A%84%E6%A6%82%E5%BF%B5)
    * [6\.1\.2 接口的属性](#612-%E6%8E%A5%E5%8F%A3%E7%9A%84%E5%B1%9E%E6%80%A7)
    * [6\.1\.3 接口与抽象类](#613-%E6%8E%A5%E5%8F%A3%E4%B8%8E%E6%8A%BD%E8%B1%A1%E7%B1%BB)
    * [6\.1\.4 静态和私有方法](#614-%E9%9D%99%E6%80%81%E5%92%8C%E7%A7%81%E6%9C%89%E6%96%B9%E6%B3%95)
    * [6\.1\.5 接口与回调](#615-%E6%8E%A5%E5%8F%A3%E4%B8%8E%E5%9B%9E%E8%B0%83)
    * [6\.1\.6 对象克隆](#616-%E5%AF%B9%E8%B1%A1%E5%85%8B%E9%9A%86)
  * [6\.2 lambda表达式](#62-lambda%E8%A1%A8%E8%BE%BE%E5%BC%8F)
    * [6\.2\.1 为什么引入lambda表达式](#621-%E4%B8%BA%E4%BB%80%E4%B9%88%E5%BC%95%E5%85%A5lambda%E8%A1%A8%E8%BE%BE%E5%BC%8F)
    * [6\.2\.2 lambda表达式的语法](#622-lambda%E8%A1%A8%E8%BE%BE%E5%BC%8F%E7%9A%84%E8%AF%AD%E6%B3%95)
  * [6\.3 内部类](#63-%E5%86%85%E9%83%A8%E7%B1%BB)
* [第7章 异常、断言和日志](#%E7%AC%AC7%E7%AB%A0-%E5%BC%82%E5%B8%B8%E6%96%AD%E8%A8%80%E5%92%8C%E6%97%A5%E5%BF%97)
  * [7\.1 处理错误](#71-%E5%A4%84%E7%90%86%E9%94%99%E8%AF%AF)
    * [7\.1\.1 异常分类](#711-%E5%BC%82%E5%B8%B8%E5%88%86%E7%B1%BB)
    * [7\.1\.2 声明检查型异常](#712-%E5%A3%B0%E6%98%8E%E6%A3%80%E6%9F%A5%E5%9E%8B%E5%BC%82%E5%B8%B8)
    * [7\.1\.3 如何抛出异常](#713-%E5%A6%82%E4%BD%95%E6%8A%9B%E5%87%BA%E5%BC%82%E5%B8%B8)
    * [7\.1\.4 创建异常类](#714-%E5%88%9B%E5%BB%BA%E5%BC%82%E5%B8%B8%E7%B1%BB)
  * [7\.2 捕获异常](#72-%E6%8D%95%E8%8E%B7%E5%BC%82%E5%B8%B8)
    * [7\.2\.1 捕获异常](#721-%E6%8D%95%E8%8E%B7%E5%BC%82%E5%B8%B8)
    * [7\.2\.2 捕获多个异常](#722-%E6%8D%95%E8%8E%B7%E5%A4%9A%E4%B8%AA%E5%BC%82%E5%B8%B8)
    * [7\.2\.3 再次抛出异常与异常链](#723-%E5%86%8D%E6%AC%A1%E6%8A%9B%E5%87%BA%E5%BC%82%E5%B8%B8%E4%B8%8E%E5%BC%82%E5%B8%B8%E9%93%BE)
    * [7\.2\.4 finally子句](#724-finally%E5%AD%90%E5%8F%A5)
    * [7\.2\.5 分析堆栈轨迹元素](#725-%E5%88%86%E6%9E%90%E5%A0%86%E6%A0%88%E8%BD%A8%E8%BF%B9%E5%85%83%E7%B4%A0)
  * [7\.3 使用异常的技巧](#73-%E4%BD%BF%E7%94%A8%E5%BC%82%E5%B8%B8%E7%9A%84%E6%8A%80%E5%B7%A7)
  * [7\.4 使用断言](#74-%E4%BD%BF%E7%94%A8%E6%96%AD%E8%A8%80)
    * [7\.4\.1 断言的概念](#741-%E6%96%AD%E8%A8%80%E7%9A%84%E6%A6%82%E5%BF%B5)
    * [7\.4\.2 启用和禁用断言](#742-%E5%90%AF%E7%94%A8%E5%92%8C%E7%A6%81%E7%94%A8%E6%96%AD%E8%A8%80)
    * [7\.4\.3 使用断言完成参数检查](#743-%E4%BD%BF%E7%94%A8%E6%96%AD%E8%A8%80%E5%AE%8C%E6%88%90%E5%8F%82%E6%95%B0%E6%A3%80%E6%9F%A5)
  * [7\.5 日志](#75-%E6%97%A5%E5%BF%97)
    * [7\.5\.1 基本日志](#751-%E5%9F%BA%E6%9C%AC%E6%97%A5%E5%BF%97)
    * [7\.5\.2 高级日志](#752-%E9%AB%98%E7%BA%A7%E6%97%A5%E5%BF%97)
    * [7\.5\.3 处理器](#753-%E5%A4%84%E7%90%86%E5%99%A8)
    * [7\.5\.4 日志技巧](#754-%E6%97%A5%E5%BF%97%E6%8A%80%E5%B7%A7)
* [第8章 泛型程序设计](#%E7%AC%AC8%E7%AB%A0-%E6%B3%9B%E5%9E%8B%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1)
  * [8\.1 为什么要使用泛型程序设计](#81-%E4%B8%BA%E4%BB%80%E4%B9%88%E8%A6%81%E4%BD%BF%E7%94%A8%E6%B3%9B%E5%9E%8B%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1)
    * [8\.1\.1 类型参数的好处](#811-%E7%B1%BB%E5%9E%8B%E5%8F%82%E6%95%B0%E7%9A%84%E5%A5%BD%E5%A4%84)
    * [8\.1\.2 谁想成为泛型程序员](#812-%E8%B0%81%E6%83%B3%E6%88%90%E4%B8%BA%E6%B3%9B%E5%9E%8B%E7%A8%8B%E5%BA%8F%E5%91%98)
  * [8\.2 定义简单泛型类](#82-%E5%AE%9A%E4%B9%89%E7%AE%80%E5%8D%95%E6%B3%9B%E5%9E%8B%E7%B1%BB)
  * [8\.3 泛型方法](#83-%E6%B3%9B%E5%9E%8B%E6%96%B9%E6%B3%95)
  * [8\.4 类型变量的限定](#84-%E7%B1%BB%E5%9E%8B%E5%8F%98%E9%87%8F%E7%9A%84%E9%99%90%E5%AE%9A)
  * [8\.5 泛型代码和虚拟机](#85-%E6%B3%9B%E5%9E%8B%E4%BB%A3%E7%A0%81%E5%92%8C%E8%99%9A%E6%8B%9F%E6%9C%BA)
* [第9章 集合](#%E7%AC%AC9%E7%AB%A0-%E9%9B%86%E5%90%88)
  * [9\.1 Java集合框架](#91-java%E9%9B%86%E5%90%88%E6%A1%86%E6%9E%B6)
    * [9\.1\.1 集合接口与实现分离](#911-%E9%9B%86%E5%90%88%E6%8E%A5%E5%8F%A3%E4%B8%8E%E5%AE%9E%E7%8E%B0%E5%88%86%E7%A6%BB)
    * [9\.1\.2 Collection接口](#912-collection%E6%8E%A5%E5%8F%A3)
    * [9\.1\.3 迭代器](#913-%E8%BF%AD%E4%BB%A3%E5%99%A8)
  * [9\.2 集合框架中的接口](#92-%E9%9B%86%E5%90%88%E6%A1%86%E6%9E%B6%E4%B8%AD%E7%9A%84%E6%8E%A5%E5%8F%A3)
  * [9\.3 具体集合](#93-%E5%85%B7%E4%BD%93%E9%9B%86%E5%90%88)
    * [9\.3\.1 链表](#931-%E9%93%BE%E8%A1%A8)
    * [9\.3\.2 数组列表](#932-%E6%95%B0%E7%BB%84%E5%88%97%E8%A1%A8)
    * [9\.3\.3 散列集](#933-%E6%95%A3%E5%88%97%E9%9B%86)
    * [9\.3\.4 树集](#934-%E6%A0%91%E9%9B%86)
    * [9\.3\.5 队列与双端队列](#935-%E9%98%9F%E5%88%97%E4%B8%8E%E5%8F%8C%E7%AB%AF%E9%98%9F%E5%88%97)
    * [9\.3\.6 优先队列](#936-%E4%BC%98%E5%85%88%E9%98%9F%E5%88%97)
  * [9\.4 映射](#94-%E6%98%A0%E5%B0%84)
    * [9\.4\.1 基本映射操作](#941-%E5%9F%BA%E6%9C%AC%E6%98%A0%E5%B0%84%E6%93%8D%E4%BD%9C)
    * [9\.4\.2 更新映射条目](#942-%E6%9B%B4%E6%96%B0%E6%98%A0%E5%B0%84%E6%9D%A1%E7%9B%AE)
    * [9\.4\.3 映射视图](#943-%E6%98%A0%E5%B0%84%E8%A7%86%E5%9B%BE)
    * [9\.4\.4 弱散列映射](#944-%E5%BC%B1%E6%95%A3%E5%88%97%E6%98%A0%E5%B0%84)
    * [9\.4\.5 链接散列集与映射](#945-%E9%93%BE%E6%8E%A5%E6%95%A3%E5%88%97%E9%9B%86%E4%B8%8E%E6%98%A0%E5%B0%84)
    * [9\.4\.6 枚举集与映射](#946-%E6%9E%9A%E4%B8%BE%E9%9B%86%E4%B8%8E%E6%98%A0%E5%B0%84)
    * [9\.4\.7 标识散列映射](#947-%E6%A0%87%E8%AF%86%E6%95%A3%E5%88%97%E6%98%A0%E5%B0%84)
  * [9\.5 视图与包装器](#95-%E8%A7%86%E5%9B%BE%E4%B8%8E%E5%8C%85%E8%A3%85%E5%99%A8)
    * [9\.5\.1 小集合](#951-%E5%B0%8F%E9%9B%86%E5%90%88)
    * [9\.5\.2 子范围](#952-%E5%AD%90%E8%8C%83%E5%9B%B4)
    * [9\.5\.3 不可修改的视图](#953-%E4%B8%8D%E5%8F%AF%E4%BF%AE%E6%94%B9%E7%9A%84%E8%A7%86%E5%9B%BE)
    * [9\.5\.4 同步视图](#954-%E5%90%8C%E6%AD%A5%E8%A7%86%E5%9B%BE)
    * [9\.5\.5 检查型视图](#955-%E6%A3%80%E6%9F%A5%E5%9E%8B%E8%A7%86%E5%9B%BE)
  * [9\.6 算法](#96-%E7%AE%97%E6%B3%95)
    * [9\.6\.1 为什么使用泛型算法](#961-%E4%B8%BA%E4%BB%80%E4%B9%88%E4%BD%BF%E7%94%A8%E6%B3%9B%E5%9E%8B%E7%AE%97%E6%B3%95)
    * [9\.6\.2 排序与混排](#962-%E6%8E%92%E5%BA%8F%E4%B8%8E%E6%B7%B7%E6%8E%92)
    * [9\.6\.3 批操作](#963-%E6%89%B9%E6%93%8D%E4%BD%9C)
  * [9\.7 遗留的集合](#97-%E9%81%97%E7%95%99%E7%9A%84%E9%9B%86%E5%90%88)
    * [9\.7\.1 属性映射](#971-%E5%B1%9E%E6%80%A7%E6%98%A0%E5%B0%84)
    * [9\.7\.2 位集](#972-%E4%BD%8D%E9%9B%86)
* [第10章 图形用户界面程序设计](#%E7%AC%AC10%E7%AB%A0-%E5%9B%BE%E5%BD%A2%E7%94%A8%E6%88%B7%E7%95%8C%E9%9D%A2%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1)
* [第11章 Swing用户界面组件](#%E7%AC%AC11%E7%AB%A0-swing%E7%94%A8%E6%88%B7%E7%95%8C%E9%9D%A2%E7%BB%84%E4%BB%B6)
* [第12章 并发](#%E7%AC%AC12%E7%AB%A0-%E5%B9%B6%E5%8F%91)
  * [12\.1 什么是线程](#121-%E4%BB%80%E4%B9%88%E6%98%AF%E7%BA%BF%E7%A8%8B)
  * [12\.2 线程状态](#122-%E7%BA%BF%E7%A8%8B%E7%8A%B6%E6%80%81)
    * [12\.2\.1 新建线程](#1221-%E6%96%B0%E5%BB%BA%E7%BA%BF%E7%A8%8B)
    * [12\.2\.2 可运行线程](#1222-%E5%8F%AF%E8%BF%90%E8%A1%8C%E7%BA%BF%E7%A8%8B)
    * [12\.2\.3 阻塞和等待线程](#1223-%E9%98%BB%E5%A1%9E%E5%92%8C%E7%AD%89%E5%BE%85%E7%BA%BF%E7%A8%8B)
    * [12\.2\.4 终止进程](#1224-%E7%BB%88%E6%AD%A2%E8%BF%9B%E7%A8%8B)
  * [12\.3 线程属性](#123-%E7%BA%BF%E7%A8%8B%E5%B1%9E%E6%80%A7)
    * [12\.3\.1 中断线程](#1231-%E4%B8%AD%E6%96%AD%E7%BA%BF%E7%A8%8B)
    * [12\.3\.2 守护线程](#1232-%E5%AE%88%E6%8A%A4%E7%BA%BF%E7%A8%8B)
    * [12\.3\.3 线程名](#1233-%E7%BA%BF%E7%A8%8B%E5%90%8D)
    * [12\.3\.4 未捕获异常的处理器](#1234-%E6%9C%AA%E6%8D%95%E8%8E%B7%E5%BC%82%E5%B8%B8%E7%9A%84%E5%A4%84%E7%90%86%E5%99%A8)
    * [12\.3\.5 线程优先级](#1235-%E7%BA%BF%E7%A8%8B%E4%BC%98%E5%85%88%E7%BA%A7)
  * [12\.4 同步](#124-%E5%90%8C%E6%AD%A5)
    * [12\.4\.1 竞态条件的一个例子](#1241-%E7%AB%9E%E6%80%81%E6%9D%A1%E4%BB%B6%E7%9A%84%E4%B8%80%E4%B8%AA%E4%BE%8B%E5%AD%90)
    * [12\.4\.2 锁对象](#1242-%E9%94%81%E5%AF%B9%E8%B1%A1)
    * [12\.4\.3 条件对象](#1243-%E6%9D%A1%E4%BB%B6%E5%AF%B9%E8%B1%A1)
    * [12\.4\.4 synchronized关键字](#1244-synchronized%E5%85%B3%E9%94%AE%E5%AD%97)
    * [12\.4\.5 同步块](#1245-%E5%90%8C%E6%AD%A5%E5%9D%97)
    * [12\.4\.6 监视器概念](#1246-%E7%9B%91%E8%A7%86%E5%99%A8%E6%A6%82%E5%BF%B5)
    * [12\.4\.7 volatile字段](#1247-volatile%E5%AD%97%E6%AE%B5)
    * [12\.4\.8 final变量](#1248-final%E5%8F%98%E9%87%8F)
    * [12\.4\.9 原子性](#1249-%E5%8E%9F%E5%AD%90%E6%80%A7)
    * [12\.4\.10 死锁](#12410-%E6%AD%BB%E9%94%81)
    * [12\.4\.11 线程局部变量](#12411-%E7%BA%BF%E7%A8%8B%E5%B1%80%E9%83%A8%E5%8F%98%E9%87%8F)
    * [12\.4\.12 为什么废弃stop和suspend方法](#12412-%E4%B8%BA%E4%BB%80%E4%B9%88%E5%BA%9F%E5%BC%83stop%E5%92%8Csuspend%E6%96%B9%E6%B3%95)
  * [12\.5 线程安全的集合](#125-%E7%BA%BF%E7%A8%8B%E5%AE%89%E5%85%A8%E7%9A%84%E9%9B%86%E5%90%88)
    * [12\.5\.1 阻塞队列](#1251-%E9%98%BB%E5%A1%9E%E9%98%9F%E5%88%97)
    * [12\.5\.2 高效的映射、集和队列](#1252-%E9%AB%98%E6%95%88%E7%9A%84%E6%98%A0%E5%B0%84%E9%9B%86%E5%92%8C%E9%98%9F%E5%88%97)
    * [12\.5\.3 映射条目的原子更新](#1253-%E6%98%A0%E5%B0%84%E6%9D%A1%E7%9B%AE%E7%9A%84%E5%8E%9F%E5%AD%90%E6%9B%B4%E6%96%B0)
    * [12\.5\.4 对并发散列映射的批操作](#1254-%E5%AF%B9%E5%B9%B6%E5%8F%91%E6%95%A3%E5%88%97%E6%98%A0%E5%B0%84%E7%9A%84%E6%89%B9%E6%93%8D%E4%BD%9C)
    * [12\.5\.5 并发集视图](#1255-%E5%B9%B6%E5%8F%91%E9%9B%86%E8%A7%86%E5%9B%BE)
    * [12\.5\.6 写数组拷贝](#1256-%E5%86%99%E6%95%B0%E7%BB%84%E6%8B%B7%E8%B4%9D)
    * [12\.5\.7 并行数组算法](#1257-%E5%B9%B6%E8%A1%8C%E6%95%B0%E7%BB%84%E7%AE%97%E6%B3%95)
    * [12\.5\.8 较早的线程安全集合](#1258-%E8%BE%83%E6%97%A9%E7%9A%84%E7%BA%BF%E7%A8%8B%E5%AE%89%E5%85%A8%E9%9B%86%E5%90%88)
  * [12\.6 任务和线程池](#126-%E4%BB%BB%E5%8A%A1%E5%92%8C%E7%BA%BF%E7%A8%8B%E6%B1%A0)
    * [12\.6\.1 Callable与Future](#1261-callable%E4%B8%8Efuture)
    * [12\.6\.2 执行器](#1262-%E6%89%A7%E8%A1%8C%E5%99%A8)
    * [12\.6\.3 控制任务组](#1263-%E6%8E%A7%E5%88%B6%E4%BB%BB%E5%8A%A1%E7%BB%84)
    * [12\.6\.4 fork\-join框架](#1264-fork-join%E6%A1%86%E6%9E%B6)
  * [12\.7 异步计算](#127-%E5%BC%82%E6%AD%A5%E8%AE%A1%E7%AE%97)
    * [12\.7\.1 可完成Future](#1271-%E5%8F%AF%E5%AE%8C%E6%88%90future)
  * [12\.8 进程](#128-%E8%BF%9B%E7%A8%8B)
    * [12\.8\.1 建立一个进程](#1281-%E5%BB%BA%E7%AB%8B%E4%B8%80%E4%B8%AA%E8%BF%9B%E7%A8%8B)
    * [12\.8\.2 运行一个进程](#1282-%E8%BF%90%E8%A1%8C%E4%B8%80%E4%B8%AA%E8%BF%9B%E7%A8%8B)
    * [12\.8\.3 进程句柄](#1283-%E8%BF%9B%E7%A8%8B%E5%8F%A5%E6%9F%84)
  * [12\.9 线程补充](#129-%E7%BA%BF%E7%A8%8B%E8%A1%A5%E5%85%85)
  
***

# 第1章 Java程序设计概述

> Java程序设计平台&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Java发展简史  
Java“白皮书”的关键术语&nbsp;&nbsp;&nbsp;&nbsp;Java applet与Internet  

## 1.1 程序设计平台
- Java并不只是一种语言，更是一个完整的平台。

## 1.2 Java“白皮书”的关键术语
### 1.2.1 简单性
### 1.2.2 面向对象

- 简单来讲，面向对象设计是程序是一种程序设计技术。它将重点放在数据（即对象）和对象的接口上。
- 面向对象和面向过程的区别 
> 用木匠打一个比方：一个“面向对象的”木匠始终首先关注的是所制作的椅子，其次才是所使用的工具；而一个“面向过程的”木匠主要考虑的是所使用的工具。
- 面向过程
> 优点：**性能比面向对象高**，因为类调用时现需要实例化，开销比较大，比较**消耗资源**；比如单片机、嵌入式开发、Linux/Unix等一般采用面向过程开发，性能是最重要的因素。  
  缺点：**不易维护、不易复用、不易扩展**。
- 面向对象
> 优点：**易维护、易复用、易拓展**，由于面向对象有**封装、继承、多态性**的特性，可以设计出**低耦合**的系统，使系统更加灵活、更加易于维护。
  缺点：**性能**比面向过程**低**。

### 1.2.3 分布式
- Java有一个丰富的例程库，用于处理TCP/IP等协议，通过URL打开和访问网络上的对象，其便捷程度就好像访问本第文件一样。

### 1.2.4 健壮性
- Java编译器能够检测出许多在其他语言中仅在运行时才能够检测出来的问题。

### 1.2.5 安全性
- Java一开始便设计成能够防范各种攻击，其中包括：  
> 1. 运行时堆栈溢出，这是蠕虫和病毒常用的攻击手段。  
> 2. 破坏自己的进程空间之外的内存。  
> 3. 未经授权读写文件。  

### 1.2.6 体系结构中立
- Java编译器通过生成与特定计算机体系结构无关的字节码指令来实现这一特性。精心设计的字节码不仅可以很容易地在任何机器上解释执行，而且还可以动态地转换成本地机器代码。

### 1.2.7 可移植性
- 在Java中，数值类型有固定的字节数，这为代码移植提供了便利。而C/C++中，数值类型的字节数跟硬件有关。

### 1.2.8 解释型

### 1.2.9 高性能

### 1.2.10 多线程
- Java是**第一个**支持并发程序设计的主流语言。（多线程出现的原因：摩尔定律即将走到尽头。）
> 摩尔定律：当价格不变时，集成电路上可容纳的元器件数目，每隔18-24个月增加一倍。

### 1.2.11 动态性
- Java能够适应不断发展的环境。

## 1.3 Java applet 与 Internet
- 在网页中运行的Java程序称为 applet。

## 1.4 Java发展简史
- Sun公式的“Green”项目。
- 由“Oak”改名为“Java”。

***

# 第2章 Java程序设计环境


<table>
  <thead>
    <tr>
      <th>术语名</th>
      <th>缩写</th>
      <th>解释</th>
    </tr>
  </thead>
    <tbody>
    <tr>
      <td>Java Development Kit（Java开发工具包）</td>
      <td>JDK</td>
      <td>编写Java程序的程序员使用的软件</td>
    </tr>
    <tr>
      <td>Java Runtime Environment（Java运行时环境）</td>
      <td>JRE</td>
      <td>运行Java程序的用户使用的软件</td>
    </tr>
    <tr>
      <td>Server JRE（服务器JRE）</td>
      <td>——</td>
      <td>在服务器上运行Java程序的软件</td>
    </tr>
    <tr>
      <td>Standard Edition（标准版）</td>
      <td>SE</td>
      <td>用于桌面或简单服务器应用的Java平台</td>
    </tr>
    <tr>
      <td>Enterprise Edition（企业版）</td>
      <td>EE</td>
      <td>用于复杂服务器应用的Java平台</td>
    </tr>
  </tbody>
</table>

***

# 第3章 Java的基本程序设计结构
> 数据类型&nbsp;&nbsp;&nbsp;&nbsp;变量与常量  
  运算符&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;字符串  
  输入输出&nbsp;&nbsp;&nbsp;&nbsp;控制流  
  大数&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;数组  

## 3.1 数据类型

### 3.1.1 整型

<table>
  <thead>
    <tr>
      <th>类型</th>
      <th>存储需求</th>
      <th>取值范围</th>
    </tr>
  </thead>
    <tbody>
    <tr>
      <td>int</td>
      <td>4字节</td>
      <td>-2 147 483 648 ~ 2 147 483 （2<sup>4*8</sup>）</td>
    </tr>
    <tr>
      <td>short</td>
      <td>2字节</td>
      <td>-32 768 ~ 32767 （2<sup>2*8</sup>）</td>
    </tr>
    <tr>
      <td>long</td>
      <td>8字节</td>
      <td>-9 223 372 036 854 775 808 ~ 9 223 372 036 854 775 807 （2<sup>8*8</sup>）</td>
    </tr>
    <tr>
      <td>byte</td>
      <td>1字节</td>
      <td> -128 ~ 127 （2<sup>1*8</sup>）</td>
    </tr>
  </tbody>
</table>

### 3.1.2 浮点型
<table>
  <thead>
    <tr>
      <th>类型</th>
      <th>存储需求</th>
      <th>取值范围</th>
    </tr>
  </thead>
    <tbody>
    <tr>
      <td>float</td>
      <td>4字节</td>
      <td>大约±3.402 823 47E+38F（有效位数为6~7位）</td>
    </tr>
    <tr>
      <td>double</td>
      <td>8字节</td>
      <td>大约±1.797 693 134 862 315 70E+308（有效位数为15位）</td>
    </tr>
  </tbody>
</table>

- 三个特殊的浮点数值：
> 正无穷大  
  负无穷大  
  NaN（不是一个数字）（计算0/0或者负数的平方根结果为NaN。）

### 3.1.3 char类型
- 由于一些Unicode字符需要两个char值描述，所以使用char类型可能导致乱码。

### 3.1.4 boolean类型
- True 
- False

## 3.2 变量与常量

### 3.2.1 变量声明与初始化
- 如果可以从变量的初始值推断出它的类型，就可以使用关键字var而无须指定类型。

```java
var n = 12; //number is an int
var s = "Lam"; //s is a String
```
### 3.2.2 常量
- 在Java中，利用关键字final指示常量，表示这个变量只能被赋值一次。习惯上，常量名使用全大写。  

```java
final double PI = 3.14;
```
### 3.2.3 枚举类型
```java
enum Size { SMALL, MEDIUM, LARGE, EXTRA_LARGE };
//现在可以声明这种类型的变量
Size s = Size.MEDIUM;
```
## 3.3 运算符

### 3.3.1 算术运算符
### 3.3.2 数学函数与常量
```java
double y = Math.pow(x,a); //将y的值设置为x的a次幂
double x = Math.PI； //将x的值设置为π
```
### 3.3.3 强制类型转换
```java
double x = 9.997;
int nx = (int) x; //nx = 9，截取整数部分
int nx = (int) Math.round(x); //nx =10，四舍五入
```
### 3.3.4 位运算符
- “&” （与）
- “&#124;” （或）
- “^” （异或）
- “~” （非）
- “>>” （右移）
- “<<” （左移）
> 移位运算符的右操作数要完成模**32**的运算（左操作数为long类型时，模64）。  

```java
1 << 35 = 1 << 3;
```
## 3.4 字符串
- Java没有**内置**的字符串类型，而是在标准Java类库中提供了一个预定义类**String**。

### 3.4.1 子串
```java
String greeting = "Hello";
String s = greeting.substring(0,3); // s = "Hel"
```
- substring方法的第二个参数是**不想复制的第一个位置**。

### 3.4.2 拼接
```java
//join方法
String all = String.join("/","S","M","L","XL"); // all is "S/M/L/XL";
//repeat方法
String repeated = "LAM".repeat(3);// repeated is "LAMLAMLAM";
```
- 提示: Java字符串不是字符数组。（C程序员初学Java误区。）

### 3.4.3 检测字符串是否相等
- 不能使用 == 运算符检测两个字符串是否相等，而要使用**equals**方法。  

```java
s.equals(t); //返回值为 true 或者 false
```

### 3.4.4 空串与Null串
- 空串不等同于Null串。
- 空串是一个Java对象，有自己的串长度（0）和内容（空）。
- 检查一个字符串既不是null也不是空串

```java
if (str != null && str.length() != 0) //先检查是否null，因为对null串调用length()方法会报错
```

### 3.4.5 构建字符串
```java
StringBuilder sb = new StringBuilder();
sb.append(ch);// appends a single character
sb.append(str);// appends a string
String completedString = sb.toString(); 
```

## 3.5 输入与输出

### 3.5.1 读取输入
```java
Scanner in = new Scanner(System.in);
String name = in.nextLine();
```

> nextLine() 读一行  
  next() 读一次（空格结束）  
  nextInt() 读一整数

### 3.5.2 格式化输出
```java
System.out.println("LAM"); // print LAM
```

### 3.5.3 文件输入与输出

```java
//文件输入

//方法一
Scanner in = new Scanner(Path.of("inputfile.txt"),StandardCharsets.UTF_8);
String s1=in.nextLine();

//方法二（性能高） 
BufferedReader bf = new BufferedReader(new FileReader("inputfile.txt"));
String s2=bf.readLine(); //BufferedReader的read()方法返回int类型。

//...

//文件输出
PrintWriter pw = new PrintWriter("outputfile.txt",StandardCharsets.UTF_8);
pw.print("hello");
pw.close();// 必要
```

### 3.5.4 中断控制流程的语句

```java
break; // 终止循环
continue； // 终止本次循环，跳到循环首部(进行下一次循环)。
```

## 3.6 大数
- 如果基本的整数和浮点数精度不够，可以使用**java.math**包中的**BigInteger**和**BigDecimal**;

## 3.7 数组

### 3.7.1 声明数组

```java
int[] a = new int[100]; // or var a = new int[100];
```

### 3.7.2 for each 循环

```java
for (int e : a){
    System.out.println(e); // 打印数组a中每一个元素
}
```

### 3.7.3 数组拷贝
- 在Java中，允许将一个数组变量拷贝到另一个数组变量。

```java
int[] lunckyNumbers = smallPrimes;
luckyNumbers[5] = 12; // now smallPrimes[5] is also 12
//即不会新建数组，本质上是同一个数组。
```

- 要新建一个数组，可以使用**Arrays**类中的**copyOf**方法。

```java
inr[] copy = Arrays.copyOf(luckyNumbers, luckyNumbers.length); // copy是一个新的数组
```

- **length用于获取数组长度，而length()用于获取字符串长度。**

### 3.7.4 数组排序
- 使用**Arrays**类中的**sort**方法。

```java
// int[] a = {3,1,2};
Arrays.sort(a); //  升序，优化的快速排序（QuickSort）算法
// now a = {1,2,3}
```

### 3.7.5 多维数组
- Java实际上没有多维数组，多维数组被解释为“数组的数组”。

# 第4章 对象与类
> 面对对象程序设计概述  
  对象构造  
  使用预定义类  
  包  
  用户自定义类  
  静态字段与静态方法  
  文档注释
  方法参数  
  类设计技巧

***

## 4.1 面对对象程序设计概述
- 面对对象程序设计（object-oriented programming，**OOP**）是当今主流的程序设计范型。
- Algorithms + Data Structures = Programs

### 4.1.1 类
- **类**（class）是构造对象的模板或者蓝图。

### 4.1.2 对象
- 对象的三个主要特性：
> 对象的行为——可以对对象完成哪些操作，或者可以对对象应用哪些方法？  
  对象的状态——当调用方法时，对象会如何响应？  
  对象的标识——如何区分具有相同行为与状态的不同对象？  

### 4.1.3 识别类
- 识别类的一个简单经验是在分析问题的过程中寻找名词，而方法对应着动词。

### 4.1.4 类之间的关系
- **依赖**（use-a）
- **聚合**（has-a）
- **继承**（is-a）

## 4.2 使用预定义类
### 4.2.1 对象与对象变量
- 构造器的名字应该与类名相同。

## 4.3 静态字段与静态方法
### 4.3.1 静态字段
- 如果将一个字段定一为**static**，每个类只有一个这样的字段。
- 静态字段被称为**类字段**。术语“静态”至少沿用了C++的叫法，并无实际意义。

```java
class Employee{
    private static int nextId = 1;
    private int id;
    ...
}
```
> 每一个Employee对象都有一个自己的id字段，但这个类的所有实例将共享一个nextId字段。

### 4.3.2 静态常量

```java
public class Math{
    ...
    public static final double PI = 3.14159265358979323846;
    ...
}
```
> 在程序中我们就可以使用Math.PI来访问这个常量。

### 4.3.3 静态方法
- 以下两种情况可以使用静态方法：
> 方法不需要访问对象状态，因为它需要的所有参数都通过显示参数提供（例如：Math.pow）。  
  方法只需要访问类的静态字段。

## 4.4 方法参数
- 在Java中，对方法参数能做什么和不能做什么：
> 方法不能修改基本数据类型的参数（即数值型和布尔型）。  
  方法可以改变对象参数的状态。
  方法不能让一个对象参数引用一个新的对象。

## 4.5 对象构造
### 4.5.1 重载
- 有些类有多个构造器。这种功能叫做**重载**（overloading）。

### 4.5.2 默认字段初始化
- 数值为0
- 布尔值为false
- 对象引用为null

### 4.5.3 无参数的构造器
- 由无参数构造器创建对象时，对象的状态会设置为设当的默认值。如果写一个类时没有编写构造器，就会为你提供一个无参数构造器。

### 4.5.4 参数名

```java
public Employee(String name, double salary){
    this.name = name;
    this.salary = salary;
}
```

## 4.6 包
- C/C&#43;&#43;程序员经常将import与#include弄混。实际上，两者完全不同。C/C&#43;&#43;编译器无法查看任何其他文件的内部，必须使用#include来加载外部特性的声明。Java编译器则不同，可以查看其他文件的内部，只需要告诉它到哪里去查看就可以了。

## 4.7 文档注释
### 4.7.1 类注释
- 类注释必须放在import语句之后，类定义之前。

### 4.7.2 方法注释

```java
/**
* @param variable description 参数
* @return description 返回值
* @throws class description 可能的异常
*/
```

### 4.7.3 通用注释

```java
/**
* @author name 作者
* @version text 版本
*/
```

## 4.8 类设计技巧
> 1. 一定要保证数据私有。  
> 2. 一定要对数据进行初始化。
> 3. 不要在类中使用过多的基本类型。
> 4. 不是所有的字段都需要单独的字段访问器和字段更改器。
> 5. 分解有过多职责的类。
> 6. 类名和方法名要能够体现它们的职责。
> 7. 优先使用不可变的类。

***

# 第5章 继承
> 类、超类和子类  
  参数数量可变的方法  
  Object：所有类的超类  
  枚举类  
  泛型数组列表  
  反射  
  对象包装器与自动装箱  
  继承的设计技巧  
  
## 5.1 类、超类和子类
### 5.1.1 定义子类
- 可以如下继承Employee类定义Manager类，使用关键字**extends**表示继承。

```java
/* public class Employee{
    ...
    int getSalary(){
        ...
    }
}
*/
public class Manager extends Employee{
    //子类特有字段
    private double bonus;
    ...
    //调用父类中的方法
    super.getSalary();
}
```

- 一般的方法放在超类中，特殊的方法放在子类中。

### 5.1.2 子类构造器

```java
public Manager(String name, double salary, int year, int month, int day){
    super(name, salary, year, month, day);
    bonus = 0;
}
```

- 一个对象变量可以指示多种实际类型的现象称为多态。在运行中能够自动地选择适当的方法，称为动态绑定。

### 5.1.3 继承层次
- 继承不仅限于一个层次。

### 5.1.4 阻止继承：final类和方法
- 不允许扩展的类被称为final类。

```java
public final class Example{
    ...
}
```

- 方法声明为final，意味着子类不能覆盖整个方法（final类中的所有方法自动地成为final方法）。

```java
public class Employee{
    ...
    public final String getName(){
        return name;
    }
    ...
}
```

### 5.1.5 抽象类
- 关键字a**bstract**
- 包含一个或多个抽象方法的类本身必须被声明为抽象的。

### 5.1.6 受保护的访问
<table>
  <thead>
    <tr>
      <th>作用域</th>
      <th>当前类</th>
      <th>同一package</th>
      <th>子孙类</th>
      <th>其他package</th>
    </tr>
  </thead>
    <tbody>
    <tr>
      <td>public</td>
      <td>√</td>
      <td>√</td>
      <td>√</td>
      <td>√</td>
    </tr>
    <tr>
      <td>protected</td>
      <td>√</td>
      <td>√</td>
      <td>√</td>
      <td>×</td>
    </tr>
    <tr>
      <td>friendly（不修饰）</td>
      <td>√</td>
      <td>√</td>
      <td>×</td>
      <td>×</td>
    </tr>
    <tr>
      <td>private</td>
      <td>√</td>
      <td>×</td>
      <td>×</td>
      <td>×</td>
    </tr>
  </tbody>
</table>

## 5.2 Object: 所有类的超类
### 5.2.1 Object类型的变量
- 可以使用Object类型的变量引用任何类型的对象：

```java
Object obj = new Employee("Lam",35000);
```

### 5.2.2 equals方法
- Object类中的equals方法用于检测一个对象是否等于另外一个对象。

### 5.2.3 相等测试与继承
- 自反性：对于任何非空引用x，x.equals(x)应该返回true。
- 对称性：对于任何引用x和y，当且仅当x.equals(y)返回true时，y.equals(x)返回true。
- 传递性：对于任何引用x、y和z，如果x.equals(y)返回true，y.equals(z)返回true，x.equals(z)也应该返回true。
- 一致性：如果x和y引用的对象没有发生变化，反复调用x.equals(y)应该返回同样的结果。
- 对于任何非空引用x，x.equals(null)应该返回false。

## 5.3 泛型数组列表
- ArrayList是一个有类型参数的泛型类。

### 5.3.1 声明数组列表
- 声明和构造一个保存Employee对象的数组列表：

```java
ArrayList<Employee> staff = new ArrayList<Employee>();
//or ArrayList<Employee> staff = new ArrayList<>();

// Java 10中，避免重复写类名
var staff = new new ArrayList<Employee>();
```

- 方法：

```java
//添加
staff.add(new Employee("Lam", ...);

//元素个数
staff.size();
```

### 5.3.2 访问数组列表元素

```java
//set 修改第i个元素
staff.set(i,lam); // var lam = new Employee("Lam", ...);

//get 获取第i个元素
staff.get(i);
```

## 5.4 对象包装器与自动装箱
- 数组列表<>中的类型参数不允许是基本类型。

```java
var list = new ArrayList<Integer>(); // instead of new ArrayList<int>();
```
- 调用list.add(3);时，会自动变换成list.add(Integer.valueOf(3)); 这种变换称为自动装箱（autoboxing）。

## 5.5 反射
- 反射库提供了一个丰富且精巧的工具集，可以用来编写能够动态操纵Java代码的程序。
- 反射机制可以用来：
> 在运行时分析类的能力。  
  在运行时检查对象。  
  实现泛型数组操作代码。  
  利用Method对象，这个对象很像C++中的函数指针。

### 5.5.1 Class类
- 在程序运行期间，Java运行时系统始终为所有对象维护一个**运行时类型标识**。
- Object类中的getClass()方法将会返回一个Class类型的实例。

```java
Employee e;
...
Class cl = e.getClass();
```

- 最常用的Class方法就是getName，这个方法会返回类的名字。

```java
System.out.println(e.getClass().getName() + " " + e.getName());
// if Eployee e, print "Employee Lam"
// if Manager e, print "Manager Lam"
```

### 5.5.2 声明异常入门
- 异常有两种类型：**非检查型**（unchecked）异常和**检查型**（checked）异常。
- 如果一个方法包含一条可能抛出检查型异常的语句，则在方法名上增加一个throws子句。

```java
public static void doSomethingWithClass(String name)
    throws ReflectiveOperationException{
        Class cl = Class.forName(name); // might throw exception
        ...
    }
```

## 5.6 继承的设计技巧
> 1. 将公共操作和字段放在超类中。  
> 2. 不要使用受保护的字段。  
> 3. 使用继承实现“is-a”关系。  
> 4. 除非所有继承的方法都有意义，否则不要使用继承。  
> 5. 在覆盖方法时，不要改变预期的行为。  
> 6. 使用多态，而不要使用类型信息。  
> 7. 不要滥用反射。  

***

# 第6章 接口、lambda表达式与内部类
> 接口  
  服务加载器  
  lambda表达式  
  代理  
  内部类  
  
## 6.1 接口
- **接口**（interface）用来描述类应该做什么，而不指定它们具体应该如何做。
- 一个类可以实现一个或多个接口。

### 6.1.1 接口的概念
- 接口不是类，而是对希望符合这个接口的类的一组需求。
- 实现接口使用关键字implements。

```java
// Comparable是一个接口
class Employee implements Comparable
```

### 6.1.2 接口的属性
- 接口不是类。具体来说，不能使用new运算符实例化一个接口。但是可以声明接口的变量，接口变量必须引用实现了这个接口的类对象：

```java
x = new Comparable(...); // ERROR
```

```java
Comparable x = new Employee(...); // OK provided Employee implements Comparable
```

### 6.1.3 接口与抽象类
- 使用抽象类表示通用属性存在一个严重的问题——每个类只能扩展一个类。

### 6.1.4 静态和私有方法
- 在**Java 8**中，允许在接口中增加静态方法。

### 6.1.5 接口与回调
- **回调**（callback）是一种常见的程序设计模式。在这种模式中，可以指定某个特定事件发生时应该采取的动作。

```java
import java.awt.*;
import java.awt.event.*;
import java,time.*;
import javax.swing.*;

public class TimerTest{
    public static void main(String[] args){
        var listener = new TimePrinter();
        // construct a timer that calls the listener
        // once every second
        var timer = new Timer(1000, listener);
        timer,start();
        

    }
}
```
### 6.1.6 对象克隆

```java
var original = new Employee("Lam", 50000);
Employee copy = original; // 本质上是同一个对象
copy.raiseSalary(10); // oops--also changed original
```
- 如果希望copy是一个新的对象，就需要使用**clone**方法。

```java
Employee copy = original.clone();
copy.raiseSalary(10); // OK--just copy changed
```

## 6.2 lambda表达式

### 6.2.1 为什么引入lambda表达式
- **lambda**表达式是一个可传递的代码块，可以在以后执行一次或多次。

### 6.2.2 lambda表达式的语法
- **lambda**表达式的一种形式：

```java
(String first, String second) -> 
{
    if(first.length() < second.length()) return -1;
    else if (first.length() > second.length()) return 1;
    else return 0;
}
```

- 如果一个lambda表达只在某些分支返回一个值，而另外一些分支不返回值，这是不合法的。例如，**(int x) -> { if (x >= 0) return 1; }**就不合法。

## 6.3 内部类
- 内部类是定义在另一个类中的类。
> 内部类可以对同一个包中的其他类隐藏。  
  内部类方法可以访问定义这个类的作用域中的数据，包括原本私有的数据。

***

# 第7章 异常、断言和日志
> 处理错误  
  使用断言  
  捕获异常  
  日志  
  使用异常的技巧  
  调试技巧  

## 7.1 处理错误
- 如果由于出现错误而使得某些操作没有完成，程序应该：
> 1. 返回到一种安全状态，并且能够让用户执行其他的命令；或者
> 2. 允许用户保存所有工作的结果，并且以妥善的方式终止程序。

- 错误类型：
> 1. 用户输入错误。
> 2. 设备错误。
> 3. 物理限制。
> 4. 代码错误。

### 7.1.1 异常分类

![image](/assets/img/post_img/Exception.png)

- 所有的异常都是由**Throwable**继承而来的，但在下一层立即分解为两个分支：**Error**和**Exception**。
- **Error**类层次结构描述了Java运行时系统的内部错误和资源耗尽错误。
- **Exception**类层次：
- 派生于RuntimeException的异常包括以下问题：
> 1. 错误的强制类型转换  
> 2. 数组访问越界  
> 3. 访问null指针

- 不是派生于RuntimeException的异常包括：
> 1. 试图超越文件末尾继续读取数据。  
> 2. 试图打开一个不存在的文件。
> 3. 试图根据给定的字符串查找Class对象，而这个字符串表示的类并不存在。

- Java语言规范将派生于**Error**类或**RuntimeException**类的所有异常称为**非检查型**（unchecked）异常，所有其他的异常称为**检查型**（checked）异常。

### 7.1.2 声明检查型异常
- 4种情况会抛出异常：
> 1. 调用了一个抛出检查型异常的方法，例如，**FileInputStream**构造器。
> 2. 检测到一个错误，并且利用throw语句抛出一个检查型异常。
> 3. 程序出现错误，例如，**a[-1] = 0**会抛出一个非检查型异常。
> 4. Java虚拟机或运行时库出现内部错误。

- 一个方法必须声明所有可能抛出的检查型异常，而非检查型异常要么在你的控制之外（**Error**），要么是由从一开始就应该避免的情况所导致的（**RuntimeException**）。
- 若超类方法没有抛出任何检查型异常，子类也不能抛出任何检查型异常。

### 7.1.3 如何抛出异常

```java
String readData(Scanner in) throws EOFException{
    ...
    while(...){
        if (!in.hasNext()) // EOF encountered
        {
            if (n < len)
                throw new EOFException();
        }
        ...
    }
    return s;
}
```

### 7.1.4 创建异常类
- 定义一个派生于**Exception**的类，或者派生于**Exception**的某个子类，如**IOException**。
- 自定义的异常类通常包含两个构造器，一个是默认的构造器，另一个是包含详细描述信息的构造器。

```java
class FileFormatException extends IOException{
    public FileFormatException() {
    
    }
    public FileFormatException(String gripe){
        super(gripe);
    }
}
```

- 现在，就可以抛出自定义的异常类型了。

```java
String readData(BufferedReader in) throws FileFormatException{
    ...
    while(...){
        if (ch == -1) // EOF encountered
        {
            if (n < len)
                throw new FileFormatException();
        }
        ...
    }
    return s;
}
```

## 7.2 捕获异常
### 7.2.1 捕获异常
- 捕获异常需要设置**try/catch**语句块。

```java
try {
    code
    more code
    more code
}
catch (ExceptionType e){
    handler for this type
}
```
- 若try语句块中的任何代码抛出了catch子句中指定的一个异常类，那么
1. 程序将跳过try语句块的其余代码。
2. 程序将执行catch子句中的处理器代码。

- 若try语句块中的代码没有抛出任何异常，那么程序将跳过catch语句。

### 7.2.2 捕获多个异常

```java
try {
    code that might throw exceptions
}
catch (FileNotFoundException e){
    emergency action for missing files
}
catch (IOException e){
    emergency action for all other I/O problems
}
...
```

- **e.getMessage()**得到详细的错误消息，**e.getClass().getName()**得到异常对象的实际类型。

### 7.2.3 再次抛出异常与异常链

```java
try {
    access the database
}
catch (SQLException e) {
    throw new ServletException("database error: " + e.getMessage());
}
```

### 7.2.4 finally子句
- 不管是否有异常被捕获，finally子句中的代码都会执行。

```java
var in = new FileInputStream(...);
try {
    // 1
    code that might throw exceptions
    // 2
}
catch (IOException e){
    // 3
    show error message
    // 4
}
finally {
    // 5
    in.close();
}
// 6
```

- 执行顺序：
1. 代码没有抛出异常。执行顺序为 1、2、5、6。
2. 代码抛出了一个异常，并在一个catch子句中捕获。  
    若catch子句没有抛出异常，程序将执行finally子句之后的第一条语句。执行顺序为 1、3、4、5、6。  
    若catch子句抛出了一个异常，异常将会被抛回到这个方法的调用者。执行顺序为 1、3、5。  
3. 代码抛出了一个异常，但是没有任何catch子句捕获这个异常。执行完finally子句中的语句后，会将异常抛回给这个方法的调用者。执行顺序为 1、5。

- 当try语句块和finally语句块中都有return语句时。利用return语句从try语句块中间退出。在方法返回前，会执行finally子句块。finally中的返回值会覆盖原来的返回值。

```java
public static int parseInt(String s) {
    try {
        return Integer.parseInt(s);
    }
    finally {
        return 0;
    }
}
// will return 0
```

### 7.2.5 分析堆栈轨迹元素
- **堆栈轨迹**（stack trace）是程序执行过程中某个特定点上所有挂起的方法调用的一个列表。

## 7.3 使用异常的技巧
> 1. 异常处理不能代替简单的测试。
> 2. 不要过分的细化异常。
> 3. 充分利用异常层次结构。
> 4. 不要压制异常。
> 5. 在检测错误时，“苛刻”要比放任好。
> 6. 不要羞于传递异常。

## 7.4 使用断言

### 7.4.1 断言的概念
- 断言机制允许在测试期间向代码中添加一些检查，而在生产代码中会自动删除这些检查。
- 关键字 **assert**。
- 断言x是一个非负数：assert x >= 0;  
  或者 assert x >= 0 : x; （将x的实际值传递给AssertionError对象，以便以后显示）

### 7.4.2 启用和禁用断言
- 在默认情况下，断言是禁用的。

### 7.4.3 使用断言完成参数检查
- 在Java语言中，给出了三种处理系统错误的机制：
> 抛出一个异常。  
  日志。  
  使用断言。

- 断言的使用
> 断言失败是致命的、不可恢复的错误。  
  断言检查只是在开发和测试阶段打开（“在靠近海岸的时候穿上救身衣，但在海里就把救生衣脱掉”）。

## 7.5 日志
- 每个Java程序员都很熟悉在有问题的代码中插入输出语句来观察程序的行为。找到问题的根源之后，就又将这些输出语句从代码中删去。日志API就是为了解决这个问题而设计的。

### 7.5.1 基本日志
- 使用**全局日志记录器**（global logger）并调用其**info**方法：

```java
Logger.getGlobal().info("File->Open menu item selected");

/* will print：

 May 10，2013 10:12:15 PM LoggingImageViewer fileOpen
 INFO: File->Open menu item selected
 
 */
```

### 7.5.2 高级日志
- 调用**getLogger**方法创建或获取日志记录器：

```java
private static final Logger myLogger = Logger.getLogger("com.mycompany.myapp");
```

- 日志级别：
> SEVERE  
  WARNING  
  INFO  
  CONFIG  
  FINE   
  FINER  
  FINEST  

- 在默认情况下，实际上只记录前3个级别。也可以设置一个不同的级别：

```java
logger.setlevel(Level.FINE); // FINE及所有更高级别的日志都会记录。
```

### 7.5.3 处理器
- 对于一个要记录的日志记录，它的日志级别必须高于日志记录器和处理器二者的阈值。

### 7.5.4 日志技巧
> 1. 对于一个简单的应用，选择一个日志记录器。
> 2. 默认的日志配置会把级别等于或高于INFO的所有消息记录到控制台。

***

# 第8章 泛型程序设计
> 限制与局限性  
  定义简单泛型类  
  泛型类型的继承规则  
  泛型方法  
  通配符类型

## 8.1 为什么要使用泛型程序设计
- 泛型程序设计（generic programming）意味着编写的代码可以对多种不同的类型对象重用。

### 8.1.1 类型参数的好处
- 泛型提供了一个更好的解决方案：类型参数（type parameter）。ArrayList类有一个类型参数用来指示元素的类型：

```java
var list = new ArrayList<String>();
```
### 8.1.2 谁想成为泛型程序员
- 利用**通配符类型**（wildcard type），构建类库的程序员可以编写出尽可能灵活的方法。

## 8.2 定义简单泛型类
- 泛型类（generic class）就是有一个或多个类型变量的类。

```java
public class Pair<T> {
    private T first;
    private T second;
    
    public Pair() { first = null; second = null;}
    public Pair(T first, T second) { this.first = first; this.second = second;}
    
    public T getFirst() { return first;}
    public T getSecond() { return second;}
    
    public void setFirst(T newValue) { first = newValue;}
    public void setSecond(T newValue) { second = newValue;}
}
```

## 8.3 泛型方法

```java
class ArrayAlg {
    public static <T> T getMiddle(T...a) {
        return a[a.length / 2];
    }
}
```

## 8.4 类型变量的限定

```java
public static <T extends Comparable> T min(T[] a)...
//尖括号中语句表示 限制T只能是实现了Comparable接口的类。
```

## 8.5 泛型代码和虚拟机
- 虚拟机没有泛型类型对象——所有对象都属于普通类。

***

# 第9章 集合
> Java集合框架  
  视图与包装器  
  集合框架中的接口  
  算法  
  具体集合  
  遗留的集合  
  映射  

## 9.1 Java集合框架
### 9.1.1 集合接口与实现分离
- 与现代的数据结构类库的常见做法一样，Java集合类库也将接口与实现分离。

### 9.1.2 Collection接口
- 在Java类库中，集合类的基本接口是Collection接口。

```java
public interface Collection<E> {
    boolean add(E element);
    Iterator<E> iterator();
    ...
}
```
- iterator方法用于返回一个实现了Iterator接口的对象。可以使用这个迭代器对象依次访问集合中的元素。

### 9.1.3 迭代器
- Iterator接口包含4个方法：

```java
public interface Iterator<E> {
    E next();
    boolean hasNext();
    void remove();
    default void forEachRemaining(Consumer<? super E> action);
}
```

## 9.2 集合框架中的接口

![image](/assets/img/post_img/Collection.png)

## 9.3 具体集合
### 9.3.1 链表
- 从数组中删除（或添加）一个元素开销很大，其原因是数组中后续的所有元素都要移动。
- 在Java程序设计语言中，所有链表实际上都是**双向链接**的——即每个链接还存放着其前驱的引用。

### 9.3.2 数组列表
- ArrayList封装了一个动态再分配的对象数组。

### 9.3.3 散列集
- **散列表**（hash table）可以用于快速地查找对象。
- 散列表为每个对象计算一个整数，称为**散列码**（hash code）。
- 在Java中，散列表用链表实现。每个列表被称为**桶**（bucket）。
- 查找表中对象的位置：先计算它的散列码，然后与桶的总数取余，所得到的结果就是保存这个元素的桶的索引。
- **散列冲突**（hash collision）：桶已经被填充的现象称为散列冲突。

### 9.3.4 树集
- 树集是一个**有序集合**（sorted collection）。
- 排序是用一个树数据结构完成的（当前使用的是红黑树（red-black tree）。每次将一个元素添加到树中时，都会将其放置在正确的排序位置上。

### 9.3.5 队列与双端队列
- **双端队列**（deuqe）允许在头部和尾部都高效地添加或删除元素。

### 9.3.6 优先队列
- **优先队列**（priority queue）中的元素可以按照任意的顺序插入，但会按照有序的顺序进行检索。

## 9.4 映射
- **映射**（map）用来存放键/值对。如果提供了键，就能够查找到值。

### 9.4.1 基本映射操作
- Java类库为映射提供了两个通用的实现：HashMap和TreeMap。这两个类都实现了Map接口。
- 散列映射对键进行散列，树映射根据键的顺序将元素组织为一个搜索树。散列或比较函数值应用于键。与键关联的值不进行散列或比较。

### 9.4.2 更新映射条目

```java
counts.put(word, counts.get(word) + 1);
// 第一次看到word时，get会返回null，会出现NullPointerException异常

/** 补救方法 1 
  * getOrDefault方法 
  * 若未在映射中找到这个键，
  * 则返回defaulValue。
  */
counts.put(word, counts.getOrDefault(word, 0) + 1);

/** 补救方法 2
  * 只有当键原先存在（或者映射到null）时，
  * 才会放入一个值。
  */
counts.putIfAbsent(word, 0);
counts.put(word, counts.get(word) + 1);

/** 补救方法 3
  * merge方法
  * 若键原先不存在，
  * word会与 1 关联，
  * 否则使用Integer::sum将原值与1求和。
  */
counts.merge(word, 1, Integer::sum);
```

### 9.4.3 映射视图
- 有3种视图：键集、值集合（不是一个集）以及键/值对集。

```java
Set<K> keySet() // return 键集

Collection<V> values() // return 值集合

Set<Map.Entry<K, V>> entrySet() // return 键/值对集
```

### 9.4.4 弱散列映射
- 假定对某个键的最后一个引用已经消失，那么不会再有任何途径可以引用这个值的对象了。由于程序中的任何部分不会再有这个键，所以，无法从映射中删除这个键/值对。
- 垃圾回收器会跟踪活动的对象。只要映射对象是活动的，其中所有桶也是活动的，所以不能被回收。
- **WeakHashMap**（弱散列映射）：当对键的唯一引用来自散列表映射条目时，这个数据结构将于垃圾回收器协同工作一起删除键/值对。
- **WeakHashMap**使用弱引用（weak references）保存键。

### 9.4.5 链接散列集与映射
- **LinkedHashSet**和**LinkedHashMap**类会记住插入元素项的顺序。这样可以避免散列表中的项看起来顺序是随机的。

### 9.4.6 枚举集与映射
- EnumSet是一个枚举类型的元素集的高效实现。
- 由于枚举类型只有有限个实例，所以EnumSet内部用位序列实现。如果对于的值在集中，则相应的位被置为1。

### 9.4.7 标识散列映射
- 类IdentityHashMap有特殊的用途。
- 在对两个对象进行比较时，IdentityHashMap类使用 == ，而不适用equals。也就是说，不同的键对象即使内容相同，也被视为不同的对象。

## 9.5 视图与包装器
### 9.5.1 小集合
- Java 9 引入了一些静态方法，可以生成给定元素的集或者列表，以及给定键/值对的映射。

```java
List<String> names = List.of("Peter", "Paul", "Mary");
Set<Integer> numbers = Set.of(2, 3, 5);
// 会分别生成包含3个元素的一个列表和一个集

Mao<String, Integer> scores = Map.of("Peter",2, "Paul",3, "Mary",5);
// 生成一个映射
```

- 元素、键或值不能为null。

### 9.5.2 子范围
- 可以为很多集合建力**子范围**（subrange）视图。

```java
List<Employee> group2 = staff.subList(10,20);
// subList方法与String类中的substring方法类似
```

### 9.5.3 不可修改的视图
- Collections类可以生成集合的**不可修改视图**（unmodifiable view）。

### 9.5.4 同步视图
- 若从多个线程访问集合，必须确保集合不会被意外地破坏。

```java
var map = Collections.synchronizeMap(new HashMap<String, Employee());
// Collections类的静态synchronizedMap方法可以将任何一个映射转换成有同步访问方法的Map
```

### 9.5.5 检查型视图
- **检查型视图**用来对泛型类型可能出现的问题提供调试支持。

## 9.6 算法
### 9.6.1 为什么使用泛型算法
- 泛型集合接口有一个很大的优点，即算法只需要实现一次。

### 9.6.2 排序与混排

```java
var staff = new LinkedList<String>();
fill collection
Collection.sort(staff);
// Collections类中的sort方法可以对实现了List接口的集合进行排序。
```

### 9.6.3 批操作

```java
coll1.removeAlL(coll2); // 从集合1中删除集合2中出现的所有元素

coll2.retainAll(coll2); // 从集合1中删除所有未在集合2中出现的元素
```

## 9.7 遗留的集合
### 9.7.1 属性映射
- **属性映射**（property map）是一个特殊类型的映射结构。它有下面3个特性：
> 1. 键与值都是字符串。
> 2. 这个映射可以很容易地保存到文件以及从文件加载。
> 3. 有一个二级表存放默认值。

### 9.7.2 位集
- Java平台的BitSet类用于存储一个位序列（他不是数学上的集，如果称为位向量或位数组可能更为合适）。

***

# 第10章 图形用户界面程序设计
- 略

***

# 第11章 Swing用户界面组件
- 略

***

# 第12章 并发
> 什么是线程  
  线程状态  
  线程属性  
  同步  
  线程安全的集合  
  任务和线程池  
  异步计算  
  进程  

- 每个任务在一个**线程**（thread）中执行，线程是控制线程的简称。
- 如果一个程序可以同时运行多个线程，则称这个程序是多线程的（multithreaded）。
- 多进程和多线程的本质区别：每个进程拥有自己一整套变量，而线程则共享数据。

## 12.1 什么是线程
- 线程（thread）是操作系统能够进行运算调度的最小单位。它被包含在进程之中，是进程中的实际运作单位。

## 12.2 线程状态
- 线程可以有如下6种状态：
> 1. New（新建）
> 2. Runnable（可运行）
> 3. Blocked（阻塞）
> 4. Waiting（等待）
> 5. Timed waiting（计时等待）
> 6. Terminated（终止）

### 12.2.1 新建线程
- 创建一个线程（如：new Thread(r)）时，程序还没有开始运行线程中的代码。在线程运行之前还有一些基础工作要做。

### 12.2.2 可运行线程
- 一旦调用**start**方法，线程就处于可运行状态。
- 一个可运行的线程可能**正在运行**也可能**没有运行**。
- 运行中的线程有时需要暂停，让其他线程有机会运行。
- **抢占式调度**：操作系统给每一个可运行线程一个时间片来执行任务。当时间片用完时，操作系统剥夺该线程的运行权，并给另一个线程一个机会来运行。
- 在有多个处理器的机器上，每一个处理器运行一个线程，可以有多个线程并行运行。当线程数目多于处理器数目时，调度器还是需要分配时间片。

### 12.2.3 阻塞和等待线程
- 当线程处于阻塞或等待状态时，不允许任何代码，消耗最少的资源。
- 要由线程调度器重新激活这个线程。

1. 当一个线程试图获取一个内部的对象锁，而这个锁目前被其他线程占有，该线程就会被阻塞。
2. 当线程等待另一个线程通知调度器出现一个条件时，这个线程就会进入等待状态。
3. 有几个方法有超时参数，调用这些方法会让线程进入计时等待（timed waiting）状态。

### 12.2.4 终止进程
- 线程会由于以下两个原因之一而终止：
1. run方法正常退出，线程自然终止。
2. 因为一个没有捕获的异常终止了run方法，使线程意外终止。

- 状态转换图：  
![image](/assets/img/post_img/Thread_State.png)

## 12.3 线程属性
### 12.3.1 中断线程
- 当线程的run方法执行方法体中最后一条语句后再执行return语句返回时，或者出现了方法中没有捕获的异常时，线程将终止。
- 当对一个线程调用interrupt方法时，就会设置线程的中断状态。
- 检测是否设置了中断状态，调用Thread.currentThread方法获得当前线程，然后调用isInterrupted方法：

```java
while(!Thread.currentThread().isInterrupted()) {
    do more work
}
```

- 没有任何语言要求被中断的线程应当终止。中断一个线程只是要引起它的注意。被中断的线程可以决定如何响应中断。
- interrupted方法和isInterrupted方法：
> interrupted方法是一个静态方法，它检查**当前线程**是否被中断，并且清除该线程的中断状态。  
  isInterrupted方法是一个实例方法，它见擦汗是否有线程被中断，不会改变中断状态。

### 12.3.2 守护线程
- 可以通过调用**t.setDaemon(true);**将一个线程转换为守护线程（daemon thread）。
- 守护线程的唯一用途是**为其他线程提供服务**。
- 当只剩下守护线程时，虚拟机就会退出。因为如果只剩下守护线程，就没必要继续运行程序了。

### 12.3.3 线程名
- 可以用setName方法为线程设置任何名字：

```java
var t = new Thread(runnable);
t.setName("Web crawler");
```

### 12.3.4 未捕获异常的处理器
- 线程的run方法不能抛出任何检查型异常，但是，非检查型异常可能会导致线程终止。在这种情况下，线程会死亡。
- 在线程死亡之前，异常会传递到一个用于处理**未捕获异常**的处理器。
- **ThreadGroup**类实现了**Thread.UncaughtExceptionHandler**接口。它的**uncaughtException**方法执行以下操作：
> 1. 如果该线程组有父线程组，那么调用父线程组的**uncaughtException**方法。
> 2. 否则，如果**Thread.getDefaultExceptionHandler**方法返回一个非null的处理器，则调用该处理器。
> 3. 否则，如果**Throwable**是**ThreadDeath**的一个实例，什么都不做。
> 4. 否则，将**线程的名字**以及**Throwable**的栈轨迹输出到**System.err**。

### 12.3.5 线程优先级
- 在Java程序设计语言中，每一个线程都有一个**优先级**。
- 一个线程会继承构造它的那个线程的优先级。

> MIN_PRIORITY: 1  
  MAX_PRIORITY: 10  
  NORM_PRIORITY: 5

- 在没有使用操作系统线程的Java早期版本中，线程优先级可能很有用，不过现在不要使用线程优先级了。

## 12.4 同步
- 两个或两个以上的线程需要共享对同一数据的存取，这两个线程会相互覆盖，可能导致对象被破坏。这种情况通常称为**竞态条件**（race condition）。

### 12.4.1 竞态条件的一个例子

```java
// Bank.java

package threads;

import java.util.Arrays;

public class Bank {
    private final double[] accounts;

    public Bank(int n, double initialBalance) {
        accounts = new double[n];
        Arrays.fill(accounts,initialBalance);
    }

    public void transfer(int from, int to, double amount){
        if(accounts[from]<amount) return;
        System.out.println(Thread.currentThread());
        accounts[from] -= amount;
        System.out.printf(" %10.2f from %d to %d", amount, from, to);
        accounts[to] += amount;
        System.out.printf(" Total Balance: %10.2f%n", getTotalBalance());
    }

    public double getTotalBalance() {
        double sum = 0;

        for (double a : accounts)
            sum += a;

        return sum;
    }

    public int size(){
        return accounts.length;
    }
}
```

```java
// UnsynchBankTest.java
package threads;

public class UnsynchBankTest {
    public static final int NACCOUNTS = 100;
    public static final double INITIAL_BALANCE = 1000;
    public static final double MAX_AMOUNT = 1000;
    public static final int DELAY = 10;

    public static void main(String[] args) {
        var bank = new Bank(NACCOUNTS, INITIAL_BALANCE);
        for (int i = 0; i < NACCOUNTS; i++) {
            int fromAccount = i;
            Runnable r = () -> {
                try {
                    while (true) {
                        int toAccount = (int) (bank.size() * Math.random());
                        double amount = MAX_AMOUNT * Math.random();
                        bank.transfer(fromAccount, toAccount, amount);
                        Thread.sleep((int) (DELAY * Math.random()));
                    }
                } catch (InterruptedException e) {

                }
            };
            var t = new Thread(r);
            t.start();
        }
    }
}
```

### 12.4.2 锁对象
- 有两种机制可以防止并发访问代码块。Java语言提供了一个**synchronized**关键字和**ReentrantLock**类。
- ReentrantLock保护代码块的基本结构：

```java
myLock.lock(); // a ReentrantLock object
try {
    crirical section
}
finally {
// unlock操作必须，否则，其他线程将永远阻塞
    myLock.unlock(); // make sure the lock is unlocked even if an exception is thrown
}
```

- 一旦一个线程锁定了锁对象，其他任何线程都无法通过lock语句。当其他线程调用lock时，它们会暂停，直到第一个线程释放这个锁对象。

- 使用锁来保护Bank类的transfer方法：

```java
public class Bank {
    ReentrantLock bankLock = new ReentrantLock();
    ...
    public void transfer(int from, int to, int amount) {
        bankLock.lock();
        try {
            System.out.print(Thread.currentThread());
            accounts[from] -= amount;
            System.out.printf(" %10.2f from %d to %d", amount, from, to);
            accounts[to] += amount;
            System.out.printf(" Total Balance: %10.2f%n", getTotalBalance());
        }
        finally {
            bankLock.unlock();
        }
    }
}
```

### 12.4.3 条件对象
- 考虑一个账户没有足够资金转出的情况：

```java
// 错误方式
if(bank.getBalance(from) >= amount) {
    // thread might be deactivated at this point
    bank.transfer(from, to, amount);
}

// 正确方式
public void transfer(int from, int to, int amount) {
    bankLock.lock();
    try {
        while(accounts[from] < amount) {
            // wait
            ...
        }
        // transfer funds
        ...
    }
    finally {
        bankLock.unlock();
    }
}
```
- 完整代码：

```java
package threads;

import java.util.Arrays;
import java.util.concurrent.locks.Condition;
import java.util.concurrent.locks.Lock;
import java.util.concurrent.locks.ReentrantLock;

public class Bank {
    private final double[] accounts;
    // ReentrantLock bankLock = new ReentrantLock();
    private Lock bankLock;
    private Condition sufficientFunds;

    public Bank(int n, double initialBalance) {
        accounts = new double[n];
        Arrays.fill(accounts,initialBalance);
        bankLock = new ReentrantLock();
        sufficientFunds = bankLock.newCondition(); // new一个条件对象
    }


    public void transfer(int from, int to, double amount) throws InterruptedException{
        bankLock.lock();
        try {
        /** 当发现资金不足，调用sufficientFunds.await();
          * 当前线程暂停，并放弃锁。
          * 这就允许另一个线程执行。
          */
            while(accounts[from] < amount)
                sufficientFunds.await();
            System.out.println(Thread.currentThread());
            accounts[from] -= amount;
            System.out.printf(" %10.2f from %d to %d", amount, from, to);
            accounts[to] += amount;
            System.out.printf(" Total Balance: %10.2f%n", getTotalBalance());
        /** 当另一个线程完成转账时，调用sufficientFunds.signalAll();
          * signalAll方法通知等待线程，
          * 现在有可能满足条件，值得再次检查。
          */
            sufficientFunds.signalAll();
        }
        finally {
            bankLock.unlock();
        }
    }

    public double getTotalBalance() {
        bankLock.lock();
        try{

        double sum = 0;

        for (double a : accounts)
            sum += a;

        return sum;
        }
        finally {
            bankLock.unlock();
        }

    }

    public int size(){
        return accounts.length;
    }
}
```

### 12.4.4 synchronized关键字
- **锁**和**条件**：
> 1. **锁**用来保护代码片段，一次只能有一个线程执行被保护的代码。
> 2. **锁**可以管理试图进入被保护代码段的线程。
> 3. 一个**锁**可以有**一个**或**多个**相关联的**条件对象**。
> 4. 每个**条件对象**管理那些已经进入被保护代码段但还不能运行的线程。

- synchronized关键字的使用：

```java
public synchronized void method() {
    method body
}
// 等价于
public void method() {
    this.intrinsicLock.lock();
    try {
        method body
    }
    finally {
        this.intrinsicLock.unlock();
    }
}
```

- 内部锁和条件存在一些限制。包括：
> 1. 不能中断一个正在尝试获得锁的线程。
> 2. 不能指定尝试获得锁时的超时时间。
> 3. 每个锁仅有一个条件可能是不够的。

- Lock和Condition对象 or 同步方法？
> 1. 最好两者都不使用。在许多情况下，可以使用java.util.concurrent包中的某种机制，它会为你处理所有的锁定。
> 2. 如果synchronized关键字适合程序，那么尽量使用这种做法，可以减少编写的代码量，并且降低出错的概率。
> 3. 如果特别需要Lock/Condition结构提供的额外能力，则使用Lock/Condition。

### 12.4.5 同步块
- 每一个Java对象都有一个锁。线程可以通过调用同步方法获得锁。还有另一种机制可以获得锁：即进入一个**同步块**。

```java
synchronized(obj) // this is the syntax for a synchronized block
{
    critical section
}
// 会获得obj的锁
```

### 12.4.6 监视器概念
- 锁和条件是实现线程同步的强大工具，但是，严格来讲，它们不是面向对象的。
- 监视器的特性：
> 1. 监视器是只包含私有字段的类。
> 2. 监视器类的每个对象有一个关联的锁。
> 3. 所有方法由这个锁锁定。
> 4. 锁可以有任意多个相关联的条件。

### 12.4.7 volatile字段
- volatile关键字为实例字段的同步访问提供了一种免锁机制。如果声明一个字段为volatile，那么编译器和虚拟机就知道该字段可能被另一个线程并发更新。
- 假设一个对象有一个boolean标记done，它的值由一个线程设置，而由另一个线程查询：

```java
// 1. 使用锁
private boolean done;
public synchronized boolean isDone() { return done; }
public synchronized bollean setDone() { done = true; }

// 2. 使用volatile字段
private volatile boolean done;
public boolean isDone() { return done; }
public void setDone() { done = true; }
```

### 12.4.8 final变量

```java
final var accounts = new HashMap<String, Double>();
/** 其他线程会在构造器完成构造之后才看到这个accounts变量。
  * 若不使用final，
  * 就无法保证其他线程看到的是accounts更新后的值，
  * 它们可能都只是看到null，而不是新构造的HashMap。
  */
```

### 12.4.9 原子性
- **原子性**就是指该操作是不可再分的。不论是多核还是单核，具有原子性的量，同一时刻只能有一个线程来对它进行操作。简而言之，在整个操作过程中不会被线程调度器中断的操作，都可认为是原子性。比如 a = 1；
- 若对共享变量除了赋值之外并不做其他操作，那么可以将这些共享变量声明为**volatile**。

### 12.4.10 死锁
- **死**锁是指两个或两个以上的进程在执行过程中，由于竞争资源或者由于彼此通信而造成的一种阻塞的现象，若无外力作用，它们都将无法推进下去。

```java
账户1： $200
账户2： $300
线程1： 从账户1转$300到账户2
线程2： 从账户2转$400到账户1
```

### 12.4.11 线程局部变量
- 避免共享变量，使用ThreadLocal辅助类为各个线程提供各自的实例。

### 12.4.12 为什么废弃stop和suspend方法
- stop方法天生就不安全，suspend方法经常会导致死锁。

## 12.5 线程安全的集合
### 12.5.1 阻塞队列
- 当试图向队列添加元素而队列已满，或是想从队列移出元素而队列为空的时候，**阻塞队列**（blocking queue）将导致线程阻塞。
- 队列会自动地平衡负载。如果第一组线程运行得比第二组慢，第二组在等待结果时会阻塞。如果第一组线程运行得更快，队列会填满，直到第二组赶上来。
- 阻塞队列方法

<table>
  <thead>
    <tr>
      <th>方法</th>
      <th>正常动作</th>
      <th>特殊情况下动作</th>
    </tr>
  </thead>
    <tbody>
    <tr>
      <td>add</td>
      <td>添加一个元素</td>
      <td>如果队列满，则抛出IllegalStateException异常</td>
    </tr>
    <tr>
      <td>element</td>
      <td>返回队头元素</td>
      <td>如果队列空，则抛出NoSuchElementException异常</td>
    </tr>
    <tr>
      <td>offer</td>
      <td>添加一个元素并返回true</td>
      <td>如果队列满，则返回false</td>
    </tr>
    <tr>
      <td>peek</td>
      <td>返回队头元素</td>
      <td>如果队列空，则返回null</td>
    </tr>
    <tr>
      <td>poll</td>
      <td>移除并返回队头元素</td>
      <td>如果队列空，则返回null</td>
    </tr>
    <tr>
      <td>put</td>
      <td>添加一个元素</td>
      <td>如果队列满，则阻塞</td>
    </tr>
    <tr>
      <td>remove</td>
      <td>移除并返回队头元素</td>
      <td>如果队列空，则抛出NoSuchElementException异常</td>
    </tr>
    <tr>
      <td>take</td>
      <td>移除并返回队头元素</td>
      <td>如果队列空，则阻塞</td>
    </tr>
  </tbody>
</table>

### 12.5.2 高效的映射、集和队列
- java.util.concurrent包提供了映射、有序集和队列的高效实现：ConcurrentHashMap、ConcurrentSkipListMap、ConcurrentSkipListSet和ConcurrentLinkedQueue。
- 这些集合使用复杂的算法，通过允许并发地访问数据结构的不同部分尽可能减少竞争。
- 这些类的size方法不一定在常量时间内完成操作。确定这些集合当前的大小通常需要遍历。

### 12.5.3 映射条目的原子更新
- 调用compute方法时可以提供一个键和一个计算新值的函数。

```java
// 1
map.compute(word, (k, v) -> v == null ? 1 ：v + 1);

// 2 
map.merge(word, 1L, (existingValue, new Value) -> existingValue + newValue);
// or  map.merge(word, 1L, Long::sum);
```

### 12.5.4 对并发散列映射的批操作
- 有3种不同的操作：

> 1. search（搜索）为每个键或值应用一个函数，直到函数生成一个非null的结果。然后搜索终止，返回这个函数的结果。
> 2. reduce（规约）组合所有键或值，这里要使用所提供的一个累加函数。
> 3. forEach为所有键或值应用一个函数。

- 每个操作都有4个版本：
> 1. operationKeys：处理键。
> 2. operationValues：处理值。
> 3. operation：处理键和值。
> 4. operationEntries：处理Map.Entry对象。

- 对于上述各个操作，需要指定一个**参数化阈值**（parallelism threshold）。如果映射包含的元素多余这个阈值，就会并行完成批操作。如果希望批操作在一个线程中运行，可以使用阈值**Long.MAX_VALUE**。如果希望用尽可能多的线程运行批操作，可以使用阈值**1**。

### 12.5.5 并发集视图
- keySet方法

```java
// keySet方法可以生成一个映射的键集
Set<String> words = map.keySet(1L);
words.add("Java");
// 如果“Java”在words中不存在，现在它会有一个值1。
```

### 12.5.6 写数组拷贝
- **CopyOnWriteArrayList**和**CopyOnWriteArraySet**是线程安全的集合，其中所有更改器会建立底层数组的一个副本。

### 12.5.7 并行数组算法
- Arrays类提供了大量并行化操作。静态Arrays.parallelSort方法可以对一个基本类型值或对象的数组排序。

### 12.5.8 较早的线程安全集合
- 任何集合类都可以通过使用**同步包装器**（synchronization wrapper）变成线程安全的：

```java
List<E> synchArrayList = Collections.synchronizedList(new ArrayList<E>())；
Map<K, V> synchHashMap = Collections.synchronizedMap(new HashMap<K, V>());
```

## 12.6 任务和线程池
- 线程池中包含许多准备运行的线程，为线程提供一个Runnable，就会有一个线程调用run方法。当run方法退出时，这个线程不会死亡，而是留在池中为下一个请求提供服务。

### 12.6.1 Callable与Future
- Runnable封装一个异步运行的任务，可以把它想象成一个没有参数和返回值的异步方法。Callable与Runnable类似，但是有返回值。

```java
public interface Callable<V> {
    V call() throws Exception;
}
```

- Future保存异步计算的结果。

### 12.6.2 执行器
- **执行器**（Executors）类有许多静态工厂方法，用来构造线程池。

<table>
  <thead>
    <tr>
      <th>方法</th>
      <th>描述</th>
    </tr>
  </thead>
    <tbody>
    <tr>
      <td>newCachedThreadPool</td>
      <td>必要时创建线程；空闲线程会保留60秒</td>
    </tr>
    <tr>
      <td>newFixedThreadPool</td>
      <td>池中包含固定数目的线程；空闲线程会一直保留</td>
    </tr>
    <tr>
      <td>newWorkStealingPool</td>
      <td>一种适合“fork-join”任务的线程池，其中复杂的任务会分解为更简单的任务，空闲线程会“密取”较简单的任务</td>
    </tr>
    <tr>
      <td>newSingleThreadExecutor</td>
      <td>只有一个线程的“池”，会顺序地执行所提交的任务</td>
    </tr>
    <tr>
      <td>newScheduledThreadPool</td>
      <td>用于调度执行的固定线程池</td>
    </tr>
    <tr>
      <td>newSingleThreadScheduledExecutor</td>
      <td>用于调度执行的单线程“池”</td>
    </tr>
  </tbody>
</table>

### 12.6.3 控制任务组
- invokeAny方法提交一个Callable对象集合中的所有对象，并返回某个已完成任务的结果。

### 12.6.4 fork-join框架
- 假设有一个处理任务，它可以很自然地分解为子任务，如下所示：

```java
if (problemSize < threshold) {
    solve problem directly
}
else {
    break problem into subproblems
    recursively solve each subproblem
    combine the results
}
```

```java
class Counter extends RecursiveTask<Integer> {
    ...
    protected Integer compute() {
        if (to - from < THRESHOLD) {
            solve problem directly
        }
        else {
            int mid = (from + to) / 2;
            var first = new Counter(values, from, mid, filter);
            var second = new Counter(values, mid, to, filter);
            invokeAll(first, second);
            return first.join() + second.join();
        }
    }
}
/** invokeAll方法接收到很多任务并阻塞，
  * 直到所有这些任务全部完成。
  * join方法将生成结果。
  * 对每个子任务调用join，
  * 并返回其总合。
  */
```

- 在后台，fork-join框架使用了一种有效的智能方法来平衡可用线程的工作负载，这种方法称为**工作密取**（work stealing）。

## 12.7 异步计算
### 12.7.1 可完成Future
- CompletableFuture类实现了Future接口，它提供了获得结果的另一种机制。注册一个**回调**，一旦结果可用，就会（在某个线程中）利用该结果调用这个回调。

```java
CompletableFuture<String> f = ...;
f.thenAccept(s -> Process the result string s);
```

## 12.8 进程
- Process类在一个单独的操作系统进程中执行一个命令，允许与标准输入、输出和错误流交互。
- ProcessBuilder类则允许配置Process对象。

### 12.8.1 建立一个进程
- 首先指定想要执行的命令。可以提供一个List<String>，或者直接提供命令字符串。

```java
var builder = new ProcessBuilder("gcc", "myapp.c");
```

### 12.8.2 运行一个进程
- 配置了构建器之后，要调用start方法启动进程。

### 12.8.3 进程句柄
- 要获得程序启动的一个进程的更多信息，或者想更多地了解计算机上正在运行的任何其他进程，可以使用ProcessHandle接口。可以用4种方式得到一个ProcessHandle：
> 1. 给定一个Process对象p，p.toHandle()会生成它的ProcessHandle。
> 2. 给定一个long类型的操作系统进程ID，ProcessHandle.of(id)可以生成这个进程的句柄。
> 3. Process.current()是运行这个Java虚拟机的进程的句柄。
> 4. ProcessHandle.allProcesses()可以生成对当前进程可见的所有操作系统进程的Stream<ProcessHandle>。

- 给定一个进程句柄，可以得到它的进程ID、父进程、子进程和后代进程：

```java
long pid = handle.pid();
Optional<ProcessHandle> parent = handle.parent();
Stream<ProcessHandle> children = handle.children();
Stream<ProcessHandle> descendants = handle.descedants();
```

## 12.9 线程补充
- 多线程的创建方式：

```java
/** 方式1 继承于Thread类
  */ 
package threads;
/**
 *
 * 创建三个窗口卖票，总票数为100张，使用继承自Thread方式
 * 用静态变量保证三个线程的数据独一份
 *
 * 存在线程的安全问题，有待解决
 *
 * */

public class ThreadDemo extends Thread{

    public static void main(String[] args){
        Window t1 = new Window();
        Window t2 = new Window();
        Window t3 = new Window();

        t1.setName("售票口1");
        t2.setName("售票口2");
        t3.setName("售票口3");

        t1.start();
        t2.start();
        t3.start();
    }

}

class Window extends Thread{
    private static int ticket = 100; //将其加载在类的静态区，所有线程共享该静态变量

    @Override
    public void run() {
        while(true){
            if(ticket>0){
                //                try {
                //                    sleep(100);
                //                } catch (InterruptedException e) {
                //                    e.printStackTrace();
                //                }
                System.out.println(getName()+"当前售出第"+ticket+"张票");
                ticket--;
            }else{
                break;
            }
        }
    }
}
```

```java
/** 方式2 实现Runable接口方式
  */
package threads;

public class ThreadDemo1 {
    public static  void main(String[] args){
        Window1 w = new Window1();

        //虽然有三个线程，但是只有一个窗口类实现的Runnable方法，由于三个线程共用一个window对象，所以自动共用100张票

        Thread t1=new Thread(w);
        Thread t2=new Thread(w);
        Thread t3=new Thread(w);

        t1.setName("窗口1");
        t2.setName("窗口2");
        t3.setName("窗口3");

        t1.start();
        t2.start();
        t3.start();
    }
}

class Window1 implements Runnable{
    private int ticket = 100;

    @Override
    public void run() {
        while(true){
            if(ticket>0){
                //                try {
                //                    sleep(100);
                //                } catch (InterruptedException e) {
                //                    e.printStackTrace();
                //                }
                System.out.println(Thread.currentThread().getName()+"当前售出第"+ticket+"张票");
                ticket--;
            }else{
                break;
            }
        }
    }
}
```

```java
/** 方式3 实现callable接口方式
  */
package threads;


import java.util.concurrent.Callable;
import java.util.concurrent.ExecutionException;
import java.util.concurrent.FutureTask;

/**
 * 创建线程的方式三：实现callable接口。---JDK 5.0新增
 * 是否多线程？否，就一个线程
 *
 * 比runable多一个FutureTask类，用来接收call方法的返回值。
 * 适用于需要从线程中接收返回值的形式
 *
 * //callable实现新建线程的步骤：
 * 1.创建一个实现callable的实现类
 * 2.实现call方法，将此线程需要执行的操作声明在call（）中
 * 3.创建callable实现类的对象
 * 4.将callable接口实现类的对象作为传递到FutureTask的构造器中，创建FutureTask的对象
 * 5.将FutureTask的对象作为参数传递到Thread类的构造器中，创建Thread对象，并调用start方法启动（通过FutureTask的对象调用方法get获取线程中的call的返回值）
 *
 * */

//实现callable接口的call方法
class NumThread implements Callable{

    private int sum=0;//

    //可以抛出异常
    @Override
    public Object call() throws Exception {
        for(int i = 0;i<=100;i++){
            if(i % 2 == 0){
                System.out.println(Thread.currentThread().getName()+":"+i);
                sum += i;
            }
        }
        return sum;
    }
}

public class ThreadNew {

    public static void main(String[] args){
        //new一个实现callable接口的对象
        NumThread numThread = new NumThread();

        //通过futureTask对象的get方法来接收futureTask的值
        FutureTask futureTask = new FutureTask(numThread);

        Thread t1 = new Thread(futureTask);
        t1.setName("线程1");
        t1.start();

        try {
            //get返回值即为FutureTask构造器参数callable实现类重写的call的返回值
            Object sum = futureTask.get();
            System.out.println(Thread.currentThread().getName()+":"+sum);
        } catch (ExecutionException e) {
            e.printStackTrace();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
    }
}
```

```java
/** 方式4 使用线程池的方式
  */
package threads;

import java.util.concurrent.ExecutorService;
import java.util.concurrent.Executors;
/**
 * 创建线程的方式四：使用线程池（批量使用线程）
 *1.需要创建实现runnable或者callable接口方式的对象
 * 2.创建executorservice线程池
 * 3.将创建好的实现了runnable接口类的对象放入executorService对象的execute方法中执行。
 * 4.关闭线程池
 *
 * */
class NumberThread implements Runnable{
    @Override
    public void run() {
        for(int i = 0;i<=100;i++){
            if (i % 2 ==0 )
                System.out.println(Thread.currentThread().getName()+":"+i);
        }
    }
}

class NumberThread1 implements Runnable{
    @Override
    public void run() {
        for(int i = 0;i<100; i++){
            if(i%2==1){
                System.out.println(Thread.currentThread().getName()+":"+i);
            }
        }
    }
}

public class ThreadPool {

    public static void main(String[] args){

        //创建固定线程个数为十个的线程池
        ExecutorService executorService = Executors.newFixedThreadPool(10);

        //new一个Runnable接口的对象
        NumberThread number = new NumberThread();
        NumberThread1 number1 = new NumberThread1();

        //执行线程,最多十个
        executorService.execute(number1);
        executorService.execute(number);//适合适用于Runnable

        //executorService.submit();//适合使用于Callable
        //关闭线程池
        executorService.shutdown();
    }

}
```

***
