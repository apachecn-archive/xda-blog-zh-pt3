# 如何通过 Android 上的指纹扫描仪远程解锁您的 Windows PC

> 原文：<https://www.xda-developers.com/unlock-windows-pc-fingerprint-scanner-android/>

除了简单的旧密码，你可以用各种方式保护你的电脑。[例如，Windows Hello](https://www.xda-developers.com/how-to-set-up-windows-hello/) 允许你用面部、虹膜或指纹登录。虽然微软的生物识别认证当然可以在兼容设备上工作，但它没有提供使用手机远程解锁 PC 的方法。

无线技术的普及和软件的相互依赖带来了创新，用户可以通过智能手机上的兼容功能解锁电脑。尽管个人电脑仍然没有广泛的生物识别认证——特别是在预算部分——但存在依赖于操作系统的功能，如[智能锁](https://support.google.com/chromebook/answer/9617782)，它允许你解锁你的 Android 手机以进入你的 Chromebook。但如果你不是 Chrome OS 用户，也没有兼容 Windows Hello 的 PC，该怎么办？还能用安卓手机的指纹扫描仪解锁运行 Windows 的 PC 吗？

是的，你可以。6 年前，我[用 Tasker，一个叫做 AutoTools 的 Tasker 插件，和一个叫做 Unified Remote 的应用程序，创建了一个脚本](https://www.xda-developers.com/unlock-windows-pc-using-fingerprint/)，用你 Android 设备上的指纹扫描仪远程解锁你的 Windows PC。该脚本使用自动工具来验证您的指纹，并使用 Unified Remote 来执行远程输入，如点击、滑动和粘贴来解锁您的 Windows PC。尽管如此，这绝对不是一个无缝的方式来远程解锁您的电脑。

如果 [Samsung Flow](https://www.xda-developers.com/new-samsung-flow-update-lets-you-unlock-any-windows-device-via-fingerprint-and-more/) 可以用来从三星 Galaxy 手机或平板电脑远程解锁你的 Windows PC，为什么其他任何第三方应用都不能？这正是 XDA 成员 Andrew-X 问自己的问题，经过几个月的工作，他想出了一个解决方案。他开发了一个名为“远程指纹解锁”的应用程序，可以让你通过 Android 智能手机上的指纹扫描仪解锁任何 Windows PC。

## 远程指纹解锁的工作原理

与其他硬件支持的无密码身份验证方法(如 USB 或 NFC 安全密钥)相比，远程指纹解锁采用了不同的方法。该实用程序有两个模块:一个用于 Windows 的库和一个 Android 应用程序，它们通过本地网络安全地相互通信。这意味着您可以使用 Android 设备上的指纹传感器在应用程序上进行身份验证，而 Windows 模块在验证后会无缝解锁您的 Windows 用户帐户。

在幕后，凭证使用基于您的指纹生成的密钥进行加密。由于 Android 的安全机制，密钥受到为手机供电的 SoC 的可信执行环境(TEE)的保护。该应用程序本身不存储任何密码，甚至不需要互联网许可就能运行。

## 远程指纹解锁功能

远程指纹解锁支持以下设备配置:

*   Windows 模块:
    *   x86 或 x64 架构
        *   注意，Arm 设备上的 Arm64 又名 [Windows 还不被支持。我们已经就这种不兼容性联系了开发者，我们会随时向你提供最新的信息。](https://www.xda-developers.com/best-windows-on-arm/)

    *   Windows Vista、Windows 7、Windows 8/8.1、Windows 10 或 Windows 11 电脑

*   Android 模块:

免费功能包括:

*   支持通过指纹扫描仪远程解锁本地和在线微软账户
*   设置 1 台电脑和 1 个帐户进行远程解锁
*   Wi-Fi 网络共享支持

专业功能(1.99 美元应用内购买)包括:

*   没有广告
*   添加多台 Windows 电脑
*   在每台 Windows PC 上添加多个帐户
*   支持局域网唤醒

## 如何设置远程指纹解锁

设置远程指纹解锁相当简单。你只需要下载 Android 应用程序，安装 Windows 指纹凭据模块，并在应用程序中完成设置过程。如前所述，该实用程序不需要互联网连接，但仍然需要本地网络。因此，你必须确保你的 Windows PC 和 Android 手机连接到同一个 Wi-Fi/接入点。

1.  从谷歌 Play 商店下载安装[远程指纹解锁](https://play.google.com/store/apps/details?id=ro.andreimircius.remotefingerauth)。
2.  为您的 Windows PC 下载并安装最新的 [Windows 指纹认证模块](https://drive.google.com/drive/folders/1bktvp0JcJKfE92efgxQlo06ARrMfLDFd)。请务必仔细阅读安装说明和警告。
3.  打开 Android 应用程序，进入扫描部分。
4.  启动扫描操作，让它找到您的 Windows PC。
5.  点击要设置的电脑。你可以选择给它一个名字和/或发送一个局域网唤醒数据包，如果你有专业版。
6.  添加电脑后，转到帐户部分。
7.  点击“添加账户”输入您想要远程解锁的帐户的用户名和密码。
8.  在 PC 上添加要解锁的帐户后，点击帐户名称，以便在名称后显示一个(选定的)(参见最后一个屏幕截图)。)如果您不这样做，您将会得到一条错误消息，类似于“没有选择默认帐户”

现在模块安装完毕，您可以尝试解锁电脑。

1.  锁定您的 Windows PC，您应该会看到一个名为“指纹解锁”的新用户如果它显示该模块处于活动状态，则您可以继续操作。
2.  打开手机上的远程指纹解锁，进入解锁部分，
3.  扫描你的指纹。
4.  如果你设置正确，你应该看到你的 Windows 电脑自动解锁！

如果你在设置时有任何问题，我们建议你看看下面的 XDA 论坛帖子。

[**查看我们论坛上的远程指纹解锁线程**](https://forum.xda-developers.com/android/apps-games/app-remote-fingerprint-unlock-unlock-t3841148)

## 使用安全吗？

我知道你们中的一些人可能对安装这样的 Windows 应用程序有所顾虑。虽然我不能保证这款应用使用起来是安全的，因为它不是开源的，但在通过各种恶意软件分析工具运行它并要求开发人员解决工具发现的问题后，我相信开发人员是值得信赖的。

为了清楚起见，我引用下面我们的对话，这样你可以自己决定:

我:

> 我用[病毒总量](https://www.virustotal.com/#/file/55b57cac70da55e7833ea920c0cbd149c20c9911dc2f0bdc75f46f468f93fbd3/detection)和[杂交分析](https://www.hybrid-analysis.com/sample/55b57cac70da55e7833ea920c0cbd149c20c9911dc2f0bdc75f46f468f93fbd3)进行了测试，他们得到了以下结果:
> 
> *   伊卡鲁斯选择了“PUA”。RV 平台"
> *   趋势科技将其提取为“可疑 _GEN.F47V0908”
> *   Filseclab 称之为“广告软件”。CsdiMonetize.AI.twym "

一周后，开发人员做了一些修改，并回复了我:

> 因此，我在一周前对安装文件做了一些更改，并设法将 VirusTotal 上的检测次数减少到只有 1/63，McAfee AV 的扫描仪是唯一一个将我的安装检测为广告软件的扫描仪。我已经给他们发了一封邮件报告错误检测，但我仍然没有收到回复。这就是我没有联系你的原因。
> 
> 令人惊讶的是，我再次扫描了最新的版本，它是干净的。他们可能更新了他们的扫描引擎，或者把我的设置加入了白名单，但是没有回复。不管怎样，我很高兴它终于不再被误报了。
> 
> 然而，x86 版本仍然被 Endgame 标记为恶意版本，如此处的[所示](https://www.virustotal.com/ro/file/fff7195ec68c39147b2b31355db2a7f153fd171001e669057699954fe8056863/analysis/1537785527/)，即使同一 AV 没有检测到 x64 版本为恶意版本。我看看能不能就此事联系他们。
> 
> 在混合分析中，Filseclab 将其检测为广告软件。很可能是因为我仍然包含了一个 Windows 更新，这是该应用程序在早于 10 的 Windows 版本上运行所必需的。对远程进程“C:\Windows\System32\wusa.exe”的写入指的是使用“wusa.exe”进程安装的前述更新，而“C:\ Windows \ System32 \ cscript . exe”指的是。为 LogonUI.exe 进程(应用程序运行的进程)创建 Windows 防火墙例外的 vbs 脚本。剧本取自[这里](https://www.codeofhonor.com/blog/installing-firewall-exception-rules)。

从他的 XDA 线程，他还分享了以下信息:

> 我花了大约 40%的开发时间让这个应用程序尽可能的安全。模块之间的通信使用 TLS (SSL)进行保护。这些帐户存储在您的计算机上，因为解锁时需要它们。但是，它们是使用基于您的指纹生成的密钥加密的。根据[这篇文章](https://doridori.github.io/android-security-the-forgetful-keystore/#sthash.Bozg9xC8.8xT4F9Pp.dpbs)，生成的密钥由一个可信的执行环境支持，这可以防止攻击者获得密钥，即使他已经破坏了内核。换句话说，只有手机上注册的指纹才能访问密钥。如果你卸载，重置你的应用程序，甚至改变你的一个注册指纹，存储帐户的文件将永远丢失，你需要重新配置你的帐户。
> 
> 最后，研究已经完成，以确保，即使是在本地，您的帐户是尽可能安全的。没有密码存储在应用程序中，一切都是在本地完成的(在应用程序和 Windows 模块之间)，我不以任何方式通过互联网发送或查看你在应用程序中键入的任何内容。

截至 2022 年 12 月，VirusTotal 下面列出的安全厂商没有一家标记远程指纹解锁的 Windows 模块([版本 1.3.0](https://www.virustotal.com/gui/file/455319d4f2ff154f2b25ad7763b5d823cca3610d947639591ed0c7bdb406a54f) 是本文撰写时的最新版本)。对于爱好者来说，该安装程序是基于 Inno 设置的，这意味着你可以使用 [innounp](https://github.com/WhatTheBlock/innounp) 或类似工具轻松地对其进行反编译，并先睹为快。

我个人认为开发商的解释已经足够了。令我惊讶的是，在开发者发布他的应用程序之前，我的 Tasker 脚本是通过 Android 上的指纹扫描仪解锁 Windows PCs 的最广泛的解决方案。回想起来，我的 Tasker 脚本真的很不优雅，但是没有人制作过可以做得更好的应用程序。当然，三星有自己的解决方案，但他们仅限于三星 Galaxy 设备。由于远程指纹解锁，我可以使用谷歌 Pixel 6a 上的指纹扫描仪远程解锁我的 Windows 11 桌面 PC。