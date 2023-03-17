# Windows 11 build 25174 新增游戏通行证小工具

> 原文：<https://www.xda-developers.com/windows-11-build-25174-adds-a-new-game-pass-widget/>

又到了周三，这意味着是时候向在 Dev 频道注册的内部人士推出新版本的 [Windows 11](https://www.xda-developers.com/windows-11/) 了。这一次，微软推出了 Windows 11 build 25174，最大的变化是为 Game Pass 提供了一个新的小工具。

事实上，这似乎是这个版本中唯一的新增加，但如果你经常在 Game Pass 上玩游戏，这很酷。这个小工具可以轮流显示最新加入服务的游戏、即将离开的游戏和突出显示类别中的游戏的信息。您可以将它添加到 Widgets 面板，就像处理任何其他小部件一样，以便快速访问这些信息。

在 widget 中，单击任何游戏都会将您带到完整的 Xbox 应用程序来安装它们、阅读评论等等。这实际上有点令人兴奋，因为到目前为止，大多数可用的小部件都将您链接到网络。这似乎是第一个真正链接到正确应用程序的应用程序，这为第三方应用程序最终也支持小工具提供了可能性。

微软表示，它计划增加对使用你的微软账户登录 Game Pass widget 的支持，这样你就可以看到你最近玩过的游戏和更适合你的信息。不过，就目前而言，对每个人来说，内容看起来都差不多。

除此之外，在这个版本中并没有太多新东西。对于已经拥有新的选项卡式文件资源管理器的用户来说，有一个小的变化，在窗口左侧的导航窗格中用鼠标中键单击一个文件夹将在一个新的选项卡中打开该文件夹。

当然，还有一些常见的修复和已知问题，这两者都相当昂贵。你可以在下面看看。

### Windows 11 内部版本 25174 中的修复

**【文件浏览器】**

*   修正了打开新的文件浏览器窗口时可能导致 explorer.exe 崩溃的问题。
*   修复了在使用黑暗模式时以特定方式(例如，从命令行)启动文件资源管理器时，在明亮模式下意外显示文件资源管理器主体的问题。
*   修正了一个问题，当你使用黑暗模式时，文件浏览器中的左/右箭头处于明亮模式，导致它们没有足够的对比度来显示它们何时被启用。
*   修正了一个问题，导航窗格中的分隔线有时会重叠/画得离文本太近。
*   修复了一个问题，如果你拖放一个文件夹到导航窗格中，有时会意外地将该文件夹放在列表的底部，而不是你拖放的位置。
*   修复了当使用 F11 将文件浏览器置于全屏模式时导致文件浏览器中 UI 问题的问题。

**【任务栏】**

*   修正了一个问题，导致各种系统托盘元素意外失踪的一些内部人员对以前的建设。

**【设置】**

*   修复了一些电脑在进入系统>存储>磁盘和卷时遇到的崩溃问题。

**【其他】**

*   修正了一个导致鼠标和键盘输入在最近两次飞行的某些游戏中不能正常工作的问题。
*   修复了一个问题，该问题被认为是导致 SQL Server Management Studio 无法为一些内部人员启动。
*   修复了一个问题，在 Windows 安全中的内存完整性可能会显示一个警告说，由于不兼容的驱动程序而无法启用，但不兼容的驱动程序列表将是空白的。
*   修正了一个问题，当在 Windows 安全中启用核心隔离时，导致一些应用程序在最后几个航班中意外无法启动。

### Windows 11 内部版本 25174 中的已知问题

**【通用】**

*   一些使用 Easy Anti-check 的游戏可能会崩溃或导致您的电脑进行错误检查。
*   **【新】**我们正在调查一些内部人士在升级到最后一趟航班后音频停止工作的报道。
*   **【NEW】**我们正在修复一个问题，该问题导致一些内部人员在最近的航班上玩某些游戏时由于使用了错误的显卡而导致 FPS 下降。
*   **【新】**我们正在调查一些不同应用在最近版本中开始崩溃的报告。

**【文件浏览器】**

*   文件浏览器标题栏的左半部分不能通过鼠标或触摸拖动。
*   文件资源管理器选项卡中的向上箭头没有对齐。这将在未来的更新中得到解决。
*   **【新功能】**我们正在修复一个问题，该问题会导致主页、文档、图片和其他潜在文件夹在文件资源管理器的导航窗格中意外重复或出现在桌面上。
*   **【新】**我们正在解决一个问题，即文件浏览器中的搜索框背景颜色可能与您当前模式的颜色相反。
*   **【新】**我们正在修复导致 delete 键在文件资源管理器中无法正常工作的问题。如果您遇到这种情况，您仍然可以使用上下文菜单来删除。

**【微件】**

*   任务栏上的通知徽章编号可能会出现错位。
*   在某些情况下，某些徽章的通知横幅不会出现在小部件板上。
*   我们正在修复一个导致小部件首选项(温度单位和固定小部件)意外重置为默认值的问题。

**【印刷】**

*   **【新】**我们正致力于解决在最后一次飞行中尝试从某些应用程序(如 Excel)打印时导致挂起和崩溃的问题。
*   **【新】**我们正在调查最近开发频道航班的报告，从某些应用程序打印表格时不包括这些行。

这里有一些大问题，比如音频和打印可能对一些人不起作用，所以像往常一样，如果你知道你要进入的是什么，最好只安装内部版本。

除了这个特定版本中包含的内容，微软最近推出了针对 Linux 的 Windows 子系统的更新- [版本 0.65.1](https://github.com/microsoft/WSL/releases/tag/0.65.1) -该更新可在 Insider 计划的所有渠道中获得。这更新了 Linux 内核和一些其他组件，尽管没有重大的特性变化。你可以在下面找到这些变化。

### WSL 0.65.1 中的新特性

*   改进了 localhost 中继，以获得更好的性能并准确报告绑定故障。
*   使用`/dev/ptp0`让游客与主人保持同步
*   如果无法获取发行版列表，请改进错误消息，并将其连接到`wsl.exe --list --online`
*   将 Linux 内核更新到 5.15.57.1
    *   修复自上一个 5.10 WSL2 内核以来的 9p 文件系统退化
    *   启用对精确时间协议(PTP)时钟设备的支持
    *   在 x86_64 版本中启用 Retbleed 缓解
    *   启用 nftables 和流量控制
    *   启用 VGEM 驱动程序
*   更新 Microsoft。WSLg 到版本 1.0.41
    *   WSLg:添加默认 x11 铃声
    *   WSLg: Update /etc/wsl.conf 将默认用户设置为 WSLg
    *   WSLGd:在 gdbserver 下添加启动 weston 的选项
    *   WSLGd:简化 weston 命令行构造
    *   合成器:添加 wslgd-notify
    *   合成器:停止陷印信号
    *   合成器:最后加载 xwayland 模块
    *   rdp:调整 MoveWindow/SnapArrange PDU 的边距调整大小
    *   rdpaudio:使用 pthread_cancel 而不是 pthread_kill
    *   xwayland:给 Xwayland 它自己的会话
    *   xwayland:不要为覆盖重定向窗口跟踪焦点

若要获取最新的 Windows 11 版本，你需要在设置应用中检查更新。Windows Subsystem for Linux 更新主要通过微软商店发布，如果你使用的是 Windows 11 中的版本，你必须在这里[下载商店版本](https://www.microsoft.com/store/productId/9P9TQF7MRM4R)才能获得这个新的更新。

* * *

来源:[微软](https://blogs.windows.com/windows-insider/2022/08/03/announcing-windows-11-insider-preview-build-25174/)