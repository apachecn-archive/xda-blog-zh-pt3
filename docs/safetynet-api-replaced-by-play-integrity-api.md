# 谷歌停止 SafetyNet API 以支持 Play Integrity API

> 原文：<https://www.xda-developers.com/safetynet-api-replaced-by-play-integrity-api/>

[SafetyNet](https://www.xda-developers.com/how-to-pass-safetynet-android/) 是一个可能 Android modding 社区的每个人都很熟悉的术语。解锁引导加载程序和[刷新自定义 ROM](https://www.xda-developers.com/how-to-install-custom-rom-android/) 后，如果你想使用银行应用和网飞等流媒体应用，通过安全网完整性测试至关重要。多年来，绕过安全网变得越来越难，尤其是在谷歌[开始实施硬件支持认证](https://www.xda-developers.com/safetynet-hardware-attestation-feature-here-to-stay/)之后。但是 API 现在正在消失，看起来社区将很快与一个新的恶魔战斗。

谷歌宣布计划逐步淘汰 SafetyNet，这是一种反滥用 API，允许应用程序检查 Android 设备的完整性。它将被新的 Play Integrity API 取代，谷歌称这是一种更先进和复杂的方法，可以保护应用程序和游戏免受篡改以及潜在的风险和欺诈性交互。它最初是在去年的谷歌游戏开发峰会上宣布的。

“随着我们进一步改进反滥用解决方案的产品组合，我们计划到 2024 年逐步淘汰 SafetyNet 认证 API。安全网 API 客户团队的一份官方声明中写道:“这种逐步弃用的做法应该会让您有时间迁移到新的 Play Integrity API，并避免业务中断。”。

到 2024 年，安全网证明 API 将被弃用。谷歌建议应用开发者尽快将 Play Integrity API 集成到他们的应用中。截至 2023 年 6 月 30 日，尚未迁移到新 API 的应用将不再能够使用 SafetyNet 认证。但是，如果您已经迁移，它仍将在您的应用程序的旧安装上工作。但从 2024 年 6 月开始，SafetyNet 认证 API 将不再适用于任何版本的应用程序。

谷歌表示，新的 Play Integrity API 几乎在所有方面都优于旧 API。它整合了多种完整性产品，包括安全网证明完整性裁决。迁移过程非常简单，因为这两个 API 在概念上是相似的。你可以点击查看迁移指南[。](https://developer.android.com/google/play/integrity/migrate)

Play Integrity API 对 Android modding 社区意味着什么，它将如何影响自定义 ROM 场景，还有待观察。然而，有一点是清楚的——用新的 API 绕过设备完整性测试肯定不容易。如果有什么不同的话，Play Integrity API 只是标志着一个新的猫捉老鼠游戏的开始。但是我们总是希望社区会再次找到一种方法来绕过它。

* * *

**来源** : [谷歌集团](https://groups.google.com/g/safetynet-api-clients/c/ac_AmiRCn0U/m/hFFBlOhdCQAJ)