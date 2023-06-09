# 谷歌信息准备添加类似 Gmail 的“轻推”

> 原文：<https://www.xda-developers.com/google-messages-preparing-nudges-feature/>

早在 2018 年，谷歌就在 Gmail 中添加了“轻推”功能，提醒你跟进该服务认为重要的电子邮件。我们发现有证据表明，谷歌正计划在 Android 的谷歌消息应用程序中添加类似的功能。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

谷歌消息应用程序 9.5 测试版最近在谷歌 Play 商店推出，它包括即将到来的“轻推”功能的新字符串，谷歌计划将其添加到其消息应用程序。我们反编译了 APK，发现了下面的字符串，它们清楚地描述了这个特性是如何工作的。

```
 <string name="nudge_continuation_enabled_pref_key">nudge_continuation_enabled</string>
<string name="nudge_continuation_enabled_pref_summary">Messages you might need to follow up on will appear at the top of your inbox</string>
<string name="nudge_continuation_enabled_pref_title">Suggest messages to follow up on</string>
<string name="nudge_learn_more_info_text">%1$s about nudges</string>
<string name="nudge_learn_more_pref_key">nudge_learn_more</string>
<string name="nudge_reply_enabled_pref_key">nudge_reply_enabled</string>
<string name="nudge_reply_enabled_pref_summary">Messages you might have forgotten to respond to will appear at the top of your inbox</string>
<string name="nudge_reply_enabled_pref_title">Suggest messages to reply to</string>
<string name="nudge_settings_page_title">Nudges</string>
<string name="nudge_settings_parent_pref">nudge_settings_parent</string> 
```

一旦你启用了“轻推”，该应用将自动在你的收件箱顶部显示“你可能忘记回复的邮件”。同样，这款应用还会将你的注意力吸引到“你可能需要跟进的信息”上

下面附上的截图显示了“轻推”的设置页面在发布时的样子:

“信息”应用已经可以让你[手动设置提醒来回复你认为重要的文本](https://www.xda-developers.com/google-messages-5-2-adds-chat-reminders-prepares-support-bubble-notifications-suggested-stickers/)，但如果有一个自动化系统也不错。

请注意，“轻推”功能还没有开始向用户推出。我们不知道谷歌计划何时公开它。假设谷歌不放弃它，这项功能很可能会先出现在测试频道，然后再向所有人推广。如果你想成为第一个试用它的人，你可以[加入 Messages](https://play.google.com/apps/testing/com.google.android.apps.messaging) 的测试程序。

在过去的几个月里，Google Messages 增加了几个新功能，比如[标记重要消息的能力](https://www.xda-developers.com/google-messages-categories-auto-delete-otps/)、[人工智能支持的消息排序、自动 OTP 删除](https://www.xda-developers.com/google-messages-categories-auto-delete-otps/)等等。