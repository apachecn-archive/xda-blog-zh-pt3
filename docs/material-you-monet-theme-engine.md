# Material You 的莫奈主题引擎是 Android 12 的一大亮点，下面是它的工作原理

> 原文：<https://www.xda-developers.com/material-you-monet-theme-engine/>

到目前为止， [Android 12](https://www.xda-developers.com/android-12/) 最大的变化是 [Material You](https://www.xda-developers.com/material-you/) ，这是谷歌材料设计语言的最新版本。正如谷歌描述的那样，“*寻求创造适合每一种风格的个性化设计，满足每一种需求，生动活泼，适合每一个屏幕。*“在开发 Android 12 时，谷歌创建了一个代号为“monet”的新主题引擎，它可以从用户的壁纸中生成丰富的彩色调色板[。然后，这些颜色被应用到系统的各个部分，它们的值通过用户应用程序可以调用的 API 来提供，从而让应用程序决定是否也要对其 UI 重新着色。谷歌一直在全力以赴打造“材料你”，该公司已经更新了大部分应用程序，加入了动态色彩。](https://www.xda-developers.com/android-12-wallpaper-theme/)

对于材料设计历史的速成班，它首先与 Android 5 Lollipop 一起推出，与生俱来地关注用户体验。正如谷歌所说，“材料是一个可适应的指南、组件和工具的系统，支持用户界面设计的最佳实践。”它的特色是平面、柔和的调色板、深度、柔和的灯光和逼真的物理效果。Android 9 Pie 见证了 Material Design 2 的出现，尽管它远没有第一次 Material Design 迭代那样大的视觉革新。Android 12 见证了[材质设计 3](https://material.io/blog/migrating-material-3) 的推出，这是一次更重大的大修。

然而，去掉颜色主题引擎，你的材料实际上并没有什么不同。事实上，由“你”所代表的个人因素或多或少完全消失了。

## 莫奈主题引擎的工作原理

“莫奈”主题引擎是神奇的地方，当它涉及到你的材料时，它是决定从壁纸中选择什么颜色的算法。“莫奈”在 Android 12L 中被添加到 AOSP。自定义 ROM 开发者也可以实现这个[开源实现的“Monet”](https://www.xda-developers.com/android-12-material-you-theming-system-recreated/)。第三方应用开发者现在可以自由添加对动态颜色的支持，即使它目前只能在有限的设备上运行。

我敢肯定大多数人对 Material You 的第一个问题是，它是如何选择每次都能很好地搭配和对比的颜色的。我尝试了无数的壁纸，试图打破颜色选择算法，但没有一个成功做到这一点。至少可以说，它仍然每次都能选择搭配的颜色，这是一个令人印象深刻的壮举。为了深入了解 Android 12 的颜色选择算法是如何工作的，两个复活节彩蛋中的一个以小部件的形式出现，你可以将它添加到你的桌面上。该小部件显示莫奈选择的所有颜色，您可以轻按它来全屏显示它。当它全屏显示时，您可以轻按一种颜色来共享它。共享时，输出如下所示:

```
 A1-600 (@android:color/system_accent1_600)
currently:  
```

当用户在 Android 12 设备上更改他们的壁纸时，图像被分析以选择颜色，并使用初始种子颜色通过算法选择原色、二色、三色和错误颜色。还选择了两种中性色，让材料呈现整体色调。同时，它还应用了色彩理论和可访问性规则。根据这些颜色，该算法创建从 0%亮度(黑色)到 100%亮度(白色)的色调调色板。动态主题化或自定义主题化使用这些色调调色板中的值来设置该颜色范围的主题属性。它从墙纸中提取多达 128 种颜色到 CIELAB 颜色空间作为媒介，然后这些颜色被[映射到 CAM16](https://twitter.com/jpohhhh/status/1405262496416555011) 。cam 16[**c**olor**a**appearance**m**odel](https://cs.android.com/androidx/platform/frameworks/support/+/androidx-main:core/core/src/main/java/androidx/core/content/res/CamColor.java;l=26;bpv=0)用于对颜色进行排序和过滤，以确定实际的种子颜色，然后使用该种子颜色生成调色板。之后，这些颜色被映射回 RGB，用于设置整个系统的颜色。

CIELAB 有时也被称为“L*a*b*”。L*代表感知的亮度/明度，a*和 b*代表人类视觉的四种独特颜色-红色、绿色、蓝色和黄色。亮度用于计算对比度，保证可读性。一旦应用，您就可以获得所有漂亮的系统级颜色，这些颜色可以在系统 UI、应用程序等中实现。

## 运行时资源覆盖(rro)发生了什么变化？

rro 没有去任何地方，并且您的材料通过捏造的覆盖 API 工作。在过去，我们已经讨论过[如何使用制作的覆盖图来恢复无根主题化](https://www.xda-developers.com/android-12s-fabricated-overlay-api-brings-back-rootless-themes/)。人造覆盖是 Android 12 的新功能，它们的工作方式与 RROs 略有不同。首先，rro 通过安装在设备上的叠加 APK 工作，而虚构的叠加只是告诉应用程序使用什么颜色。

制造的覆盖层也比 rro 更受限制。在 Android 11 之前，rro 可以覆盖几乎任何资源:布尔值、整数、维度、属性、布局，甚至原始数据文件。Android 11 对 rro 的工作方式做了一些改变，使得覆盖布局不再可行。另一方面，虚构的覆盖图只能覆盖可以用整数表示的值。这包括整数、维度、布尔和颜色。您不能使用它们来覆盖原始数据资源、布局、字符串或数组——至少不容易。

尽管如此，当涉及到你和莫奈的材料时，这些限制并不重要。制作的覆盖层使系统可以轻松地动态应用颜色和尺寸覆盖层，而无需等待 APK 编译或系统重启来应用。

## 你的材料仍在改进

Material You 的动态色彩当然也不是没有问题，从根本上打破它也不是那么难。例如，如果你快速更换壁纸，你可以[有效地发起拒绝服务攻击](https://www.xda-developers.com/android-12-material-you-lagging/)。米沙·拉赫曼[已经证实](https://www.reddit.com/r/Android/comments/quk192/android_12_the_ars_technica_review/hkqhd7j/)这个拒绝服务攻击已经在 Android 12L 中修复。我真诚地希望 Material You 在未来的版本中有所改进，因为虽然我喜欢它和它的概念，但它需要大量的工作。从我个人的经验来看，我觉得它的 bug 是它没有被添加到 AOSP 的部分原因...这一点，以及谷歌有效地使其成为 Pixel 系列的定时独家新闻这一事实。我最近甚至在我的谷歌 Pixel 7 Pro 上更新到 Android 13 的 12 月补丁后遇到了一个问题，后来我在 logcat 中追踪到这是由你和谷歌 Pixel launcher 的材料引起的。

令人恼火的是， [Android 12 移除了自定义字体和自定义图标选择](https://www.xda-developers.com/android-12-missing-font-icon-shape-customization/)，支持动态主题化。主题系统最初是通过 Pixel Themes 应用程序引入的，它基于 Android 的基于覆盖的主题框架。虽然 Android 12 的 Material You theming 系统更加可定制，但它没有谷歌在 Android 10 中引入的定制风格。在谷歌问题追踪器的评论中，一名谷歌员工给出了如下理由:

*“R 中的自定义样式功能(字体、图标形状、图标包和强调色)正在被我们在 s 中引入的新的动态主题功能所取代。我们认为新的动态主题功能更加现代和智能。我们希望所有用户都能享受到简单愉悦的体验。”*

谷歌似乎不太可能在未来重新推出字体和自定义图标选择。许多用户表达了他们对 Google 的 Material You changes 的失望，考虑到它有多糟糕，我完全理解为什么。我们希望谷歌改进它的实现，或者其他原始设备制造商在他们的实现中不会陷入谷歌的陷阱。

## Android 13 的变化

[谷歌为](https://www.xda-developers.com/android-13-more-material-you-color-options/) [Android 13](https://www.xda-developers.com/android-13) 的发布改进了 Material You ，首批改进之一是增加了五种额外的颜色样式。这些新的颜色风格被称为色调点，充满活力，富有表现力，SPRITZ，彩虹和水果沙拉。我们已经截图展示如下。

*   色调 _ 专色:默认材质你的颜色
*   充满活力:生成色调更丰富的调色板，色调稍有变化，二级色和背景色更加丰富多彩
*   表现力:生成具有多种突出色调的调色板，这些色调比鲜艳的色彩更丰富
*   SPRITZ:生成一个更低的调色板

Android 13 还为开发者引入了主题应用图标的功能，这样他们就可以采用系统主题。开发者可以通过在他们的应用程序中提供自适应图标和单色图标来支持这一点。启动器仍然需要支持主题图标，比如 Google Pixel 启动器。

* * *

*感谢 XDA 资深会员 [kdrag0n](https://forum.xda-developers.com/m/kdrag0n.7291478/) ，ProtonAOSP 和[一个素材 You 主题化系统](https://www.xda-developers.com/android-12-material-you-theming-system-recreated/)的再创作的开发者，对本文的帮助！*