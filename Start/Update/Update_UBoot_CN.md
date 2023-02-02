# CoolPI-4B 升级UBoot

[English](./Update_UBoot.md) | 简体中文

## 简介

在产品不断迭代的过程中我们会对UBoot进行升级，如果旧设备没有得到及时的更新，可能会错过一些新的特性。
这个文档将教会你如何升级UBoot。

## 下载升级固件包

在开始升级UBoot之前你需要下载我们最新的固件包。
我们提供了两种方式（百度网盘和Onedrive）让开发者下载升级固件包，你可以通过以下链接到达我们的下载地址:

* [百度网盘](https://pan.baidu.com/s/1QV7RyMLqqK70ugYMxcXnbQ?pwd=qg2f): `coolpicoolpi/loader/RKDevTool_Release_v2.92_loader0104.zip`
* [Onedrive](https://coolpi-my.sharepoint.com/:f:/g/personal/coolpi_coolpi_onmicrosoft_com/EuWQQ9Cxt0pKs2-UxgJjFFABVwsC916i49ZcjPIxM9wq8w?e=DFiNvC): `coolpi-4b/loader/RKDevTool_Release_v2.92_loader0104.zip`

## 更新固件包

下载完固件包后请按照以下步骤更新你的UBoot固件:

* 把`MASKROM`和`GND`连接。
  ![](https://www.cool-pi.com/assets/uploads/files/1673498091109-484cb5bd-12d1-48ed-87f6-0756e04cc019-image.png)
* 连接USB和电脑，注意这里要使用USB2USB的数据线
  ![](https://www.cool-pi.com/assets/uploads/files/1673498333264-2cd71480-ce1c-422c-acb2-501d266d276e-image.png)
* 上电将自动进入烧写模式。软件将出现提示 `发现一个MASKROM设备`
  ![](https://www.cool-pi.com/assets/uploads/files/1673498473100-5ab7434e-30a8-4e2d-aa7e-8d613d21256f-image.png)
* 勾选 `强制按地址写`
  ![](https://www.cool-pi.com/assets/uploads/files/1673498587285-96f556fc-ab5d-4c4e-a808-b4ca035d4268-image.png)
* 点击 `执行`
  ![](https://www.cool-pi.com/assets/uploads/files/1673498676194-909c4f7c-b55a-4e2a-9c5b-af56d097eb01-image.png)

## 可能发生的错误

如果你已经短接了`MASKROM`和`GND`，但是软件没有提示`发现一个MASKROM设备`，这说明你没有安装驱动。
请进入下载固件的网址，在`usb driver`目录下有`DriverAssitant_v5.12.zip`文件，请解压并且安装这个驱动。
