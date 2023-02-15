English | [简体中文](./README_CN.md)

# Coolpi has been adapted to FastDeploy

## Brief Introduction

[FastDeploy](https://github.com/PaddlePaddle/FastDeploy) is an easy-to-use and high performance AI model deployment toolkit for Cloud, Mobile and Edge with out-of-the-box and unified experience, end-to-end optimization for over 150+ Text, Vision, Speech and Cross-modal AI models. Including image classification, object detection, image segmentation, face detection, face recognition, keypoint detection, matting, OCR, NLP, TTS and other tasks to meet developers' industrial deployment needs for multi-scenario, multi-hardware and multi-platform.

We spent a lot of time on the adaptation of FastDeploy for Coolpi. The model we have adapted can be used in Detection, Face Detection, Face Recognition, Face Alignment, Segmentation, OCR and other fields. These models will greatly improve Coolpi's ability in edge computing.

## Model List

In order to facilitate you to choose a reasonable model to apply to your project, we have provided the running speed of the model.

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


## Contribution

Thanks to Baidu FastDeploy team for making such a good tool so that we can easily deploy AI model.

## 导航

* [CoolPI论坛](https://www.cool-pi.com): If you need to get real-time information and communicate with developers around the world, please join us.
* [Issues](https://github.com/yanyitech/coolpi_4B_docs/issues): If you have other ideas, please discuss them here.
* [FastDeploy Github](https://github.com/PaddlePaddle/FastDeploy) 