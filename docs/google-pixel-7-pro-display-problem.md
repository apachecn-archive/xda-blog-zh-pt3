# 谷歌 Pixel 7 Pro 可能有一个大的显示问题

> 原文：<https://www.xda-developers.com/google-pixel-7-pro-display-problem/>

谷歌 Pixel 7 系列最近发布了，我们已经花了很多时间和专业人士和非专业人士在一起。我们一直喜欢[的相机](https://www.xda-developers.com/google-pixel-7-pro-camera-review/)，软件，甚至升级后的显示屏。然而，事实证明，在高亮度下使用时，显示屏是一个电池杀手——比我们在几乎任何其他旗舰设备上看到的电池杀手都要多。

自周一以来，我一直在使用 Pixel 7 Pro，我注意到电池寿命比谷歌 Pixel 6 Pro 有很大改善...直到我走出去。昨天早上出去喝咖啡，50%准时坐在屏幕前近三个小时。从各方面来看，这确实是很好的电池寿命。然而，走到外面，边走边用我的手机，十五分钟内电池寿命立刻下降了 10%左右。我很快意识到，我在外面时，我的亮度更高了。我询问了团队的其他成员，Valnet 的技术品牌负责人 Daniel Bader 提到他也经历过同样的事情。

事情是这样的，*很明显*在室外使用显示器会消耗更多的能量。问题是能量消耗似乎真的不成比例。我与 XDA 家族的其他成员交谈过，并从他们的设备上收集了读数，看起来谷歌 Pixel 7 Pro 可能有一个相当大的显示问题。我在 XDA 显示器分析师 Dylan Raga 的帮助下对此进行了调查，我们使用 Pixel 6 Pro 和 Galaxy S22 Plus 的测量数据来构建 Pixel 7 Pro 非凡行为的背景。

## Pixel 7 Pro 的显示屏出了什么问题？

在 600 尼特，我们的所有四个谷歌 Pixel 7 Pro 设备都在 3.5W 和 4W 之间。更糟糕的是:在最大亮度下(谷歌 Pixel 7 Pro 的额定亮度高达 1500 尼特，我触发了高亮度模式)，它的功耗高达 6W。这些显示器亮度等级通常测量 1% APL 时的峰值亮度——或者换句话说，屏幕的一小部分被点亮。当显示白屏(100% APL)时，整个面板的高亮度模式应该跳到 1000 尼特，看起来也差不多是这样。

作为参考，三星 Galaxy S22 Ultra 将使用约 600 尼特的 2W，约 1000 尼特的 4W。Dylan Raga 告诉我，我收集的数据显示，Pixel 7 Pro 显示器的功耗比三星 Galaxy S22 Ultra 和三星 Galaxy S22 Plus 高出约 50%。

我们在对三星 Galaxy S22 Plus 和谷歌 Pixel 6 Pro 的显示器评测中读取了功耗数据。三星 Galaxy S22 Plus 在 1100 尼特时似乎消耗了 4.5 瓦，这是一个相当可观的数字。相比之下，谷歌 Pixel 6 Pro 的 4W 接近 800 尼特。迪伦向我指出，如果你将他的谷歌 Pixel 6 Pro 显示器功耗图向同一方向延伸，你基本上会越过我们在谷歌 Pixel 7 Pro 上经历的相同值。这表明谷歌过去在面板方面存在更大的问题，谷歌 Pixel 7 Pro 似乎只是让情况变得更糟。

我与 *Android Police* 的 Ben Sin、Daniel Bader 和 Manuel Vonau 进行了交谈——这三个人拥有谷歌 Pixel 7 Pro 设备，这些设备来自世界不同地区的公共关系。我给他们三个都发了指令，告诉他们如何在最大亮度下测量显示器的耗电量。他们所有的价值观都和我的大致一致。在下表中，你可以看到谷歌 Pixel 7 Pro 与三星 Galaxy S22 Plus 和谷歌 Pixel 6 Pro 的对比。

| 

功率消耗

 | 

谷歌 Pixel 6 Pro

 | 

谷歌 Pixel 7 Pro

 | 

三星 Galaxy S22 Plus

 |
| --- | --- | --- | --- |
| 100% APL 时 600 尼特 | 2.9W | 3.5W-4W | 2W |
| 100% APL 时 800 尼特 | 4W | - | - |
| 100% APL 时 1000 尼特 | - | 6W | 4W |

## 谷歌 Pixel 7 Pro 的显示功耗到底有多差？

为了更好地理解这个问题，谷歌 Pixel 7 Pro 的张量 G2 可能有大约 10-12W 的 TDP。我们还没有完成我们的测试，但这意味着在全手动亮度下，显示器单独使用的功率可能略低于芯片组最大功率的一半。在玩高强度游戏时，在高亮度模式下，您可以随时使用高达 18W 的电池。这将在不到三个小时内耗尽任何智能手机电池，而这仅仅是显示屏和芯片组。你的手机也有其他组件，所以如果你使用高亮度的 Pixel 7 Pro，你会比在相同条件下在竞争对手的设备上更快地粘在墙上。

## 谷歌能做些什么来解决这个问题？

在这个初步阶段很难说。我们已经在多个设备上进行了测试，发现所有设备的功耗相同。值得一提的是，我们还在两台谷歌 Pixel 7 设备上进行了读取，它看起来正常得多，所以这似乎是专业人士专有的问题。目前还不清楚谷歌是否能够通过软件更新让这个面板更有效，不过我怀疑它不会这么做。尽管如此，这就是为什么我们说“*可能*有一个大的显示问题——谷歌可能最终会解决它。不管是硬件问题还是软件问题，目前都还不确定——我们只知道有问题。

值得一提的是，在较低的亮度下，Pixel 7 Pro 显示器的功能更接近预期。迪伦指出，我收集的在最低亮度下使用显示器的功率值仍然偏高，大约消耗 0.7 瓦。尽管如此，这比达到 6 瓦要容易管理得多。如果你对谷歌 Pixel 7 Pro 持观望态度，我们建议你等等看会发生什么。谷歌 Pixel 7 似乎也没有同样的问题，这可能使它成为那些长时间呆在户外、阳光充足的环境中或者只是喜欢高亮度显示的人的更好选择。

我们已经联系了谷歌进行评论，如果有回音，我们一定会更新这篇文章。

## 谷歌的 Pixel 7 Pro 也有其他显示问题

这也不仅仅是显示器功耗的问题。GSMArena 的普拉萨德·纳伊克在 Twitter 上指出，即使在关闭后，显示屏仍会在一小段时间内保持活动状态。

我在我的单位也注意到了同样的问题，只有当我看到这条推文时，我才意识到这是原因。有几次我一直在听音乐，用手机，关掉屏幕，把它转过去放进口袋。我已经以这种方式跳过几次曲目，这令人难以置信地沮丧，但我认为这只是我做错了什么。然而，我已经证实了我也有同样的问题，在我关闭屏幕后，显示器仍然亮着大约一秒钟。

目前还不清楚这是否是一个错误，或者是否可以通过禁用任何特定设置来修复。如果我们听到更多，我们一定会更新这篇文章。