# 奇异果浏览器准备自动更新到最新的铬版本

> 原文：<https://www.xda-developers.com/kiwi-browser-next-chromium-updates/>

有很多第三方网络浏览器，其中很多都使用 Chromium 作为基础。安卓上可用的一个这样的浏览器叫做[奇异果浏览器](https://www.xda-developers.com/tag/kiwi-browser/)，由 XDA 资深会员[阿诺 42](https://forum.xda-developers.com/m/arnaud42.9196003/) 开发。Kiwi 面向高级用户，具有内置广告拦截器、加密劫持保护等功能，最重要的是支持扩展，这是大多数基于 Chromium 的浏览器——尤其是谷歌 Chrome 本身——在移动设备上缺乏的功能。

对于一个独立开发者来说，维护一个在很多方面偏离主代码库的 Chromium 分支并不容易，这就是为什么 Kiwi 浏览器的更新一直很慢，底层 Chromium 版本也没有与谷歌的版本同步。自从谷歌最近从 6 周的时间表[转移到 4 周的时间表](https://www.xda-developers.com/chrome-updates-will-now-be-released-every-4-weeks/)以来，跟上 Chromium 的发布周期变得更加困难。然而，这种情况可能会很快改变，因为 Kiwi 浏览器的未来更新将自动包含最新的 Chromium 版本。

## Kiwi Next 的自动发布

这要归功于开发人员在一个名为“奇异果下一个”的项目中所做的工作，这个项目就是“奇异果浏览器用最新的铬自动重定基础。”开发人员告诉我们，他一直在开发脚本和自动化工具，以便更有效地遵循新的 Chromium 发布周期。这将有望使奇异果与最新的铬版本保持同步，这样用户就不会错过关键的错误修复或新的浏览器功能。由于合并产生的代码冲突，自动重定基准可能会导致无法预见的错误或中断，但是开发人员似乎已经找到了如何在最新 chrome 版本的基础上快速集成现有代码的方法。

## 基于 Chromium 93 的奇异果浏览器

除了奇异果下一个项目之外，开发者还一直致力于推出奇异果浏览器应用的一个新的重大更新。最新的更新基于 Chromium 版本 93.0.4577，因此与网站的兼容性和性能都有了显著提高，这要归功于谷歌在过去几个月里所做的所有改进。更新还带来了增强的内容拦截器、新的开发工具、对一系列点击故障问题的纠正、对一系列白页的修复、新的夜间模式(使用安卓的黑暗主题系统和 Chrome 的“网络内容强制黑暗模式”)和新的通知管理系统。

因为更新是基于最新的 Chromium 版本，遗留的垂直标签切换器[已经完全从代码库中移除了](https://www.xda-developers.com/google-chrome-91-stable-rollout/)。Kiwi dev 在设置中为那些完全讨厌新标签系统的人添加了他们自己的垂直标签切换器选项，但请注意，这不是 1:1 的替代。

你现在就可以在谷歌 Play 商店上查看奇异果浏览器[的最新更新。Play Store 版本的大小只有 49MB，因为开发者告诉我们他已经改用新的交付机制，但如果你从其他来源获取更新，它的大小将超过 150MB。](https://play.google.com/store/apps/details?id=com.kiwibrowser.browser)

**[XDA 奇异果浏览器论坛帖子](https://forum.xda-developers.com/t/app-4-1-kiwi-browser-chromium-adblock-caf-night-mode-2020-04-17-active.3797252/)**