# Android 12.1 可能是 Android 的下一个版本，而不是 Android 13

> 原文：<https://www.xda-developers.com/android-12-v2-update/>

谷歌可能刚刚泄露了下一版本 Android 的秘密。Android 的下一个版本可能是对 Android 12 的小更新，将在几周内发布。传统上，这些微小的版本颠簸被称为点更新，但谷歌自 2017 年 Android 8.1 Oreo 以来就没有发布过点更新。如果谷歌确实在进行 Android 12.1 更新，那么我们有可能在今年晚些时候看到它与 [Pixel 6](https://www.xda-developers.com/google-pixel-6/) 系列一起推出。

今天早些时候，科技巨头[宣布](https://www.xda-developers.com/android-12-beta-5-changelog/)Android 12 的第五个测试版，这是几周后稳定更新推出之前的最后一个测试版。在发布之前，开发人员被建议将他们的应用程序更新到目标 API 级别 31，这是 Android 12 提供的框架 API。之前的 Android 版本——Android 11——对应的 API 等级是 30，而之前的 API 等级是 29，对应的是 Android 10。从一开始，每一个新的 API 级别都伴随着 Android 版本号的上升，只有 API 级别 20 的[是唯一的例外，它对应于可穿戴设备的 Android 4.4 KitKat 独家版本。因此，如果我们发现 Google 提高了 API 级别，那么可以肯定的是版本号也会提高。](https://developer.android.com/studio/releases/platforms#4.4)

自然地，我们的第一个假设是 API level 32 将对应于 [Android 13 提拉米苏](https://www.xda-developers.com/google-android-13-t-tiramisu-dessert-name/)，因为，正如我们之前提到的，谷歌已经多年没有发布更新了。然而，我们在 AOSP·格里特(H/T XDA 公认的开发者 [luca020400](https://forum.xda-developers.com/m/luca020400.5778309/) )中发现了一些证据，表明 API 级别 32 对应于 Android 12“sc-v2”而不是 Android 13“T”。在[的新代码更改](https://android-review.googlesource.com/c/platform/frameworks/native/+/1820832)中，一名谷歌员工将首次提供的新 NDK API 级别从 32 更改为 33。根据评论中的讨论，原因是“目前在 sc-v2-dev 中没有计划的 NDK API”这表明 API 等级 33 对应的是 Android 13 T，比即将发布的 Android 12 版本对应的 API 等级(API 等级 31)高两个 API 等级。)

很可能“sc-v2”中的“sc”指的是“雪筒”，也就是传闻中 Android 12 的甜点代号。提交给 AOSP Gerrit 的[少数](https://android-review.googlesource.com/c/platform/frameworks/base/+/1715469) [其他](https://android-review.googlesource.com/c/platform/system/apex/+/1717640) [代码变更](https://android-review.googlesource.com/c/platform/cts/+/1736896)提到了 sc-v2-dev 分支，但它们都没有暗示 sc-v2-dev 将在 API 级别上有所提升。然而，根据我们今天看到的新证据，谷歌似乎有可能在 Android 12 和 Android 13 之间发布一个临时更新。通常，这些临时更新或维护发布会伴随着用户可见的版本号的变化，这就是为什么我们认为我们可能会看到 Android 12.1 点发布。然而，也有可能这个新的 API 级别根本不会伴随着新的版本号，或者这个新的 API 级别可能会对应于针对另一种形式的发布，就像 API 级别 20 是如何专属于 Android 4.4w 的。

在发布新手机后不久，谷歌习惯于向 AOSP 上传一堆新代码，在 Pixel 3 和 Android 9 Pie 之前，这些代码通常被标记为新的维护版本，并作为点更新发送给用户。自从 Pixel 3 以来，他们一直在继续这种做法，尽管他们已经停止增加版本号和 API 级别，也许是为了让 OEM 和开发人员更容易跟上版本发布。我们有兴趣了解为什么谷歌这么快就提高 API 水平，以及这对平台和开发者会有什么影响，尽管我们怀疑这不会改变 [Play Store 的变化目标版本要求](https://www.xda-developers.com/play-store-updated-requirements-api-level-64-bit/)，因为谷歌只跟踪每个 Android 甜点发布。无论如何，我们必须等到今年晚些时候才能知道 Android 12.1 是否真的会发布。

* * *

代码变更的评论[中有一句话，我们不太确定是什么意思。一位谷歌人声称“我们的一些 Nest 设备可能不会迁移到 T”，这肯定是一件*有趣的*事情，因为据我们所知，Nest 设备上的操作系统与任何现代 Android 版本都不匹配。事实上，远非如此:](https://android-review.googlesource.com/c/platform/frameworks/native/+/1820832)[看起来](https://twitter.com/MishaalRahman/status/1272581465382010881)至少一些旧的 Nest 设备曾经运行非常非常精简的 Android 4.0 版本，谷歌正在将第一代 Nest Hub 设备从 Cast OS [迁移到其内部的 Fuchsia OS](https://www.xda-developers.com/google-fuchsia-os-debut-nest-hub/) 。因此，我们不确定如何理解这句话，但我们认为无论如何都值得指出，因为对话中提到了它。

*这篇文章的标题改为“之前”,以消除对 Android 13 状态的混淆。*