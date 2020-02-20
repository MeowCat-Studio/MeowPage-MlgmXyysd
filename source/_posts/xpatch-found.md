---
title: 找到了合适的 Xposed 框架
date: 2019-12-20 09:07:51
id: '<%= page.date %>'
tags: 
- Xposed
- 随笔
- 原创
- Android
- 技术笔记
---
最近发现了一个新的（貌似是我火星了）开源 Xposed 框架：

[Xpatch: 免Root实现App加载Xposed插件的一种方案](https://windysha.github.io/2019/04/18/Xpatch-%E5%85%8DRoot%E5%AE%9E%E7%8E%B0App%E5%8A%A0%E8%BD%BDXposed%E6%8F%92%E4%BB%B6%E7%9A%84%E4%B8%80%E7%A7%8D%E6%96%B9%E6%A1%88/)

<!--more-->
源码: [https://github.com/WindySha/Xpatch](https://github.com/WindySha/Xpatch)

和众多免 root 的 Xposed 框架原理类似，都是在 App 中插入 Appllication，让 App 在运行时执行加载模块的操作，需要修改 app

加载模块的源码：[https://github.com/WindySha/xposed_module_loader](https://github.com/WindySha/xposed_module_loader)

这样一来就可以开搞之前说的那个"[安全问题](http://mlgmxyysd.meowcat.org/2019/11/02/new-xposed-security-problem/)"了