name: byte-code.md
time: 2024/6/5 Wed
title: Design Pattern byte code

# Byte Code Game Design Pattern (字节码模式)

## 定义
将整个逻辑的一部分脚本化或数据化，通过虚拟机或者解释器来执行的一种方式方法。将代码数据化脚本化的这种行为模式，就称作是 **字节码模式**。

## 使用场景
- 在需要经常变动的地方，可以避免每次都重新编译整个项目
- 或者需要提供给别人一些接口，但是又不想把整个源代码暴露出来
- 在游戏开发中，经常用在技能系统，剧情对白系统

## 优缺点
#### 优点
1. 一定程度上的解耦
1. 提高了灵活性，使得一部分逻辑数据化，降低了硬编码的概率
2. 实现了数据驱动（Data Driver），使得代码逻辑清晰易读

#### 缺点
1. 需要实现一个虚拟机或者解释器，算是一个不小的工作量
1. 提高了灵活性的同时，项目复杂度也跟着提高了
1. 通常情况下，实现字节码的脚本或数据配置，有一定的学习门槛


## 使用案例



## 相关文章和链接
- 一本不错的游戏编程模式书，作者放出了电子版[游戏编程模式](http://gameprogrammingpatterns.com/bytecode.html) 
- “四人帮”写的那本《设计模式》
- 一本神书，讲解如何从零开始写一个虚拟机[游戏脚本高级编程](https://book.douban.com/subject/1927405/)
- 