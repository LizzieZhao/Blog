---
layout:     post
title:      "工作项目总结"
subtitle:   " \"Work Summary\""
date:       2016-11-20 08:00:00
author:     "Lina"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - 工作
    - Node
    - Webpack
    - React
    - Ajax
---

> “When you wake up in the morning you have two choices: go back to sleep, or wake up and chase those dreams.”


## 前言

不能再每天糊里糊涂的做项目了，要把这个项目中遇见的问题和学到的知识总结下来。    

Come on ！！！

---

## 正文

### 2016/11/21
1. Node安装完毕，却在使用时候报错：“node is not a command”,同时在 cmd 中也启动不了 Node。但是检查发现 Node 确实安装成功了。
**原因：** 一般情况上，如果默认 Node 的安装路径，一般都会安装在 C 盘，此时，系统会默认把这个路径添加系统环境变量。但是如果是自定义位置安装，系统添加的默认路径有可能就是错误的。这个时候检查系统环境变量的 Path 路径，大多会有以下两个问题：1. 根本没有 Node 这个安装路径；2. 路径显示错误，可能多一个'/'。

2. React 中，如果想给组件添加一个自定义属性，并且想获取这个自定义属性值应该怎么办。
**办法：** event.target.getAttribute('props')      
现在还没有在项目中使用，所以具体不做介绍。    

3. XMLHttpRequest.abort()   撤销上传文件。
**总结：** 这是 Ajax 中的一个方法，即使现在的项目中使用的都是 fetch，也要明白 fetch 也是在 ajax 的基础上进行改造的。所以要重视 Ajax。

4. cannot find module reactDom
**问题：** 这是同事在编译项目的时候出现的问题，但是没有找到问题所在，当时的解决方法是直接返回到初始源文件。     
初步查看资料是因为 webpack 的文件写法有问题。等自己遇到这个问题要把它解决了。

5. blob
**认识：** 这是 FormData 中的一种。没有用到，只是在看别人代码中遇见了。应该明天会用到这个。到时候再做处理。



---

## 后记

> ＂Yesterday, you said tomorrow＂
