# 谷歌信息将于 4 月份停止在未经认证的安卓手机上运行

> 原文：<https://www.xda-developers.com/google-messages-stop-working-uncertified-android-phones-april-2021/>

# 谷歌信息将于 4 月份停止在未经认证的安卓手机上运行

最新的谷歌消息应用程序中的一个新字符串表明，该应用程序将在 2021 年 4 月停止在未经认证的安卓智能手机上工作。

谷歌消息是谷歌最受欢迎的应用之一，许多用户每天都在使用它，甚至没有意识到他们在使用它。这个名字很普通，很多设备都预装了它作为默认的 SMS 和 RCS 客户端。大多数用户应该对应用程序提供的功能感到满意，没有真正的理由去探索替代品。但如果其中一个可能即将到来的变化成为现实，他们可能需要寻找替代方案，因为应用程序中的新字符串表明，谷歌消息将在 2021 年 4 月停止在未经认证的安卓手机上工作。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

在谷歌信息 7.2.203 中发现了一个新的字符串:

```
 <string name="ip_compliance_warning_message">On March 31, Messages will stop working on uncertified devices, including this one.</string> 
```

正如消息中明确指出的，从 2021 年 3 月 31 日起，消息将停止在未经认证的 Android 设备上工作。未经认证的 Android 设备是那些运行在 Android 上，但跳过或未通过谷歌官方对谷歌移动服务的认证过程的设备。这些设备没有附带强制性的谷歌应用程序，但这些设备的卖家通常会就用户如何下载谷歌应用程序和服务框架提供咨询。谷歌确实终止了设备制造商的这种做法，但谷歌消息作为一个应用程序仍然不受这些决定的影响。首先，如果你没有预装谷歌消息，它可以很容易地被侧装，而且它不需要谷歌登录就可以独立工作，所以它仍然可以在所有安卓设备上工作(包括华为的新设备)。

但这很快就会改变。如果你有一个未经认证的 Android 设备，该应用程序将无法工作。这被认为是 [RCS 端到端加密部署](https://www.xda-developers.com/google-rcs-e2ee-messages/)的扩展，因为谷歌将无法保证未经认证的设备是否未被入侵，以及这些设备的用户随后的对话是否以任何方式被入侵。考虑到这将对活跃的带 GMS 的 Android 设备的大世界产生多么小的用户基础，这将是谷歌的一个小插头。