# 谷歌的睡眠 API 帮助开发者构建更好的睡眠跟踪应用

> 原文：<https://www.xda-developers.com/google-sleep-api-sleep-tracking/>

谷歌推出了一种新的睡眠 API，开发者可以使用它来显示用户的睡眠信息，从而产生更高级的睡眠跟踪应用程序。睡眠 API 现在作为最新版本的 Google Play 服务的一部分提供。

根据谷歌的说法，睡眠 API 是一个“简单的 API，它以节省电池的方式集中了睡眠检测处理。”这是谷歌 [Android 活动识别](https://www.xda-developers.com/apk-google-play-services-4-4-brings-street-view-api-activity-recognition-game-services-update-wallet-fragments-and-more/) API 的一部分，可以用来检测用户的活动，比如他们是骑自行车还是走路。

“我们做的很多事情都依赖于良好的夜间休息，”谷歌说。“我们的手机已经成为对我们的睡眠做出更明智决定的伟大工具。通过了解睡眠习惯，人们可以在一天中就睡眠做出更好的决定，这会影响注意力和心理健康。”

睡眠 API 将使用设备上的机器学习模型，根据来自手机光线和运动传感器的输入来推断用户的睡眠状态。谷歌表示，其新的 API 将使开发者不必花时间开发自己的方法来确定用户何时开始或结束睡眠。此外，与其他睡眠跟踪 API 相比，使用谷歌的 API 还有其他优势，包括需要更少的电力，并在数据收集方面提供更多的可靠性。后者尤为重要，因为与第三方应用相比，Google Play 服务受 Doze 和其他电池管理服务的影响较小。

一旦收集了信息，就会以两种方式进行报告:

1.  “睡眠信心”，定期报告(最多 10 分钟)
2.  检测到唤醒后报告的每日睡眠段

在其博客文章中，谷歌强调了一款名为 Sleep 的安卓应用，该应用使用了新的 Sleep API。该应用程序可以跟踪睡眠持续时间、规律、阶段、打鼾等信息，由于切换到睡眠 API，功耗比以前更低，可靠性更高。“睡眠时长是确保良好睡眠的最重要参数之一，”睡眠机器人团队表示。“新的睡眠 API 为我们提供了一个绝佳的机会，让我们能够以最有效的方式自动跟踪睡眠。”

(顺便说一下，Sleep as Android 团队[创建了 DontKillMyApp 网站](https://www.xda-developers.com/phone-software-killing-apps-background/)来强调积极的 OEM 电源管理服务如何不断扼杀他们应用程序的睡眠跟踪服务。)

第三方应用目前使用谷歌的新睡眠 API，但需要提示用户授予 ACTIVITY_RECOGNITION 权限。这确保了用户可以控制哪些应用程序可以跟踪他们的睡眠。感兴趣的开发者可以通过查看谷歌的 API 文档来了解更多关于 Sleep API 的信息。