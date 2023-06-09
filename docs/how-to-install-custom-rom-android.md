# 如何在 Android 上安装自定义 ROM 以在手机上获得新功能

> 原文：<https://www.xda-developers.com/how-to-install-custom-rom-android/>

每部智能手机都预装了默认的 ROM 或 UI。它可以是基于 AOSP 的，没有太多的附加功能，通常被称为股票 Android，或者它可以是一个特定品牌的定制皮肤。例如，三星手机使用基于 Android 的定制 OneUI。小米手机用 MIUI，Oppo 用 ColorOS，一加用 OxygenOS 等。每个用户界面看起来都不一样，有不同的特性。

虽然有些人可能喜欢某个 UI 或皮肤，但有些人可能不喜欢。一些用户喜欢功能丰富的界面，能够安装主题和修改系统元素，而一些用户可能想要一个干净、简单、没有装饰的体验。这就是安装自定义 Android ROM 的原因。

自定义 ROM 本质上是用你选择安装的 ROM 来替换你手机上的 ROM 或皮肤。例如，如果你有一部小米或红米手机运行在 MIUI 上，但你不喜欢它的界面，你可以安装一个自定义 ROM，将 UI 更改为股票 Android 或其他你喜欢的东西。

安装自定义 Android ROM 有多种好处。如果你正在使用的 UI 有很多广告或膨胀软件，你可以安装一个定制的 ROM 来清除它们。如果你的手机的 OEM 已经停止更新你的设备，而你还停留在旧版本的 Android 上，你可以使用基于新版本 Android 的定制 ROM。如果你喜欢一个不同的 OEM 的用户界面，并希望在你的手机上尝试，你可以安装一个自定义的 ROM。

