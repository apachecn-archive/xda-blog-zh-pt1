# 2022 年 ChromeOS 上的 Linux 应用:完整指南

> 原文：<https://www.xda-developers.com/linux-apps-chrome-os/>

ChromeOS 功能强大，用途广泛，可以在各种硬件上运行，也可以运行各种应用程序。除了运行 Play Store 中的 Android 应用程序，还可以运行完整的 Linux 应用程序。对于许多用户来说，Chromebook 的基本功能已经足够了。然而，如果你发现自己想要一个 Chromebook 没有提供的应用程序或服务，Linux 应用程序可能适合你。

运行 Linux 应用程序到底能完成什么？ChromeOS 默认是一个云计算平台，它省略了一些你可能在 Mac 或 PC 上看到的桌面级应用程序。例如，如果你需要原生运行 Photoshop，这在你的 Chromebook 上是不可能的。ChromeOS 上默认情况下视频编辑也相当困难。这两个问题都可以通过 Linux 应用程序来解决。

此外，如果你是一名开发人员，你无疑需要 Linux 作为编码工具。虽然不是所有的 chrome book 都支持 Linux 应用程序(有一些基本的系统要求)，但大多数现代 chrome book 都有这个选项。在本指南中，我们将详细介绍如何在 Chromebook 上启用和安装 Linux 应用程序，以及如何在 ChromeOS 上运行最好的 Linux 应用程序。

## 如何在 ChromeOS 上启用 Linux 应用

如前所述，你需要先检查你的 Chromebook 是否真的支持 Linux 应用。下面是如何做到这一点。

1.  打开 ChromeOS 设置(通过点击桌面右下角的时间区域，然后点击齿轮状的设置图标)。
2.  点击*高级*选项卡，选择*开发者*。
3.  点击 *Linux 开发环境*选项，选择*打开*。

按照屏幕上的提示在 Chromebook 上安装 Linux。在设置过程中，您将为 Linux 环境选择一个用户名。用户名可以是任何东西，所以不要太担心这个。您还需要决定将多少可用存储空间用于 Linux，但这可以在以后修改。

安装需要几分钟，所以需要一点耐心。当安装结束时，你会看到一个类似上面的终端窗口。现在，您终于可以下载并安装一些 Linux 应用程序了。

## 如何在 ChromeOS 上下载和安装 Linux 应用程序

有两种相当简单的方法可以在 Chromebook 上下载和安装 Linux 应用程序。如果你是一个命令行老手，终端提供了一个快速安装任何你想要的应用程序的方法。然而，如果你更喜欢点击，这对于许多应用程序来说也是可能的。让我们来看看这两个选项。

### 使用 Debian 安装 Linux 应用程序。deb)文件

