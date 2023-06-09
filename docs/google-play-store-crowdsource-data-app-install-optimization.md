# Play Store 的应用安装优化功能减少了应用安装时间

> 原文：<https://www.xda-developers.com/google-play-store-crowdsource-data-app-install-optimization/>

**更新 1 (04/23/2021 @ 04:07 PM ET):** 谷歌现在推出新的众包应用安装优化功能。[点击这里了解更多信息。](#update1)文章发表于 2021 年 3 月 17 日，下面保留。

早在 2018 年，谷歌推出了一种新的应用发布格式，名为 [Android 应用捆绑](https://www.xda-developers.com/android-app-bundle-google-play-dynamic-delivery-apk-size/)，帮助应用开发者大幅减少 APK 大小，并在需要时提供功能，而不是在安装时一次性捆绑所有内容。为了进一步改善最终用户的应用安装体验，并减少在我们的 Android 设备上下载、打开和运行应用所需的时间，谷歌推出了一项名为应用安装优化的新计划。

当[应用安装优化](https://support.google.com/googleplay/answer/10122796)(via[*9 to 5 Google*](https://9to5google.com/2021/03/16/google-play-app-install-optimization/))功能开启时，谷歌会收集你如何与新安装的应用互动的数据，或者你第一次打开应用时访问了应用的哪些部分。谷歌将从庞大的用户群中收集这些数据，并将其结合起来，以找到共同的行为，并确定应用程序的哪些部分更重要。谷歌表示，利用这些信息，它可以加快应用程序的安装、打开和运行时间。

> 当你打开应用程序安装优化时，谷歌可以告诉你在安装后第一次打开应用程序时使用的是哪个部分。当足够多的人这样做时，谷歌可以优化应用程序，以便为每个人更快地安装、打开和运行。

谷歌指出，应用程序安装优化功能不会收集任何个人数据，如电子邮件地址、您的姓名或存储在您设备上的内容。

谷歌表示，它将利用众包数据来:

*   加快 Google Play 应用程序的安装速度
*   减少打开和运行应用程序所需的时间
*   减轻设备的 CPU、电池和存储压力

应用程序安装优化功能是可选的，用户可以选择在 Play Store 应用程序中打开或关闭它。谷歌的[支持页面](https://support.google.com/googleplay/answer/10122796)指出，即使你禁用该功能，你仍然可以从其他用户收集的数据中受益。

目前，该功能在我们运行 Play Store 版本 24.4.23 的设备上不可用。我们会密切关注这一功能，并会让你知道它何时对所有人开放。与此同时，这是 Android 应用程序开发人员和逆向工程师 Alessandro Paluzzi 的一张图片，显示一旦 Play Store 应用程序上线，您将在其中找到该选项。

* * *

## 更新 1:推出

Twitter 上的 Tipster @ [AlaSabo3](https://twitter.com/AlaSabo3) 告诉我们，当他们今天打开 Play Store 应用程序时，他们收到了一个弹出窗口，通知他们“谷歌正在你的帮助下优化应用程序安装”。描述是“Google Play 根据人们最常用的东西，让应用程序安装、打开和运行更快。安装后首次打开应用程序时，Google 会记录下您使用的应用程序部分。当有足够多的人这样做时，你的应用程序会安装得更快。应用安装优化会自动打开，但您可以在“设置”中将其关闭。”

在用户与我们分享的另一张截图中，我们可以看到有一个新的“应用程序安装优化”开关。正如描述中所提到的，默认情况下为它们启用了切换。

我们的线人在他们运行 [Android 12](https://www.xda-developers.com/android-12/) DP3 的 Pixel 设备上的 24.9.19-21 版本的 Play Store 应用程序上看到了这一功能。我们在运行 Android 12 DP3 和谷歌 Play 商店版本 25.0.31-21 的 Pixel 3 XL 上没有看到切换，这表明这是一个有限的服务器端部署。