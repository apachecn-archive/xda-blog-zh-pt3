# 如何将 Magisk 安装到 Root 或定制您的 Android 手机

> 原文：<https://www.xda-developers.com/how-to-install-magisk/>

如果你曾经想过对你的手机进行改造，或者对它的某些方面进行改造，那么你很可能听说过 Magisk。但是 Magisk 是什么？Magisk 是一个可以用来在你的设备上获得 root 访问权限的工具，类似于 SuperSU，但并不仅限于此。Magisk 是由的论坛的资深开发人员开发的，Magisk 是一个可以在你的 Android 手机上进行各种修改的门户网站。您可以在手机上安装几个 Magisk 模块，用于不同的用途。

有用于主题化的模块，[广告拦截器](https://www.xda-developers.com/block-ads-on-android/)，启用 Camera2API，以及许多其他系统级的修改，否则你无法完成。如果你是一个超级用户，想要扩展手机的功能并将其推向极限，你需要试试 Magisk。如果这些听起来对你来说很有趣，我们将告诉你如何在你的 Android 设备上安装 Magisk 来定制它，并在你的手机上做你从未想过要做的事情。

## 如何安装 Magisk

安装 Magisk 需要您有一个自定义恢复，为此您的手机需要有一个解锁的引导加载程序。如果你已经解锁了手机上的引导程序，你就可以开始了。如果你没有，也不知道我们在谈论什么，我们建议你去 XDA 论坛[搜索你的设备，然后寻找解锁引导程序的指南。没有通用的方法，因为每个手机都不一样。一旦你解锁了引导程序，你就可以继续了。](https://forum.xda-developers.com/)

免责声明:解锁引导程序将会擦除您智能手机上的所有数据，在某些情况下，甚至可能会使您的保修无效。在执行这些步骤之前，建议[备份所有数据](https://www.xda-developers.com/how-to-backup-android/)。同样重要的是要明白，不正确地遵循这些步骤可能会导致手机死机，所以请确保您知道如何将您的手机恢复到原始状态，以防您最终遇到这种情况。

此外，Magisk 可能会导致一些银行和支付相关的应用程序出现问题，因此如果这些对您来说绝对重要，请谨慎操作。

在我们开始之前，请确保您可以访问安装了 [ADB 和 Fastboot](https://www.xda-developers.com/install-adb-windows-macos-linux/) 的 PC/Mac。

### 步骤 1:识别启动映像包的类型

从项目的 GitHub 库下载最新版本的 Magisk 应用[。由于 Magisk 的 APK 位于谷歌 Play 商店之外，你可能需要先允许从未知来源下载应用程序，然后](https://github.com/topjohnwu/Magisk/releases/latest)[手动安装下载的软件包](https://www.xda-developers.com/how-to-sideload-install-android-app-apk/)。

安装后，打开 Magisk 应用程序。您应该会看到这样的屏幕:

现在，我们需要记下以下参数的值:

### 步骤 2:定位启动映像包

为了给你的设备打补丁，你需要从官方的固件包中提取它。如果你使用的是像[linegeos](https://www.xda-developers.com/five-reasons-xda-loves-lineageos/)这样的定制 ROM，闪存 ZIP 文件包含启动映像。

**第一种情况:您可以访问可恢复的闪存 ZIP 文件**

如果您的设备仍然使用 A-only 分区方案，您可以在可恢复的 flash ZIP 文件中找到“boot.img”。只需使用合适的归档程序提取它。

![POCO M3 boot.img inside recovery ZIP](img/64fa365955841be58b9716cbd9b08cb5.png)

请注意 POCO M3 的恢复 ZIP 中的 boot.img 文件。

但是，如果您的设备使用 A/B 分区方案，那么引导映像和其他分区映像会进一步打包在名为 *payload.bin* 的文件中，如下所示。

![Google Pixel 5 payload.bin inside recovery ZIP](img/cf3e0a815110f6ae5e7c6f242667d450.png)

Google Pixel 5 的恢复 ZIP 包含一个 payload.bin 文件。在这种情况下，您必须首先提取 payload.bin 文件，然后使用一个社区开发的 payload.bin 解包器从其中取出 boot.img。我们强烈建议您选择

[extractor written in Go](https://forum.xda-developers.com/t/tool-a-quick-android-ota-payload-dumper.4173271/)

因为它是跨平台的

[actively developed](https://github.com/ssut/payload-dumper-go)

.

这个分支被称为“payload-dumper-go ”,它甚至允许最终用户提取单个分区映像，而无需打开整个 payload.bin，这对于这个使用场景特别有用。

**第二种情况:您可以访问快速启动可闪存映像**

谷歌和小米等少数原始设备制造商为他们的设备提供快速启动可刷新的工厂图像。如果您设法获得了这样一个包，那么可以很容易地从归档中提取原始的 boot.img。

**特例:三星**

三星 Galaxy 设备没有传统的快速启动接口，因此它们的出厂映像打包方式不同。

1.  使用[三星固件下载器](https://www.xda-developers.com/download-samsung-software-updates-samsung-firmware-downloader/)为您的型号下载出厂映像。
2.  解压缩解密的包，并在您的设备上找到 AP tar 文件。它通常被命名为 AP _[设备型号软件版本].tar.md5。

### 步骤 3:修补启动映像包

现在我们已经有了启动映像，我们应该继续打补丁了。

**情况一:参数“Ramdisk”的值为“Yes”**

*   将启动映像复制到您的设备。事实上，您可以在不同于目标设备的其他 Android 设备上对其进行修补，但您也需要在辅助设备上安装 Magisk 应用程序。
*   按下 Magisk 卡上的*安装*按钮。
*   选择*选择*方法*下的一个文件*，选择股票引导镜像。

*   Magisk 应用程序会将映像修补到*[内部存储]/Download/Magisk _ patched _[random _ strings]。img* 。

请记住，可以通过像 [TWRP](https://www.xda-developers.com/how-to-install-twrp/) 这样的定制恢复，在具有 boot ramdisk 的传统设备上动态修补启动映像，但这种方法在现代设备上不再被推荐。话虽如此，如果你有一部旧手机，并想坚持定制回收路线，步骤如下:

*   下载 Magisk APK。
*   重命名。APK 文件扩展名为。ZIP(例如 Magisk-v 23.0 . apk→Magisk-v 23.0 . ZIP)。
*   Flash 压缩文件就像任何其他普通的可 flash 压缩文件。

*   请注意，模块的 sepolicy.rule 文件可能存储在缓存分区中，因此**不会清除它**。
*   检查是否安装了 Magisk 应用程序。如果没有自动安装，请手动安装 APK。

**情况二:参数“Ramdisk”的值为“否”**

在这种情况下，您需要从设备的出厂映像中找到 recovery.img 文件，而不是 boot.img 文件。这是因为 Magisk 需要安装在恢复分区中，这意味着每次您想要访问 Magisk 时都必须重新启动到恢复模式。

在这个阶段，有三种可能的情况:

*   正常加电:你最终将没有 Magisk。
*   恢复键组合→闪屏→释放所有按钮:系统应该用 Magisk 启动。
*   恢复键组合→闪屏→持续按音量键:进入纸张恢复模式

**特例:三星**

### 第四步:验证

最后一步是验证一切工作正常。找到新安装的 Magisk 应用程序并打开它。我们希望在“Installed”参数旁边看到一个版本号。这意味着您已经成功安装了 Magisk。干得好！

现在您已经安装了 Magisk，是时候尝试一些不错的 Magisk 模块了。你可以找到许多用于特定目的的模块，而且由于 Magisk 给你[根访问](https://www.xda-developers.com/root/)，你甚至可以为根设备安装一些最好的应用程序。因此，安装你喜欢的任何应用程序和模块，并得到调整！