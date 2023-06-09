# 谷歌用新功能升级 ARCore API，让用户沉浸其中

> 原文：<https://www.xda-developers.com/ar-core-raw-depth-api-recording-api-google-io-2021/>

在谷歌 I/O 2021 上，谷歌宣布对该公司的增强现实平台 ARCore 进行一些重要升级，该平台为全球超过 8.5 亿部安卓智能手机提供动力。与需要专门硬件的 Project Tango 不同，ARCore 依靠手机现有的硬件和传感器来收集深度、运动跟踪和光线估计的数据，以帮助开发人员建立交互式 AR 体验。

自推出以来，谷歌一直在稳步改善 ARCore 的功能集和功能，推动增强现实应用开发者利用 Android 智能手机现有硬件所能完成的极限。去年，谷歌[发布了 arCore Depth API](https://www.xda-developers.com/google-arcore-depth-api-public-launch/) ，允许开发人员仅使用单个 RGB 相机来生成深度图，并创建更真实的 AR 体验。如今，该公司正在为 ARCore 的军火库添加两个新工具:Raw Depth API 和录音回放 API。

## ARCore 原始深度 API

新的原始深度 API 建立在[深度 API](https://developers.google.com/ar/develop/java/depth/overview) 的基础上，通过生成具有相应置信度图像的原始深度图来提供周围物体的更详细的表示。虽然深度 API 专注于生成具有所有像素的深度估计的平滑深度图，但 Raw 深度 API 旨在捕捉具有置信度图像的更真实的深度图，从而提供每像素深度估计。

另一个改进领域是点击测试，现在使用深度图而不是平面来提供更多的点击测试结果，即使在非平面和低纹理地板上。TeamViewer 的 LifeAR 应用程序利用深度点击测试将 AR 功能集成到视频通话中。

这些新的改进不需要飞行时间(ToF)传感器等专用硬件，因此可以在绝大多数 ARCore 认证的设备上实施。从今天开始，开发人员可以使用原始深度 API 和深度命中测试。

## ARCore 记录和回放 API

除了新的 Raw Depth API，谷歌还在 ARCore 中推出了一个新的录制和播放 API，让应用程序开发人员在测试不同的 AR 体验时有更大的灵活性。在构建新的 AR 体验时，开发人员往往需要在特定的环境和场所中不断进行测试。借助新的录制和播放 API，开发人员现在可以录制带有深度和 IMU 运动传感器数据等 AR 元数据的视频镜头，并使用它来重建相同的环境以进行进一步测试。这里的想法是记录一次镜头，并将其作为模板来测试其他 AR 效果和体验，而不是每次都拍摄新的镜头。打车应用滴滴顺风车使用该 API 在其应用中构建和测试 AR 驱动的方向，并在 R&D 上节省了 25%的成本，并将开发周期缩短了 6 个月。

对于最终用户，录制和回放 API 还支持新的增强现实体验，如后期捕捉增强现实。这使得用户可以将之前录制的视频馈送到 AR 应用程序，从而无需亲临现场进行实时摄像。换句话说，用户可以一次拍摄镜头，稍后添加 AR 效果。ARCore 录音和回放 API 从今天开始对开发者开放，你可以在[这个页面](https://developers.google.com/ar/develop/java/recording-and-playback)上了解更多信息。