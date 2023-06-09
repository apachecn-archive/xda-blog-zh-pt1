# 在 Wear OS 上侧装应用程序很快会变得更加复杂

> 原文：<https://www.xda-developers.com/sideloading-apps-wear-os-complicated/>

目前，如果你想在 Wear OS 设备上下载谷歌 Play 商店上没有的应用程序，你可以前往手表上的 [Play Store](https://www.xda-developers.com/tag/google-play-store/) 的*手机应用程序*部分，安装手机上已经有的应用程序。然而，从 2021 年 3 月 10 日开始，谷歌正在摆脱这一功能。这将限制用户使用像 [Android Debug Bridge](https://www.xda-developers.com/install-adb-windows-macos-linux/) (ADB)这样的开发工具在他们的智能手表上下载应用程序，使这个过程变得更加复杂。

根据开发者和 Reddit 用户 malbry 最近的一篇帖子(通过 [*Android Police*](https://www.androidpolice.com/2021/02/12/wear-os-is-making-app-sideloading-much-more-difficult/) )显示，谷歌已经开始向应用开发者发送电子邮件，提醒他们这一变化。邮件中写道:

*“从 3 月 10 日开始，使用传统嵌入式应用模式的 Wear OS 应用将不再显示在“手机上的应用”部分，并且在 on-watch Play 商店中实际上是不可发现的。我们鼓励开发者迁移到更新的多 APK 模式，使他们的应用程序可以在手表上被发现，并减少他们手机 apk 的大小。”*

对于不知情的人来说，传统的[嵌入式应用模型](https://developer.android.com/training/wearables/apps/packaging#wear-1x)允许开发者将 Wear OS 代码添加到 Android 应用中。实际上，这让用户可以从手机上的*应用*部分下载应用到他们的 Wear OS 设备上。然而，谷歌打算摆脱这种分发模式，为每个人制作更小的手机应用程序。虽然这一举措将有利于没有 Wear OS 智能手表的用户，但它将使使用上述方法的侧装应用程序变得不可能。用户将不得不依赖开发者工具，通过 ADB 将这些应用程序推送到他们的 Wear OS 手表上。

正如 *Android Police* 解释的那样，此举背后的主要想法是将 Wear OS 应用与 Android 应用分离，它应该不会影响许多用户，因为大多数在 Play Store 上发布应用的开发者已经转向新的应用分发模式。然而，它将主要影响不通过 Play Store 发布的应用程序。