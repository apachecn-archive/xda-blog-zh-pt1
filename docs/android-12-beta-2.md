# Android 12 Beta 2 带来了新的隐私功能，在谷歌 I/O 上遭到嘲笑

> 原文：<https://www.xda-developers.com/android-12-beta-2/>

在上个月的谷歌 I/O 开发者大会上，谷歌揭开了其最新 Android 操作系统的面纱: [Android 12](https://www.xda-developers.com/android-12/) 。围绕谷歌的[素材](https://www.xda-developers.com/material-you/)到过多的[新隐私功能](https://www.xda-developers.com/android-12-privacy-private-compute-core-privacy-dashboard/)的可定制设计，Android 12 正在成为谷歌多年来最大的操作系统版本。虽然谷歌在活动中发布了第一个 Android 12 测试版，但它没有谷歌 I/O 上的大多数新隐私功能。随着 Android 12 Beta 2 的发布，这种情况发生了变化。

谷歌今天早些时候发布了第二个 Android 12 测试版，新闻稿强调增加了新的隐私功能，包括**隐私仪表盘**以及**麦克风和摄像头的开关和指示器**。在其他变化中，还有一个**改进的 Wi-Fi 体验**。以下是 Android Beta 2 的新特性:

*   **隐私仪表盘:**该页面显示您的手机上有哪些数据被访问过，以及这些数据被访问的频率。它有一个简单的时间轴视图，显示过去 24 小时内对设备的麦克风、摄像头和位置的所有访问。该页面还帮助用户了解应用程序访问敏感数据的原因，并更快地调整权限。开发者可以通过响应新的系统意图[ACTION _ VIEW _ PERMISSION _ USAGE _<wbr>FOR _ PERIOD](https://developer.android.com/reference/android/content/Intent.html#ACTION_VIEW_PERMISSION_USAGE_FOR_PERIOD)来解释为什么他们的应用会处理敏感数据。开发人员也被建议利用 Android 的数据审计 API 来跟踪他们代码和第三方库中的访问。
*   **麦克风和摄像头切换和指示灯:**当您在设备上使用麦克风或摄像头时，您会在状态栏中看到指示灯。您还可以访问禁用摄像头或麦克风访问的快速设置磁贴。开发者[被建议](https://developer.android.com/about/versions/12/behavior-changes-all#mic-camera-indicators)检查他们的应用程序对麦克风或摄像头的使用，删除任何不必要的使用。
*   **剪贴板读取通知:** Android 12 Beta 2 现在每当应用程序使用 [getPrimaryClip()](https://developer.android.com/reference/android/content/ClipboardManager#getPrimaryClip()) 方法读取剪贴板时，都会在底部显示一条 toast 消息。但是，如果剪贴板是从同一个应用程序中复制的，则不会显示 toast 消息。为了避免在社交媒体上被羞辱，开发者[被建议](https://developer.android.com/about/versions/12/behavior-changes-all#clipboard-access-notifications)尽量减少他们的应用程序从剪贴板上的读取。
*   **更新的 Wi-Fi UX 体验**:第二个 Android 12 测试版增加了“跨越状态栏、快速设置和设置的更简单、更直观的连接体验”有一个新的互联网面板，当你长按互联网快速设置磁贴时会弹出(这个磁贴在早期版本中被称为“Wi-Fi”)。此面板可帮助您快速切换网络和解决问题，而无需深入设置。

随着 Android 12 Beta 2 的发布，现在还剩两个测试版，直到今年晚些时候的稳定版发布。平台稳定性版本将于 2021 年 8 月推出，可能会推出 Beta 4。届时，面向应用的系统行为、SDK/NDK API 和非 SDK 列表将最终确定。你可以在这里了解更多关于 Android 12 beta 发布时间表[。](https://developer.android.com/about/versions/12/overview)

Android 12 Beta 2 从今天开始适用于支持的谷歌 Pixel 手机，包括 Pixel 3、Pixel 3 XL、Pixel 3a、Pixel 3a XL、Pixel 4、Pixel 4 XL、Pixel 4a、Pixel 4a 5G 和 Pixel 5。Beta 1 可用于其他手机制造商的少数手机，但谷歌将它留给原始设备制造商来推动 Beta 2 的更新。获得 Beta 1 的非像素设备有:华硕 ZenFone 8，iQOO 7 Legend，一加 9，一加 9 Pro，OPPO Find X3 Pro，Realme GT，TCL 20 Pro 5G，Tecno Camon 17，小米 Mi 11，小米 Mi 11 Ultra，小米 Mi 11 Pro，小米 Mi 11X Pro / Mi 11i / Redmi K40 Pro+，中兴 Axon 30 Ultra 5G。

值得注意的是，Beta 2 也适用于 Android TV，因此开发人员可以启动模拟器或将构建版本闪存到 ADT-3 上。

如果你正在寻找 Android 12 测试版的下载链接，[看看这篇文章](https://www.xda-developers.com/how-to-download-android-12/)。一旦你下载了测试版，[按照这个指南](https://www.xda-developers.com/how-to-install-android-12/)来学习如何安装它。对于通过谷歌网站注册测试版的 Pixel 手机来说，这个过程相当简单，但对于那些出于任何原因需要下载更新的人，我们的指南将教你如何做。