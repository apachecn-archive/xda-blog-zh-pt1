# 面向桌面和网络的 JetBrains Compose 现已发布

> 原文：<https://www.xda-developers.com/jetbrains-compose-multiplatform-alpha/>

如果你没听说过 [Jetpack Compose](https://www.xda-developers.com/jetpack-compose-google-ui-toolkit-android-alpha/) ，那你最近去哪里了？Google 创建了这个声明式 UI 框架来取代 Android 中的标准 XML 布局引擎。Compose 允许开发人员在 Kotlin 中创建他们的布局和伴随的逻辑。Kotlin 背后的 JetBrains 公司也加入了 Compose 行动，并致力于将其移植到桌面和网络上。

JetBrains Compose for Desktop and Web 已经开发了一段时间了。它有一个公开的 pre-alpha“技术预览版”,开发者可以使用它在 Compose 中创建跨平台的应用程序。我个人已经在我的三星固件下载器应用程序中使用了它，它运行得相当好。

今天，JetBrains 正在向 alpha 推广它的 Compose 版本。这意味着一个更稳定的 API，以及一些新的特性和变化。

## 为 Web 撰写

首先，网络。Web 版的 Compose 甚至比桌面版的 Compose 还要新，而且它缺少了很多东西。不过，这并不意味着它毫无用处。虽然开发人员可能无法获得桌面和 Android 可用的花哨的核心 UI 元素，但开发人员仍然可以获得用 Kotlin 编写声明式设计原则的好处。

现在 Compose 处于 alpha 阶段，Web API 应该更加稳定，随着时间的推移，即使有，也会有更少的破坏性更改。

## 撰写窗口管理

回到桌面，开发者在应用程序中与 windows 交互的方式发生了一些变化。

第一个是新的[可组合窗口 API](https://github.com/JetBrains/compose-jb/tree/master/tutorials/Window_API_new) 。这使得开发人员可以在他们的应用程序中以声明的方式与窗口进行交互。例如，窗口标题现在可以用状态来改变，窗口甚至可以根据状态来打开和关闭。

新窗口 API 的另一部分允许开发人员选择以自适应(而不是固定)大小打开新窗口。这意味着 Compose 会根据窗口的内容计算出窗口需要有多大，自动设置初始大小，然后打开窗口。

## 插件

JetBrains Compose 一直有一个 Gradle 插件来执行编译和执行。随着 alpha 的发布，这个插件将会有一个版本升级，同时还会有一些错误修正。

然而，在 Gradle 插件之上，现在有一个 IntelliJ IDEA 和 Android Studio 的 IDE 插件来更好地支持桌面和 Web 的 Compose。与 Android 的 Compose 类似，这个插件允许开发人员将可组合函数注释为预览，并直接在 IDE 中查看布局预览。

这个插件现在非常简单。它目前唯一的另一个特性是消除了 IDE lint 关于对可组合函数名使用大小写的警告。但随着时间的推移，它将获得更多的功能，如实时预览。

## 架构支持

尽管 JetBrains Compose 的目标是跨平台的，但它还没有完全支持所有的 CPU 架构。alpha 将当前支持扩展到以下内容:

*   macOS: x86-64 (amd64)，arm64
*   Windows: x86-64 (amd64)
*   Linux: x86-64 (amd64)，arm64
*   Web:最近有什么消息吗

虽然这肯定不能涵盖所有方面，但支持在未来只会越来越好。

## 未来发展

JetBrains 选择让 Compose 进入 alpha 状态是很重要的。这意味着他们计划继续开发，最终会有测试版和稳定版。当然，还有更多功能。

## 结论

看到 Compose 能带来什么是非常令人兴奋的。在 Android 上，它取代了一个过时的(尽管完全可用)布局引擎。在桌面和 Web 上，它使用比基于类型脚本的语言更容易使用(至少对我来说)的强类型语言带来了声明式设计。尤其是在桌面上，Compose 有助于填补功能布局引擎的一个相当大的空白。

如果你有兴趣尝试 JetBrains Compose yourself，[查看 GitHub 库](https://github.com/JetBrains/compose-jb)了解更多关于如何开始的细节。