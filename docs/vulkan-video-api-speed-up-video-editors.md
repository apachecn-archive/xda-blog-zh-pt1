# Vulkan 视频 API 可以帮助视频编辑不那么可怕

> 原文：<https://www.xda-developers.com/vulkan-video-api-speed-up-video-editors/>

Vulkan API 在 2016 年首次发布时是计算机图形学的一个重要里程碑。它为微软的 DirectX 框架提供了一个跨平台的竞争对手，成为老化的 OpenGL 架构的真正继承者。Vulkan 1.2 在一年多前完成[，现在一个小的更新引入了新的东西——视频支持。](https://www.xda-developers.com/khronos-vulkan-graphics-api-1-2/)

Vulkan 图形 API 的维护者克罗诺斯集团[今天](https://www.khronos.org/blog/an-introduction-to-vulkan-video)宣布临时的 Vulkan 视频加速扩展已经准备好供开发者试用。这些技术统称为“Vulkan Video”，为游戏和应用程序提供处理视频的低级 API。该小组在公告中写道，“利用现有的 Vulkan 框架，可以高效、低延迟、低开销地使用处理资源，包括在多个 CPU 内核和视频编解码器硬件之间分配流处理任务——所有这些都具有跨多个平台和设备(从小型嵌入式设备到高性能服务器)的应用可移植性。”

这些都是大话，但总的目标是给处理视频的应用程序(视频编辑器，网络浏览器，文件转换器等。)Vulkan 为游戏和图形工具提供的一些相同功能。这包括底层硬件优化、标准化 API 以及 Windows 和 Linux 的开源代码示例。Vulkan Video 已经支持 H.264 视频的编码和解码，VP9、AV1 和 H.265 兼容性预计将很快实现。

然而，Vulkan 视频还远未完成。克罗诺斯目前正在寻求开发者的反馈，新的 API 可以使用 NVIDIA 的 beta Vulkan 驱动程序进行测试。“Khronos 现在将致力于最终确定 Vulkan Video 1.0 规范、SDK 和一致性测试，因此重点可以转向支持其他编解码器和更高级的视频功能，”该组织在一篇博客文章中说。