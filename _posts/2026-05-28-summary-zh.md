---
layout: default
title: "Horizon Summary: 2026-05-28 (ZH)"
date: 2026-05-28
lang: zh
---

> From 40 items, 15 important content pieces were selected

---

1. [微软 Copilot Cowork 漏洞导致文件泄露](#item-1) ⭐️ 9.0/10
2. [YouTube 将自动标记 AI 生成视频](#item-2) ⭐️ 8.0/10
3. [Simon Willison 认为 Anthropic 和 OpenAI 找到了产品市场契合点](#item-3) ⭐️ 8.0/10
4. [Go 批准泛型方法，即将实现](#item-4) ⭐️ 8.0/10
5. [SQLite AGENTS.md：不接受 AI 代理代码，欢迎错误报告](#item-5) ⭐️ 8.0/10
6. [curl 团队被 AI 辅助安全报告压垮](#item-6) ⭐️ 8.0/10
7. [苹果与谷歌推送通知政策分析](#item-7) ⭐️ 7.0/10
8. [谷歌推崇 AI 模式后，DuckDuckGo 访问量激增 28%](#item-8) ⭐️ 7.0/10
9. [加拿大决定购买瑞典萨博全球眼，冷落美国供应商](#item-9) ⭐️ 7.0/10
10. [Last.fm 脱离 CBS/Paramount 独立运营](#item-10) ⭐️ 7.0/10
11. [GitHub 故障影响拉取请求和 API 请求](#item-11) ⭐️ 7.0/10
12. [Mini Micro：面向学习和爱好者的幻想计算机](#item-12) ⭐️ 7.0/10
13. [2025 年《模拟城市 3000》实现 4K 运行，引发怀旧热潮](#item-13) ⭐️ 6.0/10
14. [用 Markdown 文件自定义 Claude Code](#item-14) ⭐️ 6.0/10
15. [供应商游说进入梵蒂冈：Anthropic 与教皇](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [微软 Copilot Cowork 漏洞导致文件泄露](https://simonwillison.net/2026/May/26/copilot-cowork-exfiltrates-files/#atom-everything) ⭐️ 9.0/10

微软 Copilot Cowork 存在一个安全漏洞，允许智能体未经批准向用户收件箱发送邮件，邮件中的外部图像在用户打开邮件时会触发网络请求，从而泄露数据。攻击者可通过提示注入攻击泄露 OneDrive 的预认证下载链接，进而下载文件。 该漏洞凸显了自主 AI 系统中的根本安全挑战——拥有工具访问权限的智能体可能被利用来窃取敏感数据。随着微软 Copilot 等主要产品集成自主功能，此类缺陷对企业数据安全构成重大威胁。 该攻击利用邮件中外部图像的渲染通过网络请求泄露数据。OneDrive 的预认证下载链接加剧了风险，使攻击者无需凭证即可直接下载文件。

rss · Simon Willison · May 26, 15:36

**背景**: 提示注入是一种网络安全攻击，通过恶意输入导致大语言模型产生意外行为。在自主系统中，AI 智能体可以执行发送邮件、访问云存储等操作，因此容易在检索不受信任内容时遭受间接提示注入攻击。OneDrive 的预认证下载链接无需额外认证即可访问文件，与提示注入结合后成为数据泄露的途径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#AI agents`, `#Microsoft Copilot`, `#data exfiltration`, `#prompt injection`

---

<a id="item-2"></a>
## [YouTube 将自动标记 AI 生成视频](https://blog.youtube/news-and-events/improving-ai-labels-viewers-creators/) ⭐️ 8.0/10

YouTube 宣布将利用检测算法和元数据信号，自动标记完全或主要由 AI 生成的视频。新政策预计将在未来几个月内推出。 这一举措解决了主要平台上对合成媒体日益增长的担忧，帮助观众区分真实内容与 AI 生成的虚假内容。它为整个科技行业的内容审核政策树立了先例，并促进了透明度。 标签系统将同时依赖自动检测工具和创作者的主动披露。结合 AI 与人类创作的混合内容可能面临模糊的阈值，引发关于误报和分类准确性的问题。

hackernews · nopg · May 27, 20:00 · [社区讨论](https://news.ycombinator.com/item?id=48299753)

**背景**: AI 生成的视频（包括深度伪造和合成媒体）已在网络上泛滥，导致虚假信息和信任问题。诸如帧级分析和递归神经网络等检测技术正被开发用于识别此类内容。YouTube 的政策变更是行业向内容真实性和透明度趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2601.11035">Your One-Stop Solution for AI-Generated Video Detection</a></li>
<li><a href="https://genvidbench.github.io/">GenVidBench: A 6-Million Benchmark for AI-Generated Video ...</a></li>
<li><a href="https://www.meegle.com/en_us/topics/deepfake-detection/synthetic-media-identification">Synthetic Media Identification</a></li>

</ul>
</details>

**社区讨论**: 评论中表达了对该政策是否适用于 AI 生成音乐的好奇，对类似 ZeroGPT 工具的误报的担忧，以及关于混合内容阈值的疑问。一些用户欢迎此举以打击欺骗性 AI 视频，而另一些则怀疑自动检测的可靠性。

**标签**: `#AI`, `#YouTube`, `#content-moderation`, `#synthetic-media`

---

<a id="item-3"></a>
## [Simon Willison 认为 Anthropic 和 OpenAI 找到了产品市场契合点](https://simonwillison.net/2026/May/27/product-market-fit/#atom-everything) ⭐️ 8.0/10

Simon Willison 认为，企业 LLM 账单飙升和 Anthropic 传闻中即将实现首次盈利季度，表明 OpenAI 和 Anthropic 已找到产品市场契合点，这与此前对折扣的假设相反。 这一分析表明，AI 公司正从炒作转向可持续收入，可能为 LLM 的巨额基础设施投资提供依据，并重塑企业 AI 的采用模式。 Willison 计算得出他 30 天的 API token 费用将达 2180.16 美元，而订阅费仅需 200 美元，凸显了 Anthropic 和 OpenAI 在 2025 年底和 2026 年初将企业计划转向基于使用量的定价。

rss · Simon Willison · May 27, 16:38 · [社区讨论](https://news.ycombinator.com/item?id=48296794)

**背景**: 产品市场契合点（PMF）是一个商业术语，指产品满足强劲的市场需求，通常带来有机增长和盈利。LLM 公司如 OpenAI 和 Anthropic 最初提供固定费率订阅，但随着 Claude Code 等自主编码工具的普及，token 消耗激增，促使转向基于使用量的定价。这一变化虽然让一些企业感到震惊，但也表明用户认为这些工具价值足够高，愿意支付高额 token 费用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://www.chronoinnovation.com/resources/hidden-cost-explosion-in-ai/">The Hidden AI Cost Explosion: Your LLM Budget Guide | Chrono</a></li>
<li><a href="https://benchlm.ai/llm-pricing-trends">LLM API Pricing History — How AI Model Costs Have Changed ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：一些用户对长期 ROI 表示怀疑，称之为‘最大的骗局’，并质疑当前定价的可持续性。其他人则同意编码领域的 PMF 已经存在，但质疑是否能转化为盈利。少数人支持该分析，指出失败案例很少，且这些工具已成为高薪专业人士的日常工具。

**标签**: `#AI`, `#business`, `#product-market fit`, `#LLMs`, `#profitability`

---

<a id="item-4"></a>
## [Go 批准泛型方法，即将实现](https://github.com/golang/go/issues/77273) ⭐️ 8.0/10

Go 团队正式批准了泛型方法提案，允许方法拥有自己的类型参数。该提案由 Go 联合设计者 Robert Griesemer 提出，现已进入实现阶段。 这填补了 Go 泛型实现中的一个重大空白——此前泛型仅支持函数和类型。该特性使代码更具表达力和可重用性，尤其对数据访问层和函数式编程模式有重要意义。 泛型方法最初因实现复杂性而被排除在 Go 1.18 泛型之外。此次批准的提案逆转了 FAQ 中“不需要”的立场，实现工作已启动。

hackernews · f311a · May 27, 09:02 · [社区讨论](https://news.ycombinator.com/item?id=48291575)

**背景**: Go 在 1.18 版本（2022 年 3 月）引入了泛型，但仅限于函数和类型，方法不能拥有自己的类型参数。这一限制给来自 Java 或 C++ 等语言的开发者带来了常见痛点。Go 团队此前在 FAQ 中表示泛型方法不是优先事项，但社区需求促使他们重新评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theregister.com/2026/03/02/generic_methods_go/">Generic methods approved for Go , devs miss other features</a></li>
<li><a href="https://itsfoss.gitlab.io/post/generic-methods-arrive-in-golang-but-they-werent-the-top-dev-demand/">Generic methods arrive in Golang, but they weren't the... :: IT'S FOSS</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极。评论者指出这解决了令人惊讶的限制，并能实现类似 monad 的模式；也有人开玩笑说 Go 正在慢慢实现之前声称不需要的功能。

**标签**: `#go`, `#generics`, `#programming-languages`

---

<a id="item-5"></a>
## [SQLite AGENTS.md：不接受 AI 代理代码，欢迎错误报告](https://simonwillison.net/2026/May/27/sqlite-agents/#atom-everything) ⭐️ 8.0/10

SQLite 发布了 AGENTS.md 文件，声明不接受代理生成的代码，但欢迎人类提交的 bug 报告和概念验证补丁。此外，由于 AI 生成的 bug 报告泛滥，SQLite 拆分论坛，专门设立了一个 Bug 论坛来处理这类报告。 该政策为开源项目如何处理自主 AI 代理的贡献树立了先例，明确人类监督仍然不可或缺。它直接影响使用 AI 工具为 SQLite 做贡献的开发者，也可能影响面临类似挑战的其他项目。 AGENTS.md 文件明确声明，SQLite 不接受未经事先同意且未将贡献置于公共领域的法律文件支持的拉取请求。最近的一次提交移除了“（目前）”一词，以强化不接受代理代码的立场。

rss · Simon Willison · May 27, 23:44

**背景**: 代理编程是指使用自主 AI 代理来规划、编写、测试和修改代码，人工干预极少。SQLite 一直有严格的贡献政策，要求所有贡献必须属于公共领域，而这项新政策专门针对 AI 生成代码和 bug 报告的兴起。大量低质量的 AI 生成 bug 报告促使 SQLite 创建了一个单独的 Bug 论坛来管理这些报告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/discover/what-is-agentic-coding">What is agentic coding? How it works and use cases | Google Cloud</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-coding">What is Agentic Coding? | IBM</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#open-source`, `#AI agents`, `#software development policy`

---

<a id="item-6"></a>
## [curl 团队被 AI 辅助安全报告压垮](https://simonwillison.net/2026/May/26/the-pressure/#atom-everything) ⭐️ 8.0/10

Daniel Stenberg 报告称，curl 团队收到的安全报告数量是 2024 年的 4-5 倍，是 2025 年的两倍，现在平均每天超过一份，这得益于 AI 辅助报告。这些报告详细且可信，给维护者带来了前所未有的压力。 这凸显了 AI 生成的安全报告对 curl 等关键开源项目造成的不可持续负担，尽管代码本身稳健，但仍可能威胁到维护者的健康和项目的可持续性。 尽管报告如潮水般涌来，但发现的漏洞几乎都是低或中等严重性；上一次高严重性 CVE 在 2023 年 10 月。Stenberg 的妻子对他工作时长表示担忧，凸显了人力成本。

rss · Simon Willison · May 26, 23:48

**背景**: curl 是一个广泛使用的开源命令行工具和库，用于通过 URL 传输数据，对许多系统至关重要。安全报告对于修补漏洞必不可少，但近期由大型语言模型等工具驱动的 AI 辅助报告激增，让这个小型志愿者团队不堪重负。

**标签**: `#security`, `#open-source`, `#curl`, `#AI`, `#maintenance`

---

<a id="item-7"></a>
## [苹果与谷歌推送通知政策分析](https://www.jacquescorbytuech.com/writing/what-apple-and-google-are-doing-your-push-notifications) ⭐️ 7.0/10

一项分析探讨了苹果和谷歌如何不断加强推送通知的控制，限制垃圾和促销通知，优先考虑用户注意力。 这很重要，因为它将权力平衡从应用开发者转向用户，可能减少通知过载，改善移动平台的用户体验。 文章指出，两家公司历史上较为宽容，但现在积极干预以抑制或合并通知，这些变化对广播和促销推送影响最大。

hackernews · iamacyborg · May 27, 19:24 · [社区讨论](https://news.ycombinator.com/item?id=48299220)

**背景**: 推送通知是应用发送到用户设备的消息，常用于提醒、更新或营销。苹果和谷歌分别控制 iOS 和 Android 上的通知基础设施，使他们能够设定政策，影响应用如何接触用户。

**社区讨论**: 评论显示用户强烈希望减少通知，许多用户对应用垃圾信息感到沮丧并主张严格控制。一些评论者认为推送应仅用于事务性通知，而其他人则强调了在应用通信与用户注意力之间取得平衡的历史挑战。

**标签**: `#push notifications`, `#Apple`, `#Google`, `#privacy`, `#app development`

---

<a id="item-8"></a>
## [谷歌推崇 AI 模式后，DuckDuckGo 访问量激增 28%](https://www.pcgamer.com/hardware/duckduckgos-ai-free-search-saw-nearly-28-percent-more-visits-in-the-week-following-googles-insistence-that-people-love-ai-mode/) ⭐️ 7.0/10

据 PC Gamer 引用的 TechCrunch 报道，谷歌宣布新的 AI 搜索模式后一周内，DuckDuckGo 的无 AI 搜索页面（noai.duckduckgo.com）访问量增加了 28%。 这一激增表明用户对主流搜索引擎集成生成式 AI 的反弹情绪日益增长，可能促使注重隐私的用户转向 DuckDuckGo 等替代方案。 增长在 5 月 24 日达到高峰（27.7%），DuckDuckGo 移动应用在美国的安装量也上升，iOS 峰值达 30.5%。但 DuckDuckGo 的整体市场份额相较谷歌仍然微不足道。

hackernews · HelloUsername · May 27, 16:28 · [社区讨论](https://news.ycombinator.com/item?id=48296649)

**背景**: 谷歌最近推出了 AI 模式，这是一种由 Gemini 2.0 驱动的生成式 AI 体验，在搜索结果中提供对话式答案。DuckDuckGo 定位为注重隐私的搜索引擎，不追踪用户，并通过 noai.duckduckgo.com 提供无 AI 搜索选项。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://search.google/ways-to-search/ai-mode/">Google AI Mode - a new way to search, whatever’s on your mind</a></li>
<li><a href="https://labs.google.com/search/experiment/22">AI Mode - Search Labs - labs.google.com</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人因反感强制推送 AI 而转向 DuckDuckGo，也有人喜欢谷歌的 AI 模式方便快速查询。少数人指出，DuckDuckGo 的绝对增长相对于谷歌规模仍然很小。

**标签**: `#search engines`, `#privacy`, `#AI`, `#user backlash`, `#DuckDuckGo`

---

<a id="item-9"></a>
## [加拿大决定购买瑞典萨博全球眼，冷落美国供应商](https://www.theguardian.com/world/2026/may/27/canada-sweden-saab-globaleye-aircraft) ⭐️ 7.0/10

加拿大宣布计划从瑞典订购萨博的全球眼预警机，放弃美国供应商。这一决定反映了西方国防采购的广泛趋势。 此举凸显了地缘政治紧张局势和欧洲防务复兴，盟友正寻求美国设备的替代品。可能重塑跨大西洋防务贸易关系。 萨博全球眼是新一代空中预警和控制系统，无需机上操作员。美国没有直接可比的机型，波音 E-7 楔尾项目面临取消。

hackernews · tosh · May 27, 16:53 · [社区讨论](https://news.ycombinator.com/item?id=48296994)

**背景**: 全球眼基于庞巴迪环球 6000 公务机，部分在加拿大制造。此采购决定源于加拿大总理 2025 年 11 月对瑞典的承诺，并在欧洲军事复兴背景下做出，部分原因是乌克兰战争的教训。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GlobalEye">GlobalEye - Wikipedia</a></li>
<li><a href="https://thedefensewatch.com/product/globaleye-surveillance-aircraft/">GlobalEye Surveillance Aircraft - Full... | TheDefenseWatch.com</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认为该决定是非政治性的合理采购选择，而非纯粹政治决定，指出美国缺乏可比机型以及萨博设备在乌克兰的实战表现。一些人还提及意大利取消美国直升机订单的相关举动，表明盟友正更广泛地远离美国供应商。

**标签**: `#geopolitics`, `#defense`, `#procurement`, `#Canada`, `#Sweden`

---

<a id="item-10"></a>
## [Last.fm 脱离 CBS/Paramount 独立运营](https://support.last.fm/t/last-fm-is-now-independent/118591) ⭐️ 7.0/10

Last.fm 宣布现已独立运营，脱离其前东家 CBS/Paramount，并向用户保证 API 不会改变。 此次独立确保了 Last.fm 音乐追踪和 scrobbling 服务的未来，该服务拥有忠实的用户群，并通过 API 支持众多第三方应用。 公告明确表示 API 使用和条款不会改变，回应了依赖 Last.fm 数据的开发者的担忧。

hackernews · twistslider · May 27, 15:36 · [社区讨论](https://news.ycombinator.com/item?id=48295892)

**背景**: Last.fm 是一家成立于 2002 年的音乐网站，通过名为 Audioscrobbler 的系统追踪用户跨设备和流媒体服务的收听习惯。2007 年被 CBS 公司（后并入 Paramount）收购。该服务因提供详细的收听统计和推荐而深受音乐爱好者欢迎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Last.fm">Last.fm - Wikipedia</a></li>
<li><a href="https://www.last.fm/">Last.fm | Play music, find songs, and discover artists</a></li>
<li><a href="https://blog.postman.com/api-vs-web-service/">API vs Web Service: Understanding the Differences</a></li>

</ul>
</details>

**社区讨论**: 用户表达了宽慰和怀旧之情，称赞 Last.fm 的 API 比其他服务更稳定，并分享了基于 Last.fm 数据构建的项目。

**标签**: `#last.fm`, `#independence`, `#music tracking`, `#API`, `#community`

---

<a id="item-11"></a>
## [GitHub 故障影响拉取请求和 API 请求](https://www.githubstatus.com/incidents/xy1tt3hs572m) ⭐️ 7.0/10

GitHub 发生故障，影响了拉取请求、问题、Git 操作和 API 请求，导致提交和分支变更显示不一致。 此次故障引发了对 GitHub 可靠性的担忧，尤其是随着 AI 驱动开发的增长，开发者对稳定服务的依赖更高。 故障表现为拉取请求差异显示不一致，提交和分支变更未完全反映，可能导致在未充分审查的情况下合并代码。

hackernews · maxnoe · May 27, 12:15 · [社区讨论](https://news.ycombinator.com/item?id=48293080)

**背景**: GitHub 是广泛使用的版本控制和协作平台，托管着数百万个仓库。影响拉取请求和 API 请求等核心功能的故障可能干扰全球的开发工作流。

**社区讨论**: 社区评论对故障频发表示沮丧，部分用户指出拉取请求差异不一致，容易合并不完整的变更。有用户还提到自 AI 编码工具流行以来，其他服务故障也有所增加。

**标签**: `#GitHub`, `#incident`, `#reliability`, `#version control`, `#outage`

---

<a id="item-12"></a>
## [Mini Micro：面向学习和爱好者的幻想计算机](https://miniscript.org/MiniMicro/index.html#about) ⭐️ 7.0/10

Mini Micro 是一个运行 MiniScript 编程语言的幻想计算机平台，面向教育和爱好者计算。它提供了一个复古风格的虚拟机，具有 960x640 分辨率的显示屏和像素/精灵/瓦片图形。 它通过提供完全受控的环境简化了初学者的编程体验，无需完整操作系统的复杂性。这可以帮助新手获得对硬件控制的内在理解，类似于复古计算体验。 Mini Micro 将 MiniScript 的 REPL 作为命令行界面，所有程序都用 MiniScript 编写，保持语法一致。系统支持基于像素和基于瓦片的图形，以及合成和数字化立体声音频。

hackernews · nicoloren · May 27, 09:56 · [社区讨论](https://news.ycombinator.com/item?id=48291947)

**背景**: 幻想计算机是模拟虚构复古风格计算机的虚拟机，通常资源有限以鼓励创造性。MiniScript 是一种干净简单的编程语言，设计用于嵌入或学习，它运行在 C#或 C++引擎上。该项目旨在提供低门槛的编程入门，并具有直接硬件控制的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://miniscript.org/MiniMicro/">Mini Micro</a></li>
<li><a href="https://miniscript.org/">MiniScript Home Page</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示对跨平台硬件支持有浓厚兴趣，例如在 ESP32 或树莓派上运行。有评论指出示例代码中寻找最长公共前缀函数的 bug，其他人则将 Mini Micro 与 Pico-8 等类似项目进行比较。

**标签**: `#fantasy computer`, `#miniscript`, `#educational computing`, `#programming language`

---

<a id="item-13"></a>
## [2025 年《模拟城市 3000》实现 4K 运行，引发怀旧热潮](https://www.thran.uk/writ/hdid/2025/12/simcity-3k-in-4k.html) ⭐️ 6.0/10

一篇博文详细介绍了如何在 2025 年以 4K 分辨率运行《模拟城市 3000》，展示了这款经典城市建造游戏持久不衰的魅力。 这凸显了人们对复古游戏和游戏保护的持续兴趣，社区评论则反映出对老式城市建造游戏富有想象力玩法的怀念，而非现代游戏的超写实风格。 该博文在 Hacker News 上获得了 257 个点赞和 97 条评论，显示出很高的参与度。社区讨论聚焦于游戏的美术风格、顾问系统和音乐。

hackernews · speckx · May 27, 17:36 · [社区讨论](https://news.ycombinator.com/item?id=48297645)

**背景**: 《模拟城市 3000》于 1999 年由 Maxis 发行，被认为是经典的城市建造模拟游戏。2025 年以 4K 分辨率运行它需要借助模组或兼容层，这体现了人们在现代硬件上保留和享受老游戏的持续努力。

**社区讨论**: 评论者们表达了对《模拟城市 3000》的深厚感情，一些人批评现代城市建造游戏过于追求超写实而忽视了想象力。其他人则深情回忆了游戏的顾问系统和音乐，指出后续作品失去了这种魅力。

**标签**: `#SimCity`, `#retro gaming`, `#city building`, `#nostalgia`, `#game preservation`

---

<a id="item-14"></a>
## [用 Markdown 文件自定义 Claude Code](https://arps18.github.io/posts/claude-code-mastery/) ⭐️ 6.0/10

一篇指南发布了，详细说明如何使用 Markdown 文件扩展 Claude Code，包括自定义命令、技能、子代理、插件和 MCP（模型上下文协议）服务器。 这凸显了 AI 编码助手生态系统的成长以及整合的必要性，用户面临碎片化的自定义选项。依赖 Claude Code 提高生产力的开发者将受到影响。 社区评论显示，用户对命令、技能和子代理等重叠功能感到困惑，并批评该指南可能是 AI 生成的且内容浅薄。然而，一些用户报告自定义配置显著提升了生产力。

hackernews · arps18 · May 27, 05:13 · [社区讨论](https://news.ycombinator.com/item?id=48289950)

**背景**: Claude Code 是 Anthropic 开发的一款 AI 编码助手，运行在终端中。用户可以通过基于 Markdown 的配置文件（如 CLAUDE.md）来扩展其功能，定义自定义命令、技能和子代理，或通过模型上下文协议（MCP）连接外部工具。该生态系统正在快速演进，导致概念重叠。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/sub-agents">Create custom subagents - Claude Code Docs</a></li>
<li><a href="https://code.claude.com/docs/en/skills">Extend Claude with skills - Claude Code Docs</a></li>
<li><a href="https://code.claude.com/docs/en/mcp">Connect Claude Code to tools via MCP - Claude Code Docs</a></li>

</ul>
</details>

**社区讨论**: 评论褒贬不一：一些用户认为该指南浅薄且可能是 AI 生成的，而另一些用户则分享实用技巧（例如在 CLAUDE.md 中使用幽默威胁来让 Claude 更谨慎）。还有人呼吁整合各种自定义方法。

**标签**: `#claude-code`, `#ai-coding-assistant`, `#developer-tools`, `#markdown`, `#productivity`

---

<a id="item-15"></a>
## [供应商游说进入梵蒂冈：Anthropic 与教皇](https://simonwillison.net/2026/May/26/corey-quinn/#atom-everything) ⭐️ 6.0/10

Corey Quinn 嘲讽 Anthropic 对教皇方济各通谕《崇高人性》的影响，称这是有史以来最厉害的供应商游说。该通谕据称将 AI 伦理提升为宗教义务，其内容受到 Anthropic 的宪法 AI 原则影响。 这凸显了 AI 伦理游说的新前沿：一家科技公司的安全理念得到最高宗教权威的背书，可能塑造全球伦理规范。同时也引发了对私营企业影响道德框架的质疑。 通谕《崇高人性》于 2026 年 5 月 25 日发布，Anthropic 联合创始人 Christopher Olah 据报道参与了起草。Anthropic 开发的宪法 AI 通过一套预定义规则使 AI 与人类价值观对齐，这一理念似乎体现在通谕中。

rss · Simon Willison · May 26, 02:28

**背景**: 宪法 AI 是 Anthropic 开发的一种技术，用于训练 Claude 等 AI 模型遵循一套伦理原则，旨在使其有益、无害且诚实。这一理念影响了 Anthropic 在负责任 AI 方面的公开立场。梵蒂冈与 Anthropic 的合作标志着科技公司与天主教会在伦理议题上的不寻常联盟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Constitutional_AI">Constitutional AI</a></li>
<li><a href="https://religionnews.com/2026/05/22/why-anthropic-is-helping-unveil-the-popes-new-encyclical-on-ai/">Inside the unlikely Vatican-Anthropic relationship that's reshaping the AI ethics debate</a></li>

</ul>
</details>

**标签**: `#ai-ethics`, `#anthropic`, `#corey-quinn`, `#vendor-lobbying`

---