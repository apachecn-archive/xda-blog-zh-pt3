# 新的 Windows 11 预览版使得从通知中复制 2FA 代码更加容易

> 原文：<https://www.xda-developers.com/windows-11-dev-25295-2fa-notifications/>

微软刚刚在 Dev 频道向内部人士发布了 Windows 11 的每周版本[,这一次，我们将获得版本 25295。该版本包括一些较小的更改，但最值得注意的可能是能够轻松地从通知中复制双因素身份验证代码。](https://www.xda-developers.com/windows-11/)

事实上，如今许多服务都要求或至少允许双重认证，这意味着你必须通过电子邮件、短信或认证应用程序获得安全代码。现在，当这些通知包含这些代码时，例如 Steam 登录电子邮件，会有一个按钮将代码复制到您的剪贴板，以便您可以在相应的应用程序或网站中输入代码。不仅如此，如果你正在使用 Phone Link 应用程序，这还可以处理来自你手机的通知。当然，它可能不是完美的，但微软建议，如果您注意到某个特定的通知没有检测到安全代码，请发送反馈。

除此之外，没有一吨是新的。微软已经完成了任务栏搜索栏的最新设计，这意味着开发者频道的每个人现在都应该可以看到它了。

一个有趣的补充是针对商业/企业用户的新策略。该策略允许 IT 管理员在默认情况下启用通过维护更新(不是主要年度更新)提供的功能。目前，在 Dev 频道中还没有默认禁用的特性，但是这个策略将很快在 Beta 频道中推出，在那里它将更加有用。

除了这些变化，这个版本中所有的新东西都是错误修复，尽管它们总是受欢迎的。这包括一个内部人员在以前的版本中可能会遇到的一些错误检查错误的 fox，以及一个安装新版本的意外长时间的 fox。以下是完整列表:

**【通用】**

*   升级到 Build 25284+后导致一些内部人员重复错误检查的问题现在应该被修复了。
*   对导致内部人员在最近的航班中经历冻结的问题进行了另一次修复(特别是在这种情况下，如果你试图在玩游戏的同时使用应用程序，应用程序可能会冻结)。
*   修复了安装 Build 25290 后，设置> Windows Update >更新历史下的更新历史页面对某些用户为空白的问题。
*   修复了一个问题，一些用户在安装最近的版本时经历了比预期更长的更新时间。如果您再次遇到此问题，请在反馈中心提交带有日志的新反馈项目。

**【文件浏览器】**

*   修复了一个问题，如果文件资源管理器最大化，并且您使用阿拉伯语或希伯来语显示语言，添加和关闭选项卡按钮在文件资源管理器中不起作用。

**【输入】**

*   修复了使用多指屏幕触摸手势后可能导致应用程序窗口无响应的问题。
*   修正了一个潜在的问题，当共享你的屏幕时，导致你的鼠标看起来像是启用了指针轨迹。

**【设置】**

*   “添加设备”对话框应该不再有意外的大边框。

**【开窗】**

*   修正了一个问题，当你在屏幕上拖动它时，可能会导致某些应用程序移动非常缓慢。
*   修正了最近飞行中的 DWM 崩溃，这可能会导致你的屏幕黑屏。
*   修复了一个问题，即如果您断开并重新连接显示器，捕捉的窗口可能不记得它们的位置。

**【其他】**

*   修正了一个影响应用程序使用[图形能力的潜在崩溃。捕获](https://learn.microsoft.com/uwp/api/windows.graphics.capture?view=winrt-22621)在最近的航班上进行截屏。
*   修正了一个潜在的问题，当在最近的航班中试图打印到 pdf 时，会导致某些应用程序崩溃。

当然，还有一些常见的已知问题，现在这个列表已经相当广泛了。Arm 设备上 Windows Hello 面部识别的一个长期问题尚未解决，而且还有几个新问题。您可以在下面阅读更多信息:

**【通用】**

*   **【新】**一些 AAD (Azure Active Directory joined)用户在更新最新版本后登录 Windows 时，现在会看到“为您做好准备”屏幕。我们正在调查这个问题。
*   **【新增】**一些用户在向需要 windows 集成身份验证的企业网站进行身份验证时遇到问题。这将在未来的更新中解决。
*   启动组策略编辑器可能会显示找不到 displayName 属性的错误。
*   使用 Windows Hello 通过面部识别登录可能无法在 Arm64 PCs 上运行。解决这一问题的方法是使用 Hello PIN 路径。
*   我们正在修复与 combase.dll 相关的一个潜在问题，该问题导致多个使用 GetKnownFolder APIs 的应用在升级到 Build 25290 后崩溃，包括 IME 用户的记事本和 Windows 终端。
*   使用 Windows Recovery Environment(WinRE)或全新安装 Build 25290 时，用户可能会遇到呈现问题，从而给使用这些进程带来困难。如果您需要对您的设备进行全新安装，请从[https://aka.ms/wipISO](https://aka.ms/wipISO)获取最新的开发频道 ISO。

**【微件】**

*   窗口小部件选择器中的“查找更多窗口小部件”链接目前已断开。这将在未来的更新中修复并链接到商店收藏[这里](ms-windows-store://collection/?collectionid=MerchandiserContent/Apps/WidgetCollection/Widgetsforeverything)。
*   第三方微件可能偶尔会从微件面板中消失。可以通过单击刷新或从小部件选择器中重新锁定来重新添加它们。
*   当 Microsoft 帐户用于登录多个 Windows 11 设备时，第三方小工具可能偶尔会被取消锁定。
*   小部件固定/取消固定 toast 通知上的撤销按钮有时不起作用。

**【任务栏&系统托盘】**

*   对于一些拥有多台显示器的内部人员，任务栏上的应用程序图标可能会出现在错误的显示器上。

**【任务栏上的搜索】**

*   有一个问题是，在某些情况下，您将无法通过任务栏设置将任务栏搜索框更改为仅显示图标。要解决此问题，首先更改为不同的选项，然后，您应该可以选择仅显示为图标。

**【Windows 聚光灯】**

*以下已知问题仅适用于 Windows 内部人员，他们接受了 Windows Spotlight 的不同待遇之一，该待遇开始向内部人员推出*[*Build 25281*](https://blogs.windows.com/windows-insider/2023/01/19/announcing-windows-11-insider-preview-build-25281/)*:*

*   点击辅助显示器并不能消除全屏体验。
*   Spotlight 壁纸在多/混合分辨率显示器上没有显示正确的分辨率。

和往常一样，如果你注册了开发者频道，Windows 11 build 25295 可以通过 Windows Update 下载。如果没有，你可能想检查一下预览版中所有可用的 [Windows 11 功能，看看是否值得冒安装不稳定软件的风险。](https://www.xda-developers.com/windows-11-features-in-preview/)

* * *

**来源:** [微软](https://blogs.windows.com/windows-insider/2023/02/09/announcing-windows-11-insider-preview-build-25295/)