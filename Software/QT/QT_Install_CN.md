# 如何在CoolPI-4B上安装QT

[English](./QT_Install.md) | 简体中文

在CoolPI-4B上安装QT时，如果你安装的操作系统的版本不同，那么你的安装过程也会有所不同。
请根据你的系统版本选择对应的安装步骤。

## Ubuntu 20.04之前

```Bash
sudo apt-get install build-essential
sudo apt-get install libgl1-mesa-dev
sudo apt-get install cmake 
sudo apt-get install qt5-default qtcreator
sudo apt-get install qt5*
```

## Ubuntu 20.04之后

```Bash
sudo apt-get install build-essential
sudo apt-get install libgl1-mesa-dev
sudo apt-get install cmake 
sudo apt-get install qtbase5-dev qtchooser qt5-qmake qtbase5-dev-tools
sudo apt-get install qtcreator
sudo apt-get install qt5*
```