# Firefox 87 更新为 HTTP Referrer 策略带来了智能阻止和更新

> 原文：<https://www.xda-developers.com/firefox-87-smart-block-update/>

Firefox 已经收到了一个新的更新，升级到 87 版。在 2 月收到[更新后，新版本带来了两个重要的特性:智能阻止和改进的引用修剪。](https://www.xda-developers.com/firefox-86-total-cookie-protection/)

Firefox 默认情况下会阻止第三方跟踪脚本，虽然它运行得很好，但在某些情况下，脚本不会被跟踪。这可能会干扰页面的呈现，导致页面延迟或完全中断。通过 Smart Block，Firefox 增加了一个额外的步骤，即嵌入第三方跟踪器的页面可以正确呈现。Mozilla 在其[安全博客](https://blog.mozilla.org/security/2021/03/23/introducing-smartblock/)中表示:“SmartBlock 智能修复被我们的跟踪保护破坏的网页，而不会损害用户隐私。”。

通过提供与 Firefox 捆绑在一起的本地插件，浏览器提供了行为与原始脚本一样的脚本，以确保网站正常工作。这有助于打破依赖原始脚本加载的网站，而不会影响其功能。作为额外的安全措施，追踪器不会加载任何第三方内容，因此不可能追踪到你。Firefox 还确保这些替身不包含任何支持跟踪功能的代码。

新的 [Firefox 87 更新](https://www.mozilla.org/en-US/firefox/87.0/releasenotes/)也增加了关于 HTTP referrer 头的严格规则。传统上，浏览器在 HTTP Referrer 头中发送引用文档的完整 URL(通常是地址栏中的 URL ),几乎包含每个导航或子资源(图像、样式、脚本)请求。这些信息可用于各种用途，包括分析、日志记录或优化缓存。HTTP Referrer 标头通常包含私人用户数据，例如，用户在推荐网站上阅读的文章，甚至包括用户在网站上的帐户信息。最新的更新将把默认的推荐策略设置为“严格起源-交叉起源”,这将减少用户在 URL 中可以访问的敏感信息。它将整理从 HTTPS 到 HTTP 的请求信息，并整理所有跨源请求的路径和查询信息。

新的 Firefox 87 更新还将对“在页面中查找”的“突出显示全部”功能进行改进，在该功能中，勾选标记将显示在与该页面上找到的匹配位置相对应的滚动条旁边。还将全面支持 macOS 的内置屏幕阅读器 VoiceOver 和各种其他小的 UI 增强功能，以及安全性和常规调整。