---
title: 博客建立记 ——hexo错误解释
tags: 博客建成
categories: 技术
banner_img: /img/1.png
index_img: /img/1.png
abbrlink: 14554
date: 2023-04-29 14:50:25
updated: 2023-04-29 16:01:08
---
## 明明安装了ssl密钥，但显示为添加
1.重新获取密钥
```cmd
	ssh-keygen -t rsa "你的邮箱"
	cat id_rsa.pub
```
第一行获取ssh，第二行查看
2.在GitHub两种模式都试试
3.关闭steam++等加速器，同类型的同理为什么显示无法连接仓库
## 仓库连接不成功
1.检查是不是仓库地址
注：不是pages地址，是仓库地址
2.网址后加点git
3.网络问题，多试几次

前文说了，不能用steam++，不然会显示没有ssl密钥
## 为什么弄完了依旧404
原因有很多，但重点
1.2020/10/1之后默认分支改成了main，所以分支要改
2.GitHub pages 没有开启 可以去仓库设置打开，记得选择从分支创建
3.仓库格式不是 用户名+github.io，这样的话，你的地址其实是，用户名+github.io/仓库名.io
可以重新创建仓库