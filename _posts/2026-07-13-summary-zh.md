---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> From 35 items, 9 important content pieces were selected

---

1. [vLLM v0.25.0 发布，Model Runner V2 成为默认](#item-1) ⭐️ 9.0/10
2. [Chromium 148 的 Math.tanh 可识别操作系统](#item-2) ⭐️ 8.0/10
3. [Claude Code 与 OpenCode 令牌开销对比](#item-3) ⭐️ 8.0/10
4. [迁移至 GPT-5.6 带来 2.2 倍速度和 27%成本节省](#item-4) ⭐️ 8.0/10
5. [陶哲轩谈用编程代理做非关键应用](#item-5) ⭐️ 8.0/10
6. [爱尔兰数据中心消耗全国 23%的电力](#item-6) ⭐️ 8.0/10
7. [Meta 将于九月投产 AI 芯片，计算能力翻倍](#item-7) ⭐️ 8.0/10
8. [微型模拟器：8 位系统的引脚级仿真](#item-8) ⭐️ 7.0/10
9. [Anthropic 因算力限制延长 Fable 5 访问](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0 发布，Model Runner V2 成为默认](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 将 Model Runner V2 设为所有稠密模型的默认执行路径，移除了旧版 PagedAttention 实现，并使 Transformers 建模后端的性能与原生 vLLM 持平。该版本还增加了众多新模型、一个流式解析引擎以及推测解码的改进。 这一重大版本代表了 vLLM 的架构性转变，通过淘汰基础性的 PagedAttention 以支持更灵活的 Model Runner 框架，简化了代码库。Transformers 后端的性能持平降低了用户的迁移门槛，而扩展的模型支持和动态推测解码等新功能拓宽了该库在生产级 LLM 服务中的适用范围。 该版本包含来自 232 位贡献者的 558 次提交，新增内容包括流式解析引擎（统一的工具调用/推理解析）、用于异构词表的通用推测解码（TLI），以及对 GLM-5、DeepSeek-V3.2、Hy3 等模型的支持。移除 PagedAttention 是一个标志性变化，因为它是 vLLM 得名的原始核心算法。

github · khluu · Jul 11, 20:06

**背景**: vLLM 是一个用于高性能 LLM 推理和服务部署的开源库，主要由加州大学伯克利分校开发。其最初的创新 PagedAttention 通过分页方式高效管理注意力键值缓存，实现了接近零浪费和高吞吐量。Model Runner V2 是早期执行管道的继任者，提供了更模块化和灵活的架构，能够处理多种模型类型和量化方法。Transformers 后端允许 vLLM 直接利用 Hugging Face Transformers 的模型实现，此前性能落后，但现在已与原生速度持平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2023-06-20-vllm">vLLM: Easy, Fast, and Cheap LLM Serving with PagedAttention</a></li>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm -project/ vllm</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#release`, `#open-source`, `#AI`

---

<a id="item-2"></a>
## [Chromium 148 的 Math.tanh 可识别操作系统](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 8.0/10

从 Chromium 148 开始，Math.tanh 函数的实现反映了底层操作系统的 libm，使得攻击者可以通过一次函数调用识别操作系统。 这一变化对浏览器指纹识别产生了重大影响，因为它提供了一个精确且稳定的操作系统检测向量，且难以伪造，引发了用户的隐私担忧。 该技术利用了 Math.tanh、CSS 三角函数和 Web Audio 压缩器都通过主机 libm 路由的特点，因此舍入差异会暴露操作系统。

hackernews · joahnn_s · Jul 12, 21:12 · [社区讨论](https://news.ycombinator.com/item?id=48884853)

**背景**: 浏览器指纹识别是一种无需 cookie 即可通过收集设备特有属性来识别用户的做法。由于不同操作系统的浮点实现不同，Math.tanh 等数学函数会存在差异。历史上，这种差异很小，但 Chromium 148 的更改使其更加明显且可利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS , and Anti-Bot...</a></li>
<li><a href="https://news.ycombinator.com/item?id=48884853">Since Chronium 148, Math . tanh is now fingerprintable... | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人质疑其新颖性，并指出这或许能识别浏览器版本范围；另有人怀疑作者所在公司从这类披露中获益。也有人主张采用正确舍入的数学函数来缓解此问题。

**标签**: `#fingerprinting`, `#privacy`, `#chromium`, `#math`, `#security`

---

<a id="item-3"></a>
## [Claude Code 与 OpenCode 令牌开销对比](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

一项实证研究表明，Claude Code 在读取提示前发送约 33,000 个令牌，而 OpenCode 仅发送 7,000 个，表明 Claude Code 的缓存和框架设计存在显著的令牌低效问题。 这种令牌开销直接影响使用 AI 编码助手的开发者的成本，尤其是在大规模使用时，并突显了框架效率的重要性。这些发现还引发了关于子代理成本和工具调用滥用等代理工具中更广泛问题的讨论。 该研究记录了编码工具与 Anthropic 端点之间的所有请求，测量了系统提示大小和框架开销。值得注意的局限包括比较聚焦于单一任务类型，作者计划增加更深入的定性分析。

hackernews · systima · Jul 12, 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48883275)

**背景**: AI 编码助手中的令牌开销是指系统提示、工具模式和框架逻辑消耗的额外令牌，超出了用户实际任务所需。高效的框架能最小化这些令牌以降低成本与延迟。子代理可能因编排和上下文重复而大幅增加令牌使用量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ai-boost/awesome-harness-engineering">GitHub - ai-boost/awesome-harness-engineering: Awesome list for AI agent harness engineering: tools, patterns, evals, memory, MCP, permissions, observability, and orchestration. · GitHub</a></li>
<li><a href="https://www.cockroachlabs.com/blog/agentic-ai-costs-at-scale/">The Bill Arrives: How to Manage Agentic AI Costs at Scale</a></li>

</ul>
</details>

**社区讨论**: 社区成员指出子代理是令牌消耗的主要来源，一位用户报告称单个任务启动了 7 个子代理。其他人强调了即使对于像'嘿'这样的简单提示也会出现工具调用滥用，并质疑 Claude Code 更高的令牌使用量是否是出于盈利动机。作者回应承诺增加定性比较。

**标签**: `#AI coding assistants`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#cost analysis`

---

<a id="item-4"></a>
## [迁移至 GPT-5.6 带来 2.2 倍速度和 27%成本节省](https://ploy.ai/blog/migrating-a-production-ai-agent-to-gpt-5-6) ⭐️ 8.0/10

一篇详细报告展示了将生产环境中的 AI 代理迁移至 GPT-5.6 后，速度提升 2.2 倍、成本降低 27%，且质量保持不变。 这展示了升级到新 LLM 的具体可量化收益，鼓励在成本敏感和性能关键的生产系统中采用。 该代理自主构建和编辑营销网站；GPT-5.6 在完成评分、速度和成本方面均优于之前的默认模型（Opus）。

hackernews · brryant · Jul 12, 17:13 · [社区讨论](https://news.ycombinator.com/item?id=48882716)

**背景**: GPT-5.6 Sol 是 OpenAI 的下一代模型，在编码、推理和效率方面取得了最先进的结果。迁移生产 AI 代理通常涉及切换模型端点并重新评估质量，对于简单工作流可能只需一行代码改动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT‑5.6 Sol: a next-generation model - OpenAI</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>

</ul>
</details>

**社区讨论**: 评论既赞扬也质疑了结果：有人指出在简单工作流中也有类似改进，而另一些人批评了写作风格，并建议 Reasonix 或 Fable 等替代方案可能有不同表现。

**标签**: `#AI`, `#GPT-5.6`, `#performance`, `#cost optimization`, `#migration`

---

<a id="item-5"></a>
## [陶哲轩谈用编程代理做非关键应用](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

菲尔兹奖得主陶哲轩发表博文，讨论他如何利用现代 AI 编程代理（如 Claude）快速构建研究论文中的交互式可视化和小型应用，强调其在非关键任务中的实用性。 陶哲轩指出，这些由大语言模型生成的工具只是核心研究的补充，并非关键任务，因此使用 AI 代理进行引导式交互的下行风险是可以接受的。这篇博文展示了平衡的观点，既看到了当前编程代理的能力，也看到了其局限性。

hackernews · subset · Jul 12, 11:09 · [社区讨论](https://news.ycombinator.com/item?id=48880170)

**背景**: 现代编程代理是能够根据自然语言描述生成、调试和重构代码的 AI 系统。像 Cursor、Claude Code 和 Zencoder 等工具允许用户描述所需功能并直接获得可运行的代码。这些代理降低了软件创建的门槛，使没有深厚编程经验的人也能构建定制化应用。陶哲轩的博文 exemplifies 即使是专家程序员也使用这些代理来快速原型化想法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/">Cursor: AI coding agent</a></li>
<li><a href="https://www.warp.dev/">Warp — The Agentic Development Environment</a></li>
<li><a href="https://zencoder.ai/">Zencoder | The AI Coding Agent</a></li>

</ul>
</details>

**社区讨论**: 评论者赞赏陶哲轩的平衡观点，有人指出大语言模型使他们能够实现一直想要但没时间构建的可视化。其他人幽默地将陶使用编程代理比作米其林星级厨师发现微波炉晚餐，并预测由于软件的潜在需求，这些工具将得到广泛应用。

**标签**: `#AI-assisted coding`, `#LLM applications`, `#Terry Tao`, `#software development`

---

<a id="item-6"></a>
## [爱尔兰数据中心消耗全国 23%的电力](https://www.theregister.com/on-prem/2026/07/11/irish-datacenters-now-guzzle-23-of-the-countrys-electricity/5270013) ⭐️ 8.0/10

根据《The Register》的最新报告，爱尔兰的数据中心目前消耗了该国总电力的 23%，突显了科技行业对能源的巨大需求。 这种水平的能耗引发了关于科技投资驱动的经济增长与环境影响之间平衡的严肃质疑，尤其对爱尔兰的可再生能源目标构成挑战。这场辩论突显了全球范围内对数据中心能源使用的更广泛矛盾。 23%的数字相比往年显著增长，爱尔兰因优惠的企业税率和良好的网络连接而成为科技巨头的重要枢纽。然而，这一电力消耗数据并不包括数据中心设备制造和建设过程中的能源使用。

hackernews · Bender · Jul 12, 20:16 · [社区讨论](https://news.ycombinator.com/item?id=48884322)

**背景**: 数据中心是容纳计算机服务器的设施，为云计算、流媒体和在线服务提供动力。爱尔兰温和的气候减少了冷却需求，使其成为有吸引力的选址地，但数据中心的快速扩张给国家电网带来压力，并引发了关于住宅与工业用电优先级的争论。

**社区讨论**: 用户 cadamsdotcom 认为能源使用反映了经济活动和价值创造，而 mrtksn 将其与公共教育资金和住房等其他问题相类比。其他人质疑数据中心是否为基础设施成本支付了足够费用，还有用户将爱尔兰的人均用电量与加州对比，指出居民承担更高电费。

**标签**: `#datacenters`, `#energy consumption`, `#ireland`, `#infrastructure`, `#environment`

---

<a id="item-7"></a>
## [Meta 将于九月投产 AI 芯片，计算能力翻倍](https://www.investing.com/news/stock-market-news/meta-to-put-ai-chip-into-production-in-september-as-it-looks-to-double-computing-capacity-memo-shows-4787372) ⭐️ 8.0/10

根据内部备忘录，Meta 宣布计划于 2025 年 9 月开始生产其自研 AI 芯片 MTIA（Meta 训练与推理加速器），并旨在将计算能力翻倍以支持不断增长的 AI 工作负载。 此举表明 Meta 致力于减少对外部 GPU 供应商（如 NVIDIA）的依赖，并优化面向数十亿用户的 AI 基础设施。计算能力翻倍可能加速 Meta 各平台上先进 AI 模型和功能的开发。 MTIA 芯片是与 Broadcom 合作开发的，专为推理任务设计，在低到中等复杂度的应用中效率略有提升，但在复杂工作负载上仍落后于 GPU。Meta 的第二代芯片 MTIA 2i 已大规模部署，服务于数十亿用户。

rss · Investing.com All News · Jul 12, 19:00

**背景**: Meta 一直在开发自己的 AI 芯片系列 MTIA，以应对其平台巨大的计算需求。第一代 MTIA 是实验性芯片，而 MTIA 2i 现已大规模部署。自研芯片使 Meta 能够针对特定工作负载优化性能，并减少对商用 GPU 的依赖，尽管目前在高复杂度任务上仍落后于 GPU。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://encord.com/blog/meta-ai-chip-mtia-explained/">All You Need to Know About Meta ’s New AI Chip MTIA</a></li>
<li><a href="https://medium.com/mlworks/meta-chips-built-for-billion-people-4a9d48bb6153">Meta Chips — Built For Billion People | by Mayur Jain | Medium</a></li>
<li><a href="https://aisystemcodesign.github.io/papers/MTIA-ISCA25.pdf">Meta 's Second Generation AI Chip : Model- Chip Co-Design and...</a></li>

</ul>
</details>

**标签**: `#Meta`, `#AI chip`, `#computing capacity`, `#hardware`

---

<a id="item-8"></a>
## [微型模拟器：8 位系统的引脚级仿真](https://floooh.github.io/tiny8bit-preview/index.html) ⭐️ 7.0/10

Andre Weissflog 的“微型模拟器”项目提供了一系列基于浏览器的 8 位计算机模拟器，这些模拟器在引脚级别模拟硬件，强调模块化组件行为和实时交互。 这种引脚级方法在复古计算模拟中提供了前所未有的灵活性和保真度，使开发者和爱好者能够以模块化方式理解和实验硬件交互。 这些模拟器通过 WebAssembly 完全在浏览器中运行，支持 KC85、Amstrad CPC 以及多种 8 位游戏机等系统。该项目已存在多年，最新版本提供了更高的准确性和性能。

hackernews · naves · Jul 12, 20:23 · [社区讨论](https://news.ycombinator.com/item?id=48884395)

**背景**: 引脚级仿真模拟芯片每个引脚上的确切电信号，从而实现对硬件行为的精确仿真。传统模拟器通常对此进行抽象，而微型模拟器的方法能够更准确地再现边界情况和组件之间的复杂交互。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://floooh.github.io/tiny8bit/">Tiny Emulators</a></li>
<li><a href="https://blog.adafruit.com/2025/04/28/the-tiny-emulators-allows-8-bit-gameplay-in-browser/">The Tiny Emulators allows 8-bit gameplay in browser</a></li>
<li><a href="https://boingboing.net/2021/11/30/tiny-emus-simple-emulators-of-8-bit-computers-that-launch-in-the-browser.html">Tiny Emus: simple emulators of 8-bit computers that launch in the browser - Boing Boing</a></li>

</ul>
</details>

**社区讨论**: 社区赞扬了引脚级模型的模块化和灵活性，一位评论者指出明确定义的薄接口可能是互操作性中未被充分探索的领域。另一位用户提到某些模拟器的音频音量意外地高。第三位指出该项目已存在至少 8 年。

**标签**: `#emulation`, `#retrocomputing`, `#hardware simulation`, `#open source`

---

<a id="item-9"></a>
## [Anthropic 因算力限制延长 Fable 5 访问](https://simonwillison.net/2026/Jul/12/bump/#atom-everything) ⭐️ 7.0/10

Anthropic 再次延长了其 Claude Fable 5 模型在付费计划中的访问时间至 7 月 19 日，原因是算力限制；与此同时，OpenAI 取消了 GPT-5.6 Sol 的使用限制并宣布了效率改进。 这凸显了不同的策略：Anthropic 在为其先进的 Mythos 级模型提供容量方面面临困境，而 OpenAI 在规模化提供 GPT-5.6 Sol 方面显得更有信心，这可能会影响用户选择倾向 OpenAI。 Fable 5 作为 Mythos 级模型，在付费计划中仍可使用每周用量限额的一半，之后转为信用额度。GPT-5.6 Sol 被描述为 OpenAI“迄今为止最好的编码模型”，最近取消了五小时使用上限并推出了效率提升。

rss · Simon Willison · Jul 12, 21:20

**背景**: Mythos 级模型是 Anthropic 最强但也最危险的 AI 系统，Fable 5 是首个公开可用的 Mythos 级模型。算力限制指的是缺乏足够的基础设施来规模化提供该模型，而不会产生高成本或性能下降。2026 年初，Anthropic 已因类似限制而对 Fable 5 的访问进行了限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/news/redeploying-fable-5">Redeploying Claude Fable 5 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 文章作者认为 Anthropic 应让 Fable 在付费计划中永久可用，因为 OpenAI 正因 Fable 访问的不确定性而赢得用户。未提供其他社区评论。

**标签**: `#AI`, `#language models`, `#Anthropic`, `#OpenAI`, `#compute constraints`

---