# Windows 11 build 22621.457 发布了带有更多修复的预览版

> 原文：<https://www.xda-developers.com/windows-11-build-22621-457-release-preview-fixes/>

微软正在发布预览版频道中为运行 [Windows 11 版本 22H2](https://www.xda-developers.com/windows-11-22h2/) 的 Windows Insiders 发布新的累积更新，使内部版本号达到 22621.457。这次更新主要集中在修复广泛的问题，但也有一些更显着的改进。这些很大程度上基于 8 月初在测试频道发布的[版本 22621.450。](https://www.xda-developers.com/windows-11-build-22622-450-22621-450-fixes/)

在新功能中，可以在设置应用程序中查看系统资源的使用历史，如相机、麦克风、电话等。你可以在设置应用的**隐私&安全**部分找到这个，它可以让你看到过去七天有哪些应用访问了这些资源，所以你可以掌握你的隐私。其他改进包括更有效的 Windows Defender for Endpoint，它现在应该在拦截勒索软件攻击方面做得更好，以及对 SMB 压缩的改进，使文件无论大小都始终被压缩。

除此之外，在这个版本中主要是修复，这是可以预料的。上次我们听说，微软计划在 9 月 20 日发布 Windows 11 版本 22H2 [，所以在正式发布之前修复任何问题的时间已经不多了。您可以在下面找到完整的修复列表。](https://www.xda-developers.com/windows-11-22h2-september-20th-report/)

### Windows 11 内部版本 22621.457 中的修复

*   我们修复了导致 Windows 在一些没有触摸屏的设备上显示平板模式功能的问题。
*   我们修复了导致一些应用程序窗口在任务视图预览中有空白部分的问题。
*   我们修复了一些人从网络驱动器复制文件时出现的问题。错误代码是 0x80070026。
*   我们修复了可能导致本地安全机构服务器服务(LSASS)泄漏令牌的问题。此问题会影响已安装日期为 2022 年 6 月 14 日或更高版本的 Windows 更新的设备。当设备在作为网络服务运行的不可信计算基础(TCB) Windows 服务中为用户(S4U)执行特定形式的服务时，会出现此问题。
*   我们修复了一个在某些情况下会导致 **sihost** 的问题。 **exe** 使用大量的 CPU。
*   我们修复了当您使用 IE 模式时导致 Microsoft Edge 停止响应的问题。这个问题还会阻止您与对话框进行交互。40242609
*   我们修复了当您删除 App-V 注册表节点时导致 App-V 客户端服务泄漏内存的问题。
*   我们修复了一个问题，如果 URL 的长度超过 2084 个字符，您将无法打开该 URL。此更新支持最多 8192 个字符的 URL。
*   我们修复了阻止从 Microsoft 商店更新编解码器的问题。
*   我们修复了导致**server assigned configuration s**在一些完整配置场景中为空的问题。
*   我们修复了一个问题，这个问题有时会过早地中断快照辅助区域的大小调整操作。
*   我们修复了一个问题，该问题可能会导致在您重置设备后，Windows Hello for Business 证书的部署在某些情况下失败。
*   我们修复了一个问题，该问题阻止您在删除通用打印机后重新安装它们。
*   我们修复了一个问题，该问题阻止非 Windows 设备在连接到基于 Windows 的远程桌面并使用智能卡作为身份验证方法时进行身份验证。
*   我们修复了在访问**隐私** > **活动历史**页面**时导致设置应用在服务器域控制器(DC)上停止工作的问题。**
*   我们修复了影响使用只读域控制器(RODC)从本地域查找不存在的安全 ID (SID)的问题。查找意外返回 STATUS_TRUSTED_DOMAIN_FAILURE 错误，而不是 STATUS_NONE_MAPPED 或 STATUS_SOME_MAPPED 错误。
*   我们修复了阻止存储迁移服务(SMS)在具有许多共享的服务器上完成清单的问题。错误事件 2509 出现在 Microsoft-Windows-StorageMigrationService/Admin 通道中(ErrorId =-2146233088/error message = "无效的表 Id ")。
*   我们修复了影响“设置>系统>剪贴板”下的“跨设备同步”选项的问题。该选项将不会保持启用状态。

据报道，微软正计划在年底前发布 Windows 11 版本 22H2 的第一个“moment”更新，这似乎目前正在测试频道与 Windows 内部人士进行测试。如果你注册获得 Windows 11 build 22622，你已经可以拥有任务栏溢出这样的功能了。看起来像这样的小功能将在这些“时刻”更新中发布，这有点像 Android 世界中的像素功能下降。这应该能让我们坚持到下一个版本的 Windows，我们暂时称之为 [Windows 12](https://www.xda-developers.com/windows-12/) 。

* * *

来源:[微软](https://blogs.windows.com/windows-insider/2022/08/23/releasing-windows-11-build-22621-457-to-the-release-preview-channel/)