# 谷歌 Pixel 6 和 Pixel 7 有一个私人计算核心；这是我们所知道的

> 原文：<https://www.xda-developers.com/private-compute-core/>

Android 12 带来了大量的新功能，其中最神秘的是私有计算核心(PCC)。它本质上是一个可以在设备上处理敏感数据的地方，远离其他一切正在发生的地方。它为谷歌 Pixel 6 提供了独有的功能，如现在播放、直播字幕和智能回复，但很长一段时间以来，没有太多关于它如何工作的信息。我们被迫猜测并试图自己找出答案。

[谷歌很久以前就说过](https://security.googleblog.com/2021/09/introducing-androids-private-compute.html)它将开放私人计算服务(PCS)的代码，这样独立的安全研究人员就可以对其进行审计。它[最终在 2022 年底发布了代码](https://github.com/google/private-compute-services)，同时发布的还有一份详细说明其工作原理的技术白皮书。据说，私有计算服务在 PCC 和云之间提供了一个隐私保护的桥梁，使通过安全路径提供新的人工智能模型和沙盒机器学习功能的其他更新成为可能。谷歌表示，功能和电脑之间的通信通过一套有目的的开源 API 进行，从数据中删除识别信息，并应用隐私技术，如[联合学习](https://www.xda-developers.com/google-federated-learning-hey-google-accuracy/)，联合分析和私人信息检索。

谷歌用它自己的话说:

> *【PCC】是 Android 操作系统内部的一个安全、隔离的数据处理环境，让您可以控制内部的数据，例如决定是否、如何以及何时与他人共享数据。通过这种方式，PCC 可以启用 Live Translate 等功能，而无需与包括谷歌在内的服务提供商共享连续的传感数据。PCC 是 Protected Computing 的一部分，Protected Computing 是一个技术工具包，它改变了数据处理的方式、时间和位置，以从技术上确保其隐私和安全。*

## 私有计算核心是一个虚拟沙箱

现在我们已经有了基本的东西，PCC 到底是什么？谷歌现在已经给出了其架构的一些技术细节，以及它如何存在于自己的隔离虚拟沙盒中。特性可以在沙箱中运行，处理操作系统级或环境数据，结果通过可信操作系统或访问控制的开源框架 API 显示给用户。

本质上，它是一个处理敏感信息的功能的沙箱。智能回复显然会扫描你的信息，而直播字幕会听任何正在播放的内容。现在玩也听身边的音频。这些功能都包含在 Android 系统智能中，它完全依赖 PC 来连接这个沙箱之外的设备。PCS 支持以下功能:

*   联合学习和联合分析
*   私人信息检索
*   HTTPS 仅下载传输

例如，在对话中键入内容时，谷歌解释说，Gboard 会要求智能回复根据屏幕上的对话提出建议。智能回复然后在 PCC 中安全、保密地处理对话。敏感数据不会与应用程序、键盘或谷歌共享，Gboard 得到的回应只是一个建议回复列表。

在计算核心内处理的任何东西也只能通过与 PC 交互来访问网络，PC 剥离识别信息并使用隐私技术，包括联合学习、联合分析和私人信息检索。这将互联网连接许可*从敏感功能*中抽象出来，并将只通过“非常狭窄的、有目的的 API”来做类似“下载模型、使用联合学习等等”的事情

但是，PCC 在 Android 智能手机上是否像谷歌解释的那样活跃呢？谁也说不准。我的直觉是，“开发预览版”是为非常具体的功能而存在的，仅此而已，因为它甚至在 Android 12 官方网站上[也宣传为活动的。如果这是它尚未开源的原因，这也是有意义的，因为它似乎只适用于一组专有的谷歌功能。Now Playing 可以绕过麦克风指示器，因为它通过计算核心运行，这一事实进一步支持了这一点。](https://www.android.com/android-12/)

在这个沙箱中存储和处理的数据不会暴露给其他应用程序，除非用户另有要求。例如，智能回复建议将一直隐藏在你的键盘和你正在输入的应用程序中，直到你点击它。个人电脑不仅在个人电脑和你的智能手机之间架起了一座桥梁，而且还通过新的基于人工智能的模型和变化来保持这些功能的更新。

## 智能回复、实时字幕和屏幕关注如何工作

谷歌在发布的技术白皮书中概述了 Android 系统智能的三个功能如何在 PCC 环境下工作。

### 智能回复

智能回复建议根据以前和当前的屏幕内容快速回复邮件。Android 系统智能从应用程序中提取相关实体，如地址、姓名和其他信息，然后将它们作为建议提供给用户。这些建议通过 PCC 得以实现。Google 采取以下步骤来安全可靠地实现该功能。

*   使用内容捕获 API 作为数据源，这是一个具有访问限制的 Android 框架 API。
*   用户和应用程序开发人员可以选择退出智能回复。
*   设备管理员可以通过使用禁用屏幕捕获的策略来禁用此功能。
*   用户可以明确允许数据离开 PCC。
    *   渲染时没有数据离开 PCC 边界，因为它通过特定的 Android 框架 API 使用委托 UI。
    *   由于键盘能够获取显示的候选答案数量，因此在一系列击键后，按输入筛选候选答案将被禁用。
    *   数据在 PCC 中保存时间很短，这意味着建议是基于最近观察到的数据
    *   只有通过系统中的允许列表，才能从 PCC 理解如何读取的应用程序中获取数据

*   使用 PCS APIs 进行网络访问
    *   ML 模型是非用户特定的
    *   分析是通过具有安全聚合的联合分析来执行的

### 实时字幕

实时字幕为智能手机上当前播放的任何内容提供字幕，处理所有音频并在 AOSP 渲染的用户界面中显示文字记录。应用程序无法访问这些数据。Google 采取以下步骤来安全可靠地实现该功能。

*   使用 Android Audio APIs 作为数据源，这是一个具有访问限制的 Android 框架 API。
*   该功能必须由用户启用，默认情况下不启用。
*   数据不会离开 PCC，只会呈现在系统图面中
    *   它使用窗口管理器 API 绘制的覆盖图来显示
    *   数据会在 PCC 中保留一小段时间

*   使用 PCS APIs 进行网络访问
    *   模型更新不是特定于用户的

### 屏幕注意

当用户看着他们的电话时，如果他们在屏幕变暗的预定时间看着它，屏幕注意力保持显示活动。如果检测到人脸，则推迟调光。Google 采取以下步骤来安全地实现该功能。

*   使用 Android Audio APIs 作为数据源，这是一个具有访问限制的 Android 框架 API
*   此功能必须由用户启用，默认情况下不启用
*   数据不会离开 PCC，仅在 PCC 和操作系统中通过 AttentionManagerService 框架 API 进行处理。数据只保留很短的一段时间
*   不使用任何网络功能。模型只能通过 APK 更新

## 私有计算核心是像素独占的吗？

这就是事情变得非常复杂的地方。

PCC 从未被明确地宣传为像素专有的功能。它在 Android 官方网站上，谷歌在 Android 的背景下谈论 PCC 而不是在像素的背景下。话虽如此，从技术上讲，莫奈在某一点上是像素专属的。唯一不同的是，谷歌表示，在未来发布的 Android 中，monet 将被推送到 AOSP [，现在原始设备制造商可以自己实现它。然而，关于 PCC 的措辞是模糊的，并模糊地提到了“Android 系统智能提供的功能，这些功能在 Pixel 和其他潜在的 Android 12 设备中实现。”](https://www.xda-developers.com/android-12-1-monet-open-source/)

从我收集的信息来看，至少 Android 系统智能在其他设备上也在使用。我的三星 Galaxy S22 Ultra 安装了 Android 系统智能，但它是否通过私人计算核心实现了谷歌所说的那些功能还不清楚。

## 私有计算核心对企业用户来说很有意义

我们希望谷歌能更容易地提供与 PCC 相关的信息，以及它如何保护用户隐私，特别是它与其他设备的关系。PCC 是像素独占的吗？其他主机厂能实现吗？目前还不好说，尽管背后的想法是好的。它也可以成为保护智能手机用户的有用资产，特别是那些可能将设备用于企业，但受到“现在播放”和智能回复等更具“侵入性”功能干扰的用户。

要考虑的另一个方面是，随着时间的推移，是否会引入新的功能。虽然他们显然可以，但它看起来不像(从白皮书，无论如何)任何新的东西真的来了一年的 PCC。虽然如果不需要的话，并不是所有的东西都需要通过它，但用户显然更喜欢在可能的情况下保护他们的数据。