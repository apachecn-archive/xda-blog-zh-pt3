# 如何在 Windows 11 中批量重命名文件

> 原文：<https://www.xda-developers.com/how-to-batch-rename-files-windows-11/>

当你有一整个文件夹都是照片或者其他什么东西的时候，重命名文件可能是一件非常乏味的事情。如果你一次一个地给它们重新命名，你可能会在那里呆上一段时间。值得庆幸的是，如果你想重命名一堆文件，在 Windows 11 上有更有效的方法。事实上，在 Windows 11 中有大量的应用程序或程序可以用来批量重命名文件，但即使是操作系统本身也可以相对容易地一次更改多个文件的名称。

在这篇文章中，我们将向您展示几种重命名文件的方法，如果您想节省一些时间，并且在将来更容易找到您要找的东西。同样，还有其他方法可以做到这一点，但这些方法应该可以满足您的大部分需求。让我们开始吧。

## 使用 Windows 11 文件资源管理器重命名文件

虽然不是很明显，但 Windows 11 中的文件资源管理器确实让一次性重命名一批文件成为可能。这并没有给你太多的选择，但是如果你想要的只是将一堆文件重命名为标准格式，那么这可能就是你所需要的。你可以这样做:

*   打开文件资源管理器，导航到包含要重命名的文件的文件夹。
*   选择所有要重命名的文件。如果不想选择每个文件，可以按住 **Shift** 键，单独选择文件。
*   点击工具栏上的**重命名**按钮，或者右键单击选中的一个文件，然后在右键菜单中选择**重命名**选项。
*   只有其中一个文件会显示可编辑的文本框，但该名称将应用于您选择的每个文件。写下你想要的文件名，然后按键盘上的**回车**。
*   您的文件现在都有了您选择的名称，后面跟着一个数字。

这是一个相当简单的过程，正如我们已经提到的，你没有太多的选择，但它可能对很多人来说都很好。

## 使用 PowerToys 重命名文件

如果你想要更多的选择来重命名你的文件，那么一个很好的选择就是使用微软自己的 PowerToys 软件。PowerToys 的现代版(最初的 PowerToys 是为 Windows 95 和 XP 设计的)附带了一个名为 PowerRename 的工具，你可以使用一系列条件批量重命名 Windows 11 上的文件，以获得你想要的确切格式。这有点复杂，但为了得到您想要的结果，这可能是值得的。首先，您需要安装 PowerToys 并确保 PowerRename 正在运行:

*   从 GitHub 下载最新的 PowerToys 安装程序[(你需要向下滚动到页面底部找到安装文件)并安装程序。安装完成后,“欢迎使用 PowerToys”窗口会自动打开。](https://github.com/microsoft/PowerToys/releases/tag/v0.58.0)
*   从侧边菜单中选择**电源重命名**，然后点击**打开设置**。如果你没有看到欢迎窗口，从你的开始菜单中打开 PowerToys，然后从左边的工具条中选择 **PowerRename** 。
*   确保在上将 PowerRename 功能设置为**(这应该是默认设置)。**

启用 PowerRename 后，您现在可以转到您的文件并开始重命名它们。PowerRename 的功能远比 Windows 11 中简单的重命名工具强大。您可以匹配原始文件名中的任何单词或字符，并将其替换为其他内容，因此您可以只更改文件名的一部分，以使文件更容易识别。您还可以使用正则表达式(RegEx)来创建某些条件，以匹配文件名并将它们更改为其他名称。以下是如何做到这一点:

*   使用文件资源管理器导航到文件所在的文件夹。
*   选择所有你想要重命名的文件，然后右击它们并在上下文菜单中选择**查看更多选项**。然后，在第二个上下文菜单中选择**电源重命名**。
*   现在，您将看到包含所有选定文件的 PowerRename 界面。例如，下面的图片是来自智能手机的相机样本，它们都被命名为“IMG ”,后跟日期和时间。假设我们希望保留时间戳，并且只将“IMG”部分替换为更容易识别的部分。只需在你想要匹配的文本上方的框中写下“IMG”。**注意:**在这里，你可以使用各种条件来重命名你想要的文件。您可以匹配原始名称中的任何文本，使用正则表达式匹配整个单词和数字，等等。您可以单击文本框旁边的信息图标来查看支持哪些类型的表达式。
*   在底部的框中，您可以选择匹配的文本将被替换为什么。这些是为我们的[联想 Yoga 6 评测](https://www.xda-developers.com/lenovo-yoga-6-review/)拍摄的图片，所以让我们以笔记本电脑命名这些文件。我们还将在末尾添加一个额外的空格，以便时间戳与单词本身分开。正如我们提到的，这里有很多选项，包括给文件名添加日期和时间，如果还没有的话。如果你用相同的名称命名，你也可以列举项目。在应用更改之前，您可以看到最终的文件名是什么样子，所以请确保一切都是您想要的。
*   点击**应用**，文件名将根据您的标准改变。您可以在文件资源管理器中看到新名称。

如果你想在你的 Windows 11 电脑上重命名一批文件，这应该就够了。还有其他方法，但这两种方法应该可以满足大多数人的需求。我们认为 Windows 内置的方法可能对几乎每个人都足够好，但是 PowerToys 肯定提供了一些更强大的定制来获得您想要的确切文件名。

如果你想了解 Windows 11 的其他功能，为什么不看看[如何启用上帝模式](https://www.xda-developers.com/how-to-enable-god-mode-windows-11-what-is-it/)以便快速访问各种 Windows 设置？或者学习如何[关闭 Windows 11 开始菜单中的推荐内容](https://www.xda-developers.com/how-to-turn-off-start-menu-recommended-content-windows-11/)。