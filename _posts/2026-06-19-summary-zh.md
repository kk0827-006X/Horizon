---
layout: default
title: "Horizon Summary: 2026-06-19 (ZH)"
date: 2026-06-19
lang: zh
---

> From 50 items, 14 important content pieces were selected

---

1. [研究者发现 1 万个 GitHub 仓库分发木马恶意软件](#item-1) ⭐️ 9.0/10
2. [诺姆·沙泽尔加入 OpenAI](#item-2) ⭐️ 9.0/10
3. [GLM-5.2：最强大的开源权重 LLM 发布](#item-3) ⭐️ 9.0/10
4. [医院和大学以降低 90%的成本重新利用药物](#item-4) ⭐️ 8.0/10
5. [消费者倡导者挑战强制同意，Elkjop 被罚 180 万欧元](#item-5) ⭐️ 8.0/10
6. [瑞士议会解除新建核电站禁令](#item-6) ⭐️ 8.0/10
7. [W Social：欧洲数字主权还是政治作秀？](#item-7) ⭐️ 8.0/10
8. [慈善·梅杰斯：AI 让代码变成一次性](#item-8) ⭐️ 8.0/10
9. [康奈尔大学 CS 6120 高级编译器课程提供在线自学版](#item-9) ⭐️ 7.0/10
10. [网站检测 LLM 对你在线存在的识别程度](#item-10) ⭐️ 7.0/10
11. [掌握 Git 忽略：超越.gitignore](#item-11) ⭐️ 7.0/10
12. [Datasette Apps 插件发布，提供沙箱 SQL 访问](#item-12) ⭐️ 7.0/10
13. [Ubiquiti 发布基于 ZFS 的企业级 NAS](#item-13) ⭐️ 6.0/10
14. [Datasette ACL 插件扩展为通用资源共享系统](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [研究者发现 1 万个 GitHub 仓库分发木马恶意软件](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 9.0/10

一位安全研究人员发现约 1 万个 GitHub 仓库正在分发木马恶意软件，这很可能是一场针对自动化代理和开发者的协调供应链攻击的一部分。 这一发现揭示了一场针对开源生态系统的大规模自动化攻击，可能感染无数下游项目和用户，凸显了软件供应链中的关键漏洞。 恶意仓库通过频繁提交新内容来出现在搜索结果中并逃避检测；它们专门设计用于被自动依赖解析器和 AI 编码助手抓取。

hackernews · theorchid · Jun 18, 11:45 · [社区讨论](https://news.ycombinator.com/item?id=48583928)

**背景**: 木马恶意软件伪装成合法软件以诱骗用户安装。供应链攻击针对开发者与其依赖之间的关系，将恶意代码注入可信来源。托管数百万个仓库的 GitHub 是此类攻击的主要载体。

**社区讨论**: 社区成员确认了类似经历，有人发现自己的名字被附加到未知仓库上。讨论强调攻击是自动化的，针对 AI 代理和自动化工具而非直接针对人类用户，并提到了过去真实事件，如迪士尼工程师因 GitHub 工具而受到入侵。

**标签**: `#security`, `#malware`, `#github`, `#supply-chain-attack`, `#open-source`

---

<a id="item-2"></a>
## [诺姆·沙泽尔加入 OpenAI](https://twitter.com/NoamShazeer/status/2067400851438932297) ⭐️ 9.0/10

诺姆·沙泽尔——具有里程碑意义的论文《注意力就是你所需要的一切》的合著者、前谷歌 Gemini 联合负责人——已离开谷歌并加入 OpenAI。 此次高调的人才流动凸显了人工智能研究领导权方面的激烈竞争，沙泽尔在 Transformer 架构方面的专业知识是现代语言模型的基础。 沙泽尔最初于 2021 年离开谷歌，联合创立了 Character.AI；随后于 2024 年通过一笔据称价值 27 亿美元的授权交易回归谷歌，而现在他又再次离开，转投 OpenAI。

hackernews · lukasgross · Jun 18, 00:26 · [社区讨论](https://news.ycombinator.com/item?id=48578913)

**背景**: Transformer 架构由沙泽尔合著的 2017 年论文《注意力就是你所需要的一切》提出，它用自注意力机制取代了循环层，彻底改变了自然语言处理。沙泽尔在联合创立 Character.AI 之前是谷歌的长期研究员，回归谷歌后担任了 Gemini AI 模型项目的联合负责人。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/models">Models - Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**社区讨论**: 评论者指出沙泽尔在谷歌工程史上的传奇地位，并提供了他从 Character.AI 回归谷歌再转投 OpenAI 的职业变动背景，部分人对他在最近回归后这么快再次离开表示惊讶。

**标签**: `#AI`, `#transformers`, `#openai`, `#google`, `#talent`

---

<a id="item-3"></a>
## [GLM-5.2：最强大的开源权重 LLM 发布](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai 于 2026 年 6 月 16 日发布了 GLM-5.2，这是一个 753B 参数的混合专家（MoE）LLM，拥有 40B 活跃参数、100 万 token 的上下文窗口，并采用 MIT 许可证。它在 Artificial Analysis Intelligence 指数 v4.1 上以 51 分领先于其他开源权重模型。 GLM-5.2 为开源权重 LLM 树立了新标杆，超越了 DeepSeek V4 Pro 和 Kimi K2.6 等模型，并在 Code Arena WebDev 排行榜上仅次于 Claude Fable 5 排名第二。此次发布极大地推动了开源 AI 发展，以宽松许可证提供了尖端能力。 GLM-5.2 是纯文本模型，总大小 1.51TB，采用 MoE 架构，每个 token 激活 40B 参数。它特别消耗 token，每个任务使用 43k 输出 token，高于其前身 GLM-5.1（26k）和竞品。该模型通过 OpenRouter 提供，价格为每百万输入 token $1.40、每百万输出 token $4.40。

rss · Simon Willison · Jun 17, 23:58

**背景**: GLM-5.2 是 Z.ai 的 GLM-5 系列的一部分，由从清华大学分拆出来的中国公司智谱 AI（Zhipu AI）开发。它针对编码和智能体任务进行了优化，拥有 100 万 token 的大上下文窗口，适用于超长范围任务。混合专家（MoE）架构使得模型总参数数量巨大，但每个 token 只激活一部分，从而提高了效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacamp.com/blog/glm-5-2">GLM - 5 . 2 : Features, Setup, Benchmarks, and Model ... | DataCamp</a></li>
<li><a href="https://www.verdent.ai/guides/what-is-glm-5-2">What Is GLM - 5 . 2 ? A Developer's Guide to Z.ai's Coding Model</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**标签**: `#LLM`, `#open-source`, `#AI`, `#natural-language-processing`, `#transformer`

---

<a id="item-4"></a>
## [医院和大学以降低 90%的成本重新利用药物](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

医院和大学正在将现有药物重新用于新适应症，与品牌替代品相比，成本降低高达 90%。 这种方法可以显著降低医疗成本，并改善对黄斑变性等疾病和罕见病的治疗可及性，挑战当前的药品定价模式。 一个显著例子是阿瓦斯汀（贝伐珠单抗）被重新用于黄斑变性，每剂 50 美元，而 Lucentis 每剂 1500 美元。然而，未经制造商同意或自身成为制造商，超说明书使用缺乏监管途径。

hackernews · giuliomagnifico · Jun 18, 10:33 · [社区讨论](https://news.ycombinator.com/item?id=48583386)

**背景**: 药物再利用是指将已获批药物用于新的医疗适应症，成本通常仅为原药的零头。这在眼科和精神病学中很常见，但监管和财务障碍阻碍了广泛采用。

**社区讨论**: 评论中提到了真实案例，如阿瓦斯汀治疗黄斑变性，以及 Spravato（艾司氯胺酮）与氯胺酮的比较。用户指出 Spravato 是氯胺酮的专利修饰版本，但效果较差，并批评激励机制的扭曲。一位评论者提到了非营利组织 Cures Within Reach，该组织资助药物再利用研究。

**标签**: `#drug repurposing`, `#healthcare costs`, `#pharmaceuticals`, `#macular degeneration`, `#ketamine`

---

<a id="item-5"></a>
## [消费者倡导者挑战强制同意，Elkjop 被罚 180 万欧元](https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/) ⭐️ 8.0/10

一名挪威消费者倡导者坚持挑战 Elkjop 客户俱乐部中的强制同意做法，五年后导致该公司被处以 180 万欧元的 GDPR 罚款。 此案表明个人能够针对大公司执行 GDPR 权利，并为忠诚度计划中强制同意营销的行为设立了非法先例。 该罚款由挪威数据保护局（Datatilsynet）在倡导者拒绝同意并记录违规行为后发出。该公司承认，成为会员是接收营销优惠的条件。

hackernews · speckx · Jun 18, 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48589501)

**背景**: 通用数据保护条例（GDPR）要求数据处理同意必须是自由给予、具体、知情且明确的。强制同意——以同意不必要处理作为服务条件——违反了 GDPR 第 7 条第 4 款。客户忠诚度计划经常收集个人数据，但必须在不捆绑的情况下获得有效同意。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gdpr.eu/what-is-gdpr/">What is GDPR , the EU’s new data protection law? - GDPR .eu</a></li>
<li><a href="https://gdpr-info.eu/">General Data Protection Regulation ( GDPR ) – Legal Text</a></li>
<li><a href="https://martech.org/gdpr-day-1-google-and-facebook-sued-for-forced-consent/">GDPR day 1: Google and Facebook sued for ' forced consent '</a></li>

</ul>
</details>

**社区讨论**: 社区成员赞扬了倡导者的坚持，有人指出类似的抵制行为很少见，尤其是在美国。其他人提供了官方决定和机器翻译的链接，提供了技术资源。一位评论者幽默地指出了起诉为他赢得案件的机构的讽刺意味。

**标签**: `#privacy`, `#GDPR`, `#consent`, `#regulation`, `#consumer rights`

---

<a id="item-6"></a>
## [瑞士议会解除新建核电站禁令](https://www.bluewin.ch/en/news/switzerland/parliament-lifts-ban-on-new-nuclear-power-plants-3257535.html) ⭐️ 8.0/10

瑞士议会投票决定解除新建核电站的禁令，不过该决定仍需在全民公投中获得批准才能生效。 这一政策转变可能显著改变瑞士的能源战略，重新引发关于能源安全、安全性以及核能在清洁能源未来中角色的辩论。 该禁令最初是在 2011 年福岛核事故后引入的；新决定必须通过可能的全民公投，而左翼和绿党强烈反对。

hackernews · leonidasrup · Jun 18, 14:17 · [社区讨论](https://news.ycombinator.com/item?id=48585746)

**背景**: 瑞士目前运营着四座核反应堆，提供约三分之一的电力。2011 年的福岛事故导致逐步淘汰的决定，禁止新建核电站。近期的能源安全关切和气候目标重新激发了人们对核能作为低碳能源的兴趣。

**社区讨论**: 社区评论反映了两极化的辩论：一些人认为核电安全且提供能源安全，而另一些人则强调成本、废物和依赖进口燃料的问题。有人怀疑新电站能否及时建成，并希望可再生能源和水力储能能填补缺口。

**标签**: `#nuclear energy`, `#energy policy`, `#Switzerland`, `#clean energy`, `#energy security`

---

<a id="item-7"></a>
## [W Social：欧洲数字主权还是政治作秀？](https://blog.elenarossini.com/w-social-public-institutions-and-the-theater-of-european-digital-sovereignty/) ⭐️ 8.0/10

Elena Rossini 发表了一篇批判性博文，审视了被标榜为欧洲数字主权倡议的社交网络 W Social，质疑其透明度，并指出这更像是一场政治作秀，而非真正的开源社区建设。 这一分析对欧洲数字主权项目的真实性提出了重要质疑，探讨这些项目究竟是真正服务于公共利益，还是仅仅是政治人物的表演性举措。 博文指出，W Social 是闭源的，以有限责任公司形式运营且追求盈利，并迅速吸引了多位欧盟高层政治家加入；而名为 Eurosky 的开源替代方案却未得到任何媒体关注。

hackernews · nemoniac · Jun 18, 12:46 · [社区讨论](https://news.ycombinator.com/item?id=48584497)

**背景**: 欧洲数字主权指的是欧盟推动减少对非欧洲技术平台依赖的努力。W Social 作为本土替代品推出，旨在抗衡 X 等平台，但其闭源性质和企业结构，与通常与数字主权项目（如基于 AT Protocol 的 Eurosky）相关的开放理念形成对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bangkokpost.com/world/3272749/w-marks-the-xspot-european-social-network-takes-on-musk">W marks the X-spot: European social network takes on Musk</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了怀疑，将 W Social 与 Truth Social 相提并论，并指出其公司架构和缺乏透明度。有人提到一个透明的开源替代方案 Eurosky 被媒体忽视，而其他人则指出欧盟政治家迅速加入是一个警示信号。

**标签**: `#digital sovereignty`, `#social media`, `#EU politics`, `#closed-source`, `#community critique`

---

<a id="item-8"></a>
## [慈善·梅杰斯：AI 让代码变成一次性](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

知名工程师慈善·梅杰斯（Charity Majors）指出，AI 从根本上改变了代码生产的经济模式，使代码生成变得几乎免费且即时，代码从珍贵资产变为一次性消费品。 这一转变对软件工程实践、项目管理以及代码本身的价值产生了深远影响。开发者可能需要重新思考如何设计、维护和投资代码库。 梅杰斯特别指出，这一变化在 2025 年‘几乎一夜之间’发生。她强调，尽管代码生产成本低廉，工程纪律反而变得更加重要，而非更不重要。

rss · Simon Willison · Jun 17, 17:12

**背景**: 传统上，编写代码是劳动密集且耗时的，因此开发者将代码视为需要重用和精心维护的宝贵资产。随着大型语言模型（LLM）等 AI 辅助编程工具的出现，生成代码变得轻而易举，挑战了这一长期假设。

**标签**: `#ai-assisted-programming`, `#generative-ai`, `#software-engineering`, `#economics-of-code`, `#charity-majors`

---

<a id="item-9"></a>
## [康奈尔大学 CS 6120 高级编译器课程提供在线自学版](https://www.cs.cornell.edu/courses/cs6120/2025fa/self-guided/) ⭐️ 7.0/10

康奈尔大学的高级编译器课程 CS 6120 现已作为自引导在线课程开放，所有材料（包括讲座、笔记和作业）均可免费获取用于自学。 这使得高质量的高级编译器教育对任何人开放，有助于培养下一代编译器工程师和研究人员。该课程涵盖静态单赋值（SSA）形式和动态编译等核心概念，这些都是现代编译器设计的基础。 课程涵盖死代码消除、数据流分析、支配者分析和 SSA 形式等主题，其中关于动态编译器的部分侧重于踪迹编译。社区反馈指出踪迹编译被认为是死胡同，且该材料可能更适合作为编译器入门课程而非高级课程。

hackernews · ibobev · Jun 18, 11:04 · [社区讨论](https://news.ycombinator.com/item?id=48583606)

**背景**: 静态单赋值（SSA）形式是优化编译器中使用的中间表示，其中每个变量只赋值一次，从而支持高效的数据流分析。动态编译（包括即时编译）根据执行概况在运行时优化代码，常用于现代编程语言运行时（如 Java 的 HotSpot）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Static_single-assignment_form">Static single-assignment form - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dynamic_compilation">Dynamic compilation</a></li>

</ul>
</details>

**社区讨论**: 用户 'titzer' 批评课程对踪迹编译的侧重是死胡同，建议更好地覆盖类型反馈、推测和去优化。'j2kun' 质疑课程的“高级”标签，指出许多主题是典型的第一门编译器课程内容。尽管有这些批评，但总体情绪对免费资源表示感激。

**标签**: `#compilers`, `#online-course`, `#academic`, `#systems`

---

<a id="item-10"></a>
## [网站检测 LLM 对你在线存在的识别程度](https://www.intheweights.com/) ⭐️ 7.0/10

一个新网站 intheweights.com 并行查询多个 LLM，根据个人在线存在判断它们识别该人的程度，并给出评分和响应聚类。 随着流量从网络转向 LLM，该工具揭示了个人的数字足迹在模型权重中的编码程度，引发隐私和认知问题。 该网站查询前沿和小型模型，对响应进行聚类以评估一致性，并将仅单个模型给出合理但可能错误答案的情况归为幻觉。

hackernews · turtlesoup · Jun 18, 20:49 · [社区讨论](https://news.ycombinator.com/item?id=48591348)

**背景**: LLM 的'权重'是训练过程中学到的参数，存储了知识。此类工具探测个人的在线数据（如 Reddit 历史）是否嵌入在这些权重中，即个人是否'存在于权重中'。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@tahirbalarabe2/llm-weights-context-and-memory-explained-simply-03685b6789c0">LLM Weights Context and Memory Explained Simply - Medium</a></li>
<li><a href="https://arxiv.org/pdf/2605.17110">Capturing LLM Capabilities via Evidence-Calibrated Query ...</a></li>

</ul>
</details>

**社区讨论**: 用户反馈结果不一：有的被正确识别，有的则是幻觉。一位用户注意到非确定性和添加更多关键词分数会提高；另一位则质疑隐私问题。

**标签**: `#LLM`, `#privacy`, `#training data`, `#recognition`, `#community discussion`

---

<a id="item-11"></a>
## [掌握 Git 忽略：超越.gitignore](https://nelson.cloud/.gitignore-isnt-the-only-way-to-ignore-files-in-git/) ⭐️ 7.0/10

理解这些替代方法有助于开发者保持.gitignore 文件的整洁和项目特异性，避免提交如 IDE 工件等不需要的文件，并通过使用全局排除项来更有效地协作个人工作流程。 .git/info/exclude 文件是每个仓库的但不被提交，适用于仅本地的忽略规则。全局.gitignore（通过 core.excludesfile 配置）适用于机器上的所有仓库，非常适合操作系统或编辑器特定的文件。此外，.gitattributes 可以忽略某些文件的差异而不阻止跟踪。

hackernews · FergusArgyll · Jun 18, 10:29 · [社区讨论](https://news.ycombinator.com/item?id=48583356)

**背景**: Git 提供了多种忽略文件不被跟踪的方式。最常见的是.gitignore 文件，它是版本控制的并与团队共享。然而，还有本地和全局机制：.git/info/exclude 用于仓库特定的个人忽略，以及通过 git config core.excludesfile 配置的全局.gitignore 文件。这些对于忽略永远不应提交的文件（如操作系统或编辑器临时文件）非常有用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://git-scm.com/docs/gitignore">Git - gitignore Documentation</a></li>
<li><a href="https://docs.github.com/en/get-started/git-basics/ignoring-files">Ignoring files - GitHub Docs</a></li>
<li><a href="https://stackoverflow.com/questions/7335420/can-i-use-a-global-user-profile-scope-gitignore-file">Can I use a global (user-profile-scope) .gitignore file? Usage example</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了这篇文章并补充了更多见解。有人强调了.gitattributes 用于忽略如 package-lock.json 等嘈杂文件的差异。另一个人强调全局排除可以避免用 IDE/OS 文件弄乱项目的.gitignore。一个用户指出~/.config/git/ignore 是全局 Git 配置文件的合适位置。总体情绪是积极的，感谢揭示了不太为人知的 Git 功能。

**标签**: `#git`, `#.gitignore`, `#version control`, `#best practices`

---

<a id="item-12"></a>
## [Datasette Apps 插件发布，提供沙箱 SQL 访问](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 7.0/10

发布了 datasette-apps 插件，允许用户在 Datasette 中嵌入自定义 HTML+JavaScript 应用，这些应用在沙箱 iframe 中运行，可执行只读 SQL 查询，并通过存储查询可选地执行写操作。 该插件将 Datasette 从数据探索工具转变为构建和托管交互式数据驱动 Web 应用的平台，能够安全嵌入第三方应用而不损害数据隐私。 应用在具有 sandbox="allow-scripts allow-forms"的 iframe 中运行，并通过 CSP 头部阻止外部 HTTP 请求，防止数据泄露；只有配置了适当权限的存储查询才允许执行写操作。

rss · Simon Willison · Jun 18, 23:58

**背景**: Datasette 是一个开源工具，用于将数据探索和发布为交互式网站和 API，基于 SQLite 构建。它提供 JSON API 用于自定义前端。datasette-apps 插件通过为任意 HTML 和 JavaScript 应用提供安全沙箱来扩展此功能，灵感来自 Claude Artifacts 和作者早期的 vibe-coding 工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/datasette: An open source multi-tool for ... The Datasette Ecosystem Introduction to Datasette, a Frontend to Tabulated Data datasette · PyPI Datasette Reviews, Pricing & Alternatives (2026) | Toolradar Datasette - skills.network</a></li>
<li><a href="https://www.w3schools.com/tags/att_iframe_sandbox.asp">HTML iframe sandbox Attribute</a></li>

</ul>
</details>

**标签**: `#datasette`, `#plugin`, `#web app`, `#SQL`, `#data visualization`

---

<a id="item-13"></a>
## [Ubiquiti 发布基于 ZFS 的企业级 NAS](https://blog.ui.com/article/introducing-enterprise-nas) ⭐️ 6.0/10

Ubiquiti 发布了企业级 NAS，该设备基于 ZFS 文件系统构建，配备双 25GbE SFP28 端口和冗余电源。 这标志着 Ubiquiti 进入企业存储市场，利用 ZFS 的高级数据完整性和快照功能。然而，社区对 Ubiquiti 软件可靠性和安全历史的质疑可能影响其采用。 该 NAS 采用 ZFS，提供容错和通过 Merkle 树结构实现的高效增量备份。它针对企业用户，但面临关于机械硬盘能否饱和 25GbE 链路的质疑，以及过去安全事件（如 AWS 密钥泄露和未经授权的摄像头访问）的担忧。

hackernews · ksec · Jun 18, 14:24 · [社区讨论](https://news.ycombinator.com/item?id=48585866)

**背景**: ZFS 是一种结合文件系统和卷管理器的技术，最初由 Sun Microsystems 开发，以数据完整性、可扩展性以及快照和复制等高级功能著称。Ubiquiti 是一家网络硬件公司，过去曾因软件质量和安全漏洞受到批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ZFS">ZFS - Wikipedia</a></li>
<li><a href="https://itsfoss.com/what-is-zfs/">What is ZFS ? Why are People Crazy About it?</a></li>

</ul>
</details>

**社区讨论**: 评论中既有对 ZFS 的兴奋，也有对 Ubiquiti 的怀疑。用户提到过去的安全问题和软件质量问题，有人称该产品为“在生产环境中测试”。其他人则欣赏没有持续费用，但担心长期可行性。

**标签**: `#Ubiquiti`, `#NAS`, `#ZFS`, `#storage`, `#enterprise`

---

<a id="item-14"></a>
## [Datasette ACL 插件扩展为通用资源共享系统](https://simonwillison.net/2026/Jun/18/datasette-acl/#atom-everything) ⭐️ 6.0/10

datasette-acl 插件 0.6a0 版本发布，从仅限表的权限扩展到为多用户 Datasette 实例提供通用资源共享系统。 此次发布为 Datasette 中的细粒度访问控制铺平了道路，支持更灵活的多用户部署和复杂的数据共享场景。 主要工作由 Alex Garcia 完成，该插件现在支持管理不仅仅是表的资源权限，正向全面的 ACL 系统迈进。

rss · Simon Willison · Jun 18, 19:03

**背景**: Datasette 是一个开源工具，用于探索和发布数据，将其转化为交互式网站和 API。datasette-acl 插件增加了高级权限控制，允许管理员为不同用户授予或限制对特定数据资源的访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/18/datasette-acl/">Release: datasette-acl 0.6a0 - simonwillison.net</a></li>
<li><a href="https://github.com/datasette/datasette-acl">GitHub - datasette/datasette-acl: Advanced permission ...</a></li>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>

</ul>
</details>

**标签**: `#datasette`, `#acl`, `#permissions`, `#plugin`

---