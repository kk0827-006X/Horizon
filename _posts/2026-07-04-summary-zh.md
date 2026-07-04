---
layout: default
title: "Horizon Summary: 2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> From 55 items, 12 important content pieces were selected

---

1. [飞马间谍软件攻击欧盟议会调查人员](#item-1) ⭐️ 8.0/10
2. [SearXNG：一个免费保护隐私的元搜索引擎](#item-2) ⭐️ 7.0/10
3. [本地运行顶尖 LLM 的高价指南](#item-3) ⭐️ 7.0/10
4. [Costco：反亚马逊商业模式](#item-4) ⭐️ 7.0/10
5. [开源 AI 差距地图收录 426 个产品](#item-5) ⭐️ 7.0/10
6. [Josh Comeau 报告 AI 导致课程销量下滑](#item-6) ⭐️ 7.0/10
7. [让 AI 编程助手自行判断以节省 Token](#item-7) ⭐️ 7.0/10
8. [使用 DSPy 评估和改进 Datasette Agent 提示词](#item-8) ⭐️ 7.0/10
9. [理解才能参与：与 AI 协作需要深入理解代码](#item-9) ⭐️ 7.0/10
10. [工厂不过就是房间](#item-10) ⭐️ 6.0/10
11. [Simon Willison 六月通讯：AI 模型与工具更新](#item-11) ⭐️ 6.0/10
12. [Simon Willison 发布 llm-coding-agent 0.1a0 阿尔法版本](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [飞马间谍软件攻击欧盟议会调查人员](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

公民实验室发现，欧洲议会议员斯特利奥斯·库洛格鲁（Stelios Kouloglou）的 iPhone 感染了飞马间谍软件，他本人正是调查间谍软件委员会的成员，感染发生在 2022 年 10 月和 2023 年 3 月。 这次感染表明，一个拥有跨欧洲授权的主权行为者正在积极监视调查间谍软件滥用的委员会本身，这破坏了民主监督，并对欧盟机构构成严重的网络安全威胁。 感染是通过对库洛格鲁的 iPhone 进行取证分析发现的，首次感染与一次针对欧洲俄语和白俄罗斯语流亡记者的飞马间谍软件活动重叠，表明这是一次协调行动。

hackernews · ledoge · Jul 3, 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: 飞马是由以色列公司 NSO Group 开发的间谍软件，能够远程访问移动设备的数据和传感器。它只出售给政府，但被广泛滥用于针对记者、活动家和政治家。公民实验室是多伦多大学的一个研究小组，专门调查数字威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>

</ul>
</details>

**社区讨论**: 评论者对后果表示怀疑，指出过去希腊曾发生飞马间谍软件针对政治人物的丑闻但未得到解决。一些人质疑欧盟议员的工作和个人设备分离问题，而另一些人则强调需要更好的监督。

**标签**: `#cybersecurity`, `#surveillance`, `#Pegasus`, `#espionage`, `#European Parliament`

---

<a id="item-2"></a>
## [SearXNG：一个免费保护隐私的元搜索引擎](https://github.com/searxng/searxng) ⭐️ 7.0/10

SearXNG 是一个免费互联网元搜索引擎，它聚合多个来源的结果，同时尊重用户隐私。 它提供以隐私为中心的搜索引擎替代方案，使用户避免被追踪和画像。其开源特性和活跃的社区支持使其成为注重隐私的用户和构建 AI 代理的开发者的重要工具。 SearXNG 支持 JSON 结果输出，可用于内部文档搜索或 RAG 应用。但可能比直接搜索引擎慢，且偶尔需要解决验证码。

hackernews · theanonymousone · Jul 3, 20:15 · [社区讨论](https://news.ycombinator.com/item?id=48779454)

**背景**: 元搜索引擎将多个底层搜索引擎的结果聚合到一个列表中。SearXNG 是 Searx 的一个分支，而 Searx 本身受 Seeks 项目启发。它允许用户自托管引擎，从而控制自己的搜索数据。该项目在 GitHub 上积极维护，拥有超过 15,000 颗星。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Metasearch_engine">Metasearch engine - Wikipedia</a></li>
<li><a href="https://github.com/searxng/searxng">GitHub - searxng/searxng: SearXNG is a free internet metasearch engine which aggregates results from various search services and databases. Users are neither tracked nor profiled. · GitHub</a></li>
<li><a href="https://docs.searxng.org/user/about.html">About SearXNG - SearXNG Documentation (2026.7.3+21773bbb2)</a></li>

</ul>
</details>

**社区讨论**: 社区评论既提到了好处也指出了权衡。原始创建者指出了元搜索概念的局限性，并转向了一个新的全文索引项目。用户欣赏其隐私保护，但承认速度较慢且可能被某些搜索引擎屏蔽。有评论者指出 SearXNG 是为本地模型提供搜索的关键工具。

**标签**: `#privacy`, `#search engine`, `#open source`, `#metasearch`

---

<a id="item-3"></a>
## [本地运行顶尖 LLM 的高价指南](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob 发布了一份全面指南，介绍如何花费 4 万美元以上搭建本地设施来运行顶尖 LLM（如 GLM-5.2 和 Qwen3.6），并提供了详细的硬件建议和量化技术。 该指南凸显了在本地实现接近云端质量的 LLM 推理所需的巨大成本障碍，引发了关于本地搭建相较于每月 200 美元的 Claude Opus 等订阅服务是否经济可行的讨论。 推荐配置使用四块每块 1.2 万美元的 GPU（如 H200），总花费约 5 万美元，并依赖 NVFP4 等极度量化和 REAP 剪枝技术将模型参数从约 1 万亿降至约 5940 亿。但社区成员指出，即使经过量化，模型质量可能下降或出现推理循环问题。

hackernews · livestyle · Jul 3, 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 本地运行大型语言模型需要大量 GPU 显存——例如，FP16 精度的 700 亿参数模型需要约 140GB 显存。量化通过使用更低精度的数字（如 4 位）来减少内存占用，但可能影响性能。许多爱好者选择更便宜的配置，如两块 RTX 3090（共 48GB 显存）来运行较小模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/deep-learning/recommended-hardware-for-running-llms-locally/">Recommended Hardware for Running LLMs Locally</a></li>
<li><a href="https://epoch.ai/data-insights/llm-inference-price-trends">LLM inference prices have fallen rapidly but unequally across ...</a></li>
<li><a href="https://localllm.in/blog/quantization-explained">The Complete Guide to LLM Quantization | LocalLLM.in</a></li>

</ul>
</details>

**社区讨论**: 评论者对成本持怀疑态度，jacobgold 指出 5 万美元相当于 16.8 年的 Claude Opus 订阅费。Aurornis 警告不要对期望值过高并注意隐藏成本。GTP 建议采用中间方案，使用 128GB 统一内存（如 Apple M 系列）通过 DwarfStar 运行 DeepSeek V4 flash，认为这对许多人来说是更实际的折中方案。

**标签**: `#local-llm`, `#hardware`, `#cost-analysis`, `#guide`, `#llm-inference`

---

<a id="item-4"></a>
## [Costco：反亚马逊商业模式](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

一项分析认为，Costco 的商业模式刻意避开最后一英里配送的复杂性，而是优化大批量到店购物，使其在战略上成为亚马逊的对立面。 这项分析揭示了物流和商业模式设计中的战略权衡，为软件工程师和企业家提供了关于避免不必要复杂性的宝贵智慧。 Costco 采用会员制、有限产品选择和大包装来最小化物流成本，而亚马逊则大力投资最后一英里配送基础设施。

hackernews · bookofjoe · Jul 3, 15:14 · [社区讨论](https://news.ycombinator.com/item?id=48776044)

**背景**: 最后一英里配送是指供应链的最后一段，即货物从配送中心运至客户家门口。由于交通、配送失败和分散性，这一环节以昂贵和复杂著称。Costco 的模式完全规避了这些挑战，依赖顾客自行批量搬运商品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dhl.com/discover/en-global/logistics-advice/import-export-advice/last-mile-solutions">What Is Last Mile Delivery & How Can You Improve It? - DHL</a></li>
<li><a href="https://www.ascm.org/topics/last-mile-delivery/">Understanding Last-Mile Delivery in Supply Chain | ASCM</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同意文章的观点，有人将 Costco 的做法比作工程格言‘智者避问题’。还有人称赞 Costco 是美国伟大的典范。也有评论提到了地区差异，例如英国 Costco 的会员要求。

**标签**: `#business-strategy`, `#logistics`, `#costco`, `#amazon`, `#ecommerce`

---

<a id="item-5"></a>
## [开源 AI 差距地图收录 426 个产品](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 7.0/10

Current AI 发布了开源 AI 差距地图 v0.1，索引了开源 AI 堆栈中的 421 个产品（后更新至 426 个），包括软件工具、模型、数据集和硬件项目。 这份全面的地图有助于识别开源 AI 生态系统中的差距，指导投资与合作，从而加强公共利益 AI，特别是考虑到 Current AI 拥有 4 亿美元的资金支持。 该地图涵盖了来自 228 个组织的 266 个软件工具、85 个模型、50 个数据集和 20 个硬件项目，底层数据以 MIT 许可证在 GitHub 上发布。

rss · Simon Willison · Jul 3, 22:04

**背景**: Current AI 是一个非营利性全球合作伙伴关系，于 2025 年 2 月在巴黎人工智能行动峰会上启动，旨在构建公共利益 AI。差距地图基于哥伦比亚会议、MOF、Hugging Face 等组织的工作，对开源 AI 堆栈进行编目并识别缺失的组件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.currentai.org/">Current AI | Building Public Interest AI Technology Together</a></li>
<li><a href="https://map.currentai.org/">Current AI – Open Source AI Gap Map</a></li>

</ul>
</details>

**标签**: `#open source`, `#artificial intelligence`, `#ecosystem mapping`, `#Current AI`, `#Gap Map`

---

<a id="item-6"></a>
## [Josh Comeau 报告 AI 导致课程销量下滑](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

Josh W. Comeau 报告称，他的新课程《Whimsical Animations》预计销量仅为通常的三分之一，现有课程销售额较去年下降超过 50%，他认为主要原因是 AI。 这凸显了一个日益明显的趋势：AI，特别是大型语言模型（LLM），正通过制造就业不确定性以及提供免费或低成本的个性化辅导，扰乱开发者教育市场，威胁付费课程创作者的业务模式。 知名前端开发者教育者 Josh W. Comeau 推出了第三门课程，销量约为平常的三分之一；他指出，他接触的多位课程创作者都报告了类似的收入下降，降幅达 50%或更多。

rss · Simon Willison · Jul 3, 21:25

**背景**: 大型语言模型（LLM），如 GPT-4，是在海量文本数据上训练的 AI 系统，能够生成、总结和分析文本。它们越来越多地被用于代码生成、调试甚至个性化辅导，这与传统的付费课程形成竞争。许多开发者担心 AI 可能会取代他们的工作，从而降低了投资学习新技能的意愿。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/large-language-models">What Are Large Language Models (LLMs)? | IBM</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/large-language-model-llm/">Large Language Model (LLM) - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: 在讨论中，Josh W. Comeau 感叹 AI 不仅减少了课程销量，还未经同意或补偿就吞噬了创作者的作品。其他课程创作者也表达了类似的经历，表明大家一致认为 AI 正在严重损害他们的收入。

**标签**: `#AI impact`, `#developer education`, `#online courses`, `#job market`

---

<a id="item-7"></a>
## [让 AI 编程助手自行判断以节省 Token](https://simonwillison.net/2026/Jul/3/judgement/#atom-everything) ⭐️ 7.0/10

Simon Willison 分享了来自 Claude Code 团队的建议：让 Fable 自行判断是否进行测试，并将较小的编码任务委托给更便宜的模型（如 Sonnet 或 Haiku），以节省昂贵的 Fable Token。 这种实用方法有助于开发者在使用高端 AI 编程助手（如 Claude Fable）时最大化 Token 效率、降低成本，尤其是在 Token 即将涨价之际。 Willison 创建了一个记忆文件，指示 Claude Code 生成子代理并覆盖模型配置：Sonnet 用于实质性实现，Haiku 用于简单编辑，而需要判断力的任务仍由主模型处理。

rss · Simon Willison · Jul 3, 18:51

**背景**: Claude Fable 是 Anthropic 能力最强的模型，专为复杂的代理式编程优化，但每条 Token 运行成本较高。Claude Code 工具支持模型别名功能，如 Opus 用于规划、Sonnet 用于执行，以平衡成本与能力。随着 AI 编程助手在日常开发中的广泛采用，Token 优化技术变得至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/model-config">Model configuration - Claude Code Docs</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://www.c-sharpcorner.com/article/ai-token-optimization-techniques-every-developer-should-know/">AI Token Optimization Techniques Every Developer Should Know</a></li>

</ul>
</details>

**标签**: `#AI coding assistant`, `#Claude Code`, `#software development`, `#productivity`

---

<a id="item-8"></a>
## [使用 DSPy 评估和改进 Datasette Agent 提示词](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison 使用 DSPy 框架自动评估并改进了 Datasette Agent 的 SQL 系统提示词，他将此任务委托给了 Claude Code 配合 Claude Fable 5 完成。优化发现了模式列表中缺失列名等问题，这些问题曾导致错误的 SQL 查询。 这展示了针对 AI 智能体的一种实用、自动化的提示工程方法，减少了对手动试错的依赖。它突显了 DSPy 如何在数据查询等实际应用中系统地改进智能体行为。 评估使用了 GPT-4.1 mini 和 nano 模型进行测试，并发现模式列表缺少列名，导致列名猜测和错误重试循环。修复方法包括在提示词中加入列名，或软化有关不要调用 describe_table 的建议。

rss · Simon Willison · Jul 2, 18:25

**背景**: DSPy 是斯坦福 NLP 实验室开发的框架，强调通过编程而非提示来使用语言模型，支持模块化和可优化的 AI 系统。Datasette Agent 是 Datasette（一个用于探索和发布 SQLite 数据库的工具）的 AI 助手，能够生成并执行只读 SQL 查询以回答用户问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp / dspy : DSPy : The framework for...</a></li>
<li><a href="https://simonw.substack.com/p/datasette-agent-an-ai-assistant-for">Datasette Agent: an AI assistant for Datasette built on LLM</a></li>

</ul>
</details>

**标签**: `#DSPy`, `#Datasette`, `#prompt engineering`, `#AI agents`, `#SQL`

---

<a id="item-9"></a>
## [理解才能参与：与 AI 协作需要深入理解代码](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 7.0/10

Geoffrey Litt 在 2026 年 AI 工程师世界博览会上提出了'理解才能参与'的概念，认为开发者必须深入理解 AI 代理的代码变更，以保持创造性参与并避免认知债务。 随着 AI 编码代理生成越来越大、越来越复杂的代码变更，如果开发者不跟上理解，就有积累认知债务的风险。这一概念为保持参与度和创造力提供了框架，对维护代码质量和开发者主动权至关重要。 Litt 的方法强调在深入细节之前先建立代码变更的丰富心智模型，并利用 AI 工具高效地赶上理解进度。他认为，如果没有深入理解，开发者在项目中的创造性思考能力将受到限制。

rss · Simon Willison · Jul 2, 17:07

**背景**: 认知债务指的是开发者在依赖 AI 但不完全理解代码时积累的心智负担，类似于技术债务但发生在开发者脑中。随着 AI 代理变得越来越强大，需要更多方法来帮助人类保持参与和理解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck.html">Understanding is the new bottleneck</a></li>
<li><a href="https://twitter.com/geoffreylitt/status/2072522251300409556">Geoffrey Litt on X: "Hot take: I think it's still important to understand the code that our agents write! In this mega thread (based on my AIE talk today), I will explain why that's the case, and show some ideas for how to efficiently understand code. Alright, let's dive in. 1/ https://t.co/765DNZh6LN" / X</a></li>
<li><a href="https://www.linkedin.com/pulse/cognitive-debt-when-ai-becomes-our-google-maps-k-subramanian-vnguc">Cognitive Debt : When AI Becomes Our Google Maps for Software...</a></li>

</ul>
</details>

**标签**: `#AI-assisted coding`, `#cognitive debt`, `#software engineering`, `#developer experience`

---

<a id="item-10"></a>
## [工厂不过就是房间](https://interconnected.org/home/2026/07/03/factories) ⭐️ 6.0/10

一篇随笔提出，工厂本质上不过就是房间，挑战了制造业复杂且资本密集的认知。作者以此观点倡导一种更简单、更易入门的生产观。 这一重新定义鼓励创业者和爱好者重新审视制造业的准入门槛，可能推动更多小规模、本地化的生产。它强调，概念的简单性可以促进制造的民主化。 这篇随笔是反思性的而非技术性的，社区参与度高（73 条评论），分享了许多在小工厂和制造业中的个人经历。讨论深化了核心论点，既展现了机遇也揭示了挑战。

hackernews · arbesman · Jul 3, 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48776035)

**背景**: 人们通常认为工厂是大型自动化设施，需要巨额资本投入。这篇随笔指出，工厂的核心不过是用来制造物品的房间，强调关键要素是人力和流程，而非昂贵的机器。这一观点与 DIY 文化和小批量制造运动相契合。

**社区讨论**: 评论者分享了经营小工厂的个人经历、动手工作的价值，并将快餐厨房比作高效工厂。大家对制造业的简单性表示赞赏，但也认识到商业持续性、流程改进等挑战。

**标签**: `#manufacturing`, `#mindset`, `#small business`, `#making things`

---

<a id="item-11"></a>
## [Simon Willison 六月通讯：AI 模型与工具更新](https://simonwillison.net/2026/Jul/3/june-newsletter/#atom-everything) ⭐️ 6.0/10

Simon Willison 发布了 2026 年 6 月赞助人专属通讯，内容涵盖新 AI 模型（如 Claude Fable 5、GPT-5.6 和 GLM-5.2）、美国出口限制以及 Datasette 及相关工具的更新。 该通讯提供了 AI 和开发者工具最新动态的精选概览，帮助读者了解快速演进的技术。对 Claude Fable 5 和 GLM-5.2 的聚焦反映了专有模型与开放权重模型之间的持续竞争。 Anthropic 于 2026 年 6 月 9 日发布的 Claude Fable 5 被描述为在编码和自主任务上处于领先地位，而 Z.AI 的 GLM-5.2 已成为 Artificial Analysis Intelligence Index 上领先的开放权重模型。Tokenmaxxing（最大化 AI 令牌使用量的趋势）被认为已经过时，转向了 valuemaxxing。

rss · Simon Willison · Jul 3, 14:50

**背景**: Simon Willison 是知名开发者，也是开源数据探索与发布工具 Datasette 的创建者。他的月度通讯仅对赞助人开放，汇总了 AI、LLM 和开发者工具领域的重大新闻。Tokenmaxxing 是指最大化 AI 令牌使用量的做法，通常与 Claude Code 等编码代理相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://artificialanalysis.ai/articles/glm-5-2-is-the-new-leading-open-weights-model-on-the-artificial-analysis-intelligence-index">GLM-5.2 is the new leading open weights model on the Artificial Analysis Intelligence Index</a></li>
<li><a href="https://www.forbes.com/sites/timkeary/2026/06/02/why-tokenmaxxing-is-out-and-valuemaxxing-is-in/">Why ‘Tokenmaxxing’ Is Out And ‘Valuemaxxing’ Is In</a></li>

</ul>
</details>

**标签**: `#newsletter`, `#AI`, `#LLM`, `#datasette`, `#tools`

---

<a id="item-12"></a>
## [Simon Willison 发布 llm-coding-agent 0.1a0 阿尔法版本](https://simonwillison.net/2026/Jul/2/llm-coding-agent/#atom-everything) ⭐️ 6.0/10

Simon Willison 发布了基于其 LLM 库构建的编码代理 llm-coding-agent 的早期阿尔法版本 0.1a0。该代理包含读取和编辑文件、执行命令以及搜索代码等工具，可通过命令行运行或作为 Python API 使用。 此次发布展示了 LLM 库如何演变为代理框架，使得创建类似于 Claude Code 的编码助手成为可能。它展示了开源、可定制的编码代理的潜力，能够根据特定工作流程进行定制。 该代理是使用 Claude Code for web 构建的，先编写规范，然后在 Fable 5 的帮助下通过测试驱动开发实现。它附带 edit_file、execute_command、list_files、read_file 和 search_files 等工具，并支持 `--yolo` 标志来自动批准所有操作。

rss · Simon Willison · Jul 2, 19:33

**背景**: Simon Willison 的 LLM 库是一个用于访问多种大语言模型的 CLI 工具和 Python 库。该库最近经历了重大重构（版本 0.32a0），以更像一个代理框架。这个编码代理是一个实验，旨在探索基于该框架构建的简单编码代理会是什么样子，遵循了类似 Claude Code 的工具的模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#coding agent`, `#Python`, `#Simon Willison`

---