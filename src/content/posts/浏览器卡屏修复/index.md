---
title: 浏览器卡屏/切换页面卡住问题修复
published: 2025-10-27
pinned: false
description: 浏览器切换页面上半部分卡死，只有下半部分正常显示
tags: [疑难杂解]
category: 疑难杂解
author: Nth2Miss
draft: false
---



**此问题已在 Windows 11 Canary build 27959 已彻底修复该问题**

![3](./images/3.png)




# 方法一：下载注册表文件，双击直接导入注册表，然后重启即可


<a href="/files/浏览器卡屏修复.reg" download>浏览器卡屏修复.reg</a>

[//]: # (<a href="https://nth2miss.lanzoue.com/iUthI39gx0ob" target="_blank">浏览器卡屏修复.reg</a>)

<br>

# 方法二：手动操作



按下Win+R，输入regedit，打开 注册表

![](./images/0.png)

打开之后定位到 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\Dwm

![](./images/1.png)



右侧空白部分，右键 > 新建DWORD > 命名为OverlayTestMode

双击OverlayTestMode，设置值为5，十六进制

![2](./images/2.png)



然后重启电脑即可。



