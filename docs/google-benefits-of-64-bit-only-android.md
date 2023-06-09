# 谷歌解释了 Pixel 7 系列如何受益于 64 位技术

> 原文：<https://www.xda-developers.com/google-benefits-of-64-bit-only-android/>

在[谷歌 Pixel 7 和 Pixel 7 Pro](https://www.xda-developers.com/best-google-pixel-7-deals/) 发布后不久，[证实](https://www.xda-developers.com/google-pixel-7-64-bit-only-apps/)这两款手机是第一对仅支持 64 位应用的安卓手机。现在，谷歌也通过其 Android 开发者博客分享了这一消息，列出了这一做法的一些好处。

虽然我们之前报道过，但谷歌澄清说，在这种配置下，不再支持 32 位应用程序，这意味着没有 64 位库的旧版本软件将无法工作。这种变化带来了许多好处，其中最重要的一点是设备可以更高效地运行。通过转移到 64 位应用程序，应用程序现在可以运行得更快，因为“它们可以访问 32 位应用程序不可用的额外寄存器和指令。”

由于不支持 32 位应用程序，操作系统还可以通过释放高达 150MB 的 RAM 来受益，这意味着更少的应用程序死亡和更少的 jank。此外，针对运行 64 位代码而优化的 CPU 可以提供更大的能力，性能提升高达 25%。除了提高效率之外，您还可以获得安全优势，如地址空间布局随机化(ASLR)的效率提高，这有助于保护操作系统，以及“保护控制流完整性”的额外能力

就后端而言，开发人员还可以获得 64 位应用支持的好处，能够提供更快的更新，并获得像 [HWASan](https://source.android.com/docs/security/test/hwasan) 这样的内存错误检测工具，这比 ASan 效率高得多。谷歌确实警告应用程序开发者，他们在测试应用程序时可能需要更加注意，确保他们也是专门针对 64 位设备进行测试的。谷歌提供了[预发布报告](https://support.google.com/googleplay/android-developer/answer/9844487)来帮助这个过程。

谷歌 [Pixel 7](https://www.xda-developers.com/google-pixel-7-review/) 和 [Pixel 7 Pro](https://www.xda-developers.com/google-pixel-7-pro-review/) 是两款 Android 智能手机，是新事物的开始。展望未来，你可以期待看到更多的设备采用 64 位的方法。虽然很难说哪些公司会大幅降价，但据传谷歌的下一款硬件产品 Pixel 平板电脑是 64 位的。值得庆幸的是，作为消费者，你不必过于担心这一变化，因为谷歌早在 2017 年就已经为此做好了[基础](https://www.xda-developers.com/play-store-updated-requirements-api-level-64-bit/)工作，以确保平稳过渡。

 <picture>![The Pixel 7 packs the second-gen Tensor SoC, a brighter display, and improved cameras.](img/8b31c0e15e95c3f8bf719fbd3ebefc29.png)</picture> 

Google Pixel 7

##### 谷歌 Pixel 7 和 Pixel 7 Pro

Pixel 7 包含第二代 Tensor SoC、更亮的显示屏和改进的摄像头，以及新的照片取消模糊功能。

* * *

**来源** : [安卓开发者博客](https://android-developers.googleblog.com/2022/10/64-bit-only-devices.html)