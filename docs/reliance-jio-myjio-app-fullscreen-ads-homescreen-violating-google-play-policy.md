# Jio 的 MyJio 应用向主屏幕发送全屏广告，违反了 Google Play 政策

> 原文：<https://www.xda-developers.com/reliance-jio-myjio-app-fullscreen-ads-homescreen-violating-google-play-policy/>

除非你一直生活在印度的岩石下，否则你可能听说过 Reliance Jio——这家运营商几乎在一夜之间[改变了印度的 4G 格局](https://www.xda-developers.com/reliance-jio-crosses-100-million-subscribers-in-india-in-5-months-launches-jio-prime-subscription-plan/)，现在[也将目光投向了 5G](https://www.xda-developers.com/reliance-jio-enter-india-5g-market-early-2021/) 。作为印度领先的电信服务提供商，Jio 已经为自己找到了一个具体的空间，到 2020 年底将聚集超过 4 亿用户。基于该国的智能手机市场，可以有把握地认为，这些用户中有相当多的人是在安卓智能手机上使用 Jio 的服务的。如果你是这样一个用户，你可能不得不在最近的过去与你的主屏幕上的全屏横幅广告作斗争。事实证明，它们是由配套的 [MyJio 应用](https://play.google.com/store/apps/details?id=com.jio.myjio)直接交付的，这直接违反了 Google Play 的政策。

在 Android 智能手机上，你只需插入 Jio sim 卡，就可以立即开始使用电信的服务。但是，如果你使用 Jio 的其他服务，如 JioFiber connection，或者你想查看目前为止你每天消耗了多少数据，或者你想给你的数据包充值，那么你需要在你的手机上安装 MyJio companion 应用程序。MyJio 应用程序是“充电、UPI 和支付、管理 Jio 设备、电影、音乐、新闻、游戏、测验等的一站式目的地”。不用说，如果你已经涉足 Jio 生态系统(如果你住在印度还没有，我会很惊讶)，你的设备上已经安装了这个应用程序。

不幸的是，MyJio 应用程序有一个相当恼人的习惯，那就是将全屏广告横幅直接发送到用户的主屏幕上。

这个广告横幅是由我的[三星 Galaxy S21 Ultra](https://www.xda-developers.com/samsung-galaxy-s21/) 上的 MyJio 应用程序发起的，那是当时手机上唯一的 Jio 应用程序。这款应用在那时已经有几天没有出现在前台了，但是这个横幅通知劫持了主屏幕。环顾四周，我发现这种情况已经发生了好几个月了，许多用户抱怨主屏幕被劫持。点击横幅，你会看到这个[预先生成的 WhatsApp 消息](https://wa.me/917000770007/?text=hi)，给提到的号码发短信。

我们很难有意识地触发弹出横幅。我们已经检查了该应用程序，有迹象表明，当切换飞行模式和拔掉设备的充电插头时，会触发横幅。但是这些常见的动作并不是每次都会触发横幅，它出现的频率也很低。我们假设 Firebase 通知接收器上还设置了更多的触发器，在我们的测试中可能没有满足这些触发器的条件。

初步看来，这种劫持行为是由应用程序从后台启动的全屏活动引起的。这直接违反了 Google Play 的广告政策:

> ### 干扰应用程序、第三方广告或设备功能
> 
> 与您的应用程序关联的广告不得干扰其他应用程序、广告或设备的操作，包括系统或设备按钮和端口。这包括覆盖、配套功能和 widgetized 化广告单元。广告只能在为其服务的应用程序中显示。

谷歌谈到的例子与 MyJio 应用程序演示的行为非常相似。我们可以得出结论，MyJio 应用程序通过劫持主屏幕推出显示在其应用程序外部的广告，直接违反了 Google Play 政策。

奇怪的是，该应用程序能够在没有获得“显示在应用程序上”/“出现在顶部”的许可的情况下推送这一劫持广告。MyJio 应用程序甚至没有请求这种许可，所以我非常好奇该应用程序如何在主屏幕上推送广告。

在扎卡里的帮助下，我挖得更深了。我们发现该应用程序集成了 MADME SDK，并且有名为“OverlayAdActivity”的活动，这使得人们对其意图几乎没有怀疑的余地。

访问 [Madme 的网站](https://www.mad-me.com/solutions)证实了我们的发现，因为他们自豪地展示了电信解决方案，推出这些带有劫持意图的弹出广告横幅。

MyJio 应用程序集成了 Madme 的一系列活动、服务和接收者，而且数量太多了。

有几种方法可以摆脱这些劫持弹出窗口。第一个也是最明显的解决方案是简单地卸载 MyJio 应用程序。很多用户很少使用这款应用，你可以在需要的时候重新安装。在这中间的周期里，你至少不会因为离开主屏幕而感到烦恼。

互联网广泛建议的第二种解决方案是禁用应用程序的所有权限。与第一个解决方案非常相似，这是一个非常广泛的解决方案，将导致应用程序的某些功能无法正常工作。

第三种解决方案采用了更精确的方法，但是也需要 root。您可以使用类似于 [Root Activity Launcher](https://play.google.com/store/apps/details?id=tk.zwander.rootactivitylauncher) 的应用程序来禁用 Jio 应用程序中与 Madme SDK 相关的所有活动、服务和接收器。

这里是所有相关的活动、服务和接收者。请注意，您可能不需要禁用所有这些功能，我只是列出了我能发现的所有功能。在我们这边很难强制触发全屏弹出窗口，所以我们还是要用一种全面的方法。

*   活动:
    *   com . mad me . mobile . SDK . activity . ad activity
    *   com . mad me . mobile . SDK . activity . adlist activity
    *   com . mad me . mobile . SDK . activity . browseractivity
    *   com . mad me . mobile . SDK . activity . madmecmclickactivity
    *   com . mad me . mobile . SDK . activity . madmepermissionactivity
    *   com . madme . mobile . SDK . activity . myoffershistoryactivity
    *   com . mad me . mobile . SDK . activity . overlayadeactivity
    *   com . mad me . mobile . SDK . activity . overlaysurveyactivity
    *   com . mad me . mobile . SDK . activity . change profile activity
    *   com . mad me . mobile . SDK . activity . savedadactivity
    *   com . mad me . mobile . SDK . activity . survey 活动
    *   com . mad me . mobile . SDK . activity . thankyouactivity
    *   com . mad me . mobile . SDK . activity . webview activity
    *   com . mad me . mobile . SDK . activity . legalinformationactivityresources
    *   com . madme . mobile . SDK . activity . terms activity
    *   com . mad me . mobile . SDK . activity . benefits 活动
*   服务:
    *   com . mad me . mobile . SDK . service . ad . showad service
    *   com . madme . mobile . SDK . service . adalarmhelperservice
    *   com . mad me . mobile . SDK . service . adreminderhelperservice
    *   com . madme . mobile . SDK . service . adtriggereventsservice
    *   com . mad me . mobile . SDK . service . campaignhelperservice
    *   com . mad me . mobile . SDK . service . cdncampaignjobservice
    *   com . mad me . mobile . SDK . service . cdncampaignservice
    *   com . madme . mobile . SDK . service . cloud messaging . cloudmessagingregistrationservice
    *   com . mad me . mobile . SDK . service . dbupdateservice
    *   com . madme . mobile . SDK . service . download service
    *   com . mad me . mobile . SDK . service . location . geofenceservice
    *   com . mad me . mobile . SDK . service . log in service
    *   com . mad me . mobile . SDK . service . LSF service
    *   com . mad me . mobile . SDK . service . lsjobservice
    *   com . mad me . mobile . SDK . service . lsjobservice 2
    *   com . mad me . mobile . SDK . service . ls service
    *   com . mad me . mobile . SDK . service . MFA service
    *   com . mad me . mobile . SDK . service . SBS tservice
    *   com . mad me . mobile . SDK . service . surveysubmissionjobservice
    *   com . mad me . mobile . SDK . service . surveysubmissionservice
    *   com . mad me . mobile . SDK . service . tracking service
    *   com . mad me . mobile . SDK . service . trackingsubmissionjobservice
    *   com . mad me . mobile . SDK . service . trackingsubmissionservice
*   接收器:
    *   com . mad me . mobile . SDK . broadcast . adalarmreceiver
    *   com . mad me . mobile . SDK . broadcast . adreminderreceiver
    *   com . mad me . mobile . SDK . broadcast . ad triggers . airplanemodechangedad trigger
    *   com . mad me . mobile . SDK . broadcast . ad triggers . powerconnectionadtrigger
    *   com . madme . mobile . SDK . broadcast . ad triggers . roamingadtrigger
    *   com . mad me . mobile . SDK . broadcast . ad triggers . wifi adtrigger
    *   com . madme . mobile . SDK . broadcast . ad triggers . wifi available trigger
    *   com . mad me . mobile . SDK . broadcast . boot receiver
    *   com . mad me . mobile . SDK . broadcast . daily task receiver
    *   com . madme . mobile . SDK . broadcast . EOC trigger
    *   com . mad me . mobile . SDK . broadcast . geofence receiver
    *   com . mad me . mobile . SDK . broadcast . idsns receiver
    *   com . madme . mobile . SDK . broadcast . madmesmstrigger
    *   com . mad me . mobile . SDK . broadcast . notificationactiontrigger
    *   com . mad me . mobile . SDK . broadcast . package removal receiver
    *   com . mad me . mobile . SDK . broadcast . unlock receiver

禁用所有这些将有效地使 Madme SDK 无用，并应防止横幅再次劫持您的主屏幕。

谷歌 Play 商店上的应用程序已经因为更加无辜的行为而被移除，这让我很惊讶，Madme SDK 和 Jio 的主屏幕广告行为以前没有被发现、强调和解决。Madme 肯定没有隐藏它的所作所为，他们自豪地强调这种行为是一个卖点，让我们集体挠头，他们想出了哪个漏洞来获得这样的信心和假定的豁免权。如果他们的网站是可信的，印度的其他电信提供商也使用他们的服务，尽管我们还没有遇到他们的主屏幕劫持广告横幅。

我们希望谷歌认识到这些弹出窗口的主屏劫持行为，并澄清它们与 Google Play 政策的存在。