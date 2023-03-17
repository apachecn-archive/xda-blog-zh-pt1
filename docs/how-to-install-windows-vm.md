# 如何在虚拟机中安装 Windows 11 来试用新功能

> 原文：<https://www.xda-developers.com/how-to-install-windows-vm/>

Windows 11 于 2021 年首次亮相，随之而来的是我们从 Windows 10 中所知道的 Windows 界面的大量改变。自首次发布以来，它还获得了第一次重大更新——Windows 11 版本 22 H2——带来了更多的变化。虽然 Windows 11 确实包含了一些很棒的东西，但它做出的改变可能对一些人来说有点太不和谐了，也许你还没有准备好在你的电脑上迁移到它。如果你不确定 Windows 11 是否适合你，你可以使用虚拟机(VM)来尝试。即使你已经安装了 Windows 11，你也可以使用虚拟机来测试内部版本或 22H2 版本更新。

虚拟机是测试软件而不损坏计算机的好方法。它们创建了一个隔离的环境，因此虚拟机内处理的任何文件都不会影响主机操作系统。当你想尝试操作系统时，虚拟机还能让你轻松启动和关闭操作系统，这样你就不必重启你的电脑或准备另一台电脑。

有许多程序允许您创建虚拟机，但在这种情况下，我们将使用 Hyper-V。此功能内置于 Windows 中，但它是一个可选功能，您需要启用。正式来说，你需要一个专业版、企业版或教育版的 Windows 10，但通过一些小改动，也有可能将其安装在家庭版上。

## 如何在 Windows 10/11 中启用 Hyper-V

