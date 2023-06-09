# 最新的 Windows 11 更新将任务管理器添加到任务栏上下文菜单中

> 原文：<https://www.xda-developers.com/windows-11-build-22621755-task-manager-taskbar-menu/>

在过去的一周左右，微软已经发布了相当多的 Windows 更新，现在又有一个新的推出。该公司本月为 Windows 11 用户发布了可选更新，包括原始版本和 Windows 11 版本 22H2。这是继 Windows 11 版本 22H2 的首次“时刻”更新之后——你可以称之为功能下降，这是上周刚刚发布的[，具有文件资源管理器标签](https://www.xda-developers.com/windows-11-22h2-file-explorer-tabs-available/)等大功能。

这两个更新有很多共同之处，但主要的共享元素是在右键单击任务栏时出现的上下文菜单中添加了一个任务管理器按钮。这在上周发布给 Windows 内部人员的许多版本中都有，现在普通用户也可以使用。任务栏是 Windows 10 中访问上下文菜单最简单的方式，但 Windows 11 中删除了该选项，所以很高兴看到它回来。

除此之外，每个更新包都有不同的变化，尽管 Windows 11 版本 22H2 的用户可以获得大部分消息。那些用户可以安装标签为 [KB5018496](https://support.microsoft.com/en-us/topic/october-25-2022-kb5018496-os-build-22621-755-preview-64040bea-1e02-4b6d-bad1-b036200c2cb3) 的更新，可以在这里手动下载[。这使得内部版本号达到 22621.755。此次更新的亮点包括搜索体验和 Windows 备份设置的一些视觉变化。以下是较大变化的分类:](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5018496)

> *   ***新！*** 它增强了任务栏上的搜索视觉处理，提高可发现性。这最初只面向一小部分受众，在接下来的几个月里会有更广泛的部署。当我们收集反馈时，一些设备可能会注意到不同的视觉处理。要了解更多有关您可能会看到这些变化的原因，请参见[在任何地方搜索任何内容](https://support.microsoft.com/windows/search-for-anything-anywhere-b14cc5bf-c92a-1e73-ea18-2845891e6cc8)。
> *   ***新增！*** 使用您的 Microsoft 帐户(MSA)时，它增强了备份体验。一些设备可能会注意到这种增强的视觉处理。这最初只面向一小部分受众，在接下来的几个月里会有更广泛的部署。
> *   ***新增！*** 它在设置中增加了对微软账号体验的改进。例如，您可以管理您的 Microsoft OneDrive 订阅和相关存储警报。
> *   ***新！当你右击任务栏时，它将任务管理器添加到上下文菜单中。这项功能将在未来几周内推出。***
> *   它解决了在 IE 模式下影响 Microsoft Edge 的一个问题。弹出窗口和选项卡的标题是错误的。
> *   它解决了可能导致屏幕上出现垂直和水平线伪像的问题。
> *   它解决了中的一个问题，即当您使用 Microsoft Edge 时，凭据用户界面无法在 IE 模式下显示。
> *   它解决了当您使用 Xbox Game Bar 录制游戏时可能无法同步音频的问题。
> *   它解决了一个影响文件资源管理器的问题。当您浏览 Microsoft OneDrive 文件夹时，它不太可靠。
> *   它解决了一个影响开始菜单的问题。当您使用键盘命令将锁定的项目移动到列表末尾的文件夹时，它将停止工作。
> *   它将在 2022 年 10 月底停止约旦夏令时的开始。约旦时区将永久转换为 UTC + 3 时区。

如果您想全面了解发生的变化，可以在下面找到:

*   ***新增！*** 它在设置中增加了对微软账号体验的改进。例如，您可以管理您的 Microsoft OneDrive 订阅和相关存储警报。
*   ***新！*** 它在任务栏上增强搜索视觉处理，提高可发现性。这最初只面向一小部分受众，在接下来的几个月里会有更广泛的部署。当我们收集反馈时，一些设备可能会注意到不同的视觉处理。要了解为什么您可能会看到这些变化，请参见[在任何地方搜索任何内容](https://support.microsoft.com/windows/search-for-anything-anywhere-b14cc5bf-c92a-1e73-ea18-2845891e6cc8)。
*   ***新增！*** 使用您的 Microsoft 帐户(MSA)时，它可以增强备份体验。一些设备可能会注意到这种增强的视觉处理。这最初只面向一小部分受众，在接下来的几个月里会有更广泛的部署。
*   ***新增！当你右击任务栏时，它将任务管理器添加到上下文菜单中。这项功能将在未来几周内推出。***
*   它使 ms-appinstaller 统一资源标识符(URI)能够为 DesktopAppInstaller 工作。
*   它将在 2022 年 10 月底停止约旦夏令时的开始。约旦时区将永久转换为 UTC + 3 时区。
*   它解决了一个影响分布式组件对象模型(DCOM)身份验证强化的问题。它会自动提高从 DCOM 客户端到 RPC _ C _ AUTHN _ LEVEL _ PKT _ INTEGRITY 的所有非匿名激活请求的身份验证级别。如果身份验证级别低于数据包完整性，就会出现这种情况。
*   它解决了影响 Windows 搜索服务的一个问题。使用该服务时，索引进度很慢。
*   它解决了影响安全密钥和 Fast Identity Online 2.0 (FIDO2)身份认证的缓存凭据的问题。在加入混合域的设备上，系统会删除这些缓存的凭据。
*   它解决了一个可能影响某些类型的安全套接字层(SSL)和传输层安全性(TLS)连接的问题。这些连接可能会出现握手失败。对于开发人员来说，受影响的连接可能会在单个输入缓冲区内发送多个帧，然后是大小小于 5 个字节的部分帧。如果连接失败，您的应用程序将收到错误“SEC_E_ILLEGAL_MESSAGE”。
*   它解决了一个影响 Microsoft Azure Active Directory(AAD)应用程序代理连接器的问题。它不能代表用户检索 Kerberos 票证。错误消息是，“指定的句柄无效(0x80090301)。”
*   它解决了一个影响证书映射的问题。一旦失败，**lsass.exe**可能会停止在**schannel.dll**的工作。
*   它解决了在 IE 模式下影响 Microsoft Edge 的一个问题。弹出窗口和选项卡的标题是错误的。
*   它解决了一个影响 Microsoft Edge IE 模式的问题。它会阻止您打开网页。当您启用 Windows Defender 应用程序防护(WDAG)并且没有配置网络隔离策略时，会出现这种情况。
*   它解决了使用第三方工具自定义标题栏时影响标题栏的问题。标题栏没有呈现。此更新确保标题栏呈现；但是，我们不能保证所有的文本定制都像以前一样工作。
*   它解决了可能导致屏幕上出现垂直和水平线伪像的问题。
*   它解决了一个影响微软和第三方输入法编辑器(IME)的问题。当你关闭 IME 窗口时，它们停止工作。如果 IME 使用 Windows 文本服务框架(TSF) 1.0，就会出现这种情况。
*   它解决了当您使用 Xbox Game Bar 录制游戏时可能无法同步音频的问题。
*   它更新 DriverSiPolicy.p7b 文件中的 Windows 内核易受攻击的驱动程序阻止列表。这一更新还确保了 Windows 10 和 Windows 11 之间的阻止列表是相同的。更多信息见 [KB5020779](https://support.microsoft.com/en-us/topic/kb5020779-the-vulnerable-driver-blocklist-after-the-october-2022-preview-release-3fcbe13a-6013-4118-b584-fcfbc6a09936) 。
*   它扩展了原始设备制造商(OEM)对目标硬件配置的虚拟机管理程序保护代码完整性(HVCI)实施的控制。
*   它解决了一个影响文件资源管理器的问题。当您浏览 Microsoft OneDrive 文件夹时，它不太可靠。
*   它解决了一个影响按钮样式 BS_PUSHLIKE 的问题。具有这种样式的按钮在深色背景下很难识别。
*   它解决了中的一个问题，即当您使用 Microsoft Edge 时，凭据用户界面无法在 IE 模式下显示。
*   它解决了影响服务器管理器的一个问题。当几个磁盘具有相同的 UniqueId 时，它可能会重置错误的磁盘。更多信息，请参见 [KB5018898](https://support.microsoft.com/en-us/topic/kb5018898-server-manager-resets-the-wrong-disk-if-many-virtual-disks-have-the-same-uniqueid-5b4b7d32-e65f-469e-a266-e7dc4b22467f) 。
*   它解决了影响 CopyFile 功能的一个问题。当用无效的源文件调用它时，它返回 ERROR_INVALID_HANDLE 而不是 ERROR_FILE_NOT_FOUND。
*   它解决了一个影响开始菜单的问题。当您使用键盘命令将锁定的项目移动到列表末尾的文件夹时，它将停止工作。

至于 Windows 11 初始版本的用户，他们将获得标签为 [KB501848](https://support.microsoft.com/en-us/topic/october-25-2022-kb5018483-os-build-22000-1165-preview-8b337b02-4bde-4971-b205-ad828f953fff) 的更新，这将使他们获得 22000.1165 版本。这个更新可以在这里手动下载[，并且在任务栏的任务管理器选项中，唯一的其他主要增加是改进了 Windows 搜索的性能。以下是亮点:](https://www.catalog.update.microsoft.com/Search.aspx?q=KB5018483)

> *   ***新！它增加了对 Windows 搜索结果和性能的改进。***
> *   ***新增！当你右击任务栏时，它将任务管理器添加到上下文菜单中。这项功能将在未来几周内推出。***
> *   它解决了导致操作系统升级停止响应，然后失败的问题。
> *   它解决了影响您计划每两周运行一次的任务的问题。它改为每周运行。
> *   它解决了一个影响 Microsoft Direct3D 9 游戏的问题。如果硬件没有本机 Direct3D 9 驱动程序，图形硬件将停止工作。
> *   它解决了一个影响三个汉字字体的问题。当您将这些字符格式化为粗体时，宽度大小是错误的。
> *   它解决了在某些平台上使用微软 D3D9 的游戏中的图形问题。
> *   它解决了在 IE 模式下影响 Microsoft Edge 的一个问题。弹出窗口和选项卡的标题是错误的。
> *   它解决了图形编辑程序中影响套索工具的问题。
> *   它解决了一个影响双卡通话的问题。如果您在手机上选择**无 SIM 卡**并在手机上发起通话，则双卡功能将不起作用。
> *   它解决了中的一个问题，即当您使用 Microsoft Edge 时，凭据用户界面无法以 IE 模式显示。
> *   It stops the start of daylight saving time in Jordan at the end of October 2022\. The Jordan time zone will permanently shift to the UTC + 3 time zone

如果你想知道所有的细节，你可以阅读下面的完整更新日志:

*   ***新增！它增加了对 Windows 搜索结果和性能的改进。***
*   ***新！当你右击任务栏时，它将任务管理器添加到上下文菜单中。这项功能将在未来几周内推出。***
*   它解决了一个影响分布式组件对象模型(DCOM)身份验证强化的问题。它会自动提高从 DCOM 客户端到 RPC _ C _ AUTHN _ LEVEL _ PKT _ INTEGRITY 的所有非匿名激活请求的身份验证级别。如果身份验证级别低于数据包完整性，就会出现这种情况。
*   它解决了影响远程过程调用服务(**rpcss.exe**)的 DCOM 问题。如果指定了 RPC_C_AUTHN_LEVEL_NONE，它会将身份验证级别提升到 RPC _ C _ AUTHN _ LEVEL _ PKT _ INTEGRITY，而不是 RPC_C_AUTHN_LEVEL_CONNECT。
*   它解决了一个影响 Microsoft Azure Active Directory(AAD)应用程序代理连接器的问题。它不能代表用户检索 Kerberos 票证。错误消息是，“指定的句柄无效(0x80090301)。”
*   它解决了在具有特定处理器的设备上影响计划的本机映像生成器(【Ngen.exe】)任务的问题。
*   它解决了一个影响证书映射的问题。当它失败时，lsass.exe 的**可能会停止在 schannel.dll 的**工作。****
*   它解决了导致操作系统升级停止响应，然后失败的问题。
*   它解决了影响您计划每两周运行一次的任务的问题。它改为每周运行。
*   它解决了一个影响 Microsoft Direct3D 9 游戏的问题。如果硬件没有本机 Direct3D 9 驱动程序，图形硬件将停止工作。
*   它解决了一个影响三个汉字字体的问题。当您将这些字符格式化为粗体时，宽度大小是错误的。
*   它解决了在某些平台上使用微软 D3D9 的游戏中的图形问题。
*   它解决了在 IE 模式下影响 Microsoft Edge 的一个问题。弹出窗口和选项卡的标题是错误的。
*   它解决了一个影响 Microsoft Edge IE 模式的问题。它会阻止您打开网页。当您启用 Windows Defender 应用程序防护(WDAG)并且没有配置网络隔离策略时，会出现这种情况。
*   它解决了一个影响微软和第三方输入法编辑器(IME)问题。当你关闭 IME 窗口时，它们停止工作。如果 IME 使用 Windows 文本服务框架(TSF) 1.0，就会出现这种情况。
*   它解决了图形编辑程序中影响套索工具的问题。
*   它解决了影响通用打印机的一个问题。删除后，您不能重新安装它。
*   它解决了创建重复打印队列的问题。因此，原始打印队列停止工作。
*   它解决了影响某些驱动程序的问题。当您播放受硬件保护的数字版权管理(DRM)内容时，它们会消耗更多的电能。
*   它解决了在某些硬件上影响驱动程序安装的问题。您看不到安装进度的显示。
*   它解决了一个影响 Windows 11 SE 版中 Clipchamp 应用程序的问题。Clipchamp 不会跑。
*   它解决了一个影响。msi 文件。禁用脚本强制时，Windows Defender 应用程序控制(WDAC)将忽略它们。
*   它解决了一个影响远程桌面虚拟桌面基础架构(VDI)方案的问题。会话可能使用了错误的时区。
*   它解决了影响远程桌面(RD)会话主机上的文件资源管理器的问题。文件资源管理器停止工作。当非 Windows 客户端连接到 Windows 11 RD 会话主机，并且您启用了时区重定向策略时，会出现这种情况。
*   它解决了一个影响按钮样式 BS_PUSHLIKE 的问题。具有这种样式的按钮在深色背景下很难识别。
*   它解决了中的一个问题，即当您使用 Microsoft Edge 时，凭据用户界面无法以 IE 模式显示。
*   它解决了一个影响双卡通话的问题。如果您在手机上选择**无 SIM 卡**并在手机上发起呼叫，则双卡功能不起作用。
*   它解决了影响服务器管理器的一个问题。当几个磁盘具有相同的 UniqueId 时，它可能会重置错误的磁盘。更多信息见 [KB5018898](https://support.microsoft.com/en-us/topic/kb5018898-server-manager-resets-the-wrong-disk-if-many-virtual-disks-have-the-same-uniqueid-5b4b7d32-e65f-469e-a266-e7dc4b22467f) 。
*   它更新 DriverSiPolicy.p7b 文件中的 Windows 内核易受攻击的驱动程序阻止列表。这一更新还确保了 Windows 10 和 Windows 11 之间的阻止列表是相同的。更多信息见 [KB5020779](https://support.microsoft.com/en-us/topic/kb5020779-the-vulnerable-driver-blocklist-after-the-october-2022-preview-release-3fcbe13a-6013-4118-b584-fcfbc6a09936) 。
*   它使微软符合美国政府(USG)版本 6 修订版 1 ( [USGv6-r1](https://www.nist.gov/programs-projects/usgv6-program/usgv6-revision-1) )。
*   它将在 2022 年 10 月底停止约旦夏令时的开始。约旦时区将永久转换为 UTC + 3 时区。

像往常一样，这些更新是可选的，所以它们不会自动安装。然而，这些更改将与微软在此之前所做的任何其他更改一起，纳入 11 月 8 日的下一个周二补丁更新中。这种更新将是强制性的，所以每个人迟早都会得到这些变化。