# 第四代至强处理器是英特尔在数据中心东山再起的机会

> 原文：<https://www.xda-developers.com/intel-xeon-4th-gen-launch/>

众所周知，英特尔多年来一直在努力追赶数据中心的竞争对手，其中主要包括 AMD，但也包括基于 Arm 的 CPU 设计者，如 Ampere 和亚马逊。该公司的数据中心和 AI 集团报告去年第三季度的运营利润率为 0%，这基本上意味着它的盈利和亏损一样多；就在一年前，它还能赚 23 亿美元。主要问题是，英特尔根本无法跟上其竞争对手，但全新 CPU 和 GPU 的到来可能会改变这一点。凭借其第四代至强可扩展处理器和 Max 系列 CPU 和 GPU，英特尔旨在扭转其多年来的颓势。

## 第四代至强处理器是向前迈出的重要一步，但并不完全是赢家

自从 AMD 在 2019 年推出第二代 Epyc 罗马 CPU 以来，英特尔一直处于守势。数据中心效率为王，Epyc Rome 使用的是 TSMC 的 7nm 工艺，比英特尔当时使用的古老的 14nm 节点效率要高得多。罗马也配备了 64 个核心，而英特尔只能在典型的至强处理器上配备 28 个核心，56 个核心的选项已经存在于纸面上，尽管它从未流行起来。不仅仅是 7 纳米节点使 Rome 成为可能，还有小芯片设计，这使 AMD 能够真正增加核心数量，而不会浪费大量的硅。

在许多方面，第四代至强处理器(代号 Sapphire Rapids)是英特尔对 Epyc 的挑战。它使用英特尔的 10 纳米工艺，大约相当于 TSMC 的 7 纳米工艺，有四个小芯片或瓦片，每个小芯片或瓦片有 15 个核心和 CPU 需要的所有其他功能。每个小芯片基本上都是一个 CPU，这是第四代至强处理器和最新的 Epyc CPUss 之间的一个关键区别，Epyc CPU 有两种类型的芯片:用于内核的芯片和用于 I/O 的芯片。这意味着 Sapphire Rapids 实际上与第一代 Epyc Naples 最相似，后者在 2017 年被英特尔嘲笑为具有“粘合在一起”的芯片。

不可否认，即使有了第四代至强处理器，英特尔在小芯片领域仍然落后，但该公司有一个锦囊妙计:HBM2。高带宽内存(HBM)是一种紧凑和高速的内存形式，HBM2 通常用于 GPU 作为超高速 VRAM，但高端 Sapphire Rapids CPUs(官方称为 Intel Max)使用 64GB 的这种内存作为一种 L4 缓存。AMD 的全新 [Epyc Genoa 芯片不会采用 HBM2](https://www.hpcwire.com/2022/11/10/amds-4th-gen-epyc-genoa-96-5nm-cores-across-12-compute-chiplets/) ，因为该公司认为这根本没有必要，但英特尔不同意，假以时日，我们将看到谁是正确的。

Sapphire Rapids 带来了许多架构改进，英特尔声称，在“通用计算”方面，第四代至强处理器比第三代至强处理器 Ice Lake 平均快 53%，这基本上是你在 Cinebench 等基准测试中看到的性能。其他应用程序看到更大的提升，从两倍到十倍不等。也许最重要的是，英特尔声称其效率提高了 Ice Lake 的 2.9 倍，这对于降低数据中心的总拥有成本(TCO)极其重要。此外，第四代至强处理器支持 DDR5 和 [PCIe 5.0](https://www.xda-developers.com/pcie-5/) ，这两种技术对于高端服务器都非常重要。

虽然 Sapphire Rapids 对于至强处理器来说无疑是一个巨大的改进，但它可能不会主宰数据中心。AMD 没有固步自封，其最新的 Epyc Genoa CPUs 使用 TSMC 的 5 纳米工艺和 Zen 4 架构，就像锐龙 7000 一样。高端 Genoa 有 96 个内核，而不是 64 个，这意味着英特尔仍然处于很大的劣势，如果 Genoa 也更高效也不会令人惊讶，因为 TSMC 的 5 纳米比英特尔的 10 纳米更新。

顺便提一下，英特尔还没有宣布任何基于 Sapphire Rapids 的工作站至强处理器，但[有传言称这些处理器将在稍后](https://www.tomshardware.com/news/intel-sapphire-rapids-ws-lineup-leak)发布。据称，这些至强 W 芯片不会提供 Sapphire Rapids 的全部 60 个内核，最多只有 56 个，但仍然可以证明是 AMD 的锐龙 Threadripper 芯片的有力竞争对手。

## 帝国反击战？

距离英特尔上次在 AMD 上占据优势已经过去了大约三年，现在该公司终于有机会发起反击。英特尔还通过 Ponte Vecchio 在数据中心 GPU 领域发起攻势，英特尔将其统称为数据中心 GPU Max 系列。英特尔没有真正提供任何关于其总体性能的具体细节，但 GPU 有超过 1000 亿个晶体管分布在 47 块瓷砖上。这是对 AMD、[和任何其他拥有数据中心处理器的公司的两面夹击，AMD 最近发布了其庞大的 MI300 服务器 APU](https://www.anandtech.com/show/18721/ces-2023-amd-instinct-mi300-data-center-apu-silicon-in-hand-146b-transistors-shipping-h223) 。

鉴于英特尔最近的历史，人们很容易对该公司的机会持怀疑态度，我相信第四代至强和 Ponte Vecchio 将有初期问题，但 AMD 能够将自己从濒临破产转变为世界领先的处理器设计者之一。如果 AMD 能做到，为什么英特尔不能？这可能是让英特尔重新获得性能领先地位的跳板，也许不是这一代，而是下一代。