# 如何在 iPhone 上设定“电池电量低”或“电池电量已满”的声音通知

> 原文：<https://www.xda-developers.com/how-to-set-audible-battery-notification-iphone/>

# 如何在 iPhone 上设定“电池电量低”或“电池电量已满”的声音通知

这份详细的指南将教你如何在 iPhone 上设置电池电量快用完或充满时的声音通知。

多年来，Android 手机一直提供低电量和满电量警报。然而，伟大的 iPhone 却不是这样。当你的电池充满时，iOS 根本不会通知你。同样，低电量警告是一个无声的弹出窗口，只有在手机解锁时你才会看到。不过，好消息是，多亏了[苹果快捷方式应用](https://www.xda-developers.com/guide-shortcuts-macos/)，你可以在 iPhone 上创建自己的电池通知。以下是方法。

## 如何在 iPhone 上设定声音电池通知

1.  在你的 iPhone 上启动**快捷方式**应用。
2.  点击底部导航栏中的**自动化**选项卡。
3.  点击**创建个人自动化**。
4.  滚动列表并点击**电池电量**。
5.  这是你必须决定它是低电量还是满电量通知的地方。您可以相应地设置滑块。
6.  如需电池电量已满的通知，将滑块拖至最右侧，并在其下方的列表中选择**等于 100%** 。
7.  对于低电量通知，向左拖动滑块，直到它显示所需的百分比，如 20%。从下面的列表中选择**低于 20%** 。
8.  点击右上角下一个的**。**
9.  点击屏幕底部的搜索栏。
10.  搜索**通知**。
11.  从列表中选择**显示通知**。
12.  点击 **Hello World** 旁边的箭头图标将其展开。
13.  在**标题**字段中输入**电池警报**。很明显，你可以给它起任何你想要的名字，但是我更喜欢用我的名字来描述。
14.  确保**播放声音**选项打开。
15.  选择 **Hello World** ，删除，键入**你的电池电量低。**或**您的电池已经充满电。** —取决于您正在构建的自动化。您也可以将文本更改为您想要的任何其他内容。
16.  之后点击右上角下一个的**。**
17.  运行前关闭**询问，得到提示后确认。否则，该特性将不起作用，因为它会用一个听不见的通知来提示您，请求手动许可来运行自动化，这违背了整个目的。**
18.  点击右上角的**完成**。
19.  瞧啊。现在，每当你的手机电池电量低/满时，你会收到一个声音通知。
20.  您可以为每个低/满电池实例创建两个自动化。只需遵循相同的步骤，并相应地调整第二个自动化。

* * *

就我个人而言，我不使用任何电池警报自动装置，因为我不在乎我的 iPhone 何时充满电，我很少让电池电量下降到 20%以下。尽管如此，拥有创建这些自动化的选项对苹果来说是一个受欢迎的补充。它只是反映了 Shortcuts 应用程序有多么强大，以及在某种程度上，它如何能够在 iOS 上定制体验。

您会使用快捷方式自动功能在 iPhone 上接收电池声音通知吗？请在下面的评论区告诉我们。