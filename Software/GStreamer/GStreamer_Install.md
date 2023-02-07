# How to install GStreamer

## Introduce

GStreamer is an open source multimedia framework used to build streaming media applications. Its goal is to simplify the development of audio/video applications. It has been used to process multimedia data in multiple formats such as MP3, Ogg, MPEG1, MPEG2, AVI, Quicktime, etc.

## Installation process of GStreamer

### Install GStreamer basic library

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

### Install the GStreamer Rockchip third-party library

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
