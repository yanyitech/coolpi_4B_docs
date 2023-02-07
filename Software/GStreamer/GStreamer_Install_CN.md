# 如何安装GStreamer

## 简介

GStreamer 是用来构建流媒体应用的开源多媒体框架(framework)，其目标是要简化音/视频应用程序的开发，已经能够被用来处理像 MP3、Ogg、MPEG1、MPEG2、AVI、Quicktime 等多种格式的多媒体数据。

## 安装GStreamer的过程

### 安装GStreamer基础库

```bash
sudo apt-get install libgstreamer1.0-0 \
                      gstreamer1.0-plugins-base \
                      gstreamer1.0-plugins-good \
                      gstreamer1.0-plugins-bad \
                      gstreamer1.0-plugins-ugly \
                      libgstreamer-plugins-bad1.0-dev \
                      gstreamer1.0-nice \
                      gstreamer1.0-libav \
                      gstreamer1.0-tools \
                      gstreamer1.0-x \
                      gstreamer1.0-alsa \
                      gstreamer1.0-gl \
                      gstreamer1.0-gtk3 \
                      gstreamer1.0-qt5 \
                      gstreamer1.0-pulseaudio \
                      libgstreamer1.0-dev \
                      libgstreamer-plugins-base1.0-dev \
                      gstreamer1.0-tools
```

### 安装GStreamer Rockchip第三方库

```bash
sudo apt-get install build-essential
sudo apt-get install libgl1-mesa-dev
sudo apt-get install meson
sudo apt-get install rockchip-mpp
sudo apt-get install rockchip-mpp-dev
sudo apt-get install librga-dev
sudo apt-get install rockchip-rga
sudo apt-get install rockchip-rga-dev
sudo apt-get install librga2
sudo apt-get install gstreamer1.0-rockchip1 
```

