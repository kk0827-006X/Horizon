---
layout: default
title: "Horizon Summary: 2026-05-12 (ZH)"
date: 2026-05-12
lang: zh
---

> From 31 items, 16 important content pieces were selected

---

1. [加州大学洛杉矶分校宣布首款修复中风脑损伤的药物](#item-1) ⭐️ 10.0/10
2. [TanStack NPM 供应链攻击事后分析](#item-2) ⭐️ 9.0/10
3. [纽约时报更正 AI 生成的虚假引用](#item-3) ⭐️ 9.0/10
4. [学习软件架构的反思文章](#item-4) ⭐️ 8.0/10
5. [欧盟拟打击 TikTok 和 Instagram 针对儿童的成瘾设计](#item-5) ⭐️ 8.0/10
6. [AI 写作催生“僵尸互联网”，杰森·科布勒指出](#item-6) ⭐️ 8.0/10
7. [Shopify 的 River AI 助手在 Slack 上公开促进学习](#item-7) ⭐️ 8.0/10
8. [如果 AI 写代码，为何还要用 Python？](#item-8) ⭐️ 7.0/10
9. [极低频通信：潜艇联络的历史与技术](#item-9) ⭐️ 7.0/10
10. [Anthropic 在 AWS 上推出 Claude 平台](#item-10) ⭐️ 7.0/10
11. [开发者用 AI 自制睡眠追踪工具](#item-11) ⭐️ 7.0/10
12. [GitLab 的“第二幕”：裁员与组织重组](#item-12) ⭐️ 7.0/10
13. [AI 编程代理必须降低维护成本以避免长期负担](#item-13) ⭐️ 7.0/10
14. [老桌面操作系统截图怀旧合集](#item-14) ⭐️ 6.0/10
15. [软件内部原理读书会](#item-15) ⭐️ 6.0/10
16. [在脚本 shebang 行中使用 LLM](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [加州大学洛杉矶分校宣布首款修复中风脑损伤的药物](https://stemcell.ucla.edu/news/ucla-discovers-first-stroke-rehabilitation-drug-repair-brain-damage) ⭐️ 10.0/10

加州大学洛杉矶分校的研究人员发现了首款能够修复中风引起的脑损伤的药物，该药物针对幸存神经网络的连接中断而非细胞死亡本身。 这一突破可能通过提供药物干预来恢复丧失的脑功能，从而彻底改变中风康复治疗，可能影响全球数百万中风幸存者。 该药物针对受“瘀伤”的脑细胞，重新建立远端网络的节律性活动，但无法恢复发生细胞死亡的梗死核心区域的功能。

hackernews · bookofjoe · May 11, 17:53 · [社区讨论](https://news.ycombinator.com/item?id=48098261)

**背景**: 中风是由于大脑部分供血中断导致脑细胞死亡。此前，没有药物能够修复由此产生的脑损伤；康复依赖于大脑的自然可塑性和治疗。加州大学洛杉矶分校的药物代表了一种新方法，专注于挽救受“瘀伤”的细胞并重新连接神经回路。

**社区讨论**: 评论者指出中风会导致细胞死亡，但受“瘀伤”的细胞可以恢复，该药物针对的是连接中断而非直接修复细胞。一位用户提供了该化合物的 PubMed 链接（https://pubmed.ncbi.nlm.nih.gov/39106304/），另一位用户询问它是否对阿尔茨海默病有效。

**标签**: `#stroke`, `#brain damage`, `#drug discovery`, `#neuroscience`, `#rehabilitation`

---

<a id="item-2"></a>
## [TanStack NPM 供应链攻击事后分析](https://tanstack.com/blog/npm-supply-chain-compromise-postmortem) ⭐️ 9.0/10

TanStack 发布了一份事后分析报告，详细说明了攻击者如何利用 CI 管道漏洞，通过窃取的 GitHub 令牌并安装一个致命开关（dead-man's switch），一旦令牌被撤销就会擦除用户主目录。 此事件凸显了供应链安全的关键弱点，特别是 CI 管道权限相关的风险以及 Trusted Publishing 的局限性。它引发了社区关于保护 CI 管道的广泛讨论，并促使开发者重新审视其发布工作流。 攻击安装了一个 systemd 用户服务（Linux）或 LaunchAgent（macOS），每 60 秒用窃取的令牌轮询 api.github.com/user；如果令牌返回 4xx 错误，就会执行`rm -rf ~/`。此外，@mistralai/mistralai npm 包也作为同一蠕虫的一部分被入侵。

hackernews · varunsharma07 · May 11, 21:08 · [社区讨论](https://news.ycombinator.com/item?id=48100706)

**背景**: 对 npm 等包注册表的供应链攻击利用 CI/CD 管道中的漏洞注入恶意代码。致命开关（dead-man's switch）是一种机制，当满足某个条件（如令牌撤销）时触发破坏性操作。Trusted Publishing 使用 OIDC 来认证发布者，无需静态令牌，但它不能完全防止 CI 被攻破。CI 管道漏洞（如中毒管道执行）可能让攻击者获取机密信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fail-safe">Fail-safe - Wikipedia</a></li>
<li><a href="https://docs.npmjs.com/trusted-publishers/">Trusted publishing for npm packages | npm Docs</a></li>
<li><a href="https://circleci.com/blog/is-my-pipeline-vulnerable/">Is my CI pipeline vulnerable ? - CircleCI</a></li>

</ul>
</details>

**社区讨论**: 评论者对致命开关表示担忧，用户 cube00 警告了其在令牌撤销时的行为。其他人则讨论了 Trusted Publishing 的安全性，jonchurch_认为如果 CI 被攻破，它是不够的。讨论还涉及了 CI YAML 配置的复杂性以及在部署恶意更改前需要冷却期。

**标签**: `#supply-chain`, `#security`, `#npm`, `#CI/CD`, `#postmortem`

---

<a id="item-3"></a>
## [纽约时报更正 AI 生成的虚假引用](https://simonwillison.net/2026/May/10/new-york-times-editors-note/#atom-everything) ⭐️ 9.0/10

《纽约时报》发布编者按，承认之前文章中引用的加拿大保守党领袖皮埃尔·波利耶夫的言论实际上是 AI 生成的摘要，而非直接引语。记者未能核实 AI 工具的返回结果。 这一事件凸显了在新闻业中未经适当验证就使用生成式 AI 的危险性，因为 AI 可能产生听起来合理但实际是伪造的引语。它强调了对 AI 在新闻编辑室的使用进行严格事实核查和制定道德准则的必要性。 编者按说明，文章现已准确引用波利耶夫在 4 月的一次演讲内容，且他在那次演讲中并未将改变立场的政客称为“叛徒”。原文是关于加拿大选举的报道。

rss · Simon Willison · May 10, 23:58

**背景**: AI 幻觉指的是大型语言模型自信地产生虚假或捏造信息的情况。在新闻业中，记者有时会使用 AI 工具来总结或生成文本，但这些工具可能会编造引语或事实。这一案例是主流报纸中此类失败的显著例子。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)">Hallucination (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.evidentlyai.com/blog/ai-hallucinations-examples">8 AI hallucinations examples</a></li>

</ul>
</details>

**标签**: `#ai-ethics`, `#hallucinations`, `#generative-ai`, `#journalism`

---

<a id="item-4"></a>
## [学习软件架构的反思文章](https://matklad.github.io/2026/05/12/software-architecture.html) ⭐️ 8.0/10

一篇关于学习软件架构的反思文章，融合了实用原则、哲学视角和经典参考文献，并通过富有洞察力的社区评论加以丰富。 这篇文章及其社区讨论为寻求加深对软件架构理解的软件工程师提供了丰富的资源，既提供了实用启发，又蕴含哲学深度。它强调了永恒的原则和经典文本，尽管技术不断演进，这些内容仍具有现实意义。 社区评论包括设计原则速查表（如减少意外、隔离数据转换）、与中国儒家和道家学习哲学的对比，以及经典架构书籍推荐，如 Ousterhout 的《软件设计哲学》和 Shaw/Garlan 的《软件架构：新兴学科视角》。还有评论将软件架构比作管道，强调它必须服务于更大的系统。

hackernews · surprisetalk · May 12, 09:30 · [社区讨论](https://news.ycombinator.com/item?id=48106024)

**背景**: 软件架构指软件系统的高层结构，定义其组件、相互关系及设计原则。关键的现代方法包括领域驱动设计（DDD），强调建模软件以匹配业务领域；以及整洁架构，强调关注点分离和层独立性。事件溯源是另一种模式，将状态变更记录为不可变事件，常用于复杂领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Domain-driven_design">Domain-driven design</a></li>
<li><a href="https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html">The Clean Architecture by Uncle Bob - The Clean Code Blog</a></li>
<li><a href="https://martinfowler.com/eaaDev/EventSourcing.html">Event Sourcing</a></li>

</ul>
</details>

**社区讨论**: 社区评论非常有建设性，分享了实用原则（如“减少意外”、“耦合是万恶之源”）并推荐了基础读物。一条评论将学习过程比作儒家修身和道家简约，另一条则指出文章的建议可能更偏向通用软件开发而非特定架构。总体情绪积极且充满赞赏。

**标签**: `#software architecture`, `#learning`, `#design principles`, `#philosophy of software`

---

<a id="item-5"></a>
## [欧盟拟打击 TikTok 和 Instagram 针对儿童的成瘾设计](https://www.cnbc.com/2026/05/12/tiktok-instagram-social-media-addictive-eu-crack-down.html) ⭐️ 8.0/10

欧盟委员会建议 TikTok 和 Instagram 修改其平台，消除针对儿童的成瘾设计功能，指出其违反了《数字服务法》。 这项法规可能为社交媒体平台如何对算法成瘾（尤其是对未成年人）负责树立先例，并可能影响全球政策。它标志着将成瘾设计视为与烟草类似公共健康问题的转变。 《数字服务法》第 25 条针对欺骗或操纵用户的在线界面设计，欧盟特别关注无限滚动、个性化推荐以及利用儿童脆弱性的通知系统。这些建议不具有约束力，但具有重大的政治分量。

hackernews · thm · May 12, 11:00 · [社区讨论](https://news.ycombinator.com/item?id=48106534)

**背景**: 《数字服务法》是欧盟一项全面的法规，要求数字平台承担处理非法内容、虚假信息和系统性风险的义务。成瘾设计指利用心理机制最大化用户参与度的功能，如无限滚动、自动播放和算法推送，通常以损害心理健康为代价。欧盟此前已根据该法对主要平台采取行动，包括对 TikTok 启动正式程序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.europeaninterest.eu/eu-accuses-tiktok-of-addictive-design-that-harms-children-in-breach-of-the-digital-services-act/">EU accuses TikTok of ' addictive design ' that harms children in breach....</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/policies/digital-services-act">The Digital Services Act | Shaping Europe ’s digital future</a></li>

</ul>
</details>

**社区讨论**: 评论者大多支持欧盟的行动，许多人将算法成瘾比作香烟，并指出这个问题影响所有年龄段，而不仅仅是儿童。一些人提出了算法拦截器等技术解决方案，而另一些人则质疑为什么相同的保护措施不适用于成年人。大家一致认为无限滚动和推荐算法有害，应予以监管。

**标签**: `#social media`, `#regulation`, `#addiction`, `#technology policy`, `#algorithms`

---

<a id="item-6"></a>
## [AI 写作催生“僵尸互联网”，杰森·科布勒指出](https://simonwillison.net/2026/May/11/zombie-internet/#atom-everything) ⭐️ 8.0/10

杰森·科布勒发表了一篇题为《你的 AI 使用正在摧毁我的大脑》的文章，提出了“僵尸互联网”这一术语，用以描述在线无处不在且令人精神疲惫的 AI 生成内容。 这篇评论强调了互联网用户因需要持续过滤 AI 生成内容而承受的精神负担，并通过强调人与 AI 互动的纠缠关系，完善了“死互联网”理论。 科布勒将“僵尸互联网”与“死互联网”区分开来，指出前者涉及人类与机器人互动、人类使用 AI 与其他人类交流，以及为了盈利而生成的 AI 垃圾内容，而非仅仅是机器人与机器人对话。

rss · Simon Willison · May 11, 19:21

**背景**: “死互联网”理论推测大多数在线流量来自机器人，人类活动很少。科布勒的“僵尸互联网”在此基础上进行了扩展，描述了 AI 生成内容无处不在、难以与人类创作的内容区分的状态，导致精神疲惫并扭曲了人类的写作风格。

**标签**: `#AI`, `#internet culture`, `#content quality`, `#zombie internet`, `#ethics`

---

<a id="item-7"></a>
## [Shopify 的 River AI 助手在 Slack 上公开促进学习](https://simonwillison.net/2026/May/11/learning-on-the-shop-floor/#atom-everything) ⭐️ 8.0/10

Shopify CEO Tobias Lütke 宣布，其内部 AI 编码助手 River 仅在公共 Slack 频道中运作，拒绝私信，鼓励开放协作。这种方法将每次编码会话变成所有员工均可搜索、透明的学习机会。 通过公开 AI 交互，Shopify 创造了‘渗透学习’环境，开发者通过观察他人与 AI 协作来学习，可能加速整个组织的技能发展。这种模式挑战了典型的私有 AI 助手部署方式，可能影响其他公司整合 AI 工具的方式。 River 不回复私信，而是提示用户创建公共频道；CEO Lütke 的频道#tobi_river 有超过 100 人关注，他们做出反应、补充背景并帮助审查。公司将其描述为‘Lehrwerkstatt’（教学工场），工作的可见性使得无需正式课程即可学习。

rss · Simon Willison · May 11, 15:46

**背景**: AI 编码助手是基于大型语言模型（LLM）的工具，帮助开发者编写、理解和调试代码。通常，这些助手在私有环境中运行，个人对话与同事隔离。Shopify 的 River 方法使得所有交互在公司 Slack 内公开且可搜索，类似于 Midjourney 通过公共 Discord 频道成功的透明度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://habr.com/ru/articles/875816/">Внедряем AI Code Assistant в разработку бесплатно и без... / Хабр</a></li>

</ul>
</details>

**标签**: `#AI coding assistant`, `#software engineering`, `#transparent AI`, `#Shopify`, `#learning`

---

<a id="item-8"></a>
## [如果 AI 写代码，为何还要用 Python？](https://medium.com/@NMitchem/if-ai-writes-your-code-why-use-python-bf8c4ba1a055) ⭐️ 7.0/10

文章讨论了在 AI 生成代码的背景下，考虑到可读性、训练数据量和静态类型等因素，Python 是否仍然是最优的编程语言。 这一讨论至关重要，因为它影响开发者如何选择语言以最大化 AI 辅助效率，可能推动软件开发实践向更严格的静态类型或熟悉的生态系统转变。 文章强调 Python 的极端可读性和大量训练数据是其优势，但也指出像 Rust 这样的静态类型语言由于反馈循环更短，在智能体工作流中可能表现更好。

hackernews · indigodaddy · May 11, 20:45 · [社区讨论](https://news.ycombinator.com/item?id=48100433)

**背景**: Python 因其简洁性和丰富的库在 AI 和机器学习领域被广泛使用。在 AI 代码生成中，语言选择还取决于大型语言模型生成代码的质量以及人类审查的便利性。静态类型在编译时强制类型约束，减少运行时错误，而 Python 这样的动态类型则提供更多灵活性。

**社区讨论**: 评论者意见分歧：一些人认为 Python 的可读性和训练数据量是关键优势，而另一些人则主张像 Rust 这样的静态类型语言能提高智能体的可靠性。还有评论者纠正了文章关于 Nicholas Carlini 项目的事实性错误。

**标签**: `#AI code generation`, `#Python`, `#programming languages`, `#static typing`, `#software development`

---

<a id="item-9"></a>
## [极低频通信：潜艇联络的历史与技术](https://computer.rip/2026-05-09-extremely-low-frequencies.html) ⭐️ 7.0/10

这篇文章深入探讨了用于潜艇联络的极低频（ELF）无线电通信的历史和技术，涵盖了早期的意外发现和现代军事系统。 极低频通信对军用潜艇至关重要，因为它能让深潜潜艇在不浮出水面的情况下接收信号，确保战略任务中的隐蔽性和作战安全。 极低频系统工作在约 30–100 Hz 的频率上，数据速率极低（每分钟几个比特），但其信号能穿透数百米深的海水，只需几个发射机就能实现全球覆盖。

hackernews · pinewurst · May 12, 03:59 · [社区讨论](https://news.ycombinator.com/item?id=48104041)

**背景**: 极低频（ELF）无线电波占用 3–300 Hz 频段，在海水中衰减极低，因此非常适合与深潜潜艇进行单向通信。与要求潜艇接近海面的较高频段甚低频（VLF）波不同，极低频波能在潜艇作战深度到达它们，尽管数据速率非常慢。像美国海军的“桑吉恩计划”和克拉姆湖设施等项目就是利用这项技术建造的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Extremely_low_frequency">Extremely low frequency - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Project_Sanguine">Project Sanguine - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论包括关于一位祖父很可能在 20 世纪 50–60 年代参与机密极低频实验的个人轶事，对历史叙述的赞赏，以及指向甚低频和水声通信额外资源的链接。总体情绪是积极和补充性的。

**标签**: `#ELF`, `#submarine communication`, `#radio technology`, `#history`, `#military`

---

<a id="item-10"></a>
## [Anthropic 在 AWS 上推出 Claude 平台](https://claude.com/blog/claude-platform-on-aws) ⭐️ 7.0/10

Anthropic 在 AWS 上推出了 Claude 平台，提供原生的 Claude API 功能，数据处理在 AWS 边界之外进行，并支持自定义代理托管和 MCP 服务器集成。 此举使企业能够在其 AWS 基础设施中利用 Claude 的能力，同时提供托管代理服务，可能简化 AI 代理的部署和与现有工作流的集成。 与也提供 Claude 模型的 AWS Bedrock 不同，AWS 上的 Claude 平台由 Anthropic 直接运营，数据在 AWS 边界之外处理。它支持自定义代理托管和 MCP 服务器集成，允许用户构建和部署带有自定义工具的代理。

hackernews · matrixhelix · May 12, 01:24 · [社区讨论](https://news.ycombinator.com/item?id=48103042)

**背景**: AWS Bedrock 是一项托管服务，提供来自包括 Anthropic 的 Claude 在内的多个供应商的基础模型。新的 AWS 上的 Claude 平台是 Anthropic 直接管理服务的独立产品，为代理定制提供了更多灵活性。MCP（模型上下文协议）是一种将 AI 模型与外部工具和服务器集成的协议。

**社区讨论**: 评论者对“在 AWS 上”的命名感到困惑，因为数据在 AWS 边界之外处理，但他们认识到托管代理和 MCP 集成的价值。一些人希望支持 Azure，而另一些人则将其与 AWS Bedrock 比较，并质疑额外的优势。

**标签**: `#AWS`, `#Claude`, `#Anthropic`, `#AI platform`, `#cloud computing`

---

<a id="item-11"></a>
## [开发者用 AI 自制睡眠追踪工具](https://martin.sh/i-let-ai-build-a-tool-to-help-me-figure-out-what-was-waking-me-up-at-night/) ⭐️ 7.0/10

一位开发者利用 AI 分析传感器数据，构建个人工具以识别夜间醒来的原因，如噪音或二氧化碳浓度。 该项目展示了 AI 如何帮助个人用低成本的自制方案解决健康问题，激励他人探索类似方法。 该工具可能整合麦克风和 CO2 监测器等传感器数据，用 AI 关联事件与醒来记录；开发者在博客上分享了项目并获得社区反馈。

hackernews · showmypost · May 11, 21:04 · [社区讨论](https://news.ycombinator.com/item?id=48100662)

**背景**: 睡眠追踪通常使用可穿戴设备或 App，但定制方案能精确关联环境因素。卧室 CO2 浓度可能超标，影响睡眠质量。AI 可自动化分析多数据流。

**社区讨论**: 评论强调了耳塞和 CO2 监测等睡眠卫生建议，有人分享了类似的 DIY 睡眠追踪项目，并指出 CO2 浓度过高的问题。

**标签**: `#AI`, `#sleep tracking`, `#personal project`, `#sensors`

---

<a id="item-12"></a>
## [GitLab 的“第二幕”：裁员与组织重组](https://simonwillison.net/2026/May/11/gitlab-act-2/#atom-everything) ⭐️ 7.0/10

此次重组反映了科技公司如何适应人工智能驱动软件开发的“代理时代”，可能为远程优先的组织树立先例。在价值观中不再明确提及多样性可能会引发关于企业优先级的讨论。 该计划包括将小型团队所在国家数量减少最多 30%（从近 60 个国家减少），在某些职能部门移除最多三层管理，并将独立研发团队数量几乎翻倍。GitLab 还将用“质量的速度、主人翁精神、客户成果”取代其 CREDIT 价值观。

rss · Simon Willison · May 11, 23:58

**背景**: GitLab 是一个以全远程团队著称的 DevOps 平台，业务覆盖近 60 个国家。“代理时代”指的是人工智能代理在软件开发中的日益普及，GitLab 认为这将倍增软件需求。此次重组旨在为公司适应这一转变做好准备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://about.gitlab.com/blog/gitlab-act-2/">GitLab Act 2</a></li>
<li><a href="https://www.investing.com/news/stock-market-news/gitlab-announces-restructuring-plan-shares-slide-4678673">GitLab announces restructuring plan, shares slide By Investing.com</a></li>

</ul>
</details>

**标签**: `#GitLab`, `#remote work`, `#workforce reduction`, `#strategy`, `#tech industry`

---

<a id="item-13"></a>
## [AI 编程代理必须降低维护成本以避免长期负担](https://simonwillison.net/2026/May/11/james-shore/#atom-everything) ⭐️ 7.0/10

James Shore 提出，AI 编程代理必须按比例降低维护成本以匹配生产力提升，否则将变成长期负担。 这一见解凸显了 AI 辅助编程中一个常被忽视的关键权衡，将影响开发者工作流和软件经济学。 Shore 的数学推导显示，如果编码速度翻倍但维护成本不变，总维护成本仍将翻倍；因此 AI 必须成反比地降低维护成本。

rss · Simon Willison · May 11, 19:48

**背景**: 软件维护成本常常超过初始开发成本。AI 编程代理提高了代码生成速度，但若管理不当，可能会增加技术债务和长期维护负担。

**标签**: `#AI`, `#software engineering`, `#maintenance`, `#productivity`

---

<a id="item-14"></a>
## [老桌面操作系统截图怀旧合集](http://www.typewritten.org/Media/) ⭐️ 6.0/10

typewritten.org/Media 网站精心整理了老式桌面操作系统的截图，引发了社区关于用户界面演变的讨论。 该合集作为用户界面设计的视觉历史，提醒用户那些已消失的易用性，并引发对现代界面复杂性的讨论。 该合集注重广度，涵盖了许多系统如 BeOS、NeXTSTEP 和 Amiga Workbench，但一些评论者指出缺少早期 Linux 桌面等。

hackernews · adunk · May 12, 05:11 · [社区讨论](https://news.ycombinator.com/item?id=48104428)

**背景**: typewritten.org/Media 网站汇集了已过时的桌面环境截图，从早期的 Mac OS 和 Windows 到小众系统如 BeOS、NeXTSTEP 和 Amiga Workbench。这些操作系统各有独特的视觉语言，专为不同的硬件设计。该合集为复古计算爱好者提供了数字博物馆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BeOS">BeOS - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/NeXTSTEP">NeXTSTEP - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amiga_Workbench">Amiga Workbench</a></li>

</ul>
</details>

**社区讨论**: 评论者哀叹像可见滚动条和可调整窗格等可发现 UI 元素的消失。有人希望现代操作系统提供复古模式，还有人分享了类似合集的链接以覆盖更广。

**标签**: `#retro computing`, `#UI design`, `#desktop environments`, `#nostalgia`

---

<a id="item-15"></a>
## [软件内部原理读书会](https://eatonphil.com/bookclub.html) ⭐️ 6.0/10

一篇博客文章介绍了一个软件内部原理读书会，提供了阅读清单和讨论形式，但参与需要 LinkedIn 账户，这引发了不同的反馈。 该读书会为工程师提供了一种通过精选阅读来深入理解系统内部原理的结构化方式，但 LinkedIn 要求可能限制参与和可及性。 阅读清单包括 Tanenbaum 的操作系统等知名书籍，讨论形式涉及一个大型群组，通常只有 1-2%的活跃参与者。

hackernews · aragonite · May 12, 02:28 · [社区讨论](https://news.ycombinator.com/item?id=48103511)

**背景**: 软件内部原理指操作系统、编译器、数据库等系统的内部工作机制。读书会通过社区讨论和共同阅读，帮助工程师系统性地学习这些复杂主题。

**社区讨论**: 评论中对阅读清单表示赞赏，但一些用户对 LinkedIn 要求和电子邮件验证问题提出异议。此外，还提到了一篇关于如何运行读书会的相关文章。

**标签**: `#software engineering`, `#book club`, `#systems internals`, `#reading list`

---

<a id="item-16"></a>
## [在脚本 shebang 行中使用 LLM](https://simonwillison.net/2026/May/11/llm-shebang/#atom-everything) ⭐️ 6.0/10

Simon Willison 演示了如何在 shebang 行中使用 LLM 命令行工具，将纯英文文本文件作为脚本执行，通过 LLM 生成输出，包括工具调用和带有自定义 Python 函数的 YAML 模板。 这项技术模糊了自然语言与可执行代码之间的界限，使得用户可以编写提示词作为可直接执行的脚本，开销极低，从而带来新颖的工作流程。 shebang 使用 `#!/usr/bin/env -S llm -f` 进入片段模式，`-T name_of_tool` 进行工具调用，以及 `-t` 用于 YAML 模板，直接在脚本中定义额外的 Python 函数作为工具。

rss · Simon Willison · May 11, 18:48

**背景**: Simon Willison 开发的 LLM 命令行工具是一个多功能的 CLI，用于通过 API 或本地模型与各种大型语言模型交互。Shebang 行（#!/usr/bin/env）允许脚本指定解释器，而 LLM 片段功能可将文件内容作为提示的上下文传递。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the command-line · GitHub</a></li>
<li><a href="https://llm.datasette.io/en/stable/fragments.html">Fragments - LLM - Datasette</a></li>
<li><a href="https://news.ycombinator.com/item?id=40782755">Language models on the command line | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 在 Hacker News 上，Kim_Bruning 评论说，现在可以在英文文本文件上放置 shebang 行，“如果你足够勇敢”，这突显了这一技巧的新颖但可能不稳定的性质。

**标签**: `#llm`, `#command-line`, `#scripting`, `#shebang`, `#generative-ai`

---