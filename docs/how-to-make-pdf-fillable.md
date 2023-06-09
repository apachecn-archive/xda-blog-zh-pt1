# 需要分享一个 PDF 表单？以下是如何使 PDF 可填充

> 原文：<https://www.xda-developers.com/how-to-make-pdf-fillable/>

有多少次你收到一个需要填写的 PDF 文件，却没有方便的方法去做？我们都经历过这种情况，打印文档或找到可以用来填表的软件的麻烦可能有点烦人。像 Microsoft Word 这样的应用程序实际上可以将 PDF 文件转换成可编辑的格式，但它们经常在这个过程中破坏格式，而且 Microsoft Word 也不是一个免费的工具。即使您不是自己填写表单的人，您也可能会因为没有让其他人更方便地填写您的表单而感到难过。幸运的是，有很多方法可以让任何打开 PDF 文件的人都可以填写它。

当然，最官方的方法是在你的台式机或笔记本电脑上使用 Adobe Acrobat DC(付费版)。但是我们是免费工具的忠实粉丝，我们在这里帮助你免费创建一个可填写的 PDF 表单。为此，我们将使用一个名为[的在线工具。这个工具也可以作为一个桌面应用程序，但很像 Adobe Acrobat，像这样的高级编辑功能是付费的。网络版支持广告，但你可以免费使用。但是有一些限制——文件大小必须小于 10MB，并且少于 100 页。](https://www.pdfescape.com/)

## 从头开始创建可填充的 PDF

PDFescape 为您提供了从头创建自己的 PDF 表单或上传 PDF 文件进行编辑的选项。如果您已经创建了表单，但不知道如何使其可填充，这将非常有用。然而，我们将从头开始制作一个。我们将用一个简单的表格来展示各种可能性。

*   前往[www.pdfescape.com/open](https://www.pdfescape.com/open/)并选择*创建新的 PDF 文档*。选择页数(最多 25 页)和页面尺寸，然后点击*创建*。
*   首先，将所需的文本添加到表单中。点击左上角的*文本*按钮添加文本。您可以从一些字体、字体大小和其他格式选项中进行选择。就像我们说过的，我们在这里举一个非常简单的例子。例如，假设我们正在为一个事件创建一个注册表单。这是我们希望在示例中创建的表单的基础。

*   现在，我们必须添加我们想要用来使 PDF 可填充的表单域。对于*姓名*和*电子邮件*字段，我们打算使用文本表单字段类型。这允许用户输入单行文本。点击*表单域*，选择默认类型*文本*，点击*选择*。然后在你想放置它的地方画一个场。您可以简单地单击任意位置，在那里创建一个具有默认尺寸的字段，并在之后调整其大小。

一旦创建了该字段，您就可以自己填充它，作为给用户提示应该写什么的一种方式。名为 *Name* 的字段应该是不言自明的，但它可能对其他人有用。

*   对于国家字段，我们可以使用下拉字段类型。

1.  *   首先点击*表单字段*，然后选择*下拉*类型，点击*选择*。单击要放置字段的位置，并根据需要调整其大小。
    *   要在列表中添加多个选项，右键单击表单域并选择*对象属性*。

*   *   将每个选项作为单独的一行添加到*字段选项*的旁边。完成后点击*确定*。
    *   现在，您有了一个下拉菜单，可以从您添加的选项中进行选择。
*   对于年龄字段，假设我们只想指定一个年龄组。我们可以为此使用单选按钮。方法如下:

1.  *   点击*表单字段*，然后选择*电台*类型，点击*选择*。
    *   为了使单选按钮按预期工作——在中，您只能选择一个——您需要一次创建所有单选按钮。我们将在这里创建六个选项。您也可以右键单击一个现有的按钮，并选择*复制*将其附加到同一组按钮。
    *   现在，单选按钮没有标签，所以您必须将它们作为文本添加。最后，它看起来会像这样:

*   接下来，为了选择兴趣，我们将使用常规复选框。与单选按钮不同，这些按钮允许您选择任意多的选项。点击*表单字段*，选择*复选框*类型，然后点击*选择*。勾选你认为合适的复选框。与单选按钮非常相似，复选框没有附加标签，所以您必须手动添加一些文本。您的表单应该看起来像这样，虽然希望有更好的对齐。

*   对于最后一个字段，我们的目标是让用户书写更长的文本，所以我们将使用文本段落，而不是标准的文本表单字段。点击*表单字段*，选择*文本段落*类型，然后点击*选择*。然后，画一个供用户书写文字的方框。至此，我们的表单就完成了。
*   现在，使用左侧边栏并点击*保存&下载 PDF...*按钮(带有两个箭头的绿色方块)。现在你就有了一个合适的 PDF 文件。您可以在任何 PDF 阅读器中打开它，它将是可填充的。以下是填写后的样子:

现在，您可以与任何人共享您的原始文件，并要求他们填写它。当然，你不必完全按照我们的方式来设计它——我们只是想用这样的工具展示一些可能性。

## 使用现有的 PDF

虽然上述步骤绝对是创建可填充 PDF 文件的有效方法，但它并不总是您想要的。如果您收到一个 PDF 文件，并且您想将那个转换成一个可填充的表单，该怎么办？或者，您可能使用了像 Microsoft Word 这样更强大的工具来格式化文档，但现在您希望它是可填充的？PDFescape 也可以做到这一点。下面是它如何工作的一个快速展示:

*   您的 PDF 将会打开，现在您有了和以前一样的工具来使它可填充。
*   在此添加您需要添加的所有字段。您还可以添加更多的文本，如果您想使用单选按钮或复选框，这很重要。以下是我们在示例中所做的工作:

*   没有用于签名的字段，但您应该不需要。大多数 PDF 阅读器允许您对文件进行注释，如果需要，可以将其用于签名。对于像[平板电脑](https://www.xda-developers.com/best-windows-tablets/)和[敞篷车](https://www.xda-developers.com/best-convertible-laptops/)这样的设备，用户甚至可以使用数字笔来书写他们的签名。

创建像这样的可填写表单使获取表单的答案变得容易得多，因为填写表单的人不需要任何特殊的软件来完成它。它可能不适用于非常基本的 PDF 查看器——比如手机上预装的软件——但是如果它允许注释，你应该没问题。我们用微软 Edge 浏览器中的 PDF 浏览器填写了这些表格。

这是可以创建可填充 pdf 的工具的一个例子，但是还有其他的。例如，LibreOffice 是另一个让你做到这一点的免费工具。我们使用 PDFescape 是因为它更简单，不需要任何安装。我们希望本指南对您有用。如果我们还有什么需要补充的，一定要让我们知道。