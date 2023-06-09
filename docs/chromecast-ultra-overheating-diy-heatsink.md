# PSA: Chromecast 过热问题可以通过 DIY 散热器解决

> 原文：<https://www.xda-developers.com/chromecast-ultra-overheating-diy-heatsink/>

直到最近，谷歌 Chromecast Ultra 一直是该系列的旗舰产品，这在很大程度上要归功于其 4K 功能和以太网连接，这使其成为该公司 Stadia 游戏服务的天然合作伙伴。问题是，那种资源密集型的渲染会让 Chromecast Ultra 运行起来有点热。嗯，好吧，很热。事实上，大约四个小时后，它变得过热而关闭，并且没有任何明显的警告——如果你要击败一个等级老板，这不是理想的。在某些情况下，当您的控制器开始随机出错并失去连接时，您会得到一些线索，但这仍然不理想。幸运的是，有一个解决方案。

 <picture>![Chromecast Ultra with Heatsink](img/959954a431907612ce7557466bd1b740.png)</picture> 

Credits: Redditor [JamesStrang1](https://www.reddit.com/user/JamesStrang1)

一位名叫 [Jamesstrang1](https://www.reddit.com/r/Stadia/comments/jod2an/rate_my_ccu_heat_sink_setup/) 的 Redditor 发布了他如何使用一个简单的散热器的细节，这种散热器可以在网上花几美元买到，用导热胶带(通常包括在内)将一些多余的温度从设备中带走。然后，将一个便宜的 USB 风扇(同样，价值几美元)插入电视背面的 USB 端口，带走的热量就会消散。正如设计师指出的那样，通过从电视的 USB 为风扇供电，它只在需要时运行——当电视打开时。鉴于 Marvell Armada SoC 应该能够应对超过 100c 的工作温度，因此自 Stadia 问世以来，内置缓解措施一直未能应对也就不足为奇了。为了证明这不是侥幸或软件修复，海报的另外两个没有经过定制散热器处理的 Chromecast Ultra 单元仍然失败——这一个不是。

YouTuber Spawn Wave 也在这方面用 Raspberry Pi 散热器进行了一些测试，甚至只是简单地粘上一个小散热器就开始在 Chromecast Ultra 模块内产生温度差异。

虽然令人沮丧的是，谷歌最贵的 Chromecast 变种和推荐给 Stadia 的版本有如此明显的设计缺陷，但令人欣慰的是，解决方案既简单又便宜。

*特色图片鸣谢:Redditor[James strang 1](https://www.reddit.com/user/JamesStrang1)*