---
title:  使用@media媒体查询定义常用移动端设备
subtitle: 持续补充中
date: 2/22/2017 3:54:58 PM  
comments: true
tags: 
	- 前端
	- 媒体查询
	- media
	- 移动设备
categories: 前端开发
author:
  nick: 元宝
  github_name: shenxiaai

---


**iPhone 4 only**
```
@media (max-width: 320px) {
	/* iPhone 4 only */
}
```


**iPhone 5 only**
```
	@media only screen and (min-device-width: 560px) and (max-device-width: 1136px) and (-webkit-min-device-pixel-ratio: 2) {
	    /* iPhone 5 only */
	}
```