# Oppo 在 2022 年骁龙峰会上展示了其面向移动设备的开放式光线追踪解决方案

> 原文：<https://www.xda-developers.com/oppo-ray-tracing-mobile-partnership-qualcomm/>

# Oppo 在 2022 年骁龙峰会上展示了其面向移动设备的开放式光线追踪解决方案

它旨在帮助开发者在手机游戏和其他体验中轻松实现光线追踪

今年早些时候，三星推出了首款支持硬件加速光线跟踪的 Exynos SoC。全新的 [Exynos 2200](https://www.xda-developers.com/samsung-exynos-2200/) 采用了其首款基于 AMD RDNA 2 的 GPU Xclipse 920，不仅支持移动设备上的光线跟踪，还承诺在移动游戏中实现“控制台质量”的沉浸式视觉效果。Arm [在 6 月份推出了 Immortalis-G715 GPU](https://www.xda-developers.com/arm-second-generation-armv9-ray-tracing-gpu/) ，这是其第一款支持硬件加速光线跟踪的 GPU。高通现在也在跟进其最新的旗舰芯片组，骁龙 8 代 2。在正式发布之前，Oppo 展示了其开放式光线跟踪解决方案，该解决方案将使开发人员和创作者能够在采用高通最新芯片组的设备上提供新的光线跟踪体验。

Oppo 的移动设备光线跟踪解决方案利用了 Oppo 专有的 PhysRay SDK 的修改版本，使光线跟踪技术*“能够应用于移动设备上复杂的大规模游戏场景。”*在 2022 年骁龙峰会上，Oppo 通过一款名为“Camp Guard”的第一人称射击游戏展示了其技术实力，该游戏拥有超过 2000 个物理模型、80 万个三角形和近 100 种纹理。互动演示展示了改进的阴影，灯光和反射，真实地反映了模型的运动和玩家的相机角度。Oppo 声称其第一人称射击游戏演示可以在装有骁龙 8 代 SoC 的室温设备上以每秒 60 帧的速度在 720p 分辨率下运行半小时。

在关于其新光线跟踪解决方案的新闻稿中，Oppo 指出，它与高通合作进行了*“游戏场景中的驱动程序测试、着色器优化和编译器工具开发。”*两家公司还优化了 PhysRay Engine 2.0 驱动程序，以便新的骁龙 8 Gen 2 可以流畅地渲染不同的光线跟踪效果和纹理。Oppo 的解决方案还支持高通的可变速率明暗处理(VRS)技术，这确保了 PhysRay Engine 2.0 *”可以在骁龙 8 Gen 2 上高效运行。在解决功耗问题的同时极大地提高了图形质量。”*

虽然 Oppo 的 PhysRay Engine 2.0 利用了专有的 PhysRay SDK，但它是一个完全开放的光线跟踪解决方案，可供全球所有游戏开发者和创作者使用。该公司认为，以下三个功能使其成为希望在其游戏中实现光线跟踪的游戏开发人员的绝佳选择:

*   方便:PhysRay 引擎支持光线跟踪和光栅化的混合渲染。游戏开发者可以直接添加 Oppo 的移动光线追踪管道，而无需对传统的渲染管道进行大刀阔斧的改动。
*   自适应:PhysRay 引擎不仅能够根据不同场景动态调整光线跟踪算法的复杂度和效率，而且采用了标准端口。与人工智能融合，支持物理传感器，以便将来支持全路径光线追踪等效果。开发人员可以在移动设备上不受限制地充分利用光线追踪技术，产生更加独特和令人惊讶的结果。
*   平衡:Opp 与高通技术公司的合作使 PhysRay Engine 在性能和功耗方面更加平衡。基于优质的骁龙 8 Gen 2，Oppo 的 PhysRay 引擎将其光线跟踪效率提高了 5 倍，将 CPU 工作负载减少到十分之一，并支持所有 PBR 纹理。