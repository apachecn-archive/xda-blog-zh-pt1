# 如何在 Mac 上删除隐藏的下载日志

> 原文：<https://www.xda-developers.com/how-to-delete-hidden-download-log-mac/>

你知道吗，每次你下载一些东西到你的 Mac 上，下载文件的记录就会被添加到一个日志中，并保存在你的系统中。它可以是任何东西，从谷歌图片，从你老板那里得到的 PDF 文档，或者是电影院最新电影的盗版。如果你把它下载到你的 Mac 笔记本电脑硬盘上，它的记录将会被记录在日志中。

苹果没有宣传这已经完成，我个人也不知道为什么会完成。也许是出于故障排除的原因，谁知道呢？但是从隐私的角度来看，这是相当侵入性的，特别是如果有人正在你的计算机周围窥探，并且知道在哪里可以找到日志。如果你有大量下载的习惯，记录下你下载的所有东西当然不方便。要了解如何删除 Mac 上隐藏的下载日志，请继续阅读。

## 首先，在 Mac 上找到下载日志

很容易找到日志。打开终端窗口并键入:

```
sqlite3 ~/Library/Preferences/com.apple.LaunchServices.QuarantineEventsV* 'select LSQuarantineDataURLString from LSQuarantineEvent'
```

这将产生一个完整的下载列表，从你最后一次删除它。如果这是你第一次查看这个列表，这个列表很可能会追溯到你第一次购买 Mac 的时候！

## 现在，删除日志

删除它也不难。只需在终端中键入:

```
sqlite3 ~/Library/Preferences/com.apple.LaunchServices.QuarantineEventsV* 'delete from LSQuarantineEvent'
```

下载列表现在将被清除。如果您再次运行第一个命令，您将得到一个空白列表。

理想情况下，你应该养成每周或每月这样做一次的习惯，这取决于你下载了多少，以及还有谁可以访问你的 Mac 笔记本电脑。为了简化任务，您可以使用命令运行 Automator 脚本，这样只需点按鼠标或触控板即可完成。

* * *

除此之外，苹果电脑还是很棒的计算机器，这要归功于它们的软件、硬件，甚至是苹果配件生态系统。但是如果这种下载记录让你感到厌烦，你可以探索我们在[最佳笔记本电脑](https://www.xda-developers.com/best-laptops)列表中提到的其他选择。