# 此应用程序允许您列出手机支持的 Camera2 和 CameraX 扩展

> 原文：<https://www.xda-developers.com/camerax-info-list-camera2-extensions-database/>

谈到设备，Android 用户有许多选择，有各种规格、功能，当然还有预算。不仅是老顾客被选择宠坏了，而且当涉及到不容易测量和比较的功能时，这也使资深用户感到困惑。以相机性能为例。得益于改进的硬件和计算摄影技术，Android 端因拥有市场上一些最好的智能手机摄像头而赢得了声誉。也就是说，Android 相机处理的当前状态远不是一个开放的标准，不同 OEM 厂商之间的情况变得更加复杂。

如果您必须比较两个不同的原始设备制造商如何在其产品组合中向第三方相机应用程序展示库存相机功能，答案可能不容易找到。现在，扎克里·旺德，又名 XDA 公认的开发者[扎克里·1](https://forum.xda-developers.com/m/zacharee1.7055541/)已经承担起自己的责任，通过建立一个来自不同 Android 设备的相机数据数据库来补救这种情况，该数据库专注于它们的整体能力。认识一下 **CameraX Info** ，这是一个轻量级应用程序，用于列举支持的 Camera2 和 CameraX 扩展以及其他与相机相关的功能。

对于外行来说，谷歌的 CameraX 库旨在简化 Android 上的相机应用程序开发过程。在引擎盖下，它包装了 [Camera2](https://www.xda-developers.com/camera2-api/) ，这是一个 API，允许应用程序探测设备上的相机功能，前提是 OEM 将这些相机功能暴露给 API。为了减少相机功能碎片，设备制造商可以选择在手机中附带 CameraX 兼容的扩展库，允许第三方开发人员无缝利用原生相机功能。

如果你不是开发人员，但仍然想知道你手机的普通相机应用程序的散景效果是否也适用于第三方相机应用程序，该怎么办？这就是 CameraX Info 派上用场的地方。无需修改任何代码，因为该应用程序将列出所有支持的 CameraX/Camera2 扩展和主相机和自拍相机显示的其他功能(如 ARCore)。更有趣的是，该应用程序还提供了一个在线数据库，用户可以匿名上传、浏览和下载 JSON 格式的不同设备和 Android 版本的相机支持数据。

以下是 CameraX Info 提供的功能列表:

*   查看 Camera2 扩展支持。
*   查看 CameraX 扩展支持。
*   查看检测到的逻辑和物理摄像机及其基本规格。
*   匿名上传您的相机数据。
*   匿名查看摄像头数据。
*   查看 ARCore 支持。

如果你有兴趣探索你的 Android 手机的相机功能，给 CameraX Info 一个机会。app 本身是开源的，源代码[可在开发者的 GitHub 简介](https://github.com/zacharee/CameraXInfo)上获得。

* * *

*特色图片:一加 10 Pro 和三星 Galaxy S22 Ultra 的后置摄像头。*