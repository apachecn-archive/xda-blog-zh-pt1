# Google Play 服务将终止旧版本 Android 的更新

> 原文：<https://www.xda-developers.com/google-play-services-end-updates-android-jelly-bean/>

# Google Play 服务将终止旧版本 Android 的更新

谷歌将结束 Android 4.1、4.2 和 4.3 上的 Google Play 服务更新，这些版本统称为 Android“果冻豆”。

Google Play Services 是一个可以在所有谷歌认证的 Android 设备上找到的库，它为 Play Store 和数十个第三方应用程序可以使用的应用程序 API 提供支持。Play Services 也是谷歌向旧版本 Android 推出新功能的渠道，比如最近所有 Android 6.0 以上设备都推出了附近的共享功能。然而，一些*非常旧的*手机和平板电脑将不会获得新的 Play 服务更新。

谷歌今天[在一篇博文](https://android-developers.googleblog.com/2021/07/google-play-services-discontinuing-jelly-bean.html)中宣布，将不再更新 Android Jelly Bean 上的 Google Play 服务，该服务包括 4.1-4.3 版本(API 级别 16、17 和 18)。谷歌表示，旧的操作系统正在被淘汰，因为果冻豆现在只占不到 1%的 T2 活跃安卓用户。Jelly Bean 设备的最终版本将是 Play Services v21.30.99，预计将于 8 月底发布。目前该应用的最新版本是 21.24.18。

“当前 SDK 版本所需的功能，”谷歌表示，“已经存在于带有 Google Play 服务的(Jelly Bean)设备上，并将继续工作，不做任何改变。”建议在其应用中使用 Play Services SDK 的开发人员使用 API 级别 19 (Android 4.4 KitKat)作为最低支持的 API 级别，以避免出现问题。如果开发人员需要维护对 Jelly Bean 设备的支持，他们也可以编译多个 APK，每个 APK 包含不同版本的 Play Services 库。

Android 4.1 果冻豆于 2012 年 7 月首次发布，具有可扩展通知、USB 音频和更流畅的界面等功能。Android 4.2 于 2012 年 11 月发布，提供了锁屏改进和多用户帐户支持，Android 4.3 于 2013 年 7 月发布，提供蓝牙 le 和一个重新制作的相机应用程序。