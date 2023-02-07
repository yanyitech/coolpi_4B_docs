# How to install OpenCV on CoolPI-4B

English | [简体中文](./OpenCV_Install_CN.md)

## Introduce

Opencv is one of the necessary third-party libraries for computer vision. 
We usually use it to process images.
The native Opencv cannot directly call the hardware decoding function of RK3588, so decoding the input data will take up a lot of CPU resources.
We can consider using Opencv+GStreamer to solve this problem.

## Installation process

Take OpenCV-3.4.16 as an example to teach you to install OpenCV with GStreamer plug-in. 
Please check whether you have installed GStreamer correctly before installation.

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

## Navigation

* [Installation of GStreamer](../GStreamer/GStreamer_Install.md)