---
layout: default
title: "Horizon Summary: 2026-05-25 (ZH)"
date: 2026-05-25
lang: zh
---

> From 41 items, 10 important content pieces were selected

---

1. [内存成本升至 AI 芯片组件成本的近三分之二](#item-1) ⭐️ 8.0/10
2. [约束衰减：LLM 代理在严格架构规则下失效](#item-2) ⭐️ 8.0/10
3. [微软开源最早的 DOS 源代码](#item-3) ⭐️ 8.0/10
4. [Greg Brockman 访谈：OpenAI 内幕与非营利争议](#item-4) ⭐️ 8.0/10
5. [骗子滥用微软内部账户发送垃圾邮件链接](#item-5) ⭐️ 8.0/10
6. [Armin Ronacher 批评 AI 生成的错误报告](#item-6) ⭐️ 8.0/10
7. [DeepSeek Reasonix：原生编码代理，高缓存低费用](#item-7) ⭐️ 7.0/10
8. [发布《精通 Dyalog APL》交互式书籍](#item-8) ⭐️ 6.0/10
9. [Datasette 1.0a30 引入可自定义的跳转菜单](#item-9) ⭐️ 6.0/10
10. [AI 仅用几分钟便从 PDF 重制了 1983 年的游戏《疯人院》](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [内存成本升至 AI 芯片组件成本的近三分之二](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 8.0/10

Epoch AI 的新分析显示，内存（尤其是 DRAM 和高带宽内存 HBM）现在约占 AI 芯片总组件成本的三分之二，而历史上这一比例约为 20%。 这一成本转变对 AI 硬件定价和设计产生重大影响，因为内存开支现在占主导地位，可能影响 AI 系统的可负担性和扩展。同时，它也凸显了内存市场的严重供应限制，若不解决，可能成为 AI 发展的瓶颈。 成本份额增加是由于 AI 加速器对 HBM 需求飙升，HBM 需要先进堆叠技术，且每 GB 消耗的晶圆容量远高于标准 DRAM。例如，美光指出 HBM 与 DDR5 晶圆容量之间的转换比为 3:1，意味着 HBM 生产直接压缩了通用内存供应。

hackernews · intelkishan · May 24, 16:31 · [社区讨论](https://news.ycombinator.com/item?id=48258684)

**背景**: 动态随机存取存储器（DRAM）是计算机主存的主要类型，而高带宽内存（HBM）是一种专门的 3D 堆叠 DRAM，为 AI 和图形工作负载提供极高的带宽。当前的供应短缺有时被称为“RAMmageddon”，始于 2024 年，由于内存制造商将产能转向 AI 用的 HBM，减少了通用 DRAM 的供应，全面推高了价格。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DRAM">DRAM</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.rambus.com/blogs/hbm3-everything-you-need-to-know/">High Bandwidth Memory (HBM): Everything You Need to Know - Rambus</a></li>

</ul>
</details>

**社区讨论**: 评论者的观点不一：一些人认为，如果 DRAM 供应能赶上，成本可能降低 3 倍；另一些人则感叹价格急剧上涨（例如，96GB 内存从两年前的 250 美元涨到 1200 美元）。用户询问如何利用这一趋势，并对 DRAM 供应增长能否跟上 AI 需求表示怀疑，导致部分用户推迟硬件升级。

**标签**: `#AI hardware`, `#memory costs`, `#semiconductor economics`, `#GPU pricing`, `#DRAM`

---

<a id="item-2"></a>
## [约束衰减：LLM 代理在严格架构规则下失效](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

一篇新论文系统评估了结构约束下 LLM 代理在后端代码生成中的表现，并识别出“约束衰减”现象——随着约束累积，断言通过率下降约 30 个百分点。 这揭示了在生产级后端开发中使用 LLM 代理的关键可靠性差距，警告开发者当前代理适合快速原型开发，但不适合需要严格遵循架构的生产代码。 该研究聚焦于多文件后端生成，发现错误主要集中在惯例密集型框架上；由于成本原因，未测试前沿模型。

hackernews · wek · May 24, 12:55 · [社区讨论](https://news.ycombinator.com/item?id=48256912)

**背景**: 大型语言模型（LLM）代理是基于自然语言提示自动生成代码的 AI 模型。“约束衰减”是指代理在被迫遵循明确的架构规则（如架构模式、ORM 映射或框架惯例）时性能下降的现象。这之所以成问题，是因为生产级后端代码通常要求严格遵守此类约束。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.06445">Constraint Decay: The Fragility of LLM Agents in Backend Code ... Constraint Decay: The Fragility of LLM Agents in Backend Code ... Constraint Decay in Backend Code Generation - agentpatterns.ai Constraint Decay: The Fragility of LLM Agents in Back End ... [PDF] Constraint Decay: The Fragility of LLM Agents in ... Constraint Decay: The Fragility of LLM Agents in Backend Code ... Constraint Decay: The Fragility of LLM Agents in Backend Code ...</a></li>
<li><a href="https://www.agentpatterns.ai/verification/constraint-decay-backend-agents/">Constraint Decay in Backend Code Generation - agentpatterns.ai</a></li>

</ul>
</details>

**社区讨论**: 评论普遍赞同这些发现。jdlshore（可能是作者）总结了论文并指出未测试前沿模型。maxbond 将其与另一篇关于长周期任务的论文联系起来。alasano 分享了他们构建结构化编排器以强制执行约束的工作，而 vishvananda 将相关模式称为“钙化”。

**标签**: `#LLM agents`, `#code generation`, `#backend development`, `#constraint decay`, `#AI reliability`

---

<a id="item-3"></a>
## [微软开源最早的 DOS 源代码](https://arstechnica.com/gadgets/2026/04/microsoft-open-sources-the-earliest-dos-source-code-discovered-to-date/) ⭐️ 8.0/10

微软开源了已知最早的 DOS 源代码，这些代码是由历史学家团队通过 OCR 从纸质打印件中精心恢复而来的。 此次开源让人们得以一窥启动微软操作系统业务并推动个人电脑革命的软件起源。 源代码是通过 OCR 从 Tim Paterson 提供的几十年前的打印件中恢复而来，仓库中还包括了早期的 BASIC 解释器。

hackernews · DamnInteresting · May 24, 01:21 · [社区讨论](https://news.ycombinator.com/item?id=48253386)

**背景**: DOS（磁盘操作系统）是早期 IBM PC 及其兼容机的基础操作系统。微软最初从 Seattle Computer Products 获得了 86-DOS 的授权，后来演变为 MS-DOS。该代码库使用汇编语言编写，按现代标准来看规模非常小。

**社区讨论**: 评论者对此次开源表示感谢并强调了其历史重要性，指出 BASIC 代码可能更为关键。艰苦的 OCR 恢复过程也引起了讨论。

**标签**: `#open source`, `#DOS`, `#Microsoft`, `#software history`, `#assembly`

---

<a id="item-4"></a>
## [Greg Brockman 访谈：OpenAI 内幕与非营利争议](https://fs.blog/knowledge-project-podcast/greg-brockman/) ⭐️ 8.0/10

OpenAI 核心人物 Greg Brockman 在一次深度访谈中回顾了公司历史，讨论了近期的领导层动荡以及非营利结构的争议。 此次访谈提供了关于 OpenAI 内部冲突与治理问题的罕见内幕视角，这些正是当前 AI 发展方向及非营利实体在科技行业中角色辩论的核心。 访谈涉及董事会解雇 Sam Altman、Ilya Sutskever 的角色以及 Elon Musk 的诉讼。Brockman 还分享了作为诉讼证据的个人日记片段。

hackernews · prakashqwerty · May 24, 08:29 · [社区讨论](https://news.ycombinator.com/item?id=48255593)

**背景**: OpenAI 最初作为非营利性 AI 研究公司成立，后来设立了利润上限的子公司。该结构被批评为利用漏洞，允许创始人在声称非营利的同時获利。近期事件包括董事会争斗和联合创始人 Elon Musk 的诉讼。

**社区讨论**: 评论者对 OpenAI 的非营利声称持怀疑态度，有评论指出此类结构可能开创先例，使非营利地位形同虚设。另一些人则对关键细节未被深入探讨（如 Ilya Sutskever 的动机）表示失望。

**标签**: `#OpenAI`, `#AI`, `#interview`, `#non-profit`, `#drama`

---

<a id="item-5"></a>
## [骗子滥用微软内部账户发送垃圾邮件链接](https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/) ⭐️ 8.0/10

骗子正在利用一个内部微软账户发送垃圾邮件链接，借助该账户的受信任状态绕过安全过滤器。 此事件揭示了微软在域名管理和安全实践上的漏洞，可能削弱用户对来自微软域名邮件的信任，影响数百万用户。 该攻击利用了微软自己 Entra 租户内的一个内部账户，使垃圾邮件看似合法。微软尚未公开披露完整范围或修复措施。

hackernews · spike021 · May 24, 00:51 · [社区讨论](https://news.ycombinator.com/item?id=48253186)

**背景**: 微软使用大量域名进行内部和客户通信，导致难以追踪合法的邮件来源。攻击者经常滥用 Microsoft 365 租户通过 onmicrosoft.com 域名发送垃圾邮件，而此次事件似乎涉及对内部账户的类似利用。正确的域名管理和安全配置（如 DMARC 和 SPF）对于防止此类滥用至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://practical365.com/onmicrosoft-com-domains/">Stopping Spam Sent from Bad Microsoft 365 Domains | Practical365</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/01/06/phishing-actors-exploit-complex-routing-and-misconfigurations-to-spoof-domains/">Phishing actors exploit complex routing and misconfigurations to spoof domains | Microsoft Security Blog</a></li>
<li><a href="https://entra.news/p/inside-microsofts-entra-tenant-the">Inside Microsoft’s Entra Tenant: The Internal App Governance ...</a></li>

</ul>
</details>

**社区讨论**: 评论表达了对微软域名复杂性和安全问题的沮丧，一些用户注意到类似的钓鱼滥用，并建议使用子域名（如 internal.microsoft.com）而非分散的域名。

**标签**: `#security`, `#spam`, `#Microsoft`, `#phishing`, `#domain abuse`

---

<a id="item-6"></a>
## [Armin Ronacher 批评 AI 生成的错误报告](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Flask 和 Jinja 的创建者 Armin Ronacher 于 2026 年 5 月 24 日发表博文，批评 AI 生成的错误报告冗长、不准确且浪费维护者时间。他倡导采用简单的四点模板来描述人工观察到的问题。 这一评论凸显了开源维护中日益增长的问题：AI 工具生成的低质量错误报告加重了志愿维护者的负担。如果 Ronacher 提出的简洁格式被广泛采用，将有助于提高效率并减少开源社区中的倦怠现象。 Ronacher 特别用 'clanker'（对 AI 的贬称）来形容 AI 生成的报告，这些报告包含 '虚假的最小复现' 和 '对根本原因的完全猜测'。他建议错误报告只应包括：运行的命令、预期行为、实际行为以及确切的错误或日志输出。

rss · Simon Willison · May 24, 18:46

**背景**: 随着开发者使用大型语言模型（LLM）辅助软件开发，AI 生成的代码和错误报告变得越来越普遍。然而，这些报告往往缺乏准确性，包含自信但错误的结论，给维护者带来更多工作。'clanker' 一词是对 AI/机器人的贬义俚语，已在网络上流行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Clanker">Clanker - Wikipedia</a></li>
<li><a href="https://www.npr.org/2025/08/06/nx-s1-5493360/clanker-robot-slur-star-wars">What is a clanker and why do we need this word? : NPR</a></li>
<li><a href="https://stackoverflow.blog/2026/01/28/are-bugs-and-incidents-inevitable-with-ai-coding-agents/">Are bugs and incidents inevitable with AI coding agents? - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#open-source`, `#bug reporting`, `#AI`, `#software maintenance`, `#LLM`

---

<a id="item-7"></a>
## [DeepSeek Reasonix：原生编码代理，高缓存低费用](https://esengine.github.io/DeepSeek-Reasonix/) ⭐️ 7.0/10

DeepSeek Reasonix 是一款针对 DeepSeek V4 Pro 优化的原生编码代理，通过积极利用缓存来大幅降低 API 费用。它在终端中运行，采用缓存优先循环和闪存优先成本控制策略。 通过最大化缓存命中率，Reasonix 减少了 token 消耗和费用，使 DeepSeek V4 Pro 对开发者更经济实惠。这解决了 AI 编码代理的一个关键痛点——高昂的 API 费用，可能促进更广泛的采用。 然而，Reasonix 的用户体验受到批评：网站设计不佳，动画打字导致布局错位，一些用户质疑是否需要专用代理，因为现有工具已经可以利用 DeepSeek 的缓存。

hackernews · Alifatisk · May 24, 13:02 · [社区讨论](https://news.ycombinator.com/item?id=48256953)

**背景**: DeepSeek V4 Pro 是一个大型混合专家语言模型，拥有 1.6 万亿参数（激活 49B），支持 100 万 token 的上下文。其 API 提供缓存折扣，但有效利用缓存需要精心设计提示。Reasonix 旨在自动化这一缓存优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://esengine.github.io/DeepSeek-Reasonix/">Reasonix — DeepSeek -native AI coding agent</a></li>
<li><a href="https://api-docs.deepseek.com/quick_start/agent_integrations/reasonix">Integrate with Reasonix | DeepSeek API Docs</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：一些用户指出，通过简单的桥接即可实现缓存优势，另一些则批评代理的 UX 和网站设计。有用户建议作者应向现有工具提交 PR，而不是构建单独的工具。总体而言，对该工具的新颖性存在怀疑。

**标签**: `#AI coding agent`, `#DeepSeek`, `#caching`, `#cost optimization`

---

<a id="item-8"></a>
## [发布《精通 Dyalog APL》交互式书籍](https://mastering.dyalog.com/README.html) ⭐️ 6.0/10

一本名为《精通 Dyalog APL》的综合交互式书籍发布，包含 Jupyter Notebook 示例，提供 Dyalog APL 编程语言的现代交互式介绍。 该资源通过交互式示例降低学习 APL 的门槛，APL 以其简洁的数组导向语法著称。它帮助程序员在实用的现代环境中探索数组编程概念。 该书可在 mastering.dyalog.com 上以嵌入 Jupyter Notebook 的 HTML 形式获取，同时提供 PDF 版本供离线阅读。原书已获好评，交互式形式进一步提升了学习体验。

hackernews · tosh · May 24, 11:42 · [社区讨论](https://news.ycombinator.com/item?id=48256475)

**背景**: APL（A Programming Language）是肯尼斯·艾佛森在 1960 年代开发的编程语言，其核心数据类型是多维数组。它使用大量特殊符号表示函数和运算符，使得代码极为简洁。Dyalog APL 是 Dyalog Ltd.开发的现代专有实现，常用于金融和数据分析领域，因其强大的数组处理能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dyalog_APL">Dyalog APL</a></li>
<li><a href="https://en.wikipedia.org/wiki/APL_(programming_language)">APL (programming language) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论对交互式笔记本格式表示肯定，认为其使 APL 符号的学习更直观。部分读者对 Dyalog 的专有许可表示担忧，并推荐了像 learnapl 这样的开源学习资源。还有人分享了使用 LLM 学习 APL 或将 APL 程序翻译为 NumPy 的个人经验。

**标签**: `#APL`, `#Dyalog`, `#programming-language`, `#learning-resource`, `#array-programming`

---

<a id="item-9"></a>
## [Datasette 1.0a30 引入可自定义的跳转菜单](https://simonwillison.net/2026/May/24/datasette/#atom-everything) ⭐️ 6.0/10

Datasette 1.0a30 新增了可自定义的“跳转到...”菜单，用户可以快速导航到数据库、表格等资源。同时引入新的插件钩子 jump_items_sql()，允许插件添加自己的可搜索项。 该功能提升了用户导航体验，并增强了 Datasette 的可扩展性，插件开发者可以集成自定义导航项。这改善了用户体验，并促进了生态系统的成长。 菜单通过按“/”键触发，在任意 Datasette 实例（例如 latest.datasette.io）上均可使用。jump_items_sql() 插件钩子允许插件定义 SQL 查询，查询结果会成为菜单中的可搜索项。

rss · Simon Willison · May 24, 23:52

**背景**: Datasette 是一个开源 Python 工具，用于将 SQLite 数据库探索和发布为交互式网页。它通过钩子支持插件扩展新功能。此版本为 alpha 版本，表示仍在开发中，在稳定版 1.0 发布前可能会有变动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/datasette/issues/2283">`query_actions` plugin hook - like `table_actions` and `database_actions` for the query/canned query page · Issue #2283 · simonw/datasette</a></li>

</ul>
</details>

**标签**: `#datasette`, `#python`, `#sqlite`, `#plugin`, `#data publishing`

---

<a id="item-10"></a>
## [AI 仅用几分钟便从 PDF 重制了 1983 年的游戏《疯人院》](https://simonwillison.net/2026/May/24/usborne-mad-house/#atom-everything) ⭐️ 6.0/10

Simon Willison 将 1983 年 Usborne 出版的《Creepy Computer Games》PDF 输入到 Anthropic 的 Claude AI 中，随后 Claude 生成了一个完全可交互的 JavaScript 和 HTML 版本的《疯人院》游戏。 这展示了大型语言模型如何快速现代化遗留软件，让历史游戏无需手动编程即可再次游玩，降低了复古游戏保存的门槛。 Willison 使用了一个提示词给 Claude：‘使用纯 JavaScript 构建一个能精确重现书中《疯人院》游戏的制品，确保支持移动端并具有合适的复古美学。’他还要求游戏标明书籍出处并链接到 Usborne 的免费 PDF。

rss · Simon Willison · May 24, 17:14

**背景**: Usborne 在 20 世纪 80 年代出版了一系列计算机书籍，包含供 ZX81 和 Commodore 64 等家用电脑输入的游戏。近年来，Usborne 在线提供了这些书籍的免费 PDF。Claude 是 Anthropic 开发的大型语言模型，以其代码生成能力而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_AI">Claude AI</a></li>
<li><a href="https://archive.org/details/Creepy_Computer_Games_1983_Usborne_Publishing">Usborne creepy computer games : Reynolds, Colin... : Internet Archive</a></li>

</ul>
</details>

**社区讨论**: 在 Hacker News 上，用户表达了对 Usborne 书籍的怀旧之情，并对使用 AI 从 PDF 重制其他经典游戏表示兴趣。一些人讨论了重制的准确性以及 AI 生成代码的局限性。

**标签**: `#retro computing`, `#AI`, `#game recreation`, `#javascript`, `#claude`

---