# 以下是如何下载和安装 Windows 11

> 原文：<https://www.xda-developers.com/download-windows-11/>

Windows 11 已经推出一年多了，这是该公司制作的最好的操作系统之一。Windows 11 的最初版本带来了一种全新的设计语言，有更多的渐变、颜色和圆角，以及许多重新设计的应用程序。最近，Windows 11 2022 更新进行了更多更新，为平板电脑添加了新的触摸手势，改造了任务管理器，等等。但 Windows 11 对我们许多人来说仍然是新的，部分原因是高系统要求，加上它是一个可选的更新。如果你想在你的电脑上安装 Windows 11，有几种方法可以实现。

然而，即使你不打算升级，有时执行 Windows 11 的全新安装也是好的，只是为了整理东西，让体验再次更流畅。如果您已经开始注意到操作系统的一些问题，它也会有所帮助。因此，让我们来看看您可以在 PC 上下载和安装 Windows 11 的所有主要方式。

## 下载前

在我们开始之前，你要做的第一件事是确保你的电脑符合 Windows 11 的[系统要求。如果你运行的是 Windows 10，你可能会发现一些更难满足的新要求，比如 4GB 内存、64 位 CPU 或 TPM 2.0 模块。事实上，有一个兼容](https://www.xda-developers.com/windows-11-minimum-requirements/)的[CPU 列表，而且是一个相当有限的列表。](https://www.xda-developers.com/cpus-compatible-windows-11/)

除此之外，在进行这样的升级之前，最好是安全起见，所以请确保您已经将文件备份到云服务或外部存储设备，如闪存驱动器或外部 SSD。

## 使用 Windows Update 下载 Windows 11

现在下载 Windows 11 最简单的方法是通过 Windows Update。绝大多数运行 Windows 10 的受支持 PC 应该可以通过 Windows Update 找到 Windows 11。

要做到这一点，只需打开 Windows 10 PC 上的设置应用程序，并转到**更新&安全**部分。如果你的电脑被选中进行首次展示，你会看到一个宣传 Windows 11 的大横幅，你可以选择立即下载。

这将会以最简单的方式下载和安装 Windows 11，并且在安装之后你不需要设置任何东西。如果可以的话，我们建议你走这条路，但是如果这条路不通的话，你会有更多的选择。

另一种下载 Windows 11 的官方方式是使用微软提供的工具手动下载 Windows 11。最通用的方法是使用媒体创建工具，因为您可以使用它来升级您当前的电脑或为另一台电脑创建安装媒体，如果您离线或稍后互联网速度较慢，您可以使用它。以下是要做的事情:

1.  进入 [Windows 11 下载页面](https://www.microsoft.com/en-us/software-download/windows11)。
2.  在**创建 Windows 11 安装介质**下，点击*立即下载*。
    *   或者，你可以直接从网站的**下载 Windows 11 磁盘镜像(ISO)** 下下载一个 ISO。如果有，请跳到步骤 7。

3.  运行您刚刚下载的文件，并接受条款和条件。
4.  为您的 Windows 11 安装选择所需的语言和版本设置。默认情况下，它会为您的电脑选择正确的设置，但如果您要为另一台电脑创建安装介质，您可以更改这些设置。
5.  选择是要创建 ISO 文件还是可引导 USB 闪存驱动器。
    *   **注**:如果您想要使用可引导的 USB 介质执行全新安装，请选择您想要使用的 USB 闪存驱动器，然后单击下一步。你可以跳到下面的[如何安装 Windows 11 部分](#Install)。

6.  下载将会开始，您的 ISO 文件将会保存在您选择的文件夹中。
7.  在想要升级的电脑上，双击 ISO 文件，然后运行里面的**安装**文件。
8.  按照屏幕上的步骤将您的电脑升级到 Windows 11 或重新安装操作系统。

如果需要，您可以稍后使用此 ISO 文件创建可启动的 USB 闪存驱动器。查看下面的[从 ISO 部分创建安装介质](#CreateInstallMedia)以了解如何操作。

正如我们上面提到的，如果你下载了一个 ISO 文件，而你只是想升级到 Windows 11，你实际上可以在 Windows 中挂载 ISO 文件，并从那里运行安装文件。双击 ISO 文件，运行安装文件，就可以开始了。但是，如果您想要执行全新安装或格式化您的电脑，您可能需要创建一个可引导的 USB 驱动器。你可以使用你已经下载的 ISO 来完成。另外，这种方法还可以让你在非官方支持的硬件上安装 Windows 11。

如果你想创建一个 USB 安装媒体，可以用于其他电脑或干净的安装，你需要一个像 Rufus 的程序。这可以把你的 ISO 文件闪存到你的闪存驱动器，这样你就可以从它启动。在开始之前，请确保您的 USB 驱动器上没有任何重要文件，因为它们会在此过程中被删除。USB 驱动器还需要 8GB 或更大的容量。一旦解决了这个问题，下面是你需要做的:

1.  [下载 Rufus](https://rufus.ie/en/) 并安装程序(或下载便携版)。
2.  插上你的 u 盘运行 Rufus。
3.  点击 SELECT，找到之前下载的 ISO 文件。所有其他选项将自动填写。
4.  单击开始，等待该过程完成。

## 如何使用 u 盘安装 Windows 11

实际上安装 Windows 11 是一个非常简单的过程。创建安装介质后，您只需启动闪存驱动器中的安装文件，然后点击完成安装过程。一旦安装过程完成，你将运行 Windows 11。如果你想这样做，这和有一个 ISO 文件差不多。

但是，如果您想要一个干净的体验，并将 Windows 11 PC 设置为全新的机器，您可以进行干净的安装。这意味着删除你的驱动器上的所有数据，但它会让你有一个最干净的体验。开始之前，请确保您已经备份了所有需要的数据。插入 USB 安装介质后，按照以下步骤操作:

*   进入**设置- >更新&安全- >恢复**。
*   在*高级启动*下，点击*立即重启*。
*   在弹出的菜单中，点击*选择设备*，然后点击你的 USB 驱动器。

*   从这里，您将被带到安装环境。选择您的语言和键盘设置，然后单击*立即安装*并接受许可条款。

*   在下一个屏幕中，您需要选择*自定义:仅安装 Windows(高级)*。

*   您将看到电脑上的驱动器和分区列表。

*   您可以选择格式化或删除它们，并在未分配的空间中创建一个新的分区。不管怎样，你都会丢失数据。在这种情况下，我们删除了分区并创建了一个新分区。Windows 会自动创建一些运行所需的附加分区。

*   点击*下一步*，安装将开始。

安装完成后，您将获得开箱即用的体验(OOBE)。这是您第一次设置新电脑时或重置后看到的画面。

## 设置 Windows 11

要准备好使用 Windows 11，您需要完成几个步骤。整个过程如下:

*   首先，您需要选择您的地区和键盘布局。

*   接受许可条款，然后您将有机会命名您的电脑。

*   然后会要求您使用 Microsoft 帐户登录。这对于 Windows 10 家庭用户是强制性的，但有些版本可以使用本地帐户。

*   登录后，您可以设置 PIN 来替换您的密码。如果您使用 Microsoft Authenticator 登录，则必须设置 PIN。

*   Windows 11 中的一个新功能是备份您的设置和已安装的应用程序，这使得设置新电脑更加容易。如果你以前使用过 Windows 11，你会看到一个从以前的备份中恢复的选项。

*   接下来，您需要完成一些隐私设置。这些包括允许应用程序使用你的位置、你要向 Microsoft 发送多少诊断数据，或者应用程序是否可以使用你的广告 ID。选择适合你的应用，然后点击*下一步*。

*   接下来，您可以设置您的设备使用情况。你可以告诉 Windows 你更有可能用你的电脑做什么，你将获得基于此的建议和提示。你也可以什么都不选，点击*下一个*这里。

*   最后，您可以设置是将文件保存在 OneDrive 上还是仅保存在您的电脑上。将你的文件保存到 OneDrive 意味着你可以备份这些文件，以防你的计算机出现问题，但你可能需要订阅 Microsoft 365 才能容纳所有文件。

*   在短暂的设置阶段后，你将被带到 Windows 11 桌面。

这就是你现在下载安装 Windows 11 需要了解的全部内容。由于它仍处于早期测试阶段，所以下载操作系统的选项并不多，但以后会有更多的选项。随着更多选项的出现，我们将更新这篇文章，这样您可以更容易地选择您喜欢的选项。