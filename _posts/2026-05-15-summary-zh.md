---
layout: default
title: "Horizon Summary: 2026-05-15 (ZH)"
date: 2026-05-15
lang: zh
---

> From 46 items, 15 important content pieces were selected

---

1. [首个公开的苹果 M5 内核漏洞绕过 MTE](#item-1) ⭐️ 9.0/10
2. [vLLM 0.21.0 发布，包含破坏性变更和新后端](#item-2) ⭐️ 8.0/10
3. [拆除 RAV4 调制解调器和 GPS 阻止远程信息收集](#item-3) ⭐️ 8.0/10
4. [RTX 5090 外接 GPU 在 M4 MacBook Air 上：游戏与 LLM 突破](#item-4) ⭐️ 8.0/10
5. [新 Nginx 漏洞 可绕过 ASLR](#item-5) ⭐️ 8.0/10
6. [arXiv 因 AI 幻觉引用封禁作者一年](#item-6) ⭐️ 8.0/10
7. [硬盘固件黑客技术深度解析](#item-7) ⭐️ 8.0/10
8. [Amazonbot 终于遵守 robots.txt](#item-8) ⭐️ 7.0/10
9. [AI 编程代理降低技术锁定风险](#item-9) ⭐️ 7.0/10
10. [批评‘11 个 AI 智能体’的说法毫无意义](#item-10) ⭐️ 7.0/10
11. [美国法官审查 Anthropic 15 亿美元版权和解协议](#item-11) ⭐️ 7.0/10
12. [Codex 现已集成到 ChatGPT 移动应用](#item-12) ⭐️ 6.0/10
13. [Mitchell Hashimoto：编程语言如今可替代](#item-13) ⭐️ 6.0/10
14. [Datasette IP 速率限制插件 0.1a0 发布](#item-14) ⭐️ 6.0/10
15. [Simon Willison 的 CSP 允许列表实验](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [首个公开的苹果 M5 内核漏洞绕过 MTE](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

Calif 公开了针对苹果 M5 芯片的首个内核内存破坏漏洞利用，成功绕过了内存标记扩展（MTE）安全特性。 该漏洞利用展示了苹果最新 M5 芯片的重大安全缺陷，可能影响数百万 macOS 用户，并对 MTE 作为缓解措施的有效性提出质疑。 该漏洞利用针对 macOS 内核的内存破坏，并绕过了旨在防止此类攻击的硬件安全特性 MTE。一份 55 页的报告详细说明了这一发现。

hackernews · quadrige · May 14, 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48139219)

**背景**: 内存标记扩展（MTE）是一种 ARM 硬件安全特性，通过为内存分配分配标签来检测缓冲区溢出和释放后使用错误。苹果 M5 芯片是 Mac 上最新的基于 ARM 的 SoC，是 M4 的继任者。该漏洞利用首次展示了在苹果芯片上实际绕过 MTE 的方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://source.android.com/docs/security/test/memory-safety/arm-mte">Arm memory tagging extension | Android Open Source Project</a></li>
<li><a href="https://8ksec.io/arm64-reversing-and-exploitation-part-10-intro-to-arm-memory-tagging-extension-mte/">ARM64 Reversing Part 10: Intro to ARM MTE | 8kSec</a></li>
<li><a href="https://grokipedia.com/page/Apple_M5">Apple M5</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了敬畏和怀疑的混合情绪：一些人称赞技术成就，并推测漏洞赏金可能高达 150 万美元，而另一些人质疑缺乏公开的技术细节。一条讽刺评论将其与虚假漏洞相提并论，还有用户后悔因安全特性购买了 M5。

**标签**: `#macOS`, `#kernel exploit`, `#Apple M5`, `#memory corruption`, `#security`

---

<a id="item-2"></a>
## [vLLM 0.21.0 发布，包含破坏性变更和新后端](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

vLLM 0.21.0 已发布，包含来自 202 位贡献者的 367 次提交。它废弃了 transformers v4，要求 C++20，将 KV offload 与混合内存分配器集成，并为 Blackwell GPU 引入了 TOKENSPEED_MLA 注意力后端。 这对于广泛使用的 LLM 推理库来说是一次重要发布，引入了重大的性能和内存改进。破坏性变更需要迁移工作，但能够支持更新的硬件和更大的模型。 KV offloading 子系统现在使用带滑动窗口组支持的混合内存分配器，提高了内存效率。TOKENSPEED_MLA 后端利用专有内核，在 Blackwell GPU 上为 DeepSeek-R1/Kimi-K25 模型提供最佳性能。

github · khluu · May 14, 23:15

**背景**: KV 缓存卸载将注意力键值数据从 GPU 移动到 CPU 内存，以释放 GPU 资源。与固定块分配器相比，混合内存分配器减少了内存浪费。TokenSpeed 是一个高性能推理引擎，为 Blackwell 提供了优化的 MLA 内核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bentoml.com/llm/inference-optimization/kv-cache-offloading">KV cache offloading | LLM Inference Handbook</a></li>
<li><a href="https://github.com/lightseekorg/tokenspeed">GitHub - lightseekorg/tokenspeed: TokenSpeed is a speed-of-light LLM inference engine. · GitHub</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#GPU`, `#transformers`, `#release`

---

<a id="item-3"></a>
## [拆除 RAV4 调制解调器和 GPS 阻止远程信息收集](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/) ⭐️ 8.0/10

一篇详细指南发布了，指导如何从 2024 款丰田 RAV4 混合动力车上移除蜂窝调制解调器和 GPS 接收器，以防止车辆向丰田发送远程信息数据。 此事很重要，因为现代汽车越来越多地收集和共享驾驶员数据，往往未经明确同意；该指南为注重隐私的车主提供了一种实用的 DIY 方法来停止数据传输。 移除调制解调器后，通过蓝牙连接手机仍会让汽车利用手机的互联网连接发送远程信息；但使用有线 USB CarPlay 不会触发此行为。

hackernews · arkadiyt · May 14, 17:08 · [社区讨论](https://news.ycombinator.com/item?id=48138136)

**背景**: 现代车辆包含一个带有蜂窝调制解调器和 GPS 的远程信息控制单元（TCU），持续收集位置、速度、驾驶行为等数据。这些数据通常与制造商和第三方共享，引发隐私担忧。物理移除或断开 TCU 是实现无法传输远程信息的网络隔离车辆的一种方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rav4world.com/threads/how-to-fully-disable-telemetry-and-have-an-air-gapped-car.343029/">How to fully disable telemetry and have an "air-gapped" car | Toyota RAV4 Forums</a></li>
<li><a href="https://en.wikipedia.org/wiki/Telemetry">Telemetry - Wikipedia</a></li>
<li><a href="https://disappearme.ai/blog/car-reporting-complete-guide-disabling-vehicle-telemetry-data-collection-2025">Disable Car Data Collection: Complete Brand-by-Brand Guide to Vehicle Telemetry</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，拆除调制解调器后，蓝牙连接仍可能通过手机泄露数据，而 CarPlay 本身也会收集车辆远程信息。一位用户希望进行此改装以修复 CarPlay 中的 GPS 指南针问题，但丰田拒绝处理。另一人指出，2024 款福特 Maverick 可通过拔掉一个保险丝来禁用远程信息单元。

**标签**: `#privacy`, `#car telemetry`, `#Toyota RAV4`, `#DIY`, `#GPS`

---

<a id="item-4"></a>
## [RTX 5090 外接 GPU 在 M4 MacBook Air 上：游戏与 LLM 突破](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 8.0/10

一位开发者成功将 NVIDIA RTX 5090 外接 GPU 连接到 M4 MacBook Air，通过自定义虚拟机设置，展示了可运行游戏并大幅提升 LLM 推理性能。 这一成就挑战了苹果关于 Apple Silicon 不支持外接 GPU 的官方立场，为 Mac 游戏和本地 AI 工作负载开辟了新可能，尤其适合在便携设备上需要高 GPU 性能的用户。 该方案依赖带 GPU 直通的虚拟机，绕过了 macOS 的限制；但受限于苹果 1.5 GB 的 DMA 传输内存窗口。外接 GPU 显著加速了 LLM 提示预填充阶段，而这是 Apple Silicon 上已知的瓶颈。

hackernews · allenleee · May 14, 15:47 · [社区讨论](https://news.ycombinator.com/item?id=48137145)

**背景**: eGPU（外接 GPU）通过 Thunderbolt 将桌面显卡连接到笔记本电脑，通常用于提升图形性能。苹果官方仅对 Intel 版 Mac 支持 eGPU，且仅限 AMD 显卡。Apple Silicon Mac 因统一内存架构缺乏官方 eGPU 支持。LLM 推理分为预填充（提示处理）和解码（生成 token）两个阶段；预填充对内存带宽要求高，在 Mac 上通常较慢。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-us/102363">Use an external graphics processor with your Mac - Apple Support</a></li>
<li><a href="https://www.linkedin.com/pulse/external-graphics-processing-unit-egpu-real-world-5-uses-zpfff">External Graphics Processing Unit Egpu in the Real World: 5 Uses...</a></li>
<li><a href="https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/">Mastering LLM Techniques: Inference Optimization | NVIDIA Technical...</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常积极，称赞这一技术成就及其对 LLM 工作负载的实际意义。评论者注意到该方案复杂度高，并希望获得苹果官方支持，同时也指出了 1.5 GB 内存窗口仍存在的限制。

**标签**: `#eGPU`, `#Apple Silicon`, `#Mac gaming`, `#RTX 5090`, `#LLM inference`

---

<a id="item-5"></a>
## [新 Nginx 漏洞 可绕过 ASLR](https://github.com/DepthFirstDisclosures/Nginx-Rift) ⭐️ 8.0/10

一个名为 Nginx-Rift 的 nginx 内存损坏漏洞已被公开，该漏洞利用 rewrite 和 set 指令，并声称可绕过 ASLR。 由于 nginx 承载着大量网络服务，该漏洞构成了重大安全风险，但使用命名捕获组等缓解措施降低了其严重性。 该漏洞需要特定前提条件：rewrite 指令中替换字符串包含问号，并且随后的 set 指令引用正则表达式捕获组（例如 set $var $1）。概念验证假设 ASLR 已禁用，但漏洞描述声称存在可靠的 ASLR 绕过方法。

hackernews · hetsaraiya · May 14, 17:17 · [社区讨论](https://news.ycombinator.com/item?id=48138268)

**背景**: Nginx 是一款流行的网络服务器，使用 rewrite 和 set 等指令进行 URL 操作。Rewrite 规则可包含正则表达式捕获组（例如 $1、$2）来捕获 URL 的特定部分。命名捕获组（例如 $name）是一种替代方案，不受此漏洞影响。ASLR（地址空间布局随机化）是一种内存保护技术，通过随机化内存地址来增加漏洞利用难度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.digitalocean.com/community/tutorials/nginx-rewrite-url-rules">Nginx Rewrite URL Rules Examples | DigitalOcean</a></li>
<li><a href="https://nickjanetakis.com/blog/using-nginx-regex-capture-groups-to-redirect-url-paths">Using NGINX Regex Capture Groups to Redirect... — Nick Janetakis</a></li>

</ul>
</details>

**社区讨论**: 社区讨论指出，ASLR 是一种深度防御机制，因概念验证禁用了 ASLR 而轻视该漏洞是错误的。评论者强调漏洞真实存在且前提条件苛刻，但 F5 已发布了针对 1.31.0 和 1.30.1 版本的补丁。

**标签**: `#nginx`, `#exploit`, `#security`, `#vulnerability`, `#ASLR`

---

<a id="item-6"></a>
## [arXiv 因 AI 幻觉引用封禁作者一年](https://twitter.com/tdietterich/status/2055000956144935055) ⭐️ 8.0/10

arXiv 宣布了一项新政策，对提交包含幻觉引用（很可能是 AI 生成）的论文的作者处以一年封禁，该政策适用于未来的投稿。 这项政策直接应对 AI 生成垃圾内容污染科学文献日益严重的问题，有助于维护学术诚信和对预印本的信任。 封禁期为一年，之后作者必须先有论文被权威同行评审场所接受，才能再次向 arXiv 投稿。该政策针对的是易于检测的幻觉引用，而非诚实错误。

hackernews · gjuggler · May 14, 20:39 · [社区讨论](https://news.ycombinator.com/item?id=48140922)

**背景**: 幻觉引用是指看起来真实但实际上并不存在的虚构引用，通常由 ChatGPT 等 AI 语言模型生成。Nature 的一项分析发现，2025 年的数万篇论文可能包含此类无效引用。arXiv 作为一个免费的预印本库，旨在通过惩罚性措施遏制这一趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)">Hallucination (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.nature.com/articles/d41586-026-00969-z">Hallucinated citations are polluting the scientific literature. What can be done?</a></li>

</ul>
</details>

**社区讨论**: 社区普遍支持该政策，评论如“对科学来说非常好”和“对易于检测的幻觉引用施加后果只能是好事”。但也有一些评论者呼吁在实施封禁前进行仔细审查，并指出该政策可能尚未生效。

**标签**: `#arXiv`, `#academic integrity`, `#AI hallucination`, `#scientific publishing`

---

<a id="item-7"></a>
## [硬盘固件黑客技术深度解析](https://icode4.coffee/?p=1465) ⭐️ 8.0/10

一篇详细的技术文章系列解释了如何导出、逆向工程和修改硬盘固件，包括使用 JTAG 进行实时调试以及利用 AI 分析未知架构。 这项工作揭示了硬盘和固态硬盘中严重的固件级漏洞，凸显了安全研究人员的风险以及潜在威胁行为者的利用可能。同时为数据恢复和取证分析提供了宝贵的技术手段。 该系列涵盖通过 JTAG 进行实时调试、修改固件以及使用 AI 对未知微控制器架构进行分类。第一部分侧重于无需 AI 的固件导出和修改，后续部分则引入 AI 辅助。

hackernews · jsploit · May 14, 16:19 · [社区讨论](https://news.ycombinator.com/item?id=48137553)

**背景**: 硬盘固件是控制驱动器物理操作的低级软件。破解此类固件可让攻击者隐藏恶意代码或改变驱动器行为。历史上，研究人员曾演示过针对硬盘和固态硬盘的固件级攻击，并使用 JTAG 调试等技术提取固件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://icode4.coffee/?p=1465">HDD Firmware Hacking Part 1 – I Code 4 Coffee</a></li>
<li><a href="https://malwaretech.com/2015/04/hard-disk-firmware-hacking-part-1.html">Hard Disk Firmware Hacking (Part 1)</a></li>
<li><a href="https://spritesmods.com/?art=hddhack&page=6">Sprites mods - Hard disk hacking - Software flashing</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了相关工作，包括三星 840 EVO 固态硬盘固件的反编译以及一个修改了/etc/shadow 密码的类似硬盘破解。有人提到了 NSA 的固件黑客能力，凸显了此类研究的现实意义。

**标签**: `#firmware hacking`, `#HDD`, `#reverse engineering`, `#security`, `#hardware hacking`

---

<a id="item-8"></a>
## [Amazonbot 终于遵守 robots.txt](https://xeiaso.net/notes/2026/amazonbot-respecting-robots-txt/) ⭐️ 7.0/10

亚马逊的网页爬虫 Amazonbot 终于开始遵循 robots.txt 的指示，此前它经常忽略这些规则，导致用户遭受大量不必要的流量。 这一变化意义重大，因为许多网站运营者之前不得不手动阻止 Amazonbot，消耗了大量带宽和资源。它为 AI 爬虫遵守道德抓取规范树立了先例。 这一变化是在用户抱怨 Amazonbot 带来高流量（包括访问禁止路径）之后被发现的。亚马逊似乎在没有公开声明的情况下更新了爬虫行为。

hackernews · xena · May 14, 20:22 · [社区讨论](https://news.ycombinator.com/item?id=48140730)

**背景**: Robots.txt 是一个标准文件，用于告知网页爬虫网站的哪些部分可以访问。虽然是自愿遵守，但许多信誉良好的爬虫都会遵循。Amazonbot 是亚马逊的爬虫，用于索引搜索结果并为 Alexa AI 助手提供支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datadome.co/bots/amazonbot/">What is Amazonbot ? How to block it ?</a></li>

</ul>
</details>

**社区讨论**: 评论显示，用户曾因 Amazonbot 遭遇大量数据消耗，例如某个用户的公共仓库流量达到了 750 GiB。部分用户仍持怀疑态度，指出 robots.txt 仅仅是一种君子协议，其他 AWS 用户代理仍在制造问题。

**标签**: `#robots.txt`, `#web scraping`, `#Amazonbot`, `#AI crawlers`, `#Hacker News`

---

<a id="item-9"></a>
## [AI 编程代理降低技术锁定风险](https://simonwillison.net/2026/May/14/not-so-locked-in/#atom-everything) ⭐️ 7.0/10

Simon Willison 反思了 AI 编程代理如何降低软件重写的成本，从而减轻平台和语言锁定的担忧。他提到一家公司使用编程代理将其 iPhone 和 Android 应用重写为 React Native，并确信必要时可以移植回原生，同时引用 Bun 从 Zig 迁移到 Rust 的例子。 这一进展意义重大，因为它降低了选择特定技术栈的战略风险，让组织拥有更多灵活性，并能适应未来变化。通过降低转换成本，这可能加速新语言和框架的采用。 React Native 的重写由 AI 编程代理驱动，该公司明确表示必要时可以撤销该决定。Mitchell Hashimoto 关于 Bun 从 Zig 迁移到 Rust 的引述强调了更广泛的趋势：编程语言不再是不可逆的锁定。

rss · Simon Willison · May 14, 22:53

**背景**: AI 编程代理是使用大型语言模型来帮助编写、重构和重写代码的工具，通常能自动化复杂任务。技术锁定是指一旦平台或语言在项目中深度嵌入后，切换的难度和成本。React Native 是一个用于构建跨平台移动应用的框架，而 Bun 是一个 JavaScript 运行时，最初使用 Zig，现在正被移植到 Rust。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/jtorchia/bun-migrates-from-zig-to-rust-what-my-real-benchmarks-say-about-whether-it-matters-3fm7">Bun Migrates from Zig to Rust : What My Real... - DEV Community</a></li>
<li><a href="https://www.theregister.com/2026/05/05/bun_rust_port/">Anthrophic's Bun team trials port from Zig to Rust • The Register</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#React Native`, `#software engineering`, `#lock-in`, `#programming languages`

---

<a id="item-10"></a>
## [批评‘11 个 AI 智能体’的说法毫无意义](https://simonwillison.net/2026/May/13/boris-mann/#atom-everything) ⭐️ 7.0/10

知名技术人士 Boris Mann 批评‘11 个 AI 智能体’这一说法毫无意义，并将其比作毫无上下文地数电子表格或浏览器标签页。 这一批评突显了‘AI 智能体’一词在行业炒作中常被模糊使用，可能会混淆关于 AI 能力和部署的讨论。 Mann 在 Bluesky 上的帖子因其简洁的比喻而受到关注，并被 Simon Willison 分享到他的博客，加入了关于定义 AI 智能体的持续讨论。

rss · Simon Willison · May 13, 16:15

**背景**: 近年来，‘AI 智能体’一词变得流行，常被用来描述能够执行任务的自主软件。然而，它的含义可能差异很大，从简单的聊天机器人到复杂的多步推理系统。没有明确的定义，像‘11 个 AI 智能体’这样的说法反而模糊不清。

**标签**: `#ai-agents`, `#ai`, `#terminology`, `#criticism`

---

<a id="item-11"></a>
## [美国法官审查 Anthropic 15 亿美元版权和解协议](https://www.investing.com/news/stock-market-news/us-judge-considers-anthropics-15-billion-settlement-of-authors-lawsuit-4690939) ⭐️ 7.0/10

美国法官正在审查 Anthropic 提出的 15 亿美元和解协议，以解决作者指控其 AI 模型使用版权材料进行训练的诉讼。 这一和解为 AI 公司使用受版权保护的作品进行训练树立了重要先例，可能影响未来的诉讼和版权许可实践。 和解金额至少为 15 亿美元，用于补偿其版权作品被未经授权用于训练 Claude AI 模型的创作者。

rss · Investing.com All News · May 14, 23:49

**背景**: 生成式 AI 模型如 Claude 需要大量文本数据用于训练，通常包括受版权保护的书籍。作者起诉侵犯版权，认为未经同意使用其作品违反法律。此案是此类争议中首批重大和解之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wvtf.org/2025-09-05/anthropic-settles-with-authors-in-first-of-its-kind-ai-copyright-infringement-lawsuit">Anthropic settles with authors in first-of-its-kind AI copyright ... | WVTF</a></li>
<li><a href="https://biz.chosun.com/en/en-it/2025/09/07/C3PX7HJJKJFXLLUAGJNLB5KWI4/">Anthropic settles AI copyright lawsuit , agrees to pay... - CHOSUNBIZ</a></li>

</ul>
</details>

**标签**: `#AI`, `#litigation`, `#copyright`, `#Anthropic`, `#settlement`

---

<a id="item-12"></a>
## [Codex 现已集成到 ChatGPT 移动应用](https://openai.com/index/work-with-codex-from-anywhere/) ⭐️ 6.0/10

OpenAI 已将其 AI 编程助手 Codex 集成到 ChatGPT 移动应用中，所有登录 ChatGPT 账户的用户均可免费使用。 这扩展了 AI 辅助编程对移动设备的覆盖，使开发者可以随时随地处理代码，但移动设备的可用性限制可能影响其处理复杂任务的效能。 移动应用中的 Codex 包含远程控制功能，可连接桌面版 Codex 应用，但不包含 Codex Cloud 或 CLI 版本。免费版中的所有交互数据可能被用于训练。

hackernews · mikeevans · May 14, 20:06 · [社区讨论](https://news.ycombinator.com/item?id=48140529)

**背景**: Codex 是 OpenAI 面向开发者的 AI 助手，能够理解、生成和修改十多种编程语言代码。它运行在先进的 GPT 模型上，允许用户用自然语言描述软件需求，由 AI 编写代码并推送到 GitHub。此前，Codex 仅通过桌面端或 CLI 使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/getting-started-openai-codex-tpms-diving-deep-guide-vibe-doron-katz-a5fdc">Getting Started with OpenAI Codex : A TPM’s Diving Deep Guide to...</a></li>
<li><a href="https://techglimmer.io/openai-codex-review-2026/">OpenAI Codex 2026: The New macOS App Turns AI into Your Coding ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户对免费使用 Codex 感到兴奋，而另一些用户则认为由于屏幕尺寸和缺少键盘，移动端使用效果不佳。多位用户指出缺少 Linux CLI 支持以及移动版本未集成 Codex Cloud 等限制。

**标签**: `#Codex`, `#ChatGPT`, `#mobile`, `#AI coding`, `#OpenAI`

---

<a id="item-13"></a>
## [Mitchell Hashimoto：编程语言如今可替代](https://simonwillison.net/2026/May/14/mitchell-hashimoto/#atom-everything) ⭐️ 6.0/10

HashiCorp 联合创始人 Mitchell Hashimoto 在 Twitter 上表示，编程语言正变得越来越可替代，他以 Bun 从 Zig 快速重写为 Rust 为例，说明语言不再是绑定因素。 这一观察挑战了传统观念——选择一种编程语言会导致长期绑定，暗示借助现代工具和 AI 辅助，语言迁移可以快速完成。这影响了开发者和公司评估新项目语言决策的方式。 Bun 是一个最初用 Zig 编写的 JavaScript 运行时，其新所有者 Anthropic 实验性地用 Rust 重写了它。Hashimoto 声称重写大约花了一两周，突显了语言的可替代性。

rss · Simon Willison · May 14, 22:31

**背景**: Bun 是一个高性能 JavaScript 运行时和工具包，旨在作为 Node.js 的直接替代品，使用 JavaScriptCore 引擎。Zig 是一种专注于简洁性和性能的系统编程语言，常与 C 比较。Rust 是一种内存安全的系统语言，在性能关键型应用中越来越受欢迎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig ( programming language ) - Wikipedia</a></li>
<li><a href="https://www.stork.ai/blog/buns-rust-rewrite-the-betrayal-that-killed-zig">Bun 's Rust Rewrite : An Analysis of the Zig vs. Rust Debate | Stork.AI</a></li>

</ul>
</details>

**标签**: `#programming-languages`, `#rust`, `#zig`, `#bun`, `#mitchell-hashimoto`

---

<a id="item-14"></a>
## [Datasette IP 速率限制插件 0.1a0 发布](https://simonwillison.net/2026/May/14/datasette-ip-rate-limit/#atom-everything) ⭐️ 6.0/10

Simon Willison 发布了 datasette-ip-rate-limit 0.1a0 版本，这是一个用于 Datasette 的插件，通过限制 IP 地址的请求速率来阻止激进的爬虫。该插件借助了 OpenAI 的 Codex AI 代理进行开发。 该插件解决了 Datasette 用户常遇到的恶意爬虫问题，无需复杂基础设施即可保护网站性能。同时也展示了 AI 辅助开发在实际软件工具中的应用。 该插件支持按路径配置速率限制规则，最多跟踪 10,000 个 IP 地址，并可对静态文件等路径豁免。在生产配置中，它对某些演示数据库路径限制为每 60 秒 60 次请求，违规 IP 将被封禁 20 秒。

rss · Simon Willison · May 14, 04:10

**背景**: Datasette 是一个开源的 Python 工具，用于探索和发布结构化数据，常用于在线共享数据集。速率限制是一种控制客户端在给定时间内请求数量的技术，可防止服务器过载。Codex 是 OpenAI 开发的 AI 编码代理，旨在自动化编写功能、修复 Bug 等软件工程任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex ( AI agent) - Wikipedia</a></li>
<li><a href="https://faceprep.medium.com/what-is-codex-openais-latest-ai-coding-agent-3e487915d486">What is Codex ? OpenAI’s latest AI coding agent | by FACE... | Medium</a></li>

</ul>
</details>

**标签**: `#datasette`, `#rate-limiting`, `#python`, `#ai-assisted`

---

<a id="item-15"></a>
## [Simon Willison 的 CSP 允许列表实验](https://simonwillison.net/2026/May/13/csp-allow/#atom-everything) ⭐️ 6.0/10

Simon Willison 构建了一个工具，将应用加载在受 CSP 保护的沙箱 iframe 中，并拦截 fetch 错误，提示用户将被阻止的域名加入允许列表，然后刷新页面。 该实验展示了一种新颖且用户友好的方法来管理内容安全策略（CSP）限制，而不会破坏功能，可能通过减少摩擦来提高 Web 安全性的采用率。 该工具使用自定义的 fetch() 拦截 CSP 错误并将其传递给父窗口，父窗口随后显示一个对话框，询问是否将源添加到 connect-src 允许列表。该实现是在 Codex 桌面应用中使用 GPT-5.5 xhigh 构建的。

rss · Simon Willison · May 13, 04:50

**背景**: 内容安全策略（CSP）是一种安全标准，限制网页可以加载哪些资源，以防止跨站脚本攻击。沙箱 iframe 功能有限，可用于隔离不受信任的内容。CSP 违规通常会导致请求被阻止，从而可能破坏功能；该实验提供了一种基于用户同意动态更新策略的方法。

**标签**: `#CSP`, `#web security`, `#sandbox`, `#iframe`, `#JavaScript`

---