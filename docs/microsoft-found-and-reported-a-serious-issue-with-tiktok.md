# 微软在抖音安卓应用中发现了一个漏洞

> 原文：<https://www.xda-developers.com/microsoft-found-and-reported-a-serious-issue-with-tiktok/>

Android 抖音应用程序有一个严重的安全问题，是微软报告的。该公司最近向网络安全社区详细介绍了这一发现，表明这一高严重性漏洞可能允许攻击者只需点击一下鼠标即可危及账户安全。抖音也收到了微软关于这个问题的通知，并且已经得到了修补。

根据微软的说法，这个特定的漏洞影响了 Android 23 . 7 . 3 和更低版本的抖音，需要几个问题链接在一起才能利用，并且没有在野外使用。这意味着没有人可能受到它的影响。Android 上实际上有两个版本的抖音，一个用于东亚和东南亚，另一个用于世界其他地区。微软进行了漏洞评估，发现两者都受到了影响，这意味着该漏洞影响了总共 15 亿次安装。

然而，利用这个漏洞，黑客可以在用户不知道用户是否点击了某个链接的情况下，劫持一个基于安卓系统的抖音账户。攻击者可能已经访问了受损的抖音个人资料，让他们看到私人视频，发送消息，或上传视频。

那么，攻击者是如何利用这个漏洞的呢？据微软称，抖音安卓应用允许绕过应用的 deeplink 验证。攻击者可以强迫应用程序加载应用程序 WebView 的 URL。这将允许该 URL 中的页面访问 WebView 的 JavaScript 桥，从而为黑客提供更多功能和 70 种快速访问用户信息的方式。攻击者还可以通过触发对受控服务器的请求并记录 cookie 和请求头来检索用户的身份验证令牌。

微软[过去曾报道过这个 JavaScript bridges 问题](https://www.microsoft.com/security/blog/2022/05/27/android-apps-with-millions-of-downloads-exposed-to-high-severity-vulnerabilities/)，而[CVE 的一篇文章](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2022-28799)提供了这个抖音漏洞的更多细节。该公司于 2022 年 2 月通过微软安全漏洞研究中心( [MSVR](https://www.microsoft.com/en-us/msrc/cvd?rtc=1) )通过协同漏洞披露(CVD)报告了这一问题，并在披露一个月后由抖音修补。微软认为，这种情况表明，在技术行业中协调研究和威胁情报是多么重要。

**来源:** [微软](https://www.microsoft.com/security/blog/2022/08/31/vulnerability-in-tiktok-android-app-could-lead-to-one-click-account-hijacking/)