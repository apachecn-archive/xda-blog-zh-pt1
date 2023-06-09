# 适用于桌面平台和 Android 的 Firefox 91 有什么新功能

> 原文：<https://www.xda-developers.com/firefox-91/>

# Firefox 91 带来了改进的 cookie 保护、Android 上的标签变化等等

Firefox 91 开始推出，桌面上有默认的 HTTPS 和 cookie 改进，Android 上有新的默认行为。

Firefox 是少数几个拥有自己渲染引擎的浏览器之一，Opera、Brave、Edge 和其他浏览器现在都使用谷歌的 Chromium 引擎。然而，Mozilla 在保持 Mozilla 与其他浏览器的竞争力方面并没有太大的困难，因为 Firefox 在现实世界中的速度与 Chrome 和 Edge 相当。上个月，Firefox 90 推出了新的渲染功能和保存信用卡信息的能力，现在 Firefox 91 也开始推出。

桌面上的 Firefox 91 更新了浏览器的总 Cookie 保护，将 Cookie 限制在创建它们的网站上，修复了各种数据泄漏和其他改进。默认情况下，Mozilla 还打开了 HTTPS，它试图通过 HTTPS 加载所有内容，除非失败(然后它会通过不安全的 HTTP 再次尝试)。早在 6 月份，谷歌就开始为 Chrome [测试类似的功能。](https://www.xda-developers.com/google-chrome-prepares-https-only-mode/)

### Firefox 91 桌面变更日志

*   在全面 Cookie 保护的基础上，我们添加了一个更全面的逻辑来清除 Cookie,防止隐藏的数据泄露，并使用户可以轻松了解哪些网站存储了本地信息。
*   Firefox 现在支持使用 Windows 单点登录登录微软、工作和学校账户[。](https://support.mozilla.org/kb/windows-sso)
*   打印时简化页面功能[又回来了](https://support.mozilla.org/kb/print-friendly-pages-firefox-clutter-free-printing)！打印时，在“更多设置”>格式下，选择简化选项(如果可用),以获得整洁的页面。
*   HTTPS 第一政策:Firefox 的私人浏览窗口现在试图使所有网站连接安全，只有当网站不支持时才回到不安全的连接。
*   地址栏现在也可以在私人浏览窗口中切换到标签结果。
*   当在 MacOS 上选中“增加对比度”时，Firefox 现在会自动启用高对比度模式
*   Firefox 现在对几乎所有的用户交互都进行了补绘，使大多数用户交互的响应时间提高了 10-20%。
*   桌面平台现在支持[可视视窗 API](https://developer.mozilla.org/docs/Web/API/Visual_Viewport_API) 。
*   苏格兰语(sco)已被添加为区域设置。
*   修正了各种[安全问题](https://www.mozilla.org/security/advisories/mfsa2021-33/)。

### 火狐 91 安卓变更日志

*   新安装的浏览器会在通知面板上显示“将 Firefox 设为默认浏览器”的信息。
*   增加了易贝搜索来帮助用户满足他们的购物需求。
*   为了改进选项卡导航，选项卡托盘的默认布局从列表视图更改为网格视图。
*   默认自动播放设置已更新为仅阻止音频。
*   选择退出遥测现在也将删除所有以前收集的使用数据。
*   三星键盘上的密码字段不再自动以大写字母开头
*   修正了各种[安全问题](https://www.mozilla.org/security/advisories/mfsa2021-33/)。

[Android 浏览器](https://www.mozilla.org/en-US/firefox/android/91.0/releasenotes/)现在使用网格视图作为标签托盘的默认布局，但是列表视图选项没有任何用处。易贝现在也可以作为一个搜索引擎选项，就像桌面应用程序已经提供了一段时间。最后，Firefox for Android 在默认情况下匹配 Chrome 在自动播放视频中阻止音频的行为，而不是阻止视频*和*音频自动播放。

可以从[浏览器官网](https://www.mozilla.org/en-US/firefox/new)下载桌面平台的 Firefox。安卓版本在谷歌 Play 商店的[有售。](https://play.google.com/store/apps/details?id=org.mozilla.firefox)