# 如何以两种简单的方式在 Chromebook 上运行 AutoCAD

> 原文：<https://www.xda-developers.com/how-to-run-autocad-chromebook/>

人们普遍认为 Chromebooks 无法运行 PC 或 MAC 上的强大软件。如果你是一名工科学生，你可能需要在你的笔记本电脑上运行一些相当密集的应用程序。Chromebooks 是学生的绝佳解决方案，因为它们既安全又经济实惠。

如果你是一名使用 Chromebook 的工科学生，你可能需要运行 AutoCAD 来完成一些课程作业。与在 PC 上不同，AutoCAD 不提供原生 ChromeOS 安装。幸运的是，仍然有一些简单的方法可以在 [Chromebook 或其他 ChromeOS 设备](https://www.xda-developers.com/best-chromebooks/)上利用 AutoCAD 的绘图功能。我们将了解面向学生的 AutoCAD 在线版本，并讨论如何使用 Parallels 面向企业客户运行完整版本的 AutoCAD。

## 使用浏览器![auto cad web app splash](img/e88da8c96c77c0095c753d719a3a8f9d.png)在 Chromebook 上运行 AutoCAD

如果您只需要 AutoCAD 来完成非常基本的任务，如工程入门或制图课程，那么您的最佳选择是在浏览器中运行 AutoCAD 或使用 Progressive Web App (PWA)。AutoCAD 为云计算提供了一个强大的在线平台。

要使用 AutoCAD online，您只需登录到您的[大学或组织的](https://www.xda-developers.com/best-business-chromebooks/) AutoDesk 帐户，并选择 online 选项。如果您已经登录到您的 AutoDesk 帐户，您可以通过[web.autocad.com](https://web.autocad.com)直接访问在线平台。

使用 AutoCAD online 的主要缺点是必须将文件存储在云中。令人欣慰的是，AutoCAD 让你可以轻松地将任何你想要的云服务与他们的 web 应用程序相集成。这与 MATLAB online 的情况形成鲜明对比。在 AutoCAD web 应用程序中，您可以选择 Dropbox、box、OneDrive、Google Drive 等作为您的主要云存储服务。此选项使在浏览器中使用 AutoCAD 进行任务和协作项目变得更加容易。

老实说，浏览器的速度令人印象深刻。对于大多数 2D 设计任务，AutoCAD 可以在 web 应用程序中完美运行。如果你尝试更高级的 3D 绘图，会有一点滞后，但这是意料之中的。web 应用程序中的功能包括:

*   通过选择功能区或命令行来编辑几何图形，并在图形中选择、移动、旋转和缩放对象。
*   访问易于使用的绘图工具并管理视图、属性和图层。使用清晰的图标和现代的蓝色界面减轻眼睛疲劳。
*   安全地审阅并直接向 DWG 文件添加反馈，而无需修改现有绘图。
*   将您的绘图的受控副本发送给队友和同事，以便他们随时随地访问。
*   查看、编辑、共享和保存存储在 Autodesk Drive 和 Autodesk Docs 以及 OneDrive、Google Drive、Dropbox 和 box 中的图形。
*   轻松访问命令行，该命令行停靠在绘图区域的左下角，显示提示、选项和消息。
*   进行测量并在绘图中添加尺寸。

可以肯定的是，只有在 PC 版的 AutoCAD 中才有一些高级的旋转和操作功能，但 web 应用程序的功能总体来说令人印象深刻。

## 为 ChromeOS 使用 AutoCAD 扩展![auto cad drive app](img/d474ddc950e0e3402fbb260551725637.png)

对于那些计划经常使用 AutoCAD 应用程序的人，你可能还想在 Chromebook 的应用程序抽屉中添加一个 web 应用程序的快捷方式。您还可以通过 Google Workspace Marketplace 为 AutoCAD web 应用程序安装 Google Drive 扩展。这允许你直接将 AutoCAD 与 Google Drive 集成。安装此扩展后，您可以通过右键单击使用 Drive 中的“打开方式”选项直接在 AutoCAD 中打开文件。

显然，在 PC 上使用 AutoCAD 的本地副本要好得多，它具有附加功能和本地文件存储。尽管如此，对于在作业中使用 AutoCAD 的学生来说，这应该可以完成任务。你可以随时选择在 AutoCAD 的云存储和你自己的 Google Drive 或 Dropbox 文件夹之间来回移动文件。显然，这并不理想，但在必要时可以完成工作。如果你有一台 [LTE Chromebook](https://www.xda-developers.com/best-chromebooks-lte-5g/) ，确保在 AutoCAD 中关闭云服务的自动同步。

## 使用 Parallels Desktop 在 Chromebook 上运行 AutoCAD![chrome os chromebooks windows parallels](img/3f245882332111b36b0512c80ca9ab0b.png)

对于那些无法使用在线解决方案的人，如果您是企业或教育客户，还有另一个方便的选择。可以使用 Parallels Desktop for ChromeOS 安装 Windows 版本的 AutoCAD。

[Parallels Desktop](https://www.anrdoezrs.net/links/100122946/type/dlg/sid/UUxdaUeUpU4743/https://www.parallels.com/products/desktop/chrome/?utm_source=google&utm_medium=cpc&creative=474284210573&keyword=parallels+desktop+chrome&matchtype=e&network=g&device=c&gclid=Cj0KCQjw5auGBhDEARIsAFyNm9Gj-6BHVMW13Co32nbONHgpMYwfmCwskWBthIjP60S22K0P89GygCAaAiIDEALw_wcB) 是一个全功能的 Windows 容器，原生运行在 ChromeOS 上。这个软件允许你运行完整版的 Windows，但是有一些重要的事情需要注意。

Parallels Desktop 软件目前仅面向企业客户，因此目前个人用户很少使用该选项。借助 Parallels Desktop for Chrome OS，IT 部门可以在 Chrome OS 设备上在线或离线使用专有的全功能 Windows 应用程序，包括 AutoCAD。您需要升级 Chrome Enterprise 才能运行 Parallels。Parallels Desktop for ChromeOS 的主要功能包括:

*   对关键业务 Windows 应用的不间断访问
*   在 ChromeOS 和 Windows 之间轻松切换——无需重启。
*   暂停和恢复 Windows 以立即恢复运行。
*   使用 Windows 应用程序打开 ChromeOS 上的文件。
*   额外奖励:使用附带的 Parallels Toolbox 访问 30 多个一键工具。
*   利用桌面应用程序的全部功能，包括 Word、Excel、PowerPoint 等。
*   从 Chrome OS 文件访问 Windows 桌面、文档、下载和自定义文件夹。
*   没有网络？没问题！无论在线还是离线，文件和应用程序都是完全可访问的。
*   通过共享剪贴板在 Chrome 操作系统和 Windows 之间轻松移动内容。
*   从 Windows 打印到支持的打印机。
*   借助无缝鼠标、摄像头、麦克风、音频和坞站以及 USB 智能卡读卡器支持，与时俱进。
*   享受动态分辨率和全屏支持带来的视觉享受。

### 运行 Parallels Desktop 的要求

在 Chromebook 上运行 Parallels 有最低系统要求。您至少需要 ChromeOS 版或更高版本。此外，如果您希望分发到组织中的多台机器，您需要 Google 管理控制台、Chrome 企业升级/Chrome 教育升级、Microsoft Windows ISO、Windows 许可证和存储服务器。在硬件方面，支持的处理器包括英特尔酷睿 i5 或 i7 以及 AMD 锐龙 5 或 7。您的设备上还需要至少 8 GB 的 RAM 和 128 GB 的 SSD 本地存储。

虽然其中一些规范似乎有所限制，但请记住，该软件目前面向企业客户。有很多宏碁、惠普、联想的企业级 Chromebooks 符合要求。如果你的 Chromebook 或 ChromeOS 平板电脑满足最低要求，你可能也会喜欢购买一个 T2 坞站，将你的 Chromebook 变成一个完整的工作站。

从技术上来说，如果你是个人，你可以在支持的 Chromebook 上升级到 Chrome Enterprise。你需要做的就是从 Squarespace 这样的提供商那里购买一个网站域名，然后将它链接到一个 Google Workspace 账户。Google Workspace、Chrome Enterprise 和你的域名都有相关的成本，所以如果你没有真正的业务，这可能是一个非常昂贵的方法。

不过，如果您是企业客户，Parallels Desktop 绝对值得。如果你对通过 Parallels 在 Chromebook 上运行 Windows 的完整过程感兴趣，[参见我们的完整教程](https://www.xda-developers.com/windows-10-chrome-os/)。

一切就绪，这就是使用 web 应用程序或 Parallels 在 Chromebook 或其他 ChromeOS 设备上安装 AutoCAD 的整个过程。我们希望这能成为一次美好的经历。对于需要本地安装的用户，Parallels Desktop 也是企业用户的绝佳选择。请在下面的评论区告诉我们您使用这两种方法的体验。