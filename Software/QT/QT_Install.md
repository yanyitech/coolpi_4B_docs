# How to install QT on CoolPI-4B

English | [简体中文](./QT_Install_CN.md)


When installing QT on CoolPI-4B, if you install different versions of the operating system, your installation process will also be different.

## Before Ubuntu 20.04

```Bash
sudo apt-get install build-essential
sudo apt-get install libgl1-mesa-dev
sudo apt-get install cmake 
sudo apt-get install qt5-default qtcreator
sudo apt-get install qt5*
```

## After Ubuntu 20.04

```Bash
sudo apt-get install build-essential
sudo apt-get install libgl1-mesa-dev
sudo apt-get install cmake 
sudo apt-get install qtbase5-dev qtchooser qt5-qmake qtbase5-dev-tools
sudo apt-get install qtcreator
sudo apt-get install qt5*
```