首先，您需要确保您有一台与 Hyper-V 兼容的电脑。运行虚拟机不是一个轻量级的工作负载，因此您的主机电脑上至少需要 4GB 的内存。事实上，对于 Windows 11，您会想要更多，因为根据[系统要求](https://www.xda-developers.com/windows-11-minimum-requirements/)，您正在创建的虚拟机本身应该有 4GB 来支持 Windows 11。

你还需要两件东西:

*   具有二级地址转换(SLAT)的 64 位处理器。
*   虚拟机监控模式扩展的 CPU 支持(英特尔 CPU 上的 VT-x)。

大多数现代处理器应该支持这些特性，但是最好确保。您可以使用命令提示符或 PowerShell 检查您的计算机是否支持 Hyper-V。以下是如何做到这一点:

*   右击开始图标或按下 *Windows 键* + *X* ，然后选择*命令提示符(Admin)* 、*Windows PowerShell(Admin**)*或 *Windows 终端(Admin)* 。显示哪个选项取决于您的 Windows 版本。
*   在命令提示符/PowerShell 窗口中键入*systeminfo.exe*，按*回车*。
*   检查最后的 *Hyper-V 要求*部分。所有项目都应该说*是*Hyper-V 才能工作。

如果在固件中启用的*虚拟化说*不*，你可以在你的计算机的固件/BIOS 设置中启用它，但这些会因设备而异。最后，您需要确保 Hyper-V 作为可选功能启用。为此，请按照下列步骤操作:*

*   打开开始并键入*控制面板*，然后按回车键。
*   点击*程序*，然后*开启或关闭 Windows 功能*。
*   Hyper-V 应该是首选之一。确保它及其附加功能都已启用，如下所示:

## 下载 Windows ISO

解决了所有这些问题后，您就差不多可以创建虚拟机了。你最不需要的就是一个 ISO。这里有几个选项:

*   从[微软网站](https://www.microsoft.com/en-us/software-download/windows11?9d47a9e1-e53b-49a1-92ca-a647d62dc410=True)下载最新稳定版 Windows 11 的 ISO。这是下载 Windows 11 设置 VM 最简单可靠的方法。
*   下载最新的 [Windows Insider 预览版 ISO](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewiso) ，以防你想在 Windows 11 即将发布之前测试它们。
*   如果你愿意的话，创建你自己的 Windows 11 ISO。不过，我们推荐另外两个选项中的一个。

## 在 Hyper-V 中创建 Windows 虚拟机

在 Hyper-V 中创建虚拟机并不像最初看起来那么可怕。以下是使用 Windows 10 或 11 设置虚拟机所需的内容:

*   打开 Start 并键入 *Hyper-V* 。按回车键启动 *Hyper-V 管理器*。
*   如果这是您第一次启动它，您可能需要首先在左侧菜单中单击您的电脑名称。
*   在右侧菜单中，点击*新建*，然后点击*虚拟机*。
*   虚拟机向导将启动，引导您完成整个过程。点击*下一步，*然后为你的 Windows 11 虚拟机选择一个名字。

*   虚拟机保存为文件，如果愿意，您可以更改文件的保存位置。完成后，点击下一步的*。*
*   在这里，您将被询问您想要创建哪一代虚拟机。对于 Windows 的新版本，比如 Windows 10 或 11，你会希望使用第二代。

*   接下来，您必须指定要分配给虚拟机的内存量。如前所述，您至少需要 4GB 的内存，所以输入 4096MB 或更多。此外，确保启用*动态内存*选项。

*   下一步，将连接类型更改为*默认开关*。这将允许您的虚拟机访问互联网，如果您计划使用互联网安装更新或测试某些功能，您将需要互联网。

*   现在，你必须建立一个虚拟硬盘。这将是可供您的虚拟机使用的存储空间，您可以选择任何您想要的值，只要您的主机 PC 有可用空间。然而，你必须记住，Windows 11 需要 64GB 的存储空间，所以这是你需要选择的最低存储空间。您还可以更改虚拟硬盘的存储位置并更改其名称，但这完全是可选的。

*   这是您需要之前下载的 ISO 文件的地方。选择*从可引导镜像文件*安装操作系统，然后点击*浏览*搜索您下载的 ISO 文件。

*   点击*下一个*，然后*结束*。
*   在 Hyper-V 管理器窗口中，右键单击您刚刚创建的虚拟机，然后单击*设置...*。
*   点击左侧菜单中的*安全*部分，确保*启用安全引导*和*启用可信平台模块*选项均已启用。对于 Windows 11 虚拟机，您将需要这些。另外，启用显示*加密状态和虚拟机迁移流量*的选项。继续之前，点击*应用*。

*   切换到左侧菜单上的*处理器*部分，将虚拟处理器的数量增加到两个或更多。这是运行 Windows 11 的另一个最低要求，所以你的 VM 需要匹配。只要你有足够强大的处理器，你可以选择你的电脑允许的数量。

您现在可以使用您的 Windows 11 虚拟机了。双击您新创建的虚拟机，然后单击*启动*。你必须全新安装 Windows 11。

## 在您的虚拟机上安装 Windows 11

从这里开始，安装和设置 Windows 11 就像在真正的 PC 上全新安装一样。下面是如何做到这一点:

*   选择您的语言和区域设置。默认设置应该没问题，可以点击下一个*。在下一页，点击*立即安装*。*
*   如果您手头有产品密钥，请输入产品密钥。您可以选择暂时跳过这一步，但以后会用到它。
*   选择要安装的 Windows 10 版本。您必须选择与您使用的产品密钥相匹配的版本。

*   接受许可协议，然后选择 **自定义:仅安装 Windows(高级)。**
*   你现在必须创建一个分区来安装 Windows。简单的点击*驱动 0 未分配空间*，然后点击*新建*。使用默认尺寸，然后点击*应用*，再点击*确定*。将创建多个分区。

*   点击*下一步*开始安装，你很快就可以运行 Windows 11 了。
*   从这里开始，您可以像在全新的电脑上一样设置 Windows 11。如果你在这个过程中需要任何帮助，我们有一个关于如何安装 Windows 11 的指南(OOBE)。

现在，您将在虚拟机中运行 Windows 11。如果您想获得最新功能，Windows Update 中可能有更多更新可供下载。请务必查看我们的[更新跟踪器](https://www.xda-developers.com/windows-11-update-tracker/)以了解 Windows 11 的所有最新更新。如果你想知道你现在可以尝试的一切，我们也有一个广泛的列表，列出了已经在 Windows 11 预览版中[提供的一切。](https://www.xda-developers.com/windows-11-features-in-preview/)

最后，如果你不确定你的电脑是否支持 Windows 11，我们有一个将获得升级的电脑的[列表，但你也可以检查 Windows Update 或使用你电脑上的](https://www.xda-developers.com/windows-11-compatible-pc/)[电脑健康检查](https://www.xda-developers.com/windows-11-pc-health-check-available-for-everyone/)应用程序。不过，大多数现代电脑都应该支持它，如果你的电脑不再受支持，你也可以看看我们的[最佳笔记本电脑](https://www.xda-developers.com/best-laptops/)清单。