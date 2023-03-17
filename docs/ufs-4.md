# UFS 4.0 是下一代闪存存储规范，但它对您意味着什么？

> 原文：<https://www.xda-developers.com/ufs-4/>

你的下一部旗舰智能手机可能会安装 UFS 4.0 或通用闪存 4.0。更大的版本号通常意味着更好，但是这对你来说到底意味着什么呢？为什么 UFS 4.0 比 UFS 3.1 有所改进？UFS 到底是什么？

## 通用闪存:相对于 eMMC 的优势

通用闪存(UFS)是由联合电子设备工程委员会(JEDEC)设计和增加的标准，JEDEC 是一个为不同电子系统设计开放标准的全球性组织。 [JEDEC 于 2022 年 8 月发布了 UFS 4.0 标准](https://www.jedec.org/document_search?search_api_views_fulltext=jesd220f)，最近一次更新是 UFS 3.1，发布于 2020 年。

UFS 比 eMMC 有一个明显的优势，那就是它的全双工接口。半双工可以想象成单行道；交通可以单向流动，但不能同时双向流动。这意味着在 eMMC，你只能读或写，但不能同时读和写。相比之下，UFS 可以同时进行这两项操作，这允许并行进行读写操作。

这些是 eMMC 对 UFS 3.1 和 UFS 4.0 达到的最大额定速度。请记住，现在很少有智能手机发布 eMMC 存储，并且在过去一两年发布的任何旗舰产品都可以保证使用 UFS 3.0 或 UFS 3.1。

|  | **顺序读取(MB/s)** | **顺序写入(MB/s)** | **随机读取(IO/s)** | **随机写入(IO/s)** |
| **eMMC 5.1** | 250 | 125 | 11000 | 13000 |
| **UFS 3.1** | 2100 | 1200 | 100000 | 70000 |
| **UFS 4.0** | 4200 | 2800 | *不适用* | *不适用* |

如果你看上面的表格，UFS 4.0 有一些相当大的改进。存储速度如此重要的原因是，将大文件从手机存储器转移到手机内存会受到存储速度的限制。你可以拥有世界上最快的芯片组，但如果你的存储速度慢，游戏仍然需要很长时间才能加载，你的手机仍然需要很长时间才能开机。

## UFS 4.0 比 UFS 3.1 有哪些改进？

先说大家最关心的数字:UFS 4.0 比 UFS 3.1 快很多。它将顺序读取速度从 2.1GB/s 提高了一倍，达到 4.2GB/s，并将顺序写入速度从 1.2GB/s 提高了一倍多，达到 2.8GB/s。这些都是巨大的改进，将提高您的手机启动应用程序和将文件保存到存储设备的速度。

然而，速度并不是全部。有幸推出 UFS 4.0 的三星公司表示，它的耗电量也比 UFS 3.1 低 46%。它说，你每 6.0Mbps 的传输速度将消耗大约 1mA，尽管电流不是功耗的一个很好的衡量标准。这很可能是在手机电池处于标称电压(或 3.6v/3.7v)时测得的。存储远不是智能手机中最大的电池消耗者(肯定是芯片组和显示屏)，但任何和所有的能效改进都是受欢迎的。

最重要的是，UFS 4.0 模块非常小。三星表示，它们只有 1 毫米厚，1TB 模块的最大尺寸为 13 毫米长和 11 毫米宽。这是在一个小包装中的大量存储，并确保在您的设备的有限空间内有更多的空间用于其他组件。

## 手机什么时候会有 UFS 4.0？我应该升级吗？

如果你正在寻找一部装有 UFS 4.0 的手机，那么你不用等太久了。 [Vivo X90 系列](https://www.xda-developers.com/vivo-x90-series-launch/)已经有了，其他公司也紧随其后。[一加 11](https://www.xda-developers.com/oneplus-11-review/) 、[三星 Galaxy S23 系列](https://www.xda-developers.com/samsung-galaxy-s23-review/)(基本款 S23 除外)，以及无数其他旗舰也都有。

至于你是否应该只基于 UFS 4.0 进行升级，答案几乎肯定是否定的。虽然这里有实质性的改进，但它们不会那么明显，因为如此大的改进可能会产生递减的回报。如果一个游戏的加载速度从五秒降低到四秒，那么花几百美元升级真的值得吗？

因此，UFS 4.0 是你升级时受益于*的改进之一，但你绝对不应该升级*，因为它的*。智能手机总是在不断改进，更快的存储不会让一切变得神奇地更好。芯片组的改进仍将是最引人注目的升级，即使这些改进现在每一代都在减少。*