# Android 12 阻止第三方应用程序替换共享表

> 原文：<https://www.xda-developers.com/android-12-blocks-third-party-apps-from-replacing-the-share-sheet/>

Android Sharesheet 是一个菜单，当你点击应用程序中的分享按钮时，它会从底部弹出，列出所有可能的分享选项和分享方式。但是你可能已经注意到了，Android Sharesheet 的用户界面在不同的应用程序之间看起来会有很大的不同。这是因为谷歌没有强制 share sheet 的 UI 一致性，而是允许第三方应用和原始设备制造商根据自己的意愿定制它。Android 用户可以完全绕过 Android Sharesheet 的方法之一是使用第三方应用程序，如 Sharedr，它提供了更一致、更简单的用户界面，也取消了直接共享，这在一些设备上可能会很慢——尽管在 Android 11 中[获得了显著的性能提升](https://www.xda-developers.com/android-10-share-menu-faster-quantified/)。但看起来，在 [Android 12](https://www.xda-developers.com/android-12/) 中，使用第三方共享表来替代 Android 共享表并不容易。

在 Android 12 中，谷歌不再允许第三方应用程序将自己设置为默认的共享表。Sharedr 的开发者最近[在 AOSP 错误追踪器上开了一张罚单](https://issuetracker.google.com/issues/183035750?pli=1#comment2)，详细说明了在 Android 12 上，系统不再显示在 Sharedr 和 Android Sharesheet 之间进行选择的提示，而是默认总是打开 Android Sharesheet。作为对这个问题的回应，一名谷歌员工证实这是有意为之的行为，而不是一个错误。换句话说，谷歌在 Android 12 中阻止了第三方应用取代 sharesheet。

> 我们实际上从未打算让应用程序取代共享对话框，我们的意图是让应用程序启动共享对话框。能够替换共享对话框也变得越来越不可能——你不能实现 UI 的直接共享部分，也不能实现 R 中的个人与工作简介标签，等等。这是不可行的，让应用程序来取代。

你仍然可以使用 Sharedr 和其他 share sheet 替代品，但应用程序本身无法响应共享事件，因此当你试图共享某些内容时，你将无法选择将它们设为默认。相反，你必须在股票分享表中选择 Sharedr，然后使用它来选择要分享的目标应用程序，这又增加了一个步骤。目前还不清楚这种新行为是否会阻止 Android OEMs 定制 Android Sharesheet。例如，像三星和 LG ( [RIP](https://www.xda-developers.com/lg-exits-smartphone-business/) ) [这样的原始设备制造商让你禁止直接分享目标](https://www.xda-developers.com/remove-direct-share-share-menu-root/)出现在分享表中。明确一点，这个问题只适用于 Android 12。如果你运行的是 Android 11 或之前的版本，你应该可以毫无问题地使用 Sharedr 或其他 share sheet 应用程序。

*特色图片:Sharedr 更换安卓分享单*