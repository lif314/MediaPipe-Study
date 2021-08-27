# MediaPipe Pose

1. [Overview](https://google.github.io/mediapipe/solutions/pose.html#overview)
2. [ML Pipeline](https://google.github.io/mediapipe/solutions/pose.html#ml-pipeline)
3. [Pose Estimation Quality](https://google.github.io/mediapipe/solutions/pose.html#pose-estimation-quality)
4. Models
   1. [Person/pose Detection Model (BlazePose Detector)](https://google.github.io/mediapipe/solutions/pose.html#personpose-detection-model-blazepose-detector)
   2. [Pose Landmark Model (BlazePose GHUM 3D)](https://google.github.io/mediapipe/solutions/pose.html#pose-landmark-model-blazepose-ghum-3d)
5. Solution APIs
   1. Cross-platform Configuration Options
      1. [static_image_mode](https://google.github.io/mediapipe/solutions/pose.html#static_image_mode)
      2. [model_complexity](https://google.github.io/mediapipe/solutions/pose.html#model_complexity)
      3. [smooth_landmarks](https://google.github.io/mediapipe/solutions/pose.html#smooth_landmarks)
      4. [min_detection_confidence](https://google.github.io/mediapipe/solutions/pose.html#min_detection_confidence)
      5. [min_tracking_confidence](https://google.github.io/mediapipe/solutions/pose.html#min_tracking_confidence)
   2. Output
      1. [pose_landmarks](https://google.github.io/mediapipe/solutions/pose.html#pose_landmarks)
      2. [pose_world_landmarks](https://google.github.io/mediapipe/solutions/pose.html#pose_world_landmarks)
   3. [Python Solution API](https://google.github.io/mediapipe/solutions/pose.html#python-solution-api)
   4. [JavaScript Solution API](https://google.github.io/mediapipe/solutions/pose.html#javascript-solution-api)
6. Example Apps
   1. Mobile
      1. [Main Example](https://google.github.io/mediapipe/solutions/pose.html#main-example)
   2. Desktop
      1. [Main Example](https://google.github.io/mediapipe/solutions/pose.html#main-example-1)
7. [Resources](https://google.github.io/mediapipe/solutions/pose.html#resources)



## Overview

Human pose estimation from video plays a critical role in various applications such as [quantifying physical exercises](https://google.github.io/mediapipe/solutions/pose_classification.html), sign language recognition, and full-body gesture control. For example, it can form the basis for yoga, dance, and fitness applications. It can also enable the overlay of digital content and information on top of the physical world in augmented reality.

quantifying physical exercises   ---- 量化体育锻炼

full-body gesture control ---- 全身手势控制

 augmented reality  --- 增强现实

**应用：**

- 构成瑜伽、舞蹈和健身应用的基础
- 在增强现实中将数字内容和信息叠加在物理世界之上。

MediaPipe Pose is a ML solution for high-fidelity body pose tracking, inferring 33 3D landmarks on the whole body from RGB video frames utilizing our [BlazePose](https://ai.googleblog.com/2020/08/on-device-real-time-body-pose-tracking.html) research that also powers the [ML Kit Pose Detection API](https://developers.google.com/ml-kit/vision/pose-detection). Current state-of-the-art approaches rely primarily on powerful desktop environments for inference, whereas our method achieves real-time performance on most modern [mobile phones](https://google.github.io/mediapipe/solutions/pose.html#mobile), [desktops/laptops](https://google.github.io/mediapipe/solutions/pose.html#desktop), in [python](https://google.github.io/mediapipe/solutions/pose.html#python-solution-api) and even on the [web](https://google.github.io/mediapipe/solutions/pose.html#javascript-solution-api).

high-fidelity ---- 高保真

utilize --- 利用

MediaPipe Pose 是一种用于**高保真**身体姿势跟踪的 ML 解决方案，利用我们的 BlazePose 研究从 RGB 视频帧推断全身 33 个 3D 地标，该研究也为 ML Kit 姿势检测 API 提供支持。当前最先进的方法主要依赖于强大的桌面环境进行推理，而我们的方法在大多数现代手机、台式机/笔记本电脑、python 甚至网络上实现了实时性能。

[ML Kit介绍：](https://developers.google.com/ml-kit)

ML Kit是一个强大易用的工具包，它将谷歌在机器学习方面的专业知识带给了普通的移动应用开发者。

- 针对移动设备进行 了优化

- 由Google专业知识构建

- 全面而且易于使用 --- 你可以使用现有的解决方案（基于API），也可以使用自己的算法模型。你可以根据需要选择是离线还是在线使用。

- 基于API，无缝的将机器学习嵌入到你的APP中

  - 图像打标，可以识别图像中的物体，位置，活动形式，动物种类，商品等等。

  - 文本识别，从图像中识别并提取文字。

  - 人脸检测，检测人脸和人脸的关键点。

  - 条码扫描，扫描和处理条码。

  - 地标识别，在图像中识别比较知名的地标。

  - 智能回复（即将上线），提供符合上下文语境的文字回答。

- 定制模型  ----- 如果MK的Base API中没有包括你需要的使用场景，那么你可以使用你自己的基于TF Lite的算法模型。只需要上传你的模型，我们会负责模型的管理和使用。



## ML Pipeline



































