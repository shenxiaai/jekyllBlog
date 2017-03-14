---
title:  ife斌斌JS笔记（持续更新中）
subtitle: JS学习笔记
date: 3/2/2017 2:57:40 PM 
comments: true
categories: 笔记
author:
  nick: 元宝
  github_name: shenxiaai

---

> 3/2/2017 2:57:49 PM

## 任务四：基础JavaScript练习（一）

![](../assets/images/img11.png)

html布局

```
	<input id="ipt" type="text" name="">
	<button id="leftIn">左侧入</button>
	<button id="rightIn">右侧入</button>
	<button id="leftOut">左侧出</button>
	<button id="rightOut">右侧出</button>

	<ul id="list">
	</ul>
```

list是添加后的数据存放的盒子

![](../assets/images/img12.png)

js代码

```
	var list = document.querySelector('#list')；

	//点击list中元素删除此元素
	list.addEventListener('click', function (event) {
		var _this = event.target;
		listArr.splice(_this.ind, 1);
		exaggerate();
	});
```

此时，事件不是绑定在list里面的li上，而是绑定在父级list上。click事件的默认参数event的target属性可以找到父元素list中哪个元素被点击到了。


#### event.target

**target** 事件属性可返回事件的目标节点（触发该事件的节点），如生成事件的元素、文档或窗口，即返回哪个 DOM 元素触发了事件。

event.currentTarget指向事件所绑定的元素，而event.target始终指向事件发生时的元素。