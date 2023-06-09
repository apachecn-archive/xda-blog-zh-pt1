# ARCore 1.23 增加了对改进的深度图的双摄像头支持

> 原文：<https://www.xda-developers.com/google-arcore-1-23-dual-camera-depth-map/>

# 谷歌的增强现实 API 将很快使用两个摄像头来制作更好的深度地图

谷歌正在推出 ARCore SDK 版本，该版本在 Pixel 4 等受支持的设备上添加了对深度 API 的双摄像头支持。

ARCore 是谷歌用于创建增强现实应用的 SDK，它不需要专门的硬件来工作，不像谷歌失败的 Project Tango 实验。您的手机只需要一个 RGB 摄像头、一个提供精确陀螺仪和加速度计读数的 IMU 传感器，以及大量校准数据。使用这些基本的传感器和一个摄像头，ARCore 的[深度 API 可以创建深度图](https://www.xda-developers.com/google-arcore-depth-api-create-depth-maps-using-single-camera/)，以实现诸如遮挡、更真实的物理、路径规划、表面交互等功能。虽然单个摄像头已经令人印象深刻，但如果你能引入另一个摄像头，这种体验将更加身临其境。这似乎正是谷歌计划在其最新版本的增强现实 SDK 中做的事情。

使用 ARCore 的深度 API 使用单个 RGB 相机创建遮挡。来源:谷歌

正如 [*AndroidPolice*](https://www.androidpolice.com/2021/03/01/googles-about-to-enhance-ar-performance-by-taking-advantage-of-your-phones-dual-cameras/) 所指出的，ARCore SDK 版本的变更日志提到了“支持设备上的双摄像头立体深度”有意思的是，GitHub 上的 ARCore 1.23 [的发布说明并没有提到双摄像头立体深度支持，但是在 Google 开发者页面](https://github.com/google-ar/arcore-android-sdk/releases/tag/v1.23.0)的发布说明[中提到了。谷歌开发者页面上的发布说明指向谷歌支持 SDK 的设备列表，最近](https://developers.google.com/ar/whatsnew-arcore#whats_new_in_arcore_v1230)[更新了](https://www.xda-developers.com/galaxy-s21-series-mi-10i-oneplus-nord-n10-5g-more-gain-ar-apps-support/)以声明“双摄像头支持将在未来几周内推出”Pixel 4 和 Pixel 4 XL。

谷歌的 Pixel 4 和 4 XL 是唯一配备辅助长焦摄像头的 Pixel 手机，而谷歌的 Pixel 4a 5G 和 Pixel 5 配备了辅助超广角摄像头。考虑到添加对第二个摄像头的支持可能需要大量的校准工作，一些现有设备可能不会支持双摄像头立体深度图。然而，多部手机都有飞行时间传感器，[通过减少扫描时间和改善平面检测来提高](https://www.xda-developers.com/google-arcore-depth-api-public-launch/)深度映射体验质量。双摄像头深度支持将带来多大的改进还有待观察，但希望谷歌在本月晚些时候发布公告后会展示一些演示。