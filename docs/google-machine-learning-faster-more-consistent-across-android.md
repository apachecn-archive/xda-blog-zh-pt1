# 谷歌正在让机器学习在 Android 上更快、更一致

> 原文：<https://www.xda-developers.com/google-machine-learning-faster-more-consistent-across-android/>

继昨天在谷歌 I/O 2021 上的主要演示之后，该公司举行了几场会议，现在可以通过 YouTube 点播。其中一场会议涵盖了 Android 机器学习的新内容，以及谷歌如何让开发者更快、更一致地学习。

机器学习负责为 Android 用户每天使用的功能提供动力，从图像中的背景模糊，视频通话应用中的背景替换，到 Pixel 手机上通话中的[实时字幕](https://www.xda-developers.com/live-caption-transcribe-phone-calls-google-pixel-4a/)。虽然机器学习变得越来越先进，但谷歌表示，在部署 ML 驱动的功能方面仍然存在几个挑战，包括对应用膨胀和性能变化的担忧。还有功能可用性的问题，因为不是每个设备都可以访问相同的 API 或 API 版本。

*图片:谷歌*

为了解决这个问题，谷歌宣布了 Android 的可更新的、完全集成的 ML 推理堆栈，因此将有一组通用组件跨所有设备一起工作。这为应用开发者带来了以下好处:

*   开发人员不再需要在自己的应用中捆绑代码进行设备上的推理。
*   机器学习 API 与 Android 的集成程度更高，可以提供更好的性能。
*   谷歌可以在 Android 版本和更新之间提供一致的 API。API 的定期更新直接来自 Google，独立于操作系统更新而存在。

*图片:谷歌*

为了实现这一点，谷歌正在做几件事。首先，它表示 [TensorFlow Lite for Android](https://www.xda-developers.com/tensorflow-lite-mobile-machine-learning/?) 将通过 Google Play 服务预装在所有 Android 设备上，因此开发者不再需要将其与自己的应用捆绑在一起。谷歌还在 Android 上添加了一个内置的兼容 GPU 列表，可用于硬件加速。这家搜索巨头还推出了“自动加速”，将开发者的机器学习模型纳入考虑范围，并可以检查模型在 CPU、GPU 或其他加速器上加速是否效果更好。

*图片:谷歌*

接下来，谷歌还表示，它正在将 NNAPI 从核心操作系统框架中移走，以便它可以通过 Google Play 服务进行更新。这意味着开发人员可以使用相同的 NNAPI 规范，即使两个设备运行不同的 Android 版本。值得注意的是，在 Android 11 中， [NNAPI 运行时](https://source.android.com/devices/architecture/modular-system/nnapi)被添加为[主线模块](https://www.xda-developers.com/android-project-mainline-modules-explanation/)，这可能是这些更新的交付方式。谷歌正在与高通合作，在运行 Android 12 的设备上提供可更新的 NNAPI 驱动程序，新功能将在芯片组的商业生命周期内进行反向移植。此外，更新[将定期交付](https://www.qualcomm.com/news/onq/2021/05/20/announced-google-io-2021-regular-google-nnapi-updates-qualcomm-snapdragon-mobile)，也将向后兼容旧的骁龙处理器。

机器学习的改进只是谷歌本周宣布的一小部分。这家搜索巨头公布了 Android 12 的重大重新设计，并分享了与三星合作[改进 Wear OS](https://www.xda-developers.com/new-wear-os-update-hands-on/) 的首批细节。

\ r \ nht TPS://www . YouTube . com/watch？v=uTCQ8rAdPGE\r\n