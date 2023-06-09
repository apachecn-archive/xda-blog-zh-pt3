# 开发者现在可以使用 Android Jetpack 在应用中实现超宽带(UWB)支持

> 原文：<https://www.xda-developers.com/developers-ultra-wideband-uwb-android-jetpack/>

去年，谷歌在 AOSP 增加了一个新的 API 来更好地支持超宽带设备。当时，我们了解到该 API 仅限于系统应用，这意味着第三方应用无法访问它。这种情况现在终于改变了，因为开发人员可以通过新推出的 Jetpack 库在他们的应用程序中实现 UWB 支持。androidx.core.uwb Jetpack 库的 1.0.0-alpha 版本可用于应用程序中，与支持 uwb 的设备进行交互，如[谷歌 Pixel 6 Pro](https://www.xda-developers.com/google-pixel-6-pro-review/) 或三星 Galaxy S22 Plus 和 Ultra。

这意味着从现在开始，开发人员可以与运行他们应用程序的 Android 智能手机的 UWB 功能进行交互，而不再仅限于系统应用程序。目前，UWB API 要求设备运行 [Android 12](https://xda-developers.com/android-12) 或更新版本，尽管几乎所有拥有 UWB 的设备都可能已经运行了。UWB 可以利用低能量密度进行短程测量，并在大部分无线电频谱上执行高带宽信号传输。

苹果的空中标签利用了 UWB，这样你就可以用你的智能手机准确地定位它们，第一款支持 UWB 的现代智能手机是 iPhone 11。在 Android 方面，三星是第一个将这项技术推向市场的[,推出了 Galaxy Note 20 和 Note 20 Ultra 智能手机。小米还宣布了加入 UWB 技术的计划，展示了它如何利用该技术控制其智能家居生态系统。](https://www.xda-developers.com/tsamsung-galaxy-note-20-ultra-features-nfc-esim-uwb-tech-single-nxp-chip/)

至于为什么它作为 Android Jetpack 库发布，这是有原因的。鉴于谷歌每年的操作系统发布周期和 Google Play 不断变化的 API 要求，为 Android 开发可能是一件痛苦的事情，*这就是为什么我们看到谷歌在“Android Jetpack”的保护伞下维护一套支持库。它是一组 Android 组件、工具和指南，灵感来自支持库的向后兼容性和 Android 架构组件的易用性。*

考虑到 UWB 库是在 alpha 中，它可能还没有开发人员想要的所有功能。开发人员应该确保通读这个新库的开发人员文档，以确保他们了解如何使用它。

*感谢米莎尔·拉赫曼的提示！*

* * *

**来源: [Android 开发者文档](https://developer.android.com/guide/topics/connectivity/uwb)、 [Jetpack 库](https://developer.android.com/jetpack/androidx/releases/core-uwb)、**

**Via: [米沙·拉赫曼](https://twitter.com/MishaalRahman/status/1532114919746785280)**