# ncnn-android-nanodet

---

Android Real-time video stream detect By using NanoDet model based on NCNN framework

---

1. 基于 [**NCNN 框架**]() 结合 [**OpenCV--Android**](https://github.com/nihui/opencv-mobile) 实现模型在安卓端的部署与实现
2. 模型采用  **YOLO思路**  下基于安卓与嵌入式特别开发的开源模型 [**NanoDet**](https://github.com/RangiLyu/nanodet)


## 一些介绍

---

模型文件存储在```/app/src/main/assets```

链接库采用```<project dir>/app/src/main/jni/CMakeLists.txt```中CMakeLists进行链接

图形界面采用 ```JAVAFX``` 框架

整体工程文件采用 ```build.gradle``` 进行构建

此为模型部署，故没有**Python**部分内容 ，整体项目框架所采用的语言为```C```与```JAVA```



## 更新日志 Update Log

---

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





