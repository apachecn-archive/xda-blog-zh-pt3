# 新的 Windows 11 测试版修补了任务管理器和搜索框的一些错误

> 原文：<https://www.xda-developers.com/new-windows-11-beta-builds-fixes-bugs-task-manager-search-box/>

# 新的 Windows 11 测试版修补了任务管理器和搜索框的一些错误

尽管本周的 Windows 11 测试版规模较小，但微软已经修补了任务管理器和搜索框的几个问题。

微软发布了两个新的 Windows 11 beta 通道版本。有**构建 22623.1250** 给那些推出新功能的人，然后**构建 22621.1250** 给那些默认关闭新功能的人。这些没有带来任何重要的功能，第二次构建(为那些有新功能的人)专注于任务栏、任务管理器和搜索的错误修复。

首先从两个版本的**变化开始，你只需要知道一个。微软表示，它正在为 it 管理员增加一项新政策，以管理任务栏上的搜索框在他们的组织中的显示方式。新的 ConfigureSearchOnTaskBarMode 策略可以隐藏任务栏上的搜索、仅隐藏搜索图标、隐藏搜索图标和标签，或者显示搜索框。如果没有这些策略，Windows 将被设置为默认值，用户可以自行更改设置。如果你好奇的话，微软在另一篇博客文章中谈到了这一点。**

对于版本 22623.1250 中的**变化，你可以查看下面的完整日志。基本上，这些都是针对一些问题的补丁，比如讲述人不起作用，在搜索框周围拖动窗口，文本缩放，或者搜索框直接消失。**

*   现在，在搜索框中键入 F 应该又可以工作了。
*   修正了一个问题，讲述人没有读出对话框中的一些文本。
*   使用搜索框区域拖动窗口现在应该可以工作了(就像标题栏的其他区域一样)。
*   如果您进行搜索，然后按下向下箭头，键盘焦点现在应该从搜索框移到结果中。
*   修正了一个在细节标签中结束进程不显示确认对话框的问题。
*   增加文本缩放比例不再会导致“查看更多”按钮没有内容出现。
*   修复了一个问题，焦点可能不会正确设置为搜索，导致讲述人没有说焦点是在搜索框上。
*   如果您启用了一个对比主题，并选择了 Processes 页面中的一行，该行现在应该显示它已被选中。
*   修正了当你点击搜索框时，搜索框会随机消失的问题(在任务栏上留下一个空白)。
*   修正了当你点击搜索框时，搜索框会轻微向一侧移动的问题。
*   如果您将任务栏设置为自动隐藏，然后按 Windows 键并开始键入，任务栏应该不会再意外隐藏。

这就是本周关于 beta 频道建设的所有信息。如果你运行的是 Windows 11，并且有一台电脑注册了 Dev 频道，那么你可以在本周早些时候下载一个版本。该版本提供了新的 Spotify 和 Phone Link 小工具。

**来源:** [微软](https://blogs.windows.com/windows-insider/2023/02/02/announcing-windows-11-insider-preview-build-22621-1250-and-22623-1250/)