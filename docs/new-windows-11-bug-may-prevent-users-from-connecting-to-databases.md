# 新的 Windows 11 错误可能会阻止用户使用 SQL Server 连接到数据库

> 原文：<https://www.xda-developers.com/new-windows-11-bug-may-prevent-users-from-connecting-to-databases/>

Windows 11 对错误和问题并不陌生，微软刚刚证实了用户在使用最新版本的操作系统时可能会遇到的另一个问题。在 11 月 8 日发布的针对版本 Windows 11 初始版本)和 22H2 的最新补丁星期二更新中发现，这个新问题可以阻止某些数据库连接工作。目前，没有已知的解决方法。

具体来说，微软表示，当通过 Micrososft ODBC SQL Server 驱动程序(sqlsrv32.dll)使用 Microsoft ODBC(开放式数据库连接)连接到数据库时，您可能会遇到问题。连接错误可能会导致错误消息，用户会看到“消息:[Microsoft][ODBC SQL Server 驱动程序 TDS 流中的协议错误”或“消息:[Microsoft][ODBC SQL Server 驱动程序]从 SQL Server 收到未知令牌”。

该问题最早出现在 Windows 11 build 22000.1219(针对运行版本 21H2 的用户)和 build 22621.819(针对版本 22H2)，目前尚未修复，即使在 11 月晚些时候发布了后续可选更新。

不幸的是，也没有解决方法。如果您遇到这个问题，除了等待修复问题的更新之外，您别无选择。你现在能做的就是检查你的应用程序是否受到了这个 bug 的影响。如果你遇到了数据库问题，并且不确定原因，你可以打开一个使用数据库的应用程序，然后启动命令提示符(或 Windows 终端)并键入*任务列表/m sqlsrv32.dll*。这将显示是否有任何任务正在使用导致问题的 SQL Server 驱动程序。

令人欣慰的是，微软表示正在努力解决这个问题，不久的将来应该会有一个解决方案。12 月的星期二补丁更新将于下周发布，所以希望修复程序将包括在内。请记住，这将是今年的最后一次更新，因为微软不会在 12 月发布其 C 或 D 可选更新，因为它会在假期期间发布。就在上周，[发现了另一个问题](https://www.xda-developers.com/windows-11-november-optional-update-task-manager-issue/)，由于显示不正确的颜色，可能会使任务管理器中的文本不可读，这也在等待修复。

* * *

**来源:** [微软](https://learn.microsoft.com/en-us/windows/release-health/status-windows-11-22h2#2970msgdesc)