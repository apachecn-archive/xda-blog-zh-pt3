# iPadOS 16 Dev Beta 1 实际操作:iPad 实现真正的多任务处理！

> 原文：<https://www.xda-developers.com/ipados-16-developer-beta-1-hands-on/>

自 2015 年该系列首次亮相以来，苹果一直称 iPad Pro 为“电脑替代品”，当时，这种说法太过牵强。当时的 iPad Pro 一次只能运行一个应用程序，而且没有文件系统。什么样的电脑不能多任务或者下载存储一个文件？iPad Pro 是一款巨型 iPhone。

这是一个缓慢而漫长的过程，但七年后的今天，iPad Pro 终于兑现了最初的承诺，推出了 T4 的 iPad OS 16 T5，这是 iPad 操作系统自问世以来最大的一次革新...永远不会。即使在其当前的开发者测试版中(最终的消费者就绪软件还要几个月才能上市)，iPadOS 16 也是一个绝对的游戏改变者。在过去的 12 个小时里，我一直在一台 [2021 iPad Pro(与 M1)](https://www.xda-developers.com/ipad-pro-2021-review/) 上测试 iPadOS 16 的[开发者测试版，下面是新的内容。](https://www.xda-developers.com/ipad-might-finally-be-laptop-replacement/)

## 舞台监督

Stage Manager 是苹果新窗口组织系统的官方名称，这是 M1 驱动的 iPads 多任务处理的新水平。如上所述，iPads 最初一次只能运行一个应用程序。但 2017 年的 iOS 11 引入了分屏多任务处理，允许 iPads 同时运行两个应用程序，并在一个更小的浮动窗口中运行第三个应用程序。这提高了 iPad 作为生产力机器的地位，但这还不足以完成真正的工作。Stage Manager 最终解决了这个问题，它允许 M1 驱动的 iPads 在可调整大小的窗口中运行应用程序。

要激活 Stage Manager，你必须在 iPadOS 16 中进入控制中心，点击带有一个矩形和三个圆点的新图标(如上截图)。一旦你点击它，任何打开的应用程序(之前拉伸了整个 iPad 屏幕)都会缩小，变成一个浮动窗口。你可以用手指移动窗口，但有趣的是，你必须用 iPad 的鼠标光标来调整窗口的大小。我不确定这是一个将在后续版本中修复的错误还是苹果的意图，但如果是后者，这意味着苹果认为 Stage Manager 主要是为与[苹果的 Magic Keyboard](https://www.xda-developers.com/apple-standalone-magic-mouse-keyboard-trackpad-black-silver/) 或蓝牙鼠标/触控板一起使用而设计的。

在 Stage Manager 中，默认情况下，一次只能在浮动窗口中打开一个应用程序。如果你点击另一个应用程序，该应用程序会在浮动窗口中打开，但你之前的应用程序会被推到左侧。要同时打开多个应用程序，您必须打开一个浮动窗口，然后长按并拖动另一个应用程序进入视图。习惯这个动作需要几秒钟，但一旦我掌握了窍门，我就开始用下面这样的应用程序填充我的 iPad Pro 屏幕——我同时打开了 Safari、Slack、YouTube 和 Twitter。iPadOS 16 最终将允许这些窗口变得透明。但是现在在这个测试版软件中，我不能这么做，所以 Twitter 在后面被完全屏蔽了。

我可以打开这些配对的多个实例，例如，我可以以浮动形式打开三个工作窗口(Slack、Safari、Gmail)，在左侧的选项卡中打开另一组休闲窗口(YouTube 和 Instagram)。是的，第三方应用程序，甚至是谷歌的，现在都可以以浮动窗口的形式打开，尽管它们有很多问题(有时屏幕会变黑，不重新启动就不能正常显示)。下面，我在 iPad Pro (12.9 英寸屏幕)上的浮动窗口中并排打开了 Google Drive 和 Google Docs。如果我愿意，还有空间放第三个应用程序。这就是让我高效完成工作的多重任务。

现在你可能会认为 iPad Pro 的屏幕太窄了，无法同时运行三个以上的应用程序。嗯，这就是 iPadOS 16 的另一个巨大的附加功能 T1 的用武之地...

## 外部显示器支持

iPadOS 允许 M1 驱动的 iPads 将其显示扩展到外部显示器。这在以前是不可能的，因为将 iPad 插入外部显示器只会镜像屏幕。值得注意的是，外部显示器上的 iPad 屏幕*始终处于舞台管理器模式*(你不必像打开 iPad 主屏幕一样打开它)，而 iPad 本身可以处于其常规布局或通过舞台管理器处于浮动窗口中。有了足够大的外部显示器，你可以同时打开五六个应用程序。苹果公司表示，在整个设置中，你最多可以打开八个。我下面的设置是将 iPad Pro 插入华为 MateView，后者 3:2 的纵横比对于多任务处理来说绝对是荣耀的。

这个 UI 设置终于让我可以像在“普通”电脑上一样工作了。我在 XDA 的工作需要我随时打开 Slack，一个网络浏览器(在这里是 Safari ),我还经常使用 Twitter 和 Adobe Lightroom。所有这些应用都能在 iPadOS 上完美运行。在 WWDC 的发布会上，苹果承诺为 iPadOS 开发“桌面级应用”，因此这些应用只会越来越好。由于 2021 年的 iPad Pro 和 2022 年的 iPad Air 与苹果的 MAC 电脑运行在同一芯片上，这使得 MacOS 开发者可以轻松地将他们的应用移植到 iPadOS 上。

舞台管理器和外部显示器支持使 iPad Pro 成为现实的电脑替代品

舞台管理器和外部显示器支持是对 iPadOS 的突破性补充，从根本上改变了 iPad 的功能。这两个特点在我看来最终使 iPad Pro 成为现实的电脑替代品。不过当然，iPadOS 16 还有更多新功能。

## 显示缩放

如果你对 iPad 过于简单的分屏多任务处理感到满意，并且不需要浮动窗口，那会怎么样？嗯，iPadOS 16 在这方面也有所改进，增加了显示像素密度，这样你就可以在屏幕上看到更多信息。下面是 iPad Pro 在分屏视图下运行苹果的 Files 应用和 Twitter 的两张截图。你可以看到第一个截图以更大的形式显示了所有内容，因此你看到的比第二个要少。在第二组中，我可以一次看到多达 20-30 个文件夹(如果我有那么多的话)，屏幕上至少有两条推文。

## 视频的实时文本

Live Text 是去年为 iOS 和 iPadOS 推出的一项功能，允许你与照片中的文本进行互动，例如，你可以在照片中高亮显示一家餐馆的名称，复制文本并开始对该餐馆进行网络搜索。或者你可以复制并粘贴一个汽水罐配料盒的文本(前提是图像足够清晰)。

对于 iPadOS 16(和 iOS 16)，你现在也可以对视频这样做。最重要的是，你现在可以抓取视频中某个主题的剪切图像，并将剪切图像移动到另一个第一方苹果应用程序，如 Notes 或 Mail。解释起来有点复杂，所以只要看看下面的视频就知道了:我可以抓取我和我朋友的剪影，然后把那个 PNG 文件拖到苹果的 Notes 应用程序上。

不幸的是，这目前不能与任何谷歌应用一起使用(例如，我不能拖到 Gmail 或谷歌文档)，但第三方视频编辑应用 LumaFusion 支持这一点。

## 天气应用

这听起来很荒谬，但 iPads 直到现在都没有专门的天气应用程序。iPad 问世十多年了，却没有一款官方的苹果天气应用。好吧，这不再是 iPadOS 16 的情况，因为苹果的官方天气应用程序正在向 iPad 发展。它旨在利用更大的屏幕，显示详细的每小时天气预报，以及一系列附加信息，如紫外线指数，日出时间，甚至风速和风向。

## 其他花絮

还有其他重要的 iPadOS 16 更新我无法测试，因为它们在第一个测试版中不可用，包括 [Freeform](https://www.xda-developers.com/apple-freeform-whiteboard-collaboration-ipad-iphone-macos/) ，这是一个新的协作应用程序，允许多个 iOS/iPadOS 用户跳到一个空白区域，他们可以在那里写笔记、画草图、在字段中键入文本，以及在角落里主持实时 FaceTime 通话。

还有一个新的 [iCloud 共享照片库](https://www.xda-developers.com/apple-photos-sharing-wwdc-22/)，允许苹果用户为家人和朋友创建一个单独的照片库。每个人都可以贡献照片和编辑，所有人都会看到。我无法尝试这样做，因为我不使用 iCloud(我实际上是一个谷歌迷)，而且我的直系亲属中没有人使用苹果产品。但是这应该足够简单，没有什么突破性的。从很多方面来说，这是苹果在追赶谷歌照片。

还有改进的语音听写功能——我确实试过，但现在在测试版中有点问题——和“参考模式”，让创意人员使用 12.9 英寸的 iPad Pro 和 Liquid Retina XDR 显示器作为颜色指南，与 MacBook 和其他设备匹配颜色。这个功能对于色彩分级的视频专业人士应该非常有用。在写这篇文章的时候，我还不能测试这个特性。

总之，iPadOS 16 无疑是 WWDC 2022 上宣布的最重要的软件更新，它真正释放了 M1 iPad Pro 和 iPad Air 的隐藏潜力。这些设备已经是市场上最好的平板电脑，现在安装了更智能、功能更多的软件？iPads 将会占据更大的主导地位。

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

如果你想试用新软件，这里有[如何在你的苹果 iPad](https://www.xda-developers.com/how-to-install-ipados-beta/) 上安装 iPadOS 16 测试版。