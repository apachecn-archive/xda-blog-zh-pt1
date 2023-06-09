# 为什么 Magisk 不再支持隐藏应用程序的 root 访问权限

> 原文：<https://www.xda-developers.com/magisk-development-continues-without-magiskhide/>

早在五月，Magisk 的开发者 topjohnwu[宣布](https://www.xda-developers.com/magisk-developer-topjohnwu-leaves-apple-joins-google/)他已经加入谷歌的 Android 平台安全团队。鉴于 Magisk 被用于为 Android 设备提供根目录，并规避应用程序中的根目录检测措施，许多人怀疑谷歌会允许开发者以当前形式继续进行该项目，甚至根本不会。幸运的是，topjohnwu 已经获准继续开发 Magisk，但这一批准取决于该项目放弃对其名为 MagiskHide 的根隐藏功能的支持。

在一篇博客文章中，topjohnwu 谈到了 Magisk 开发的现状，以及该项目未来的变化。他的第一点反驳了他的雇主谷歌禁止他参与该项目的指控，而事实上，他只是不得不通过许多繁文缛节来获得他参与该项目所需的批准。对于谷歌这样的科技公司来说，审查员工的外部工作并不罕见，尤其是当外部工作直接影响员工受雇从事的产品时。在 topjohnwu 的案例中，他在 Android 平台安全团队的工作使他能够深入了解 Android 当前和未来的安全措施，当 Magisk hide——Magisk 的根隐藏组件——旨在规避谷歌当前的安全措施之一，即安全网认证时，这就出现了明显的利益冲突。为此，topjohnwu 别无选择，只能停止 MagiskHide 的开发，并拆除其大部分基础设施。

## MagiskHide 达到寿命终点

不过，终止 MagiskHide 的开发对 topjohnwu 来说并不是一个困难的决定。在个人层面上，开发人员表示，自从他上次发现绕过根检测方法的工作令人愉快以来，已经有一段时间了，这是可以理解的，因为这本质上是一场猫捉老鼠的游戏。当然，Magisk 的受欢迎程度很大程度上可以归功于它在 Google Pay 和 Pokémon Go 中成功绕过了根检测，但为了跟上不断变化的形势，不得不不断修补项目令人疲惫。此外，随着[硬件支持认证](https://www.xda-developers.com/safetynet-hardware-attestation-hide-root-magisk/)的实施，规避根检测变得更加困难，而[当前的变通办法](https://www.xda-developers.com/bypass-safetynet-hardware-attestation-unlocked-bootloader-magisk-module/)可能不会永远奏效。

尽管 MagiskHide 即将寿终正寝，但该工具仍将在非常有限的意义上存在，因为 topjohnwu 认为应用程序能够“选择退出”修改非常重要。开发者说，用户“将能够分配一个进程拒绝列表，Magisk 拒绝进一步的修改，并恢复它所做的所有更改。Magisk 不会欺骗/改变/操纵任何与 Magisk 无关的信号或痕迹来规避任何设备状态检测。”基本上，MagiskHide 将不再对应用程序隐藏 root 访问权限，而是用于确保用户选择的应用程序不会被修改。使恢复更改变得更容易也将加快模拟器上的测试，因为开发人员将不再需要重启或修补模拟器映像。

当然，即使官方 Magisk 应用程序正在放弃对隐藏根访问的支持**，但这并不意味着它不能恢复该功能，或者不能发布根隐藏模块**。然而，任何这样做的开发人员最终都会遇到与 topjohnwu 相同的问题，这意味着他们将不得不玩同样的猫捉老鼠游戏，这种游戏导致了 topjohnwu 对 Hide 的失望。

## 集中式 Magisk 模块报告的结尾

Magisk 的另一个即将到来的变化是从应用程序中移除 Magisk 模块 repo。Magisk 应用程序中集成了 [Magisk-Modules-Repo](https://github.com/Magisk-Modules-Repo) ，这使得用户可以在应用程序中搜索和下载模块。它的删除将意味着用户将不得不手动下载模块 ZIP 文件，并从应用程序中安装它们，这与现有的解决方案相比有点不方便，但一点也不难做到。此外，带有 Magisk 模块组件的应用程序可以通过运行`magisk --install-module ZIP`命令为用户轻松安装模块，为用户省去手动步骤。

然而，更大的损失是通过集中管理的回购发现新模块，但 topjohnwu 说 **Magisk-Modules-Repo 将很快转移到“受信任的社区成员”**。这意味着**回购本身不会消失**，但应用程序目前不会指向它。虽然最终， **topjohnwu 确实希望让用户将 Magisk 应用指向他们想要的任何在线模块源**，有点像 F-Droid，但这不是他目前实施的优先事项。

这种变化并不是由 topjohnwu 在谷歌的任职引起的，而是考虑到缓和回购所需的时间投资，这种变化必然会发生。

## 合子中的 Zygist - Magisk

在过去的几个月里，topjohnwu 和其他几个开发人员一直在开发一个叫做“Zygisk”的东西，也就是 Zygote 中的 Magisk。Zygote 是处理每个应用程序进程分叉的操作系统进程，因此**在 zygote 进程中运行 Magisk 的部分将使模块更加健壮(包括使根隐藏更加强大)**。Topjohnwu 表示，Zygisk 也符合他的 Magisk 哲学，即让开发者不同意修改的应用“让开”，因为当一个进程被添加到 MagiskHide denylist 时，Magisk“将清理该进程的内存空间，以确保没有应用任何修改。”

这个项目仍在进行中，但当它准备好进行 beta 测试时，我们会听到更多的实现细节。

## Magisk 开发的未来

Magisk 从一开始就是 topjohnwu 的业余爱好项目，但开发者希望更认真地对待这个项目。他已经开始在 GitHub 上进行持续集成，并将通过与 [AVD](https://developer.android.com/studio/run/managing-avds) 的集成，在每次发布之前开始回归测试变更。

Topjohnwu 还指出，其他有才华的开发人员已经向 Magisk 的核心提交了有价值的代码更改，修复了许多错误并扩展了设备兼容性。尽管 Magisk 从一开始就是开源的，但它一直是 topjohnwu 的唯一领域，所以当 topjohnwu 自己没有太多时间和精力投入这个项目时，很高兴看到其他人为这个项目做出贡献。