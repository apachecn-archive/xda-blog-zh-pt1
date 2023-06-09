# Discord 可能很快会让你注销在其他设备上打开的会话

> 原文：<https://www.xda-developers.com/discord-log-out-sessions-other-devices/>

允许用户在多个设备上登录其帐户的信息服务通常会提供一个选项，帮助他们注销在其他设备上打开的会话。例如，Telegram 在应用程序设置的设备部分有一个按钮，让你只需轻按一下就可以终止所有其他会话。WhatsApp 也提供了类似的功能，让你可以在应用程序设置中访问所有链接的设备，你可以点击一个链接的设备来立即终止会话。然而，Discord 不提供这样的功能，它不允许你从其他设备上打开的会话中注销。但这种情况可能很快就会改变。

根据开发人员在 Discord 数据挖掘 GitHub 中发现的新字符串，Discord 目前正在开发一项新功能，让用户从其他设备上打开的会话中注销。字符串表明，该功能将要求用户输入密码和/或授权码，以便从另一台设备上的活动会话中注销。

+ AUTH_SESSIONS:"会话"

+AUTH _ SESSIONS _ LOGOUT _ PASSWORD _ MODAL _ TITLE:"输入密码以注销会话"

+AUTH _ SESSIONS _ LOGOUT _ MFA _ MODAL _ TITLE:"输入授权码以注销会话"

+AUTH _ SESSIONS _ LOGOUT _ MANY _ PASSWORD _ MODAL _ TITLE:"输入密码以注销{sessionCount，plural，=1 {# Session} other {# Sessions}} "

+AUTH _ SESSIONS _ LOGOUT _ MANY _ MFA _ MODAL _ TITLE:"输入授权码以注销{sessionCount，plural，=1 {# Session} other {# Sessions}} "

+ AUTH_SESSIONS_DESCRIPTION:"这是目前使用您的 Discord 帐户登录的所有设备。您可以单独注销每个会话，也可以注销所有其他会话。\ n \ n 如果您看到一个您不认识的条目，请退出该会话并立即更改您的 Discord 帐户密码。

+ AUTH_SESSIONS_CURRENT:"当前会话"

+ AUTH_SESSIONS_OTHERS:"其他会话"

+AUTH _ SESSIONS _ OTHERS _ LOG _ OUT _ TITLE:"注销所有其他会话"

+AUTH _ SESSIONS _ OTHERS _ LOG _ OUT _ DESCRIPTION:"您必须在所有设备上重新登录。"

+AUTH _ SESSIONS _ OTHERS _ LOG _ OUT _ ACTION:"注销所有其他会话"

+AUTH _ SESSIONS _ ACTIVE _ recent:"不到一小时前"

+AUTH _ SESSIONS _ SESSION _ MENU _ LABEL:"会话操作"

+ AUTH_SESSIONS_SESSION_LOG_OUT:"注销会话"

+ AUTH_SESSIONS_OS_UNKNOWN:"未知"

在验证过程之后，Discord 将向用户显示当前使用其 Discord 帐户登录的所有设备的列表。然后，用户可以选择终止特定设备或列表中所有其他设备上的活动会话。字符串进一步指出，列表还将显示用户在每个设备上活动的最后时间。

虽然该功能目前尚未上线，但开发者 justsomederpystuff 已经设法手动启用它，以显示它在发布时的样子。正如你在所附的截图中看到的，该功能将作为一个新的“会话”选项出现在 Discord 的用户设置中。

单击会话选项将打开一个新的选项卡，列出当前会话和所有其他会话。要注销特定的会话，用户必须单击“其他会话”标题下列出的会话旁边的三点菜单按钮，然后单击“注销会话”按钮。这将弹出一个带有密码字段的窗口，您需要验证您的帐户才能退出该会话。

或者，用户可以选择通过点击标签底部的“注销所有其他会话”按钮来注销所有其他会话。目前，Discord 还没有分享任何关于该功能的官方信息，我们也不知道它何时会向用户推出。我们一有更多的消息就会通知你。

就在 Discord 开始为拥有多个账户的用户推出易于使用的账户切换器的几个月后，关于注销其他会话能力的细节出现了。

* * *

**来源:** [不和谐数据挖掘 GitHub](https://github.com/Discord-Datamining/Discord-Datamining/commit/55ea89a1839f7685e9c768b939eaac768d3bc2f5#commitcomment-77310798)

*感谢 XDA 资深会员 [Some_Random_Username](https://forum.xda-developers.com/m/some_random_username.8234677/) 的提示！*