# DirectStorage 1.1 现已提供 GPU 压缩，加载速度更快

> 原文：<https://www.xda-developers.com/directstorage-11-is-now-available-with-gpu-decempression/>

微软宣布 DirectStorage 1.1 现已正式面向开发者开放，承诺将为 Windows 上的游戏带来更快的加载速度。这要归功于新增加的对 GPU 解压缩的支持，它从 CPU 中卸载了解压缩游戏资产的工作。

GPU 解压缩是 DirectStorage 承诺的一个重要部分，尽管今年早些时候该 API 首次向 PC 游戏开发者提供时并没有出现。几周前，[微软表示，它将在年底前推出 DirectStorage 1.1](https://www.xda-developers.com/directstorage-1-1-soon-gpu-decompression-pc-games/) ，谢天谢地，这并没有花太长时间。

过去，当你玩游戏时，CPU 的工作是解压缩存储在 PC 上的资产，然后这些资产将被发送到 GPU，以便根据需要显示它们。但是，正如微软指出的那样，GPU 在处理这类任务方面非常出色，速度要快得多，因此将这项工作交给 GPU 是有意义的。当然，为了配合这一点，微软还必须创建一种新的压缩格式，GDeflate，它是与 Nvidia 合作开发的。这种格式针对 GPU 解压缩进行了优化，根据微软的测试，由于这种增强，资产的解压缩速度几乎快了三倍。

虽然所有支持 DirectX 12 和 Shader Model 6.0 的 GPU 都支持 GPU 解压缩，但 GPU 制造商可以对其驱动程序进行优化(称为元命令)，以便专门提高其硬件的性能。[英特尔](https://www.intel.com/content/www/us/en/developer/articles/news/directstorage-on-intel-gpus.html)和[英伟达](https://developer.nvidia.com/blog/accelerating-load-times-for-directx-games-and-apps-with-gdeflate-for-directstorage/)已经在其最新版本的 GPU 驱动程序中针对 DirectStorage 1.1 和 GDeflate 进行了优化。AMD 表示，它已经有了支持 metacommand 的驱动程序，但它们将与 NDA 旗下的 ISV 合作伙伴共享。你可以关注 AMD 的支持页面，在最新的驱动发布时获取它们。

虽然 DirectStorage 旨在用于 Windows 游戏，但微软表示，它将发布 GDeflate 压缩器和解压缩器的源代码，以便开发人员可以在其他平台上压缩资产。既然 GPU 解压缩得到了官方支持，游戏开始实现它应该只是时间问题，当这种情况发生时，您应该会看到加载时间的显著差异。

* * *

**来源:** [微软](https://devblogs.microsoft.com/directx/directstorage-1-1-now-available/)