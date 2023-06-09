# 谷歌和索尼联手在 Android 中添加 360°现实音频支持

> 原文：<https://www.xda-developers.com/google-sony-360-reality-audio-support-android/>

索尼基于 MPEG-H 3D 音频编解码器开发 360°现实音频技术已经有一段时间了。这项技术主要限于索尼自己的一些智能手机，并且只适用于兼容的应用程序，但现在看来，更广泛的 360°现实音频支持可能会出现在 Android 上。

Android 开源项目中的[系列代码审查](https://android-review.googlesource.com/q/topic:360RA)提到了[360°现实音频](https://www.sony.com/electronics/360-reality-audio)，代码由索尼和谷歌的开发者提交。其中一些工作是为 Android 的 MPEG4Extractor 系统组件带来 MPEG-H 3D 支持，而其他代码则是专门针对索尼的 360°现实音频。

还有[对索尼](https://android-review.googlesource.com/c/platform/frameworks/base/+/1669510/1#message-0d2c3c1c419a412dcc37308dd9c23daeec55862e)软件工程师[村山圭的代码审查的评论](https://www.linkedin.com/in/%E6%95%AC-%E6%9D%91%E5%B1%B1-7788764a/)，这似乎证实了这是谷歌和索尼之间的合资企业。“这是谷歌和索尼在 Android OS 360RA 支持’会议上提到的补丁之一，”它说。

索尼 360 Reality Audio 目前需要音乐提供商明确支持，以及兼容的扬声器或耳机。索尼的网站将亚马逊音乐高清版、Nugs.net 和 Tidal 列为唯一提供 360°现实音轨的音乐流媒体服务。虽然这项技术可以与任何耳机或扬声器配合使用，但 3D 效果将在为 360 Reality Audio 打造的扬声器中最为明显，如[索尼的 SRS-RA5000 扬声器](https://www.sony.com/electronics/wireless-speakers/srs-ra5000)、[亚马逊 Echo Studio](https://www.amazon.com/echostudio?tag=xda-3mi3l72-20&ascsubtag=UUxdaUeUpU1837&asc_refurl=https%3A%2F%2Fwww.xda-developers.com%2Fgoogle-sony-360-reality-audio-support-android%2F&asc_campaign=Short-Term) 和[森海塞尔 Ambeo Soundbar](https://sennheiser.com/ambeo-soundbar) 。

谷歌和索尼之间正在进行的工作意味着 Android 将获得一个内置的 MPEG-H 3D 音频解码器，因此任何应用程序都将更容易添加 3D 音频播放。与已经拥有 360 Reality Audio 的应用程序一样，你不一定需要特殊的耳机或扬声器——其中一条评论提到，v irtualizer " 可以将来自这些通道的单个声音放在任何耳机上的 360 球形声场中。

我们希望这些变化能够及时完成，以便与 Android 12 一起发布，否则我们很可能要等到明年才能在 Android 中获得增强的 3D 音频。

*感谢 XDA 公认的开发者 [luca020400](https://forum.xda-developers.com/m/luca020400.5778309/) 的提示！*