安装 Linux 应用程序最简单的方法是使用 Debian 扩展文件。你可以在你感兴趣的最流行的 Linux 应用程序的网页上找到这个安装包。Slack 是最受欢迎的 Linux 应用之一，它是一个全功能的团队通信工具。如果你导航到 [Slack Linux 下载页面](https://slack.com/downloads/linux)，你会注意到下载为. deb 文件的选项。

将该文件下载到 Chromebook 会将其放在下载文件夹中。如果你打开下载文件夹，双击给定的文件，ChromeOS 会为你安装软件。新应用现在会出现在你的应用抽屉里，甚至可以钉在 dock 上。

这当然是安装 Linux 应用程序最简单的方法，但是有时候你想要的应用程序可能没有 Debian 文件。

### **从终端安装 Linux 应用**

大多数 Mac 和 PC 用户对使用终端命令并不熟悉。命令行界面是 Linux 生产力的核心。对于没有 Debian 下载的应用程序，你可以使用快捷命令轻松安装。在开始之前，值得使用以下代码更新 Linux:

***须藤 apt-get 更新***

现在，您可以安装一些应用程序。假设你要安装现在流行的 Photoshop 替代 GIMP？只需运行命令:

***sudo apt-get 安装 gimp-y***

您会注意到一堵文字墙在命令行中向下滚动——这在安装过程中是正常的。最后，GIMP 将被放在启动程序中的 Linux apps 文件夹中。虽然使用命令行并不需要太多的工作，但是谷歌搜索您需要的程序的确切名称有时会很烦人。您必须在命令行中准确地输入名称，否则这种方法不起作用。

### **更新 Linux 应用**

偶尔你需要更新你的 Linux 应用程序。与 Android 或 iOS 上的应用程序不同，你需要手动检查这些更新。方便的是，Linux 允许你同时检查所有已安装应用的更新。为此，请打开终端并键入:

***须藤升级&须藤升级***

这个双重命令将检查你的所有应用程序的更新，然后继续下载任何可用的。

### **卸载 Linux 应用**

你也可能决定不再需要 Chromebook 上的某些 Linux 应用程序。卸载应用程序也可以从命令行完成。例如，如果您想卸载 GIMP，您可以打开终端并键入:

***sudo apt-get remove gimp***

真的就这么简单。您可以对每个要卸载的应用程序重复此过程。

## 2022 年 ChromeOS 最佳 Linux 应用

### 瘸子

GIMP 是一个功能齐全的照片编辑套件，类似于 Photoshop，但没有高昂的价格。如果你是一名正在过渡到 ChromeOS 的平面设计师，你会发现 GIMP 是一个不可或缺的工具。功能和文件类型与您在其他照片编辑软件中所期望的完全一致。有许多先进的工具，如层，套索，和大量的画笔，以保持高级用户满意。如果你需要在 Chromebook 上安装照片编辑应用，这是唯一的选择。

**下载使用:**

***sudo apt-get 安装 gimp-y***

### 书店老板

微软 Office 是 PC 和 Mac 上的文字处理之王，但你的 Chromebook 自带谷歌文档作为默认的文字处理器。也许你想要一个更强大的程序来编辑文档和电子表格？如果你需要微软 Office 提供的所有功能，Libre Office 是一个可靠的替代品。你还会得到一个演示应用，类似于 Powerpoint。Libre Office 支持从 Microsoft Word 到 Apple Pages 和 Keynote 的大量文件格式。有了 Libre Office，你可以轻松地在 Chromebook 上照常办公。

**下载使用:**

***sudo apt install-y libre office libre office-gtk3***

### Visual Studio 代码

如果你打算用 Chromebook 编写应用程序，Visual Studio Code 是一个优秀的代码编辑器。通过支持几种流行的编码语言，您可以获得自动完成功能和对版本控制的 Git 支持。凭借流畅的用户界面、可选的扩展和主题支持，这是开发人员在 ChromeOS 上需要的一个强大的代码编辑器。经常编码的人可能也会考虑为他们的 Chromebook 选择一个[漂亮的扩展坞](https://www.xda-developers.com/best-docking-stations-chromebooks/)，以提高工作效率。

**下载使用:**

访问 [Visual Studio 代码](https://code.visualstudio.com/Download)下载页面，下载 Debian 文件。

### 大胆

对于创作者来说，你可能需要一个好的应用程序来录制或编辑音频。这是一个高级的音频编辑器和录音机，当你想播放各种音频文件时，它会派上用场。Audacity 有很多功能，允许你创建自己独特的曲目或混音其他歌曲。Audacity 还有许多插件，可以让你连接到声音设备和其他音频程序。总的来说，这是你在 ChromeOS 设备上可以获得的最好的音频编辑应用程序。

**下载使用:**

***sudo apt-get 安装 audacity -y***

### Kdenlive

如今视频剪辑是一件大事。每小时有数百万人上传视频到 Youtube、Twitch 和 Tiktok。如果你对视频编辑很认真，迁移到 ChromeOS 可能会有点可怕。谢天谢地，Kdenlive 是一个不错的 Linux 视频编辑程序，可以在你的 Chromebook 上运行。那些习惯运行 Final Cut Pro 或 Adobe Premiere Pro 的人将很快学会直观的界面。值得注意的是，虽然 Kdenlive 在 ChromeOS 上运行良好，但你需要一个相当强大的 Chromebook 来充分利用这个应用程序。

**下载使用:**

***须藤 apt-get 安装 kdenlive -y***

这些是我们最喜欢的应用程序，可以帮助你在任何一款顶级 Chromebooks 上开始使用 Linux。还有无数其他的 Linux 应用程序也可以增强你对 ChromeOS 的体验。也许启用 Linux 应用程序最令人兴奋的部分是探索所有新的可能性。无论您需要生产力应用程序、专业编辑应用程序，还是只想在 Chromebook 上享受媒体，Linux 都有适合每个人的东西。

既然我们已经分享了我们的最爱，请在下面的评论中加入你在 ChromeOS 上的常用 Linux 应用程序。