# 开发者将 Android TV 13 带入树莓 Pi 4

> 原文：<https://www.xda-developers.com/raspberry-pi-4-android-tv-13-custom-rom/>

通过附加一个[安卓电视盒子或棒](https://www.xda-developers.com/best-android-tv-box/)，很容易让一台旧的“哑”电视变得焕然一新，但当你只是为自己的 DIY 项目准备一个树莓派时，事情就没那么简单了。即使家酿修补旗手使用与大多数 Android 设备相同的 ARM 架构，将 Android 移植到 Pi 一直是一个棘手的过程。尽管如此，XDA 资深成员 [KonstaT](https://forum.xda-developers.com/m/konstat.7223862/) 一直负责为流行的信用卡大小的计算机编译 Android，他的最新努力现在是将 Android TV 13 与 Raspberry Pi 4 相结合。

这款用于树莓 Pi 的 Android TV 13 构建基于 LineageOS 20 代码库，并包括 2022 年 11 月的最新安全补丁。这里的一个主要好处是，这个版本也与 Raspberry Pi 400 兼容，这是一个完全成熟的紧凑型 PC，所有这些都包含在一个迷你键盘形状因素中。计算模块 4 也可以运行该端口，尽管您应该至少选择 2GB RAM 版本，并将其连接到合适的载板以运行操作系统。

与[之前的 Android 13 端口](https://www.xda-developers.com/raspberry-pi-4-b-pi-400-compute-model-4-android-13-port/) by *KonstaT* 不同，ROM 在电视模式下运行 Android，而不是作为典型的平板电脑界面。这可能更适合 Raspberry Pi，因为在与外部 GPIO IR 模块配对后，您可以使用标准的 IR 遥控器从您的沙发上导航 UI。

值得注意的是，超级用户可以从外部 USB 存储介质引导 ROM。可以通过转至`/boot/config.txt`来设置参数。ROM 的论坛线程说，硬件加速视频播放目前缺失。此外，你不能使用 Chromecast，因为它不是谷歌认证的端口。不过，这些构建与 Android TV 兼容的 [Gapps 包](https://www.xda-developers.com/download-google-apps-gapps/)一起工作，所以如果需要的话，你可以访问 Play Store。

Raspberry Pi 4 上的 Android TV 13 并不是这里唯一的壮举，因为开发者还为微型 ARM 驱动的 PC 编译了非官方的 LineageOS 20 版本。如果你想了解更多，或者在你自己的 Raspberry Pi 上尝试一个 ROM 版本，请查看下面的论坛主题链接。

**[下载 Android TV 13 端口为树莓 Pi 4 型号 B，Pi 400，计算模块 4](https://forum.xda-developers.com/t/4516545/)**