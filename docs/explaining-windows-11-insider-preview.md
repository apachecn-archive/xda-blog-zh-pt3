# 解释 Windows 11 betas 版的 Windows Insider 计划渠道

> 原文：<https://www.xda-developers.com/explaining-windows-11-insider-preview/>

微软在 2014 年 10 月 1 日推出了 Windows Insider 计划，此前一天它已经发布了 Windows 10。当时，Windows 10 Insider 预览版被称为 Windows 10 技术预览版。我们只有两个戒指——快和慢；发布预览是后来添加的，部分是作为 Windows Phone 用户获得 Windows 10 Mobile RTM 版本的一种方式，官方更新在几个月后推出。

Windows Insider 计划发生了很多变化。这并不奇怪，因为已经快八年了。环现在是通道，它们不再以与新发布的节奏相对应的方式命名。

现在 [Windows 11](https://www.xda-developers.com/windows-11/) 已经发布，新版本正在内部测试中，你可能是新用户。以下是 Windows Insider 计划在 2022 年如何运作的概述。

## Windows Insider 计划开发频道-获取 Windows 11 预发布版本

如果你在开发频道，你现在就可以测试 Windows 11 预发布版本。这些不依赖于特定的更新；他们的目的是测试新特性，这些新特性可能会也可能不会在产品中出现，并且没有特定的时间表。

Dev 通道过去被称为快速环。如果你想活在边缘，这就是你报名的原因。此外，你也放弃了对正在发生的事情进行抱怨的权利。记住，任何事情都可能发生。

通常，当 Windows 的一个版本处于测试中时，它来自 rs_prerelease 分支(“rs”代表 Redstone，它曾经是 Windows 10 各种版本的代号)。当你在开发频道时，你应该处于一种永久的预发布状态。即使微软有时会做奇怪的 A/B 测试，你也应该总是得到最新的可测试的东西。

### 神奇的窗户

在 Windows Insider 计划中，有一段时间被称为“魔法窗口”。这是如何工作的。当您在 Windows Update 中检查更新时，您的电脑几乎会将您的内部版本号发送到服务器，检查是否有更高内部版本号的更新可供您使用，如果有，则发送该更新。因此，从 Windows 11 Insider 预览版回滚的唯一方法是全新安装操作系统。

例如，Windows 11 版本 21H2 的内部版本是 22000。如果你在开发频道，你是在一个较新的版本上，所以没有办法不清理你的机器就简单地回滚。

Build 22000 是一扇神奇的窗户。如果你在 Dev 渠道测试 Windows 11，一旦有其他选择，比如在 Beta 渠道测试，你可以安全地取消注册你的机器。在这短暂的一段时间内，Insider 程序与 Windows 的发布版本保持一致，如果你愿意，你可以跳出预览版。

这与以前的工作方式略有不同。曾经有一段难得的时间，所有的频道都会排队。现在，您必须等待开发与测试版保持一致，切换，然后等待测试版与生产版保持一致。

即使是现在，开发频道也不同于 Windows 11 最初的测试。原来微软只是发布了 build 22000，剩下的都是累积更新。这使得知道 build 22000 是 RTM 变得很容易。现在，我们再次在 Dev 频道中测试 Windows 的完整版本，所以我们必须在下一个神奇窗口出现之前暂停一下。这应该发生在秋季功能更新之前的某个时间。

在此之前，自 2020 年春季以来就没有出现过魔法窗口，尽管在此之前，每年都会出现两次。在 1909 版中，微软采用了一种包含启用包的更新交付方法，而不是交付 Windows 的完整版本。Windows 10X 本应在明年秋季发布，因此 20H2 最终也成为了一个支持包。然后 Windows 10X 被推迟到春天，所以 21H1 也是一个启用包。

一直以来，Windows 内部人士都在测试 Windows 10 的完整版本。那些期待开发频道在 2020 年秋季与生产保持一致的人没有机会取消注册他们的 PC，直到 Windows 11 魔法窗口打开。这就是 Dev 频道的本质。假设微软宣称你在稳定性和可预测性方面所做的牺牲足够让你站在 A/B 测试的正确一边，你就可以在它们准备好测试的时候测试它们。

## Windows Insider 计划测试频道-下一个 Windows 11 功能更新，即将推出

Beta 通道目前正在测试 Windows 11 版本 22H2。与开发渠道不同，测试渠道与特定的功能更新相关联。虽然开发频道应该处于永久的预发布状态，但在某些时候，这些构建会分裂成一个发布分支，这就是 Beta 频道的最终结果。这就是过去被称为慢环的东西。

根据定义，测试频道比开发频道稳定得多。你实际上是在获得 RTM 版本，然后在向非内部人员发布之前，它会被维护几个月。你可以把测试频道看作是安全环，但是在那里你仍然可以测试新的东西。

现在 Windows 11 已经普遍上市，在某个时候，测试版渠道将开始测试将于明年秋天推出的功能版本。如果你不想那样，切换到发布预览频道。

## Windows Insider 计划发布预览频道-测试累积更新

发布预览频道诞生于 Windows 10 发布之后。虽然这不是唯一的目的，但当时的一件大事是 Windows Phone 和升级到 Windows 10 Mobile。当时，微软在 2015 年 11 月发布了搭载 Windows 10 Mobile 的新旗舰手机，但现有设备的 OTA 更新直到 2016 年 3 月才开始推出。

然而，明确的目的是测试即将向公众推出的更新。当某个东西出现在发布预览频道时，这意味着它应该完成了。它应该在黄金时间准备好。发布预览频道是最后一站。以前在发布预览版中也发现过 bug，但通常情况下，这就是发布的内容。

目前，Windows 11 build 22000.xxx 是发布预览版中的内容，这并不奇怪。如果你还在使用 Windows 10 并且不能升级，那里也有 21H2 版本。这种情况短期内不会改变。对于 Windows 11 用户来说，直到发布前几周，你才会在发布预览版中看到新的功能更新，最早也是 2022 年夏季*，因为它更有可能在秋季发布。*

 *## 结论-明智地选择你的戒指

注册 Windows Insider 计划是一个简单的过程。你只需要进入**设置- >更新&安全- > Windows Insider 程序- >开始使用。**系统会要求您链接您的 Microsoft 帐户，并选择您的铃声。

需要注意的关键是，你走得越高，就越难回头。正如我之前提到的，在 Windows 11 到来之前，自 2020 年初以来，开发频道没有机会在不进行工厂重置的情况下取消注册 PC。测试版渠道每六个月就有一次机会，但随着 Windows 11 发布节奏的不同，它每年都会有一次机会。

还有，做好一些不稳定的准备。你在测试，如果你在做这个，你知道你会让自己陷入什么。下周的建设可能没有本周稳定。事情就是这样，如果你不愿意，要么不要注册，要么注册一个较低的渠道。*