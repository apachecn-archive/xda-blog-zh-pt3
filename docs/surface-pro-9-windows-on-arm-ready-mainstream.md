# Surface Pro 9 表明 Arm 上的 Windows 终于准备好了

> 原文：<https://www.xda-developers.com/surface-pro-9-windows-on-arm-ready-mainstream/>

Surface Pro 9 可能就在上周发布，但它已经把我带回了微软的过去。2012 年，微软发布了 Surface RT，这是一款新奇的[二合一平板电脑](https://www.xda-developers.com/best-windows-tablets/)，它彻底改变了我们对笔记本电脑的看法。但有一样东西微软也包括在内，它最终成为了该设备失败的主要原因:Windows。

正如微软经常发生的事情一样，几年后的 2019 年，随着 [Surface Pro X](https://www.xda-developers.com/surface-pro-x/) ，这种情况再次发生。它对 Surface Pro 进行了大胆的重新设计，Surface Pro 主要采用了冲洗重复设计，但 Windows 10 显然不适合平板电脑。

你看，Surface RT 是由一个锁定的 Arm 专用版本的 Windows 8 驱动的，称为 Windows RT，它有一个非常糟糕的应用程序商店，不能运行经典的 Win32 应用程序。Surface Pro X 虽然可以在 Windows 10 中运行特定的 Win32 应用程序，但也遇到了性能问题，原因是像我这样的爱好者所熟知的“Arm 上的 Windows”

然而，Surface Pro 9 首次将基于 Arm 的芯片引入微软的主要 PC 之一，而不是像 Surface Pro X 那样的突破性产品。通过它，微软展示了它从 Windows 和 Surface 的过去中吸取的经验，并最终使 Arm 上的 Windows 为主流做好了准备。

## 关于应用程序仿真

Surface RT 失败的主要原因是它无法运行经典的 Win32 Windows 应用程序和网络浏览器，如 Mozilla Firefox。几年后，微软试图通过仿真来确保 Surface Pro X 与更小的 Win32 应用程序库兼容，从而修复这些错误。

在 Surface Pro X 上，许多不是由开发人员编码为 Arm 架构上的 Windows 原生的应用程序都在 32 位仿真下运行。尽管听起来不错，但模拟性能仍低于预期。这是因为，当时，许多开发人员已经将他们的应用程序推至 64 位格式，这与 Arm 上的 Windows 仿真层不兼容。

将一个强大的基于 Arm 的芯片放在 Surface Pro 9 上与英特尔对抗，表明 Arm 上的 Windows 已经准备好了。

只要问问所有尝试运行谷歌 Chrome 的技术评测人员，就会发现它要么崩溃，要么无法正常运行。见鬼，连我都对 Surface Pro X 不屑一顾，认为它是“我试图去爱，但最终却讨厌的 Surface。”

在 2022 年，这种情况已经改变了。多亏了 Surface Pro 9 上的 Windows 11，你现在可以在 Arm 上的 Windows 上运行 64 位应用程序，没有任何问题。就像 32 位应用程序仿真是如何内置到 Arm 上的 Windows 10 中一样，Windows 11 现在包括基于 Arm 的系统上的 64 位应用程序仿真。是的，即使有了这一层仿真，一些应用和游戏仍然无法正常工作，但这仍然[释放了更好性能的好处](https://blogs.windows.com/windows-insider/2020/12/10/introducing-x64-emulation-in-preview-for-windows-10-on-arm-pcs-to-the-windows-insider-program/)，以便应用可以在 Arm 系统的 Windows 上占用更多内存。

说到性能。最后要提的一点把我带到了 Surface Pro 9 内部芯片的强大之处。我还没有试过，但我知道它是基于 [ThinkPad X13s 内部的新高通骁龙 8cX Gen 3。](https://www.xda-developers.com/lenovo-thinkpad-x13s-review/#LenovoThinkPadX13sPerformance)上一代高通骁龙 8cX 芯片在性能方面表现平平。在 8cX 代之间，您将获得 85%的 CPU 性能和 60%的 GPU 性能。

这远不如苹果公司用 MacBook M1 做的好，但这是一个巨大的进步。我发现它的性能甚至和旧的第十代英特尔酷睿 i5 CPU 一样好。将这款强大的基于 Arm 的芯片放在 Surface Pro 9 上，与英特尔对抗，表明 Arm 上的 Windows 已经准备好了。微软希望你尝试它，并享受它。我希望它能帮助 Surface Pro 9 最终成为该公司有史以来[最好的 Surface 设备](https://www.xda-developers.com/best-microsoft-surface-pcs/)之一。

## 微软表示关心 Arm 上的 Windows

Surface Pro X 发布的时候，对微软来说是一个奇怪的时间。Windows 团队和 Surface 团队是分开的。2022 年，帕诺斯·帕奈现在两者兼而有之。他一直在为 Windows 和硬件推出优秀的软件，这体现在微软在过去几个月采取的一些不同举措中。这也是 Surface Pro 9 显示 Arm 上的 Windows 已经就绪的另一个原因。

如果 Volterra 项目没有表明 Arm 上的 Windows 是认真的，那么我不知道还有什么会认真。

你看，与 Surface Pro X 出现时不同，微软向开发者表明，它终于认真对待 Arm 上的 Windows 了。开发人员用来编写应用程序的 Visual Studio 现在针对 Windows 11 进行了原生编码，没有模拟功能。微软 Edge 浏览器在没有仿真的情况下工作，甚至 Surface Pro 9 上的相机应用程序现在也针对 Arm 进行了优化，具有强大的 Windows Studio 视觉效果，可以模糊你的背景。微软团队等其他应用也进行了优化。

综上所述，人们每天在 Surface Pro 9 上使用的基本应用程序都经过了优化，可以在 Arm 上运行 Windows。

微软甚至正在开发 Volterra 项目，这是一款基于 Arm 的迷你电脑，只供开发人员用来编写应用程序。如果这不能说明 Windows on Arm 是认真的，那么我不知道还有什么能说明这一点。像 Photoshop 这样的外围应用在 Arm 上的 Windows 上可能不是最好的，但对于生产力来说，Arm 上的 Windows 已经准备好了。微软已经尽了自己的一份力量，现在就看开发者如何跳上这个平台了。

## 结束语:微软正在倾听&未来是光明的

最后，我想提一件过去很多人抱怨过的事情。当谈到 Arm 上的 Windows 时，微软显然正在听取反馈。这不再仅仅是一件事后想起的事情。微软希望 Arm 上的 Windows 能满足你的需求。它只需要正确的旗舰软件。

最好的展示是什么？这是最近到来的一款 [Arm 原生 Xbox 应用](https://www.xda-developers.com/xbox-app-windows-cloud-gaming-arm-devices/)。对于那些想在 Arm 上玩 Windows 游戏的人来说，这是缺失的部分之一，它终于来了。同样，微软可能需要一段时间才能做到这一点，但现在已经做到了。如果这个问题得到了解决，我相信 Windows 内部人士抱怨的其他问题也会得到解决。我相信微软，从现在开始事情只会变得更好。

 <picture>![The Surface Pro 9 is a top-tier Windows tablet with Intel or Qualcomm processors, and it comes in multiple colors for the first time ever.](img/c897b1dbaad1bda308e45baff9efe412.png)</picture> 

Surface Pro 9 (Wi-Fi Model)

##### Surface Pro 9 (Wi-Fi 机型)

Surface Pro 9 是一款采用英特尔或高通处理器的顶级 Windows 平板电脑，它首次拥有多种颜色。

 <picture>![The Surface Pro 9 with 5G is powered by the new Microsoft SQ3 chipset and it has a 120Hz display.](img/e30e5e5992565041d1922a71a246db88.png)</picture> 

Surface Pro 9 5G

##### Surface Pro 9 5G

5G 版 Surface Pro 9 由新的微软 SQ3 芯片组提供支持，并具有 120Hz 的显示屏。