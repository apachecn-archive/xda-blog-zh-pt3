# Linux 和 Android 是手持游戏的未来

> 原文：<https://www.xda-developers.com/linux-android-handheld-gaming-future/>

像 Steam Deck、Ayaneo 2 甚至任天堂 Switch 这样的设备近年来风靡全球。便携式手持控制台开启了一个全新的体验世界。虽然任天堂多年来一直在制造手持设备，但前两者提供了移动 PC 游戏，具有良好的性能，出色的电池寿命，以及用该软件做更多事情的能力。

然而，Steam Deck 在一个大的方面比 Ayaneo 2 有优势:操作系统。在 steam OS(Arch Linux 的一个分支)上做你想做的事情要容易得多，更不用说减少的开销了。一方面，这降低了成本，因为不需要为其发行支付软件许可。然而，使用 Linux 也有缺点，例如需要[质子兼容层](https://www.xda-developers.com/how-proton-on-the-steam-deck-works/)来确保为 Windows 构建的游戏仍然可以玩。

然而，很明显，手持游戏的未来很可能是 Android 和 Linux 的结合，原因如下。

## Linux 是开放和免费的

就软件而言，对于任何一家打算开发新游戏机的公司来说，Linux 显然是一个有吸引力的选择。它不仅是一个开放和免费的内核，而且有大量的发行版可供公司继承和开发他们的系统。(参见 SteamOS，基于 Arch。)由于手持设备的目标是在充分利用有限硬件的同时尽可能降低成本，Linux 成为了一个更有吸引力的选择。

当然，最大的缺点是 Linux 基础可能要求操作系统是开源的。例如，您可以浏览 SteamOS 的代码，即使 Steam 客户端本身是专有的。像微软、索尼和任天堂这样的公司依靠反盗版和锁定系统来保护他们的游戏销售，开源操作系统可能会吓跑这些公司。

然而，像任天堂 ds 这样的掌上电脑表明，即使面对猖獗的盗版，游戏仍然可以卖得非常好，证明是有利可图的。在 PC 如此开放的情况下，破解游戏无处不在，但玩家还是会购买游戏。向这些公司证明这一点本身就是一项壮举，但这是可以做到的，而且 PC 市场证明，总的来说，人们会购买他们的游戏，而不是盗版。

## Android 游戏手持设备已经出现了

与此同时，运行 Android 的游戏手持设备已经有了先例。像罗技云和 T2 Razer Edge 这样的设备都是基于安卓系统的，而且已经有大量的游戏可以在这些系统上运行。不仅如此，智能手机 GPU 也相当强大。毕竟，任天堂 Switch 使用的是 Tegra X1，该 SoC 上的 Maxwell GPU(未对接时也以较低的时钟速度运行)长期以来一直被像[骁龙 8 代 2](https://www.xda-developers.com/qualcomm-snapdragon-8-gen-2/) 中的 Adreno 740 这样的 GPU 所超越。

这还没提到多年来人们是如何在安卓系统上模仿游戏的。手机游戏也越来越受欢迎，像 *Genshin Impact* 和 *Call of Duty Mobile* 这样的图形密集型游戏高居榜首。Android 已经是一个重要的游戏平台，利用这一优势的手持设备开始更频繁地发布。

当然，在视频游戏社区中，主要在移动设备上玩游戏仍然是一种耻辱，但这种看法正在开始转变，因为即使是最持怀疑态度的人也意识到了现代 Android 旗舰产品的真正力量。罗技云基本上是一款中端 Android 智能手机，但其云游戏功能是通过操作系统的开放性实现的。

## 甚至任天堂 Switch 也使用安卓系统

一个鲜为人知的事实是，即使是任天堂 Switch 也在一定程度上使用安卓系统。除了 Stagefright 多媒体框架之外，它在 *hosbinder* 服务中使用了一个名为“SurfaceFlinger”的显示管理器。这些都是经过修改后实现的，以适应任天堂 Switch 操作系统的代号 HorizonOS。这很可能是因为 Nvidia 已经做了关于制作图形显示管理器的调查工作，该图形显示管理器可以与 Android 设备中使用的 Tegra X1 芯片组一起工作。

有趣的是，几年前，现已去世的 Cyanogen 创始人兼首席执行官科特·麦克马斯特(Kirt McMaster)声称，任天堂希望与 Cyanogen 合作，为一款即将推出的设备(后来成为 Switch)创建一个操作系统。他告诉他们“坚持到底”，这就是为什么它从来没有实现。这并不奇怪，特别是考虑到开关的 Tegra 根。

如果 Android 的图形堆栈对于像任天堂 Switch 这样的手持设备来说足够好，那么它显然足够好，足以让公司考虑将其作为他们整体游戏的主要操作系统。是自 2017 年首次亮相以来最畅销的游戏设备之一。

*感谢 Skyline 团队的 Mark 对本文这一部分的帮助！*

## 未来游戏机和手持设备将使用 Android 和 Linux

我不确定它是否会是下一代，但我确信未来的游戏机和手持设备将会使用某种版本的 Android 或 Linux 系统。它节省了开发成本和时间，允许更小的公司测试这些游戏操作系统。

这并不是说，如果该系统配有 Android 或 Linux 发行版，公司将允许用户访问该系统。事实上，他们不太可能。比如 PlayStation 运行 Orbis OS，一个基于 FreeBSD 的操作系统。虽然如果你越狱的话，可以在上面运行 Linux，但是索尼已经锁定了它最新的游戏机。对于下一代手持设备，公司可能会使用高度锁定的 Android 和 Linux 版本，除了在设置中的许可披露中提到之外，可能无法识别。公司不太可能因为害怕盗版甚至网络游戏中的作弊而放弃对软件的控制。

然而，很明显，公司开始将 Android 和 Linux 纳入他们的游戏机软件路线图。任天堂已经考虑将其用于 Switch(甚至在一定程度上执行)，像 Valve with the Steam Deck 这样的公司已经证明它可以非常非常好地工作。对于游戏玩家来说，这是一个激动人心的时代，所使用的技术是其中的一个重要原因。