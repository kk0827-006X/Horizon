---
layout: default
title: "Horizon Summary: 2026-07-12 (ZH)"
date: 2026-07-12
lang: zh
---

> From 34 items, 10 important content pieces were selected

---

1. [vLLM v0.25.0：Model Runner V2 成为默认，移除 PagedAttention](#item-1) ⭐️ 9.0/10
2. [ClickHouse 利用 so_reuseport 和 Peering 将 PgBouncer 吞吐量提升 4 倍](#item-2) ⭐️ 8.0/10
3. [别再叫我去问大语言模型了](#item-3) ⭐️ 7.0/10
4. [Nvidia、CoreWeave 与 Nebius：GPU 循环融资内幕](#item-4) ⭐️ 7.0/10
5. [为什么应在 SQLite 中使用严格表](#item-5) ⭐️ 7.0/10
6. [女划手打破加州至夏威夷单人纪录](#item-6) ⭐️ 7.0/10
7. [尼莱·帕特尔：AR 眼镜必然侵犯隐私](#item-7) ⭐️ 7.0/10
8. [sqlite-utils 4.1 新增自定义代码、类型覆盖和删除索引](#item-8) ⭐️ 6.0/10
9. [Ant：新 JavaScript 运行时与生态系统引发争议](#item-9) ⭐️ 6.0/10
10. [免费平台教你从零重建 Redis、Git 和数据库](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0：Model Runner V2 成为默认，移除 PagedAttention](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 发布，将 Model Runner V2 设为所有密集模型的默认执行路径，移除了传统的 PagedAttention 实现，实现了 Transformers 后端与原生性能的持平，并引入了新模型和流式解析引擎。 此次发布是广泛使用的 LLM 推理引擎的重大架构变革，提升了性能、可维护性和可扩展性，巩固了 vLLM 作为领先开源推理系统的地位。 此版本包含来自 232 位贡献者的 558 次提交，将 Model Runner V2 设为密集模型的默认路径，移除了 PagedAttention，并实现了 Transformers 后端的性能持平。新增了 LLaVA-OneVision-2、GLM-5 和 MiniMax-M3 等模型，引入了新的流式解析引擎，并支持异构词汇表的通用推测解码。

github · khluu · Jul 11, 20:06

**背景**: vLLM 是一个高性能大语言模型推理引擎，最初使用 PagedAttention 实现高效的 KV 缓存管理。Model Runner V2 是重新设计的执行核心，提升了模块化和性能。PagedAttention 曾是关键技术，但其旧实现已在 v0.25.0 中被更高效的 V1/MRv2 后端取代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#open-source`, `#performance`, `#release notes`

---

<a id="item-2"></a>
## [ClickHouse 利用 so_reuseport 和 Peering 将 PgBouncer 吞吐量提升 4 倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse 工程师通过利用 Linux 的 SO_REUSEPORT 套接字选项并在工作进程之间实现 peering 机制以正确转发取消请求，将 PgBouncer 的吞吐量提升了 4 倍。 这一改进使 PgBouncer 在高流量 PostgreSQL 部署中更具竞争力，可能减少对像 Odyssey 或 pgdog 等替代池化工具的依赖，并展示了如何将内核特性与应用层更改相结合来扩展遗留软件。 SO_REUSEPORT 允许多个 PgBouncer 进程绑定到同一端口，使内核能够分发连接，而 peering 在工作进程之间共享会话所有权，从而确保取消请求落到正确的进程上。

hackernews · saisrirampur · Jul 11, 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是 PostgreSQL 的轻量级连接池工具，通过管理数据库连接池来降低开销。在典型设置中，单个 PgBouncer 进程处理所有连接，可能成为瓶颈。SO_REUSEPORT 是 Linux 内核 3.9 引入的套接字选项，允许多个套接字绑定到同一端口，使内核能够将传入连接负载均衡到多个工作进程。Peering 是 PgBouncer 内部的一种机制，用于在工作进程之间共享会话所有权信息，以正确处理取消请求等操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/how-modern-kernels-handle-massive-traffic-use-jisan-ahmed-ghg1c">How Modern Kernels Handle Massive Traffic : the use of...</a></li>
<li><a href="https://github.com/yandex/odyssey">GitHub - yandex/ odyssey : Scalable PostgreSQL connection pooler</a></li>
<li><a href="https://github.com/pgdogdev/pgdog">GitHub - pgdogdev/pgdog: PostgreSQL connection pooler, load balancer and database sharder. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者推荐了像 Odyssey 和 pgdog 这样的替代池化工具，指出它们天生具有可伸缩性。一些人称赞了技术细节，特别是 SO_REUSEPORT，而另一些人则询问了 peering 的配置。总体情绪是正面的，但也强调其他工具中存在类似功能。

**标签**: `#PgBouncer`, `#PostgreSQL`, `#connection pooling`, `#performance optimization`, `#systems engineering`

---

<a id="item-3"></a>
## [别再叫我去问大语言模型了](https://blog.yaelwrites.com/stop-telling-me-to-ask-an-llm/) ⭐️ 7.0/10

作者批评了那种遇到问题就让人“去问大语言模型”的反射性建议，指出自己已经问过但仍需要人类专业知识，并凸显了其先前询问被忽视的沟通鸿沟。 这篇观点文章揭示了大语言模型普及后技术社区中日益增长的摩擦，强调了改善沟通和尊重已有努力的必要性，并影响我们设计 AI 交互和工作流程的方式。 作者特别提到使用了 Claude，并举例说明自己如何被“去问 Claude”的回答搪塞。这篇文章并非反大语言模型，而是批评那种不承认已有努力、不经思考就将问题抛给 AI 的做法。

hackernews · theorchid · Jul 11, 22:28 · [社区讨论](https://news.ycombinator.com/item?id=48876441)

**社区讨论**: 评论呈现多元观点：一些人认同这是沟通问题，建议主动说明已做的研究；另一些人则认为预先展示工作成果可以避免这种反射性回应。总体共识是清晰的沟通和上下文至关重要。

**标签**: `#LLM`, `#human-computer interaction`, `#communication`, `#AI limitations`, `#technical discussion`

---

<a id="item-4"></a>
## [Nvidia、CoreWeave 与 Nebius：GPU 循环融资内幕](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 7.0/10

文章揭示了 Nvidia、CoreWeave 和 Nebius 之间的循环融资模式，引发了对经济可持续性的担忧。 这种模式可能吹大 AI 泡沫并扭曲市场信号，影响投资者和整个 AI 基础设施生态系统。 Nvidia 向 CoreWeave 投资 20 亿美元获得 9%股权，而 CoreWeave 计划 2026 年投入 350 亿美元资本支出，展现了循环资金的规模。

hackernews · adletbalzhanov · Jul 11, 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48873836)

**背景**: 循环融资是指科技巨头投资 AI 初创公司，然后初创公司用这些资金购买投资者的产品。在 GPU 云市场中，Nvidia 投资于 CoreWeave 和 Nebius 等 GPU 云提供商，后者再购买 Nvidia 的 GPU，形成收入循环。这种做法引发了关于估值过高和增长不可持续的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://markets.financialcontent.com/stocks/article/marketminute-2026-3-5-the-great-ai-loop-why-circular-financing-is-raising-alarms-on-wall-street">FinancialContent - The Great AI Loop: Why ' Circular Financing ' is...</a></li>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nebius_Group">Nebius Group - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者就循环融资的重要性展开辩论。有人认为 Nvidia 的投资仅占 CoreWeave 资本支出的一小部分，并非真正的循环。另有人质疑旧硬件盈利能力和过度建设风险。还有评论指出许可延迟可能限制过剩产能。

**标签**: `#GPU`, `#cloud computing`, `#AI infrastructure`, `#investment`, `#Nvidia`

---

<a id="item-5"></a>
## [为什么应在 SQLite 中使用严格表](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 7.0/10

Evan Hahn 的一篇博文建议在 SQLite 中使用 STRICT 表来强制执行类型安全，认为默认的灵活类型可能导致微妙的错误。文章指出，自 SQLite 3.37.0 起可用的 STRICT 表会强制列类型并拒绝不匹配的数据。 这一建议对依赖数据完整性的 SQLite 用户尤为重要，尤其是当多个应用程序访问同一数据库时。采用 STRICT 表可以防止数据损坏并使调试更容易，但这牺牲了 SQLite 众所周知的灵活性。 STRICT 表要求每一列都有类型，并拒绝与声明的类型不匹配的值（例如，在 INTEGER 列中存储文本）。然而，它们不支持某些数据类型如 DATE，并且由于要保持向后兼容性和“灵活类型”哲学，它们不是默认选项。

hackernews · ingve · Jul 11, 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48873940)

**背景**: SQLite 传统上使用动态类型关联，这意味着列可以存储任何类型，而不管声明的类型如何。这种灵活性在 SQLite 的 'flextypegood' 文档中有所阐述，是为了兼容旧脚本和临时查询而故意为之。2021 年引入的 STRICT 表提供了一种可选的方式来实现静态类型，使 SQLite 在需要严格模式的用例中与传统关系数据库保持一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite.org/stricttables.html">STRICT Tables - SQLite</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>

</ul>
</details>

**社区讨论**: 社区讨论意见不一：一些用户强烈偏好严格类型并希望它成为默认，而另一些用户则引用 SQLite 官方的 'flextypegood' 理由，强调灵活性的好处。评论者还指出 STRICT 表缺少诸如 DATE 等类型，可能不适合所有嵌入式用例，但总体而言，这篇文章引发了关于 SQLite 设计理念的健康讨论。

**标签**: `#SQLite`, `#database`, `#type safety`, `#best practices`

---

<a id="item-6"></a>
## [女划手打破加州至夏威夷单人纪录](https://www.theguardian.com/us-news/2026/jul/04/california-hawaii-rowing-solo-journey) ⭐️ 7.0/10

凯尔西·芬德勒成为从加州划船到夏威夷最快的人，以 44 天完成旅程，比之前的男性纪录快六天。 这一成就凸显了人类惊人的耐力以及女性在极限运动中的日益认可，激励着未来的冒险者。 所使用的船长度为 21 英尺，宽度为 5.5 英尺，专为长途海洋划船设计，并精心安排了物资补给。

hackernews · speckx · Jul 11, 17:03 · [社区讨论](https://news.ycombinator.com/item?id=48873692)

**背景**: 海洋划船是一项艰苦的耐力运动，单人划船者要面对极端天气、海浪和孤独。纪录通常在大西洋或太平洋等重大海洋横渡中创造。从加州到夏威夷的航线大约 2400 英里。

**社区讨论**: 评论者对这一身体和心理挑战表示惊叹，有人提到自己 45 英里的横渡用了 9 小时就精疲力尽。其他人则对船只设计和后勤技术支持细节感兴趣，表现出既钦佩又好奇的态度。

**标签**: `#human endurance`, `#ocean rowing`, `#record-breaking`, `#adventure`

---

<a id="item-7"></a>
## [尼莱·帕特尔：AR 眼镜必然侵犯隐私](https://simonwillison.net/2026/Jul/10/nilay-patel/#atom-everything) ⭐️ 7.0/10

尼莱·帕特尔指出，增强现实眼镜本质上需要持续摄像头录制和云端处理，使得隐私侵犯成为不可避免的代价。他认为社会成本可能过高，并质疑是否应该制造这类产品。 这一观点挑战了围绕 AR 眼镜的主流乐观叙事，聚焦于可能影响公共政策和消费者接受度的关键隐私困境。若被广泛接受，可能会减缓 AR 技术的投资和监管进程。 帕特尔声称，目前没有芯片能同时满足装在眼镜腿上所需的强大性能和低功耗，必须将数据发送到云端处理。替代方案如苹果 Vision Pro 需要外接电池组，体积庞大，并非理想中的轻量形态。

rss · Simon Willison · Jul 10, 17:05

**背景**: 增强现实（AR）眼镜通过头戴式显示器将数字信息叠加到现实世界中。为了实现这一点，摄像头必须实时捕捉用户的视野，而设备端处理需要强大且节能的芯片——帕特尔认为目前尚不存在这样的芯片。云端处理会引入延迟，并因持续传输视频流至远程服务器而带来隐私风险。

**标签**: `#augmented reality`, `#privacy`, `#technology ethics`, `#cloud computing`

---

<a id="item-8"></a>
## [sqlite-utils 4.1 新增自定义代码、类型覆盖和删除索引](https://github.com/simonw/sqlite-utils/releases/tag/4.1) ⭐️ 6.0/10

sqlite-utils 4.1 增加了 --code 选项用于内联 Python 行生成，--type 用于覆盖 CSV/TSV 的列类型，以及 drop-index 命令。还支持从标准输入读取查询和自动检测 upsert 的主键。 这些更新提高了数据操作任务的灵活性和便利性，特别是对于保留邮政编码前导零等边缘情况。新功能减少了对外部脚本的需求，简化了工作流程。 --code 选项可以接受一段 Python 代码或 .py 文件路径。--type 选项允许覆盖 CSV/TSV 列的自动检测类型。drop-index 命令支持 --ignore 以静默处理缺失的索引。transform 命令现在接受 --strict 和 --no-strict 来切换 SQLite 严格模式。

github · simonw · Jul 11, 23:50

**背景**: sqlite-utils 是一个 Python 库和命令行工具，用于创建和操作 SQLite 数据库。它提供了方便的插入、查询和转换数据的方法。SQLite 是一个轻量级、嵌入式的关系数据库引擎。此版本专注于增强 CLI 体验并更好地处理边缘情况。

**标签**: `#sqlite`, `#python`, `#cli`, `#database`

---

<a id="item-9"></a>
## [Ant：新 JavaScript 运行时与生态系统引发争议](https://antjs.org/) ⭐️ 6.0/10

Ant 是一个拥有自有 JavaScript 引擎的运行时，现已扩展为包含包管理器、注册表和桌面应用构建器的完整生态系统，该消息在 Hacker News 上发布。 Ant 试图提供 Node.js 和 Electron 等现有 JavaScript 栈的端到端替代方案，但社区对其原创性的质疑可能影响其采用。 该运行时使用名为 Silver VM 的自定义字节码虚拟机，但早期版本基于 AGPL 许可的 Elk JavaScript 引擎，作者后来自行重写了代码。项目托管在个人 GitHub 账户下，尽管作者宣称已成立公司。

hackernews · theMackabu · Jul 11, 20:07 · [社区讨论](https://news.ycombinator.com/item?id=48875377)

**背景**: JavaScript 运行时如 Node.js 和 Deno 在浏览器外执行 JavaScript。从头构建运行时需要实现 JavaScript 引擎，这非常复杂。Ant 声称拥有自有引擎，但最初版本基于 AGPL 许可的嵌入式 JS 引擎 Elk 构建。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/theMackabu/ant">theMackabu/ ant | DeepWiki</a></li>
<li><a href="https://news.ycombinator.com/item?id=48875377">Show HN: Ant – A JavaScript runtime and ecosystem | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 评论对'从头构建'的说法提出质疑，有用户指出 GitHub 问题显示原始代码依赖 Elk。其他人提到与 Apache Ant 的命名冲突，质疑独立开发者构建的经济可行性，并因公司招聘页面失效而指出信任问题。

**标签**: `#javascript`, `#runtime`, `#ecosystem`, `#web-development`, `#controversy`

---

<a id="item-10"></a>
## [免费平台教你从零重建 Redis、Git 和数据库](https://shipthatcode.com/) ⭐️ 6.0/10

新上线的免费平台 shipthatcode.com 通过引导式项目，教授用户如何从零重建 Redis、Git 和数据库。 它提供了像 CodeCrafters 这类付费资源的免费替代方案，让学习者通过从零构建核心基础设施来掌握系统编程，可能降低初学者的学习门槛。 该平台免费提供重建 Redis、Git 和数据库的课程，但社区反馈显示它与《Building Git》一书和 CodeCrafters 等现有资源相似，且部分用户在注册时遇到速率限制错误。

hackernews · acley · Jul 11, 13:40 · [社区讨论](https://news.ycombinator.com/item?id=48871973)

**背景**: 通过从零重建知名系统来学习是深入理解软件内部原理的流行方法。现有资源如 CodeCrafters（付费）和《Building Git》（书籍）提供类似内容。该平台旨在免费提供此类学习，但其原创性以及是否使用了 AI 生成内容受到质疑。

**社区讨论**: 社区评论褒贬不一：有人赞赏免费访问，但其他人质疑其原创性并怀疑内容由 AI 生成。还有关于增加 Zig 支持的提问，以及用户报告了注册错误。

**标签**: `#learning`, `#redis`, `#git`, `#database`, `#open source`

---