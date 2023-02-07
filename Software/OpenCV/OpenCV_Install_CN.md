# 如何在CoolPI-4B上安装OpenCV

[English](./OpenCV_Install.md) | 简体中文

## 简介

Opencv是计算机视觉的必备第三方库之一。
我们通常使用它对图片进行处理。
原生的Opencv无法直接调用RK3588的硬件解码功能，因此对输入数据进行解码时会占用比较大的CPU资源。
我们可以考虑使用Opencv + GStreamer来解决这个问题。

## 安装过程

下面以OpenCV-3.4.16为例子教你安装带GStreamer的插件的OpenCV。
在安装前请检查你是否正确安装了GStreamer。

```bash
sudo apt install libgtk2.0-dev
cd opencv-4.5.0
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=RELEASE \
      -DWITH_GSTREAMER=ON \
      -DBUILD_DOCS=OFF \
      -DBUILD_EXAMPLES=OFF \
      -DBUILD_TESTS=OFF \
      -DBUILD_PERF_TESTS=OFF \
      -DCMAKE_INSTALL_PREFIX=${PWD}/opencv \
      ..
make -j8     
make install
```

## 其他资源

* [GStreamer的安装](../GStreamer/GStreamer_Install_CN.md)