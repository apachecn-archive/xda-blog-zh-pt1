# ZenFone 7 和 7 Pro 接收 Kirisakura 自定义内核

> 原文：<https://www.xda-developers.com/asus-zenfone-7-pro-kirisakura-kernel-omnirom-android-11/>

# 华硕 ZenFone 7 系列开发更新:Kirisakura 内核和 Android 11 ROM

华硕 ZenFone 7 系列的第一个定制内核以及基于 Android 11 的 OmniROM 的第一个版本都在这里。

华硕本月早些时候发布了 ZenFone 8 系列，刷新了其旗舰阵容。ZenFone 8 和 Zenone 8 Flip [提供顶级规格](https://www.xda-developers.com/asus-zenfone-8-review/)，同时仍然比许多骁龙 888 驱动的同行便宜得多。然而，如果你拥有去年的 ZenFone 7 或 ZenFone 7 Pro，你会发现[没有什么理由升级](https://www.xda-developers.com/asus-zenfone-7-pro-review-a-flipping-fantastic-flagship-smartphone/)，因为除了稍微快一点的芯片组和其他增量升级，没有什么值得兴奋的。此外，如果你厌倦了华硕的软件，你可以随时在定制 rom 和内核的世界中寻求庇护。华硕 ZenFone 7 和 7 Pro 没有一长串的定制 ROM 可供尝试，但他们有一个官方构建的 OmniROM 和官方 TWRP 支持。现在，该设备已经收到了它的第一个定制内核。

**[【ASUS zenfone 7/7 pro xd 论坛】](https://forum.xda-developers.com/c/asus-zenfone-7-7-pro.11393/)**

ZenFone 7 系列的 Kirisakura 内核由 XDA 公认的开发者/公认的贡献者 [Freak07](https://forum.xda-developers.com/m/freak07.3428502/) 提供。根据开发者的说法，Kirisakura 内核提供了更流畅的用户界面体验，同时仍然提供了与普通内核相同的电池寿命。内核包含了最新的 CAF-上游内核基础，并提供了以下主要特性:

*   基于华硕为 Android 11 提供的最新内核资源，旨在用于最新的华硕股票固件(目前为 30.41.69.51)
*   用 Clang 12.0.5 编译，用-O3 速度优化构建
*   Linux-稳定-上游包括到 4.19.190
*   骁龙 865/+ (SD865/+)的 CAF 基础更新为上游 CAF
*   从 4.19 内核/通用和 Pixel 5/4/XL 内核移植而来的内核控制流集成(CFI)和链接时间优化(LTO)
*   影子调用堆栈(SCS)安全功能
*   使用在 Pixel 4 XL Android R-Preview 内核中首次使用的 ThinLTO，而不是完整的 LTO，以获得完整的程序可见性(CFI 需要)
*   修复在各种子系统中发现的违反 CFI 的问题，如华硕/设备特定的驱动程序和高通驱动程序
*   将内核与 LLD 链接起来，并使用 RELR 重定位
*   包括来自 kernel/common 的重要修复/改进
*   闪内核会保留根！
*   可通过 EXKM、FKM 或 TWRP 在根系统上刷新！
*   禁用各种调试配置，根据 google，perf 构建内核不需要这些配置。
*   禁用 SELinux 审计(我们不必处理 SELinux 否认从
*   显示调整以减少静态渲染图像的功耗

如果这一切听起来让你兴奋，你可以在下面的链接中找到更多的信息，包括 flashable 内核 zip 和一步一步的安装说明。

**[下载 ZenFone 7 系列的 Kirisakura 内核](https://forum.xda-developers.com/t/kernel-15-05-2021-android-11-kirisakura-1-1-3-for-asus-zenfone-7-pro-aka-tequila.4269677/)**

在 ZenFone 7 系列的其他开发相关新闻中，OmniROM 已经更新到 Android 11。ZenFone 7 系列的 OmniROM 过去是基于 Android 10 的，但 XDA 高级成员 [micky387](https://forum.xda-developers.com/m/micky387.4251307/) 最近发布了一个官方支持的 Android 11 版本。点击下面链接获取基于 Android 11 的 OmniROM 的最新版本。

**[为 ZenFone 7 系列](https://forum.xda-developers.com/t/rom-official-omnirom-for-zenfone7-7pro-android-11.4203251/)** 下载基于 Android 11 的 OmniROM