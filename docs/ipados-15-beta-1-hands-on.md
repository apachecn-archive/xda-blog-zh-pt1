# iPadOS 15 开发者 Beta 1 实践:快速笔记、分屏等等！

> 原文：<https://www.xda-developers.com/ipados-15-beta-1-hands-on/>

我最近写了一篇关于 [iPadOS 如何阻碍新的 M1 驱动的 iPad Pro](https://www.xda-developers.com/apple-ipad-pro-ipados-limitations/) 的观点文章，因为如果 iPad 上的软件只是 iPhone UI 的放大版本，那么拥有可以超越英特尔驱动的台式机的超级强大的硅有什么好处呢？我的抱怨包括有限的多任务处理和受限的主屏幕。嗯，苹果昨天在 WWDC 发布会上发布了 iOS 15 和它的兄弟 iPadOS 15，解决了一些问题。

在过去的几个小时里，我一直在测试 iPadOS 15 的开发者测试版，以下是我的印象。iOS 15/iPadOS 15 测试版可供开发者和发烧友下载，但我们不建议现在就在你的主要日常设备上安装，因为该软件存在很多问题。如果你愿意，你也可以看看我们的 iOS 15 开发者测试版 1 的[实践。](https://www.xda-developers.com/ios-15-beta-1-hands-on/)

## iPadOS 15 上的新主屏

 <picture>![iPadOS 15 homescreen as it first appears after installing](img/c1e9948325fbece5b5b54a4ab7678758.png)</picture> 

iPadOS 15 homescreen with widgets being allowed anywhere.

iPad 一启动 iPadOS 15，大多数人会注意到的第一件事是，他们的主屏幕应该会被打乱。在之前的 iOS 版本(14.5)中，所有位于主屏幕左侧的小工具都被移到了 iPadOS 主屏幕的顶部。这是因为 iPadOS 15 允许用户在主屏幕的任何地方和任何页面上放置小工具。过去，它们只允许出现在第一页的左侧。这一点，加上“应用程序库”(基本上是苹果版的 Android 应用程序抽屉)的添加，意味着我现在可以显著清理我的 iPad 的主屏幕，而不是我的所有应用程序都在主屏幕上。

 <picture>![iPadOS 15 with app library](img/7bb1217f3897064770c96cd2b1758e70.png)</picture> 

App Library on iPadOS 15 Beta 1.

值得一提的是，这些更新只是针对 iPadOS 的“新”更新，因为 iOS 14 去年就已经获得了这些改进。

此外，iPadOS 主屏幕网格仍然不是真正免费的，这意味着所有的东西和小工具仍然必须按照从上到下，从左到右的顺序放置。例如，我不能在屏幕的下半部分有一个空的主屏幕，上面有两个应用程序和一个小工具。

## 改进了 iPadOS 15 上的多任务处理

令人欣慰的是，iPadOS 15 全面提高了多任务处理能力。

### 分屏操作

最值得注意的新功能是可以通过一个新的小屏幕按钮直接在任何 iPad 应用程序中手动触发分屏操作，该按钮位于屏幕的顶部中间部分，每当用户进入应用程序时就会出现。点击按钮，它会打开一个选项，立即将应用程序切换到半屏布局或浮动“滑动”布局。轻按半屏或滑动会将应用程序切换到所需的格式，将屏幕的一部分带回主屏幕，供您选择另一个应用程序打开。这是对以前分屏多任务处理方法的巨大改进，以前的方法需要几次滑动和一次点击，另外第二个应用程序必须已经存储在 dock 中。

 <picture>![Screenshot of iPadOS 15 running two apps.](img/c9820414cf5a99ffeca266d6863ddf92.png)</picture> 

Note the floating button at the top middle portion of the screen asking how I would like to display Twitter: full-screen, split-screen, or floating Slide Over mode.

已经配对的应用程序也会记住它们的配对。例如，如果我在分屏视图中打开 Twitter 和谷歌文档，即使我退出应用程序观看网飞一个小时，稍后再次点击 Twitter 也会在谷歌文档旁边以分屏模式打开它。

 <picture>![iPadOS 15 running four apps.](img/81bda1aa289408efa14d83b150049233.png)</picture> 

iPadOS 15 Beta running two apps in split-screen mode with a third app in Slide Over, and Quick Notes opened for technically four apps at once.

### 超赞的快速笔记

在多任务处理方面，一个可以说是更大的更新实际上是 iPad 独有的“快速笔记”，它允许用户在一个更小的浮动窗口中快速打开苹果的笔记应用程序，而不会挡住整个屏幕。只需用 Apple Pencil 从右下角向上滑动，即可调出应用程序。浮动的“快速笔记”窗口可以在屏幕上四处移动，并且还知道屏幕上已有内容的上下文。例如，如果我在 Safari 的 XDA 主页上打开快速笔记，快速笔记窗口会显示一个快捷按钮，可以快速将网站链接粘贴到页面上。

 <picture>![iPadOS 15 with Quick Notes](img/c549d321e3ee1c64fde5d9c4ffd9bc9d.png)</picture> 

Quick Notes showing its context aware: asking if I want to paste the XDA article link on the note.

在典型的苹果时尚中，快速笔记*只有在你有一支苹果铅笔的情况下才有效*。用手指滑动没有任何作用。

 <picture>![iPad Air with iPadOS 15 running Quick Notes.](img/0a1dbb33fb27c29f26636868409c2218.png)</picture> 

Quick Notes in action.

## 实时文本在英文和中文上效果很好，但是现在有很多问题

另一个非常有用的新功能是“动态文本”，它将所有照片中的文本数字化。这意味着我可以抓拍一篇杂志文章的图片，并将文章中的文字转换成我可以编辑或复制粘贴的文本。Live Text 在目前的测试版中有很多问题，大约一半的时间会冻结或崩溃，但另外 50%的时间它会工作，工作得非常好。Live Text 能够接收到印在我的索尼相机按钮上的微小文字，甚至是画在画上的风格化的中文文字。只需抓拍照片，然后点击照片应用程序中的文字，应该会有一个光标覆盖在文字上，以便进行进一步的操作，如复制或在网络上查找。

作为一个能看懂中文但不会写的人，这个功能在和朋友分享地址或餐厅名称时会超级有用。

## iPadOS 15 的其他变化

iPadOS 15 还有无数大大小小的其他更新，包括改进的 Safari，使标签之间的循环更容易，全系统翻译(在大多数应用程序中只需突出显示一个单词，就会弹出翻译成另一种语言的选项)，以及开发人员直接在 iPad 上建立 iPadOS/iOS 应用程序并提交到苹果商店的能力。其中一些，比如翻译，已经做得很好了。随着我们花更多时间使用 iPadOS 15，我们将进一步测试这些功能。

 <picture>![System wide translation on iPadOS 15.](img/1580968553e352198ac52aedd3f080d2.png)</picture> 

System-wide translation working on Safari in iPadOS 15 Beta 1.

## iPadOS 15 进一步使 iPad 成为一台功能强大的工作机器

自 2015 年以来，苹果一直声称 iPad Pro 可以替代电脑。考虑到 iPad 一次只能打开一个应用程序，并且没有文件管理系统，这种说法在当时是可笑和侮辱性的。但是苹果每年都在慢慢更新 iPad 的软件，使其功能越来越强大。

 <picture>![iPad Air running iPadOS 15 beta.](img/ee6bdc5e589d3f2071945be5a11fbb50.png)</picture> 

Multi-tasking on the iPad Air is better than before.

这些新的更新改变了我的立场吗？我认为 M1 在新的 iPad Pro 上有些过头了。有一点——我认为改进后的分屏多任务将使像我这样的作家更容易写出文章。我真的认为 Quick Notes 是一个游戏规则改变者，它会让人们不太可能使用 Google Keep 和 Evernote 这样的替代品。但我仍然渴望一个真正免费的主屏幕网格，在可调整大小的浮动窗口中运行应用程序的能力，以及更好的外部显示支持。

但那是我特殊的使用需求；对许多人来说，iPad 已经足够用了，而 iPadOS 15 则是锦上添花。

 <picture>![The 11-inch iPad Pro 2021 comes with Apple's M1 chip and 5G, making it one of the most powerful tablets out there.](img/cc8edd58f8f6669c7c28ebca7ff8c60d.png)</picture> 

iPad Pro 2021 11-inch

##### 苹果 iPad Pro 11 英寸(2021 年)

11 英寸的 iPad Pro 可能没有迷你 LED 屏幕，但它仍然有改变游戏规则的 M1 处理器，并具有高度便携的尺寸。

 <picture>![The 12.9-inch iPad Pro comes with the powerful Apple M1 processor and a stunning mini-LED display.](img/99b89d94574484cef3f7cff61838a257.png)</picture> 

12.9-inch iPad Pro

##### 苹果 iPad Pro 12.9 英寸(2021 年)

这款 12.9 英寸 iPad Pro 上的屏幕要亲眼看到才会相信。加上 M1 芯片，这对于一台 iPad 来说几乎太强大了。

 <picture>![The new Magic Keyboard is specially designed to mount the new and slightly thicker 12.9-inch iPad Pro. It retains the same fluid experience as the previous model but you can now also get it in white color.](img/05c1f04ccaaabec872f05fa718ce7290.png)</picture> 

Magic Keyboard for iPad Pro 2021 12.9-inch

##### 适用于 iPad Pro 12.9 英寸的苹果魔法键盘

如果你想充分发挥 iPad Pro 的潜力，你需要一个键盘，苹果官方的 Magic Keyboard 在相对较薄的 folio 外壳上拥有最佳的打字和触控板体验。