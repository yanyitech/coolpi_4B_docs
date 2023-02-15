[English](./README.md) | 简体中文

# Coolpi已适配FastDeploy

## 简介

[FastDeploy](https://github.com/PaddlePaddle/FastDeploy) 是一款全场景、易用灵活、极致高效的AI推理部署工具， 支持云边端部署。提供超过 160+ Text，Vision， Speech和跨模态模型开箱即用的部署体验，并实现端到端的推理性能优化。包括 物体检测、字符识别（OCR）、人脸、人像扣图、多目标跟踪系统、NLP、Stable Difussion文图生成、TTS 等几十种任务场景，满足开发者多场景、多硬件、多平台的产业部署需求。
我们花费了很多时间来适配它. 
我们适配的模型能够应用在 Detection, Face Detection, Face Recognition, Face Alignment, Segmentation, OCR 等领域. 
这些模型将极大的提升CoolPI开发版在边缘计算领域的能力


## 模型列表

为了方便开发者们使用模型，我们提供了模型速度一览表，你可以快速的查到模型在CoolPI-4B上的速度。

|Task|Model Name|Model Version|Whether to Quantify|RKNN Speed(ms)|
|-|-|-|-|-|
|Classification|ResNet|ResNet50_vd|No|33|
|Detection|Picodet|Picodet-s|No|112|
|Detection|PaddleDetection Yolov8|yolov8-n|No|100|
|Detection|PPYOLOE|ppyoloe-s|Yes|141|
|Detection|RKYOLOV5|YOLOV5-S-Relu|Yes|57|
|Detection|RKYOLOX|yolox-s|Yes|130|
|Detection|RKYOLOV7|yolov7-tiny|Yes|58|
|Segmentation|Unet|Unet-cityscapes|No|-|
|Segmentation|PP-HumanSegV2Lite|portrait|Yes|43|
|Segmentation|PP-HumanSegV2Lite|human|Yes|43|
|Face Detection|SCRFD|SCRFD-2.5G-kps-640|Yes|42|
|Face FaceRecognition|InsightFace|ms1mv3_arcface_r18|Yes|12|


## Demo

- [Face Detection with SCRFD](https://cool-pi.com/topic/173/do-face-detection-on-coolpi-with-fastdeploy)
- [Face Recognition with ArcFace](https://cool-pi.com/topic/174/do-face-recognition-on-coolpi-with-fastdeploy)
- [Try to deploy YOLOv5 on coolpi](https://cool-pi.com/topic/205/try-to-deploy-yolov5-on-coolpi)


## 致谢

感谢百度团队提供了这么好的工具让大家使用.

## 导航

* [CoolPI论坛](https://www.cool-pi.com): 如果你需要获取实时的信息并与全球的开发者们交流，请加入我们。
* [Issues](https://github.com/yanyitech/coolpi_4B_docs/issues): 如果你有其他想法，请在这里讨论。
* * [FastDeploy Github](https://github.com/PaddlePaddle/FastDeploy) 