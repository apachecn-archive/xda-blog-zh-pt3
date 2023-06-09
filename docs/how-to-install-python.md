# 如何在 Windows、Linux 和 macOS 上安装 Python

> 原文：<https://www.xda-developers.com/how-to-install-python/>

如果你想从事开发，我最喜欢的编程语言之一就是 Python。它是一种多范式语言，支持命令式、函数式、过程式和面向对象的编程。它非常开放，几乎可以用于任何事情，是许多从事人工智能或机器学习的人的首选语言。我用它来实现很多自动化，它甚至是我们使用的一些测试工具所用的语言。

Python 是一门强大的语言，如果你想开始学习，本指南将教你基础知识。您不仅需要安装 Python 二进制文件并确保它在您的路径中，还需要一些东西来实际编写代码。你可以使用一个成熟的 IDE(集成开发环境),比如 PyCharm，或者你可以使用一个文本编辑器，比如预装的 IDLE 或者 Sublime Text 3。有很多选择，但是这个指南应该让你从基础开始。

## 安装 Python

### 在 Windows 和 macOS 上

安装 Python 是比较容易的部分，你需要决定是安装 Python 2.7 还是 Python 3.x. Python 2.7 通常用于遗留项目，但是如果你正在编写自己的软件，那么你应该安装 Python 3.x。

要在 Windows 或 Mac 上安装，请执行以下操作:

*   转到官方 Python 站点，并导航到最新版本。在撰写本文时，那是 3.10.6。
*   为您的平台下载二进制文件。
*   执行二进制文件。

除了将 Python 添加到您的路径之外，您不需要选择任何选项，因为默认安装程序拥有您需要的一切。只需点击“安装”即可。在 Mac 上，这将在 dmg 安装程序中默认完成。

### 在 Linux 上安装 Python

但是，如果您使用 Linux，那么这将取决于您使用的发行版。基于 Debian 的发行版(如 Ubuntu)可以通过执行以下命令在终端中使用 apt 包安装程序:

*   apt-get 安装 python3.6

其他发行版可能已经预装了它，如果没有，您将需要在您的发行版中使用软件包管理器。例如，在 CentOS 上，您可以执行“yum install -y python3”。

### 验证安装

您可以通过在 PowerShell、命令提示符或终端中运行“python”命令来验证您的安装是否处于活动状态。

* * *

## 选择您的 Python IDE

您需要一个 IDE 或文本编辑器来有效地编写代码，有几个选项可供选择。Python 预装了 IDLE，虽然它工作得很好，但对于可能更复杂的较大文件来说并不太好。这里是我多年来在大学和自己的项目中使用的一些 Python over。所有这些 ide 都是跨平台的，这意味着您可以在 Windows、Linux 或 macOS 上运行它们。

### 皮查姆

如果你熟悉 Android Studio 或 IntelliJ，那么你已经熟悉 PyCharm 了。它来自同一个开发者，你甚至可以通过安装 Python 插件在 IntelliJ 中启用完全相同的功能。不同之处在于，PyCharm 完全是为 Python 从头开始构建的，它包含了所有现代 IDE 的所有特性。这包括内置的版本控制、语法高亮、窗口分割、调试特性等等。

[下载 PyCharm](https://www.jetbrains.com/pycharm/)

### Spyder

如果您是一名数据科学家(或者打算将 Python 用于数据科学目的)，那么您需要安装 Spyder。这是一个集成了一些最流行的 Python 数据分析包的 IDE。其中包括 matplotlib、numpy、scipy 和 pandas。如果你想进入数据分析，数据绘图，和其他科学调查，那么 Spyder 是 100%你需要安装。Spyder 甚至内置了 Jupyter 笔记本，可以用来非常轻松地探索和绘制数据。

[下载 Spyder](https://www.spyder-ide.org/)

### 崇高文本 3

Sublime Text 3 是我的首选文本编辑器之一，这完全归功于它的简单性。它超级通用，尽管是最基本的，更适合小型项目。如果你正在编写的程序只有几百行代码，那么 Sublime Text 3 可能是最好的选择。我曾经用 Python 写了一个 web scraper，它可以读取当地的租房网站，并用 Sublime Text 3 和 Python 通过电子邮件给我和一些朋友发送新房源的链接。这是一个非常好的开发环境，我认为大多数人都应该熟悉它。

[下载崇高文字 3](https://www.sublimetext.com/3)

### Visual Studio 代码(VSCode)

Visual Studio 代码(或 VSCode)是最通用的开发环境之一。它是完全可定制的，有一个庞大的插件库，你可以从里面访问。它不能马上与 Python 兼容，但是你可以从内部安装一个 Python 插件，它将支持语法高亮、智能代码完成、Jupyter 笔记本、调试、单元测试和其他功能。我喜欢 Visual Studio 代码，实际上，当我处理复杂的东西时，它是我使用最多的 IDE。

[下载 Visual Studio 代码](https://code.visualstudio.com/)

* * *

## 下一步怎么样

如果你想开始开发，网上有很多教程会教你基础知识。在 CodeAcademy 和 w3schools 之间，有很多选择。Android 上甚至有 Python 解释器，你可以用它在手机上写东西，最好的学习方法是边做边学。但是，如果你正在做任何可能使用大量机器学习模型或人工智能的资源密集型工作，你可能需要一台[最好的笔记本电脑](https://www.xda-developers.com/best-laptops/)来处理它。

我学到的最好的方法是通过意识到一个问题或我遇到的其他困难，并试图找出一种自动解决它的方法。这就是为什么我有了写一个程序的想法，这个程序将为我节省租用网站的费用，我相信还有其他的原因让你发现你也想使用 Python。