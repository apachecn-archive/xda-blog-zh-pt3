# 新的 Windows 11 开发版本删除了 WSL 并修复了许多问题

> 原文：<https://www.xda-developers.com/windows-11-dev-channel-25272/>

在假期休息了几周之后，微软又开始向内部人士发布 Windows 11 的新版本，那些在开发频道注册的人将获得版本 25272。这个新版本没有包括很多新功能，但它确实删除了微软[在最近版本](http://www.xda-developers.com/windows-11-build-25247-search-copied-text/)中添加的几个实验，此外还删除了预装的 Linux 版 Windows 子系统。除此之外，在这个版本中也有很多修正。

## 搜索建议操作和网站推荐没有了

事实上，这个版本中最大的变化之一是微软取消了过去几周一直在测试的两个功能。一个是建议动作，当用户复制一些文本时，提示用户开始网络搜索，这将搜索所选择的术语。

另一个被删除的功能是“开始”菜单中的网站推荐。这将在开始菜单中直接显示你所在地区的热门网站，使它们更容易访问，但这也意味着你的开始菜单被你可能不关心的内容填满了。微软没有说以后会恢复这些功能，这表明它收到了关于它们的负面反馈。

## WSL 现在可以通过微软商店下载

另一个乍一看似乎很大的变化是，微软正在从 Windows 11 安装中删除 Linux 的 Windows 子系统(WSL)。这并不是因为该特性不再受支持，事实上，情况恰恰相反。面向 Linux 的 Windows 子系统将于 2022 年底[在微软商店](https://www.xda-developers.com/run-gui-linux-apps-windows-10-wsl/)上市，这使得微软能够更快地向该平台提供更新。

以前，你的 WSL 版本与你的 Windows 版本捆绑在一起，而 Windows 本身大约一年才进行一次重大更新。通过将 WSL 与操作系统分离，微软可以更好地支持它。

如果你还没有从微软商店下载 WSL，你将需要这样做来继续在 Windows 中使用你的 Linux 发行版，但是微软说它希望这在未来自动完成，这样你就不会因为过渡而经历任何中断。

## 杂项更改和修复

除了这两个大的变化，这里没有什么太大的变化。微软已经将以前在“开始”菜单的 Windows 工具文件夹中找到的快速助手工具直接移到了应用程序列表中，这样更容易找到。微软还在 Windows 打印队列中添加了一个刷新按钮。

这个版本中也有很多修复，包括一个针对 Arm 设备的修复，当从睡眠中醒来时，这些设备可能会出现黑屏。下面是完整的修复列表。

**【常规】**

*   修复了一些 Arm64 设备在从睡眠或休眠状态恢复时出现黑屏的问题。
*   修正了一个问题，导致应用程序中的各种 UI 元素有时在最近的版本中消失和重新出现。

**【任务栏上的搜索】**

*这些修复只适用于 Windows 内部人员，他们收到了任务栏上搜索外观的不同处理方式之一，这些处理方式开始向内部人员推出* [*版本 25252:*](https://blogs.windows.com/windows-insider/2022/11/28/announcing-windows-11-insider-preview-build-25252/)

*   我们修复了导致任务栏上的搜索框无法正确呈现并显示视觉效果的问题。
*   日语 IME 候选项现在应该正确显示在任务栏的搜索框中。

**【任务管理器】**

*   修复了导致按发布者名称过滤在进程页面上不正确匹配的问题。
*   修复了应用过滤后导致某些服务不显示在服务页面中的问题。
*   修正了一个问题，导致新的进程出现在一个过滤列表中，如果启动，而一个过滤器被设置。
*   修正了一个问题，任务管理器不能正确显示亮暗内容，导致潜在的不可读文本。
*   修正了一个问题，导致任务管理器中的启动应用页面没有为一些内部人员列出任何应用。
*   如果没有匹配的搜索结果，任务管理器将明确指出。
*   修正了当试图结束某些进程时可能发生的任务管理器崩溃。
*   现在，您可以通过按 CTRL + F 将焦点设置到搜索框。

**【旁白】**

*   修复了在立陶宛语和匈牙利语版本中打开或关闭讲述人后导致设置崩溃的问题。
*   讲述人现在应该可以与 Windows Defender Application Guard for Edge 一起正常工作。

**【直播字幕】**

*   我们修复了在开发频道最新的内部预览版中导致直播字幕无法工作的问题。

**【输入】**

*   将日语 IME 与“讲述人”一起使用时，“讲述人”将不再在您每次按键时读出整个合成字符串。
*   如果只安装了一种输入语言，第一次使用 ALT + Shift 时显示的消息将不再显示。
*   修复了 Surface Pen 在最近的版本中无法继续播放 PowerPoint 幻灯片的问题。
*   进行了更改，以帮助提高游戏中使用高报告率鼠标时的性能。
*   修正了一个问题，如果你使用触摸手势打开开始菜单，它可能会中途卡住。
*   修复了在使用日文或中文 ime 时，可能导致 Excel 对某些鼠标拖动事件停止响应的问题。

**【设置】**

*   修正了一个问题，当你连接到 VPN 时，如果你取消了认证认证，可能会导致挂起。
*   修正了有时打开电源和电池时设置崩溃的问题。
*   修正了当导航到蓝牙部分时导致快速设置崩溃的问题。
*   修复了设置>应用程序>默认应用程序下的应用程序图标可能模糊的问题。

**【开窗】**

*   修正了在最近的版本中，当 ALT+tab 退出某些游戏时导致黑屏的问题。
*   在使用黑暗模式时，当您在文件资源管理器和某些其他应用程序中高亮显示最大化按钮时，它应该不再比关闭和最小化按钮略小。
*   修正了几个在最近版本中引入的 DWM 崩溃。

**【其他】**

*   修复了导致一些 Windows 安全应用崩溃的问题。
*   修复了打印队列显示打印机连接打印机的陈旧作业信息的问题。
*   修复了在浏览器中为网站创建 FIDO2 凭据时，在某些情况下可能会连续看到两次对话框的问题。
*   此版本包含对某些电脑上影响 Windows Hello 的问题的修复。我们正在继续调查特定于 Arm64 电脑的问题(参见已知问题)。
*   修复了一个问题，如果你在录制视频时按下暂停，可能会导致相机应用程序显示出错。

然而，这个版本仍然有一些已知的问题，Arm 设备还没有完全摆脱这些问题。使用 Windows Hello 面部识别登录可能无法在这些设备上运行，因此您必须输入您的 PIN。以下是微软分享的已知问题的完整列表:

**【任务栏&系统托盘】**

*   使用平板电脑优化的任务栏时，任务栏有时会被裁剪成两半。您也可能在辅助显示器上看到此问题。

**【任务栏搜索】**

*以下已知问题仅适用于 Windows 内部人员，他们收到了任务栏上搜索外观的不同处理方式之一，开始向内部人员推出* [*内部版本 25252*](https://blogs.windows.com/windows-insider/2022/11/28/announcing-windows-11-insider-preview-build-25252/) *:*

*   在从右向左显示的语言中，如阿拉伯语，任务栏上搜索框中的文本存在布局问题。

**【任务管理器】**

*   从任务管理器设置页面应用时，某些对话框可能无法以正确的主题呈现。
*   当在任务管理器设置页面中应用主题更改时，流程页面的数据内容区域可能会闪烁一次。

**【微件】**

*   我们正在调查一个问题，对于中国的内部人员(也可能是其他人)来说，widgets 板会卡在一个看不见的状态，导致屏幕左侧的点击不起作用。如果遇到这种情况，按 WIN + D 可能会解决问题。
*   在像阿拉伯语这样的从右向左显示的语言中，当点击窗口小部件板的扩展视图时，在窗口小部件板调整大小之前，内容在视图之外动画显示。

如果您注册了开发人员频道，新版本将很快自动下载，但如果您不想等待，可以立即进入 Windows Update 并检查更新。微软今天还发布了一个测试版频道，其中包括开始菜单中重新设计的搜索栏。

* * *

**来源:** [微软](https://blogs.windows.com/windows-insider/2023/01/05/announcing-windows-11-insider-preview-build-25272/)