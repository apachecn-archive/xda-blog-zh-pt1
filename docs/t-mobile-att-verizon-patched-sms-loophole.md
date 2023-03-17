# T-Mobile、美国电话电报公司和威瑞森已经堵住了一个短信劫持漏洞

> 原文：<https://www.xda-developers.com/t-mobile-att-verizon-patched-sms-loophole/>

你可能读过几周前的几篇新闻，关于一种可怕的短信劫持攻击，这种攻击也很容易被任何人实施。基本上，使用一家名为 Sakari 的公司提供的服务，旨在帮助企业进行短信营销，可以让你接管某人的号码，并将他们的短信重定向到你这里:不问任何问题，受害者甚至不会收到通知，这项服务最便宜的计划只需 16 美元。[这份来自*主板*](https://www.vice.com/en/article/y3g8wb/hacker-got-my-texts-16-dollars-sakari-netnumber) 的报告揭露了一个巨大的漏洞:如果你使用的是使用短信作为认证方法的东西，黑客只需支付 16 美元就可以重新路由你的信息。不过，你现在可以高枕无忧了，因为 T-Mobile、AT & T 和威瑞森都已经修补了这个漏洞。

这是由 Aerialink(通过 [*主板*](https://www.vice.com/en/article/5dp7ad/tmobile-verizon-att-sms-hijack-change) )宣布的，这是一家帮助路由短信的通信公司。公告本身写道，“号码注册局已宣布无线运营商将不再支持其各自无线号码上的短信或彩信文本功能，”并补充说，这一变化是全行业的，影响到美国生态系统中的所有短信提供商，包括美国三大运营商:AT & T、T-Mobile 和威瑞森，以及依赖这三家公司的手机基础设施的运营商。

官方声明接着补充说，这三家公司已经“在全行业范围内回收了被覆盖的支持文本功能的无线号码”，因此，“BYON 支持文本功能的无线号码不再通过 Aerialink Gateway 路由消息流量，”指的是大多数运营商必须允许你在不获得新电话号码的情况下更换手机提供商的“自带号码”功能。这意味着无线 BYON 号码将不再通过 Aerialink 网关发送短信。这些变化中的大部分也意味着像 Sakari 这样提供改线服务的公司可能无法再正常提供这些服务。

这个漏洞的出现需要对 SMS 文本消息如何通过运营商路由进行认真的修改，我们很高兴看到这个问题正在得到解决。不过，最好的做法是不要依赖短信作为你的双重身份认证选项:提供一次性密码的应用程序，如 Authy 和 Google Authenticator，甚至更安全的方法，如硬件密钥，都是更安全的选择，可以在我们进入互联网时代时保护你的在线帐户安全。