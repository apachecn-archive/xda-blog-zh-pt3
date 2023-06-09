# 如何在 Windows 11 Home 上安装 Hyper-V

> 原文：<https://www.xda-developers.com/how-to-install-hyper-v-windows-11-home/>

Windows 的每个主要版本都有一个[几个不同的版本](https://www.xda-developers.com/windows-11-skus/)，或者 SKU，它们有不同的特性。即将到来的 [Windows 11](https://www.xda-developers.com/windows-11/) 也不例外，我们已经知道它会有家庭版、专业版等版本。通常只有 Windows 专业版才有的一大功能是 Hyper-V，但经过一些修改，你实际上可以在家庭版上获得它。如果你感兴趣的话，下面是如何在 Windows 11 Home 上安装 Hyper-V 的方法。

## 什么是 Hyper-V？

Hyper-V 是微软的虚拟机管理程序软件，它允许你在你的电脑上创建和运行虚拟机。虚拟机(VM)允许您创建不影响您的主机 PC 的操作系统的隔离实例。虚拟化软件有几种选择，但 Hyper-V 是 Windows 自带的，如果您正在管理 Windows 虚拟机，它是理想的选择。

Hyper-V 可以用于测试不稳定或危险的应用程序，或者如果您需要特定操作系统的特定功能。例如，如果你需要 Linux 的某些东西，但你更喜欢 Windows 作为你的主要操作系统，你可以安装 Ubuntu。

Hyper-V 最初是在 Windows Server 2008 上实现的，从那以后它就成为了 Windows 的一部分。对于普通的 Windows，它只适用于操作系统的专业版、企业版和教育版——也就是说，是官方版本。即使在那些版本中，它通常也是一个可选功能，所以你必须进入设置应用程序才能安装它。

在 Windows 11 上，你可以通过进入*应用* > *可选功能*来安装 Hyper-V。滚动到页面底部，点击*更多 Windows 功能*，然后找到 Hyper-V 并安装。

## 如何在 Windows 11 Home 上安装 Hyper-V

你可能认为让 Hyper-V 在家庭版 Windows 上运行很复杂，但它却出奇的简单。你需要做的是:

*   打开记事本(或其他纯文本编辑器)创建文本文件。
*   将以下内容粘贴到文件中:

`pushd "%~dp0"`

目录/b % SystemRoot % \服务\包\*Hyper-V*。mum >hv.txt

for/f % % I in(' findstr/I . HV . txt 2^>nul')do dism/online/no restart/add-package:" % systemroot % \ servicing \ packages \ % % I "

del hv.txt

dism/online/enable-feature/feature name:Microsoft-Hyper-V-All/limit access/All

中止

*   用名称 **hv.bat** 保存文件。你可以把它保存在你喜欢的任何地方。
*   保存后，右键单击文件并选择*以管理员身份运行*。
*   让流程运行；这可能需要一段时间。一旦完成，你必须重新启动电脑。
*   Hyper-V 应该会自动安装，您可以通过在开始菜单中搜索找到它。它将被称为 Hyper-V 管理器。

它也可以在 Windows 工具中找到。如果它没有出现，请尝试以下操作:

*   打开设置应用，进入*应用* > *可选功能*。
*   滚动到底部，点击*更多 Windows 功能*。
*   在列表中找到 Hyper-V 并启用它。之后您可能需要重新启动。

*   现在，您应该能够使用 Hyper-V 来创建和管理虚拟机。

在 Windows 11 Home 上安装 Hyper-V 大概就知道这么多了。本指南也适用于 Windows 10。不幸的是，安装 Hyper-V 不能启用 [Windows 沙盒](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-sandbox/windows-sandbox-overview)，这是 Windows 的另一个很酷的虚拟化功能。Windows Sandbox 会创建当前 Windows 版本的干净副本，以便您可以在其上测试软件。它有一个稍微不同的用例，因为它只复制您当前的 Windows 版本，而不是您想要的任何操作系统。此外，Windows 沙盒会在每次关闭时重置。它实际上只是为了快速测试特定的应用程序或设置，而不会损坏你的电脑。

使用 Hyper-V，您可以使用自己的 ISO 文件创建虚拟机，也可以选择微软提供的选项之一。该公司实际上提供了开箱即用创建 Ubuntu 虚拟机的能力。虚拟机是持久的，除非你选择删除它们，所以与 Windows 沙盒相比，它们肯定有不同的应用程序。

想在 Windows 11 正式发布的时候拿到？确保你有一台与升级兼容的电脑[。如果你想获得最新的更新，请关注我们的](https://www.xda-developers.com/windows-11-compatible-pc/) [Windows 11 更新跟踪器](https://www.xda-developers.com/windows-11-update-tracker/)。