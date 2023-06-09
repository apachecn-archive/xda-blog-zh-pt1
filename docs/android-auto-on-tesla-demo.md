# 特斯拉上的安卓汽车？这个概念证明展示了它是如何工作的

> 原文：<https://www.xda-developers.com/android-auto-on-tesla-demo/>

车载信息娱乐(IVI)系统中运行的软件通常是由汽车制造商定制的，通常不是很好。尽管美国最受欢迎的电动汽车制造商特斯拉为其信息娱乐系统开发了自己的家酿 Linux 发行版，但你在汽车上发现的许多操作系统都源于[汽车级 Linux](https://www.automotivelinux.org/) 。许多用户不再使用 IVI，而是将手机软件投射到信息娱乐系统的屏幕上，但特斯拉的汽车不支持这一功能。虽然特斯拉的软件相当不错，但在某些情况下，Android Auto 或苹果 CarPlay 会更受欢迎。幸运的是，一个有进取心的开发者已经设法让 Android Auto 在特斯拉上工作，尽管它还处于非常非常早期的阶段。

几天前，XDA 认可的开发者 Emil bor coni T1 在 T2 的 Reddit T3 上展示了这个概念验证。对于那些不知道的人，Emil 是 AAGateWay 应用程序的首席开发人员，也是 [AAWireless 项目](https://www.xda-developers.com/aawireless-dongle-enable-wireless-android-auto-wired-head-units/)的负责人之一，所以如果有人知道如何实现这一点，那就是他。

在 Reddit 上，Emil 透露了一些关于他如何让 Android Auto 在特斯拉上运行的细节。他说他在一个安卓设备上运行一个安卓汽车服务器，然后让特斯拉通过一个热点连接到那个服务器。他的网络服务器以 NAL 单位发送编码视频信号，并在特斯拉上运行 broadway.js(用 JavaScript 编写的 H.264 解码器)。

现在，他正在努力提高性能。在一条评论中，他说他通过两个持续约 60 公里的驱动器实现了这一点，但不得不将分辨率降低到 480p 才能在没有巨大延迟的情况下工作。麦克风输入似乎和缩放一样有效。下面嵌入的视频演示了 Emil 的特斯拉上的 Android Auto。正如你所看到的，这个项目还远远没有准备好，但是 Emil 希望他能在正式发布之前解决任何遗留问题。

\ r \ nht TPS://www . YouTube . com/watch？v=HGeoWXG7hn4\r\n

Emil 还与我们分享了另外两个视频:较长的视频分辨率设置为 720p，而较短的视频分辨率设置为 480p。

Google Play 上有一个名为 [TeslaMirror](https://play.google.com/store/apps/details?id=com.hustmobile.teslamirror) 的应用程序，可以让你将整个手机屏幕镜像到你的特斯拉上，但一旦完成，Emil 的解决方案将更胜一筹，因为你将获得针对汽车优化的 Android Auto 界面和应用程序，而不是通过 TeslaMirror 获得的针对手机优化的应用程序。