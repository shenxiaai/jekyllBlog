---
title:  使用Koa2
subtitle: 
date: 3/14/2017 2:16:27 PM 
comments: true
tags: 
	- 前端
	- Koa2
	- Node
categories: 前端开发
author:
  nick: 元宝
  github_name: shenxiaai

---

元宝君以前用过node的Express框架，最近听说Koa最近大热，似有超越Express之势，所以今天本君试试用Koa2搭建一个Web项目。

跟Express的上手套路一样，从“Hello World！”开始。

# 自定义方式

## 安装koa

```
	node install -g koa(或node install koa --save)
```

## 新建一个app.js文件：

```
	var koa = require('koa');
	var app = new koa();
	
	app.use(function *(){
	  this.body = 'Hello World';
	});
	
	app.listen(3000);
	console.log('Koa app started at port 3000...');
```

> 其实Koa框架已经用ES6啦，这里为了好理解还是用的ES5，后面会慢慢开始用ES6。

## 在控制台运行app.js:

```
	node app.js
```

## 运行结果：

**控制台：**

![](/assets/images/img4.jpg)

**页面上：**

![](/assets/images/img5.jpg)

# 使用koa应用生成器

使用Express时有express-generator，用koa时也有koa-generator。

## 安装koa-generator

```
	npm install -g koa-generator（或npm install koa-generator --save）
```

然后使用koa命令创建koa 1.x项目

然后使用koa2命令创建koa 2.x项目

## 新建myKoa文件夹

```
	mkdir myKoa
	koa2 myKoa
	cd myKoa
	npm install
	npm start
```

**运行结果：**

![](/assets/images/img6.jpg)

![](/assets/images/img8.jpg)

![](/assets/images/img9.jpg)

![](/assets/images/img10.jpg)
