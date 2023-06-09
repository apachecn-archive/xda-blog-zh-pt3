# 如何在 Windows 11 上使用事件查看器检查错误

> 原文：<https://www.xda-developers.com/how-use-event-viewer-windows-11/>

你很有可能在某个时候在电脑上遇到了错误。你可能见过一两次臭名昭著的“死亡蓝屏”或其他问题。虽然大多数人可能不知道，但 [Windows 11](https://www.xda-developers.com/windows-11/) 有一个工具可以让你了解更多关于这些错误的信息，它叫做事件查看器。

事件查看器已经出现在许多 Windows 版本中，它的工作方式基本上和过去一样。它记录所有与你的 Windows 电脑相关的事件，而不仅仅是错误。您想要使用它的主要原因是为了找到关于您遇到的问题的信息。

也就是说，如果你是一个新手，使用事件查看器可能会感觉很复杂，所以我们在这里帮助你。虽然我们不会深入研究具体的错误，但本文将概述如何使用事件查看器在 Windows 11 PC 上查找错误和其他事件。

## Windows 事件查看器界面

在 Windows 11 上打开事件查看器最简单的方法是在开始菜单中搜索它。只需打开开始，在搜索栏中输入**事件查看器**。应该是第一个结果。

首次启动事件查看器时，您会在电脑上看到最近事件的摘要。它包括过去一周记录的所有事件，但也分解了过去 24 小时和过去一小时的事件，从而更容易了解问题可能在何时发生。您还会看到窗口左侧的导航树，以及右侧的**操作**窗格。

正如您在上面看到的，事件查看器跟踪四种常见类型的事件:**严重**、**错误**、**警告**和**信息**。信息事件是最常见的，因为只要事情按预期运行，它们就会出现。警告事件也不是特别有趣，因为它们不一定与任何重大问题相关。

错误事件更有趣，因为它们可能暗示更严重的问题，但是它们也可能在一切正常运行时突然出现。你不应该把这些数字当作某件事一直出错的保证。事情可能很简单，比如一个服务在第一次尝试时无法启动，但后来还是启动了。关键事件是导致计算机崩溃的错误，这些可能是您最常查找的错误。如果你一直碰到蓝屏死机，那是因为这一类的错误。

虽然此摘要很有帮助，但您的注意力可能会集中在左侧导航窗格中的 **Windows Logs** 文件夹上。如果你展开它，你会看到五个不同的日志，最有可能对你很重要的是**系统**和**应用**日志，它们与 Windows 11 本身和安装的应用相关。**安全**日志记录各种安全事件，包括登录尝试，而**设置**日志包括与更新相关的事件。

您可以单击这些日志中的任何一个来查看日志中的所有事件，其中大多数都可能具有**信息**类型。如果您发现想要了解更多信息的错误或警告，您可以点按它，相关信息将出现在窗口底部。您也可以连按事件，在单独的窗口中查看该信息。

事件属性窗格/窗口包括对错误的描述，其中应包含足够的信息，以便您了解错误所在以及如何修复错误(如有必要)。您可能还想查看事件 ID，它可以帮助您在线查找有关该问题的更多信息。在某些情况下，描述本身包括一个错误代码，如果您想在线搜索它，这是很好的。

## 在事件查看器中搜索特定事件

如果您想在日志中找到一个特定的事件，假设您已经知道要查找什么，事件查看器也可以帮助您做到这一点。两个主要的搜索工具会有所帮助，一个更基本，另一个给你更多的高级选项。

### 查找(基本搜索)

更基本的工具叫做 **Find，**你可以用它在任何相关的字段中搜索一个术语来找到一个事件。您可以搜索创建事件的服务、任务类别或事件 ID。以下是如何做到这一点:

1.  打开**事件查看器**。
2.  展开 **Windows Logs** 文件夹(您也可以使用自定义视图，我们稍后会讲到)。
3.  选择您想要搜索的日志，如**系统**。
4.  在窗口右侧的**动作**窗格中点击**查找**。
    *   或者，右击日志并在上下文菜单中选择**查找**

5.  在文本字段中输入关键字、事件 ID 或其他搜索词，然后点击**查找下一个**。
6.  事件查看器将突出显示与关键字匹配的事件，您可以一次循环查看一个事件。

这种更基本的搜索可以帮助您找到一个特定的事件，但它有一定的局限性，因为您一次只能看到一个结果，其他不相关的事件仍然可见。这就是高级搜索工具的用武之地。

### 过滤日志(高级搜索)

如果要查找符合特定条件集的所有事件，最好使用事件查看器中的日志过滤选项。此功能提供了更多方法来查找您要查找的事件。以下是如何做到这一点:

1.  打开**事件查看器**并导航至您想要搜索的日志(如上述步骤 1-3 所述)。
2.  在**动作**窗格中，点击**过滤当前日志**。
3.  在这里，您可以基于多个标准过滤事件。首先，您需要选择您想要查看的事件级别，例如**严重**、**错误**、**警告**或**信息**事件类型。
4.  顶部的 **Logged** 字段允许您选择事件发生的时间，因此如果您知道最近发生了一个特定的错误，您可以过滤它，例如，过去一个小时。
5.  **事件源**过滤器(可选)可让您选择创建您正在寻找的事件的服务或应用。
6.  如果您更具体地知道您正在寻找哪种事件，您也可以输入一个**事件 ID** 。
7.  最后，**关键词**字段提供了您可能正在寻找的常见关键词列表。
8.  应用过滤器后，点击**确定**。
9.  现在，您可以对所有符合您的标准的错误进行排序，并查看有关它们的更多详细信息。

考虑到有成千上万的事件并不总是相关的，这应该更容易找到 Windows 11 中的特定错误。

## 在事件查看器中创建自定义视图

如果事件查看器提供的默认日志对于您的使用来说过于混乱或不完善，您还可以创建自定义视图。这对于经常寻找特定事件的普通用户特别有用，这些事件现在可能在默认日志中组织得很好。自定义视图的工作方式与过滤器类似，只是它们永远可用。以下是创建自定义视图的方法:

1.  打开**事件查看器**。
2.  在左侧窗格中，点击**自定义视图**。
3.  从窗口右侧的**动作**窗格中选择**创建自定义视图**。
4.  **记录的**字段按照我们上面解释的方式工作，因此您可以按日期过滤事件。您也可以像以前一样选择相同的事件级别。
5.  在这里，您可以选择是通过日志过滤结果**还是通过源**过滤结果**。**
    *   **按日志**让你选择事件发生的一个或多个日志，如**系统**和**应用**。
    *   **按来源**让您选择创建了您想要过滤的事件的服务或应用。

6.  一旦您选择了上面的字段，其余字段的工作方式与普通过滤器类似。如果您知道想要在自定义视图中看到什么事件，您可以选择一个**事件 ID** 、一个**任务类别**和**关键字**。
7.  点击**确定**
8.  为您的自定义视图选择名称和描述。您还可以选择在导航树上存储自定义视图的位置，如果您有许多自定义视图，这将非常有用。
9.  点击**确定**。
10.  现在，您将在**自定义视图**文件夹(或您选择为其创建的任何文件夹)中看到您的自定义视图。只需从左侧窗格中选择它，即可在您的自定义视图中查看事件。

## 如何备份事件日志

如果您不知道如何调查特定的错误或需要更多帮助，您可以将事件日志保存到一个文件中，这样您就可以与可以从您的计算机上查看事件的其他人共享该文件。方法如下:

1.  打开**事件查看器**。
2.  导航到要导出的日志或自定义视图。
3.  在右侧的**动作**窗格中，选择**将所有事件另存为...**(用于日志)或**将自定义视图中的所有事件另存为...**
    *   或者，您可以手动选择特定事件，然后选择**保存所选事件**。

4.  选择文件的名称和位置，点击**保存**。
5.  然后，您可以将此文件发送给信任的人，这样他们就可以检查您的计算机可能发生了什么问题。

## 如何清除事件日志

大多数情况下，应该没有理由清除事件日志，但是如果您需要在驱动器上节省一些空间，您可以删除日志中的所有事件。我们不一定推荐这样做，但是如果你想这样做，这里有一些方法:

1.  打开**事件查看器**。
2.  展开左侧面板上的 **Windows 日志**选项。
3.  打开想要清除的日志(如**系统**，在**动作**窗格中选择**清除日志**。
4.  选择**清除**删除日志中的所有事件，或**保存并清除**如果您想在删除之前将事件备份到单独的文件中。

这就是你在 Windows 11 中使用事件查看器所需要知道的全部内容。正如你所看到的，有很多东西，弄清楚你通常使用的很棒的个人电脑或笔记本电脑发生了什么会非常有用。如果你想了解 Windows 11 的其他功能，请查看[如何使用 BitLocker](https://www.xda-developers.com/how-to-use-bitlocker-windows-11/) 或[如何定制 Windows 11](https://www.xda-developers.com/how-customize-windows-11/) ，如果你想调整你的体验。