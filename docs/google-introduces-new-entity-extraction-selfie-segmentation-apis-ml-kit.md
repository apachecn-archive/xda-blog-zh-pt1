# Google 将实体提取、自拍分割 API 引入 ML 工具包

> 原文：<https://www.xda-developers.com/google-introduces-new-entity-extraction-selfie-segmentation-apis-ml-kit/>

几年前，谷歌[推出了 ML Kit](https://www.xda-developers.com/google-ml-kit-machine-learning/) ，让开发者更容易在应用中实现机器学习。从那时起，我们已经看到了用于数字墨水识别、设备上翻译和人脸检测的 API。现在，谷歌正在向 ML 工具包添加新的实体提取和新的自拍分割功能。

谷歌表示，新的实体提取 API 将允许开发者从原始文本中检测和定位实体，并根据这些实体采取行动。

谷歌表示:“该 API 适用于静态文本，也可以在用户打字时实时运行。”“它支持 11 种不同的实体和 15 种不同的语言(未来还会有更多)，允许开发人员为用户提供更丰富的文本交互体验。”

以下是受支持的实体:

*   **地址** *(剑桥第三街 350 号)*
*   **日期-时间****(2020 年 12 月 12 日，明天下午 3 点)(明天下午 6 点见)*
*   **邮箱**【(entity-extraction@google.com】T2)
*   **航班号*** *(LX37)*
*   **伊班****(CH52 0483 0000 0000 0000 9)*
*   **ISBN ****(978-1101904190)*
*   **货币(包括货币)****(＄1225 美元)*
*   **支付卡*** *(4111 1111 1111 1111)*
*   **电话号码** *((555) 225-3556，12345)*
*   **跟踪号码****(1z 204 e 380338943508)*
*   **网址**【https://en.wikipedia.org/wiki/Platypus, (www . Google . com，seznam.cz)

谷歌表示，它一直在测试 TamTam 的实体提取 API，以允许该应用程序在聊天对话中向用户提供有用的建议。例如，当一个地址出现在屏幕上时，点击它会弹出一个菜单来复制地址，用另一个应用程序打开，或者获得该位置的方向。

> 实体提取 API 中的神经网络标注器/模型工作如下:给定的输入文本首先被分割成单词(基于空格分隔)，然后生成某个最大长度的所有可能的单词子序列(在上面的示例中为 15 个单词)，并且对于每个候选项，评分神经网络基于其是否表示有效实体来分配一个值(在 0 和 1 之间)。
> 
> 接下来，删除重叠的生成实体，优先选择得分较高的实体，而不是得分较低的冲突实体。然后，使用第二个神经网络将实体的类型分类为电话号码、地址或在某些情况下的非实体。

谷歌表示，ML Kit 的实体提取 API 建立在 Android 10 推出的智能 Linkify 功能的技术基础上。

除了基于文本的实体提取，谷歌还宣布了新的自拍分割 API。该功能将允许开发者将背景从场景中分离出来。这将使用户能够为自拍添加酷炫的效果，甚至将自己插入到更好的背景中。谷歌表示，新的 API 能够在 Android 和 iOS 上以低延迟产生出色的结果。

ML Kit SDK 将谷歌多年来在机器学习方面的工作整合到一个 Firebase 包中，移动应用程序开发人员可以使用它来增强他们的应用程序。自从 ML Kit 推出以来，已经推出了许多 API，使得开发人员可以更容易地在应用程序中实现机器学习功能。有了实体提取和自拍分割，未来的应用会变得更好。