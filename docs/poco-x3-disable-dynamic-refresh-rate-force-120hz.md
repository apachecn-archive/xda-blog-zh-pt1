# 强制 120Hz 刷新率，在 POCO X3 上获得更流畅的体验

> 原文：<https://www.xda-developers.com/poco-x3-disable-dynamic-refresh-rate-force-120hz/>

POCO X3 是你现在能买到的最物有所值的中档智能手机之一。在 POCO X2 成功的基础上，小米的分拆品牌最新的 POCO X 智能手机提供了更好的电池寿命，适度的处理器升级和更新的设计。就像以前的型号一样，showstopper 功能仍然是 120Hz 显示屏，在系统 UI 和第一方应用程序之间提供流畅的滚动体验。与 POCO X2 类似，POCO 使用其所谓的动态刷新率功能来控制刷新率，该功能可以智能地调整显示器刷新率，以最大限度地延长电池寿命。

**[POCO X3 论坛](https://forum.xda-developers.com/xiaomi-poco-x3-nfc)**

这一直是许多 POCO X3 用户争论的焦点，因为即使明确选择了 120Hz 模式，手机也会在某些情况下回落到 60Hz 以节省电池。例如，动态刷新率功能可以在观看视频时将刷新率调低至 60Hz，在观看静态图像时将刷新率调低至 50Hz。相反，如果你在滚动或玩支持的游戏，刷新率会跳到 120Hz。当这种动态刷新率切换发生时，它会导致明显的口吃和抖动，有时会破坏原本流畅的体验，让用户感到沮丧。

不过请放心，XDA 成员 [Slim K](https://forum.xda-developers.com/member.php?u=6687636) 已经把你覆盖了。用户已经[找到了禁用动态刷新率](https://forum.xda-developers.com/xiaomi-poco-x3-nfc/how-to/guide-disable-dynamic-refresh-rate-poco-t4178515)的方法，在所有应用中解锁超平滑的 120Hz 刷新率。

如果你是一台 POCO X3 的骄傲拥有者，并且想要让你的显示器始终以 120Hz 的刷新率呈现一切，即使这意味着牺牲电池寿命，我们已经整理了一个小指南来引导你完成这些步骤。在您继续之前，应该注意到您的 POCO X3 必须有一个解锁的引导加载程序，并以 Magisk v21.0 为根。这样一来，下面是解锁持续 120Hz 模式的步骤。

1.  下载以下软件:

3.  打开终端 app，运行:“su*”*
4.  接下来，运行:"*道具"*
5.  从列表中选择选项 5:*添加/编辑自定义道具*
6.  选择**n***新定制道具*
7.  现在输入下面一行代码:

    ```
     ro.vendor.dfps.enable 
    ```

8.  默认值为*真*。键入*假。*
9.  现在选择 2 " *后 fs 数据*"
10.  选择 **n** ，但先不要重启。
11.  键入下面一行:

    ```
     ro.vendor.smart_dfps.enable 
    ```

12.  同样，默认值为 *true，*表示动态刷新率已启用。键入 *false* 将其禁用。
13.  最后，选择 2 " *后 fs 数据*"
14.  重启。您的设备现在应该一直以 120Hz 的频率运行。

开发者只在股票 MIUI 上测试了这个解决方法，所以如果你运行的是定制的 ROM，它可能不工作——尽管你可以尝试。

不言而喻，启用持续的 120Hz 刷新率将严重消耗电池寿命——用户的个人测试表明，屏幕打开时间会减少 10%至 18%。但是，如果这听起来对你来说不算太糟糕，无论如何，尝试一下这种变通办法来解锁强制 120Hz 模式。要了解更多细节，请点击下面的链接查看用户的原始帖子。

**[禁用 POCO X3 的动态刷新率](https://forum.xda-developers.com/xiaomi-poco-x3-nfc/how-to/guide-disable-dynamic-refresh-rate-poco-t4178515)**