# BFM模型可视化工具 - C++

通过C++和Qt5构建的一个Basel人脸模型（Basel Face Model, BFM）的可视化工具。

<img src="https://github.com/Great-Keith/bfm-visual-tool/raw/master/assets/avg_v2.0.gif" width="80%">



## 功能介绍

### 生成随机人脸

设置`random range` 后的滑动条，可以调节随机程度（正态分布的方差），0.0时为平均脸。

设置完成之后点击下方按钮即可在左侧生成随机人脸。

### 设置PC权重

可以修改面部Shape、Texture和Expr的PC权重，BFM共有199个PC可以在左侧下拉栏中选择，右测滑动条调节数值大小，调节完成后点击对应的按钮完成设置。

*[NOTE] 修改PC权重需要在已经生成人脸的前提下使用*

### 将生成人脸存储到文件

目前支持的文件格式仅有PLY格式，可以通过MeshLab打开进行查看。



## 其他功能

### 预然人脸操作

该部分通过Qt5内置OpenGL实现，支持按键如下：

* 鼠标左键：长按后可以拖拉旋转人脸；
* 鼠标滚轮：缩放；
* 键盘A/W/S/D：向左转/放大/向右转/缩小。

