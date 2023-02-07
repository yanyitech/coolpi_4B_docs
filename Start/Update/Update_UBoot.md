# CoolPI-4B Update UBoot

English | [简体中文](./Update_UBoot_CN.md)

## Introduce

In the process of product iteration, we will upgrade UBoot. If the old equipment is not updated in time, we may miss some new features.
This document will teach you how to upgrade UBoot.

## Download upgrade firmware package

Before you start upgrading UBoot, you need to download our latest firmware package.
We provide two ways (Baidu Netdisk and Onedrive) for developers to download the upgrade firmware package. You can reach our download address through the following link:

* [Baidu Netdisk](https://pan.baidu.com/s/1QV7RyMLqqK70ugYMxcXnbQ?pwd=qg2f): `coolpicoolpi/loader/RKDevTool_Release_v2.92_loader0104.zip`
* [Onedrive](https://coolpi-my.sharepoint.com/:f:/g/personal/coolpi_coolpi_onmicrosoft_com/EuWQQ9Cxt0pKs2-UxgJjFFABVwsC916i49ZcjPIxM9wq8w?e=DFiNvC): `coolpi-4b/loader/RKDevTool_Release_v2.92_loader0104.zip`

## Update firmware package

After downloading the firmware package, please follow the following steps to update your UBoot firmware:

* Connect `MASKROM` and `GND`.
  ![](https://www.cool-pi.com/assets/uploads/files/1673498091109-484cb5bd-12d1-48ed-87f6-0756e04cc019-image.png)
* Connect USB and computer. Note that USB2USB data cable should be used here.
  ![](https://www.cool-pi.com/assets/uploads/files/1673498333264-2cd71480-ce1c-422c-acb2-501d266d276e-image.png)
* Power on will automatically enter the burning mode. The software will prompt `发现一个MASKROM设备`
  ![](https://www.cool-pi.com/assets/uploads/files/1673498473100-5ab7434e-30a8-4e2d-aa7e-8d613d21256f-image.png)
* Tick `强制按地址写`
  ![](https://www.cool-pi.com/assets/uploads/files/1673498587285-96f556fc-ab5d-4c4e-a808-b4ca035d4268-image.png)
* Click `执行`
  ![](https://www.cool-pi.com/assets/uploads/files/1673498676194-909c4f7c-b55a-4e2a-9c5b-af56d097eb01-image.png)

## 可能发生的错误

If you have short-circuited 'MASKROM' and 'GND', but the software does not prompt`发现一个MASKROM设备`，it means that you have not installed the driver.
Please go to the website for downloading firmware. There is `DriverAssistant` under the' usb driver `DriverAssitant_v5.12.zip` file, please unzip and install this driver.
