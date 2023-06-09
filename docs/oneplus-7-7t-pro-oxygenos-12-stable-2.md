# 一加 7 和 7T 系列获得另一个稳定的 OxygenOS 12 更新

> 原文：<https://www.xda-developers.com/oneplus-7-7t-pro-oxygenos-12-stable-2/>

经过长时间的中断，一加[在本月早些时候为一加 7 和一加 7T 系列推出了第一个稳定的 OxygenOS 12 更新](https://www.xda-developers.com/oneplus-7-7t-pro-android-12-oxygenos-12-stable/)。这次更新带来了谷歌在 Android 12 中引入的所有新功能，以及一加自己的一些新功能。有趣的是，一加 7、一加 7 Pro、一加 7T 和一加 7T Pro 的第一次 OxygenOS 12 稳定更新仅适用于印度版本，这让许多用户不满。一加现在在稳定频道上发布了一个新的更新。

一加在其社区论坛的最近帖子中宣布推出，并透露由于网络问题，它决定不在其他地区推出之前的版本。因此，一加 7 和一加 7T 系列的最新 OxygenOS 12 稳定更新(MP2)将是欧盟和全球变型的首次更新。

此次更新包含了之前版本中提供的所有更改，以及一些系统稳定性改进和通信稳定性优化。与之前的版本一样，最新版本包含了 2022 年 8 月的 Android 安全补丁。

一加还为所有地区提供了回滚版本，以帮助用户在遇到任何问题时恢复到 OxygenOS 11。此外，该公司还为所有变体提供了最新的 OxygenOS 11 包，以帮助用户在回滚后恢复丢失的应用程序。您可以从下面链接的公告线程中下载适用于您设备的 rollback 和 OxygenOS 11 软件包。

**XDA 论坛:[一加 7](https://forum.xda-developers.com/c/oneplus-7.8833/) || [一加 7 Pro](https://forum.xda-developers.com/c/oneplus-7-pro.8847/) || [一加 7T](https://forum.xda-developers.com/c/oneplus-7t.9249/) || [一加 7T Pro](https://forum.xda-developers.com/c/oneplus-7t-pro.9327/)**

* * *

## 为一加 7 和一加 7T 系列下载 OxygenOS 12 MP2

*   **一加 7**
    *   印度(GM1901_11。H.30)
    *   欧洲(GM1903_11。H.30)
    *   全球(GM1901_11。H.31)

*   **一加 7 Pro**
    *   印度(GM1911_11。H.30)
    *   欧洲(GM1913_11。H.30)
    *   全球(GM1911_11。H.31)

*   **一加 7T**
    *   印度(HD1901_11。F.17)
    *   欧洲(HD1903_11。F.17)
    *   全局(HD1901_11。F.17)

*   **一加 7T Pro**
    *   印度(HD1911_11。F.17)
    *   欧洲(HD1913_11。F.17)
    *   全球(HD1911_11。F.17)

值得注意的是，一加开始为一加 7 和 7 Pro 的全球和印度版本发布统一的软件。然而，OxygenOS 12 更新将这两个区域变体分开。如果想了解更多，可以看看下面 XDA 资深会员 [Some_Random_Username](https://forum.xda-developers.com/m/some_random_username.8234677/) 的讲解:

作为 7 系列设备 OxygenOS 11.0.8.1 更新的一部分，一加将系统更新应用程序升级到版本 2.3.0.2.220426145405.673e011。它允许向之前运行统一(全球+印度)固件的设备提供不同的区域版本。

更具体地说，根据软件属性`ro.vendor.op.india`的值，OTA 应用将向在 OTA 请求期间发送的 JSON 添加新字段“nvCarrier”。

如果`ro.vendor.op.india`的值被设置为 1，nvCarrier 值将被设置为 00011011，以便交付内部版本。否则，它将被设置为 10100001 以交付全局构建。

*感谢 XDA 资深会员 [Some_Random_Username](https://forum.xda-developers.com/m/some_random_username.8234677/) 的下载链接！*

* * *

**来源:**一加社区论坛( [1](https://community.oneplus.com/thread?id=1181167844348919809) ， [2](https://community.oneplus.com/thread?id=1181216999612088323) )