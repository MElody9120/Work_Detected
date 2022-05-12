
# ncnn-android-nanodet

---

Android Real-time video stream detect By using NanoDet model based on NCNN framework

---

1. 基于 [**NCNN 框架**](https://github.com/Tencent/ncnn) 结合 [**OpenCV--Android**](https://github.com/nihui/opencv-mobile) 实现模型在安卓端的部署与实现
2. 模型采用  **YOLO思路**  下基于安卓与嵌入式特别开发的开源模型 [**NanoDet**](https://github.com/RangiLyu/nanodet)


## 一些介绍

---

模型文件存储在```/app/src/main/assets```

链接库采用```<project dir>/app/src/main/jni/CMakeLists.txt```中CMakeLists进行链接

图形界面采用 ```JAVAFX``` 框架

整体工程文件采用 ```build.gradle``` 进行构建

此为模型部署，故没有**Python**部分内容 ，整体项目框架所采用的语言为```C```与```JAVA```

摄像头ID控制，为采用`camera_facing`参数作为参数开关，若需更改，请全局搜索项目文件，更改`camera_facing`变量即可实现更改所需要的控制摄像头

1. `facing = 1 `为开启前置摄像头
2. `facing = 0 `为开启后置摄像头

本项目需要调用`Camera2 API`,对摄像头硬件参数有要求，不能为`legacy`等级


## 更新日志 Update Log

---

### 5-11-2022 Master

#### 概述
1. 实现了获取并输出内部识别数据流的情况
2. 数据流情况可由`logcat`工具从`Android日志中获取`
3. 初步实现结构获取与数据分析算法设计
4. 摄像头部分在安卓板中仍有无法获取情况，初步判断与摄像头设置参数有关

Author : Melody

### 5-5-2022 Master

#### 概述
1. 尝试进行向下版本兼容失败，```Run```
2. 要求设备版本型号```Android >= 9.0```
3. 修改了一些```gradle```配置，增添一部分注释

Author : Melody

### 4-27-2022 Master

#### 概述
1. 修改文件，因为空间影响删除```APP/Build/Output/Debug```
2. 增添一部分注释
3. 添加```Log4J```部分内容

Author : Melody


### 4-24-2022  Master

#### 概述

1. 增添README.md
2. 模型文件调整

Author ： Melody