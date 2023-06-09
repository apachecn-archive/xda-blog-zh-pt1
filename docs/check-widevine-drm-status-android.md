# 如何检查你的 Android 设备是否支持 Widevine DRM

> 原文：<https://www.xda-developers.com/check-widevine-drm-status-android/>

许多流媒体服务，如网飞、迪士尼+、Hulu 等，使用各种类型的数字版权管理(DRM)来保护其内容不被复制和再分发。大多数 DRM 实际上并不阻止这种行为，相反，主要是用来骚扰付费内容的人，但这是另一个时间的讨论。Widevine 是一种广泛使用的 DRM 技术，经常出现在 web 和 Android 应用程序中，但并不是所有的 Android 设备都完全支持 Widevine DRM。

网飞、HBO、Disney+、Prime Video、Hulu、Sling、DirectTV 和*其他许多*流媒体服务使用 Widevine DRM 。Widevine 有三个安全级别:L3、L2 和 L1。以下是每一项的细目分类:

*   **Widevine L3:** 这是支持度最低的选项，DRM 完全基于软件。只有 Widevine L3 的设备没有运行 DRM 加密的可信执行环境(TEE)。大多数情况下，Widevine 保护的内容只能在 480p 下播放。
*   **威德文 L2:** 支持 L2 的设备拥有可信执行环境(TEE)，但视频处理是在软件或单独的视频硬件中进行的。大多数时候，Widevine 保护的内容将以最高 540p 的分辨率播放。
*   Widevine L1: 这是最高级别的保护，媒体完全在可信执行环境(TEE)中解密和处理。支持 L3 的设备可以以尽可能高的分辨率播放 Widevine 保护的内容。

大多数通过谷歌认证的 Android 设备都支持 Widevine L1，有时与其他 DRM 方法结合使用。但是，经过修改的设备(如根电话)或未经认证的电话可能仅支持 L3 或 L2。在某些情况下，[损坏的软件更新](https://www.androidpolice.com/2021/01/27/some-asus-rog-phone-3-handsets-have-lost-hd-playback-in-netflix-due-to-a-widevine-issue/)导致 Widevine DRM 恢复到 L2 或 L3。

## 如何检查 Widevine 支持

令人欣慰的是，很容易检查你的 Android 手机或平板电脑是否可以使用 Widevine DRM，包括支持哪些级别。你所要做的就是从 Play Store 下载 [DRM Info](https://play.google.com/store/apps/details?id=com.androidfung.drminfo) 应用并打开它。

每种支持的 DRM 技术都显示为一张卡片。Widevine 卡应该会告诉你是否支持 DRM，如果支持的话，是什么级别。很简单。

如果您看到 L2 或 L3 安全级别，很可能您的设备不支持高分辨率的受保护媒体，并且一些应用程序可能根本拒绝开始流媒体播放。许多应用程序还会检查当前设备的[安全网](https://www.xda-developers.com/safetynet-hardware-attestation-feature-here-to-stay/)状态，以确定媒体是否可以播放。

尤其是网飞，它有自己的一套检查机制来决定什么样的内容会流向你。除了支持 Widevine L1，您的设备还需要通过另一轮认证检查，才能播放网飞的高清或 HDR 内容。如果你想知道网飞能以什么格式传输到你的设备上，你可以点击这里查看网飞的列表。或者，你可以打开网飞应用程序，进入“设置”，然后向下滚动到“播放规格”，看看有哪些格式可用。该页面还会告诉您设备上的 Widevine DRM 级别，以防您不想下载 DRM Info 应用程序。