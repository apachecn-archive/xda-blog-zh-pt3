# 谷歌和三星联手简化 Android 健身应用程序之间的数据共享

> 原文：<https://www.xda-developers.com/google-samsung-health-connect-api/>

在 [Google I/O 2022](https://www.xda-developers.com/google-io-2022-recap-major-announcements/) 上，谷歌和三星宣布了 Health Connect，这是一个新的统一平台和 API，旨在简化健身和健康应用程序之间的互操作性。

新的 Health Connect APIs 将允许开发人员安全地访问不同健身应用程序、设备和可穿戴设备的数据，以构建更丰富的应用程序体验。它为应用程序开发人员提供了一个单一的界面来读取和写入用户的健康和健身数据。用户将能够控制哪些应用程序可以收集和共享数据，并能够随时关闭访问或删除数据。谷歌表示，所有数据都将被加密并存储在你的本地设备上。

Health Connect 支持几种常见的健康和健身数据类别，如活动、睡眠跟踪、身体测量、生命体征、心率和血压。在有多个健身应用程序提供相同数据的情况下，用户可以决定他们希望优先考虑哪个来源。对于消费者来说，这意味着如果你在 Fitbit 应用程序中保存你的健康数据，理论上，你也可以在三星健康应用程序中访问所有数据。

*健康连接如何运作*

*“在用户许可的情况下，开发人员可以使用标准化的模式和 API 行为，安全地从 Health Connect 读取数据和向其写入数据。用户将完全控制他们的隐私设置，通过精细控制来查看哪些应用程序在任何给定时间请求访问数据。谷歌产品经理克里斯·维尔克在一篇博客中写道:“健康连接中的数据都是在设备上加密的。”。*

这些新的 API 现在可以通过 Android Jetpack 提供给所有的应用开发者。三星 Health、Fitbit、谷歌 Fit、MyFitnessPal、Leap Fitness 和 Withings 将成为首批采用 Health Connect 的安卓应用。

如果你是一名 Android 应用开发者，想要利用新的 API，你可以在这里找到官方文档。有关更多详细信息，请查看下面链接的新 API 的 Google I/O 会话，它解释了开发人员如何利用 Health Connect API 来构建新的健身和健康体验。

Health Connect 应用程序目前在谷歌 Play 商店上提供早期访问，但请记住，合作伙伴的应用程序似乎还没有更新到支持它。然而，做好准备并没有错！

* * *

来源:[安卓开发者博客](https://android-developers.googleblog.com/2022/05/introducing-health-connect.html)