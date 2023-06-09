# Android 12 可能会给画中画和泡泡带来巨大变化

> 原文：<https://www.xda-developers.com/android-12-picture-in-picture-mode-bubbles-changes/>

作为一个移动操作系统，多任务处理是 Android 相对于 iOS 的最大优势之一。凭借分屏视图、画中画模式和气泡等功能，Android 提供了许多在使用其他应用程序时与应用程序交互的方式。在 [Android 12](https://www.xda-developers.com/android-12/) 中，画中画模式被设置为获得许多新功能，而气泡可能会得到微妙的动画调整。

## Android 12 上的画中画模式

画中画模式最初是在 Android Oreo 中为手机[引入的，但自那以后它的功能更新相对较少。在 Android 11 中，谷歌悄悄地增加了](https://www.xda-developers.com/enable-android-o-picture-in-picture-mode/)[调整 PiP 窗口](https://www.xda-developers.com/android-11-resize-picture-in-picture-pip-windows/)大小的功能。扩展/缩小画中画窗口包括从一个角的正外侧开始向内或向外拖动手指。以我的经验，手势有点不一致，可以改进。

*调整 Android 11 上画中画窗口的大小*

幸运的是，谷歌正在研究 Android 12 中调整 PiP 窗口大小的新方法。你可以用手指捏住来调整大小，也可以双击来自动将窗口调整到最大尺寸(或者返回到上次调整的状态)。调整大小时将使用一个漂亮的交叉渐变动画，使它看起来无缝。

调整大小并不是 Android 12 中画中画模式的新功能。谷歌还准备在 PiP 窗口中增加一个“存储”功能。此功能将允许用户通过将 PiP 窗口拖到左/右边缘来暂时隐藏大部分 PiP 窗口，直到大约三分之一的 PiP 窗口离开屏幕。用户也可以把画中画窗口从一边扔到另一边。只需轻敲 PiP 窗口，就可以使其不稳定。

## 新泡泡动画

Android 的 Bubbles 功能诞生于一个愿望，那就是用一个更专注的 API 来取代操作系统广泛的 System_Alert_Window API，为所有的消息应用程序提供脸书的聊天头功能。它从 Android 10 的测试版功能升级为 Android 11 的[公共功能，在 Android 12 中，它将进行一些 UI 调整。首先，谷歌正在为泡泡制作新的动画。当拖出一个膨胀的泡泡时，会有一个淡入淡出/缩小的动画，更柔和的膨胀/折叠动画，以及泡泡之间更柔和的过渡。在横向模式下，气泡将垂直显示在左侧/右侧，而不是水平显示在顶部。谷歌还启用了灵活的气泡大小和固定位置，这两个功能据说是为 Chrome OS 及其 ARC++容器设计的。](https://www.xda-developers.com/android-11-developer-preview-changes/)

一段视频展示了 Android 11 在 Facebook Messenger 中的气泡功能。

## 应用程序对

除了对 PiP 窗口和 bubbles 的改变，谷歌还准备升级 Android 的分屏多任务系统，增加应用对。应用程序对将允许您启动设置应用程序对，以便在分屏视图中启动，该功能最初出现在其他原始设备制造商和第三方开发人员的软件中。 *9to5Google* [首先透露了](https://www.xda-developers.com/android-12-may-app-pairs-feature/)这一功能的存在，我们现在可以确证它存在于 Android 12 中。

* * *

我们不知道这些变化在 Android 12 中会是什么样子，但我们可能不用等很久就能找到答案。这些功能可能不会在第一个 Android 12 开发者预览版中激活，如果是这样，我们将尝试启用它们，以便我们可以演示这些变化。

*特色图片:Android 11 中的画中画模式*