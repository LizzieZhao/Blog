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

廖雪峰大神的教程导图。

![Javascript 思维导图](/img/in-posts/javascript_01.png)

---

## 正文

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



