---
layout:     post
title:      Vimba C++ API 实现 MFC ActiveX OCX 控件并在 VB/C# 等应用程序中使用
subtitle:   使用Vimba C++ API异步调用方法进行图像获取，并用于 ActiveX OCX 实现
date:       2019-06-14
author:     Joe Ge
header-img: img/vimba-sdk-banner2.png
catalog: true
tags:
    - SDK
    - ActiveX
    - OCX
    - C++
---

## 简介
为了在MFC ActiveX OCX 控件中实现Vimba C++采图功能，需要使用如下软件：
1. Vimba SDK 2.1.3(或者最新版本)
2. Visual Studio Community 2017(或者类似版本)

## ActiveX OCX 控件
实现代码及工程文件下载：[`MFCActiveXControl2.zip`](../resources/vimbacpp-mfc-activex-ocx-implementation/MFCActiveXControl2.zip)   

使用了Vimba C++ API 中异步取图功能，在相机是固定帧率，自由采集及硬件触发时此控件会实时显示收到的相机图像。

## 在VB/C#等使用OCX控件
测试C#代码及工程文件下载：[`ActivX-OCX-CSharp-Test.zip`](../resources/vimbacpp-mfc-activex-ocx-implementation/ActivX-OCX-CSharp-Test.zip)   

将上述生成的ActiveX OCX控件应用于C# Forms应用中。运行此程序时，系统上的第一个Allied Vision相机将实时显示它的图片在这个控件上。


## 实现效果
此空间可以实时显示相机传来的图片并显示，如下图，FPS是每秒显示的图片数量。

![](/resources/vimbacpp-mfc-activex-ocx-implementation/screenshot.png)  

动态运行效果图： 

![](/resources/vimbacpp-mfc-activex-ocx-implementation/vimba-activex-ocx-for-CSharp.gif)


