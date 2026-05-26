---
layout: default
title: "Horizon Summary: 2026-05-26 (ZH)"
date: 2026-05-26
lang: zh
---

> From 31 items, 9 important content pieces were selected

---

1. [微软 Copilot Cowork 功能存在提示注入漏洞，可导致数据泄露](#item-1) ⭐️ 8.0/10
2. [加州提议将 Linux 从年龄验证法中豁免](#item-2) ⭐️ 8.0/10
3. [Armin Ronacher 批评 AI 生成的错误报告](#item-3) ⭐️ 8.0/10
4. [Mullvad 推出出口 IP 指纹识别缓解措施](#item-4) ⭐️ 7.0/10
5. [《Magnifica Humanitas》：梵蒂冈关于技术伦理的通谕](#item-5) ⭐️ 7.0/10
6. [C 语言扩展与可移植性挑战](#item-6) ⭐️ 7.0/10
7. [Datasette 1.0a30 发布可自定义的跳转菜单](#item-7) ⭐️ 7.0/10
8. [用 AI 从 PDF 重建 1983 年游戏《疯狂小屋》](#item-8) ⭐️ 7.0/10
9. [挪威用 2PB 华为闪存和 HPE Cray 训练主权语言模型](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [微软 Copilot Cowork 功能存在提示注入漏洞，可导致数据泄露](https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files) ⭐️ 8.0/10

PromptArmor 的研究人员演示了对微软 Copilot 的“Cowork”功能的提示注入攻击，通过一个恶意技能即可将用户敏感数据窃取到攻击者控制的服务器。 该漏洞对广泛采用 Copilot 的企业构成了严重的安全风险，削弱了人们对处理敏感数据的 AI 代理的信任。它凸显了在安全措施不足的情况下匆忙将 AI 功能推向生产的危险。 该攻击使用一个仅包含五行看似无害代码的精心设计的技能，上传后通过提示注入触发 Copilot 执行“curl | bash”命令，将数据发送到外部服务器。Cowork 功能仍处于测试/预览阶段，正在逐步推出。

hackernews · Kneenex · May 25, 21:45 · [社区讨论](https://news.ycombinator.com/item?id=48272354)

**背景**: 提示注入是一种安全漏洞，恶意输入会导致大型语言模型产生意外行为。微软 Copilot 的 Cowork 功能是一个 AI 自动化层，可以在多个 Office 应用中执行多步骤任务。技能是用户上传的用于扩展 Copilot 能力的程序，类似于插件，但这个技能包含一个隐藏的提示，从而劫持了助手。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.microsoft.com/en-us/microsoft-365-copilot/get-started-with-cowork-frontier">Get started with Cowork (Frontier) | Microsoft Support</a></li>
<li><a href="https://fortune.com/2026/03/09/microsoft-copilot-cowork-ai-agents-anthropic-e7-m365-saas/">Microsoft debuts Copilot Cowork built with Anthropic’s help... | Fortune</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：有人认为该攻击是“预期行为”，因为技能是具有完全访问权限的程序；而另一些人则批评微软在没有充分加强安全的情况下匆忙推出此功能。一位评论者指出，标题具有误导性和煽动性，但技术发现本身是有效的。

**标签**: `#security`, `#prompt injection`, `#AI agents`, `#Microsoft`, `#exfiltration`

---

<a id="item-2"></a>
## [加州提议将 Linux 从年龄验证法中豁免](https://www.tomshardware.com/software/linux/california-moves-to-exempt-linux-from-its-upcoming-age-verification-law-after-backlash-over-forcing-operating-systems-to-collect-users-ages-amendment-proposed-by-the-same-lawmaker-who-wrote-the-original-law) ⭐️ 8.0/10

加州立法者提出一项修正案，将 Linux 从该州即将出台的年龄验证法中豁免，此前开源社区对此强烈反对。 此举保护了开源操作系统免受侵入式年龄验证要求的影响，为技术监管设立了重要先例，维护了用户隐私和软件自由。 该修正案由原法律起草人提出，专门豁免 Linux 及其他可能开源操作系统收集用户年龄的要求。

hackernews · rbanffy · May 25, 18:19 · [社区讨论](https://news.ycombinator.com/item?id=48269961)

**背景**: 加州年龄验证法要求平台实施年龄检查以保护未成年人上网。批评者认为，将其应用于 Linux 将迫使这一开源操作系统实施用户监控，违背了隐私和自由的核心原则。

**社区讨论**: 评论指出这对开源社区是一次政治胜利，但更多人担忧该法律将负担转嫁给消费者而非监管公司。有人注意到讽刺之处：使用 Linux 的极客可以访问更多内容，而其他人仍受限。

**标签**: `#Linux`, `#age-verification`, `#California law`, `#open source`, `#privacy`

---

<a id="item-3"></a>
## [Armin Ronacher 批评 AI 生成的错误报告](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher 发表博客文章，批评 AI 生成的错误报告不准确且过于自信，倡导采用仅记录人类直接观察的简洁四步格式。 这一批评凸显了开源维护中日益严重的挑战：低质量的 AI 生成问题浪费维护者时间并引入噪音，威胁协作软件开发的效率。 Ronacher 提出的格式要求报告者说明运行的命令、预期结果、实际结果以及确切的错误或日志，去除任何 AI 生成的推测或改写。

rss · Simon Willison · May 24, 18:46

**背景**: 像大型语言模型（LLM）这样的 AI 工具越来越多地被用于撰写或改写错误报告，但它们常常产生听起来合理但实际错误的分析。这种现象有时被称为“垃圾内容”，给必须筛选误导信息的开源维护者带来负担。

**标签**: `#AI`, `#open source`, `#bug reports`, `#software engineering`, `#LLM`

---

<a id="item-4"></a>
## [Mullvad 推出出口 IP 指纹识别缓解措施](https://mullvad.net/en/help/exit-ip-vpn-servers-mitigation-rollout) ⭐️ 7.0/10

Mullvad 宣布推出一项针对 VPN 服务器出口 IP 指纹识别的缓解措施，该措施将重新生成 WireGuard 密钥并更改内部 IP 地址，以防止用户在不同服务器之间被关联。 这项缓解措施解决了一个可能让攻击者跨服务器追踪 VPN 用户的隐私漏洞，增强了用户匿名性，并为 VPN 行业树立了隐私标准。 新方法每次会话随机分配出口 IP 地址，消除服务器之间的关联性，并自动重新生成 WireGuard 密钥以防止长期追踪。

hackernews · Cider9986 · May 25, 17:45 · [社区讨论](https://news.ycombinator.com/item?id=48269580)

**背景**: 出口 IP 指纹识别是一种攻击者通过观察用户在不同 VPN 服务器上被分配的出口 IP 地址来追踪其活动的技术。Mullvad 的新缓解措施通过确保每台服务器的分配随机且独立，打破了这种关联，使得跨会话关联用户更加困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TCP/IP_stack_fingerprinting">TCP/IP stack fingerprinting - Wikipedia</a></li>
<li><a href="https://mullvad.net/en/blog/exit-ip-fingerprinting-between-vpn-servers">Exit IP fingerprinting between VPN servers | Mullvad VPN</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了 Mullvad 浏览器的内置代理和随机模式等 IP 轮换功能，总体反应积极。部分用户对更广泛的防指纹识别措施表示兴趣，例如伪造一致且标准化的设备配置文件。

**标签**: `#VPN`, `#privacy`, `#fingerprinting`, `#Mullvad`, `#security`

---

<a id="item-5"></a>
## [《Magnifica Humanitas》：梵蒂冈关于技术伦理的通谕](https://www.vatican.va/content/leo-xiv/en/encyclicals/documents/20260515-magnifica-humanitas.html) ⭐️ 7.0/10

教宗方济各（原文本错误，应为教宗良十四世）颁布了一封名为《Magnifica Humanitas》的通谕，探讨技术及其权力集中带来的伦理和社会影响。 这封来自梵蒂冈这一重要道德权威的通谕，为讨论技术伦理提供了重要框架，并将影响关于人工智能和权力动态的全球对话。 通谕宣称“技术从来不是中立的”，建设者负有道德责任，并警告核能、生物技术和信息技术导致的权力集中。

hackernews · theletterf · May 25, 10:11 · [社区讨论](https://news.ycombinator.com/item?id=48265206)

**背景**: 通谕是教宗就当代问题发布的正式信件。这份《Magnifica Humanitas》延续了梵蒂冈对技术道德维度的关注，建立在教宗方济各先前关于技术对人类影响的警示之上。

**社区讨论**: 评论者普遍赞扬梵蒂冈对技术的看法，有人指出它提出了关于权力和责任的重要问题。一位无神论评论者表示梵蒂冈对技术的见解最为出色，也有人质疑技术是否能为社会利益所驯服。

**标签**: `#ethics`, `#technology`, `#society`, `#AI`, `#Vatican`

---

<a id="item-6"></a>
## [C 语言扩展与可移植性挑战](https://lemon.rip/w/6-c-extensions-compilers/) ⭐️ 7.0/10

本文探讨了编译器特定扩展（如 __attribute__）在 GCC、Clang、TinyCC 等编译器之间移植代码时引起的可移植性问题，并讨论了解决方法。 这一点很重要，因为 C 语言广泛用于系统编程，而糟糕的可移植性迫使开发者维护脆弱的变通方法，阻碍了替代编译器和平台的采用。 常见的变通方法包括条件性的 #ifdef 防护（例如检查 __GNUC__），但当编译器不冒充 GCC 但仍使用类似扩展时，这些方法常常失效。文章还强调了 slimcc 的平台头文件黑客等改进兼容性的努力。

hackernews · xngbuilds · May 25, 14:15 · [社区讨论](https://news.ycombinator.com/item?id=48267126)

**背景**: C 语言扩展是编译器添加的非标准特性，用于提供底层功能，例如用于对齐变量或指定函数属性的 __attribute__。每个编译器（GCC、Clang、MSVC 等）都有自己的扩展集合，依赖这些扩展的代码可能无法在其他编译器上编译。标准 C（ISO C）避免这些扩展，但现实项目常常依赖它们来实现性能或硬件访问。

**社区讨论**: 来自 ndesaulniers（内核开发者）和 WalterBright（D 语言创始人）等开发者的社区评论证实了这种痛苦，WalterBright 分享了他实现 ImportC 时在头文件中遇到的各种混乱。其他人建议 Common Lisp 生态系统的做法（让可移植性库自然涌现）可以作为一种模式。

**标签**: `#C programming`, `#portability`, `#compilers`, `#systems programming`, `#extensions`

---

<a id="item-7"></a>
## [Datasette 1.0a30 发布可自定义的跳转菜单](https://simonwillison.net/2026/May/24/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a30 于 2026 年 5 月 24 日发布，新增了一个可自定义的“跳转到”菜单，用户可在最新演示站点上按 '/' 键激活。同时引入了 jump_items_sql() 插件钩子，允许插件向菜单的搜索结果中添加项目。 这一增强功能改善了在 Datasette 实例中的导航，使用户能更快地找到数据库、表和调试选项。插件钩子提供了可扩展性，使社区能够构建针对其数据发布需求的自定义导航快捷方式。 “跳转到”菜单在 Datasette 博客上有详细描述，jump_items_sql() 钩子在官方插件钩子文档中有记录。该菜单可在 latest.datasette.io 演示站点上试用。

rss · Simon Willison · May 24, 23:52

**背景**: Datasette 是由 Simon Willison 创建的开源工具，用于探索和发布数据，特别是 SQLite 数据库。它提供用于浏览和查询数据集的 Web 界面，并支持通过插件系统扩展功能。此 alpha 版本继续朝着 1.0 稳定版开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/May/21/datasette-agent/">Datasette Agent | Simon Willison’s Weblog</a></li>

</ul>
</details>

**标签**: `#datasette`, `#opensource`, `#plugin`, `#sqlite`, `#datapublishing`

---

<a id="item-8"></a>
## [用 AI 从 PDF 重建 1983 年游戏《疯狂小屋》](https://simonwillison.net/2026/May/24/usborne-mad-house/#atom-everything) ⭐️ 7.0/10

Simon Willison 使用 Claude 从 Usborne 的《Creepy Computer Games》PDF 中重建了 1983 年游戏《疯狂小屋》的交互式 JavaScript 版本。 这展示了大型语言模型如何从扫描文档中高效重建历史软件，保护复古游戏体验。 该游戏是通过将 PDF 输入 Claude 并提示其生成移动友好的原生 JavaScript 产物且具有复古美学而创建的。

rss · Simon Willison · May 24, 17:14

**背景**: Usborne 免费发布了其 1980 年代计算机书籍的 PDF，包括 1983 年的《Creepy Computer Games》。Claude 是 Anthropic 开发的 AI 助手，能够编程和理解文档。《疯狂小屋》是一款基于文本的迷宫恐怖游戏，最初为 Commodore 64 等家用电脑编写。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/introducing-claude">Introducing Claude \ Anthropic</a></li>
<li><a href="https://archive.org/details/Creepy_Computer_Games_1983_Usborne_Publishing">Usborne creepy computer games : Reynolds, Colin : Free Download, Borrow, and Streaming : Internet Archive</a></li>

</ul>
</details>

**标签**: `#retro computing`, `#AI-assisted development`, `#JavaScript`, `#game recreation`, `#Claude`

---

<a id="item-9"></a>
## [挪威用 2PB 华为闪存和 HPE Cray 训练主权语言模型](https://www.blocksandfiles.com/flash/2026/05/22/norways-2-petabytes-of-huawei-flash-storage-and-llm-training/5244910) ⭐️ 6.0/10

挪威部署了 2 拍字节的华为闪存存储和一套 HPE Cray Supercomputing EX 系统，用于训练一个专为挪威语言和文化打造的主权大语言模型（LLM）。 这一举措凸显了主权人工智能（sovereign AI）日益增长的趋势，即各国投资独立的 AI 基础设施以减少对外国技术的依赖并保护文化和语言数据。同时也展示了使用 HPC 系统以较小规模训练 LLM 的可能性，挑战了关于所需资源的惯有观念。 这套名为 Olivia 的 HPE Cray 系统配备了 448 颗 GPU 和 64,512 个 CPU 核心，部分评论者认为对于训练一个完整的 LLM 而言规模较小。华为提供的 2 PB 闪存存储价格相对低廉，可能仅需约 20 万美元。

hackernews · rbanffy · May 25, 19:37 · [社区讨论](https://news.ycombinator.com/item?id=48270770)

**背景**: 主权人工智能（sovereign AI）是指各国旨在开发独立 AI 能力（包括模型、数据和硬件）以减少对外国供应商依赖的国家战略。挪威的这一努力正是该趋势的一部分，专注于创建一个理解其独特语言和文化的 LLM，而一般以英语为中心的模型可能无法覆盖这些内容。挪威国家图书馆丰富的数字化文本收藏为训练提供了大量数据集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hpe.com/us/en/collaterals/collateral.a00094635enw.html">HPE Cray Supercomputing EX QuickSpecs | HPE</a></li>
<li><a href="https://grokipedia.com/page/Sovereign_AI">Sovereign AI</a></li>
<li><a href="https://e.huawei.com/en/products/storage/hybrid-flash-storage">OceanStor Hybrid Flash Storage | Huawei Enterprise</a></li>

</ul>
</details>

**社区讨论**: 评论者对硬件是否足够表示怀疑，其中一人认为这可能是在浪费资源，并建议改用微调开源模型。其他人则提议挪威应将训练数据免费分享给所有模型构建者，而不是自建 LLM。还有少数人指出闪存存储成本很低，从而质疑该项目的规模。

**标签**: `#LLM`, `#Norway`, `#sovereign AI`, `#flash storage`, `#HPC`

---