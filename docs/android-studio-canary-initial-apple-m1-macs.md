# Android Studio Canary 增加了对苹果新 M1 MAC 电脑的初始支持

> 原文：<https://www.xda-developers.com/android-studio-canary-initial-apple-m1-macs/>

除了网络，Android 可能是最容易使用的开发平台之一。实体 Android 设备可以便宜得令人难以置信，并且不缺少用于测试的仿真器选项。当然，实际的 IDE——Android Studio——可以在几乎所有现存的桌面平台上运行，包括 macOS。

然而，Android Studio 一直缺少一些东西:ARM 支持。虽然基于 ARM 的处理器主要用于移动设备，但我们开始看到它们用于笔记本电脑甚至台式机。甚至苹果公司最近也加入了这一行动，其基于 ARM 的 M1 芯片组为最新的 Macbook Air、Macbook Pro 13 和 T2 的 24 英寸 iMac 提供动力。

因为这是最近的过渡，苹果已经内置了一个兼容层，允许基于 x86 的程序在 M1 MAC 电脑上运行，而且看起来效果不错。但是没有什么能打败本土。谢天谢地，谷歌正在研究解决方案。

Android Studio 的最新 Canary 版本(撰写本文时为 15 个版本)带来了对 M1 MAC 的初始原生支持。仍然缺少很多东西，但是基本的工作正常。

*   您可以构建和运行仅支持 JVM 的应用程序(C++编译器尚未完成)。
*   您可以使用设计工具，如布局预览。
*   可以配合 Android 11 和 Android 12 使用内置仿真器。

当然也有很多现在还不行的。

*   你不能进行任何基于 C 语言的开发，因为 NDK 和编译工具还不能在 ARM 上运行。
*   一旦你更新到金丝雀 15，你将无法进行下一个版本的增量更新。
*   许多调试工具不能开箱即用。这包括数据库检查器、布局检查器和其他检查器。在 [JetBrains 的问题跟踪器](https://youtrack.jetbrains.com/issue/IDEA-257549#focus=Comments-27-4590206.0-0)上有一个解决方法。
*   模拟器存在一些用户界面问题。

这些列表都不是详尽无遗的，所以一定要查看谷歌的博客文章了解更多细节。

看到 Android Studio for ARM 的构建令人鼓舞。虽然目前这只是针对 macOS，但它有望在未来为 Windows 甚至 Linux 的 ARM 版本打开大门，这可能导致直接从 Android 开发 Android。

然而，在我们等待那个乌托邦式的未来时，如果你有一台 M1 Mac 电脑，并且你想尝试一下这个版本，请前往[谷歌的博客文章](https://androidstudio.googleblog.com/2021/04/android-studio-arctic-fox-canary-15.html)了解更多关于新功能的细节，以及你可能需要什么来让它运行起来。