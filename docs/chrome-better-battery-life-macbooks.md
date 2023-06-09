# 谷歌 Chrome 的最新更新将提高你的 MacBook 的电池寿命

> 原文：<https://www.xda-developers.com/chrome-better-battery-life-macbooks/>

谷歌对 Chrome 网络浏览器做了一些细微的调整，这样你的 MacBook 的电池就可以持续更长时间。

由于 Chrome 对 iframes、JavaScript 计时器、数据结构和重绘的处理进行了一些非常具体的改变，现在你可以在 MacBook Pro 13 英寸(M2，2022 年)上浏览网页长达 17 小时，或者在一次充电后观看 YouTube 长达 18 小时。一些变化也将适用于旧款 MacBook 机型。

深入到细节，谷歌调整了最近在网页上生成的 iframes 在 Chrome 中创建和删除的方式，以帮助减少浏览器的短期内存使用。这并不影响你在大量使用媒体的网页上预期的长期内存使用。除了 JavaScript 计时器的一个方面——这是网页内存消耗的最重要的方面——谷歌减少了计时器唤醒 CPU 的次数，并取消了内部计时器。

至于网页中的数据结构，谷歌 Chrome 现在能够确定哪些是用同一键更频繁访问的，并设法优化浏览器访问它们的模式。你可以在下面的图片中找到它的代表。

谷歌对 Chrome 做的最后一项调整与重绘有关，即浏览器解析 HTML 代码。谷歌使用机器人导航网站，并确定某些文档对象模型的变化模式不会影响您在屏幕上看到的内容。谷歌随后调整了 Chrome，因此它可以削减不必要的重绘，并绕过某些步骤，以实现更好的功耗优化。

谷歌用 M2 芯片对相对标准的 MacBook Pro 2022 型号进行了测试。它配置了 8GB 内存，运行的是 macOS Ventura 13.2.1。测量是使用开源基准完成的，该基准可以在 Chrome 版本 10.0.5481.100 的不同浏览器上运行。

要获得最新版本的 Chrome，只需访问设置菜单，选择**帮助**，然后选择**关于谷歌 Chrome。**浏览器将下载更新并提示您重启。