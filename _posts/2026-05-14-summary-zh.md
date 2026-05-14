---
layout: default
title: "Horizon Summary: 2026-05-14 (ZH)"
date: 2026-05-14
lang: zh
---

> From 37 items, 11 important content pieces were selected

---

1. [软件 Emacs 化：用户用 LLM 构建个人工具](#item-1) ⭐️ 8.0/10
2. [双胞胎兄弟被解雇后删除 96 个政府数据库](#item-2) ⭐️ 8.0/10
3. [美国在 AI 商业化领先，但盈利和开源挑战并存](#item-3) ⭐️ 8.0/10
4. [Cerebras IPO 定价 185 美元，筹资 55.5 亿美元](#item-4) ⭐️ 8.0/10
5. [免费 *.city.state.us 地方域名设置指南](#item-5) ⭐️ 7.0/10
6. [普林斯顿结束 133 年荣誉制度，强制监考](#item-6) ⭐️ 7.0/10
7. [CSP 允许列表实验](#item-7) ⭐️ 7.0/10
8. [英伟达 CEO 基金会向研究人员捐赠 1.08 亿美元 AI 算力](#item-8) ⭐️ 7.0/10
9. [对模糊的“11 个 AI 代理”术语的批评](#item-9) ⭐️ 6.0/10
10. [米切尔·桥本批评风险规避的技术决策者](#item-10) ⭐️ 6.0/10
11. [LLM 0.32a2 新增对 OpenAI 推理端点的支持](#item-11) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [软件 Emacs 化：用户用 LLM 构建个人工具](https://sockpuppet.org/blog/2026/05/12/emacsification/) ⭐️ 8.0/10

一篇题为《软件 Emacs 化》的博客文章认为，LLM 使个人能够创建可定制的软件工具，类似于 Emacs 的定制精神。Hacker News 上的讨论高度参与，tptacek 等知名人士的贡献反映了重新掌控软件的重要趋势。 这一趋势标志着从预打包软件向个人定制解决方案的转变，可能使软件创建民主化，减少对专业产品的依赖。这对开发者、高级用户和整个软件行业都意义重大，因为它挑战了商业软件的统治地位。 文章指出，播客应用、笔记应用和食谱管理器等软件现在可以通过从 Claude 获得优于替代品质量的结果来取代。但一些评论者指出个人设置的脆弱性和跨平台一致性的挑战，这呼应了 Emacs 定制的缺点。

hackernews · rdslw · May 13, 07:06 · [社区讨论](https://news.ycombinator.com/item?id=48118727)

**背景**: Emacs 是一个高度可扩展和可定制的文本编辑器，有着悠久的历史，用户经常编写大量配置文件（.emacs 文件）来定制编辑器。'Emacs 化'指的是软件变得个性化和可黑客化的模式。像 Claude 这样的 LLM（大型语言模型）能快速原型化和生成代码，使非专业人员更容易创建定制软件。

**社区讨论**: 评论者普遍同意这一趋势，dang 分享说软件生产现在足够容易实现个性化。tptacek 列出了个人工具可以重新占领的具体领域。但像 shaokind 这样的人指出个人设置的脆弱性和跨平台一致性的噩梦，这呼应了经典的 Emacs 痛点。

**标签**: `#software engineering`, `#customization`, `#LLMs`, `#personal software`, `#Emacs`

---

<a id="item-2"></a>
## [双胞胎兄弟被解雇后删除 96 个政府数据库](https://arstechnica.com/tech-policy/2026/05/drop-database-what-not-to-do-after-losing-an-it-job/) ⭐️ 8.0/10

双胞胎兄弟 Sohaib 和 Usman 在被政府承包商 Opexus 解雇几分钟后，据称使用命令 'DROP DATABASE' 删除了 96 个政府数据库。 此事件凸显了特权访问管理和内部威胁检测的关键弱点，尤其是针对敏感政府系统，可能促使更严格的安全协议和背景调查。 据称，这对双胞胎删除了包括 DHS 生产数据库在内的数据库，其中一人甚至在删除后搜索如何清除 SQL 服务器日志。他们曾有犯罪记录，引发了对招聘实践的质疑。

hackernews · jnord · May 12, 22:28 · [社区讨论](https://news.ycombinator.com/item?id=48115438)

**背景**: 内部威胁是指源于组织内部的安全风险，通常涉及拥有合法访问权限的员工滥用权限。特权访问管理（PAM）强制实施最小权限访问和按需提升，以减少滥用造成的损害。数据库中的审计跟踪可以记录更改，有助于事后调查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.beyondtrust.com/resources/glossary/privileged-access-management-pam">What is Privileged Access Management (PAM)? | BeyondTrust</a></li>
<li><a href="https://learn.microsoft.com/en-us/answers/questions/1661238/audit-trail-of-insert-update-and-delete">Audit trail of Insert, Update and Delete - Microsoft Q&A</a></li>
<li><a href="https://expertinsights.com/data-security-and-privacy/the-top-insider-threat-detection-solutions">Best 5 Insider Threat Detection Solutions For Enterprise (2026)</a></li>

</ul>
</details>

**社区讨论**: 评论者对这一故事表示怀疑，质疑双胞胎如何能访问如此敏感的系统，并指出情况的荒谬性，一些人认为当局可能对细节进行了处理。

**标签**: `#cybersecurity`, `#insider threat`, `#database`, `#government`, `#access control`

---

<a id="item-3"></a>
## [美国在 AI 商业化领先，但盈利和开源挑战并存](https://avkcode.github.io/blog/us-winning-ai-race.html) ⭐️ 8.0/10

一篇文章认为美国在 AI 商业化竞赛中领先，以 OpenAI、Anthropic 和谷歌等领先公司为例。 这一讨论凸显了美中 AI 竞争，并质疑商业化主导地位能否确保长期成功，因为存在盈利问题和开源竞争。 社区评论指出，美国 AI 公司尚未盈利，中国模型免费且可在消费级硬件上运行，而竞争可能有利于提供高效本地模型的一方。

hackernews · akrylov · May 13, 13:53 · [社区讨论](https://news.ycombinator.com/item?id=48121929)

**背景**: 中美之间的 AI 竞赛不仅涉及模型性能，还包括商业化、盈利能力和地缘政治影响。中国的开源模型（如 DeepSeek）通过以更低成本提供有竞争力的性能挑战了美国的主导地位。

**社区讨论**: 评论者表示怀疑：有人说美国公司正在亏损，中国模型快速追赶，真正的赢家可能是拥有最佳本地模型性能的一方。其他人指出地缘政治信任问题和美国政策可能削弱美国的领导地位。

**标签**: `#AI`, `#US-China competition`, `#commercialization`, `#AI models`, `#geopolitics`

---

<a id="item-4"></a>
## [Cerebras IPO 定价 185 美元，筹资 55.5 亿美元](https://www.investing.com/news/stock-market-news/cerebras-prices-ipo-at-185-per-share-to-raise-555-billion-sources-say-4686852) ⭐️ 8.0/10

Cerebras Systems 将其首次公开募股（IPO）定价为每股 185 美元，筹集约 55.5 亿美元。这使得这家 AI 芯片公司的市值约为 80 亿美元。 此次 IPO 对 Cerebras 来说是重要里程碑，该公司以独特晶圆级处理器闻名，是 AI 硬件市场的关键参与者。成功定价表明投资者对 GPU 之外专用 AI 芯片需求的强烈信心。 IPO 定价处于预期区间的高端。Cerebras 计划将收益用于研发、扩大销售和营销活动以及一般公司用途。

rss · Investing.com All News · May 14, 00:00

**背景**: Cerebras 以其晶圆级引擎（WSE）闻名，这是世界上最大的 AI 处理器。2024 年 3 月推出的 WSE-3 拥有 90 万个核心，性能是上一代的两倍，旨在以更低功耗训练大规模深度学习模型，相比 GPU 更有优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>

</ul>
</details>

**标签**: `#IPO`, `#AI hardware`, `#Cerebras`, `#semiconductor`, `#funding`

---

<a id="item-5"></a>
## [免费 *.city.state.us 地方域名设置指南](https://fredchan.org/blog/locality-domains-guide/) ⭐️ 7.0/10

2025 年发布的一份详尽指南解释了如何获取 .us 顶级域下的免费地方域名，具体格式为 city.state.us。该指南详细介绍了寻找授权地方管理商并免费注册域名的过程。 这份指南对于寻求无需年费的、具有本地特色的域名个人和小型组织非常有价值。它揭示了历史上使这类域名难以获得的官僚和技术障碍，社区讨论也证实了这一点。 地方域名要求注册人与授权管理商签订合同，一些管理商已倒闭，需要坚持寻找或选择替代注册方式。指南指出，.us 域名禁止 WHOIS 隐私服务，这对个人使用构成隐私风险。

hackernews · speckx · May 13, 14:45 · [社区讨论](https://news.ycombinator.com/item?id=48122635)

**背景**: .us 顶级域最初只允许第四级注册，格式为 organization-name.locality.state.us，基于 RFC 1480 定义的政治地理结构。2002 年引入了二级注册，但地方域名作为特殊结构仍然存在，由每个城市/州组合的授权管理商管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.about.us/locality-structure">usTLD Locality-Based Structure - US domain name</a></li>
<li><a href="https://en.wikipedia.org/wiki/.us">.us - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区成员报告了重大挑战：一位用户拥有三个域名，但其中一个注册商三年前已倒闭，需要联系其遗孀。另一位尝试注册波士顿域名，但被要求提供市政府公证信函，这几乎不可能办到。还有用户指出有 7388 个域名可通过在线注册获得，但服务器因关注度过载。

**标签**: `#dns`, `#domains`, `#locality`, `#how-to`, `#hackernews`

---

<a id="item-6"></a>
## [普林斯顿结束 133 年荣誉制度，强制监考](https://www.dailyprincetonian.com/article/2026/05/princeton-news-adpol-proctoring-in-person-examinations-passed-faculty-133-years-precedent) ⭐️ 7.0/10

普林斯顿大学教师投票决定，所有线下考试必须进行监考，结束了长达 133 年依赖学生自我监督、没有监考人员的荣誉制度传统。 这所顶尖大学的政策转变反映了对 AI 作弊日益增长的担忧，并预示着高等教育中基于信任的荣誉制度正走向衰落。 该决定推翻了 133 年的先例，此前一项调查发现，29.9%的受访者承认作弊，44.6%的高年级学生知道有未报告的违规行为。监考人员将向学生管理的荣誉委员会报告事件。

hackernews · bookofjoe · May 13, 20:12 · [社区讨论](https://news.ycombinator.com/item?id=48126848)

**背景**: 普林斯顿的荣誉制度成立于 1893 年，允许学生基于相互信任在没有监考的情况下参加考试。生成式 AI 工具（如 ChatGPT）的兴起使作弊更容易且更难被发现，促使许多机构重新考虑其政策。荣誉制度依赖学生举报违规行为，但许多人选择不报告。

**社区讨论**: 评论者反应不一：有人认为此举反映了社会从高信任向低信任文化的转变，而另一些人指出无监考考试并不常见，监考在其他地方很普遍。一些人分享了个人经历的作弊事件，并支持积极监考和没收设备。

**标签**: `#ethics`, `#education`, `#AI`, `#trust`, `#cheating`

---

<a id="item-7"></a>
## [CSP 允许列表实验](https://simonwillison.net/2026/May/13/csp-allow/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了一个交互式工具，演示了在受 CSP 保护的沙箱化 iframe 中，通过拦截 CSP 错误动态允许列表 fetch 来源的方法。 该技术实现了用户驱动的动态 CSP 允许列表，同时不降低安全性，可能简化类似 Claude Artifacts 的 Web 应用的安全沙箱实现。 该实验在 iframe 内使用自定义 fetch() 捕获 CSP 违规，并将其传递给父窗口，父窗口提示用户将域名添加到 connect-src 允许列表并刷新页面。

rss · Simon Willison · May 13, 04:50

**背景**: 内容安全策略（CSP）是一种浏览器安全机制，用于限制页面可以加载的资源。沙箱化 iframe 具有严格的默认 CSP，会阻止大多数网络请求。传统上，允许列表域名需要服务器端配置；该实验提供了一种客户端、用户可控的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/May/13/csp-allow/">Tool: CSP Allow-list Experiment - simonwillison.net</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Content-Security-Policy/sandbox">Content-Security-Policy: sandbox directive - HTTP | MDN</a></li>

</ul>
</details>

**标签**: `#CSP`, `#security`, `#sandbox`, `#iframe`, `#web development`

---

<a id="item-8"></a>
## [英伟达 CEO 基金会向研究人员捐赠 1.08 亿美元 AI 算力](https://www.investing.com/news/stock-market-news/nvidia-ceos-foundation-buys-108-million-of-ai-computing-from-coreweave-donates-it-to-researchers-4686943) ⭐️ 7.0/10

英伟达 CEO 黄仁勋的基金会从云服务商 CoreWeave 购买了价值 1.08 亿美元的 AI 计算服务，并将捐赠给研究人员以支持 AI 研究。 这项重大的慈善投资直接针对学术 AI 研究人员面临的计算资源短缺问题，通过提供高端 GPU 集群访问权限，可能加速突破性进展。 捐赠将通过国家 AI 研究资源（NAIRR）试点项目分配，该项目旨在使 AI 计算访问民主化。专注于 GPU 云计算的 CoreWeave 将提供实际的计算基础设施。

rss · Investing.com All News · May 14, 00:01

**背景**: 训练最先进的 AI 模型需要巨大的计算能力，往往超出学术机构的预算。CoreWeave 是一家提供 GPU 即服务的云提供商，允许客户按需租用英伟达 GPU。NAIRR 试点是美国政府为创建共享 AI 研究基础设施而推出的计划。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave - Wikipedia</a></li>
<li><a href="https://coreweave.com/pricing">CoreWeave Cloud Pricing | CoreWeave</a></li>

</ul>
</details>

**标签**: `#AI computing`, `#Nvidia`, `#CoreWeave`, `#philanthropy`, `#research`

---

<a id="item-9"></a>
## [对模糊的“11 个 AI 代理”术语的批评](https://simonwillison.net/2026/May/13/boris-mann/#atom-everything) ⭐️ 6.0/10

Boris Mann 批评“11 个 AI 代理”这一说法毫无意义，将其比作说“11 个电子表格”或“11 个浏览器标签”。 这一批评凸显了“AI 代理”缺乏明确定义的问题，该词作为越来越流行的流行语，可能在产品宣传和研究讨论中造成误导。 这个类比表明，没有上下文地提及“11 个 AI 代理”，其传达的信息量与说“11 个电子表格”一样少——该术语过于宽泛，没有实际意义。

rss · Simon Willison · May 13, 16:15

**背景**: “AI 代理”一词被广泛使用，但缺乏精确、普遍接受的定义。它可以指从简单聊天机器人到复杂自主系统的任何事物，使得关于代理数量的声明本质上含糊不清。这一争议反映了行业内部关于什么才算代理而非自动化工作流程的更广泛讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.normaltech.ai/p/new-paper-ai-agents-that-matter">Rethinking AI agent benchmarking and evaluation</a></li>
<li><a href="https://ppc.land/google-exposes-the-uncomfortable-truth-about-fake-ai-agents/">Google exposes the uncomfortable truth about "fake" AI agents</a></li>

</ul>
</details>

**标签**: `#ai-agents`, `#ai`, `#agent-definitions`, `#terminology`, `#critique`

---

<a id="item-10"></a>
## [米切尔·桥本批评风险规避的技术决策者](https://simonwillison.net/2026/May/12/mitchell-hashimoto/#atom-everything) ⭐️ 6.0/10

HashiCorp 联合创始人米切尔·桥本在 Lobsters 上发表评论，批评技术决策者（TDM）优先考虑不被解雇而非创新，追随 Gartner 或 McKinsey 等分析师的趋势。他是在讨论 Redis 主页设计的背景下提出这一观点的。 这一评论在软件工程社区引发广泛共鸣，反映了对倾向于安全、可辩解选择而非大胆创新的企业决策的普遍不满。它引发了关于技术领导中风险规避文化的讨论。 桥本特别提到，90% 的 TDM 会追随分析师和公众情绪支持的长期趋势，例如 AI 战略或上下文管理，以做出可辩解采购决策。最初的讨论是由 Redis 主页的设计引发的。

rss · Simon Willison · May 12, 22:21

**背景**: 技术决策者（TDM）是组织中评估和选择技术的个人，通常面临避免失败的压力。Gartner 和 McKinsey 是主要的咨询和分析公司，其报告影响企业采购。桥本是 DevOps 和基础设施软件领域的知名人物。

**标签**: `#enterprise`, `#decision-making`, `#software engineering`, `#commentary`

---

<a id="item-11"></a>
## [LLM 0.32a2 新增对 OpenAI 推理端点的支持](https://simonwillison.net/2026/May/12/llm/#atom-everything) ⭐️ 6.0/10

LLM 0.32a2 现在将支持推理的 OpenAI 模型改为使用 /v1/responses 端点而非 /v1/chat/completions，从而在工具调用中实现交错推理。用户可以看到用不同颜色显示的推理令牌摘要，并可使用 -R 参数隐藏它们。 这一更新提高了使用 GPT-5 等推理模型的用户的透明度，使其更容易理解模型的决策过程。同时也为 LLM 适应未来的 OpenAI API 变更做好了准备，因为 /v1/responses 端点正成为有状态交互的标准。 这是一个 alpha 版本（0.32a2），稳定性不能保证。/v1/responses 端点支持有状态交互以及内置工具，如文件搜索和网络搜索。

rss · Simon Willison · May 12, 17:45

**背景**: LLM 是 Simon Willison 开发的命令行工具，用于对各种语言模型运行提示。/v1/responses 端点是 OpenAI 较新的 API，用于创建与模型的有状态交互，正逐渐取代较旧的 /v1/chat/completions 端点用于推理模型。推理令牌是模型用于得出答案的内部步骤，某些模型可以将其暴露以提高透明度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/api/reference/responses/overview">Responses Overview | OpenAI API Reference</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/foundry/openai/how-to/responses">Use the Azure OpenAI Responses API - Microsoft Foundry</a></li>
<li><a href="https://openrouter.ai/docs/guides/best-practices/reasoning-tokens">Reasoning Tokens | Enhanced AI... | OpenRouter | Documentation</a></li>

</ul>
</details>

**标签**: `#llm`, `#openai`, `#reasoning`, `#tool-release`

---