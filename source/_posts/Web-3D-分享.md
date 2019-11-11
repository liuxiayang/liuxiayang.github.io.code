---
title: Web 3D 分享
catalog: true
date: 2019-10-18 17:04:17
subtitle:
header-img:
tags:
- Skill
- Notes
---

### 基本概念
#### OpenGL与WebGL
&emsp;&emsp;&nbsp;&nbsp;关于2维3维计算机图形技术、Khronos Group对各种技术进行了标准化并制定了[OpenGL]、作为Windows、Mac、Linux上的一种跨平台技术并一直活跃着。Khronos Group把这样的OpenGL技术运用到WEB浏览器并制定了WebGL。WebGL 是 OpenGL 和 JavaScript 之间的结晶、HTML5 的 canvas 元素里、利用和OpenGL同样的API、可以绘制高精度的三维图像。
&emsp;&emsp;关于WebGL的中需要注意的是、浏览器要支持WebGL、电脑中安装的图形显示卡中的OpenGL的版本必须要是2.0以上。

一句话总结:WebGL是在浏览器中实现三维效果的一套规范。

#### THREE.JS
&emsp;&emsp;&nbsp;&nbsp;2009年末、Giles发表了使用WebGL的入门向导文章「Learning WebGL」、WebGL的使用方法变得更加容易理解了。虽说通过WebGL的绘制效果甚至可能达到本地的高性能游戏专用机的绘制效果，但如果没有非常精通OpenGL的人在还是不太现实的。因此，为了能够更加简单的利用WebGL，库「Three.js」被发表了。因为 Three.js 非常好用，所以很快变得非常有人气。WebGL的javascript框架除了Three.js之外，还有「J3D」和「SceneJS」和日本开发的「gl.enchant.js」等。

### 用到的API

视图
perspective:视点到显示器的距离，默认none。
perspective-origin:试点在应用元素的位置，默认中心。

THREE.Camera
创建一个新的Camera。注意：这个类并不是被直接调用的；你所想要的或许是一个 OrthographicCamera（正交摄像机）或者 PerspectiveCamera（透视摄像机）。
OrthographicCamera( left : Number, right : Number, top : Number, bottom : Number, near : Number, far : Number )
left — 摄像机视锥体左侧面。
right — 摄像机视锥体右侧面。
top — 摄像机视锥体上侧面。
bottom — 摄像机视锥体下侧面。
near — 摄像机视锥体近端面。
far — 摄像机视锥体远端面。

![随手一截](OrthographicCamera.jpg)

PerspectiveCamera( fov : Number, aspect : Number, near : Number, far : Number )
fov — 摄像机视锥体垂直视野角度
aspect — 摄像机视锥体长宽比
near — 摄像机视锥体近端面
far — 摄像机视锥体远端面

![随手一截](PerspectiveCamera.jpg)

这些参数一起定义了摄像机的viewing frustum（视锥体）。

camera.position:相机位置
camera.lookAt:相机朝向位置
camera.up:相机顶部位置

场景

光源

模型与贴图

### 画个地球
requestAnimationFrame()

### 全景看房

### 粒子特效
#### canvas
getImageData()
![data](https://www.kkkk1000.com/images/getImgData/getImgDatadata.jpg)
### 三体水滴

### 一些特效
腾讯
https://wa.qq.com/xplan/earth/index.html?_wv=1
http://up.qq.com/act/a20170301pre/index.html#u
跑车游戏 http://hexgl.bkcore.com/
