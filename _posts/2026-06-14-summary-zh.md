---
layout: default
title: "Horizon Summary: 2026-06-14 (ZH)"
date: 2026-06-14
lang: zh
---

> From 49 items, 13 important content pieces were selected

---

1. [vLLM v0.23.0 强化 DeepSeek-V4 并扩展 Model Runner V2](#item-1) ⭐️ 9.0/10
2. [人口普查局禁止在统计产品中使用噪声注入](#item-2) ⭐️ 9.0/10
3. [警官因使用 AI‘制造证据’被调查](#item-3) ⭐️ 9.0/10
4. [美国政府下令暂停 Anthropic 的 Fable 5 和 Mythos 5 访问](#item-4) ⭐️ 9.0/10
5. [智谱 AI 发布完全开放的 GLM-5.2 前沿模型](#item-5) ⭐️ 8.0/10
6. [胰腺肿瘤治疗或揭示癌症总开关](#item-6) ⭐️ 8.0/10
7. [谷歌提议用退役手机构建低碳计算平台](#item-7) ⭐️ 8.0/10
8. [阿拉伯文字渲染：技术债务与用户困境](#item-8) ⭐️ 8.0/10
9. [Pyodide 314.0 允许将 WASM 轮子发布到 PyPI](#item-9) ⭐️ 8.0/10
10. [博客文章要求每帧 UI 动画完美](#item-10) ⭐️ 7.0/10
11. [RTX 5080 加 RTX 3090 组合在 Qwen 3.6 27B Q8 上达到 80 Tok/s](#item-11) ⭐️ 7.0/10
12. [OpenAI WebRTC 音频会话新增文档上下文与 GPT-Realtime-2 支持](#item-12) ⭐️ 6.0/10
13. [AI 可能扰乱一半初级白领工作](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [vLLM v0.23.0 强化 DeepSeek-V4 并扩展 Model Runner V2](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 9.0/10

vLLM v0.23.0 发布，包含来自 200 位贡献者的 408 次提交，大幅完善了 DeepSeek-V4 在多后端上的支持，并使 Model Runner V2 成为 Llama 和 Mistral 稠密模型的默认执行路径。 此版本为广泛使用的 DeepSeek-V4 MoE 模型带来了关键优化，并将性能提升扩展到 Llama、Mistral 等主流稠密模型，直接惠及生产环境中使用 vLLM 的数千用户。 关键技术亮点包括：为 DeepSeek-V4 解耦稀疏 MLA 元数据、新增 TRTLLM 生成注意力内核、支持 Mega-MoE 的专家并行负载均衡 (EPLB)、选择性前缀缓存保留，以及 Model Runner V2 新增 FlashInfer 采样器和可中断 CUDA 图。

github · khluu · Jun 12, 23:29

**背景**: vLLM 是一个高吞吐、内存高效的大语言模型推理引擎。DeepSeek-V4 采用混合专家 (MoE) 架构，并使用多潜在注意力 (MLA) 来减少 KV 缓存内存消耗。Model Runner V2 是一条新的执行路径，可消除流水线并行气泡，并支持可中断 CUDA 图等高级特性，从而提高 GPU 利用率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/deepseek_v4/sparse_mla/">sparse_mla - vLLM</a></li>
<li><a href="https://deepwiki.com/NVIDIA/TensorRT-LLM/9.2-trtllm-attention-backend">TRTLLM Attention Backend | NVIDIA/TensorRT-LLM | DeepWiki</a></li>
<li><a href="https://github.com/vllm-project/vllm/issues/20468">[Feature]: Support EPLB for More MoE Models, e.g. Qwen 3, Llama 4 · Issue #20468 · vllm-project/vllm</a></li>

</ul>
</details>

**标签**: `#vllm`, `#llm-inference`, `#deepseek`, `#optimization`, `#release`

---

<a id="item-2"></a>
## [人口普查局禁止在统计产品中使用噪声注入](https://desfontain.es/blog/banning-noise.html) ⭐️ 9.0/10

美国商务部发布命令，禁止人口普查局和经济分析局在其所有统计产品中使用噪声注入（一种差分隐私技术）。 这项政策移除了官方统计中保护个人数据的关键隐私机制，增加了重识别风险，并影响公众对政府数据的信任。 噪声注入通过向统计输出中添加校准的随机噪声来实现差分隐私；该命令明确禁止了这种方法，而人口普查局近期产品中曾使用该方法。

hackernews · nl · Jun 13, 13:54 · [社区讨论](https://news.ycombinator.com/item?id=48517377)

**背景**: 差分隐私是一种数学框架，通过限制从发布的统计中可推断的信息来确保个人隐私。人口普查局曾在 2020 年人口普查等产品中采用噪声注入，但批评者认为它降低了数据效用。此次禁令代表了从正式隐私保障向更重视准确性的转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://desfontain.es/blog/banning-noise.html">Banning noise will be a disaster for statistical data ...</a></li>
<li><a href="https://www.bea.gov/help/faq/1490">Why didn’t BEA use noise infusion as its statistical ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Differential_privacy">Differential privacy</a></li>

</ul>
</details>

**社区讨论**: 评论反映了深刻分歧：普查员表达了对信任丧失和数据滥用风险增加的担忧，而另一些人则认为差分隐私对保护个体至关重要。一些人提到基层政治压力反对差分隐私，并引用了州级反对的例子。

**标签**: `#differential privacy`, `#census`, `#data privacy`, `#government statistics`, `#policy`

---

<a id="item-3"></a>
## [警官因使用 AI‘制造证据’被调查](https://news.sky.com/story/derbyshire-police-officer-investigated-for-using-ai-to-create-evidence-in-multiple-cases-13553661) ⭐️ 9.0/10

一名德比郡警官因涉嫌在多个案件中使用人工智能制造或伪造证据材料而接受调查。 此案突显了执法领域中 AI 滥用的新兴风险，可能破坏证据的完整性和公众对司法系统的信任。 AI 生成证据的具体性质尚未披露，但可能涉及图像增强、深度伪造或伪造证人陈述。

hackernews · austinallegro · Jun 13, 19:54 · [社区讨论](https://news.ycombinator.com/item?id=48520807)

**背景**: 深度伪造是由 AI 生成的合成媒体，可以描绘逼真但虚构的事件。法院仍在制定验证 AI 生成证据的标准，引发了对可靠性和正当程序的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.thomsonreuters.com/en-us/posts/ai-in-courts/deepfakes-evidence-authentication/">Deepfakes on trial: How judges are navigating AI evidence authentication - Thomson Reuters Institute</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deepfake">Deepfake - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论对证据篡改表示愤怒，并质疑有多少人可能因伪造或增强的证据而被错误定罪。一些人推测该警官可能使用 AI 来‘增强’模糊图像，但这仍然不可接受。

**标签**: `#AI ethics`, `#legal evidence`, `#police misconduct`, `#technology misuse`

---

<a id="item-4"></a>
## [美国政府下令暂停 Anthropic 的 Fable 5 和 Mythos 5 访问](https://simonwillison.net/2026/Jun/13/us-government-directive-to-suspend-access/#atom-everything) ⭐️ 9.0/10

2026 年 6 月 12 日，美国政府发布出口管制指令，要求 Anthropic 立即暂停向其所有客户（包括外籍员工）提供 Fable 5 和 Mythos 5 AI 模型的访问，理由是国家安全的担忧，涉及报告的越狱漏洞。Anthropic 遵守了指令，模型在数小时内被禁用。 这一事件标志着政府在 AI 安全问题上干预的显著升级，为基于国家安全理由关闭先进 AI 模型树立了先例。它引发了关于监管过度、安全与开放平衡以及 AI 模型部署未来的关键问题。 政府的指令未提供国家安全隐患的具体细节；Anthropic 表示所谓的越狱技术很简单，并且可以在 GPT-5.5 等其他模型上复现。Fable 5 的访问于太平洋时间 6 月 12 日下午 6:59 被切断。

rss · Simon Willison · Jun 13, 01:01

**背景**: 越狱 AI 模型涉及构造对抗性输入以绕过内置安全约束，使模型生成其被训练拒绝的内容。Fable 5 是 Anthropic 最近发布的前沿模型，以其在软件工程和知识工作方面的自主能力而闻名。美国政府拥有对被认为构成国家安全风险的 AI 模型实施出口管制的权力，此前这种权力主要用于限制芯片出口而非模型访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aisecurityandsafety.org/en/guides/jailbreaking-attacks/">Jailbreaking AI Models: Attack Patterns, Examples & Defenses ...</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 评论者对为何这一特定越狱行为引发政府行动表示困惑，有人猜测亚马逊作为政府承包商参与其中。其他人指出 Fable 5 被设计为抵抗利用，而一些人则认为所有 LLM 都可以被越狱，并质疑指令缺乏透明度。

**标签**: `#AI regulation`, `#national security`, `#jailbreaking`, `#Anthropic`, `#export control`

---

<a id="item-5"></a>
## [智谱 AI 发布完全开放的 GLM-5.2 前沿模型](https://twitter.com/jietang/status/2065784751345287314) ⭐️ 8.0/10

智谱 AI（Z.ai）于 2025 年 7 月下旬发布了 GLM-5.2，这是一个完全开放权重的先进 AI 模型，强调无限制地获取前沿 AI 能力。 GLM-5.2 的开放发布与美国近期对 Fable 等模型的限制形成对比，突显了 AI 可及性方面的地缘政治分化。它为全球研究人员和开发者提供了不受限制的许可替代方案。 该模型发布时尚未有官方基准测试博客文章，但社区讨论指出发布时间与美国政府致信 Anthropic 限制 Fable 的时间吻合。GLM-5.2 是开放权重模型，其参数公开可用于微调和部署。

hackernews · aloknnikhil · Jun 13, 16:18 · [社区讨论](https://news.ycombinator.com/item?id=48518684)

**背景**: GLM 是智谱 AI（Z.ai）开发的一系列大型语言模型。之前的版本如 GLM-4.5 采用了混合专家架构。GLM-5.2 的发布延续了智谱 AI 开源模型的传统，这被视为对美国日益严格的 AI 政策的反制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://glm5.net/">GLM-5 | Zhipu AI's Next-Generation Large Language Model</a></li>
<li><a href="https://z.ai/blog/glm-4.5">GLM-4.5: Reasoning, Coding, and Agentic Abililties - z.ai</a></li>

</ul>
</details>

**社区讨论**: 社区成员对开放发布表示赞赏，一些人指出中国实验室发布开放模型而美国审查模型，这听起来像小说。其他人强调了与美国政府对 Fable 行动的精确时间巧合，并对宽松许可表示感谢。

**标签**: `#GLM`, `#AI`, `#Open Source`, `#Geopolitics`, `#Machine Learning`

---

<a id="item-6"></a>
## [胰腺肿瘤治疗或揭示癌症总开关](https://economist.com/science-and-technology/2026/06/12/treating-pancreatic-tumours-may-have-revealed-cancers-master-switch) ⭐️ 8.0/10

一种针对胰腺肿瘤的新治疗方法可能揭示了由 KRAS 突变驱动的癌症的一个关键弱点，该靶点此前被认为无法成药。 这项发现意义重大，因为 KRAS 突变存在于约 25%的肿瘤中，包括胰腺癌、肺癌和结直肠癌等难治性癌症，成功靶向它们可能为数百万患者带来有效疗法。 正如社区讨论中所指出的，这一突破仅适用于约 20%的癌症，而非全部；生物制剂设计的最新进展使得攻克像 KRAS 这样此前无法成药的靶点成为可能。

hackernews · andsoitis · Jun 13, 13:34 · [社区讨论](https://news.ycombinator.com/item?id=48517199)

**背景**: KRAS 是一种基因，其产生的蛋白质参与细胞信号传导和生长。KRAS 突变会导致细胞不受控制地生长，从而引发癌症。几十年来，KRAS 一直被认为是不可成药的，因为其光滑的表面和对 GTP 的高亲和力使得传统药物难以抑制它。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KRAS">KRAS - Wikipedia</a></li>
<li><a href="https://www.mdanderson.org/cancerwise/targeting-the-kras-mutation-for-more-effective-cancer-treatment.h00-159458478.html">Targeting the KRAS mutation for more effective cancer treatment | UT MD Anderson</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11899378/">KRAS Mutations in Cancer: Understanding Signaling Pathways to Immune Regulation and the Potential of Immunotherapy - PMC</a></li>

</ul>
</details>

**社区讨论**: 评论者指出标题有些夸张，澄清该发现仅适用于约 20%的肿瘤，但这仍然是一个重大进展。一位用户强调，靶向 KRAS 此前被认为是不可能的事，这一突破拓宽了未来治疗的前景。

**标签**: `#cancer`, `#pancreatic cancer`, `#KRAS`, `#drug discovery`, `#medical research`

---

<a id="item-7"></a>
## [谷歌提议用退役手机构建低碳计算平台](https://research.google/blog/a-low-carbon-computing-platform-from-your-retired-phones/) ⭐️ 8.0/10

谷歌研究院提出将退役智能手机用作低碳计算平台，用于边缘计算任务，将电子垃圾重新利用为分布式服务器网络。 如果成功，这种方法可以通过延长移动硬件寿命来显著减少电子垃圾和碳足迹，同时为边缘应用提供负担得起的计算资源。 该方案将每部手机视为类似于树莓派的弱服务器，但面临来自锁定引导加载程序、专有固件以及厂商有限的安全更新生命周期等挑战。

hackernews · vikas-sharma · Jun 13, 09:38 · [社区讨论](https://news.ycombinator.com/item?id=48515336)

**背景**: 边缘计算在数据源头附近处理数据而不是在中央数据中心，从而减少延迟和带宽使用。退役手机产生的电子垃圾是一个日益严重的环境问题，因为手机含有宝贵材料，但由于缺乏软件支持而经常被丢弃。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Edge_computing">Edge computing</a></li>

</ul>
</details>

**社区讨论**: 评论者对硬件再利用表示热情，但强调过时软件和锁定设备带来的安全风险。有人呼吁法规要求引导加载程序可解锁，另一些人指出当前 Android 手机比 iPhone 更容易重新利用。

**标签**: `#sustainability`, `#edge computing`, `#e-waste`, `#Android`, `#cloud computing`

---

<a id="item-8"></a>
## [阿拉伯文字渲染：技术债务与用户困境](https://lr0.org/blog/p/arabic/) ⭐️ 8.0/10

一篇详细的博文探讨了文本编辑器中阿拉伯文字渲染的系统性技术债务，揭示了双向文本算法和字体整形中的缺陷，导致日常用户困扰。 这很重要，因为阿拉伯文字被数亿人使用，但糟糕的渲染支持造成了显著的生产力损失和认知负担，凸显了国际化工作中的一个盲点。 该文章描述了 Unicode 双向算法和 OpenType 整形功能（如'init'、'medi'、'fina'和'isol'）实现不足，导致混合英文-阿拉伯文邮件中出现光标异常和文本错乱。

hackernews · bookofjoe · Jun 13, 12:40 · [社区讨论](https://news.ycombinator.com/item?id=48516710)

**背景**: 阿拉伯文字需要上下文整形：字母根据位置（独立、首字母、中字母、尾字母）改变形态。此外，阿拉伯文是从右向左书写，但常与从左向右的文本混合，需要 Unicode 双向算法。OpenType 字体格式为阿拉伯文提供了整形功能，但许多文本编辑器和系统支持不完整，导致多年积压的技术债务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bidirectional_text">Bidirectional text - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/typography/script-development/arabic">Developing OpenType Fonts for Arabic Script - Typography Arabic Script Shaping | harfbuzz/harfrust | DeepWiki Arabic Script Resources - World Wide Web Consortium (W3C) Deficiencies of Handling Arabic Script in OpenType (and Some ... Application Support - Arabic Fonts</a></li>
<li><a href="https://en.wikipedia.org/wiki/Technical_debt">Technical debt - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对阿拉伯用户表示同情，有人分享了一个生动的轶事，工程师们放弃了混合语言的电子邮件。还有人注意到阿拉伯文字的美感，并将其与英文布局的复杂性进行了比较。此外，还提供了学术论文和替代性的非连接字体的链接。

**标签**: `#typography`, `#internationalization`, `#Arabic script`, `#text rendering`, `#technical debt`

---

<a id="item-9"></a>
## [Pyodide 314.0 允许将 WASM 轮子发布到 PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 8.0/10

Pyodide 314.0（于 2026 年 6 月发布）现在允许将编译为 WebAssembly 轮子的 Python 包直接发布到 PyPI，并通过 micropip 在运行时安装，消除了之前需要 Pyodide 维护者集中托管的限制。 这一变化大幅减轻了 Pyodide 维护者的负担，消除了社区的一大瓶颈，使任何包作者都能通过标准的 PyPI 基础设施分发 WASM 编译的 Python 包。 这些轮子使用 PEP 783 中定义的新平台标签 'pyemscripten'，并且 cibuildwheel 支持构建它们。一个典型的例子是 luau-wasm 包，它将 Luau 编译器作为编译为 WebAssembly 的 CPython 扩展模块嵌入。

rss · Simon Willison · Jun 13, 23:55

**背景**: Pyodide 是一个基于 WebAssembly 的 Python 发行版，用于浏览器和 Node.js。此前，超过 300 个包必须由 Pyodide 核心团队手动构建和托管。PEP 783 标准化了 Emscripten 平台标签，使这一新工作流成为可能。WebAssembly 允许编译后的代码在浏览器中以接近原生的速度运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging | peps.python.org</a></li>

</ul>
</details>

**标签**: `#Pyodide`, `#WebAssembly`, `#Python`, `#PyPI`, `#WASM`

---

<a id="item-10"></a>
## [博客文章要求每帧 UI 动画完美](https://tonsky.me/blog/every-frame-perfect/) ⭐️ 7.0/10

一篇题为'Every Frame Perfect'的博客文章由开发者 Nikita Prokopov 撰写，主张 UI 动画的每一帧都必须完美无瑕，并批评了 macOS 中动画出现瑕疵或不完美帧的实例。 该文章挑战了计算机图形学中利用人类视觉感知限制来节省资源的常见做法，引发了开发者和设计师关于动画质量与性能之间平衡的辩论。 作者提供了 macOS 的具体示例，包括保存对话框抖动、Notes 应用按钮跳动以及 Safari 地址栏动画故障，声称即使是单个'错误'帧也会降低用户体验。

hackernews · ravenical · Jun 13, 11:40 · [社区讨论](https://news.ycombinator.com/item?id=48516251)

**背景**: 人类视觉系统仅需 3-6 毫秒的视觉刺激就能感知运动。在动画中，每一帧可以是完美的瞬间（无运动模糊），也可以包含模拟运动模糊使运动看起来更流畅。争论焦点在于 UI 动画是否应优先追求帧完美，还是依靠感知技巧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Motion_blur_(media)">Motion blur (media) - Wikipedia</a></li>
<li><a href="https://www.mdpi.com/2411-5150/3/1/5">Temporal Limits of Visual Motion Processing: Psychophysics ...</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：有人同意示例中的动画确实不佳，但不同意要求每帧都完美的严格前提，认为图形学常利用感知极限。其他人则认为论点薄弱，作者未提供更好的替代方案。

**标签**: `#UI/UX`, `#animation`, `#macOS`, `#software design`, `#human perception`

---

<a id="item-11"></a>
## [RTX 5080 加 RTX 3090 组合在 Qwen 3.6 27B Q8 上达到 80 Tok/s](https://imil.net/blog/posts/2026/rtx-5080-+-rtx-3090-setup-80+-tok-s-on-qwen-3.6-27b-q8/) ⭐️ 7.0/10

一位用户演示了将 RTX 5080 和 RTX 3090 组合在一起的本地推理配置，以 Q8 量化方式运行 Qwen 3.6 27B 模型，达到了每秒 80 个 token 的速度。 该基准测试表明，在相对实惠的消费级 GPU 上可以实现高吞吐量的本地 LLM 推理，有可能减少对云端 AI 服务的依赖。 该配置使用双 GPU 组合并搭配 llama.cpp 或类似软件，80 tokens/s 的性能是针对 27B 参数模型的 Q8 量化版本，在质量和速度之间取得了平衡。

hackernews · iMil · Jun 13, 09:55 · [社区讨论](https://news.ycombinator.com/item?id=48515454)

**背景**: 像 Qwen 3.6 27B 这样的大型语言模型通常需要大量 VRAM；量化会降低模型精度（例如 Q8 使用 8 位权重），从而适配消费级 GPU。RTX 5080（16GB 显存）和 RTX 3090（24GB 显存）合计提供 40GB 显存，足以容纳 27B Q8 模型及其额外开销。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://qwen.ai/blog?id=qwen3.6-27b">Qwen3.6-27B: Flagship-Level Coding in a 27B Dense Model</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-27B">Qwen/Qwen3.6-27B · Hugging Face</a></li>
<li><a href="https://mljourney.com/quantized-llms-explained-q4-vs-q8-vs-fp16/">Quantized LLMs Explained: Q4 vs Q8 vs FP16 - ML Journey</a></li>

</ul>
</details>

**社区讨论**: 用户分享了优化技巧（如温度、top-p、MTP 设置）并比较了性能；一位拥有 4090 和 Tenstorrent 显卡的用户仅获得 30 tps，并指出加利福尼亚州的电费使得云服务更便宜。另一位用户建议使用 25 美元的 Oculink 卡实现多 GPU 配置。

**标签**: `#LLM inference`, `#GPU optimization`, `#local AI`, `#Qwen`, `#token throughput`

---

<a id="item-12"></a>
## [OpenAI WebRTC 音频会话新增文档上下文与 GPT-Realtime-2 支持](https://simonwillison.net/2026/Jun/12/openai-webrtc/#atom-everything) ⭐️ 6.0/10

Simon Willison 更新了他的 OpenAI WebRTC 音频会话工具，新增了文档上下文粘贴功能和对 GPT-Realtime-2 模型的支持，用户现在可以围绕粘贴的文档进行语音对话。 此次更新通过让开发者能够使用先进的推理模型通过语音对话来探索文档，弥补了现有功能的空白，有望提高工作效率，并为偏好音频交互的用户提供便利。 该工具现在包含一个可折叠的“文档上下文”区域，用户可在开始会话前粘贴文本；所选模型为 GPT-Realtime-2，OpenAI 称其为首个具备 GPT-5 级推理能力的语音模型，知识截止日期为 2024 年 9 月 30 日。

rss · Simon Willison · Jun 12, 23:53

**背景**: OpenAI 的 Realtime API 允许使用 WebRTC（一种实时通信标准）构建低延迟的交互式语音应用。GPT-Realtime-2 是 2026 年 5 月推出的语音到语音模型，增强了推理能力和指令遵循能力。Simon Willison 的工具是一个基于浏览器的演示界面，展示了该 API，现在升级后包含文档上下文功能，使其更加实用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.openai.com/docs/guides/realtime-webrtc">Realtime API with WebRTC | OpenAI API</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-realtime-2">GPT-Realtime-2 Model | OpenAI API</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#WebRTC`, `#audio`, `#AI`, `#tool`

---

<a id="item-13"></a>
## [AI 可能扰乱一半初级白领工作](https://www.investing.com/news/economy-news/what-if-ai-really-does-disrupt-50-of-all-entrylevel-whitecollar-jobs-4741043) ⭐️ 6.0/10

一篇新闻文章推测，人工智能可能扰乱多达 50%的初级白领工作，认为日常任务如数据处理和报告生成可能被自动化。 这一预测突显了劳动力市场的重大转变，可能减少应届毕业生的初级岗位机会，并增加对高级技能的需求。 该文章是推测性的，没有提供具体数据或专家访谈；它侧重于重复性的行政和分析任务易受 AI 自动化影响。

rss · Investing.com All News · Jun 13, 19:45

**背景**: 初级白领工作通常涉及数据录入、日程安排和基础分析等日常任务。AI 系统，尤其是大型语言模型和机器人流程自动化，已在以更高准确性执行这些任务方面展现出能力，引发了对金融、客户服务和法律支持等行业岗位流失的担忧。

**标签**: `#AI`, `#job displacement`, `#economics`, `#white-collar jobs`

---