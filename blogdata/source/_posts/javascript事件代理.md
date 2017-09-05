---
title: javascript事件代理（事件委托）
categories: javascript
---
事件委托一直没有整明白，今天有时间了想起来了就研究一下，看到了一篇博文，深入浅出，写的不错，为了备忘，在此再总结一下。原博文地址：http://www.cnblogs.com/liugang-vip/p/5616484.html
事件委托即事件代理，主要是为了通过减少dom操作，减少占用内存进而优化网站性能。
<!-- more -->
方法

通过target方法来获取事件源。但是是有兼容性的：标准浏览器用e.target,IE浏览器用e.srcElement。
通过target.nodeName获取标签名（大写的）。
