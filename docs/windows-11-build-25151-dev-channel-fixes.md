# Windows 11 build 25151 在开发频道推出，并进行修复

> 原文：<https://www.xda-developers.com/windows-11-build-25151-dev-channel-fixes/>

# Windows 11 build 25151 在开发频道推出，并进行修复

微软正在开发频道推出 Windows 11 build 25151，但它完全专注于修复。现在就可以抓取更新了。

微软再次向 Dev 频道的内部人员推出了 Windows 11 的新版本[,这次是版本 25151。与 Dev 频道中之前的版本一样，这是即将到来的](https://www.xda-developers.com/windows-11/)[版本 22H2 更新](https://www.xda-developers.com/windows-11-22h2/)之后 Windows 11 下一个开发周期的一部分。因为我们仍然处于开发的早期阶段(版本 22H2 甚至还没有公开发布)，所以还没有大量的新功能，并且这个版本完全专注于修复。

事实上，这次即使是修复列表也相对较短。文件资源管理器选项卡的一些问题已被修复，例如选项卡对于某些用户来说显得太大。以下是完整列表:

**【文件浏览器】**

*   修正了一个缩放问题，该问题可能会导致选项卡意外变大。
*   右键单击一个选项卡，然后在文件浏览器中单击其他地方，现在应该可以更可靠地关闭上下文菜单。

**【其他】**

*   我们认为，Build 25145 中的一个底层修复解决了最近的问题，即通过开始菜单关机对一些内部人员不起作用(意外地重新启动)，因此我们从已知问题列表中删除了这个问题。如果您在最新更新中继续遇到此问题，请在反馈中心报告。
*   修正了一个高命中率的 Windows 安全应用程序崩溃。
*   更新了 Windows 安全应用中的排除页面，以便文件路径现在可以更好地利用可用空间，而不是在空间仍然可用时截断。
*   修复了在试图删除 printui /s 中的端口时导致崩溃的潜在问题。
*   修正了在最近 2 次飞行中一些内部人员在 UWP 应用程序中无法打印的问题。

尽管专注于修复，Windows 11 build 25151 仍然存在一些已知问题，您可以在下面找到这些问题。

### Windows 11 内部版本 25151 中的已知问题

**【通用】**

*   我们正在努力解决关于[云母材料](https://docs.microsoft.com/en-us/windows/apps/design/style/mica)和[丙烯酸](https://docs.microsoft.com/en-us/windows/apps/design/style/acrylic)模糊效果在操作系统表面(如开始菜单、通知中心和其他区域)呈现不正确的报告。
*   一些使用 Easy Anti-check 的游戏可能会崩溃或导致您的电脑进行错误检查。
*   我们正在调查一些内部人员在 NetAdapterCx.sys 中遇到错误检查的报告，错误消息为 KMODE_EXCEPTION_NOT_HANDLED，从内部版本 25145 开始。

**【文件浏览器】**

*   文件资源管理器选项卡中的向上箭头没有对齐。这将在未来的更新中得到解决。
*   我们正在调查这样的报告:在使用黑暗模式时，以某些方式启动文件资源管理器(例如，从命令行)会在明亮模式下意外显示文件资源管理器的主体。

**【微件】**

*   我们正在修复一个导致小部件首选项(温度单位和固定小部件)意外重置为默认值的问题。

**【直播字幕】**

*   全屏模式下的某些应用程序(如视频播放器)会阻止显示实时字幕。
*   位于屏幕顶部附近并在运行实时字幕前关闭的某些应用程序将在位于顶部的实时字幕窗口后重新启动。当应用程序有焦点时，使用系统菜单(ALT +空格键)将应用程序的窗口进一步下移。

Windows 11 目前最令人兴奋的事情是版本 22H2 的更新，目前正在测试版和发布预览版渠道与内部人士进行测试。这个应该会在未来几个月公开推出，它包含了大量的改进，包括开始菜单文件夹，新的触摸手势等等。

目前，只有几个东西是 Dev 频道独有的，包括桌面上的搜索栏和对设置应用程序中订阅管理的一些改进。不过，如果你已经在这个渠道注册了，你可以从 Windows Update 获取 Windows 11 build 25151 来获得以上修复。在接下来的一年左右，我们应该会看到更多的特性和变化。

* * *

来源:[微软](https://blogs.windows.com/windows-insider/2022/06/29/announcing-windows-11-insider-preview-build-25151/)