---
layout: default
title: "Horizon Summary: 2026-07-19 (ZH)"
date: 2026-07-19
lang: zh
---

> From 37 items, 9 important content pieces were selected

---

1. [GPT-5.6 用提示解决凸优化三十年难题](#item-1) ⭐️ 9.0/10
2. [LG 显示器通过 Windows Update 静默安装软件](#item-2) ⭐️ 8.0/10
3. [Anthropic 改变计划，永久保留 Claude Fable 5](#item-3) ⭐️ 8.0/10
4. [建设社区需要主动努力](#item-4) ⭐️ 7.0/10
5. [Fable 5 对比 GPT-5.6 Sol 在 NP 难问题上的 /goal 测试](#item-5) ⭐️ 7.0/10
6. [指南：设置备用 Mac 以控制 Claude Code](#item-6) ⭐️ 7.0/10
7. [基于 Pyodide 的 SQLite 查询解释器工具在浏览器中运行](#item-7) ⭐️ 7.0/10
8. [LLM 陈词滥调高亮工具发布](#item-8) ⭐️ 6.0/10
9. [通过将高尔夫球场改造成公园来抵消数据中心用水](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GPT-5.6 用提示解决凸优化三十年难题](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 9.0/10

OpenAI 的 GPT-5.6 模型通过一个提示解决了凸优化中一个存在 30 年的开放问题，给出了关于迭代复杂度下界的正确证明。 这一成就表明大语言模型能够为数学研究做出实质性贡献，可能加速优化及相关领域的进展。 该问题涉及在球形域上最小化凸 Lipschitz 函数的下界，证明已得到专家验证；所用模型为 ChatGPT Pro 版本（Sol Pro），而非 Ultra。

hackernews · mbustamanter · Jul 18, 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48957779)

**背景**: 凸优化是数学优化的一个子领域，研究在凸集上最小化凸函数。一个 30 年的差距指的是关于一阶方法所需迭代次数的未解猜想。像 GPT-5.6 这样的大语言模型在大量文本数据上训练，能够在适当提示下生成数学证明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization">Convex optimization</a></li>
<li><a href="https://web.stanford.edu/~boyd/cvxbook/bv_cvxbook.pdf">Convex Optimization</a></li>

</ul>
</details>

**社区讨论**: 评论者指出该问题虽然小众但仍是真实贡献，一位专家确认了证明的有效性。一些人讨论了数学研究的影响，认为低垂的果实问题可能不再需要人类努力，而另一些人将其与初级软件开发任务进行了比较。

**标签**: `#AI`, `#machine learning`, `#mathematics`, `#convex optimization`, `#LLMs`

---

<a id="item-2"></a>
## [LG 显示器通过 Windows Update 静默安装软件](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent) ⭐️ 8.0/10

LG 显示器利用 Windows Update，在通过 HDMI 连接后自动在后台安装未经签名的第三方软件，且无需用户同意，该软件拥有完全系统访问权限。 这是严重的安全和隐私侵犯，因为它在未经用户同意的情况下安装具有完全系统和互联网访问权限的软件，影响所有 LG 显示器用户，并削弱了对硬件厂商和 Windows 更新机制的信任。 一旦通过 HDMI 连接 LG 显示器，该软件就会立即安装，并在每次启动时运行，且无沙箱保护。可通过组策略或设备安装设置阻止自动下载制造商应用的解决方法。

hackernews · baranul · Jul 18, 10:21 · [社区讨论](https://news.ycombinator.com/item?id=48956688)

**背景**: Windows Update 能够自动分发硬件设备的驱动和关联软件。硬件供应商可通过 Windows 硬件开发中心提交包进行认证和分发。通常微软会验证提交，但此事件表明未经验证的软件也可能被分发。LG 利用这一机制在无用户交互的情况下推送其安装程序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/windows-hardware/drivers/dashboard/understanding-windows-update-automatic-and-optional-rules-for-driver-distribution">Understanding Windows Update rules for driver distribution - Windows drivers | Microsoft Learn</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows-hardware/drivers/dashboard/">Partner Center for Windows Hardware - Windows drivers</a></li>
<li><a href="https://windowsforum.com/threads/demystifying-windows-driver-updates-how-theyre-made-targeted-and-delivered.385588/">Demystifying Windows Driver Updates: How They're Made, Targeted, and Delivered | Windows Forum</a></li>

</ul>
</details>

**社区讨论**: 社区表达了愤怒，有评论者详细指出情况比标题描述的更严重，强调缺乏用户同意和完全系统访问权限。还有用户分享了通过组策略或设备安装设置的解决方法。一些人批评微软未执行相关规范以阻止此类行为。

**标签**: `#security`, `#privacy`, `#Windows`, `#LG`, `#software distribution`

---

<a id="item-3"></a>
## [Anthropic 改变计划，永久保留 Claude Fable 5](https://simonwillison.net/2026/Jul/18/claude-make-fable-5-permanent/#atom-everything) ⭐️ 8.0/10

Anthropic 撤销了将 Claude Fable 5 从订阅中移除的决定；从 2026 年 7 月 20 日起，Fable 5 将以 50%的限额包含在 Max 和 Team Premium 计划中。Pro 和 Team Standard 用户仍可通过使用积分访问，并获得一次性 100 美元积分。 这一转变凸显了 AI 模型市场的激烈竞争，定价和对前沿模型的访问直接影响用户留存。这也表明，来自 GPT-5.6 Sol 和 Kimi 3 等模型的竞争压力可以克服计算能力限制。 Fable 5 仍然不包含在每月 20 美元的计划中，仅包含在更高级别的 Max（每月 100 或 200 美元）和 Team Premium 计划中。最初移除该模型的计划是出于计算能力考虑，Anthropic 可能需要减少训练工作以释放 GPU 用于服务。

rss · Simon Willison · Jul 18, 06:00

**背景**: Claude Fable 5 是 Anthropic 于 2026 年 6 月 9 日推出的 'Mythos 级' 模型，具备先进的视觉和推理能力，适用于通用用途。竞争对手如 OpenAI 的 GPT-5.6 Sol 和 Moonshot AI 的 Kimi 3 近期进入市场，给 Anthropic 的定价策略带来了压力，迫使其撤销了从订阅中移除 Fable 5 的计划。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://simtheory.ai/model-card/gpt-5.6-sol/">GPT - 5 . 6 Sol - AI Model Details | Simtheory</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#Claude`, `#Fable 5`, `#AI pricing`, `#competition`

---

<a id="item-4"></a>
## [建设社区需要主动努力](https://www.benlandautaylor.com/p/if-you-build-it-they-will-come) ⭐️ 7.0/10

一篇论文指出，繁荣的社交场景并非自动出现，而是需要主动建设，将被动消费比作期待不种植就能长出野生蓝莓。 这一见解挑战了社区中普遍的消费者心态，强调孤独和社会疏离感可以通过草根努力而非被动等待来解决。 该文章在 Hacker News 上获得了 230 个赞和 83 条评论，表明强烈共鸣，评论者讨论了作为社交纽带的脆弱性以及机构在代际间的流失。

hackernews · barry-cotter · Jul 18, 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48959090)

**背景**: 许多人将社交场景视为无需维护的自然现象，就像野莓一样。这篇文章反驳了这一点，认为社区需要有意识的创造和持续的努力，呼应了开源和本地聚会中的草根运动。

**社区讨论**: 评论者分享了组织活动时感到脆弱的个人经历，并感叹年轻一代不再从长辈那里学习社交领导力的代际鸿沟。一些人呼吁从被动消费转向主动参与。

**标签**: `#community-building`, `#social-dynamics`, `#grassroots`, `#hacker-news-discussion`

---

<a id="item-5"></a>
## [Fable 5 对比 GPT-5.6 Sol 在 NP 难问题上的 /goal 测试](https://charlesazam.com/blog/fable-5-gpt-5-6-sol-goal/) ⭐️ 7.0/10

一篇博客文章对比了 Anthropic 的 Fable 5 和 OpenAI 的 GPT-5.6 Sol 在一个 NP 难问题上的表现，以评估 '/goal' 指令提示的有效性。结果显示每个模型在复杂问题求解中遵循明确目标指令的能力。 这项比较揭示了不同 AI 模型在挑战性任务中遵循指令的能力，这对自主智能体开发至关重要。研究结果帮助用户为编码和优化问题选择合适的模型及提示策略。 该博客采用了 NP 难问题作为测试案例，可能涉及搜索或优化。GPT-5.6 Sol 是 OpenAI 最新的编码模型，在 Artificial Analysis 编码智能体指数上达到了最先进水平，超越了 Fable 5，同时使用更少的 token 和更低的成本。

hackernews · couAUIA · Jul 18, 11:00 · [社区讨论](https://news.ycombinator.com/item?id=48956879)

**背景**: NP 难问题在计算上非常困难，通常需要启发式搜索。'/goal' 指令是一种提示技术，用户明确陈述目标以引导 AI 的推理。Fable 5 是 Anthropic 的高端模型，用于自主工作；而 GPT-5.6 Sol 是 OpenAI 于 2026 年 7 月发布的高级编码模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/docs/models/claude-fable-5">Claude Fable 5 | Cursor Docs</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://learnprompting.org/docs/basics/instructions">Instruction Prompting : Complex Tasks with Simple AI Prompts</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了不同观点：一些人指出 Anthropic 模型在长时间会话中会忘记指令，认为 /goal 可能对较短任务有帮助；另一些人则强调 GPT 在优化问题上的优越表现，并提到了其近期在 AtCoder 启发式竞赛中的胜利。

**标签**: `#AI`, `#large language models`, `#benchmarking`, `#problem solving`, `#machine learning`

---

<a id="item-6"></a>
## [指南：设置备用 Mac 以控制 Claude Code](https://ykdojo.github.io/claude-controls-mac/) ⭐️ 7.0/10

一份详细介绍如何设置备用 Mac 来运行 Claude Code（一个 AI 编码代理）并在隔离环境中控制它的分步指南已经发布。 该指南解决了对 AI 代理进行安全隔离的日益增长的需求，使开发者能够安全地实验，而不会危及他们的主系统。 该指南建议使用物理备用 Mac 而非虚拟机进行图形开发，但社区评论建议在一般测试中使用虚拟机替代方案，并强调通过 VLAN 进行网络隔离。

hackernews · ykev · Jul 18, 16:12 · [社区讨论](https://news.ycombinator.com/item?id=48959392)

**背景**: Claude Code 是 Anthropic 开发的一款代理式编码工具，能够理解代码库、编辑文件并运行命令。在专用机器上运行此类代理提供了一个沙盒环境，以防止对用户主系统的意外修改，这对于安全性和稳定性至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>

</ul>
</details>

**社区讨论**: 社区评论就虚拟机是否足以实现隔离展开讨论，一些用户提供了基于 libvirt 的脚本设置。另一些人则强调了网络安全的重要性，例如将备用 Mac 置于单独的 VLAN 中，并采用拒绝所有防火墙规则。

**标签**: `#AI agents`, `#Claude Code`, `#isolation`, `#security`, `#macOS`

---

<a id="item-7"></a>
## [基于 Pyodide 的 SQLite 查询解释器工具在浏览器中运行](https://simonwillison.net/2026/Jul/18/sqlite-query-explainer/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了一款交互式 SQLite 查询解释器工具，该工具通过 Pyodide 和 WebAssembly 完全在浏览器中运行。它为 EXPLAIN 和 EXPLAIN QUERY PLAN 输出提供易于理解的解释。 该工具使那些觉得原始查询计划难以理解的开发人员能够轻松分析 SQLite 查询计划。它降低了理解查询性能和优化数据库查询的门槛，尤其适用于教育目的。 该工具在 Python 中运行 SQLite，并通过 Pyodide 编译为 WebAssembly，全部在浏览器内完成。作者指出他并未完全验证解释的准确性，因此用户应谨慎使用。

rss · Simon Willison · Jul 18, 17:19

**背景**: SQLite 的 EXPLAIN QUERY PLAN 命令提供了查询执行方式的高层概述，包括索引使用和连接策略。Pyodide 是一个基于 WebAssembly 的浏览器 Python 发行版，允许 Python 代码在客户端运行。该工具结合了这两者，提供交互式学习体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pyodide.org/en/stable/console.html">pyodide .org/en/stable/console.html</a></li>
<li><a href="https://www.sqlite.org/eqp.html">Explain query plan</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#query plan`, `#webassembly`, `#tool`, `#educational`

---

<a id="item-8"></a>
## [LLM 陈词滥调高亮工具发布](https://simonwillison.net/2026/Jul/17/llm-cliche-highlighter/#atom-everything) ⭐️ 6.0/10

Simon Willison 发布了一个网页工具，用于高亮 LLM 生成文本中常见的陈词滥调，例如“无废话、无填充、无行话”。该工具是通过 Fable 5 使用 vibe coding 方式创建的。 该工具解决了对 AI 生成内容中可预测语言模式日益增长的挫败感，帮助写作者和编辑识别并避免陈词滥调。它展示了 AI 辅助开发的一个实用案例，同时批判了 AI 输出本身。 该工具高亮显示十种常见陈词滥调模式，例如“is real and”和“worth naming”。它可以通过 r.jina.ai 获取 URL 来分析文章，并提供匹配数和标记句子的摘要。

rss · Simon Willison · Jul 17, 12:11

**背景**: Vibe coding 是由 Andrej Karpathy 创造的术语，指开发者将任务描述给 LLM 并接受 AI 生成的代码而无需彻底审查的开发方式。r.jina.ai 服务可将任何 URL 转换为 LLM 友好的输入格式，使此类高亮工具能够获取并分析网页内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>
<li><a href="https://github.com/jina-ai/reader">GitHub - jina-ai/reader: Convert any URL to an LLM-friendly input with a simple prefix https://r.jina.ai/ · GitHub</a></li>
<li><a href="https://jina.ai/">Jina AI - Your Search Foundation, Supercharged.</a></li>

</ul>
</details>

**标签**: `#LLM`, `#tool`, `#writing`, `#clichés`

---

<a id="item-9"></a>
## [通过将高尔夫球场改造成公园来抵消数据中心用水](https://simonwillison.net/2026/Jul/17/spot-birds-not-golf/#atom-everything) ⭐️ 6.0/10

Simon Willison 的一篇博文提出，像 Google 这样的超大规模云服务商可以通过购买并将高尔夫球场改造成公共公园来抵消其数据中心的水消耗。具体计算显示，Google 2025 年 109 亿加仑的用水量可通过收购科切拉山谷约 40 个高尔夫球场来抵消。 这个想法凸显了数据中心用水日益增长的环境问题，尤其是在 AI 工作负载增加的背景下，并提出了一种基于土地利用的创造性解决方案，同时也能带来公共效益。它将讨论引向科技公司的企业责任和可持续发展。 计算基于 Google 2025 年 109 亿加仑的年用水量（约每天 3000 万加仑），以及科切拉山谷每个高尔夫球场每天约 75 万加仑的用水量，因此需要 40 个球场来抵消 Google 的用水量。这篇博文幽默地建议将这些球场改造成公园，并为前会员提供观鸟设备。

rss · Simon Willison · Jul 17, 02:58

**背景**: 超大规模云服务商是指像 Google、Amazon 和 Microsoft 这样运营大型数据中心的大型云提供商。数据中心需要大量水用于冷却，美国数据中心估计每天消耗 4.49 亿加仑（截至 2021 年）。英亩-英尺是一个水体积单位，约等于 325,851 加仑，常用于美国水资源管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.digitalocean.com/resources/articles/hyperscaler-cloud">What is a Hyperscaler Cloud ? Top Features and... | DigitalOcean</a></li>
<li><a href="https://www.eesi.org/articles/view/data-centers-and-water-consumption">Data Centers and Water Consumption | Article | EESI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Acre-foot">Acre-foot - Wikipedia</a></li>

</ul>
</details>

**标签**: `#ai-energy-usage`, `#data centers`, `#water consumption`, `#sustainability`

---