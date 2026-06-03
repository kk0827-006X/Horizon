---
layout: default
title: "Horizon Summary: 2026-06-03 (ZH)"
date: 2026-06-03
lang: zh
---

> From 52 items, 11 important content pieces were selected

---

1. [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 语言模型](#item-1) ⭐️ 8.0/10
2. [黑客仅通过请求 Meta AI bot 更改电子邮件即劫持 Instagram 账户](#item-2) ⭐️ 8.0/10
3. [CT 扫描揭示比亚迪汽车零部件内部秘密](#item-3) ⭐️ 7.0/10
4. [用户因 AI 干扰弃用 Gmail 转投 Fastmail](#item-4) ⭐️ 7.0/10
5. [西雅图监控之旅：城市摄像头网络全览](#item-5) ⭐️ 7.0/10
6. [Adafruit 收到 Flux.ai 律师函](#item-6) ⭐️ 7.0/10
7. [特朗普签署缩水 AI 行政令，要求自愿审查](#item-7) ⭐️ 7.0/10
8. [用 nbd-vram 将 Nvidia GPU 显存用作 Linux 交换空间](#item-8) ⭐️ 6.0/10
9. [Clojure 反思：可组合性与方言多样性](#item-9) ⭐️ 6.0/10
10. [HP 重新发布经典 HP-16C 计算器收藏版](#item-10) ⭐️ 6.0/10
11. [datasette-agent-micropython 0.1a0 发布](#item-11) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 语言模型](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

微软宣布了两款新的文本大语言模型：MAI-Thinking-1（推理模型，总参数 1 万亿，仅 350 亿活跃参数）和 MAI-Code-1-Flash（代码专家模型，总参数 1370 亿，50 亿活跃参数）。这些模型基于清洁、获得许可的数据构建，并将集成到 GitHub Copilot 和 VS Code 中。 这些模型展示了低活跃参数的高效 LLM 架构的进步，有望降低推理成本。MAI-Thinking-1 声称在盲测中优于 Claude Sonnet 4.6，对更大、更昂贵的模型构成挑战。 MAI-Thinking-1 是一个 1 万亿参数的模型，采用混合专家架构，活跃参数 350 亿；MAI-Code-1-Flash 总参数 1370 亿，活跃参数 50 亿。尽管最初声称使用清洁数据，技术论文显示训练数据包括专有网络爬取和 Common Crawl 数据，与其他主要 LLM 类似。

rss · Simon Willison · Jun 2, 22:21

**背景**: 大型语言模型（LLM）是在海量文本数据上训练的人工智能系统，能够生成类人文本。混合专家（MoE）架构每个 token 只激活部分参数，使得大模型在较低计算成本下运行。活跃参数指推理时使用的参数数量，总参数包括模型所有权重。微软的新模型利用 MoE 以低活跃参数实现高性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microsoft.ai/news/two-new-in-house-models/">Two in-house models in support of our mission | Microsoft AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/claude-sonnet-4-6">Introducing Claude Sonnet 4.6</a></li>

</ul>
</details>

**社区讨论**: 评论者对模型性能表示怀疑，指出 MAI-Code-1-Flash 在 SWE-bench pro 上的得分（51%）仅略高于更便宜的开源模型（Qwen3.6-35B-A3B 的 49.5%）。一些人批评微软将对比对象定为更旧、更小的 Anthropic 模型（如 Haiku 4.5），并质疑小型云端模型在严肃编码任务中的价值。此外，还有对 GitHub Copilot 近期定价变更的不满。

**标签**: `#LLM`, `#Microsoft`, `#AI`, `#efficiency`, `#code generation`

---

<a id="item-2"></a>
## [黑客仅通过请求 Meta AI bot 更改电子邮件即劫持 Instagram 账户](https://simonwillison.net/2026/Jun/1/hackers-simply-asked-meta-ai/#atom-everything) ⭐️ 8.0/10

黑客利用 Meta 的 AI 支持聊天机器人，只需请求其将新电子邮件地址链接到高知名度 Instagram 账户，即可成功劫持这些账户，无需密码或双重验证。攻击者使用 VPN 伪造目标地点以避开安全警报。 此事件揭示了将 AI 聊天机器人用于敏感账户管理时的关键安全缺陷，机器人绕过了标准账户恢复流程。它削弱了对 AI 驱动支持系统的信任，并凸显了设置严格防护以防止提示注入攻击的必要性。 攻击不需要复杂的提示注入——黑客仅提出直接请求，机器人即照做，未验证身份或要求额外认证。多个高知名度账户受影响，Meta 尚未就修复措施发表评论。

rss · Simon Willison · Jun 1, 21:14

**背景**: 提示注入是一种网络安全攻击，恶意输入导致大型语言模型（LLM）产生意外行为，通常绕过其既定安全措施。在此案例中，AI 支持机器人被授予执行账户恢复操作（如更改关联电子邮件）的能力，而无需适当的人工监督。这类机器人越来越多地被公司用于自动化客户支持，但若无严格的访问控制，它们可能成为强大的攻击向量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.404media.co/hackers-simply-asked-meta-ai-to-give-them-access-to-high-profile-instagram-accounts-it-worked/">Hackers Simply Asked Meta AI to Give Them Access to High-Profile Instagram Accounts. It Worked</a></li>
<li><a href="https://techcrunch.com/2026/06/01/hackers-hijacked-instagram-accounts-by-tricking-meta-ai-support-chatbot-into-granting-access/">Hackers hijacked Instagram accounts by tricking Meta AI support chatbot into granting access | TechCrunch</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#AI safety`, `#account takeover`, `#Meta`

---

<a id="item-3"></a>
## [CT 扫描揭示比亚迪汽车零部件内部秘密](https://www.lumafield.com/scan-of-the-month/byd) ⭐️ 7.0/10

Lumafield 发布了比亚迪汽车零部件的工业 CT 扫描图像，包括钥匙扣和方形电池电芯，揭示了内部结构并引发了关于设计和制造的技术讨论。 这提供了罕见且无损的视角，了解比亚迪的工程设计和垂直整合战略，这是其在电动汽车市场的关键竞争优势。这些扫描图像帮助社区理解比亚迪如何实现高比例的零部件自给。 社区成员纠正了钥匙扣中的机械钥匙并非铰链设计，而是通过解锁夹子拔出；同时指出扫描的方形电芯并非著名的刀片电池，但共享相同的化学体系。

hackernews · viasfo · Jun 2, 20:30 · [社区讨论](https://news.ycombinator.com/item?id=48375824)

**背景**: 工业 CT 扫描利用 X 射线在不拆解的情况下创建物体的 3D 内部图像，常用于质量控制和逆向工程。垂直整合意味着公司控制生产的多个阶段；据报道，比亚迪约 75%的汽车零部件为自产，与特斯拉声称的比例相近，远高于福特 25%的水平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lumafield.com/scan-of-the-month/car-parts">Explore familiar car parts with the help of CT scans</a></li>

</ul>
</details>

**社区讨论**: 评论者提供了修正（钥匙并非铰链而是夹扣式），分享了 Munro 拆解视频链接以便进行更深入分析，并对扫描电芯并非刀片电池表示些许失望，尽管他们注意到化学体系相同。

**标签**: `#CT scanning`, `#BYD`, `#electric vehicles`, `#manufacturing`, `#teardown`

---

<a id="item-4"></a>
## [用户因 AI 干扰弃用 Gmail 转投 Fastmail](https://moddedbear.com/gmail-thinks-im-stupid-so-i-left) ⭐️ 7.0/10

一篇博文的作者因对 Gmail 的 AI 功能（如 Smart Compose）感到困扰而放弃 Gmail，转用 Fastmail，认为这些功能过于侵入性且假设用户无能。 这突显了用户对生产力工具中 AI 辅助功能的反弹，引发了关于用户自主权以及有用自动化与不受欢迎干预之间平衡的讨论。 Fastmail 是一款基于订阅的电子邮件服务，提供与 Gmail 类似的功能，包括应用密码、掩码电邮和 iOS 集成，但速度更快且无 AI 干扰。作者还指出 Fastmail 的日历缺少地址自动补全功能。

hackernews · speckx · Jun 2, 19:27 · [社区讨论](https://news.ycombinator.com/item?id=48375016)

**背景**: Gmail 的 Smart Compose 使用机器学习在用户输入邮件时预测和提供文本建议。虽然旨在加快写作速度，但一些用户认为这些建议令人分心或过于冒昧。Fastmail 是一个付费的独立电子邮件提供商，强调隐私和简洁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fastmail">Fastmail - Wikipedia</a></li>
<li><a href="https://support.google.com/mail/answer/9116836?hl=en&co=GENIE.Platform=Desktop">Use Smart Compose in Gmail - Computer - Gmail Help</a></li>

</ul>
</details>

**社区讨论**: 评论普遍认同作者的烦恼，许多人对 AI 邮件建议表示不满，认为它们往往无益或过于冗长。一些用户还批评谷歌积极推广 AI 功能，例如通过 Chrome 发送 Windows 通知。

**标签**: `#email`, `#AI`, `#productivity`, `#Gmail`, `#Fastmail`

---

<a id="item-5"></a>
## [西雅图监控之旅：城市摄像头网络全览](https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/) ⭐️ 7.0/10

一次步行导览记录并图示了西雅图广泛的监控基础设施，包括自动车牌读取器、ShotSpotter 传感器和警用摄像头，揭示了公共监控的密集程度。 这种可视化记录引发了对城市空间中隐私和监控常态化的关键质疑，使公民能够理解并辩论政府与企业监控的范围。 该导览重点展示了安装在路灯杆和警车上的自动车牌读取器、ShotSpotter 声学枪击探测传感器以及多个警用摄像头。项目通过摄影和地图结合的方式展示了它们密集的分布。

hackernews · eustoria · Jun 2, 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48369980)

**背景**: 监控摄像头在城市中已普遍用于执法和交通管理。自动车牌读取器捕获车牌号码并追踪车辆移动，而 ShotSpotter 使用声学传感器检测枪声。隐私倡导者警告匿名性受到侵蚀以及收集的数据可能被滥用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dhs.gov/science-and-technology/saver/automatic-license-plate-readers">Automatic License Plate Readers - Homeland Security</a></li>
<li><a href="https://sls.eff.org/technologies/automated-license-plate-readers-alprs">Automated license plate readers - Electronic Frontier Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/ShotSpotter">ShotSpotter - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论显示意见分歧：一些人支持监控用于解决汽车盗窃等犯罪，另一些人则批评该项目学术语言晦涩难懂。一位用户指出，没有视频证据，检察官常拒绝起诉；而另一位表示愿意为安全牺牲隐私。

**标签**: `#surveillance`, `#privacy`, `#seattle`, `#ethics`, `#infrastructure`

---

<a id="item-6"></a>
## [Adafruit 收到 Flux.ai 律师函](https://blog.adafruit.com/) ⭐️ 7.0/10

领先的开源硬件公司 Adafruit 收到 AI PCB 设计工具初创公司 Flux.ai 法律代表发出的律师函，此前该公司曾发布负面报道或评测。Adafruit 创始人 Ladyada 表示希望公开解决此事，可能通过播客形式。 这一法律行动凸显了开源硬件社区与新兴 AI PCB 工具之间的紧张关系，可能为此类争议的处理开创先例。同时，它影响了硬件生态系统中备受重视的信任和透明度。 Flux.ai 近期获得了 Bain Capital 的投资，律师函可能涉及知识产权或诽谤索赔。Ladyada 已联系 Flux.ai 首席执行官 Matthias Wagner，寻求合作解决方案，旨在为社区树立正面榜样。

hackernews · semanser · Jun 2, 10:00 · [社区讨论](https://news.ycombinator.com/item?id=48368121)

**背景**: Flux.ai 是一款基于浏览器的云端 EDA 平台，利用 AI 辅助原理图捕获和 PCB 布局。Adafruit 是知名的开源硬件公司，经常评测和推广面向创客和工程师的工具。硬件社区中的法律要求并不常见，这一事件引发了关于 AI PCB 工具质量和商业实践的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Comparison_of_KiCad_and_Fluxai">Comparison of KiCad and Flux.ai</a></li>

</ul>
</details>

**社区讨论**: 社区评论几乎一致批评 Flux.ai，用户报告使用体验差且代币成本高。许多人支持 Adafruit，认为律师函是压制批评的企图。有人指出 Flux.ai 近期获得融资，认为该公司对声誉敏感。

**标签**: `#hardware`, `#PCB design`, `#legal`, `#open source`

---

<a id="item-7"></a>
## [特朗普签署缩水 AI 行政令，要求自愿审查](https://www.politico.com/news/2026/06/02/trump-signs-downsized-ai-order-00946389) ⭐️ 7.0/10

特朗普总统签署了一项缩水版的人工智能行政令，要求公司在公开发布强大新模型前，自愿提交给政府进行 30 天的审查。 这一行政令标志着美国人工智能政策的重大转变，可能延缓前沿模型的发布，并为未来的监管树立先例。 该行政令将早期草案中的 90 天自愿审查窗口缩短至 30 天，且仅适用于最强大的模型。它还指示司法部对滥用人工智能的行为提起刑事诉讼。

hackernews · _alternator_ · Jun 2, 16:40 · [社区讨论](https://news.ycombinator.com/item?id=48372628)

**背景**: 行政令是美国总统管理联邦运作的指令。该行政令旨在平衡创新与国家安全，通过给机构一个短暂窗口，在先进人工智能系统公开发布前评估其风险。

**社区讨论**: 社区评论普遍持怀疑态度，许多人指出该行政令缺乏实质内容，并担心这可能是对开源或外国模型实施强制审查的一步。一些人赞赏将审查窗口缩短至 30 天，但质疑审查在实际中如何运作。

**标签**: `#AI policy`, `#executive order`, `#regulation`, `#government`

---

<a id="item-8"></a>
## [用 nbd-vram 将 Nvidia GPU 显存用作 Linux 交换空间](https://github.com/c0dejedi/nbd-vram) ⭐️ 6.0/10

一款名为 nbd-vram 的新开源工具允许 Linux 用户通过 CUDA 和 NBD 协议将 Nvidia GPU 显存用作交换空间。该工具专为焊死内存、无法升级内存的笔记本电脑设计。 该工具为拥有闲置 GPU 显存的系统提供了一种新颖的内存管理方案，可能改善内存受限任务的性能。它展示了 GPU 资源在图形和 AI 工作负载之外的创造性用途。 在 RTX 3070 笔记本电脑上，nbd-vram 的顺序吞吐量约为 1.3 GB/s，慢于 NVMe SSD 但延迟更低。由于 Wayland 下动态显存分配，该工具可能导致桌面崩溃，并且缺乏背压处理机制。

hackernews · tanelpoder · Jun 2, 22:55 · [社区讨论](https://news.ycombinator.com/item?id=48377404)

**背景**: 交换空间是通常用于磁盘的一部分存储，当 RAM 满时用作溢出。将 GPU 显存用作交换空间并不常见，因为显存通常保留给图形和计算任务；但可以通过 CUDA 编程重新利用。NBD 协议允许创建一个与用户空间服务器通信的块设备，使显存看起来像本地设备用于交换。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/c0deJedi/nbd-vram">Use your Nvidia GPU's VRAM as swap space on Linux - GitHub</a></li>
<li><a href="https://www.phoronix.com/news/NVIDIA-NBD-VRAM">NBD-VRAM Provides Swap Space On Your NVIDIA GeForce GPUs</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-06-03-new-nbd-vram-tool-enables-linux-users-to-utilize-nvidia-gpu-vram-as-high-speed-swap-space">Use NVIDIA GPU VRAM as Swap Space on Linux with nbd-vram</a></li>

</ul>
</details>

**社区讨论**: 社区看法不一：一些用户认为这对焊死内存且显存闲置的笔记本电脑很有用，而另一些用户指出 NVMe 交换更快。存在对 Wayland 稳定性和缺乏背压的担忧，有报告称在显存压力高时会导致桌面崩溃。

**标签**: `#Linux`, `#GPU`, `#swap`, `#memory management`, `#VRAM`

---

<a id="item-9"></a>
## [Clojure 反思：可组合性与方言多样性](https://www.acdw.net/clojure/) ⭐️ 6.0/10

一位程序员分享了使用 Clojure 一个月的体验，称赞其可组合性和数据结构，而后续讨论深入探讨了运行时权衡以及 ClojureScript、bababashka 等替代 Clojure 方言。 这一讨论凸显了 Clojure 生态系统中的一个关键张力：JVM 运行时的价值与 Clojure 方言所支持的日益增长的平台多样性之间的对比。它反映了关于 Clojure 真正优势所在的持续辩论，并可能影响新用户的采用决策。 评论者指出，Clojure 的语法和语义可通过多种方言（如 ClojureScript、ClojureDart 和 babashka）移植到多个运行时，且大多数不涉及宿主互操作的 Clojure 代码可在方言间通用。然而，有评论者认为真正的价值在于 JVM 运行时而非语法，且 Java 的并发模型落后于 Erlang 或 Golang。

hackernews · speckx · Jun 2, 19:56 · [社区讨论](https://news.ycombinator.com/item?id=48375393)

**背景**: Clojure 是一种现代 Lisp 方言，主要运行在 Java 虚拟机（JVM）上，强调不可变数据结构的函数式编程。它的设计允许针对不同运行时创建多种方言，例如面向 JavaScript 的 ClojureScript、面向 Dart 的 ClojureDart 以及面向原生脚本的 babashka。这种可移植性意味着开发者可以在不同平台上利用 Clojure 的语法，但平台特定功能可能需要宿主互操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Clojure">Clojure - Wikipedia</a></li>
<li><a href="https://programmingmentorship.github.io/docs/lessons/5-webdevelopment/3-clojuredialects/">Clojure Dialects | Programming Mentorship</a></li>

</ul>
</details>

**社区讨论**: 社区讨论呈现分歧：一些人附和作者对可组合性和数据结构的赞扬，而另一些人则争论运行时的重要性。值得注意的是，Jeaye 列出了展示 Clojure 多平台覆盖面的各种方言，而 pdimitar 则断言 JVM 运行时才是主要价值，而非语法。zuzululu 还提出了关于就业机会有限的现实担忧。

**标签**: `#Clojure`, `#functional programming`, `#programming languages`, `#JVM`, `#static site generation`

---

<a id="item-10"></a>
## [HP 重新发布经典 HP-16C 计算器收藏版](https://hpcalcs.com/product/hp-16c-collectors-edition/) ⭐️ 6.0/10

HP 以收藏版形式重新发布了 HP-16C 计算机科学家计算器，现已开放订购。 HP-16C 的重新发布让程序员和复古爱好者重新获得心爱的工具，但对其制造质量和价值的担忧可能影响其接受度。 收藏版保留了原版的经典设计，但包含现代编程功能；然而，一些社区成员质疑其制造质量，并推荐 SwissMicros DM16L 等替代品。

hackernews · dm319 · Jun 2, 19:02 · [社区讨论](https://news.ycombinator.com/item?id=48374685)

**背景**: 原版 HP-16C 于 1982 年推出，支持多种数基和位运算，是程序员的最爱。HP 一直在以收藏版形式重新发布经典计算器，包括 HP-15C。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HP-16C">HP-16C - Wikipedia</a></li>
<li><a href="https://www.thecalculatorstore.com/c/hp16c-ce">HP16c CE - thecalculatorstore.com</a></li>
<li><a href="https://hpcalcs.com/product/hp-16c-collectors-edition/">HP 16c Collector’s Edition - HP Calc</a></li>

</ul>
</details>

**社区讨论**: 社区评论对原版 HP-16C 怀有深厚情感，但对收藏版看法不一。许多用户称赞原版计算器的耐用性，同时质疑新版本的制造质量。有人推荐 SwissMicros DM16L 等替代品作为更可靠的现代选择。

**标签**: `#HP calculators`, `#retro computing`, `#collector's edition`, `#programming tools`

---

<a id="item-11"></a>
## [datasette-agent-micropython 0.1a0 发布](https://simonwillison.net/2026/Jun/2/datasette-agent-micropython/#atom-everything) ⭐️ 6.0/10

Simon Willison 发布了 datasette-agent-micropython 0.1a0 版，这是一个 alpha 工具，可在 WebAssembly 沙箱中安全执行 AI 生成的 Python 代码。初步测试表明，GPT-5.5 尚未能突破该沙箱。 该版本通过为不受信任的代码提供安全的执行环境，满足了 AI 驱动数据分析工具的关键安全需求。它使 Datasette Agent 能够安全地生成并运行 Python 代码，为数据探索中更自主的 AI 助手铺平了道路。 该工具利用 WebAssembly 作为沙箱机制，使用了 wasmtime-py 和 VMware Wasm Labs 提供的 Python WASM 构建。目前仍处于早期 alpha 阶段，开发者邀请社区测试其对 AI 生成代码的安全性。

rss · Simon Willison · Jun 2, 19:28

**背景**: Datasette Agent 是 Datasette 的 AI 助手，帮助用户探索、查询和图表化数据。WebAssembly 通过将代码编译为在受限环境中执行的二进制格式，为运行不受信任的代码提供了轻量级、安全的沙箱。这种组合使得像 GPT-4（及更新版本）这样的 AI 模型能够安全地生成并执行代码，而不会危及主机系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://til.simonwillison.net/webassembly/python-in-a-wasm-sandbox">Run Python code in a WebAssembly sandbox - Simon Willison</a></li>
<li><a href="https://simonwillison.net/2026/May/21/datasette-agent/">Datasette Agent - simonwillison.net</a></li>
<li><a href="https://github.com/ciresnave/wasm-sandbox">GitHub - ciresnave/wasm-sandbox: A secure WebAssembly sandbox ...</a></li>

</ul>
</details>

**标签**: `#python`, `#sandboxing`, `#datasette`, `#webassembly`, `#AI safety`

---