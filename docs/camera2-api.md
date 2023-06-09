# 如何检查您的 Android 设备上是否启用了 Camera2 API

> 原文：<https://www.xda-developers.com/camera2-api/>

智能手机的硬件通常比软件默认允许的功能更多。这就是为什么谷歌摄像头端口在我们的论坛上变得非常受欢迎的确切原因，因为许多人认为它们是一种在各种设备上大幅提高图像质量的简单方法。通过移植的谷歌相机应用程序，你可以在非谷歌设备上使用谷歌卓越的 HDR+优化以及他们的肖像模式。然而，在阅读这些端口时，您一定遇到过一个特殊的术语——“camera 2 API”。在本教程中，您将了解该术语的实际含义，以及如何在您的 Android 手机上检查 Camera2 API 支持的状态。

* * *

## 什么是 Camera2 API？

手机上的物理摄像头模块是一个非常复杂的硬件，但 Android 不需要知道所有的底层参数来与之交互，这要归功于 SoC 供应商实现的摄像头硬件抽象层(HAL)。相机专用的应用程序编程接口(API)位于 HAL 之上，充当应用程序级的公共框架。简而言之，相机 API 允许应用程序以简化的方式探测设备上的相机功能，而不必担心相机传感器的细节。

谷歌在 Android 5.0 Lollipop 中引入了[相机 2 API](https://developer.android.com/reference/android/hardware/camera2/package-summary.html) ，作为原始[相机 API](https://developer.android.com/reference/android/hardware/Camera.html) 的继任者，以便更好地定义应用程序如何与连接到智能手机的各个相机进行交互。它向应用程序展示了许多精细的相机控制，包括高效的零拷贝突发/流流以及对曝光、增益、白平衡增益、颜色转换、去噪、锐化等的每帧控制。

Camera2 API 有五种不同的支持级别:

*   **传统:**不支持相机 API2 功能(如逐帧控制)的传统设备。这些设备通过相机 API2 接口向应用展示功能，这些功能与通过相机 API1 接口向应用展示的功能大致相同。
*   **受限:**这些设备仅支持所有摄像机 API2 功能的子集。
*   **完整:**这些设备支持 Camera API2 的所有主要功能，必须使用 Camera HAL 3.2 或更高版本以及 Android 5.0 或更高版本。
*   **Level_3:** 这些设备支持 YUV 再处理和 RAW 图像捕捉，以及基于完整 Camera2 API 支持的附加输出流配置。
*   **外部:**类似于有限的设备，但有一些例外(例如，一些传感器或镜头信息可能不会被报告，或者帧速率不太稳定)。该级别用于 USB 网络摄像头等外部摄像头。

对于大多数用户来说，你们都应该关心 Camera2 API 支持的原因是，谷歌相机端口有必要在智能手机上工作。

* * *

## 如何检查 Camera2 API 是否启用

兼容性测试套件(CTS)的[图像测试套件](https://source.android.com/compatibility/cts/camera-hal#its_tests)部分的网页声明，强烈建议运行 Android 9 或更高版本的[认证设备](https://www.xda-developers.com/check-phone-tablet-certified-android-before-buying/)使用 Camera2 API 支持 [Camera HAL3](https://source.android.com/devices/camera/camera3) 。也就是说，过去的许多设备都没有现成的 Camera2 API 支持。为了启用 API，其中一些需要 root 用户修改他们的 build.prop，或者只需要一个解锁的引导加载程序来运行特定于供应商的 Fastboot 命令。然而最近，事情开始发生变化。

要了解设备上 Camera2 API 支持的状态，请选择以下方法之一。

### 方法 1:使用亚行

在开始使用这种方法之前，请确保您可以访问安装了 [ADB 和 fast boot](https://www.xda-developers.com/install-adb-windows-macos-linux/)的 PC/Mac。

1.  在手机上，从开发人员选项中打开 USB 调试。
2.  将您的设备连接到 PC/Mac。
3.  打开命令提示符或 PowerShell (Windows)或终端窗口(macOS 或 Linux)。
    *   如果 ADB 二进制文件的位置没有在全局路径设置中定义，您必须将 shell 的工作目录更改为 ADB 二进制文件所在的位置。

4.  输入以下命令:

    ```
     adb shell "getprop | grep HAL3" 
    ```

5.  如果结果是下列之一:

    ```
     [persist.camera.HAL3.enabled]: [1] 
    ```

    ```
     [persist.vendor.camera.HAL3.enabled]: [1] 
    ```

    ，那么您的设备具有完全支持 Camera2 API 的 Camera HAL3。

* * *

### 方法 2:使用终端模拟器

如果你不想使用 PC/Mac，那么你可以使用任何终端模拟器应用程序直接从你的手机上检查 Camera2 API 的状态。

1.  下载您选择的终端模拟器应用程序。下面我们列举了几个比较受欢迎的。
2.  打开应用程序，输入以下命令:

    ```
     getprop | grep HAL3 
    ```

3.  如果结果是下列之一:

    ```
     [persist.camera.HAL3.enabled]: [1] 
    ```

    ```
     [persist.vendor.camera.HAL3.enabled]: [1] 
    ```

    ，那么您的设备具有完全支持 Camera2 API 的 Camera HAL3。

[app box Google play " jackpal . Android term "]

[appbox fdroid "com.termux"]

请记住，拥有 HAL3 支持并不意味着 Camera2 API 的所有功能都可用，因为公司仍然可以修改功能，如原始拍摄支持、ISO 级别、曝光时间等。这就是我们建议选择第三种方法的原因，因为它提供了更精细的信息。

* * *

### 方法 3:使用专用的第三方应用程序

不想摆弄命令行界面？然后只需从谷歌 Play 商店下载目标 Android 设备上的 Camera2 API Probe 应用程序。

[app box Google play " com . air beat . device . inspector "]

安装后，该应用程序将根据您设备的相机镜头数量显示两个或更多部分(例如，“相机 ID: 0”代表后置相机模块)。在每个相机 ID 下，您可以找到各种功能及其支持详细信息的子类别。我们对名为“硬件支持级别”的类别特别感兴趣，它显示了设备上的 Camera2 API 支持级别。

正如你所看到的，该应用程序不仅找出了你的设备的确切 Camera2 API 级别，还列出了相机模块支持的其他几个功能。在安装第三方相机应用程序时，这些信息可能会派上用场，比如可以利用这些功能的特定谷歌相机端口。

如果你想深入挖掘并发现更多关于支持的 Camera2(以及 CameraX)扩展的信息，试试由 XDA 公认的开发者 Zacharee1 开发的 [CameraX Info](https://www.xda-developers.com/camerax-info-list-camera2-extensions-database/) 。请注意，该应用程序仅列出了您的设备制造商向第三方应用程序公开的功能。它不应该用于枚举内置在原生相机应用程序中的功能。

* * *

我们希望您现在可以使用本指南快速发现您的设备上是否启用了 Camera2 API。请在评论中告诉我们你喜欢的方法！