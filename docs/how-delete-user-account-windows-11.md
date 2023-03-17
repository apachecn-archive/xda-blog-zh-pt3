# 如何在 Windows 11 上删除用户帐户

> 原文：<https://www.xda-developers.com/how-delete-user-account-windows-11/>

在 Windows 上支持多个账户是该操作系统最好的特性之一，而且它已经存在很长时间了。例如，与家庭成员共享电脑会变得容易得多，而不会混淆文件。但是当你不再需要它们的时候会发生什么呢？谢天谢地， [Windows 11](https://www.xda-developers.com/windows-11/) 给了你很多删除用户账户的方法。

可以说，你只需要我们下面讨论的方法中的一种，但是你可以选择你喜欢的任何一种。你可以使用 modern Settings 应用程序，但旧的控制面板仍然有效，并且也有用于命令提示符和 Windows PowerShell 的方法。值得注意的是，我们这里说的是用户账户，不是微软账户。如果你想从你的电脑中移除你的微软账户，请查看关于[切换到本地账户](https://www.xda-developers.com/windows-11-microsoft-local-account/#switching-to-a-local-account)的指南。

## 如何使用“设置”应用程序删除用户帐户

在 Windows 11 上删除用户帐户的首选方法是通过设置应用程序，因为这是更积极维护的界面。这个过程实际上可能看起来有点混乱，因为有许多与微软账户相关的选项，但这里是你需要做的。

1.  打开**设置 app** 。
2.  在左侧窗格中，点击**账户**。
3.  点击**其他用户**查看您电脑上的账户列表。
4.  点击您想要删除的账户，然后点击**账户和数据**旁边的**删除**按钮。
5.  确认您要删除该帐户，所有相关数据都将被删除。

这就是全部，所以这是一个非常简单的过程。当然，如果不喜欢用设置 app，还有很多其他方法。

## 如何使用控制面板删除用户帐户

如果你仍然喜欢使用旧的控制面板，微软仍然没有删除这样做的选项。方法如下:

1.  打开**控制面板**(可以使用开始菜单中的搜索栏找到)。
2.  点击**用户账户**。
3.  点击**删除用户账户。**
4.  您将看到您电脑上所有帐户的列表。点击您想要删除的账户，然后在下一页选择**删除账户**。
5.  系统会询问您是否要保留与该帐户相关联的文件。选择**删除文件**删除所有内容，或者**保留文件**保存到当前用户的桌面上。
6.  点击**删除账户**确认删除。

这种方法是有益的，因为如果您不想丢失这些文件，它可以让您选择保留用户的数据。请注意，微软已经将大多数控制面板选项转移到设置应用程序，所以这可能会在某个时候消失。

## 如何使用 Windows 终端(Windows PowerShell)删除用户帐户

如果您喜欢使用命令行界面来使用 Windows，您可以使用 Windows PowerShell 或 Windows 终端来删除用户帐户。Windows 终端是作为 Windows 的一部分提供的最新终端，默认情况下，它会打开 Windows PowerShell 配置文件，尽管它也可以用作经典的命令提示符(我们将在后面介绍)。要删除 Windows 终端/ PowerShell 用户帐户，请按照下列步骤操作:

1.  以管理员身份启动 **Windows 终端**。你可以右击开始菜单(或者按 **Windows + X** ，选择 **Windows 终端(管理)**来完成这个操作。
    *   **注意:**该选项也可能显示为**终端(管理)**或 **Windows PowerShell(管理)**。

2.  要查看 PC 上的所有用户帐户，请键入 **Get-LocalUser** ，然后按 **Enter** 。
3.  一旦你知道要删除什么账户，输入**Remove-local user-Name“USERNAME”**。你必须用你想删除的账户的名字替换用户名(在这个例子中，是测试(T21)
4.  该帐户将被删除，但其中的文件将保留在“用户”文件夹中。

## 如何使用命令提示符删除用户帐户

经典的命令提示符也可以用来删除 Windows 11 上的用户帐户，这与使用 Windows 终端非常相似。事实上，如果您愿意，可以在 Windows 终端中使用命令提示符。如果你喜欢这样做，下面是方法:

1.  打开开始菜单，搜索命令提示符。
2.  在第一个结果下选择**以管理员身份运行**
3.  要查看您电脑上的用户帐户，请键入 **net user** 并按回车键。
4.  要删除用户帐户，请键入**网络用户用户名** **/delete** 。你必须用你想删除的账户名替换用户名。
5.  与 PowerShell 方法类似，这将删除帐户，但不会删除关联的文件。

## 如何使用“计算机管理”删除用户帐户

上面的方法对大多数人来说应该足够了，但是如果你想走不同的路线，仍然有一些额外的方法来删除用户帐户。默认情况下，这些选项还会对删除用户保留文件。其中之一是使用计算机管理。

1.  右键单击开始菜单图标并选择**计算机管理**。
2.  在左侧窗格中，选择**本地用户&组**，然后打开里面的**用户**文件夹。
3.  右键单击要删除的帐户，然后选择**删除**。
4.  点击**是**确认删除。

该用户帐户将从您的电脑中删除，但与之关联的文件将会保留。

## 如何使用“用户帐户”对话框删除用户帐户

在 Windows 11 上，你可以用来删除用户帐户的最后一种方法是用户帐户对话框，尽管这种方法实际上有点难找到，除非你明确知道你在找什么。如果你想使用它，你需要这样做:

1.  打开开始菜单，搜索 **netplwiz** ，然后按回车键打开用户帐户对话框。
2.  在列表中点击您想要删除的账户，然后点击**删除**。
3.  在确认提示中点击**是**，然后在用户账户窗口中点击**确定**确认您的更改。

就像上面的方法一样，这种方法也将用户的文件保存在 PC 上。

* * *

这涵盖了广泛的方法，所以在删除不再需要的用户帐户时，您可以选择您喜欢的任何方法。如果你想了解更多关于 Windows 11 的最新功能，也许可以查看[如何启用 Windows 沙盒](https://www.xda-developers.com/set-up-windows-sandbox-windows-11/)如果你有 Windows 的专业版或企业版。