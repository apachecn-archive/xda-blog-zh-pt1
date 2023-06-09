# LineageOS 采用 SeedVault 作为其开源备份解决方案

> 原文：<https://www.xda-developers.com/lineageos-seedvault-open-source-backup-solution/>

Android 内置的备份机制依赖于 Google Play 服务框架，可以将联系人、通话记录、短信以及某些应用程序数据和设备设置备份到用户的个人 Google Drive 帐户。然而，备份和恢复应用程序可能是一件痛苦的事情，尤其是当你在不同 OEM 厂商的手机之间切换，或者更喜欢使用没有任何谷歌应用程序的定制 rom 时。山景城巨人可能会移除粉丝最喜欢的 [ADB 备份和恢复工具](https://www.xda-developers.com/adb-backup-and-restore-depreciated/)，这意味着用户必须选择 [root 专用工具](https://www.xda-developers.com/oandbackupx-android-backup-app/)以获得更好的备份。考虑到这些问题，LineageOS 的开发人员选择 SeedVault 作为其默认的备份解决方案。

**XDA 论坛**

对于那些不熟悉 SeedVault 的人来说，它是一个[开源的](https://github.com/stevesoltys/seedvault)备份应用，使用与`adb backup`相同的内部 API。应用程序不需要 root 访问，但必须用操作系统编译。备份位置是用户可配置的，选项从 USB 闪存驱动器到远程自托管云替代方案，如 NextCloud。这使得 SeedVault 成为不想将个人数据存储到谷歌专有的基于云的存储中的用户的一个特别可行的选择。

SeedVault 创建的所有备份内容都通过客户端加密(AES/GCM/NoPadding)进行加密，使用符合 [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki) 标准的 12 字随机生成的密钥可以解锁。此外，超级用户可以通过外部独立实用程序自由解密、检查和重新加密他们的备份[。](https://github.com/tlambertz/seedvault_backup_parser)

下面你可以看到 SeedVault 的运行。请注意，推文是在应用程序发布到 LineageOS 之前很久发布的，因此一些 UI 元素可能与当前的实现不同。

SeedVault 的 LineageOS 版本的源代码可以在[这里](https://github.com/LineageOS/android_packages_apps_Seedvault)找到。随着更多贡献者的加入，他们可以维护备份解决方案或将备份解决方案移植到不同的 Android forks，我们希望在未来几天看到 SeedVault 支持的定制 rom 的列表会增加。

* * *

*感谢 XDA 资深会员 [kurtn](https://forum.xda-developers.com/member.php?u=8031265) 的提示！*