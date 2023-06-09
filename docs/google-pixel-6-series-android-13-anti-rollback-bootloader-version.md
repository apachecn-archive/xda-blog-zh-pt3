# 如何在谷歌 Pixel 6 系列上查看 Android 13 bootloader 版本

> 原文：<https://www.xda-developers.com/google-pixel-6-series-android-13-anti-rollback-bootloader-version/>

Android 13 季正式来临。Android 的最新版本带来了一些新的用户界面变化和许多有用的功能。对于谷歌 Pixel 6 家族，稳定的 Android 13 更新也[在这些设备的引导加载器中增加了防回滚版本](https://www.xda-developers.com/android-13-downgrade-protection-pixel-6-series/)。因此，升级到 Android 13 后，您无法闪回旧的 Android 12 版本。

*   Pixel 6 系列设备已经通过稳定的 Android 13 OTA 接收了新的 bootloader 更新。
*   引导加载程序更新增加了这些手机上的防回滚版本。
*   由于防回滚保护，恢复到 Android 12 是不可能的。

**浏览这篇文章:**

## 为什么我的谷歌 Pixel 6/6 Pro/6a 需要升级 bootloader？

Google Pixel 6、 [Pixel 6 Pro](https://www.xda-developers.com/google-pixel-6-pro-review/) 和 [Pixel 6a](https://www.xda-developers.com/google-pixel-6a-review/) 上的[回滚保护](https://source.android.com/docs/security/verifiedboot/verified-boot#rollback-protection)是通过电子保险丝(eFuses)实现的。eFuse 类似于一次性写入闪存。一旦你通过写东西来翻转这些位，就没有回头路了。在“烧断”一个 eFuse 之后，它将永远保持写入该值。

为了消除一些攻击媒介，谷歌通过稳定的 Android 13 OTA 为第六代 Pixel 手机提供了一套新的引导加载程序，防止旧版本的 Android 被加载到这些设备上。只有在成功启动 Android 13 后，相关的 eFuse 才会熔断并增加回滚索引。新的引导加载程序版本、提升的回滚索引值和熔断的 eFuse 状态应该足以阻止任何 Android 13 之前的固件随后被刷新。

* * *

## 如何判断我的 Google Pixel 6/6 Pro/6a 是否已经有了更新的 bootloader？

根据定义，引导加载程序是一个加载操作系统的程序，或者在设备打开时连锁加载另一个引导加载程序。Google 的 Fastboot 实用程序提供了一种从计算机上查询 Android 设备的 bootloader 变量的简单方法。为此，我们需要将目标 Pixel 手机引导至其引导加载程序接口。

1.  确保您的 PC/Mac/Chromebook 上安装了最新版本的 ADB 和 Fastboot 实用程序。
2.  在你的手机上，进入**设置** > **关于手机** > **内部版本号**点击这个条目 7 次来启用**开发者选项**。
3.  启用后，返回主设置页面并点击**系统**，然后进入**开发者选项**。
4.  打开 **USB 调试**。
5.  使用 USB 电缆将 Pixel 6、Pixel 6 Pro 或 Pixel 6a 连接到电脑。
6.  打开终端窗口，键入以下命令，检查是否检测到您的设备:

    ```
     adb devices 
    ```

    您可能需要首次验证主机的身份。
7.  如果设备已连接，您应该可以看到它的序列号。
8.  一切准备就绪后，运行以下命令重新引导至引导加载程序模式:

    ```
     adb reboot bootloader 
    ```

9.  您的手机应该重新启动到引导模式(也称为“快速启动模式”)。
10.  现在，输入下面的命令来检查你的电脑是否在引导模式下检测到目标设备:

    ```
     fastboot devices 
    ```

    如果你在电脑上使用 Windows，那么你可能需要[安装最新的谷歌 USB 驱动](https://www.xda-developers.com/download-android-usb-drivers/)。
11.  要知道 bootloader 版本，执行下面提到的命令:

    ```
     fastboot getvar version-bootloader 
    ```

    [](https://www.xda-developers.com/google-pixel-6-series-android-13-anti-rollback-bootloader-version/fastboot-getvar-version-bootloader/)

接下来，参考下表，将引导加载程序版本与您得到的输出进行匹配:

也可以从用户空间快速引导接口(又名 fastbootd)查询引导装载程序版本。为此，使用`adb reboot fastboot`重启设备，然后执行相同的`fastboot getvar version-bootloader`命令。

如果你附近没有电脑，那么你可以直接从手机上获取引导程序版本。首先，关闭谷歌 Pixel 6/6 Pro/6a，并按下音量和电源按钮几秒钟。当快速启动模式出现时释放它们。您应该能够在屏幕上找到引导程序版本。

对于命令行爱好者，在手机上的终端模拟器应用程序中使用以下命令来获取引导加载程序版本:

```
 getprop ro.bootloader 
```

* * *

## 它说我有一个不同的 bootloader 版本，那么这是否意味着我可以回到 Android 12？

如果你的 Pixel 6/6 Pro/6a 的 bootloader 版本与上述表格中显示的版本不同，那么你可能正在运行 Android 13 的测试版或 Android 12 的旧稳定渠道版。

虽然您可以尝试使用较低版本的引导程序恢复到 Android 12，但不建议这样做。出于安全和兼容性的考虑，您应该使用稳定的 Android 13 OTA 来升级引导程序以及您设备的底层固件位。

如果你计划执行手动刷新，那么确保稳定的 Android 13 软件的分区映像被刷新到两个插槽。 **A 和 B 插槽之间的引导加载程序版本不匹配足以阻塞设备**。目前**还没有已知的方法来恢复像谷歌 Pixel 6/6 Pro/6a 这样的硬砖谷歌张量驱动设备**，所以在手动升级之前要小心谨慎。

* * *

## 如何安全升级我的 Google Pixel 6/6 Pro/6a 上的 bootloader？

为了避免硬砖的情况，你应该在成功更新并引导到 Android 13 至少一次后，将引导加载程序分区刷新到非活动插槽。这应该消除了版本不匹配的可能性，特别是如果你第一次使用稳定的 Android 13 版本更新 Pixel 6、Pixel 6 Pro 或 Pixel 6a。

### 选项 1(使用恢复/OTA 映像):

成功引导至 Android 13 后，[下载与该版本对应的完整 OTA 映像](https://www.xda-developers.com/how-to-download-android-13/)。接下来，[从 stock recovery](https://www.xda-developers.com/how-to-install-android-13/#method1) 中将其侧装，并重新启动设备，以确保两个插槽具有相同的引导加载程序版本。

### 选项 2(使用工厂映像):

解锁 bootloader 后通过刷新出厂镜像升级到 Android 13 的人应该选择这个选项。第一次成功开机进入 Android 13 后，

1.  检查当前活动插槽:`adb reboot bootloaderfastboot getvar current-slot`如果输出将当前插槽返回为“a”，则您的活动插槽应为“a”，另一个插槽为“b”。如果不是，则您的活动插槽为“b”，另一个插槽为“a”
2.  提取工厂映像 ZIP 文件的内容，并在提取的文件中找到引导加载程序映像。应该命名为“boot loader-[设备代号]-[平台代号]-[主版本]-[次版本].img。”
    *   对于 Pixel 6 和 6 Pro，平台代号是“slider”，而对于 Pixel 6a，则是“bluejay”。[](https://www.xda-developers.com/google-pixel-6-series-android-13-anti-rollback-bootloader-version/google-pixel-6-series-factory-firmware-bootloader-image/)
3.  现在，我们需要刷新两个插槽的引导加载程序。
    1.  如果您的活动插槽是“a”`fastboot --slot=other flash bootloader bootloader_filename.imgfastboot set_active bfastboot reboot bootloaderfastboot set_active afastboot reboot bootloaderfastboot reboot`
    2.  如果您的活动插槽是“b”`fastboot --slot=other flash bootloader bootloader_filename.imgfastboot set_active afastboot reboot bootloaderfastboot set_active bfastboot reboot bootloaderfastboot reboot`
4.  仅此而已。

* * *

正如你所看到的，有很多不同的方法可以检查 Pixel 6、6 Pro 或 6a 的底层引导程序版本。如果您希望让系统自行处理或手动安装更新的引导程序，请选择最符合您需求的方法。