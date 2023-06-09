# DotOS 为其下一个版本设计了一个新的类似 Android 12 的主题系统

> 原文：<https://www.xda-developers.com/dotos-new-android-12-based-dynamic-theming/>

for Droid on Time 的缩写)定制 ROM 项目的开发者已经为他们即将发布的版本设计了一个新的基于 Android 12 的动态主题引擎。新系统继承了该团队的“MonetWannabe”功能，他们之前尝试了一个基于[壁纸的主题化系统](https://www.xda-developers.com/dotos-5-1-new-wallpaper-based-theming-system-qs-ui-inspired-by-android-12/)，该系统目前在 DotOS 5.1 中可用。正如我们在 4 月份解释的那样，DotOS 的开发者通过“在仔细逆转谷歌在 Android 12 中的实现并调整底层算法以获得更好的灵活性后，从零开始编码整个框架”来实现“MonetWannabe”

自从 DotOS 5.1 中发布了“monetWannabe”之后，谷歌[发布了 Android 12 Beta 2](https://www.xda-developers.com/android-12-beta-2-features/) 和 [3](https://www.xda-developers.com/android-12-beta-3-features/) ，这两个版本都包含了他们官方的“Monet”主题化系统。就背景而言，谷歌代号为“monet”的新动态主题引擎根据从壁纸中提取的颜色生成调色板，然后将这些颜色应用到系统 UI 的各个部分和任何支持它的应用程序。这是谷歌新的 [Material You](https://www.xda-developers.com/material-you/) 设计语言的主要部分，也是 Android 12 最令人兴奋的新功能之一。

Android 12 Beta 2 发布后不久，开发者 [kdrag0n](https://forum.xda-developers.com/m/kdrag0n.7291478/) [从头开始重新创建了](https://www.xda-developers.com/android-12-material-you-theming-system-recreated/)“莫奈”主题化系统，并公布了其工作的源代码。开发者 [Quinny899](https://forum.xda-developers.com/m/quinny899.3563640/) 随后基于 kdrag0n 的工作创建了一个支持库，命名为“MonetCompat”这就是 DotOS 的新主题引擎所基于的——定制 ROM 似乎正在将 MonetCompat 库应用于系统应用程序。

DotOS 中当前的“MonetWannabe”主题化系统只对系统 UI 的某些部分重新着色——主要是快速设置面板。然而，通过“MonetCompact”，DotOS 将动态主题化支持扩展到系统的更多部分，包括各种设置页面、“关于手机”屏幕、浮动音量面板等。该团队表示，新的电池管理器和 OTA 应用程序也将更新，以支持动态颜色。下面是一些截图，展示了新的基于壁纸的动态主题系统。

新的基于 Android 12 的主题化系统将在即将到来的 DotOS 5.2 版本中推出。一旦它变得可用，用户可以在*设置>定制*下启用新的主题引擎，并选择“壁纸颜色”。团队计划何时发布带有改进的动态主题引擎的 DotOS 新版本还没有确定的时间，但是和往常一样，如果没有提供的话，最好不要问 ETA。