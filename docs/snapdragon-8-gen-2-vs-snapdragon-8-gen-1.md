# 骁龙 8 代 2 与骁龙 8 代 1 的对比:更高的效率放大了同比改进

> 原文：<https://www.xda-developers.com/snapdragon-8-gen-2-vs-snapdragon-8-gen-1/>

骁龙 8 代 2 号很可能是目前业界最好的芯片组，这要归功于许多因素。它拥有令人难以置信的强大 GPU，强大的计算能力，它将成为 2023 年发布的许多高端设备的主干。毫无疑问，这是一款比骁龙 8 代 1 更好的 SoC，但好了多少呢？

事实证明，这是一个相当大的改进。原因有很多(甚至骁龙 8 Plus Gen 1 设法[远远超过最初的骁龙 8 Gen 1](https://www.xda-developers.com/qualcomm-snapdragon-8-plus-gen-1-vs-qualcomm-snapdragon-8-gen-1/) )，这似乎可以归结为效率。骁龙 8 代 2 可以利用它汲取的能量做更多的事情，而骁龙 8 代 1 总是在挣扎。再加上原始设备制造商为驯服 8 Gen 1 而制定的功率限制，因为否则的话，他们[最终会推出滚烫的设备](https://www.xda-developers.com/black-shark-5-pro-review/)，而你的芯片组对一些人来说感觉表现不佳。

因此，骁龙 8 代 2 在许多不同的方面超越了骁龙 8 代 1，但其原因并不是正常的逐年改进。如此大的改进是不可持续的，从骁龙 8 Plus Gen 1，8 Gen 1 基本上应该有的芯片组到骁龙 8 Gen 2 的飞跃将会小得多。

***关于这个对比:*** *我们对比了一下[一加 11](https://www.xda-developers.com/oneplus-11-performance-evaluation/) 和 [O](http://www.xda-developers.com/asus-rog-phone-6d-ultimate-review/) [nePlus 10 Pro](https://www.xda-developers.com/oneplus-10-pro-review/) 。这两款设备都是出厂重置，没有链接谷歌账户，Wi-Fi 只能为需要它的基准测试安装更新包。基准测试应用程序通过 adb 安装，所有测试都在设备电池电量超过 50%的情况下在飞行模式下运行。这两款设备都启用了一加的性能模式，以消除对这些芯片组时钟速度的人为限制。*

## 骁龙 8 代 2 对骁龙 8 代 1:规格

|  | 

骁龙 8 第二代

 | 

**骁龙 8 创 1**

 |
| --- | --- | --- |
| **CPU** | 

*   1x Kryo(基于 ARM Cortex-X3)Prime core @ 3.19 GHz，1MB L2 高速缓存
*   2 个 Kryo(基于 ARM Cortex A715)性能内核@ 2.8GHz
*   2 个 Kryo(基于 ARM Cortex A710)性能内核@ 2.8GHz
*   3 个 Kryo 高效内核(基于 ARM Cortex A510)@ 2.0 GHz
*   手臂皮层 v9
*   8MB 三级高速缓存

 | 

*   1 个 Kryo(基于 ARM Cortex-X2)Prime core @ 3.2 GHz、1MB L2 高速缓存
*   3 个 Kryo(基于 ARM Cortex A710)性能内核@ 2.8GHz
*   4 个 Kryo(基于 ARM Cortex A510)高效内核@ 2.0GHz
*   手臂皮层 v9
*   6MB 三级高速缓存

 |
| **GPU** | 

*   Adreno GPU
*   Vulkan 1.3
*   骁龙精英博彩
*   骁龙影子德诺泽
*   肾上腺素框架运动引擎
*   视频播放:H.264 (AVC)，H.265 (HEVC)，VP8，VP9，4K HDR10，HLG，HDR10+，杜比视界，AV1

 | 

*   Adreno GPU
*   Vulkan 1.1
*   肾上腺素框架运动引擎
*   具有 10 位色深和录制功能的 HDR 游戏。2020 色域
*   基于物理的渲染
*   体积渲染
*   视频播放:H.264 (AVC)，H.265 (HEVC)，VP8，VP9，4K HDR10，HLG，HDR10+，杜比视界

 |
| **显示** | 

*   最大设备显示支持:4K @ 60Hz/QHD+ @ 144Hz
*   最大外部显示器支持:4K @ 60Hz
    *   10 位颜色
    *   HDR10，HDR10+，HDR 生动，杜比视觉

*   有机发光二极管均匀性的延迟和子像素着色
*   有机发光二极管老化补偿

 | 

*   最大设备显示支持:4K @ 60Hz/QHD+ @ 144Hz
*   最大外部显示器支持:4K @ 60Hz
*   HDR10 和 HDR10+
*   10 位颜色深度。2020 色域
*   用于有机发光二极管均匀性的 Dumora 和子像素着色

 |
| **艾** | 

*   带六边形矢量扩展的六边形 DSP、六边形张量加速器、六边形标量加速器、六边形直接链接
*   人工智能引擎
*   高通传感中心
    *   用于音频和传感器的双人工智能处理器
    *   始终感应照相机

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

 |
| **记忆** | LPDDR5X @ 4200MHz，16GB | LPDDR5 @ 3200MHz，16GB |
| **ISP** | 

*   三路 18 位频谱 ISP
*   高达 200 百万像素的照片拍摄
*   单摄像头:最高 108 百万像素，ZSL 每秒 30 帧
*   双摄像头:高达 64+36MP，ZSL @ 30 FPS
*   三摄像头:最高 3600 万像素，ZSL 每秒 30 帧
*   视频拍摄:8K HDR @ 30 FPS；慢动作高达 720p @ 960 FPSHDR10，HDR10+，HLG，杜比视界，HEVC

 | 

*   三路 18 位 Spectra 680 ISP
    *   高达每秒 3.2 千兆像素的计算机视觉 ISP
    *   高达 3600 万像素的三摄像头，每秒 30 帧，零快门延迟
    *   高达 64+36MP 双摄像头，30 FPS，零快门延迟
    *   高达 108 百万像素的单摄像头，每秒 30 帧，零快门延迟
    *   高达 200 MP 的照片拍摄

*   视频拍摄:8K HDR @ 30 FPS；慢动作高达 720p @ 960 FPSHDR10、HDR10+、HLG、杜比视界

 |
| **调制解调器** | 

*   骁龙 X70 5G 调制解调器
*   下行链路:10Gbps
*   上行链路:3.5Gbps
*   模式:G NR、NR-DC、EN-DC、LTE、CBRS、WCDMA、HSPA、TD-SCDMA、CDMA 1x、EV-DO、GSM/EDGE
*   毫米波:8 个载波，2x2 MIMO
*   低于 6 GHz: 4x4 MIMO

 | 

*   骁龙 X65 5G 调制解调器
*   下行链路:高达 10Gbps
*   模式:NSA、SA、TDD、FDD
*   毫米波:1000MHz 带宽，8 个载波，2×2 MIMO
*   低于 6 GHz: 300MHz 带宽，4×4 MIMO

 |
| **充电** | 高通快速充电 5 | 高通快速充电 5 |
| **连通性** | 

*   位置:北斗、伽利略、GLONASS、GPS、QZSS、[双频 GNSS 支持](https://www.xda-developers.com/dual-frequency-gnss-important-location-feature-your-phone-probably-missing/)
*   Wi-Fi:高通 FastConnect 7800Wi-Fi 7，Wi-Fi 6E，Wi-Fi 6；2.4/5GHz/6GHz
*   乐队；20/40/80/160 兆赫频道；DBS (2x2 + 2x2)，行波管，WPA3，8×8 MU-MIMO
*   蓝牙:版本 5.3、aptX 语音、aptX 无损、aptX 自适应和 LE 音频

 | 

*   定位:北斗、伽利略、GLONASS、GPS、QZSS、[双频 GNSS 支持](https://www.xda-developers.com/dual-frequency-gnss-important-location-feature-your-phone-probably-missing/)
*   Wi-Fi:高通 FastConnect 6900Wi-Fi 6E，Wi-Fi 6；2.4/5GHz/6GHz
*   乐队；20/40/80/160 兆赫频道；DBS (2×2 + 2×2)，行波管，WPA3，8×8 MU-MIMO
*   蓝牙:版本 5.3、aptX 语音、aptX 无损、aptX 自适应和 LE 音频

 |
| **制造工艺** | 4 纳米 TSMC | 4 纳米三星代工厂 |

## 基本差异

鉴于骁龙 8 Gen 2 是上一代的迭代，设计差异很小。主内核从基于 X2 皮层的设计升级到基于 X3 皮层的设计。有趣的是，高通已经从三个性能核心发展到四个，显著提高了计算能力。

因此，高通确实移除了一个效率核心，这让我担心它可能会对智能手机的整体效率产生影响。但是，正如您稍后将看到的那样，它似乎并不存在。性能仍然很好，功耗在正常范围内，唯一的问题是包含两个 A710 内核而不是四个 A715 内核。

对于骁龙 8 Plus Gen 1，我们看到了性能和效率方面的巨大改进，这种改进通常只能在年同比改进的情况下才能看到。将骁龙 8 第 2 代与骁龙 8 第 1 代进行比较，以一种典型的代际改进所不期望的方式扩大了这一差距。想到从一加 10 Pro 升级到一加 11 可能获得的计算增益，真的令人难以置信。

## 基准概述

*   **GeekBench** :一项以 CPU 为中心的测试，使用了几种计算工作负载，包括加密、压缩(文本和图像)、渲染、物理模拟、计算机视觉、光线追踪、语音识别和图像上的卷积神经网络推理。分数细分给出了具体的指标。最终分数根据设计者的考虑进行加权，重点是整数性能(65%)，然后是浮点性能(30%)，最后是加密(5%)。
*   GFXBench :旨在使用最新的 API 模拟视频游戏图形渲染。大量的屏幕效果和高质量的纹理。较新的测试使用 Vulkan，而遗留测试使用 OpenGL ES 3.1。输出是测试期间的帧数和每秒帧数(本质上是另一个数除以测试长度)，而不是加权分数。
    *   阿兹特克废墟:这些测试是 GFXBench 提供的计算量最大的测试。目前，顶级移动芯片组无法支持每秒 30 帧。具体来说，该测试提供了非常高的多边形计数几何图形、硬件镶嵌、高分辨率纹理、全局照明和大量阴影贴图、丰富的粒子效果，以及 bloom 和景深效果。这些技术中的大多数将强调处理器的着色器计算能力。
    *   **Manhattan ES 3.0/3.1** :鉴于现代游戏已经达到了他们提出的图形保真度，并实现了相同类型的技术，这项测试仍然具有相关性。它采用了复杂的几何体，包括多个渲染目标、反射(立方体贴图)、网格渲染、许多延迟光源，以及后期处理过程中的高光和景深。

*   **CPU 节流测试**:这个应用程序用 C 语言重复了一个简单的多线程测试，时间短至 15 分钟，尽管我们运行了 30 分钟。该应用程序绘制了一段时间内的分数，这样你就可以看到手机何时开始节流。这个分数是以 GIPS 来衡量的，即每秒十亿次运算。
*   **烧坏基准**:以繁重的工作负载加载不同的 SoC 组件，以分析它们的功耗、热节流和最大性能。它使用 Android 的 BatteryManager API 来计算测试期间使用的瓦特数，这可以用来了解智能手机的电池消耗情况。

## 计算工作量

这些测试是使用 Geekbench 5 而不是 [Geekbench 6](https://www.xda-developers.com/geekbench-6-released/) 进行的，尽管我们将在未来的比较中过渡到使用 Geekbench 6。

在这项测试中，骁龙 8 代 2 比骁龙 8 代 1 有一些相当大的进步，特别是在多线程工作负载方面。单核性能有所提升，尽管“只有”12.6%的提升。相比之下，多线程的改进相当于 41.7%的增长，这是相当可观的。智能手机上的大多数处理都是多线程的，因此这些改进是显著的。

## 高通骁龙 8 代 2 对高通骁龙 8 代 1:能效

Burnout Benchmark 允许我们轻松测量智能手机芯片组的功耗。以下测试在 SoC 的不同组件上运行，作为烧毁基准的一部分。

*   GPU:使用 OpenCL 的并行视觉计算
*   CPU:多线程计算主要涉及 Arm Neon 指令
*   NPU:具有典型机器学习操作的人工智能模型

首先，这里是我们收集的功耗指标。

从上面的图表中可以看出，这些芯片组在达到极限时消耗的功率是相似的。14W 的排水是一个很大的量，但是我们的手机基本上从来没有达到这个量，除非我们真的故意按下它们。游戏可能会拉近距离，但即使是游戏也有动作变得迟钝和不那么激烈的时候。

然而，这只是硬币的一面。虽然它们在极端情况下消耗的功率相似，但这两种芯片的实际性能却大相径庭。

|  | 

骁龙 8 第二代

 | 

骁龙 8 代 1

 | 

百分比变化(从 8 代 1 到 8 代 2)

 |
| --- | --- | --- | --- |
| **CPU FPS(峰值)** | 19.22 | 13.03 | 增长 47% |
| **GPU FPS(峰值)** | 27.47 | 15.34 | 增长 79% |
| **瓦数(峰值)** | 13.67 瓦 | 13.29 瓦 | 下降 2.9% |

上面显示的改进只是在*峰值*性能上，这意味着实际的差异并不严重。从上面的图表中可以看出，骁龙 8 代 2 的 GPU 启动速度稍高，但速度有所下降，然后保持其性能，而骁龙 8 代 1 则没有。峰值性能差异可能更高，因为它显示了芯片组的整体能力，即使只是在它减速前的几秒钟。

对于一年一度的改善来说，这些增长是相当可笑的，但其原因是因为骁龙 8 Gen 1 的低效率。如果我们将 8 Gen 2 与 8 Plus Gen 1 进行比较(我们会这样做)，我们会发现差距要小得多。具有相同功耗的第 1 代 8 无法实现与第 1 代 8 加相同的性能水平。以上数字也是按峰值计算的。

同样重要的是要注意，这里也可能有软件控制在起作用。我们使用来自同一个 OEM 的两个器件，因为这更有可能显示芯片组改进的相关性，这是因为 OEM 最有可能在多个器件中采用相同的频率调整原则。一加可能比其他人更多地限制了 8 代 1 的性能，这也将扭曲结果。

话虽如此，在相同瓦数下的性能改进仍然表明从 8 代 1 到 8 代 2 的重大飞跃，而且令人印象深刻。

## 制图法

GFXBench 是一个应用程序，可以通过几种不同的测试来测试智能手机 GPU 的图形功能。我们在这里运行了五个测试，计算量最大的是 1440p Aztec 测试。在测试骁龙 8 第二代时，我们看到了 13%到 43%的改进，虽然低于 79%的改进，但仍然相当可观。

这种差异的原因可能归结于所使用的测试方法以及峰值性能和持续性能之间的差异。在骁龙 8 Gen 2 中，GPU 保持的最高性能低于其最高性能，尽管不可否认没有太多。上面显示的基于 Vulkan 的工作负载性能更好，比如 Aztec 测试。

## CPU 节流测试

随着时间的推移，骁龙 8 Gen 2 保持了更好的性能，保持了更高的持续性能和更高的峰值。尽管手机发热增加，但其性能仍保持不变，这与骁龙 8 Gen 1 相比是一个好迹象。

换句话说，随着时间的推移，骁龙 8 代 2 设备的性能将会相当稳定。

## 高通骁龙 8 代 2 是一个完美的迭代

高通骁龙 8 Gen 2 是旗舰骁龙 SoC 系列的一个完美进步，也是继骁龙 8 Gen 1 之后的又一个伟大的芯片组。骁龙 8 代 2 是对骁龙 8 代 1 的重大改进，其主要原因是能效。

大约在去年的这个时候，我们开始[读到像三星这样的公司被 Geekbench](https://www.xda-developers.com/geekbench-samsung-benchmark-manipulation/) 除名，原因是他们在如何对 8 Gen 1 施加限制方面不一致。一加限制了一加 10 Pro 开箱后的性能，OPPO 也做了同样的事情。没有像这样施加限制的公司最终推出的手机可能会伤害他们的用户，对智能手机芯片组来说，这是一个非常糟糕的时期。

骁龙 8 Gen 2 是一个完美的迭代，因为它改进了最重要的东西，同时也没有真正后退一步。所有的改进都被保留了下来，同时进一步改进，这是你对下一代产品所能要求的。我们期待更多采用骁龙 8 第二代芯片组的设备发布，并希望高通在骁龙 8 第三代上保持连胜。