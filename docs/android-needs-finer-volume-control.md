# 谷歌是时候给安卓系统添加细粒度的音量控制了

> 原文：<https://www.xda-developers.com/android-needs-finer-volume-control/>

我喜欢在睡前听播客和有声读物，因为它能帮助我睡得更好。理想情况下，当你在安静的环境下听有声读物或播客时，你需要的是合适的音量——在很长一段时间内听起来都很舒服。声音大一点，会分散注意力，导致听力疲劳；声音小一点，一切都变得难以理解。我对音量变化和响度相当敏感，所以我总是花一些时间摆弄音量滑块，以找到一个舒适的水平。然而，由于 Android 处理媒体音量和音量控制的方式，找到最佳点是一场持久的斗争。无论你多么小心地调整音量滑块，它总是有点太大声或太安静。这个问题在有线和无线入耳式耳机中比在耳挂式耳机中更加明显。

这在我近年来使用的几乎所有安卓手机上都是一个难题。例如，在 iQOO 7 Legend 上，即使是最低的音量级别对于在睡前听睡眠声音或播客来说也太大声了。此外，每个音量步长都有一个很大的跳跃，所以你总是会被夹在音量太大或太小之间。如果你想从目前的水平上适度增加或减少，这几乎是不可能的。我的[小米 Mi 10i 5G](https://www.xda-developers.com/xiaomi-mi-10i-5g-review/) 基于 [Android 12L](https://www.xda-developers.com/android-12l/) 的运行 Pixel 体验在音量较低时更好，但在第三次或第四次点击后，我遇到了同样的情况，每次音量跳跃都变得非常巨大。

由于 Android 处理媒体音量的方式，找到最佳音量点是一场持久的斗争。

音量问题因 Android 的“绝对音量”控制而变得更加复杂，该控制统一了连接的蓝牙耳机的音量和手机媒体音量。这在方便性方面是一个巨大的胜利，因为它消除了独立调节蓝牙耳机上的物理音量控制和手机媒体音量的痛苦，这意味着改变手机上的音量可以控制蓝牙设备上的音量，反之亦然。

然而，这种便利是有代价的:失去了对音量的精细控制。

我不确定谷歌是什么时候把蓝牙和手机媒体音量结合起来的。我记得在早期的 Android 版本中，我可以独立于手机媒体音量来调节我的 Sennheiser HD 4.50 耳机的内部音量。这提供了更大的灵活性和对总音量输出的精确控制。我可以将手机媒体音量设置为 5，然后使用耳机上的物理控件来调整内部音量，直到我找到最佳位置。

问题是，虽然 Android 提供了一个选项来禁用绝对音量控制，这将蓝牙和手机音量分离，但我对这个选项的结果喜忧参半。虽然它可以与我的森海塞尔耳机和 OPPO Enco M31 neckband 配合使用，但它对真正的无线耳机没有任何作用。只有当你的蓝牙耳机有自己的音量控制时，它才真正有用。

以前有一个非常有效的解决这个问题的方法，就是精准量 app 的形式。该应用程序连接到您手机的音频系统，以覆盖 Android 的 15 步音量限制，并增加 100 步音量。虽然它已经很长时间没有更新了(实际上是从 2017 年开始)，而且它不再能在运行 Android 9 Pie 和更高版本的设备上工作。

在你提到它之前，是的，我也试过用 [build.prop 方法将音量步长](https://www.xda-developers.com/how-to-add-more-steps-to-your-volume-slider-root/)从 15 增加到 30。然而，它在我的例子中不起作用，增加了空的步骤，而不是将总体积平均分布在 30 个步骤中。不仅如此，这个选项对于大部分 Android 社区来说是不可行的，因为它需要[根访问](https://www.xda-developers.com/root/)。

## 谷歌应该从三星和 LG 那里汲取灵感

一个简单的解决方案是向媒体卷添加更多切实的步骤。

那么，谷歌可以做些什么来让 Android 用户对音量输出有更多的控制权呢？一个简单的解决方案是向媒体卷添加更多切实的步骤。如上所述，Android 目前提供 15 个音量步骤。相比之下，我的索尼随身听 MP3 播放器有 32 步。三星提供了一款名为[声音助手](https://galaxystore.samsung.com/detail/com.samsung.android.soundassistant?langCd=en)的应用，让 Galaxy 智能手机用户增加 150 个音量级。同时，当您启用专用 DAC 时，LG V30 和 V40 提供 75 步。如果谷歌不想走三星和 LG 的长度，即使 30 步也绰绰有余。默认情况下，Android 可以继续使用 15 步，同时给高级用户一个选项，以启用额外的步骤来更好地控制音量。

谷歌可以考虑增加的另一个选项是主音量滑块，它将限制系统范围内的整体音量输出。因此，例如，您可以将主滑块设定为 60%，以降低每个音量步长的整体强度/响度。还有一种选择是让 Android 媒体应用程序添加自己的音量滑块，独立于系统媒体音量工作。这样，您可以使用两个滑块来微调最终音量。

当然，我不是第一个提出这个问题的人。这是一个古老的问题，许多 Android 用户已经面临多年了，还没有引起谷歌的注意。据我所知，这是一个特别困扰一些用户的问题，在我自己的使用中，这个问题也存在了很长时间。

虽然我们都知道 Android 已经从早期走了很长一段路，但重要的是这些改进和生活质量的变化不会被忽视。在这一点上，它是一个成熟的操作系统，但诸如此类的问题阻碍了它的发展。