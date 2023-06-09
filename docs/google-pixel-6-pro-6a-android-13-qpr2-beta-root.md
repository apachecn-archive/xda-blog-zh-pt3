# 如何用 Magisk 谷歌 Pixel 6，6 Pro，和运行 Android 13 QPR2 Beta 的 Pixel 6a

> 原文：<https://www.xda-developers.com/google-pixel-6-pro-6a-android-13-qpr2-beta-root/>

当谷歌启动了 Android 13 第二季度平台发布(通常被称为 QPR2)的测试计划时，许多爱好者认为在这些版本上实现 root 就像在稳定的渠道固件上实现 root 一样容易，但事实证明并非如此。准确地说，涉及使用 Magisk 修补启动映像的[通用根向导](https://www.xda-developers.com/root/)对谷歌 Pixel 6 系列不再有效。如果您有 Pixel 6、6 Pro 或 Pixel 6a，Magisk 的 stable 或 Canary 版本都无法为 QPR2 beta 版本上的超级用户访问生成有效的修补启动映像。但是解决这个谜题似乎是一个时间问题，而不是如果的问题，Android 修改场景已经找到了一个聪明的方法，通过借用 [Pixel 7](https://www.xda-developers.com/google-pixel-7-pro-review/) 的一些位来为运行 Android 13 QPR2 beta 的 Pixel 6 阵容提供基础。

对于正在阅读这篇文章的人来说，你可能对 root 有好感。毕竟，由于 root 权限，你能够[在系统范围内阻止广告，调整内核参数](https://www.xda-developers.com/best-android-root-apps/)，或者完全放弃定制 ROM 的需要，这要感谢通过 [Magisk 模块](https://www.xda-developers.com/best-magisk-modules/)和 [Xposed 框架](https://www.xda-developers.com/best-xposed-modules/)提供的无数定制。也就是说，考虑到 Android 和 OEM 皮肤的成熟度，root 访问对普通用户来说毫无意义。对于运营商和设备制造商来说，root 访问实际上是一个令人头疼的问题，它阻止这些公司将你的手机锁定在他们的应用和服务生态系统中。但归根结底，这是 XDA，这意味着尽管获得 root 访问权对消费者来说是一场失败的战斗，但修改社区不会停止。

不用说，售后市场的发展似乎进展顺利。事实上，一些用户已经证实了一种有趣的 *frankenbuild* 方法的存在，这种方法可以让这些手机基于 Android 13 的最新测试版。Pixel 家族逐渐转向[通用内核映像](https://www.xda-developers.com/google-generic-kernel-image/)在这一发现中发挥了关键作用，而两代张量芯片组之间的相似性使得完成这一命运成为可能。简而言之，仍然可以根运行 Android 13 QPR2 测试版的谷歌 Pixel 6 阵容，但这个过程需要一些额外的步骤。

## init_boot 崛起

为了在 Android 设备上进行 root 访问，需要在引导时启动超级用户可执行文件和 su 守护程序。在 Marshmallow 之前，这是通过修改/system 分区来实现的，以便在 init 中包含引导时实现 root 访问所需的脚本。由于 device-mapper-verity (dm-verity)的引入，Google 基本上消除了修改/system 的可能性，这导致了“无系统”的根方法。Magisk 是最受欢迎的超级用户权限提供程序，它为目标设备的普通引导映像打补丁。然后，如果设备的引导加载程序被解锁以允许修改二进制文件，您可以刷新修补后的引导映像以获得 root 访问权限。

对于使用 Android 13 启动的设备，通用 ramdisk 将从引导映像中移除，并放在一个单独的 init_boot 分区中。例如，在 Google Pixel 7 系列上，你必须用 Magisk 为 stock init_boot 映像打补丁以获得 root 访问权限。然而，Pixel 6 系列没有 init_boot 分区，因为它们是在 Android 12 中推出的。

## 利用 GKI 生根

请记住，使用内核版本 5.10 或更高版本启动的设备必须附带 GKI 内核，以符合 [GKI 2.0 规范](https://source.android.com/docs/core/architecture/kernel/generic-kernel-image#gki2)。因此，Pixel 6、6 Pro 和 6a 的引导映像包含通用 ramdisk 和 GKI 内核。

虽然我们还不知道 Magisk 和谷歌 Pixel 6 家族的 QPR2 beta 启动映像之间不兼容的确切原因，但似乎**你可以使用 Pixel 7 系列的补丁启动映像来根化它们**。这种奇怪的现象实际上是可能的，因为:

1.  由于内部相似性，对应于驱动像素 6 的第一代张量和像素 7 的张量 G2 的核源共享相当多的公共比特。
2.  如果在带有兼容引导加载程序的传统 SAR A-only 设备上没有 OEM 提供的通用 ramdisk，Magisk [会在修补引导映像时添加一个基本的通用 ramdisk](https://github.com/topjohnwu/Magisk/commit/985249c3d0bccff479f8c1efd5967922ab8d855e) ，以便在引导模式下可以访问 Magisk 接口。这个修复也适用于一些 Android 13 GKIs，如 Pixel 6 系列，需要[一个额外的 ramdisk 压缩格式修复](https://github.com/topjohnwu/Magisk/issues/5819)。似乎没有 ramdisk 的兼容启动映像(如 Pixel 7 系列中的映像)最终可以转换为 Pixel 6 系列，使用 Magisk 手动添加的工作通用 ramdisk。

## 如何用 Magisk 运行 Android 13 QPR2 beta 的 Google Pixel 6 系列

确保您的 Pixel 6/6 Pro/6a 具有解锁的引导加载程序，以便您可以引导修改后的引导映像。重申一下，**你需要修补 Pixel 7 的启动映像，Magisk 才能工作**。最简单的方法是事先从工厂映像中提取谷歌 Pixel 7 的股票启动映像，并使用 Magisk 应用程序对其进行修补。

1.  在您的 PC/Mac 上，下载与安装在 Pixel 6/6 Pro/6a 上的 QPR2 测试版相对应的 Pixel 7 或 Pixel 7 Pro 的工厂图像。在我们的测试中，我们在 Pixel 6a 上运行 QPR2 Beta 2 (T2B2.221216.006)构建，因此 Pixel 7 的相同 Beta 应该足够了。
2.  使用您最喜欢的档案管理器打开工厂图像，找到图像- <device codename="">- <build number="">。zip 文件，并从中提取 boot.img 文件。</build></device>
3.  使用 Magisk 修补启动映像，但不要刷新它。
    *   虽然推荐使用 Magisk 的最新稳定版本(在撰写本文时是 [v25.2](https://www.xda-developers.com/magisk-25-2-release-rust-logging/) ，但是您也可以选择最新的 [Canary build](https://raw.githubusercontent.com/topjohnwu/magisk-files/canary/app-release.apk) 。
    *   启动映像可以在任何 Android 设备上打补丁——你不一定需要在 Pixel 6 或 Pixel 7 上执行该任务。

4.  将 Magisk 修补的启动映像从手机复制到 PC/Mac，并将其重命名为 magisk_patched_boot.img。
5.  如果 USB 调试打开，将 Pixel 6 (/6 Pro/6a)重新启动到引导加载程序模式:

    ```
     adb reboot bootloader 
    ```

6.  刷新补丁启动图像，重启手机。

    ```
     fastboot flash boot /path/to/magisk_patched_boot.img
    fastboot reboot 
    ```

7.  打开 Magisk 应用程序，您的 Pixel 6/6 Pro/6a 应该显示为 rooted。

我们可以确认，Pixel 7 和 Pixel 7 Pro 的补丁启动映像可以在 vanilla Pixel 6 上互换使用，在 6 Pro 和 6a 上也是如此。

**XDA 论坛:[谷歌像素 6](https://forum.xda-developers.com/f/google-pixel-6.12311/) || [像素 6 Pro](https://forum.xda-developers.com/f/google-pixel-6-pro.12313/) || [像素 6a](https://forum.xda-developers.com/f/google-pixel-6a.12605/) || [像素 7](https://forum.xda-developers.com/f/google-pixel-7.12607/) || [像素 7 Pro](https://forum.xda-developers.com/f/google-pixel-7-pro.12609/)**

到目前为止，我们论坛上的多个用户报告称，他们已经使用这种方法成功地对运行 Android 13 QPR2 beta 的 Pixel 6、6 Pro 和 6a 进行了 rooted。然而，根过程的本质本身有点挑剔，而且你不能再通过 OTA 安装更新的测试版。尽管如此，如果你拥有一台 Pixel 6 系列设备，并希望在 beta 通道上获得 root 访问权限，这似乎是实现它的唯一途径。

一定要试一试，让我们知道它是否对你有效！