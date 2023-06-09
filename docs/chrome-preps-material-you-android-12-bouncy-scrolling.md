# Chrome 为谷歌的 Material You 和 Android 12 的弹性滚动做准备

> 原文：<https://www.xda-developers.com/chrome-preps-material-you-android-12-bouncy-scrolling/>

虽然我们距离第一个稳定的 Android 12 版本还有几个月的时间，但谷歌已经开始更新其应用程序，以遵循 Android 12 新的 [Material You](https://www.xda-developers.com/material-you/) 设计语言。最近，谷歌在 Android 版 Chrome 90 中添加了一个新标志，为应用程序的溢出菜单带来了一个受你启发的微小设计变化。与此同时，Chrome for Android 也支持 Android 12 的弹性滚动，我们[在今年早些时候的 Android 12 DP3](https://www.xda-developers.com/android-12-dp3-features/#android12dp3overscrollanim) 中首次发现了这一点。

据 *[Android Police](https://www.androidpolice.com/2021/05/25/chrome-for-android-is-getting-a-material-you-tweak-heres-how-to-enable-it/)* 报道， [Chrome 90](https://www.xda-developers.com/google-chrome-90-stable-rollout/) for Android 中新的“#theme-refactor-android”标志对该应用的溢出菜单进行了小规模翻新。正如你在所附的截图中看到的，变化并不显著。但是溢出菜单的圆角符合 Android 12 Beta 1 中你设计的所有材料变化。谷歌可能会在未来几个月引入更多这样的标志，根据 Material You 指南更新用户界面。

*L:当前素材主题设计，R:你更新的新素材(图片:安卓警察)*

如果你想在 Chrome for Android 中查看你设计的材料变化，你可以前往 *chrome://flags* ，搜索上面提到的标志，并启用它。请注意，要使更改生效，您必须重新启动浏览器两次。

除了更新溢出菜单，谷歌还在 Android 版 Chrome 中增加了对 Android 12 的弹性滚动的支持。对于不知情的人，我们首先发现了今年早些时候 Android 12 DP3 中新的超滚动画。正如你在所附视频中看到的，当你到达页面底部后向上滚动时，overscroll 动画会取代当前的 inkwell 风格动画。

谷歌 [报道](https://9to5google.com/2021/05/26/google-chrome-android-12-stretchy-scrolling/)Android 上的谷歌 Chrome 将很快在运行 Android 12 的设备上获得对这种新的弹性滚动动画的支持。该出版物发现了最近添加到 Chromium 中的关于新动画效果的代码更改。它的描述称:“Android 12 和更高版本为 overscroll 提供了一种新的视觉行为，可以拉伸滚动的内容。此补丁使用弹性过度滚动标志在 Android 上启用此行为。”

该报告进一步指出，新的动画风格最初将隐藏在 chrome://flags 中的一个实验性标志后面。它还透露，代码更改没有提到任何关于限制 Android 12 滚动效果的内容，这表明它可能会在发布后进入运行旧版本 Android 的设备。