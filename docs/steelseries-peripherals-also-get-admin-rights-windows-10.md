# SteelSeries 外设还可以让你获得 Windows 10 的管理员权限

> 原文：<https://www.xda-developers.com/steelseries-peripherals-also-get-admin-rights-windows-10/>

Windows 10 用户不能因为安全漏洞而喘口气。本周早些时候，[人们发现](https://www.xda-developers.com/razer-peripherals-gain-admin-rights-windows/)将 Razer 外设插入 Windows 10 PC 可以轻松允许用户获得该 PC 的管理员权限。现在，一个非常相似的故事发生在 SteelSeries 外围设备上(通过[](https://www.bleepingcomputer.com/news/security/steelseries-bug-gives-windows-10-admin-rights-by-plugging-in-a-device/)*)。*

 *受本周早些时候发现的启发，安全研究员劳伦斯·阿梅尔试图在 Windows 10 的 SteelSeries 外设中寻找类似的漏洞。插入 SteelSeries 键盘后，Windows 会尝试安装 SteelSeries GG 应用程序，该应用程序用于管理 SteelSeries 外围设备的某些功能，如 RGB 照明。与 Razer 类似，该安装程序由受信任的系统用户运行，该用户拥有管理员权限。

然而，与 Razer 的 Synapse 软件不同，SteelSeries GG 软件的安装最初没有给用户选择文件夹来保存文件的机会，这是第一个漏洞被利用的地方。第一个安装程序将更多的安装文件提取到一个设定的位置，然后提取的安装程序也会运行。

如您所料，第二个安装程序会向用户展示一份许可协议。该页面包含 SteelSeries 网站上完整协议的链接。如果用户尚未设置默认浏览器，Windows 10 将提示他们选择一个应用程序来打开链接，如果他们选择 Internet Explorer，浏览器将像安装程序一样在系统用户下启动。此时，攻击者需要做的只是尝试保存当前网页，这将打开一个文件资源管理器窗口来选择保存文件的位置。

从那里，过程是与 Razer 漏洞相同的。这个文件资源管理器窗口允许任何人使用管理员权限轻松启动命令提示符窗口，用户可以在那里执行他们想要的任何操作。

不仅如此，这个漏洞也无法完全修补。由第一个安装程序提取的第二个安装程序将始终在系统用户下运行。即使 SteelSeries 修复了此处的问题，当前的危险文件也可以保存并分发，以便在将来实施攻击。此外，就像 Razer 漏洞一样，这不需要真正的 SteelSeries 设备，因为这些信息可以用 Android 手机欺骗 Windows 下载 SteelSeries 软件。Twitter 用户 an0n T1 证明了这一点，他也为 Razer 漏洞做了同样的事情。

随着 Windows 10 中发现的这些漏洞，这似乎可以打开闸门。除了 Razer 和 SteelSeries 外设之外，其他品牌可能在 Windows 10 上有类似漏洞的类似软件。很可能会有其他软件以类似的方式被利用来授予本地特权升级，并且我们很可能会在不久的将来听到类似的故事。*