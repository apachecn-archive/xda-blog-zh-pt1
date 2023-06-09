# 微软发布了 Windows 11 build 22000.708，并进行大量修复

> 原文：<https://www.xda-developers.com/microsoft-windows-11-build-22000-708/>

今天是微软 Build 2022 开发者大会的第一天，但这并不意味着该公司的所有消息都来自展会。该公司还发布了本月的 Windows 11 的 D 周更新，这是一个可选的更新，包括我们将在下个月的补丁星期二看到的大部分内容。

如果你正在寻找 Windows 11 的可选更新，你将获得 [KB5014019](https://support.microsoft.com/en-us/topic/may-24-2022-kb5014019-os-build-22000-708-preview-442dbde4-ce28-4345-aecf-2d4744376418) ，使内部版本号达到 22000.708。你可以在这里[手动下载。](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5014019)

虽然有大量的修复，但实际上有几个新闻功能，内部人士已经在测试了。事实上，如果你在发布预览环，你已经有了这整个更新。一个是当孩子帐户发送更多屏幕时间的请求时，更好的家庭安全验证体验。

另一个是桌面上的 Windows spotlight，它允许你将旋转图像设置为壁纸。这是我们很久以来在锁定屏幕上看到的东西。现在，您可以通过在设置中选择 Windows spotlight 将其设置为您的壁纸。

以下是本次更新的其他亮点:

*   解决了更改显示模式后无法保持显示亮度的问题。

*   解决了影响 IE 模式窗口框架的问题。
*   解决了阻止 internet 快捷方式更新的问题。
*   解决了在 IME 转换以前的文本时，如果您输入字符，输入法编辑器(IME)会丢弃该字符的问题。
*   解决了当您将鼠标悬停在任务栏上的小部件图标上时，小部件出现在错误的显示器上的问题。
*   当您单击或点击图标时，为小工具图标添加动画，并且任务栏在左侧对齐。
*   解决了影响任务栏上居中对齐的默认小工具图标的渲染的问题。
*   解决了当显示器的每英寸点数(dpi)比例大于 100%时，导致搜索结果中的应用程序图标模糊的问题。
*   解决了导致文件复制变慢的问题。
*   解决了当您选择“开始”菜单并开始键入时，无法自动为搜索框提供输入焦点的问题。

当然，那些只是亮点。完整的修复列表非常庞大。

### Windows 11 构建 22000.708 修复程序

*   ***新增！*** 改善了您发送额外屏幕时间请求时儿童帐户的家庭安全设置验证体验。
*   ***新增！*** 桌面上的 Windows spotlight 用新的背景图片把世界带到你的桌面上。使用此功能，新图片将自动显示为您的桌面背景。此功能已经存在于锁定屏幕。要打开此功能，请进入**设置>个性化>背景>个性化您的背景。**选择**窗口聚光灯**。
*   解决了导致输入(**TextInputHost.exe**)应用程序停止工作的问题。
*   解决了**searchindexer.exe**中影响在 Microsoft Visio 中搜索形状的问题。
*   防止用户在登录 Azure Active Directory (AAD)时通过断开互联网连接来绕过强制注册。
*   解决了可能将 AnyCPU 应用程序作为 32 位进程运行的问题。
*   解决了阻止具有多个部分配置的 Azure 所需状态配置(DSC)方案按预期工作的问题。
*   解决影响对 Win32_User 或 Win32_Group WMI 类的远程过程调用(RPC)的问题。运行 RPC 的域成员联系主域控制器(PDC)。当多个 RPC 同时出现在许多域成员上时，这可能会淹没 PDC。
*   解决添加具有单向信任的受信任用户、组或计算机时出现的问题。出现错误消息“所选对象与目标源的类型不匹配”。
*   解决了无法在性能监视器工具的性能报告中显示应用程序计数器部分的问题。
*   解决了更改显示模式后无法保持显示亮度的问题。
*   解决了一个问题，该问题可能会影响某些在某些显卡上使用**d3d9.dll**的应用程序，并可能导致这些应用程序意外关闭。
*   解决了影响 IE 模式窗口框架的问题。
*   解决影响组策略模板的问题。
*   解决了阻止 internet 快捷方式更新的问题。
*   解决了导致某些用户在登录和注销 Windows 时看到黑屏的问题。
*   解决了在 IME 转换以前的文本时，如果您输入字符，输入法编辑器(IME)会丢弃该字符的问题。
*   解决了影响桌面复制 API 的问题，该 API 会影响显示方向并导致屏幕上出现黑色图像。
*   解决了当低完整性级别(LowIL)应用程序打印到空端口时导致打印失败的问题。
*   解决了使用静默加密选项时 BitLocker 无法加密的问题。
*   解决了在打开 Windows Defender 应用程序控制(WDAC)的情况下运行脚本时导致误判的问题。这可能会生成 AppLocker 事件 8029、8028 或 8037，这些事件不应出现在日志中。
*   解决了应用多个 WDAC 策略时出现的问题。这样做可能会在策略允许脚本运行时阻止脚本运行。
*   解决了影响受信任的平台模块(TPM)驱动程序的问题，该驱动程序可能会增加系统的启动时间。
*   解决了在您结束会话时可能导致远程桌面客户端应用程序停止工作的问题。
*   解决了影响 Microsoft Defender Application Guard(MDAG)、Microsoft Office 和 Microsoft Edge 的鼠标光标的行为和形状方向的问题。当您打开虚拟图形处理单元(GPU)时，会出现此问题。
*   解决了当您将鼠标悬停在任务栏上的小部件图标上时，小部件出现在错误的显示器上的问题。
*   当您单击或点击图标时，为小工具图标添加动画，并且任务栏在左侧对齐。
*   解决了影响任务栏上居中对齐的默认小工具图标的渲染的问题。
*   解决了当您从任务栏搜索时，无法使选项“以管理员身份运行”和“打开文件位置”对某些结果可用的问题。
*   解决了当您选择“开始”菜单并开始键入时，无法自动为搜索框提供输入焦点的问题。
*   解决了当显示器的每英寸点数(dpi)比例大于 100%时，导致搜索结果中的应用程序图标模糊的问题。
*   解决了由于缓存管理器中写缓冲区计算错误而导致文件复制变慢的问题。
*   解决了当用户在使用 Microsoft OneDrive 时注销可能导致系统停止响应的问题。
*   解决了一个已知问题，如果您使用控制面板中的[备份和恢复(Windows 7)](https://support.microsoft.com/windows/backup-and-restore-in-windows-352091d2-bb9d-3ea3-ed18-52ef2b88cbef) 应用程序创建恢复光盘(CD 或 DVD ),可能会阻止它们启动。安装 2022 年 1 月 11 日或更高版本发布的 Windows 更新后会出现此问题。
*   解决了一个影响某些 GPU 的已知问题，该问题可能会导致应用程序意外关闭或导致间歇性问题，这些问题会影响某些使用 Direct3D 9 的应用程序。您也可能在 Windows 日志/应用程序的事件日志中收到一个错误，出错模块是**d3d9on12.dll**，异常代码是 0xc0000094。

有一个已知的问题。如果您安装此更新，一些。NET Framework 3.5 应用程序可能无法打开，因此作为解决方法，您必须重新启用。NET Framework 3.5 和 Windows 功能中的 Windows 通信基础。

同样，这是一个可选的更新。这意味着您完全可以通过 Windows Update 获得它，但您不必这样做。如果您选择忽略它，您将在星期二补丁日获得这些修复，更新将自动安装。

来源:[微软](https://support.microsoft.com/en-us/topic/may-24-2022-kb5014019-os-build-22000-708-preview-442dbde4-ce28-4345-aecf-2d4744376418)