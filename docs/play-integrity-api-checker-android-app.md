# 这个应用程序可以让你使用 Play Integrity API 检查你的 Android 设备的未修改状态

> 原文：<https://www.xda-developers.com/play-integrity-api-checker-android-app/>

作为一名 Android 应用程序开发人员，有许多原因可以让您利用滥用检测机制来检查目标设备的软件和硬件环境。谷歌的 SafetyNet 认证 API 就是这样一种反滥用 API，它允许应用程序开发人员评估他们的应用程序运行在 Android 设备上。然而，[到 2024](https://www.xda-developers.com/safetynet-api-replaced-by-play-integrity-api/) 它将被弃用，取而代之的是 Play Integrity API。自然，modding 社区将很快需要一种实用且易于使用的方法来查询 Google Play 服务的设备完整性属性。这就是 **Play Integrity API 检查器**的用武之地。

Play Integrity API Checker 由 Nikolas Spiridakis(又名 XDA 资深会员 [1nikolas](https://forum.xda-developers.com/m/1nikolas.6853617/) )创建，是一款漂亮的应用程序，用于确定 Google Play 服务报告的设备完整性状态。安装后，你需要做的就是点击**检查**按钮，应用程序会做剩下的事情。开发者接受了 KISS 原则(“保持简单愚蠢”)，这从 UI 设计语言中显而易见。

幸运的是，SafetyNet 证明 API 和 Play Integrity API 之间的设备完整性判定映射相当简单。一言以蔽之，后者的“MEETS_BASIC_INTEGRITY”属性相当于 SafetyNet 的“basicIntegrity”属性。在基础评估下添加“ctsProfileMatch ”,您将在新的 API 中获得“MEETS_DEVICE_INTEGRITY”的等价物。最后，要在“MEETS_STRONG_INTEGRITY”属性旁获得绿色勾号，设备必须满足硬件支持的安全网认证。

值得注意的是，许多偏离股票配置的事件可能会导致游戏完整性违规。在现代 Android 设备上，一个解锁的引导加载程序足以触发滥用检测系统。请记住，该应用程序不会帮助您修改设备的播放完整性状态，它只是从 Google Play 服务的角度反映状态。然而，高级用户仍然可以使用各种变通办法来通过谷歌的安全网认证和类似的反滥用检查，而不会破坏系统的任何部分。

如果你想试试 Play Integrity API Checker，可以从下面的 Google Play 链接下载这个应用。对于任何阅读这篇文章的应用程序开发人员来说，这个应用程序是[开源的](https://github.com/1nikolas/play-integrity-checker-app)，所以你可以看看代码库，提交新的补丁，或者自己编译应用程序。

* * *

【时间来源: [XDA 论坛](https://forum.xda-developers.com/posts/87226157)

**Via:**[mishal Rahman](https://twitter.com/mishaalrahman/status/1554170210097057792)