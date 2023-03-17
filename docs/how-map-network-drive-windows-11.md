# 如何在 Windows 11 上映射网络驱动器

> 原文：<https://www.xda-developers.com/how-map-network-drive-windows-11/>

当你在一个安全的共享网络上时，只要你有那台电脑的地址和你想要的文件夹，就可以访问网络上其他电脑上的文件和文件夹。然而，每次都要记住要使用的确切地址似乎令人生畏。幸运的是，你可以在 [Windows 11](https://www.xda-developers.com/windows-11/) 上映射一个网络驱动器，以便在你需要的时候更容易访问。我们将向您展示如何做到这一点。

当然，在这之前，你需要确保你的电脑在网络上是可被发现的。如果你在一个安全的网络上，这应该是默认设置，但是如果这个选项被禁用，我们也会告诉你如何做。

## 步骤 1:设置专用网络

Windows 11 上的专用网络会自动启用网络发现，但默认情况下大多数网络都标记为公共网络，以避免将您的计算机暴露给不受信任的用户。启用网络发现的理想方法是将您的网络设置为专用网络。虽然这是可能的，但不建议**为公共网络启用网络发现。你需要做的是:**

 **1.  右击任务栏右侧的互联网图标，选择**网络&互联网设置**。
2.  检查顶部的**属性**按钮是否显示**专用网络**。如果没有，请单击它。
3.  在**网络配置文件类型**下，确保选择了**专用网络**。请确保这是一个安全的网络，并且您信任连接到它的所有设备。

您需要为要连接的设备和用来连接的设备执行此操作。

## 步骤 2:确保网络发现和文件共享已启用

这应该足够了，但是如果您想确保网络发现已启用，请按照以下步骤操作:

1.  右键单击任务栏右侧的互联网图标，选择**网络&互联网设置**。
2.  点击**高级网络设置**。
3.  选择**高级共享设置**。
4.  确保**网络发现**已启用。如果不是，请单击右边的复选框。
5.  此外，确保在主机 PC(存储共享文件夹的位置)上启用了**文件和打印机共享**选项。

这样，您应该能够访问网络上的共享文件夹。默认情况下，这将要求使用存储共享文件夹的 PC 上的用户帐户进行身份验证。如果它有不同的帐户，您需要与网络上的所有用户共享文件夹，以使其可以访问。

## 步骤 3:在 Windows 11 上映射网络驱动器

网络共享启动并运行后，您可以映射网络驱动器以链接到共享文件夹。请遵循以下步骤:

1.  打开**文件浏览器**。
2.  使用左侧的导航窗格导航到**这台电脑**。
3.  点击**...顶部工具栏中的**(省略号)图标，选择**映射网络驱动器**。
4.  给驱动器分配一个盘符(可以是你电脑上没有分配的任何盘符)，然后点击**浏览**。
5.  选择要映射到网络驱动器的文件夹，然后单击**确定**。
6.  如果您希望每次登录时都连接到共享文件夹，请确保启用了**登录时重新连接**选项。
7.  点击**完成**。
8.  现在，您将在“这台电脑”页面的文件资源管理器中看到共享文件夹。

完成后，您现在可以快速访问映射为网络驱动器的文件夹。这使得从您的 PC 快速访问共享文件变得更加容易，而无需实际访问主机。如果您不再需要访问网络驱动器，您可以通过右键单击该驱动器并选择**断开**来断开连接。

如果您正在寻找其他 Windows 11 提示，请查看[如何在 Windows 11 版本 22H2 上使用智能应用程序控制](https://www.xda-developers.com/how-to-use-smart-app-control-windows-11-2022-update-version-22h2/)，或者[如何使用 Windows 11 中的事件查看器](https://www.xda-developers.com/how-use-event-viewer-windows-11/)来检查您电脑上的潜在错误。**