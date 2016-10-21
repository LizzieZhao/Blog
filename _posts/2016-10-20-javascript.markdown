---
layout:     post
title:      "JavaScript 主要内容整理"
subtitle:   "参考廖雪峰大神的 Javascript 教程，然后自己做出的思维导图"
date:       2016-10-20 08:00:00
author:     "Lina"
header-img: "img/post-bg-javascript.jpg"
catalog: true
tags:
    -
---

> “脱贫比脱单更重要，太特么穷了！！！”


## 前言

最近看各种大神们写的组件的代码，发现好多方法都不知道是干什么的。

果然 Javascript 需要好好打基础。

首先，就从廖雪峰大神的教程开始好了。。。

本来想上传一张思维导图，但是发现分支太多太大了，所以图片不是很清楚。所以就放弃好了。

附上廖雪峰大神的教程地址 [JavaScript教程](http://www.liaoxuefeng.com/wiki/001434446689867b27157e896e74d51a89c25cc8b43bdb3000)


---

## 正文

以下是在学习过程中发现的有(bu)趣(hui)的小知识：

1. 用 map 和 reduce 实现把一个字符串转变成 Number。
```javascript
    function string2int(s) {
      return s.split('').map( function(x){ return x-0 } ).reduce( function(x,y){ return x*10+y } );
    }
```

2. 用 map 实现把不规范的英文名字，变为首字母大写，其他小写的规范名字。例如输入：['adam', 'LISA', 'barT']，输出：['Adam', 'Lisa', 'Bart']。
```javascript
    function normalize(arr) {
      return arr.map( function(x){ let tail = x.substring(1).toLowerCase(); let head = x[0].toUpperCase(); return tail+head;});
    }
```

3. 用 map 把数组内的字符串转变为 Number。
```javascript
    function array2int(arr) {
      return arr.map( function(x){ return +x } );
    }
```

---

## 后记

> ＂每次只培养一个习惯＂



