# 新的 Windows 11 预览版已经发布，但仍然没有 Android 应用支持

> 原文：<https://www.xda-developers.com/windows-11-preview-out-still-no-android-app-support/>

像时钟一样，今天是周四，新的 [Windows 11](https://www.xda-developers.com/windows-11/) Insider 预览版将在 Windows Insider 计划的开发和测试频道推出。在[的博文](https://blogs.windows.com/windows-insider/2021/08/12/announcing-windows-11-insider-preview-build-22000-132/)中，只有两件事被列在“变化和改进”下面。首先，微软团队聊天现在已经在测试频道上向内部人士推出。开发用户已经有一段时间了。

另一件事更为重要。有全新的收件箱应用程序，包括一个新的剪贴工具，计算器，邮件和日历。这些是特定于 Dev 频道的。对于像 Snipping Tool 这样的东西，它代表了微软对其 Snip & Sketch 项目的逆转，该项目一度将取代 Snipping Tool 应用程序。这与 OneNote 类似，在某个时候，UWP 应用程序将取代 Win32 应用程序，现在情况正好相反。

对于邮件和日历之类的东西，这些新应用应该有望给那些感觉已经被抛在后面的应用注入新的活力。

值得注意的是，仍然缺少对 Android 应用程序的支持。这是 Windows 11 宣布的关键功能之一，但当预览版开始推出时，微软表示将在未来几个月内推出。但随着 Windows 11 的推出只有几个月的时间，人们不得不开始问，雷德蒙德公司是否仍计划像它所说的那样，今年向非业内人士提供该功能。

Android 应用程序支持将获得亚马逊应用商店的支持，并将集成到微软商店中。延迟可能是亚马逊的原因，因为微软已经在内部测试 Android 的 Windows 子系统有一段时间了。

当然，Windows 11 build 22000.132 中有一大堆修复、改进和已知问题。以下是修复的内容:

### Windows 11 构建 22000.132 修复程序

*   搜索:
    *   做了一些工作，以解决当鼠标悬停在任务栏中的搜索图标上时，最近搜索列表意外显示为空白的情况。
*   小部件:
    *   我们修复了从 widgets 面板启动链接并不总是调用应用程序到前台的问题。
    *   单击任务栏中的小部件图标，现在应该可以在正确的显示器上打开它了。
*   Windows 沙盒:
    *   任务栏(Explorer.exe)不再会在 Windows 沙盒中反复崩溃。
*   其他:
    *   解决了一个问题，导致一些内部人员在尝试返回上一次飞行时遇到错误检查。
    *   缓解了某些游戏按下回车键后没有反应的问题。
    *   修正了“位置使用中”指示器图标没有显示在任务栏中的问题。

以下是仍然存在的问题。这个名单要长得多。

### Windows 11 内部版本 22000.132 已知问题

*   **【提醒】**从 Windows 10 升级到 Windows 11 或者安装 Windows 11 的更新时，某些功能可能会被弃用或删除。[详见此处](https://www.microsoft.com/en-us/windows/windows-11-specifications#primaryR4)。
*   我们正在调查一个问题，在一些设备上，当进入[设置> Windows 更新> Windows Insider 程序](https://aka.ms/WIPSettings)时，只有“停止获取预览版本”选项可见。这防止了内部人员选择通道。我们[已经发布了答案](https://aka.ms/WIPSettingsFix)的变通办法。
*   **【BETA CHANNEL】**我们正在调查 BETA CHANNEL 内部人士的报告，他们在升级到 Windows 11 后，看不到新的任务栏，开始菜单也不起作用。如果您受到影响，请尝试转到 Windows Update >更新历史，卸载最新的 Windows 累积更新，然后通过检查更新重新安装。
*   开始:
    *   在某些情况下，使用“从开始”或任务栏搜索时，您可能无法输入文本。如果遇到此问题，请按键盘上的 WIN + R 启动“运行”对话框，然后关闭它。
    *   右键单击开始按钮(WIN + X)时，系统和 Windows 终端丢失。
*   任务栏:
    *   切换输入法时任务栏有时会闪烁。
*   搜索:
    *   单击任务栏上的搜索图标后，搜索面板可能不会打开。如果出现这种情况，请重新启动“Windows 资源管理器”进程，并再次打开搜索面板。
    *   搜索面板可能显示为黑色，并且不显示搜索框下方的任何内容。
    *   在支持笔的设备上，应用程序可能无法从搜索面板启动。如果您遇到此问题，请注销并重新登录以解决问题。
*   设置:
    *   使用“设置”中的搜索框进行的某些搜索可能会导致设置崩溃。
*   小部件:
    *   小部件面板可能显示为空。要解决此问题，您可以注销，然后重新登录。
    *   外接显示器上的小工具可能会以错误的尺寸显示。如果您遇到这种情况，您可以首先在实际的 PC 显示器上通过触摸或 WIN + W 快捷方式启动小工具，然后在辅助显示器上启动。
    *   [Family widget]即使启用了屏幕时间设置，一些用户也可能会看到“连接设备以查看屏幕时间活动”消息。
    *   [Family widget]位置信息可能对 iOS 上的某些用户不可用。
*   商店:
    *   我们正在努力提高商店中的搜索相关性，包括解决在某些情况下搜索结果排序不准确的问题。
    *   在某些有限的情况下,“安装”按钮可能还不起作用。
    *   某些应用程序不提供评级和评论。
*   Windows 沙盒
    *   在 Windows 沙盒中，单击任务栏上的切换器图标后，语言输入切换器不会启动。作为一种解决方法，用户可以通过以下任何硬件键盘快捷键来切换他们的输入语言:Alt + Shift、Ctrl + Shift 或 Win + Space(第三个选项仅在沙盒全屏时可用)。
    *   在 Windows 沙盒中，单击任务栏中的 IME 图标后，IME 上下文菜单不会启动。作为解决方法，用户可以使用以下方法之一访问 IME 快捷菜单的功能:
        *   通过设置>时间和语言>语言和地区><each ime="" language="">(例如日语)三点>语言选项><each ime="">(例如微软 ime)三点>键盘选项访问 IME 设置。</each></each>
            *   或者，您也可以启用 IME 工具栏，这是一个快速调用特定 IME 功能的替代用户界面。从上面继续，导航到键盘选项>外观>使用 IME 工具栏。
        *   使用与每种 IME 支持的语言相关联的一组独特的硬件键盘快捷键。(参见:[日文 IME 快捷键](https://support.microsoft.com/windows/microsoft-japanese-ime-da40471d-6b91-4042-ae8b-713a96476916)，[繁体中文 IME 快捷键](https://support.microsoft.com/windows/microsoft-traditional-chinese-ime-ef596ca5-aff7-4272-b34b-0ac7c2631a38))。
*   本地化
    *   有一个问题，一些内部人员可能会从他们的用户体验中丢失一些运行最新内部人员预览版本的语言子集的翻译。为了确认您是否受到了影响，[请访问此回答论坛帖子](https://aka.ms/UnderLocIssue)，并按照步骤进行补救。
*   来自微软团队的聊天
    *   体验仅针对英语(美国)进行了本地化。其他语言和地区即将推出。
    *   当您拨出电话时，如果听不到铃声，用户界面会显示电话正在接通。
    *   在视频通话中，有时人物视频会冻结或显示黑色图像。这个问题有一个解决方法，就是锁定冻结的视频，然后取消锁定来解决这个问题。
    *   在呼叫之间切换时，前一个呼叫不会自动保留，因此两个呼叫的音频和视频流都会继续。请确保在接听另一个电话之前先完成通话。

要获得 Windows 11 Insider 预览版 22000.132，您需要在开发或测试频道。如果是，您将通过 Windows Update 获得更新。如果您不是，可以通过“设置”中的“Windows Insider 计划”选项卡注册。请注意，虽然开发和测试频道现在针对 Windows 11 预览版进行了调整，但这不会持续太久。开发频道最终将转向 Windows 11 下一个功能版本的功能。

当然，其中一个功能可能最终会成为 Android 应用。不过微软没有说话，所以和往常一样，没有关于这个话题的交流。