# Android 12 上的“边下载边玩”让你更快地进入游戏

> 原文：<https://www.xda-developers.com/android-12-play-as-you-download/>

今天，谷歌游戏团队启动了一年一度的谷歌游戏开发者峰会。在峰会上，谷歌推出了新的工具和解决方案，使 Android 和 Chrome OS 上的游戏开发更容易。然而，这还不是全部。该公司还推出了一项新功能，旨在改善向用户交付游戏的体验。这项名为“边下载边玩”的功能适用于运行 [Android 12](https://www.xda-developers.com/android-12/) 或更高版本的设备，它有效地消除了下载大型游戏的等待时间。

## 在 Android 12 上边下载边玩

“下载即玩”是 Google Play 提供的一项新服务，“允许用户在几秒钟内进入游戏，同时在后台下载游戏资产。”谷歌开发这个新的“边下载边播放”功能的原因很简单“用户想马上开始玩，但随着游戏质量的不断提高，他们的大小会增加，导致漫长而乏味的下载，”谷歌解释说。这个概念本身并不新鲜——索尼的 PlayStation 和微软的 Xbox 游戏机多年来一直提供类似的功能——但直到最近安卓系统才需要它，因为大多数手机游戏的尺寸都比游戏机或 PC 游戏小得多。

 <picture>![Play as you download demo](img/4cb4b7b4e27b09814e39fa98a4af7088.png)</picture> 

Left: Without "play as you download. Right: With "play as you download."

谷歌表示，“边下载边玩”适用于所有通过 Play Store 发布应用和游戏的开发者，一旦实施，游戏“打开速度至少比以前快两倍”。在某些情况下，这种改进可能是相当引人注目的，谷歌表示，400MB 大小的游戏只需 10 秒钟就可以加载，而不是几分钟。

只有运行最新版本 Android 的设备才能利用这一新功能，原因是该功能“内置于 Android 12 的核心”。谷歌向 *XDA* 证实，私下里，“边下载边玩”利用了[安卓的增量文件系统](https://www.xda-developers.com/google-incremental-file-system-android-big-games/)，这是一个“特殊用途的 Linux 虚拟文件系统，允许在程序的二进制文件和资源文件仍在网络上被缓慢下载时执行程序。”

尽管“边下载边玩”对所有应用开发者开放，但它要求开发者以 Android 应用捆绑格式构建他们的应用。这是因为该功能利用了 [Play Asset Delivery](https://developer.android.com/guide/playcore/asset-delivery) ，这需要应用捆绑格式。2021 年 8 月 1 日[之后提交到 Google Play 的新应用被要求](https://www.xda-developers.com/google-android-app-bundle-play-store/)使用安卓应用捆绑格式，但是[一些开发者](https://www.xda-developers.com/google-play-apk-replacement-pros-cons/)对这一要求并不满意。如果你不介意捆绑软件的要求，那么“边下载边玩”将会是一个很好的功能，可以让用户更快地进入你的游戏。

开发者可以通过[填写这张表格](https://services.google.com/fb/forms/playasyoudownloadbeta/)来注册“边下载边玩”测试程序。有关新功能的更多细节，请观看 2021 年谷歌游戏开发者峰会的“交付空间更新”主题演讲。

\ r \ nht TPS://www . YouTube . com/watch？v=cVzD_TwnQDY\r\n

## 增量的启动器支持

谷歌还鼓励启动器开发者增加对 Incremental 的支持，Incremental 是“边下载边玩”的内部名称，当应用程序被增量下载时，它会在主屏幕上显示一个承诺图标和下载进度指示器。如果用户点击图标，但它还没有准备好启动，那么启动器应该将用户导航到应用程序在谷歌 Play 商店上的登录页面。一旦部分下载的应用程序准备好启动，启动器应该用常规应用程序图标替换承诺图标，但应该显示反映应用程序下载状态的下载进度指示器。单击应用程序图标现在应该会启动应用程序，当应用程序下载完成时，下载进度指示器应该会被移除。

为了实现这个特性，launcher 开发者应该使用几个 API:[package installer。SessionCallback#onCreated](https://developer.android.com/reference/android/content/pm/PackageInstaller.SessionCallback#onCreated(int)) 和[launch rapps。回调# onpackageloadingprogress changed](https://developer.android.com/reference/android/content/pm/LauncherApps.Callback#onPackageLoadingProgressChanged(java.lang.String,%20android.os.UserHandle,%20float))或[launcheractivityinfo . getloadingprogress()](https://developer.android.com/reference/android/content/pm/LauncherActivityInfo#getLoadingProgress())。

关于这应该是什么样子的例子，请查看[我们之前关于未决应用安装](https://www.xda-developers.com/google-tests-pending-apps-home-screen/)的文章，其中我们发现谷歌公开 A/B 测试 Pixel Launcher 的几个用户的这一功能。