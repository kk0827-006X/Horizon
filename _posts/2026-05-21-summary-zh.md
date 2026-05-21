---
layout: default
title: "Horizon Summary: 2026-05-21 (ZH)"
date: 2026-05-21
lang: zh
---

> From 42 items, 13 important content pieces were selected

---

1. [OpenAI 模型推翻离散几何猜想](#item-1) ⭐️ 9.0/10
2. [GitHub 确认恶意 VSCode 扩展导致 3800 个仓库遭入侵](#item-2) ⭐️ 9.0/10
3. [Qwen3.7-Max：专注智能体的新 LLM 称霸 SOTA](#item-3) ⭐️ 9.0/10
4. [SpaceX S-1 文件披露星链盈利及与 Anthropic 的每月 12.5 亿美元 AI 计算协议](#item-4) ⭐️ 9.0/10
5. [谷歌向网络宣战：人工智能威胁共生关系](#item-5) ⭐️ 8.0/10
6. [Mozilla 宣布淘汰 asm.js，WebAssembly 接棒](#item-6) ⭐️ 8.0/10
7. [Railway 的 GCP 账户暂停事件报告揭示可靠性风险](#item-7) ⭐️ 8.0/10
8. [Gemini 3.5 Flash 发布：价格更高，整合更广](#item-8) ⭐️ 8.0/10
9. [金属乐子流派交互式地图](#item-9) ⭐️ 6.0/10
10. [SBCL：终极汇编代码面包板](#item-10) ⭐️ 6.0/10
11. [模拟 LLM 令牌速度：每秒 5 到 800 个](#item-11) ⭐️ 6.0/10
12. [Simon Willison 谈 Google I/O：Gemini Spark 与 Antigravity](#item-12) ⭐️ 6.0/10
13. [五分钟回顾六个月的大语言模型进展](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI 模型推翻离散几何猜想](https://openai.com/index/model-disproves-discrete-geometry-conjecture/) ⭐️ 9.0/10

OpenAI 的模型找到了保罗·埃尔德什在离散几何中一个长期未解猜想的反例，展示了 AI 进行新颖数学推理的能力。 这一成就表明 AI 可以为基础数学做出贡献，发现新知识，挑战了 AI 仅仅重新组合现有数据的观点，并有可能加速数学研究。 这次反驳是通过找到反例而非一般性证明实现的，一些数学家指出，通过反例推翻猜想通常被认为不如证明其为真那样具有洞察力。

hackernews · tedsanders · May 20, 19:05 · [社区讨论](https://news.ycombinator.com/item?id=48212493)

**背景**: 离散几何研究有限几何对象（如点和线）的组合性质。该猜想涉及点线关联，这是离散几何中的一个经典领域。像 LLM 这样的 AI 模型现在被用于系统地探索数学猜想。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Discrete_geometry">Discrete geometry</a></li>

</ul>
</details>

**社区讨论**: 社区讨论褒贬不一：一些人激动于 AI 在数学中的潜力，而另一些人则争论 LLM 是否真正发现还是仅仅重新组合。Tim Gowers 的评论被高度推荐，一些人认为反例方法不如证明本身有影响力。

**标签**: `#AI`, `#mathematics`, `#discrete geometry`, `#LLM`, `#research`

---

<a id="item-2"></a>
## [GitHub 确认恶意 VSCode 扩展导致 3800 个仓库遭入侵](https://www.bleepingcomputer.com/news/security/github-confirms-breach-of-3-800-repos-via-malicious-vscode-extension/) ⭐️ 9.0/10

GitHub 确认超过 3800 个内部仓库因一个恶意 VSCode 扩展而遭到入侵，这是一起同时影响了微软 Python SDK 的供应链攻击。 此次入侵凸显了开发者工具链中的严重安全风险，尤其是 VSCode 扩展——它们往往未经严格审查就被信任。这可能导致大规模代码窃取或更深入的供应链攻击。 该恶意扩展来自 VSCode Marketplace，似乎是一种针对微软 Python SDK 的蠕虫。遭入侵的仓库是 GitHub 内部仓库，但该扩展的安装量高达 15 万。

hackernews · Timofeibu · May 20, 13:43 · [社区讨论](https://news.ycombinator.com/item?id=48207660)

**背景**: VSCode 扩展是提供额外功能的插件，但可以执行任意代码，因此成为供应链攻击的主要载体。VSCode Marketplace 此前就曾遭受恶意扩展的侵害，此次事件凸显了加强审查和安全措施的必要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pIXy1HWEVSRWQya05EVXpvb0hTZ0FQAQ?hl=en-IN&gl=IN&ceid=IN:en">GitHub internal repositories breached via malicious extension ...</a></li>
<li><a href="https://www.stepsecurity.io/blog/malicious-iolitelabs-vscode-extensions-target-solidity-developers-on-windows-macos-and-linux-with-backdoor">Malicious IoliteLabs VSCode Extensions Target Solidity... - StepSecurity</a></li>
<li><a href="https://www.linkedin.com/posts/abhishek-chatrath1_12-malicious-extension-in-vscode-marketplace-activity-7390035070603956225-KHXz">Malicious VSCode extensions discovered, posing data risk | LinkedIn</a></li>

</ul>
</details>

**社区讨论**: 评论者对 VSCode 扩展的攻击载体表示担忧，有人指出弹窗提示安装未经验证扩展的风险。另一位评论者猜测攻击可能涉及被入侵的 nx console 扩展。总体情绪是恐惧，并批评扩展生态系统缺乏安全性。

**标签**: `#security`, `#github`, `#vscode`, `#supply-chain`, `#breach`

---

<a id="item-3"></a>
## [Qwen3.7-Max：专注智能体的新 LLM 称霸 SOTA](https://qwen.ai/blog?id=qwen3.7) ⭐️ 9.0/10

阿里巴巴通义实验室发布了 Qwen3.7-Max，这是一款为 AI 智能体任务优化的专有大型语言模型，声称在非幻觉率等基准测试上达到最先进水平。 此次发布标志着开源生态模型在智能体领域的快速进步，挑战了 GPT-5 和 Gemini 等闭源领导者。强烈的社区参与（594 分，236 条评论）凸显了其对寻求低成本高性能替代方案的开发者和企业的重要性。 Qwen3.7-Max 具备 100 万 token 上下文窗口和显式思维链推理，并通过模型上下文协议（MCP）集成办公生产力工具。它支持多智能体编排和具身智能，但仍是专有模型，开源发布尚未确认。

hackernews · kevinsimper · May 20, 10:35 · [社区讨论](https://news.ycombinator.com/item?id=48205626)

**背景**: AI 智能体是一种结构化为自主推理并完成任务的大型语言模型，通常使用工具。Qwen3.7-Max 基于这一概念构建，利用思维链提升推理能力。该模型由阿里云旗下的通义实验室开发，延续了在开源 AI 领域有影响力的 Qwen 系列，但此版本为专有模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-7-max">Qwen 3 . 7 Max - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://ar5iv.labs.arxiv.org/html/2401.03568">[2401.03568] Agent AI : Surveying the Horizons of Multimodal Interaction</a></li>
<li><a href="https://news.aibase.com/news/28161">Tongyi Lab Launches Qwen 3 . 7 - Max with Orthogonal Decoupling...</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户称赞其 SOTA 非幻觉率，认为它是 Claude Code 的绝佳免费替代品，而另一些用户则对模型为专有而非开源表示失望。还有呼声要求与美国超大规模云服务商合作，以促进更广泛的企业采用。

**标签**: `#AI`, `#large language models`, `#open source`, `#Qwen`, `#agents`

---

<a id="item-4"></a>
## [SpaceX S-1 文件披露星链盈利及与 Anthropic 的每月 12.5 亿美元 AI 计算协议](https://www.sec.gov/Archives/edgar/data/1181412/000162828026036936/spaceexplorationtechnologi.htm) ⭐️ 9.0/10

SpaceX 向 SEC 提交的 S-1 文件显示，星链在 2025 年实现盈利，运营收入达 44 亿美元；同时披露了与 AI 公司 Anthropic 签署的每月 12.5 亿美元云计算服务协议，有效期至 2029 年 5 月。 这份文件表明星链已成为能产生现金流的业务，足以支撑 SpaceX 在 AI 基础设施上的雄心；而与 Anthropic 的巨额协议凸显了 AI 计算能力的强劲需求，可能重塑航天和 AI 产业。 2025 年星链收入 114 亿美元，运营利润 44 亿美元；但 SpaceX 整体净亏损 49 亿美元，资本支出高达 207 亿美元，主要用于星链卫星制造和发射。

hackernews · cachecow · May 20, 20:49 · [社区讨论](https://news.ycombinator.com/item?id=48213933)

**背景**: S-1 文件是公司计划上市时向 SEC 提交的注册声明，包含详细财务信息。星链是 SpaceX 的卫星互联网星座，提供全球宽带服务。Anthropic 是一家以 Claude 模型闻名的 AI 研究公司。该协议涉及 SpaceX 从其 Colossus 数据中心向 Anthropic 提供计算能力。

**社区讨论**: 评论者强调了星链出人意料的盈利能力和 Anthropic 协议的巨大规模，有人对太空数据中心的可行性及 SpaceX 相比其他科技巨头较低收入下的高估值提出质疑。也有人指出尽管运营现金流强劲，但公司资本支出和净亏损巨大。

**标签**: `#SpaceX`, `#IPO`, `#Starlink`, `#Anthropic`, `#AI`

---

<a id="item-5"></a>
## [谷歌向网络宣战：人工智能威胁共生关系](https://tante.cc/2026/05/20/on-google-declaring-war-on-the-web/) ⭐️ 8.0/10

一篇批判性分析认为，谷歌正转向人工智能生成内容，打破了网站提供内容供抓取以换取流量的传统共生关系。 这威胁到网络出版商的商业模式，可能导致一个垄断、低质量的网络环境，只有大企业能从内容中获利。 人工智能生成的摘要常常包含错误，网站所有者报告了流量的重大变化，有些人看到增长，但其他人因错误的 AI 摘要而受损。

hackernews · cdrnsf · May 20, 21:33 · [社区讨论](https://news.ycombinator.com/item?id=48214449)

**背景**: 传统上，谷歌的搜索引擎依赖抓取和索引网络内容，作为回报为网站提供流量。这种共生关系激励了内容创作。谷歌新对人工智能生成答案的关注可能完全绕过网站，消除这种激励。

**社区讨论**: 评论者担心只有大企业才能从创意中获利，而个人被排除在外。一些人担心 AI 摘要常常包含错误，并建议使用 StumbleUpon 等替代方案获取流量。其他人指出共生关系正在被破坏，网站可能会屏蔽谷歌爬虫。

**标签**: `#Google`, `#AI`, `#Web`, `#Monopoly`, `#Content Creation`

---

<a id="item-6"></a>
## [Mozilla 宣布淘汰 asm.js，WebAssembly 接棒](https://spidermonkey.dev/blog/2026/05/20/saying-goodbye-to-asmjs.html) ⭐️ 8.0/10

Mozilla 宣布淘汰 asm.js，这个用于接近原生性能的 JavaScript 子集。WebAssembly 已完全成熟并取代了其在 web 性能优化中的角色。 这标志着 web 技术一个基础时代的结束，asm.js 为在浏览器中运行原生代码开辟了道路。依赖 asm.js 的开发者将全面转向 WebAssembly，后者提供更好的性能和更小的包体积。 asm.js 是 JavaScript 的一个严格子集，通过 Emscripten 作为 C/C++ 的编译目标，实现接近原生的性能。WebAssembly 于 2017 年首次发布，现已成为 W3C 标准，其二进制格式避免了 JavaScript 解析开销，从而取代了 asm.js。

hackernews · eqrion · May 20, 12:01 · [社区讨论](https://news.ycombinator.com/item?id=48206340)

**背景**: asm.js 由 Mozilla 于 2013 年推出，作为对 Google 的 NaCl 和 PNaCl 的回应，旨在为 web 带来接近原生的性能。它通过将 JavaScript 限制为浏览器引擎可以积极优化的子集来工作。然而，asm.js 仍然是 JavaScript，导致包体积较大且存在解析开销。WebAssembly (Wasm) 被设计为真正的二进制格式，于 2019 年成为 W3C 推荐标准，现已获得所有主流浏览器的支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asm.js">Asm.js</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="http://asmjs.org/">asm . js</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了怀旧与认可。用户们回忆起 asm.js 在实现 Figma 等 web 应用中的关键作用，并引用 Gary Bernhardt 的著名演讲《JavaScript 的诞生与消亡》作为预言。一些人感叹这个时代的结束，但承认 WebAssembly 是明显的进步。

**标签**: `#asm.js`, `#WebAssembly`, `#JavaScript`, `#browser`, `#Mozilla`

---

<a id="item-7"></a>
## [Railway 的 GCP 账户暂停事件报告揭示可靠性风险](https://blog.railway.com/p/incident-report-may-19-2026-gcp-account-outage) ⭐️ 8.0/10

Railway 于 2026 年 5 月 19 日发布了一份详细的事件报告，涉及一次因 GCP 账户暂停导致的服务中断，并宣布计划减少对 Google Cloud 服务在数据平面热路径中的依赖。 此事件凸显了 Google Cloud 作为 B2B 提供商在可靠性和信任方面的重大隐患，对依赖 GCP 作为关键基础设施的企业起到了警示作用。Railway 决定重构架构以脱离 GCP 的做法，反映了业界对云供应商锁定风险日益增长的担忧。 服务中断是由于 Google Cloud 在未提前通知的情况下暂停了 Railway 的账户，导致 Railway 整个平台中断了未知时长。Railway 承认在完全依赖 GCP 方面存在架构缺陷，并计划仅将 GCP 用于辅助或故障转移场景。

hackernews · 0xedb · May 20, 08:37 · [社区讨论](https://news.ycombinator.com/item?id=48204770)

**背景**: Railway 是一个一站式智能云平台（PaaS），允许开发者通过连接 GitHub 仓库来部署 Web 应用、数据库等服务。Google Cloud Platform (GCP) 是主要的云提供商，但因不透明的账户暂停操作而受到批评。此次事件是 GCP 客户因自动化或人工账户标记而遭遇突然服务中断的更大模式的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://railway.com/">Railway | The all-in-one intelligent cloud provider</a></li>

</ul>
</details>

**社区讨论**: 社区评论对 GCP 的可靠性提出了强烈批评，用户警告他人注意 Google 的 B2B 可信度问题。一些评论者指出 Google 未能解释根本原因，并提到了过去的事件，同时赞扬 Railway 承担责任并计划减少对 GCP 的依赖。

**标签**: `#Google Cloud`, `#incident report`, `#cloud reliability`, `#B2B trust`, `#Railway`

---

<a id="item-8"></a>
## [Gemini 3.5 Flash 发布：价格更高，整合更广](https://simonwillison.net/2026/May/19/gemini-35-flash/#atom-everything) ⭐️ 8.0/10

Google 在 Google I/O 大会上发布了 Gemini 3.5 Flash，直接进入通用可用性阶段，并已将其集成到 Gemini 应用、Google 搜索、Google Antigravity 和 Gemini Enterprise Agent Platform 等核心产品中。 这标志着 Google AI 战略的重要一步，将能力更强但价格更高的模型部署到免费消费产品中，表明主要 AI 实验室正在测试客户的价格承受能力。 模型 ID 为 gemini-3.5-flash，知识截止日期为 2025 年 1 月，支持 1,048,576 个输入 token 和 65,536 个输出 token。价格为每百万输入 token 1.50 美元，每百万输出 token 9 美元，约为 Gemini 3 Flash Preview 价格的三倍。

rss · Simon Willison · May 19, 22:40

**背景**: Gemini 3.5 Flash 是 Google 最新大型语言模型系列的一部分。新的 Interactions API 处于测试阶段，提供类似 OpenAI Responses 的服务器端历史记录管理。Google 的智能体优先开发平台 Antigravity 和 Gemini Enterprise Agent Platform 旨在构建 AI 智能体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.googleantigravity.org/">AI IDE with Gemini 3 Pro | Agentic Software Development Platform</a></li>
<li><a href="https://cloud.google.com/products/gemini-enterprise-agent-platform">Gemini Enterprise Agent Platform (formerly Vertex AI) | Google Cloud</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#Machine Learning`

---

<a id="item-9"></a>
## [金属乐子流派交互式地图](https://mapofmetal.com/) ⭐️ 6.0/10

金属乐地图——一个展示金属音乐子流派及其演变的交互式可视化项目——已被其创建者从 Flash 移植到 HTML5，从而让这项老项目得以继续服务老粉丝和新访客。 该项目为金属乐爱好者保留了一份独特且具有文化意义的历史资源，并展示了如何将基于 Flash 的遗留创意作品现代化，使其在现代网络上继续可访问。 该网站最初由创建者与一位朋友在大约两周内用 Flash 构建，后来移植到了 HTML5。源代码已在 GitHub 上公开。

hackernews · robin_reala · May 20, 10:47 · [社区讨论](https://news.ycombinator.com/item?id=48205699)

**背景**: 金属乐地图是一个交互式可视化项目，描绘了重金属子流派的演变与关系，从早年的 Led Zeppelin 和 Black Sabbath 等影响者到数十种现代风格。该项目最初用 Adobe Flash 创建，成为金属乐迷钟爱的参考资料。最近移植到 HTML5 确保了它无需已停止浏览器支持的 Flash Player 即可运行。

**社区讨论**: 评论者称赞了该地图的历史准确性和怀旧价值，有人指出它与其他音乐地图（如 Ishkur 的电子音乐指南）有相似之处。用户还表达了对爵士、古典或嘻哈等其他流派类似可视化作品的兴趣，并希望增加显示乐队精神继承者等功能。

**标签**: `#music`, `#visualization`, `#HTML5`, `#interactive`, `#niche`

---

<a id="item-10"></a>
## [SBCL：终极汇编代码面包板](https://pvk.ca/Blog/2014/03/15/sbcl-the-ultimate-assembly-code-breadboard/) ⭐️ 6.0/10

一篇 2014 年的文章展示了如何使用 Steel Bank Common Lisp (SBCL) 作为宏汇编器，在 x86_64 上原型化虚拟机指令，直接将虚拟机寄存器映射到硬件寄存器，并自动处理指令对齐和填充。 该技术展示了高级 Lisp 与低级汇编之间的创造性桥梁，允许快速原型化高效的虚拟机指令集，而无需传统汇编器的繁琐。对于探索代码生成策略的编译器和虚拟机开发者来说，它仍然具有现实意义。 这种方法使用 8 个 x86_64 寄存器作为自定义虚拟机的栈槽，SBCL 的编译器宏自动计算指令对齐。该文章是 2014 年的重新发布，并非新突破，但仍在 Hacker News 上持续引起关注。

hackernews · yacin · May 20, 15:39 · [社区讨论](https://news.ycombinator.com/item?id=48209558)

**背景**: SBCL 是一个高性能、开源的 Common Lisp 实现，带有可将代码编译为高效机器码的原生编译器。Common Lisp 宏允许在编译时进行代码转换，使得 SBCL 适合作为宏汇编器使用。电子学中的“面包板”是原型开发板，这里比喻为灵活的实验环境，用于尝试汇编代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SBCL">SBCL</a></li>
<li><a href="https://archlinux.org/packages/extra/x86_64/sbcl/">Arch Linux - sbcl 2.6.4-1 (x86_64)</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的社区评论显示多年来反复出现的兴趣。用户 snazz 认为文章有挑战性，但赞赏其中的寄存器映射和对齐计算；BoingBoomTschak 推荐了一篇关于 sb-simd 的相关文章。讨论突显了该文章持久的教育价值。

**标签**: `#lisp`, `#sbcl`, `#assembly`, `#compiler`, `#low-level`

---

<a id="item-11"></a>
## [模拟 LLM 令牌速度：每秒 5 到 800 个](https://simonwillison.net/2026/May/20/tokens-per-second/#atom-everything) ⭐️ 6.0/10

Mike Veerman 制作了一个简单的 HTML 应用，能够以每秒 5 到 800 个令牌的速度直观模拟 LLM 输出，帮助用户理解广告中速率在现实中的阅读节奏。 该工具将抽象的每秒令牌数指标变得直观，使开发者和用户能够更好地评估和比较 LLM 性能声明。 该应用模拟每秒 5 到 800 个令牌的速度，其源代码可在 GitHub 上查看或修改。

rss · Simon Willison · May 20, 17:57

**背景**: 在大语言模型（LLM）中，文本被分解为令牌——类似于词语或子词的小单位。每秒令牌数（TPS）是一个常见的性能指标，表示模型生成输出的速度。然而，如果没有对实际阅读速度的感知，原始 TPS 数字很难解读。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baseten.co/blog/comparing-tokens-per-second-across-llms/">Comparing tokens per second across LLMs</a></li>
<li><a href="https://rumn.medium.com/benchmarking-llm-performance-token-per-second-tps-time-to-first-token-ttft-and-gpu-usage-8c50ee8387fa">Benchmarking LLM Performance: Token Per Second (TPS), Time to First Token (TTFT), and GPU Usage</a></li>
<li><a href="https://www.cognativ.com/blogs/post/what-is-a-token-in-llm-a-clear-guide-to-understanding-their-role/314">What is a Token in LLM A Clear Guide to Understanding Their Role</a></li>

</ul>
</details>

**标签**: `#ai`, `#llms`, `#tools`, `#visualization`

---

<a id="item-12"></a>
## [Simon Willison 谈 Google I/O：Gemini Spark 与 Antigravity](https://simonwillison.net/2026/May/20/google-io/#atom-everything) ⭐️ 6.0/10

Simon Willison 讨论了 2026 年 Google I/O 的公告，重点关注 Gemini Spark AI 代理和 Antigravity 平台，并坚持只写关于一般可用产品的政策。 Gemini Spark 标志着 Google 进入个人 AI 代理领域，直接与 OpenClaw 竞争，并在用户将敏感数据委托给代理时引发了关于代理安全和提示注入风险的关键问题。 Gemini Spark 运行在 Gemini 3.5 Flash 和 Antigravity 上，其中 Antigravity 是一个基于 Go 的 CLI 工具和 SDK；开源的 Gemini CLI 将于 6 月 18 日停止使用，由闭源的 Antigravity CLI 取代。

rss · Simon Willison · May 20, 15:32

**背景**: Gemini Spark 是一个全天候个人 AI 代理，可连接 Gmail、日历和 Drive 等 Google 应用。Antigravity 是一个平台，包含桌面应用、CLI 工具、SDK（围绕 Go 二进制文件的 Python 包装器）和 IDE（VS Code 分支）。OpenClaw 是一个开源个人 AI 助手，作为竞争对手，它在本地运行并与 LLM 集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/products/gemini-app/next-evolution-gemini-app/">The Gemini app becomes more agentic, delivering proactive, 24/7 help</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5/">Gemini 3.5: frontier intelligence with action</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>

</ul>
</details>

**标签**: `#google-io`, `#ai-agent`, `#gemini`, `#google`, `#personal-blog`

---

<a id="item-13"></a>
## [五分钟回顾六个月的大语言模型进展](https://simonwillison.net/2026/May/19/5-minute-llms/#atom-everything) ⭐️ 6.0/10

Simon Willison 在 PyCon US 2026 上用带注释的幻灯片总结了 2025 年 11 月至 2026 年 5 月期间大语言模型的关键进展。他强调了“2025 年 11 月转折点”，并指出“最佳”模型在 Anthropic、OpenAI 和 Google 之间易手五次。 这场演讲提供了对快速演变的大语言模型格局的简明快照，帮助开发者和 AI 爱好者快速把握进展速度。Willison 独特的“骑自行车的鹈鹕”测试为比较模型能力提供了创造性的、无偏见的基准。 演讲涵盖了从 2025 年 11 月到 2026 年 5 月的时期，包括 Claude Sonnet 4.5、GPT-5.1、Gemini 3、GPT-5.1 Codex Max 和 Claude Opus 等模型的发布。Willison 使用了他的注释演示工具（完全在浏览器中运行，无需将图像上传到服务器）来创建幻灯片。

rss · Simon Willison · May 19, 01:09

**背景**: Simon Willison 是著名的 Python 开发者及 Datasette 的创建者。他的注释演示工具允许用户在幻灯片图像上添加文本注释，使演讲更易于访问和分享。“骑自行车的鹈鹕”测试是他个人评估大语言模型图像生成质量的基准，选择这个任务是因为它不太可能出现在训练数据中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2023/Aug/6/annotated-presentations/">How I make annotated presentations | Simon Willison ’s Weblog</a></li>

</ul>
</details>

**标签**: `#LLM`, `#PyCon`, `#AI developments`, `#lightning talk`

---