既然你知道了自定义 ROM 可以做什么，那就告诉你如何在你的 Android 手机上安装它吧。注意，没有通用的定制 ROM，尽管[项目 Treble](https://forum.xda-developers.com/c/project-treble.7259/) 通过引入[通用系统映像](https://www.xda-developers.com/flash-generic-system-image-project-treble-device/) (GSI)的概念在某种程度上实现了它。虽然你可以安装一个 [GSI，上面点缀着你最喜欢的定制 rom](https://www.xda-developers.com/unofficial-lineageos-18-0-gsi-android-11-project-treble/) 中的所有好东西，但请记住，它可能无法为你的设备提供与微调专用定制 ROM 相同的稳定性和性能。所以说了这么多，你必须安装一个专门为你的手机定制的 ROM。不这样做可能会导致你的手机死机。然后你必须想办法把它找回来或者送到服务中心。

**注意:**安装定制 ROM 可能会使某些设备的保修失效，因为这涉及到解锁引导程序。请小心操作，因为如果没有正确遵循所有步骤，可能会对您的设备造成暂时/永久的损坏。

有时，安装说明会因您的设备而有所不同。这些是通用说明。请仔细检查您的设备论坛的变化。

## 安装自定义 ROM 的先决条件

在你开始在手机上安装定制的 Android ROM 之前，你需要做一些事情。让我们看一下所有这些，以便您的设备为安装过程做好准备。

*   一个安卓设备。
*   一个解锁的引导程序(如果你不知道如何解锁你手机的引导程序，去 [XDA 论坛](https://forum.xda-developers.com/)搜索你的设备名，然后点击“解锁引导程序”，你会找到一个指南。每个手机的流程都不同，因此请确保您遵循的是专门针对您的设备的流程。)
*   定制恢复:TWRP 是一个不错的选择，你可以按照我们的详细指南在你的手机上安装 TWRP。但是，一些定制的 rom 对您需要使用的恢复有具体的建议，所以如果有这样的说明，请遵照执行。
*   一个你想要安装的定制 ROM 压缩文件(同样，去 [XDA 论坛](https://forum.xda-developers.com/)搜索你的设备，浏览所有可用的 ROM，选择你想要安装的。)
    *   **请再次注意**定制 ROM 安装说明可能因设备和 ROM 而异。如果您选择的 ROM 带有自己的说明，请遵循它们而不是本指南。本指南是一般的说明列表，不考虑任何特殊的设备说明。

*   [GApps](https://www.xda-developers.com/download-google-apps-gapps/) 或者 Google Apps。
*   一点点耐心。

## 如何安装自定义 ROM

现在你已经做好了安装定制 ROM 的一切准备，我们可以开始这个过程了。

### 步骤 0:备份数据

在开始安装之前，你还需要做一件事，那就是备份你所有的数据。我们有一个[详细的指南来帮助你备份你手机数据的每一个方面](https://www.xda-developers.com/how-to-backup-android/),所以请确保你这样做，这样一旦你安装了新的 ROM，就可以很容易地恢复你的数据。

### 步骤 1:下载正确的 ROM

正如我们之前提到的，最好的方法是去 XDA 论坛为你的设备寻找一个最适合你需求的 ROM。定制的 ROM 是设备专用的，所以下载一个专门为你的设备制作的 ROM。此外，基于运营商、地区等，同一设备可以有多种变体。所以也要记住这一点。为您的设备找到合适的自定义 ROM。如果你不确定，在 XDA 论坛询问兼容性。

一旦你找到了你想要安装的 ROM，在你的电脑或者手机上下载压缩文件。请注意，在后面的一些步骤中，您将需要对您的手机进行数据擦除，因此建议稍后在数据擦除之后进行文件传输，但要确保您的手机可以连接到您的计算机并可以接收文件，以确保您的设备驱动程序已经就绪。稍后，你需要将 ROM 文件复制到手机内部存储器的根目录下。**不要**解压 zip 文件。

### 第二步:下载 GApps 或 Google Apps

定制光盘没有预装谷歌的应用和服务(少数例外)。所以，如果你想用你的谷歌账户登录并使用谷歌的服务，比如同步、Play Store、Gmail、Drive 等。，您需要安装一个单独的 GApps 包。您可以安装多种 GApps。你可以参考我们的[指南，找到适合你的 Gapps 包](https://www.xda-developers.com/download-google-apps-gapps/)，下载一个适合你的。这也将是一个 zip 文件的形式。下载并将其传输到手机的内部存储器中。如果你选择`adb sideload`方法，你也可以直接从你的 PC/Mac 上安装它们。

注意:Pixel Experience 等一些定制 rom 预装了 GApps。在这种情况下，您不必单独刷新 GApps 文件。

### 第 3 步:引导到 TWRP

一旦你将 ROM 和 GApps 文件复制到手机的内存中，就该启动 TWRP 来刷新文件了。如果你不熟悉在你的手机上引导进入恢复模式，我们有一个指南告诉你如何在你的手机上引导进入恢复模式，这样你就可以按照它来引导进入 TWRP。一旦你到了 TWRP，在安装 ROM 之前你需要做一些事情，我们将在下一步讨论这些。

### 步骤 4:安装自定义 ROM

一旦你到了 TWRP，在继续下一步之前，最好对你的整个系统做一个 nandroid 备份。这在安装失败的情况下会很有用。您将能够启动到 TWRP，并恢复备份，以回到您的设备以前的状态。

*   为此，在 TWRP 选择*备份*选项，选择*开机，系统镜像，数据，调制解调器，*和 *EFS* ，然后*滑动备份*。等到它完成。

*   **这一步将擦除你的整个手机:**回到 TWRP 主菜单，选择*擦除*。然后，*滑动到出厂复位*。选择*格式化数据*选项，输入“yes”并选择勾选标记来格式化您的手机。请注意，格式化`/data`分区将需要您重启一次，以便 TWRP 可以正确地识别新创建的文件系统。

*   此外，由于设备的内部存储器在格式化过程中会被擦除，因此您必须将 ROM 和 GApps 文件再次复制到手机的存储器中。
    *   你可以在 TWRP 内部做到这一点。前往*挂载*部分，选择*启用 MTP* 选项。
    *   现在，将您的手机连接到您的 PC，它应该被检测为存储设备。传输 ROM 和 gapps 文件。

*   完成后，回到 TWRP 的主菜单，选择*安装*。浏览到保存 ROM 和 GApps 文件的位置。首先，选择 ROM 并*滑动来安装*它。
    *   返回上一菜单，选择 GApps 文件。把那个也装上。安装完成后，选择*重启至系统*。
    *   如果您的安装没有按照这个步骤启动，您可能需要闪存/安装只读存储器，重新启动恢复，然后闪存 GApps 文件。在某些情况下，需要重新启动。

你现在有一个自定义的 Android ROM 安装在你的手机上！等待你的手机启动。初始启动过程可能需要一段时间，所以不要惊慌，您的手机将启动到设置过程。

这样就可以在手机上安装自定义的 Android ROM 了。这是一个相当简单的过程，只需要一点点时间和耐心，你就可以在你的手机上享受一个全新的 ROM，它增加了新的功能、定制、主题化等等。如果你安装了一个定制的 ROM，你不喜欢它或者它有问题，只需下载一个新的 ROM 并重复安装过程。