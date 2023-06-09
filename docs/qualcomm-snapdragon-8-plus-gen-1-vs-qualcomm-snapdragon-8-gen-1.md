# 高通骁龙 8 Plus Gen 1 vs 高通骁龙 8 Gen 1:旗舰芯片有什么变化？

> 原文：<https://www.xda-developers.com/qualcomm-snapdragon-8-plus-gen-1-vs-qualcomm-snapdragon-8-gen-1/>

高通骁龙 8 Gen 1 是一款自问世以来就饱受问题困扰的芯片组。我们比以往任何时候都看到原始设备制造商跳出来试图通过软件控制来解决其低效率，有些人选择在某些情况下节流。其他人，如一加，总体上抑制了它，长话短说，至少可以说，这是有问题的。骁龙 8 Plus Gen 1 试图纠正所有错误，虽然它没有做到这一点，但它已经非常接近了。

至于人们为什么认为骁龙 8 Plus Gen 1 比其非 Plus 版本好得多？Plus 采用 TSMC 的 N4 工艺制造。在芯片生产方面，没有任何官方消息来源暴露出高通对三星代工厂的不满，但从言外之意来看，很久以来就很明显三星阵营存在问题。

尽管情况越来越糟。TSMC 生产的联发科天玑 9000 在用户测试中远远超过了高通自己的效率。这是一场完美风暴，它清楚地指向了一件事——三星代工厂，无论出于什么原因，在 2021 年和 2022 年生产了低于标准的芯片组。我们在芯片发布时在华硕 SM8475 工程平台中测试了[骁龙 8 Plus Gen 1，现在我们有时间在几款不同的手机中正确使用它。不过还有一个问题:与它的非升级版相比，T4 到底表现如何？我们对它进行了测试。](https://www.xda-developers.com/qualcomm-snapdragon-8-plus-gen-1-benchmarks/)

***关于这个对比:*** *我们对比了[一加 10 Pro](https://www.xda-developers.com/oneplus-10-pro-review/) 和[一加 10T](https://www.xda-developers.com/oneplus-10t-review/) 。这两款设备都是出厂重置，没有链接谷歌账户，Wi-Fi 只能为需要它的基准测试安装更新包。基准测试应用程序通过 adb 安装，所有测试都在设备电池电量超过 50%的情况下在飞行模式下运行。这两款设备都启用了一加的性能模式，以消除对这些芯片组时钟速度的人为限制。*

## 高通骁龙 8 第 1 代 vs 高通骁龙 8 加第 1 代:规格

|  | 

**高通骁龙 8 创 1**

 | 

**高通骁龙 8 加第 1 代**

 |
| --- | --- | --- |
| **CPU** | 

*   1x Kryo(基于 ARM Cortex-X2)Prime core @ 2.995 GHz，1MB L2 高速缓存
*   3 个 Kryo(基于 ARM Cortex A710)性能内核@ 2.5GHz
*   4 个 Kryo(基于 ARM Cortex A510)高效内核@ 1.79GHz
*   手臂皮层 v9
*   6MB 三级高速缓存
*   **性能比骁龙 888 快 20%**
*   **比骁龙 888x 节能 30%**

 | 

*   1 个 Kryo(基于 ARM Cortex-X2)Prime core @ 3.2 GHz、1MB L2 高速缓存
*   3 个 Kryo(基于 ARM Cortex A710)性能内核@ 2.8GHz
*   4 个 Kryo(基于 ARM Cortex A510)高效内核@ 2.0GHz
*   手臂皮层 v9
*   6MB 三级高速缓存
*   **CPU 性能比第 1 代骁龙 8 快 10%**
*   **比骁龙 8 代 1 的能效高 30%**

 |
| **GPU** | 

*   Adreno GPU
*   Vulkan 1.1
*   肾上腺素框架运动引擎
*   具有 10 位色深和录制功能的 HDR 游戏。2020 色域
*   基于物理的渲染
*   体积渲染
*   视频播放:H.264 (AVC)，H.265 (HEVC)，VP8，VP9，4K HDR10，HLG，HDR10+，杜比视界
*   **图形渲染速度比骁龙 888 快 30%**
*   **比骁龙 888 节能 25%**

 | 

*   Adreno GPU
*   Vulkan 1.1
*   肾上腺素框架运动引擎
*   具有 10 位色深和录制功能的 HDR 游戏。2020 色域
*   基于物理的渲染
*   体积渲染
*   视频播放:H.264 (AVC)，H.265 (HEVC)，VP8，VP9，4K HDR10，HLG，HDR10+，杜比视界
*   **比骁龙 8 代 1 的 GPU 时钟速度快 10%**
*   **GPU 功耗比骁龙 8 代 1 降低 30%**

 |
| **显示** | 

*   最大设备显示支持:4K @ 60Hz/QHD+ @ 144Hz
*   最大外部显示器支持:4K @ 60Hz
*   HDR 支持
*   USB Type-C 支持上的显示端口

 | 

*   最大设备显示支持:4K @ 60Hz/QHD+ @ 144Hz
*   最大外部显示器支持:4K @ 60Hz
*   HDR10 和 HDR10+
*   10 位颜色深度。2020 色域
*   用于有机发光二极管均匀性的 Dumora 和子像素着色

 |
| **艾** | 

*   高通六角形处理器
    *   融合人工智能加速器
    *   六边形张量加速器
    *   六边形向量扩展
    *   六边形标量加速器
    *   支持混合精度(INT8+INT16)
    *   支持所有精度(INT8、INT16、FP16)

*   第七代人工智能引擎
*   第三代高通传感中心
*   拥抱脸自然语言处理
*   徕卡的莱茨外观模式
*   **比骁龙 888 快 400%的 AI 性能**
*   **张量加速器性能比骁龙 888** 快 100%
*   **比骁龙 888 节能 70%**

 | 

*   高通六角形处理器
    *   融合人工智能加速器
    *   六边形张量加速器
    *   六边形向量扩展
    *   六边形标量加速器
    *   支持混合精度(INT8+INT16)
    *   支持所有精度(INT8、INT16、FP16)

*   第七代人工智能引擎
*   第三代高通传感中心
*   拥抱脸自然语言处理
*   徕卡的莱茨外观模式
*   **性能功耗比比骁龙 8 代第 1 代产品高 20%**

 |
| **记忆** | LPDDR5 @ 3200MHz，16GB | LPDDR5 @ 3200MHz，16GB |
| **ISP** | 

*   三路 18 位 Spectra 680 ISP
    *   高达每秒 3.2 千兆像素的计算机视觉 ISP
    *   高达 3600 万像素的三摄像头，30 帧/秒，零快门延迟
    *   高达 64+36MP 双摄像头，30 FPS，零快门延迟
    *   高达 108 百万像素的单摄像头，每秒 30 帧，零快门延迟
    *   高达 200 MP 的照片拍摄

*   视频拍摄:8K HDR @ 30 fps；慢动作高达 720p @ 960 fpsHDR10、HDR10+、HLG、杜比视界

 | 

*   三路 18 位 Spectra 680 ISP
    *   高达每秒 3.2 千兆像素的计算机视觉 ISP
    *   高达 3600 万像素的三摄像头，30 帧/秒，零快门延迟
    *   高达 64+36MP 双摄像头，30 FPS，零快门延迟
    *   高达 108 百万像素的单摄像头，每秒 30 帧，零快门延迟
    *   高达 200 MP 的照片拍摄

*   视频拍摄:8K HDR @ 30 fps；慢动作高达 720p @ 960 fpsHDR10、HDR10+、HLG、杜比视界

 |
| **调制解调器** | 

*   骁龙 X65 5G 调制解调器
*   下行链路:10Gbps
*   模式:NSA、SA、TDD、FDD
*   毫米波:1000MHz 带宽，8 个载波，2×2 MIMO
*   低于 6 GHz: 300MHz 带宽，4×4 MIMO

 | 

*   骁龙 X65 5G 调制解调器
*   下行链路:高达 10Gbps
*   模式:NSA、SA、TDD、FDD
*   毫米波:1000MHz 带宽，8 个载波，2×2 MIMO
*   低于 6 GHz: 300MHz 带宽，4×4 MIMO

 |
| **充电** | 高通快速充电 5 | 高通快速充电 5 |
| **连通性** | 位置:北斗、伽利略、GLONASS、GPS、QZSS、[双频 GNSS 支持](https://www.xda-developers.com/dual-frequency-gnss-important-location-feature-your-phone-probably-missing/) Wi-Fi:高通 FastConnect 6900Wi-Fi 6E，Wi-Fi 6；2.4/5GHz/6GHz 频段；20/40/80/160 兆赫频道；DBS (2×2 + 2×2)、TWT、WPA3、8×8 MU-MIMO 蓝牙:版本 5.3、aptX 语音、aptX 无损、aptX 自适应和 LE 音频 | 位置:北斗、伽利略、GLONASS、GPS、QZSS、[双频 GNSS 支持](https://www.xda-developers.com/dual-frequency-gnss-important-location-feature-your-phone-probably-missing/) Wi-Fi:高通 FastConnect 6900Wi-Fi 6E，Wi-Fi 6；2.4/5GHz/6GHz 频段；20/40/80/160 兆赫频道；DBS (2×2 + 2×2)、TWT、WPA3、8×8 MU-MIMO 蓝牙:版本 5.3、aptX 语音、aptX 无损、aptX 自适应和 LE 音频 |
| **制造过程** | **4 纳米三星代工厂** | **4 纳米 TSMC** |

* * *

## 高通骁龙 8+第 1 代与高通骁龙 8+第 1 代:根本区别

在我们开始比较这两款芯片组之前，有必要指出这两款芯片组基本上是完全相同的。在设计层面上，它们拥有相同的内核、相同的调制解调器和相同的 GPU。唯一真正的区别是时钟速度的提高，如果有效率的提高，那很可能是因为高通能够将时钟速度提高一点点，同时仍然保持降低的功耗。

原因很简单:倍频器的最后一步消耗了最多的能量。这就是为什么一加能够通过简单地在任何时候将骁龙 8 Gen 1 的速度控制在比其最大时钟速度低一点点的速度来获得很大的里程数。高通能够从 TSMC 的生产中获得大幅减少的能源消耗，该公司可能选择推动更高的最大频率，同时仍保留一些效率改进。

鉴于时钟速度的提高是“Plus”芯片组的典型特征，除了效率之外，Plus 版本几乎没有任何改进，这很奇怪。

核心方面，常规 8 Gen 1 上的 Prime 核心主频为 2.995GHz，在 Plus 上跳至 3.2GHz。苹果 A15 性能核心主频 3.2GHz，供参考。三个 Kryo 性能核心使用 [ARM 的 Cortex-A710 设计](https://www.xda-developers.com/armv9-cpu-designs-cortex-x2-performance-gains/)，它们在常规 8 Gen 1 上的主频为 2.5GHz，在 Plus 上最高可达 2.8GHz。至于三个 Kryo 效率核心，它们基于新的 Cortex-A510 设计，也从 1.79GHz 提升到 2GHz。

我们认为，许多原始设备制造商管理骁龙 8 第 1 代系列的方式在高负荷下可能是高压手段。这就是我们努力使用来自同一家 OEM 厂商的两款设备的原因——不同的公司采用不同的芯片组，但我们相信，这两款设备及其调试都有一套完整的理念。这意味着我们应该得到这些芯片组相对于彼此的能力的更准确的表示。

## 基准概述

*   **[安兔兔](http://www.antutu.com/en/index.htm)** :这是一个整体基准。AnTuTu 测试 CPU、GPU 和内存性能，同时包括抽象测试和最近的相关用户体验模拟(例如，涉及滚动 ListView 的子测试)。最终得分根据设计者的考虑进行加权。
*   **[GeekBench](https://www.geekbench.com/)** :一个以 CPU 为中心的测试，使用了几种计算工作负载，包括加密、压缩(文本和图像)、渲染、物理模拟、计算机视觉、光线跟踪、语音识别和对图像的卷积神经网络推理。分数细分给出了具体的指标。最终分数根据设计者的考虑进行加权，重点是整数性能(65%)，然后是浮点性能(30%)，最后是加密(5%)。
*   **[GFXBench](https://gfxbench.com/result.jsp)** :旨在使用最新的 API 模拟视频游戏图形渲染。大量的屏幕效果和高质量的纹理。较新的测试使用 Vulkan，而遗留测试使用 OpenGL ES 3.1。输出是测试期间的帧数和每秒帧数(本质上是另一个数除以测试长度)，而不是加权分数。
    *   阿兹特克废墟:这些测试是 GFXBench 提供的计算量最大的测试。目前，顶级移动芯片组无法支持每秒 30 帧。具体来说，该测试提供了非常高的多边形计数几何图形、硬件镶嵌、高分辨率纹理、全局照明和大量阴影贴图、丰富的粒子效果，以及 bloom 和景深效果。这些技术中的大多数将强调处理器的着色器计算能力。
    *   曼哈顿 ES 3.0/3.1 :鉴于现代游戏已经达到了其提出的图形保真度并实现了相同类型的技术，这项测试仍然具有相关性。它采用了复杂的几何体，包括多个渲染目标、反射(立方体贴图)、网格渲染、许多延迟光源，以及后期处理过程中的高光和景深。

*   **[CPU 节流测试](https://play.google.com/store/apps/details?id=skynet.cputhrottlingtest&hl=en&gl=US)** :这个应用用 C 语言重复了一个简单的多线程测试，时间短至 15 分钟，尽管我们运行了 30 分钟。该应用程序绘制了一段时间内的分数，这样你就可以看到手机何时开始节流。这个分数是以 GIPS 来衡量的，即每秒十亿次运算。
*   **它使用 Android 的 BatteryManager API 来计算测试期间使用的瓦特数，这可以用来了解智能手机的电池消耗情况。**

* * *

## 高通骁龙 8 Plus 第 1 代 vs 高通骁龙 8 第 1 代:计算工作负载

我们首先测试了这两款芯片组的计算能力。我们使用 Geekbench 5，确保每个设备在启用飞行模式的情况下处于正常的环境温度。

从上面，我们可以注意到骁龙 8 Plus Gen 1 在计算能力方面有一些相当大的改进。在多核中，我们看到了 15%的增长，而在单核中，我们只看到了 5%的增长。尽管如此，很明显，这种芯片组的功能从一开始就已经有所改进。

## 高通骁龙 8 Plus 第 1 代与高通骁龙 8 第 1 代:能效

[烧坏基准](https://play.google.com/store/apps/details?id=org.ai.throttling)让我们能够轻松测量智能手机芯片组的功耗。当我们最初测试骁龙 8 Plus Gen 1 时，我们与开发人员安德烈·伊格纳托夫进行了交谈，以了解这款应用的工作原理。他告诉我们在最低亮度下运行这款充满电的设备，并启用飞行模式，因此，这里收集的所有数据都是在这些条件下进行的。伊格纳托夫告诉我们，以下测试是在 SoC 的不同组件上运行的，作为燃尽基准的一部分:

*   GPU:使用 OpenCL 的并行视觉计算
*   CPU:多线程计算主要涉及 Arm Neon 指令
*   NPU:具有典型机器学习操作的人工智能模型

首先，这里是我们收集的功耗指标。

在这些条件下，骁龙 8 Gen 1 的最大功率为 14.46W。标准的 5,000 mAh 电池在达到这一持续最大功率时，可以持续使用近 3.5 小时。虽然这是一个不切实际的情况(特别是因为节流，以及没有人会真的这样使用他们的手机的事实)，但它有助于想象这是什么样的电池消耗。

相比之下，根据这些测量，骁龙 8 Plus Gen 1 在其峰值功耗为 11.5 瓦。这相当于一部装有 5，000 毫安时电池的智能手机大约使用 4.3 小时。

然而，在这里，我们可以看到骁龙 8 Plus Gen 1 也比骁龙 8 Gen 1 强大得多。上面的图表可以相对于上面计算的瓦特数显示，你会看到，虽然骁龙 8 代 1 消耗更多的能量，但它在计算上并不强大。这表明骁龙 8 Plus Gen 1 的效率更高，瓦数更低也意味着热量更少。

下表显示了在这些条件下每个芯片组的最大能力，同时也显示了我们测量的百分比增长。

|  | 

骁龙 8 代 1

 | 

骁龙 8 加第 1 代

 | 

百分比变化(从 8 代 1 到 8 代加 1)

 |
| --- | --- | --- | --- |
| **CPU FPS** | 13.65 | 17.76 | 增长 30% |
| **GPU FPS** | 15.34 | 16.61 | 增长 8% |
| **最大瓦数** | 14.46 瓦 | 11.5 瓦 | 下降 26% |

值得记住的是，虽然这些值与高通自己的测量略有不同，但这可以通过软件来解释，甚至只是偶然。我们多次运行该测试，骁龙 8 Plus Gen 1 在每次迭代中都大幅领先，骁龙 8 Gen 1 的更高功耗也是一个重要因素。

也正是在这里，使用的设备可能会影响这些结果。虽然我们有信心说这里反映了能源的减少，正如我们将华硕工程平台设备与 RedMagic 7 Pro 进行比较时一样，但由于显示器、连接性等其他方面的原因，设备之间的能源使用可能会有所不同。

* * *

## 高通骁龙 8 Plus 第 1 代 vs 高通骁龙 8 第 1 代:图形

GFXBench 是一个应用程序，可以通过许多不同的测试来测试智能手机 GPU 的图形功能。我们在这里运行了五个不同的测试，计算量最大的是 1440p Aztec 测试。我们在每一项测试中都看到了大约 10%的全面增长，这符合高通对芯片组的预期，也符合我们在倦怠基准中的 GPU 测试。

* * *

## 高通骁龙 8 Plus 第 1 代 vs 高通骁龙 8 第 1 代:CPU 节流测试

从我们目前所看到的一切来看，骁龙 8 Gen 1 是一款散热效率很低的芯片组，对它的最终测试是 CPU 节流测试。这项测试是在相同的环境温度下在两台设备上并排进行的，很明显，高通骁龙 8 Plus Gen 1 的性能更好，时间更长。虽然他们最终节流到基本相同的百分比，但骁龙 8 Plus Gen 1 在更长时间内保持了更高的性能，其最低 GIPS 比骁龙 8 Gen 1 高出近 10%。

* * *

## 高通骁龙 8 加 1 代 vs 高通骁龙 8 1 代:安图图

Antutu 是一个全面的基准，可以测试智能手机的各个方面。虽然它计算出的总数并不能给你比其他智能手机更多的东西，但它仍然可以让你大致了解一部手机在计算方面比另一部手机好多少。无论怎么想象，这肯定不是一盏指路明灯，但安兔兔在行业中仍有一席之地。我们看到这里的数字增加了 6%，有利于骁龙 8 加第一代。

* * *

## 高通骁龙 8 Plus Gen 1 无疑是赢家

无论你用什么标准来比较这两款芯片组，骁龙 8 Plus Gen 1 在所有方面都是赢家。它效率更高，功率更大，产生的热量也更少。相比之下，骁龙 8 Gen 1 是一种相对低效的芯片组，消耗大量能源。两者都是强大的芯片组，但考虑到公司不得不采取的措施来驯服这一代 8 代 1，很明显三星的制造工艺中存在一些问题。

你能从这种比较中得到什么？在所有其他因素相同的情况下，您肯定会更喜欢使用骁龙 8 Plus Gen 1，而不是骁龙 8 Gen 1。