# 三星 Galaxy S22 Ultra:骁龙 8 代 1 vs Exynos 2200

> 原文：<https://www.xda-developers.com/samsung-galaxy-s22-ultra-snapdragon-vs-exynos/>

三星每年都会更新其旗舰智能手机系列，每年都有一个有争议的问题:骁龙和 Exynos 哪个更好？Exynos 是该公司的内部芯片组，每年为其一些手机提供动力，尽管几乎总是欧洲是保证获得 Exynos 芯片的一个地区。美国倾向于获得骁龙芯片，然后在所有其他地区他们将获得什么芯片组是一个掷地有声的事情。今年，印度在[三星 Galaxy S22](https://xda-developers.com/samsung-galaxy-s22) 系列中首次获得了骁龙芯片，欧洲也像钟表一样获得了 Exynos。

正如我们所指出的，三星 Galaxy S22 Ultra 的零售部门似乎存在一些重大问题。有一些显示闪烁的问题已经被修复，还有一些性能问题。自从发表我们的文章以来，我已经有许多消费者在 Twitter 上联系我，说他们在基于 Exynos 的 S22 设备上遇到了类似的性能问题。我甚至看到[的一些用户](https://twitter.com/NilsAhrDE/status/1497259344857124874?ref_src=twsrc%5Etfw)说自从最近一次更新后，情况变得更糟了。还要记住，至少[根据著名泄密者 Max Jambor](https://twitter.com/MaxJmb/status/1497123983308824577) 的说法，三星意识到了 Exynos 设备目前面临的性能问题。

为三星说句公道话，我也有很多消费者告诉我，他们的设备没有问题。本文的目的**不是说每个用户都会有这种体验**，但是有相当多的消费者在抱怨他们设备的性能。我现在已经设法得到了一台由美国三星公关公司提供的[高通骁龙 8 代 1](https://www.xda-developers.com/qualcomm-snapdragon-8-gen-1/) 驱动的 Galaxy S22 Ultra 设备，我将它与我直接从三星爱尔兰购买的 Exynos 驱动的零售设备进行了测试。结果很可能符合你的预期。

## 三星 Galaxy S22 Ultra:骁龙 vs Exynos

作为背景，我最初打算将这两个设备都设置为新的，以便相互比较，但我觉得所做的任何测试都不能说明当前正在使用的实际设备。基准可以在一个什么都没有安装的空设备上理想化，人们买手机是为了超越基准来使用，对吗？

相反，开发者选项被用来防止任何后台进程在设备上运行，并且“不保持活动”在两个设备上都被启用。在可能的情况下，这些设备也与互联网断开连接，这样就不会收到干扰测试的推送通知。本质上，我确保没有后台进程在运行，也确保没有网络干扰。

这两款设备都已更新到最新的可用软件版本，内部版本号和内部版本日期如下。

*   **Exynos 版本:** S908BXXU1AVBF / S908BOXm1AVBF(构建日期:2 月 23 日)
*   **骁龙版本:**s908 u1ueu 1 ava 6/s908 u1oy m1 ava 6(构建日期:1 月 8 日)

### 基准

首先，我对这两款设备进行了并排基准测试，以测试它们之间的差异。我在我现有的两款 Galaxy S22 Ultras 上运行了 Geekbench 5 测试，并请 *TechnikNews* 的 [Nils Ahrensmeier](https://twitter.com/NilsAhrDE) 在他的 Exynos 设备上运行测试。

这些结果已经显示了 Galaxy S22 Ultra 的 Exynos 版本和骁龙版本之间的巨大性能差异，甚至在同一台设备上的两次运行中也是如此。然而，基准并不代表一切，一部手机完全有可能表现出色，同时也没有达到基准中的具体关键指标，从而获得高分。

### 节流和持续性能

持续的性能是使用智能手机时需要注意的最重要的指标之一。如果持续的表现很差，那么在可能很短的一段时间后，你的表现会大大降低。我对这两款设备进行了测试比较，虽然两者在性能上保持一致，但骁龙芯片组始终领先。尽管如此，这仍然显示了 Exynos 更合理的结果，但这本身并不表明有问题。

### 功率消耗

在运行 CPU 节流测试时，我能够测量我拥有的两款三星 Galaxy S22 Ultra 设备的峰值功耗。我震惊地发现，在测试的峰值，两个设备的屏幕都处于最低亮度，Exynos 变体和骁龙变体分别消耗了 **11.84W 和 7.76W** 。这是功耗的巨大差异，表明 Exynos 芯片组的效率有多低。这意味着在长期使用中，Exynos 2200 设备在负载下的电池寿命将会缩短。

需要说明的是，这部分是由手机的其他因素造成的，比如屏幕。然而，在能源使用上有很大的不同。

在我的测试中，我还发现了一个高空闲消耗，这意味着用户在 Exynos 设备上的待机时间将比骁龙短。

### 应用启动测试

我们设计了一个真实世界的应用启动速度测试，连续 10 次启动我们每天使用的几个流行应用。这些应用程序都是在设备上“冷”启动的，这意味着应用程序在启动前不会缓存在内存中。当应用程序的主活动第一次开始绘制时，计时就会停止，因此无需等待从网络加载内容。因此，该测试可以确定设备将应用程序从存储加载到内存的速度，但需要注意的是，该测试对应用程序和操作系统版本的变化非常敏感。鉴于我们比较的是同一款手机的两个版本，因此更容易得出直接的结论。

骁龙设备启动应用程序的速度比 Exynos 设备快得多。在这个指标上，Exynos 设备是我见过的性能最差的设备之一。平均来说，应用程序需要一秒多的时间才能启动。这听起来不多，但想象一下，试图在智能手机上快速同时做多件事？当你在工作的路上遇到每一个小小的阻碍时，情况会变得越来越糟。

## Exynos 三星 Galaxy S22 Ultra 的一般使用情况不佳

上面，我放了一个视频来展示我在 Exynos 版本中注意到的一些问题，这些问题在骁龙版本中并不存在。它作为证据展示了这些问题在现实世界中的影响，我在两台设备上都登录了相同的应用程序。我使用这两款设备的方式与平时没有什么不同，我在 Exynos 设备上登录的所有应用程序都与我在 OPPO Find N、一加 9 Pro 和谷歌 Pixel 6 Pro 上登录的应用程序相同。

所有这些性能问题，从延迟登录到 UI 口吃和延迟的笔集成，加在一起形成了糟糕的体验。手机很慢，它严重妨碍了我的工作，而且更新软件也没有改善这种情况。甚至截图和裁剪都需要几秒钟，而在骁龙设备上这几乎是一个瞬间的过程。Exynos 2200 的体验几乎相当于使用一款经济型设备，一切都比顶级旗舰产品的预期时间长一秒钟。

Exynos 2200 的体验几乎相当于使用一台廉价设备，顶级旗舰产品的一切都比预期多花了一秒钟

正如我已经提到的，我有几个用户联系我，谈论他们对这款设备的 Exynos 2200 版本的糟糕体验。没有一个使用骁龙芯片组的用户向我抱怨过同样的问题。我不确定是否每个 Exynos 用户都会有这些问题，但肯定会有相当一部分。我甚至试图在我的电池设置中启用高性能模式，但这并没有什么影响。我也没有看到任何内存管理成为问题的迹象，因为任何时候都有空闲的 RAM 可用。

在这些设备的其他方面，我还没有真正注意到任何差异。相机彼此很接近——如果不是平起平坐的话(尽管我认为从我自己的使用来看，高通略胜一筹)，稳定似乎对任何不太极端的东西都是一样的。在巴塞罗那四处走动和拍摄在这两种设备上都可以很好地工作，我没有注意到这方面的任何问题。

## Exynos 对 Android 生态系统很重要，但这种体验是不可接受的

当谈到 Android 智能手机时，我很痛苦地说，但 **Exynos 很重要**。高通几乎垄断了安卓旗舰市场...虽然不可否认，联发科正在迅速赶上。让该领域最大的 Android OEM 厂商三星在其产品组合的很大一部分中使用自己的芯片组给高通带来了一些压力，在理想情况下，希望使用 Exynos 芯片组的用户数量与希望使用高通芯片组的用户数量相等。

很难说这些问题的原因是什么。它很可能是 Exynos 2200，因为过去其他 Exynos 也没有与骁龙并驾齐驱。或者可能是三星巧合地设法搞乱了 Exynos 变种的软件。三星似乎没有对任何关于 Exynos 变体的出版物公开发表声明，因为 *ComputerBase* 甚至表示，尽管该公司进行了接触，但它拒绝透露是否会有更新。

在过去，就像 Exynos Galaxy S21 Ultra 一样，游戏性能在整个产品生命周期中一直很差，因为 Exynos 2100 就是无法运行，无论有多少软件更新都无法使其达到骁龙的水平。因此，Galaxy S21 Ultra 未能获得出色表现的全面推荐，因为你在该设备上的游戏表现在很大程度上取决于你从哪里购买该设备。考虑到手机维持了₹1,06,000/€1,249.的发行价，这是相当不可接受的

按照目前的情况，Exynos 2200 Galaxy S22 Ultra 完全不能作为日常驱动程序使用

目前，我唯一能说的是，如果你住在欧洲，就暂缓购买三星 Galaxy S22 Ultra。按照目前的情况，Exynos 2200 Galaxy S22 Ultra 完全不能用作日常驱动程序。令人难以置信的滞后*和*电池寿命也很糟糕。它没有任何改善，我不得不在一天中多次给我的手机充值。我发现很难推荐一款价格如此之高、性能如此之差的产品，如果我不强调我在零售部门面临的这些问题，我将成为一名评论者。只要其他原始设备制造商提供的顶级旗舰产品在你所在的地区一直表现得像顶级旗舰产品一样，就没有什么理由购买 Exynos Galaxy S22 系列，并抽奖看看你是否会获得一款表现像顶级旗舰产品的设备。一些 Exynos 用户得到了一个好的设备，一些没有——这是不可接受的。

最后，骁龙 Galaxy S22 Ultra 和 Exynos Galaxy S22 Ultra 在我看来是两种完全不同的智能手机。当你购买最新的三星 Galaxy S 系列智能手机时，你购买的是一部完全不同的智能手机，这取决于你所在的地区。在几乎任何其他智能手机系列中，在一个国家购买一款设备并不意味着它的性能会比在另一个国家购买的相同设备好得多，但这正是三星创造的二分法。