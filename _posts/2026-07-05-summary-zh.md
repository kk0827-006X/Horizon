---
layout: default
title: "Horizon Summary: 2026-07-05 (ZH)"
date: 2026-07-05
lang: zh
---

> From 55 items, 15 important content pieces were selected

---

1. [安娜档案悬赏 20 万美元获取谷歌图书扫描件](#item-1) ⭐️ 9.0/10
2. [提示注入漏洞泄露 YouTube 私密视频](#item-2) ⭐️ 9.0/10
3. [GPT-5.5 Codex 推理令牌聚类导致性能下降](#item-3) ⭐️ 8.0/10
4. [韦伯望远镜发现的小红点令天体物理学家困惑](#item-4) ⭐️ 8.0/10
5. [用 500 字节通过 Deflate 压缩构建世界地图](#item-5) ⭐️ 8.0/10
6. [新版 Claude 模型在工具调用准确性上更差](#item-6) ⭐️ 8.0/10
7. [Claude Code 会话泄漏报告引发调查](#item-7) ⭐️ 7.0/10
8. [Linux 下 htop/top 输出详解指南](#item-8) ⭐️ 7.0/10
9. [Zig 将包管理从编译器移至构建系统](#item-9) ⭐️ 7.0/10
10. [Current AI 发布开源 AI 差距地图](#item-10) ⭐️ 7.0/10
11. [开发者 Josh W. Comeau 报告课程销售额因 AI 下降超 50%](#item-11) ⭐️ 7.0/10
12. [《命令与征服：将军》通过 Fable 移植到苹果设备](#item-12) ⭐️ 6.0/10
13. [Verizon 应用更新导致 Gizmo 智能手表无法使用，强制迁移](#item-13) ⭐️ 6.0/10
14. [让 AI 模型自行判断以提高效率](#item-14) ⭐️ 6.0/10
15. [Simon Willison 2026 年 6 月通讯：AI 模型与 Tokenmaxxing](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [安娜档案悬赏 20 万美元获取谷歌图书扫描件](https://software.annas-archive.gl/AnnaArchivist/annas-archive/-/work_items/234) ⭐️ 9.0/10

安娜档案（Anna's Archive），一个影子图书馆搜索引擎，于 2025 年在 GitLab 问题页面上宣布悬赏 20 万美元，寻求完整的谷歌图书扫描件或同等资料。 这一悬赏代表了将数百万数字化图书从谷歌的专有访问限制中解放出来的重大举措，可能使全球的研究人员、教育工作者和读者（尤其是在图书获取受限的地区）都能普遍获取这些资源。 该悬赏被列为安娜档案自托管 GitLab 实例上的一个工作项，旨在获取来自谷歌图书或类似项目的所有扫描件。具体条款（例如是否接受单个或多个提交）尚未明确。

hackernews · Cider9986 · Jul 4, 16:51 · [社区讨论](https://news.ycombinator.com/item?id=48786838)

**背景**: 安娜档案是一个针对影子图书馆的开源元搜索引擎，于 2022 年在 Z-Library 受到打击后推出。它聚合了来自 Z-Library、Sci-Hub 和 Library Genesis 等来源的元数据，旨在编录所有书籍。谷歌图书在过去二十年中扫描了数百万册图书，但由于版权限制，许多图书仅提供片段或有限预览，因此完整的数据转储对数字保存极具价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48786838">Google Books (or similar) all book scans – $200k bounty (2025) | Hacker News</a></li>
<li><a href="https://software.annas-archive.gl/AnnaArchivist/annas-archive/-/work_items/234">Google Books (or similar) all book scans — $200,000 bounty (#234) · Issues · AnnaArchivist / annas-archive · GitLab</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的社区评论表达了强烈支持，用户分享了通过安娜档案和 Z-Library 获取稀有书籍的个人经历。有人提及 SourceLibrary.org 等相关项目，其他人则讨论了互联网审查和版权的更广泛问题。总体情绪是积极的，但也有一些人对版权侵权提出了伦理担忧。

**标签**: `#digital archiving`, `#book scanning`, `#open access`, `#bounty`, `#information retrieval`

---

<a id="item-2"></a>
## [提示注入漏洞泄露 YouTube 私密视频](https://javoriuski.com/post/youtube) ⭐️ 9.0/10

一名安全研究人员发现，针对 YouTube AI 评论建议功能的提示注入攻击可以泄露私密视频的描述，包括未公开和私密视频的描述。 该漏洞会泄露创作者本应保密的内容，可能将未公开或私密视频的细节暴露给攻击者。它凸显了将大语言模型集成到平台时未进行适当输入清洗所带来的日益严重的安全风险。 攻击原理是攻击者在创作者的视频下留下精心构造的评论；当创作者使用 YouTube Studio 的建议 AI 提示时，恶意内容会触发模型在回复中包含私密视频的描述。研究人员向 Google 报告了该问题，但得到“不予修复”的回应，表明该公司不认为提示注入是漏洞。

hackernews · javxfps · Jul 4, 16:45 · [社区讨论](https://news.ycombinator.com/item?id=48786781)

**背景**: 提示注入是一种网络安全攻击方式，攻击者通过精心构造输入使 AI 模型产生意外行为，常常绕过安全防护。在这个案例中，YouTube 的 AI 用于总结评论并建议回复，但它未能区分合法的系统提示和对抗性用户输入。类似攻击已在其他基于 LLM 的服务上被演示，但本次直接针对内容隐私。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**社区讨论**: 一些用户无法在自己的视频上复现该攻击，对其可靠性提出质疑。一位前 Google 员工解释说，此类漏洞的处理常常落到已经不再负责该项目的工程师身上，从而导致“不予修复”的决定。文章本身因其清晰、非标题党的写作风格而受到高度赞扬。

**标签**: `#security`, `#prompt injection`, `#YouTube`, `#privacy`, `#vulnerability`

---

<a id="item-3"></a>
## [GPT-5.5 Codex 推理令牌聚类导致性能下降](https://github.com/openai/codex/issues/30364) ⭐️ 8.0/10

用户报告称，GPT-5.5 Codex 因推理令牌聚类导致性能下降，模型的推理输出令牌聚集在固定间隔（如 516 个令牌），当模型提前截断时会导致错误答案。 这一性能退化严重影响了依赖 Codex 进行编码任务的开发者，模型的推理质量变得不一致且不可靠，可能迫使用户转向 Claude 等替代方案或使用本地模型。 聚类模式在 516 个推理令牌处最为突出，并在 1034 和 1552 个令牌处出现相关峰值，表明推理推理中存在以 512 个令牌为间隔的批处理优化。当模型在这些边界停止时，通常会产生错误结果。

hackernews · maille · Jul 4, 21:51 · [社区讨论](https://news.ycombinator.com/item?id=48789428)

**背景**: GPT-5.5 Codex 等大型语言模型使用推理令牌逐步解决问题，然后生成最终答案。这些令牌在固定间隔处聚类可能表明模型被强制在任意边界停止，截断了其推理过程。此问题与今年早些时候 Claude Code 中观察到的性能退化类似，类似的令牌批处理导致了输出质量下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/openai/codex/issues/30364">GPT-5.5 Codex reasoning - token clustering at 516/1034/1552 may be...</a></li>
<li><a href="https://news.ycombinator.com/item?id=48789428">GPT-5.5 Codex reasoning - token clustering may be... | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区成员强烈确认了该问题，许多人表示已经经历了数月的性能退化。一位用户使用 Codex CLI 复现了该问题，观察到模型在恰好 516 个推理令牌时短路并返回错误结果，而更长的推理（6000-8000 个令牌）则生成正确答案。其他人推测 OpenAI 正在以 512 令牌为倍数批处理推理推理，作为一种吞吐量优化。

**标签**: `#GPT-5.5`, `#Codex`, `#AI performance`, `#reasoning tokens`, `#regression`

---

<a id="item-4"></a>
## [韦伯望远镜发现的小红点令天体物理学家困惑](https://www.quantamagazine.org/astrophysicists-puzzle-over-webbs-new-universe-20260702/) ⭐️ 8.0/10

詹姆斯·韦伯太空望远镜发现了“小红点”，这些来自早期宇宙的小型红色天体其本质成谜，对现有宇宙学模型构成挑战。 理解小红点可能彻底改变我们对早期宇宙、黑洞形成和星系演化的认识，并可能引发天体物理学的范式转变。 小红点表现为致密的红色天体，其红移对应大爆炸后 6 亿至 16 亿年；最新光谱表明它们是包裹在稠密电离气体茧中的年轻超大质量黑洞。

hackernews · jnord · Jul 4, 09:08 · [社区讨论](https://news.ycombinator.com/item?id=48783948)

**背景**: 詹姆斯·韦伯太空望远镜（JWST）于 2021 年发射，通过红外波段观测宇宙，从而能够看到遥远早期的星系。“小红点”于 2024 年 3 月首次公布，此后成为研究热点。它们极红且极小，意味着高红移和致密结构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Little_red_dot_(astronomical_object)">Little red dot (astronomical object) - Wikipedia</a></li>
<li><a href="https://www.livescience.com/space/black-holes/astronomers-weighed-a-little-red-dot-discovered-by-the-james-webb-telescope-and-found-a-naked-black-hole-inside">Astronomers weighed a 'little red dot' discovered by the James Webb telescope — and found a 'naked' black hole inside | Live Science</a></li>
<li><a href="https://www.nature.com/articles/s41586-025-09900-4">Little red dots as young supermassive black holes in dense ionized cocoons | Nature</a></li>

</ul>
</details>

**社区讨论**: 社区评论观点不一：有人指出褐矮星可能是一种解释（引用 arXiv:2506.04004），其他人则对“黑洞星”等新型天体感到兴奋。尽管存在争论，但总体对这一令人困惑的发现充满热情。

**标签**: `#astrophysics`, `#James Webb`, `#little red dots`, `#black holes`, `#cosmology`

---

<a id="item-5"></a>
## [用 500 字节通过 Deflate 压缩构建世界地图](https://simonwillison.net/2026/Jul/4/building-a-world-map-with-only-500-bytes/#atom-everything) ⭐️ 8.0/10

Iwo Kadziela（在 Codex 协助下）发明了一种方法，利用 deflate 压缩和 JavaScript 的 DecompressionStream，仅用 445 字节数据就渲染出一幅逼真的 ASCII 世界地图。压缩数据通过 data: URI 获取并在浏览器中解压。 这展示了巧妙利用现代 Web API 和压缩技术实现极致数据最小化，激励开发者创造性思考如何减小资源体积。它展示了将 fetch 与 data URI 及流解压缩结合的潜力。 整个实现仅占 500 字节，其中 deflate-raw 压缩数据本身仅 445 字节。代码片段使用 fetch('data:;base64,...')加载压缩数据，通过 new DecompressionStream('deflate-raw')进行管道处理，并将结果渲染为 pre 格式化元素。

rss · Simon Willison · Jul 4, 23:09

**背景**: Deflate 是一种无损压缩算法，结合了 LZ77 和霍夫曼编码，常用于 PNG 和 ZIP 等格式。压缩流 API（包括 DecompressionStream）为浏览器提供了原生解压缩支持。通过将压缩数据编码为 base64 的 data URI，整个地图可以内联而不需要外部资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Deflate">Deflate - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/DecompressionStream">DecompressionStream - Web APIs | MDN</a></li>

</ul>
</details>

**标签**: `#compression`, `#ASCII art`, `#JavaScript`, `#web development`, `#hacks`

---

<a id="item-6"></a>
## [新版 Claude 模型在工具调用准确性上更差](https://simonwillison.net/2026/Jul/4/better-models-worse-tools/#atom-everything) ⭐️ 8.0/10

Armin Ronacher 报告称，较新的 Anthropic Claude 模型（Opus 4.8 和 Sonnet 5）在调用工具时，更频繁地在`edits[]`数组中生成包含虚构额外字段的错误调用，导致第三方编码工具 Pi 拒绝这些调用。 这一最先进模型在工具使用质量上的倒退，削弱了依赖精确工具调用的 LLM 驱动编码代理的可靠性，迫使开发者要么调整工具，要么面临用户体验下降的风险。 错误调用包含工具模式中不存在的虚构键，且该现象仅出现在较新模型中，这表明针对 Claude Code 内置编辑工具的强化学习训练可能无意中损害了其他自定义编辑工具的性能。

rss · Simon Willison · Jul 4, 22:53

**背景**: 工具调用允许 LLM 通过输出与提供模式匹配的结构化 JSON 参数来调用外部函数。当 LLM 输出违反模式的参数（如额外或缺失字段）时，就会发生错误的工具调用。这种倒退尤其令人担忧，因为人们期望更新、更强大的模型在此类任务上改进而非退化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.promptlayer.com/how-to-debug-llm-tool-calls-3/">Debugging LLM Tool Calls: A Practical Guide for AI Teams</a></li>
<li><a href="https://portkey.ai/blog/what-is-llm-tool-calling/">What is LLM tool calling, and how does it work?</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#tool calling`, `#Claude`, `#regression`

---

<a id="item-7"></a>
## [Claude Code 会话泄漏报告引发调查](https://github.com/anthropics/claude-code/issues/74066) ⭐️ 7.0/10

一名用户报告在 Claude Code 的工作空间实例间可能出现会话或缓存泄漏，Claude Code 团队已展开调查，同时表示确信这很可能是一种幻觉。 如果证实，这种泄漏将对 LLM 编码代理的用户构成严重的隐私和安全风险，尤其是在 Claude Code 等工具日益普及的背景下。该事件也凸显了在 AI 系统中区分幻觉与真正基础设施缺陷的困难。 报告提到了多个 LLM 提供商出现类似的实例，社区成员指出极大的上下文窗口（80 万以上 token）可能增加幻觉的可能性。Claude Code 团队的 Thariq 确认收到报告并正在调查。

hackernews · chatmasta · Jul 4, 14:03 · [社区讨论](https://news.ycombinator.com/item?id=48785485)

**背景**: Claude Code 是 Anthropic 开发的 AI 驱动编码代理，可通过自然语言读取代码库、编辑文件和执行命令。它基于大型语言模型（LLM），用于软件开发。会话或缓存泄漏意味着一个用户会话的数据出现在另一个用户会话中，这是任何多租户系统中的严重安全缺陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 社区普遍持怀疑态度，许多评论者认为报告的行为是幻觉而非真正泄漏。不过，少数用户分享了与其他模型（如 Gemini）的类似经历，Claude Code 团队的官方回应确认他们正在调查。

**标签**: `#security`, `#LLM`, `#Claude Code`, `#hallucination`, `#privacy`

---

<a id="item-8"></a>
## [Linux 下 htop/top 输出详解指南](https://peteris.rocks/blog/htop/) ⭐️ 7.0/10

一篇 2019 年的博客文章全面解释了 Linux 上 htop 和 top 输出的各个方面，包括字段、颜色和内存指标。 本指南帮助 Linux 用户更好地理解系统监控工具，从而更有效地进行故障排除和系统优化。 文章强调虚拟内存报告可能具有误导性，建议使用常驻内存大小进行准确评估。它还涵盖了树视图和排序选项。

hackernews · theanonymousone · Jul 4, 12:00 · [社区讨论](https://news.ycombinator.com/item?id=48784777)

**背景**: htop 和 top 是类 Unix 系统上的命令行进程查看器，显示正在运行的进程和系统资源使用情况。htop 相比 top 提供了更交互式和色彩丰富的界面。理解它们的输出有助于用户监控 CPU、内存和进程行为。

**社区讨论**: 评论者分享了实用技巧：在 htop 中禁用用户线程并启用树状视图，在 top 中使用'>'按内存排序，以及迁移到 btop 以获得 GPU 监控等现代功能。大家一致认为常驻内存大小比虚拟内存更可靠。

**标签**: `#Linux`, `#htop`, `#top`, `#system monitoring`, `#process management`

---

<a id="item-9"></a>
## [Zig 将包管理从编译器移至构建系统](https://ziglang.org/devlog/2026/#2026-06-30) ⭐️ 7.0/10

Zig 于 2026 年 6 月 30 日宣布，将所有包管理功能从编译器移至构建系统。这一架构变化改进了工具链中的关注点分离。 这是一次重大的架构转变，明确了 Zig 工具链中的职责划分，可能简化维护并促进模块化开发。它使包管理能够独立于编译器发展，从而惠及 Zig 开发者。 此举将包的获取、解析和构建从编译器二进制文件中分离出来，符合 Zig 极简主义和显式控制的理念。这一变化是持续优化构建系统的一部分，长期计划是在 WebAssembly 虚拟机中运行构建系统。

hackernews · tosh · Jul 4, 16:30 · [社区讨论](https://news.ycombinator.com/item?id=48786638)

**背景**: Zig 是一种系统编程语言，旨在作为 C 语言的现代替代品，专注于性能、安全性和简洁性。历史上，包管理集成在编译器中，但 Zig 团队决定将其移至构建系统（属于 Zig 工具链的一部分），以降低编译器复杂性并提高模块化程度。构建系统负责编译和链接代码，而包管理处理依赖关系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极，用户赞赏关注点分离和健康的开发方式。评论者 vitaminCPP 提到长期计划是在 WebAssembly 虚拟机中运行构建系统，而 malkia 则警告包系统的泛滥可能使多语言项目复杂化。

**标签**: `#Zig`, `#package management`, `#build system`, `#programming languages`

---

<a id="item-10"></a>
## [Current AI 发布开源 AI 差距地图](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 7.0/10

全球非营利合作组织 Current AI 发布了开源 AI 差距地图 v0.1，收录了来自 228 个组织的 421 个产品，包括 266 个软件工具、85 个模型、50 个数据集和 20 个硬件项目。 该地图提供了开源 AI 生态系统的全面分类视图，帮助开发者、研究者和投资者识别差距和贡献机会，从而加速开放 AI 的发展。 这 421 个产品被组织为 14 个类别，分布在三个堆栈层：模型组件、产品/用户体验和基础设施。底层数据以 MIT 许可证发布在 GitHub 上，包含 1,184 个 YAML 文件和脚本，可通过 Datasette Lite 等工具进行进一步分析。

rss · Simon Willison · Jul 3, 22:04

**背景**: Current AI 于 2025 年 2 月在巴黎人工智能行动峰会上作为非营利组织成立，已获得 4 亿美元承诺资金。开源 AI 生态系统庞大但碎片化，利益相关者难以了解现有资源和差距。该地图旨在提供结构化概览并促进合作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://map.currentai.org/">Current AI – Open Source AI Gap Map</a></li>
<li><a href="https://www.currentai.org/blogs/introducing-the-gap-map-v0-1">Introducing the Gap Map v0.1</a></li>
<li><a href="https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/">Open Source AI Gap Map</a></li>

</ul>
</details>

**标签**: `#open source`, `#AI`, `#ecosystem`, `#mapping`, `#tools`

---

<a id="item-11"></a>
## [开发者 Josh W. Comeau 报告课程销售额因 AI 下降超 50%](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

知名开发者教育者 Josh W. Comeau 报告称，他的最新课程发布销量约为典型的三分之一，现有课程销售额也大幅下降，他将此归因于 AI 相关的就业不确定性以及基于 LLM 的个性化辅导的可用性。 来自一位受人尊敬的创作者的经验证据突显了一个日益增长的趋势：AI，尤其是大型语言模型，正在通过降低学习者购买付费课程的动机来扰乱在线教育市场，可能影响许多教育者和开发者教育生态系统。 Comeau 指出，他与多位课程创作者交流过，他们都看到收入下降了 50%或更多，随着人们转向 LLM（这些模型经常未经同意或补偿就使用创作者的作品）参与付费内容的人数减少。

rss · Simon Willison · Jul 3, 21:25

**背景**: 大型语言模型（LLM）是在大量文本上训练的神经网络，能够生成、总结和分析语言。它们为聊天机器人和辅导系统提供动力，可以提供个性化指导，这可能降低对结构化在线课程的需求。这一背景有助于解释为什么学习者可能选择免费的 AI 辅导而不是付费课程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/large-language-models">What Are Large Language Models (LLMs)? | IBM</a></li>

</ul>
</details>

**标签**: `#AI`, `#Developer Education`, `#Online Courses`, `#LLMs`, `#Tech Industry Trends`

---

<a id="item-12"></a>
## [《命令与征服：将军》通过 Fable 移植到苹果设备](https://github.com/ammaarreshi/Generals-Mac-iOS-iPad/tree/main) ⭐️ 6.0/10

基于 EA 的 GPL 源代码发布，利用 Fable 框架，《命令与征服：将军》原生移植版已发布，支持 macOS、iPhone 和 iPad。 此次移植将经典即时战略游戏带到现代苹果平台，展示了 AI 辅助代码转换和开源游戏引擎复用的潜力。 该移植基于 fbraz3/GeneralsX（已完成 macOS/Linux 转换），并增加了 iOS/iPadOS 支持及引擎修复。手势控制包括点选、框选、长按取消选择、双指滚动和捏合缩放。

hackernews · asronline · Jul 4, 19:41 · [社区讨论](https://news.ycombinator.com/item?id=48788283)

**背景**: 《命令与征服：将军》是 2003 年使用 SAGE 引擎的即时战略游戏。2025 年 2 月，EA 根据 GPL v3 许可证发布了多款 C&C 游戏的源代码，使社区移植成为可能。Fable 是一个辅助游戏跨平台移植的框架，常利用 AI 自动化转换任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/news/621397/command-conquer-open-source-ea-red-alert-renegade-generals">EA open-sources four more Command & Conquer games | The Verge</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为 AI 辅助移植是一个实用的案例，但有人觉得 AI 生成的文档风格令人不适。也有人指出该项目依赖此前的 GeneralsX 项目，并询问是否适用于《沙丘：皇帝之战》等其他游戏。

**标签**: `#game port`, `#macOS`, `#iOS`, `#open source`, `#RTS`

---

<a id="item-13"></a>
## [Verizon 应用更新导致 Gizmo 智能手表无法使用，强制迁移](https://www.jefftk.com/p/verizon-is-about-to-break-our-watches) ⭐️ 6.0/10

Verizon 的应用更新导致现有的 Gizmo 智能手表无法使用，用户必须迁移到新应用，否则将失去服务。作者描述了因 2FA 绑定到 Google Fi 号码而导致的迁移困难。 这一问题凸显了依赖运营商服务的脆弱性以及使用非标准电话号码进行双重验证的风险。它影响了依赖 Gizmo 手表进行儿童安全和沟通的家庭。 迁移过程据称很困难，一些用户丢失了联系人，需要多次尝试才能让新应用正常工作。Verizon 可能认为退款比修复问题更划算。

hackernews · jefftk · Jul 4, 17:52 · [社区讨论](https://news.ycombinator.com/item?id=48787329)

**背景**: Gizmo 智能手表是 Verizon 销售的儿童友好设备，具备 GPS、通话和家长批准的联系人功能。基于运营商的双重验证使用短信进行登录认证，但 Google Fi 号码常因被银行和企业检测到而无法接收此类短信。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.verizon.com/connected-smartwatches/verizon-gizmo-watch-3/">Gizmo Watch 3 Smart Watch | Verizon</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multi-factor_authentication">Multi-factor authentication - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，Google Fi 的双重验证问题是已知的，而且支持蜂窝网络的智能手表建立在脆弱的临时解决方案之上。一些用户费尽周折成功迁移，而另一些人则认为 Verizon 更愿意退款而不是修复问题。

**标签**: `#Verizon`, `#smartwatch`, `#2FA`, `#Google Fi`, `#carrier issues`

---

<a id="item-14"></a>
## [让 AI 模型自行判断以提高效率](https://simonwillison.net/2026/Jul/3/judgement/#atom-everything) ⭐️ 6.0/10

Simon Willison 分享了 Claude Code 团队炉边聊天的技巧：不要硬编码规则（如“只对大功能进行测试”），而是让 AI 模型（Fable）自行判断任务分配和模型选择。他还应用了一条提示词，将编码任务委托给使用较低功率模型的子代理，从而减少 token 消耗。 这种方法显著提高了使用 Claude Code 等 AI 编码助手的效率和成本效益。通过信任模型的判断，开发人员可以在不牺牲输出质量的前提下减少 token 消耗和费用，尤其是在 Fable 即将涨价的情况下。 Simon 使用了提示词：“对于所有编码任务，请运用你的判断力决定合适的较低功率模型，并在子代理中运行该模型。”Claude Code 将此保存为记忆文件，指示主循环将实现工作委托给运行 Sonnet 或 Haiku 模型的子代理，而将判断密集型任务保留在顶级 Fable 模型中。

rss · Simon Willison · Jul 3, 18:51

**背景**: Claude Code 是 Anthropic 的代理式编码工具，能够阅读代码库、编辑文件并运行命令。它提供多个模型层级：Fable（顶级，成本最高）、Opus、Sonnet 和 Haiku。Fable 功能强大但每 token 成本很高。通过允许 Fable 将常规编码委托给更便宜的模型（如 Sonnet 或 Haiku），用户可以优化 token 使用并降低成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/product/claude-code">Claude Code | Anthropic's agentic coding system \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI coding tools`, `#Claude Code`, `#prompt engineering`, `#token optimization`

---

<a id="item-15"></a>
## [Simon Willison 2026 年 6 月通讯：AI 模型与 Tokenmaxxing](https://simonwillison.net/2026/Jul/3/june-newsletter/#atom-everything) ⭐️ 6.0/10

Simon Willison 发布了 2026 年 6 月赞助者专属通讯，介绍了包括 Claude Fable 5、GPT-5.6 和 GLM-5.2 在内的主要 AI 模型发布，以及 tokenmaxxing 趋势和他个人项目（如 Datasette Apps 和 shot-scraper）的更新。 该通讯从一位受人尊敬的作者视角精选了近期重大 AI 发展动态，帮助读者了解领先模型和如 tokenmaxxing 等可能影响 AI 使用与生产力指标的新兴趋势。 该通讯仅限赞助者阅读，5 月通讯可作为预览，内容涉及 tokenmaxxing 作为有争议的生产力指标、GLM-5.2 成为最佳开源权重模型，以及 Willison 多个开源项目的更新。

rss · Simon Willison · Jul 3, 14:50

**背景**: Tokenmaxxing 是指最大化 AI token 使用量以衡量生产力的做法，但批评者认为这可能导致浪费行为和指标膨胀。GLM-5.2 是中国公司 Z.ai 发布的开源权重大型语言模型，采用 MIT 许可证，以其将论文描述转化为可运行代码的能力而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Token_maxxing">Token maxxing</a></li>
<li><a href="https://en.wikipedia.org/wiki/GLM-5.2">GLM-5.2</a></li>
<li><a href="https://github.com/simonw/shot-scraper-template">GitHub - simonw/shot-scraper-template: Template repository for setting up shot-scraper · GitHub</a></li>

</ul>
</details>

**标签**: `#AI`, `#newsletter`, `#LLMs`, `#Simon Willison`, `#models`

---