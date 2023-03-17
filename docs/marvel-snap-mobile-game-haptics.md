# 一款手机游戏如何带给我超凡的触觉体验

> 原文：<https://www.xda-developers.com/marvel-snap-mobile-game-haptics/>

人们很容易将我们与智能手机的互动视为理所当然。每天我们拿起手机来敲击、戳戳、滑动，甚至可能偶尔按下一些物理按钮。但我认为随着时间的推移，我们已经到了不再考虑这些相互作用的地步，大多数时候，它变成了肌肉记忆。虽然我们不太想它，但当我们按下电源或音量按钮时，我们会遇到反馈，这可能会以其自身微不足道的方式感到满足。按钮移动一小段距离，直到触底，产生令人满意的触觉反应，通常伴有可听见的咔嗒声。这是很难模仿的，我们知道一些最好的公司已经尝试过了。HTC 在 U12 Plus 上进行了尝试，苹果也在 iPhone 7 上进行了尝试，iPhone 7 有一个仿 home 键。

虽然与真正的按钮相比，前面的例子可能没有提供最好的体验，但它们确实揭示了实现触觉的独特方式。在很大程度上，聪明的制造商和软件开发人员已经利用这些触觉来提供反馈或帮助强调用户的体验。Android 和 iOS 设备都略有不同，但大多数智能手机通常会对我们的动作做出一些触觉反应。一个很好的例子是当你开始使用屏幕键盘输入信息时，因为它通常会有轻微的振动，让用户知道有字母被点击了。

虽然这些回应很棒，而且我们已经感受到它们很多年了，但我真的从来没有想过它们可以走得更远。然而，最近我经历了一个潜在的小样本，它在我最意想不到的地方。

## 让游戏开始吧

我是那种更多地将智能手机作为日常生活工具的人。与我的同事不同，我很少深入研究所有的函数来揭示所有细微的复杂性。也就是说，大约一个月前，我决定尝试一下*漫威快照*，因为有大量的人在网上对此赞不绝口。我不是一个游戏玩家，所以我没有任何期望。但是我很惊讶，无论是游戏性还是它对游戏性的反应。

虽然*漫威 Snap* 被吹捧为一款具有收藏价值的纸牌游戏，但它更像是一款鼓励你去玩以获得更多纸牌的纸牌游戏。让它如此令人上瘾的是，战斗的节奏相对较快，从开始到结束最多需要三分钟。玩家可以定制他们的 12 副牌，大多数都有独特的能力。开始时，你只能使用几张卡，但是你玩得越多，你赚得就越多。这就是乐趣所在，试着在你的收藏中加入一些你认识并喜爱的漫威人物。正如你所料，这款游戏包括钢铁侠、蜘蛛侠和雷神等粉丝喜爱的角色，同时也包括 Infininaut、Swarm、Zabu 等更多不知名的角色。

人们很容易在一张卡上打上一个字符，然后就此收工，尤其是关于漫威的知名度，但当你密切关注*漫威 Snap* 时，你会意识到这些卡本身没有任何字符。是的，每张卡上都有一个物理角色，但它们大多是静态的。那么如何给这些卡片带来刺激和生命呢？

这里的执行相当巧妙。开发商第二次晚餐的特点是不同的图形效果，声音和触觉，与卡片互动，有时每当玩卡片时与游戏场互动。每个效果或动画都配有制作精良的声音，增强了效果，创造了壮观的动态体验。例如，如果你决定把浩克扔下去，你会听到一声发自内心的“浩克砸吧”的叫喊，接着卡片飞到空中，然后砸到球场上，抹去了部分区域，导致裂缝和缝隙发出氖绿色的光芒。这一切都有点难以解释，但你可以通过查看下面的简短预告片来感受我所描述的内容。

然而，触觉技术才是真正区别于许多其他移动体验的地方。它是微妙的，但总是存在的，只有当我开始真正注意时，我才注意到它是多么重要。我按下“播放”按钮，手机里的微型马达就会发出尖锐而轻柔的敲击声。然后，当我开始玩游戏时，它会再次发出隆隆声。它会形成一种富有表现力和独特的流行音乐，或者当一张牌砰的一声落在游戏场上时会有雷鸣般的轰隆声，或者你可以感觉到一把刀片切过一张牌来消灭它。每次有反馈，你都能真切地感受到每一步的分量，以及背后的目的。这些振动是为了在游戏中注入独特而难忘的互动而创造的。

这种时刻的最好例子是娜琪娅第一次投掷她的环形刀片。当他们行进时，我能感觉到武器真的在移动，当它通过每一张卡片时，戒指充满能量和脉动。投掷完成后，震动停止了。另一个是杀戮者，他在矛尖飞出之前发出喉音咆哮，刺中场上受影响的牌。你可以感觉到这些矛尖击中了你的牌，在你意识到之前，你的牌消失了，爆炸成灰尘。

## 《漫威快照》中的触觉处理一丝不苟

*漫威 Snap* 采用触觉技术，创造动作背后的感觉，赋予屏幕生命的运动，让每一次互动都充满目的性。虽然触觉在主机游戏中很常见，但它并没有太多地转化为移动设备上的游戏，尽管移动游戏非常受欢迎。我对*漫威 Snap* 提供的东西很感兴趣，并寻找其他可能有这种水平反馈的游戏。尽管我在手机上下载了十几个[最受欢迎的游戏](https://www.xda-developers.com/best-android-games/)，但令我惊讶的是，它们缺乏触觉，或者大部分是不存在的。

在玩 *Clash Royale* 的时候，移动角色到游戏场感觉很平很无聊，我以为 *CSR Racing 2* 里的赛车和换挡会感觉惊险*、*但是感觉没什么。就连 FPS 重量级*使命召唤移动*这种我确定以前玩的时候会“感觉”到枪的后坐力的游戏，也没有使用触觉。我甚至检查了其中一些游戏的设置，以确保触觉没有被禁用，对于我测试的大多数游戏来说，这甚至不是一个选项。这表明一旦你经历过，这样的事情会变得多么重要。如果你对有触觉的游戏有什么建议，请在下面的评论中告诉我们。我很想感受一下开发者是如何将这一点融入他们的游戏中的。

我从来没有想过这么多年后我会在移动设备上体验如此令人耳目一新的东西，令人惊讶的是，它来自一个所有地方的游戏。这让我想要发现更多这方面的东西，无论是来自其他手机游戏，还是只是 Android 和 iOS 的原生部分。随着移动行业[停滞](https://www.xda-developers.com/smartphones-even-more-boring-next-year/)相当长一段时间，以及有传言称一些手机可能[远离物理按键](http://www.xda-developers.com/iphone-15-pro-drop-physical-volume-power-buttons/)，这可能成为公司重新审视和专注于触觉的完美风暴，以试图增强和提升体验。