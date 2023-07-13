---
title: hexo博客fruid主题加评论教程
tags: 博客
categories: 技术
comments: true
banner_img: /img/1.png
index_img: /img/1.png
abbrlink: 37247
date: 2023-04-30 10:34:28
---
## 一、安装
### 1. 看看你的主题支持哪些评论系统
我用的是fruid，支持
```
Valine (opens new window):基于 LeanCloud
Waline (opens new window): 从 Valine 衍生而来，额外增加了服务端和多种功能
Gitalk (opens new window): 基于 GitHub Issues
Utterances (opens new window): 基于 GitHub Issues
Disqus (opens new window): 基于第三方的服务
畅言 (opens new window): 基于第三方的服务
来必力(Livere) (opens new window): 基于第三方的服务
Remark42 (opens new window): 需要自托管服务端
Twikoo (opens new window): 基于腾讯云开发
Cusdis (opens new window): 基于第三方服务或自托管服务
Giscus (opens new window): 基于 GitHub Discussion
```
### 2.选择评论系统
在国内要选择不被墙的
我选择来必力，它是来自韩国的评论系统
## 二、接入
### 1.注册
到
```
https://www.livere.com/
```
注册账号
### 2.获取uid
在管理页面选择安装，选择免费的，点击普通网站安装，它会出示一段代码，把uid后的数字复制下来
## 三、主题配置
在主题配置里添加
```
post:
  comments:
    enable: true
    type: livere
livere:
	uid:xxxxxxxxxxxxx
```
就完成了