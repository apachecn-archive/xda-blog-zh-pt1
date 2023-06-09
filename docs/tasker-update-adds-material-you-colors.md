# 最新的 Tasker 更新添加了一个你在 Android 12 上的主题材料

> 原文：<https://www.xda-developers.com/tasker-update-adds-material-you-colors/>

Material You 基于壁纸的主题引擎，代号“莫奈”，终于在 [Android 12](https://www.xda-developers.com/android-12/) Beta 2 上线。虽然谷歌还没有发布关于 Material You 的文档，但我们已经看到了一批第三方应用开发者在他们的应用中实现了基于壁纸的动态主题化。早在 6 月，Tasker 就成为了 T2 首批支持 Android 12 动态主题化的应用之一。上个月，Tasker 的测试版在 Google Play 上发布了新的主题素材。现在，Tasker 开发者 joo Dias 终于将该功能引入了该应用的稳定版本。

Tasker 5.13.5 现已在 Google Play 上线，并在运行 Android 12 的设备上提供了对 Material You colors 的支持。要尝试一下，导航到*偏好> UI >主题*并从列表中选择“材料你”选项。一旦启用，Tasker 的动作栏，底部栏，各种菜单，切换，和文字将匹配你的壁纸的颜色。

在下面的视频中查看 Tasker 的新主题:

在最新的 Tasker 更新中，另一个与材料相关的特性是一个名为“获取你着色的材料”的新动作开发者说，这个动作允许用户从系统中提取所有可能的材料颜色，并在各种任务场景中使用它们。要了解有关该功能的更多信息，请直接跳到上面视频中的 [0:48](https://youtu.be/G1jAs8qV1Ik?t=48) 。

除了 Android 12 特有的功能，最新的 Tasker 更新还带来了许多新功能，包括在状态栏和导航栏上定位场景的能力，新的连接到 Wi-Fi 动作，支持导出项目描述，等等。

### 包 5.13.5 张唱片

*   **新增内容**
    *   增加了你支持 Android 12+的素材。启用 Tasker >首选项> UI >主题>素材你。
    *   为 Android 12+添加了获取材料颜色。演示
    *   当类型为叠加时，允许在状态栏和导航栏上显示叠加场景，并在显示场景操作中添加新选项。
    *   增加了连接到 Wifi 的动作，可以和新版本的 Tasker 设置应用一起使用。
    *   添加了使用共享测试服务器测试新 taskernet 功能的选项。
    *   在选择输入对话框动作中增加了应用程序、图像、图像、蓝牙名称和蓝牙地址选项。
    *   使导出的描述更具可读性。
    *   您现在可以使用 content://net . ding lisch . Android . taskerm . icon provider/wallpaper/launcher 或 content://net . ding lisch . Android . taskerm . icon provider/wallpaper/lock screen 在支持图像 URIs 的任何地方使用您的设备壁纸。
    *   增加了在 Tasker 函数动作中获取每种流类型的最大音量的函数。
    *   增加了导出描述时询问高级选项的选项(现在，你可以选择用反勾号将描述换行或者在每行前添加 4 个空格)
    *   添加了在使用“请求权限”操作时指定提示的选项，如果权限尚未授予，则会显示提示
    *   为 taskernet 项目添加了选项，以便在导入时不询问所需的权限
    *   启用硬件加速
    *   允许显示亮度输入栏中的任何值
    *   增加了土耳其语翻译
    *   当返回操作以错误结束时，输出带有值的%err 变量
    *   添加了按命名配置文件排序的选项
    *   增加了在测试任务者动作中获取当前任务名称的选项
    *   taskernet 中的项目/配置文件/任务失败时显示错误
    *   增加了通过 Google Drive 文件而不是直接通过电子邮件发送崩溃报告的选项
    *   在 logcat 条目事件中使用助手选择它们时，向 Logcat 条目添加了行号
    *   添加了显示每隔一段时间内存消耗的日志，以捕捉未来可能的内存泄漏
    *   向媒体控制操作添加了下一个、暂停、停止、播放、倒回和前进标签，以便您可以搜索这些术语并找到该操作
    *   添加了出错时继续选项以转到操作
    *   允许在某些只支持非数组变量的字段中使用数组变量
*   **变化**
    *   制作的未命名配置文件以斜体显示，这样可以很容易地与命名配置文件区分开来
    *   导入项目时，如果该项目中的任务、配置文件或场景已经存在，但项目本身不存在，如果您想要覆盖，请单独询问每个现有项目
    *   如果配置文件/任务/场景与正在导入的项目在同一个项目中，不要询问您是否要覆盖它们
    *   不要在配置文件/任务描述中输出空字段(或禁用的复选框)
    *   在可变联接动作多行中创建联接器字段
    *   当谷歌助手在 Tasker 中搜索任务时，如果只有一个匹配的任务，它会立即运行它，而不是显示一个项目列表
    *   不允许返回操作覆盖%caller()数组

除了 Tasker，其他也实现了对基于壁纸的主题化支持的应用包括 Sleep as Android、Swiftwalls 和一系列谷歌应用，如 [Gboard](https://www.xda-developers.com/gboard-dynamic-color-theme-android-12/) 、谷歌 [Chrome](https://www.xda-developers.com/material-you-dynamic-theming-chrome-for-android/) 、 [Messages](https://www.xda-developers.com/google-messages-material-you-theming-android-12/) 等等。

带有你主题的素材的 Tasker 5.13.5 在 Play Store 上线，你可以从 Play Store 或者开发者的[网站](https://tasker.joaoapps.com/download.html)下载。