# Android 12 暗示了一种带有显示指纹扫描仪的像素设备

> 原文：<https://www.xda-developers.com/google-pixel-phone-under-display-fingerprint-scanner/>

谷歌既负责维护 Android，也负责制造新的 Pixel 手机，因此有时很难判断一个新的 Android 功能何时也意味着一个新的 Pixel 功能。仅仅因为 Android 增加了对新硬件的支持并不总是意味着未来的 Pixel 手机将实际上搭载该硬件，尽管这并不意味着这永远不会发生。例如，Pixel 手机无线充电的回归和谷歌制造的无线充电底座的存在，[首先通过 Android 代码](https://www.xda-developers.com/android-p-wireless-charging-dock-google-pixel-3/)泄露。现在，我们在 [Android 12](https://www.xda-developers.com/android-12/) 中发现了证据，表明未来的 Pixel 设备可能最终会添加一个显示屏下指纹扫描仪。

今天早些时候，谷歌公布了 Android 12 的[第二次开发者预览](https://www.xda-developers.com/android-12-developer-preview-2/)。在代码中，开发者 [kdrag0n](https://twitter.com/kdrag0n) 发现了 SystemUIGoogle 应用中的几个新类。其中一个类被称为“UdfpsControllerGoogle”，其中“Udfps”指的是“显示不足的指纹扫描仪”。

现在，来自第一个 Android 12 开发者预览版的 SystemUIGoogle 应用程序[也增加了几个与显示不足的指纹读取器相关的类](https://twitter.com/MishaalRahman/status/1362550786601979905)，但我们当时没有想到这一点，因为没有任何证据表明代码不仅仅是为了 AOSP 的通用 Udfps 支持，Android 的开源版本。许多定制 ROM 开发者会告诉你，AOSP 缺乏显示下指纹扫描仪的支持已经引起了很多头痛，所以是时候让谷歌添加适当的支持了。然而，这些新的 Udfps 类是 com.google.android.systemui 路径的一部分，而不是 com.android.systemui，这表明这些类是为 Pixel 手机而不是 AOSP 开发的。这并不是未来 Pixel 手机将拥有显示屏下指纹扫描仪的明确证据，但根据我们以这种方式了解新 Pixel 功能的经验，我们有足够的信心现在提出这种可能性。

虽然谷歌在 Pixel 手机中采用显示屏下指纹扫描仪会晚一些，但这个时机是有意义的。光学显示器下指纹扫描仪已经存在多年，但这些模块的质量自首次推出以来已经提高了很多。它们仍然不如物理电容指纹扫描仪或基于硬件的面部认证安全，但与前者相比，它们允许更时尚的设计，与后者相比，成本低得多。我们面临的最大问题是:如果谷歌在未来的 Pixel 手机中安装一个显示屏下指纹扫描仪，它会是光学传感器还是超声波传感器？

最后，[谷歌也准备在 Android 12 中引入](https://www.xda-developers.com/android-12-dp2-new-features/)一种新的“[滑动通知](https://www.xda-developers.com/android-12-new-swipe-down-gesture-notification-shade-from-any-screen/)手势，这是对带有指纹扫描仪的 Pixel 手机上旧的“滑动指纹通知”手势的替代。由于显示屏下指纹扫描仪不能用于指纹滑动手势，新的“滑动通知”手势将为新的指纹硬件提供一个很好的补充。

*感谢 PNF 软件为我们提供了使用* *[JEB 反编译](https://www.pnfsoftware.com/?aid=xdadev)* *的许可，这是一款针对 Android 应用的专业级逆向工程工具。*

*特色图片:一加 7T Pro 的光学欠显指纹扫描仪。*