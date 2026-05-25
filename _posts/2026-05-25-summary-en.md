---
layout: default
title: "Horizon Summary: 2026-05-25 (EN)"
date: 2026-05-25
lang: en
---

> From 41 items, 10 important content pieces were selected

---

1. [Memory costs rise to nearly two-thirds of AI chip component costs](#item-1) ⭐️ 8.0/10
2. [Constraint Decay: LLM Agents Fail on Strict Architectural Rules](#item-2) ⭐️ 8.0/10
3. [Microsoft open-sources earliest DOS source code](#item-3) ⭐️ 8.0/10
4. [Greg Brockman Interview on OpenAI Drama and Non-Profit](#item-4) ⭐️ 8.0/10
5. [Scammers abuse internal Microsoft account to send spam links](#item-5) ⭐️ 8.0/10
6. [Armin Ronacher criticizes AI-generated bug reports](#item-6) ⭐️ 8.0/10
7. [DeepSeek Reasonix: Native coding agent with high caching, low cost](#item-7) ⭐️ 7.0/10
8. [Interactive Book for Mastering Dyalog APL Released](#item-8) ⭐️ 6.0/10
9. [Datasette 1.0a30 introduces customizable Jump to menu](#item-9) ⭐️ 6.0/10
10. [AI recreates 1983 game 'Mad House' from PDF in minutes](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Memory costs rise to nearly two-thirds of AI chip component costs](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 8.0/10

A new analysis from Epoch AI reveals that memory, particularly DRAM and high-bandwidth memory (HBM), now accounts for roughly two-thirds of the total component cost of AI chips, up from about 20% historically. This cost shift has major implications for AI hardware pricing and design, as memory expenses now dominate, potentially affecting the affordability and scaling of AI systems. It also underscores the severe supply constraints in the memory market, which could bottleneck AI progress if not resolved. The cost share increase is driven by soaring demand for HBM in AI accelerators, which requires advanced stacking and consumes significantly more wafer capacity per gigabyte than standard DRAM. For example, Micron noted a 3-to-1 conversion ratio between HBM and DDR5 wafer capacity, meaning HBM production directly compresses general-purpose memory supply.

hackernews · intelkishan · May 24, 16:31 · [Discussion](https://news.ycombinator.com/item?id=48258684)

**Background**: Dynamic random-access memory (DRAM) is the primary type of main memory in computers, while high-bandwidth memory (HBM) is a specialized 3D-stacked DRAM that offers extremely high bandwidth for AI and graphics workloads. The current shortage, sometimes called 'RAMmageddon,' began in 2024 as memory manufacturers shifted capacity to HBM for AI, reducing supply of commodity DRAM and driving up prices across the board.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DRAM">DRAM</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.rambus.com/blogs/hbm3-everything-you-need-to-know/">High Bandwidth Memory (HBM): Everything You Need to Know - Rambus</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed views: some saw a potential 3x cost reduction if DRAM supply catches up, while others lamented steep price hikes (e.g., 96GB RAM costing $1200 vs $250 two years ago). Users questioned how to capitalize on this trend and expressed skepticism about DRAM supply growth keeping pace with AI demand, leading some to delay hardware upgrades.

**Tags**: `#AI hardware`, `#memory costs`, `#semiconductor economics`, `#GPU pricing`, `#DRAM`

---

<a id="item-2"></a>
## [Constraint Decay: LLM Agents Fail on Strict Architectural Rules](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

A new paper systematically evaluates LLM agents in backend code generation under structural constraints and identifies 'constraint decay' — a ~30 percentage point drop in assertion pass rate as constraints accumulate. This reveals a critical reliability gap for using LLM agents in production backend development, warning developers that current agents are suitable for rapid prototyping but not for rigorous production code requiring strict architectural adherence. The study focused on multi-file backend generation and found errors concentrated on convention-heavy frameworks; frontier models were not tested due to cost constraints.

hackernews · wek · May 24, 12:55 · [Discussion](https://news.ycombinator.com/item?id=48256912)

**Background**: Large Language Model (LLM) agents are AI models that autonomously generate code from natural language prompts. 'Constraint decay' is the phenomenon where agent performance degrades when forced to follow explicit structural rules like architectural patterns, ORM mappings, or framework conventions. This is problematic because production backend code often requires strict adherence to such constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.06445">Constraint Decay: The Fragility of LLM Agents in Backend Code ... Constraint Decay: The Fragility of LLM Agents in Backend Code ... Constraint Decay in Backend Code Generation - agentpatterns.ai Constraint Decay: The Fragility of LLM Agents in Back End ... [PDF] Constraint Decay: The Fragility of LLM Agents in ... Constraint Decay: The Fragility of LLM Agents in Backend Code ... Constraint Decay: The Fragility of LLM Agents in Backend Code ...</a></li>
<li><a href="https://www.agentpatterns.ai/verification/constraint-decay-backend-agents/">Constraint Decay in Backend Code Generation - agentpatterns.ai</a></li>

</ul>
</details>

**Discussion**: Comments largely agree with the findings. jdlshore (likely an author) summarizes the paper and notes not testing frontier models. maxbond relates it to another paper on long-horizon tasks. alasano shares their work on a structured orchestrator to enforce constraints, and vishvananda coins 'calcification' for a related pattern.

**Tags**: `#LLM agents`, `#code generation`, `#backend development`, `#constraint decay`, `#AI reliability`

---

<a id="item-3"></a>
## [Microsoft open-sources earliest DOS source code](https://arstechnica.com/gadgets/2026/04/microsoft-open-sources-the-earliest-dos-source-code-discovered-to-date/) ⭐️ 8.0/10

Microsoft open-sourced the earliest known DOS source code, which was painstakingly transcribed from paper printouts by a team of historians. This release provides a rare glimpse into the origins of the software that launched Microsoft's operating system business and fueled the PC revolution. The source code was recovered via OCR from decades-old printouts supplied by Tim Paterson, and the repository also includes the early BASIC interpreter.

hackernews · DamnInteresting · May 24, 01:21 · [Discussion](https://news.ycombinator.com/item?id=48253386)

**Background**: DOS (Disk Operating System) was the foundational operating system for early IBM PCs and compatibles. Microsoft originally licensed 86-DOS from Seattle Computer Products, which later became MS-DOS. The codebase is written in assembly language and is remarkably small by modern standards.

**Discussion**: Commenters expressed gratitude and highlighted the historical importance, noting the BASIC code was arguably more significant. The laborious OCR recovery process was also discussed.

**Tags**: `#open source`, `#DOS`, `#Microsoft`, `#software history`, `#assembly`

---

<a id="item-4"></a>
## [Greg Brockman Interview on OpenAI Drama and Non-Profit](https://fs.blog/knowledge-project-podcast/greg-brockman/) ⭐️ 8.0/10

Greg Brockman, a key figure at OpenAI, gave an in-depth interview covering the company's history, recent leadership turmoil, and the controversy over its non-profit structure. This interview provides rare insider perspectives on OpenAI's internal conflicts and governance issues, which are central to ongoing debates about the direction of AI development and the role of non-profit entities in the tech industry. The interview touches on the firing of Sam Altman by the board, Ilya Sutskever's role, and the lawsuit by Elon Musk. Brockman also shares personal notes from his diary that were part of the lawsuit.

hackernews · prakashqwerty · May 24, 08:29 · [Discussion](https://news.ycombinator.com/item?id=48255593)

**Background**: OpenAI was originally founded as a non-profit AI research company but later created a capped-profit subsidiary. This structure has been criticized as a loophole that allows founders to profit while claiming non-profit status. Recent events include boardroom battles and a lawsuit from co-founder Elon Musk.

**Discussion**: Commenters are skeptical about OpenAI's non-profit claims, with one noting that such structures could set a precedent that non-profit status is meaningless. Others express frustration that key details, like Ilya Sutskever's rationale, remain unexplored.

**Tags**: `#OpenAI`, `#AI`, `#interview`, `#non-profit`, `#drama`

---

<a id="item-5"></a>
## [Scammers abuse internal Microsoft account to send spam links](https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/) ⭐️ 8.0/10

Scammers are exploiting an internal Microsoft account to send spam links, leveraging the account's trusted status to bypass security filters. This incident reveals weaknesses in Microsoft's domain management and security practices, potentially eroding trust in emails from Microsoft domains and affecting millions of users. The attack exploits an internal account within Microsoft's own Entra tenant, making spam appear legitimate. Microsoft has not disclosed the full scope or remediation steps publicly.

hackernews · spike021 · May 24, 00:51 · [Discussion](https://news.ycombinator.com/item?id=48253186)

**Background**: Microsoft uses a vast number of domains for internal and customer communications, making it difficult to track legitimate email sources. Attackers often abuse Microsoft 365 tenants to send spam using onmicrosoft.com domains, and this incident appears to involve similar exploitation of an internal account. Proper domain management and security configurations like DMARC and SPF are critical to prevent such abuse.

<details><summary>References</summary>
<ul>
<li><a href="https://practical365.com/onmicrosoft-com-domains/">Stopping Spam Sent from Bad Microsoft 365 Domains | Practical365</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/01/06/phishing-actors-exploit-complex-routing-and-misconfigurations-to-spoof-domains/">Phishing actors exploit complex routing and misconfigurations to spoof domains | Microsoft Security Blog</a></li>
<li><a href="https://entra.news/p/inside-microsofts-entra-tenant-the">Inside Microsoft’s Entra Tenant: The Internal App Governance ...</a></li>

</ul>
</details>

**Discussion**: Comments highlight frustration with Microsoft's domain complexity and security issues, with some users noting similar phishing abuses and suggesting subdomain solutions like internal.microsoft.com instead of scattered domains.

**Tags**: `#security`, `#spam`, `#Microsoft`, `#phishing`, `#domain abuse`

---

<a id="item-6"></a>
## [Armin Ronacher criticizes AI-generated bug reports](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher, creator of Flask and Jinja, published a blog post on May 24, 2026, criticizing AI-generated bug reports for open-source projects as verbose, inaccurate, and wasteful of maintainer time. He advocates for a simple four-point template for human-observed issue reports. This commentary highlights a growing pain in open-source maintenance as AI tools produce low-quality bug reports that burden volunteer maintainers. If widely adopted, Ronacher's proposed concise format could improve efficiency and reduce burnout in open-source communities. Ronacher specifically calls out the use of 'clanker' (a derogatory term for AI) to describe AI-generated reports that contain 'fake-minimal repros' and 'complete guesswork on root causes'. He suggests that issue reports should consist only of: the command run, expected behavior, actual behavior, and exact error/log output.

rss · Simon Willison · May 24, 18:46

**Background**: AI-generated code and bug reports are becoming common as developers use large language models (LLMs) to assist with software development. However, these reports often lack accuracy and contain confident but incorrect conclusions, creating more work for maintainers. The term 'clanker' is a derogatory slang for AI/robots that has gained popularity online.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Clanker">Clanker - Wikipedia</a></li>
<li><a href="https://www.npr.org/2025/08/06/nx-s1-5493360/clanker-robot-slur-star-wars">What is a clanker and why do we need this word? : NPR</a></li>
<li><a href="https://stackoverflow.blog/2026/01/28/are-bugs-and-incidents-inevitable-with-ai-coding-agents/">Are bugs and incidents inevitable with AI coding agents? - Stack Overflow</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#bug reporting`, `#AI`, `#software maintenance`, `#LLM`

---

<a id="item-7"></a>
## [DeepSeek Reasonix: Native coding agent with high caching, low cost](https://esengine.github.io/DeepSeek-Reasonix/) ⭐️ 7.0/10

DeepSeek Reasonix is a native coding agent optimized for DeepSeek V4 Pro, leveraging aggressive caching to drastically reduce API costs. It runs in the terminal and offers a cache-first loop with flash-first cost control. By maximizing cache hits, Reasonix can reduce token usage and cost, making DeepSeek V4 Pro more affordable for developers. This addresses a key pain point for AI coding agents—high API costs—potentially increasing adoption. However, Reasonix's UX has drawn criticism: the website is poorly designed with animated typing that causes layout shifts, and some users question whether a dedicated agent is necessary when existing tools can already leverage DeepSeek's cache.

hackernews · Alifatisk · May 24, 13:02 · [Discussion](https://news.ycombinator.com/item?id=48256953)

**Background**: DeepSeek V4 Pro is a large Mixture-of-Experts language model with 1.6 trillion parameters (49B activated) supporting a 1M token context. Its API provides caching discounts, but effectively utilizing the cache requires careful prompt design. Reasonix aims to automate this cache optimization.

<details><summary>References</summary>
<ul>
<li><a href="https://esengine.github.io/DeepSeek-Reasonix/">Reasonix — DeepSeek -native AI coding agent</a></li>
<li><a href="https://api-docs.deepseek.com/quick_start/agent_integrations/reasonix">Integrate with Reasonix | DeepSeek API Docs</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some users note that caching benefits are already achievable with simple bridges, while others criticize the agent's UX and website design. A user suggests that the author should submit a PR to existing harnesses rather than build a separate tool. Overall, there is skepticism about the tool's novelty.

**Tags**: `#AI coding agent`, `#DeepSeek`, `#caching`, `#cost optimization`

---

<a id="item-8"></a>
## [Interactive Book for Mastering Dyalog APL Released](https://mastering.dyalog.com/README.html) ⭐️ 6.0/10

A comprehensive interactive book titled 'Mastering Dyalog APL' has been released, featuring Jupyter Notebook examples for hands-on learning. It provides a modern, interactive introduction to the Dyalog APL programming language. This resource lowers the barrier to learning APL, a language known for its concise array-oriented syntax, by offering interactive examples that build muscle memory. It helps programmers explore array programming concepts in a practical, modern environment. The book is available online at mastering.dyalog.com as HTML with embedded Jupyter Notebooks. A PDF version is also provided for offline reading. The original book was already well-regarded, and the interactive treatment enhances learning.

hackernews · tosh · May 24, 11:42 · [Discussion](https://news.ycombinator.com/item?id=48256475)

**Background**: APL (A Programming Language) is a programming language developed in the 1960s by Kenneth E. Iverson, with multidimensional arrays as its central data type. It uses a large range of special symbols to represent functions and operators, enabling very concise code. Dyalog APL is a modern, proprietary implementation by Dyalog Ltd., often used in finance and data analysis for its array processing capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dyalog_APL">Dyalog APL</a></li>
<li><a href="https://en.wikipedia.org/wiki/APL_(programming_language)">APL (programming language) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments show positive reception for the interactive notebook format, which makes learning APL symbols more intuitive. Some readers express concerns about Dyalog's proprietary license and suggest alternative open-source learning resources like learnapl. Others share personal experiences using LLMs to learn APL or translating APL programs to NumPy.

**Tags**: `#APL`, `#Dyalog`, `#programming-language`, `#learning-resource`, `#array-programming`

---

<a id="item-9"></a>
## [Datasette 1.0a30 introduces customizable Jump to menu](https://simonwillison.net/2026/May/24/datasette/#atom-everything) ⭐️ 6.0/10

Datasette 1.0a30 adds a customizable 'Jump to...' menu that allows users to quickly navigate to databases, tables, and other items. It also introduces a new plugin hook, jump_items_sql(), enabling plugins to contribute their own searchable items. This feature enhances user navigation and makes Datasette more extensible, allowing plugin developers to integrate custom navigation items. It improves the overall user experience and encourages ecosystem growth. The menu is triggered by pressing '/' on any Datasette instance (e.g., latest.datasette.io). The jump_items_sql() plugin hook lets plugins define SQL queries whose results become searchable entries in the menu.

rss · Simon Willison · May 24, 23:52

**Background**: Datasette is an open-source Python tool for exploring and publishing SQLite databases as interactive web pages. It supports plugins that can add new features via hooks. This release is an alpha version, meaning it is still under development and may contain changes before the stable 1.0 release.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/datasette/issues/2283">`query_actions` plugin hook - like `table_actions` and `database_actions` for the query/canned query page · Issue #2283 · simonw/datasette</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#python`, `#sqlite`, `#plugin`, `#data publishing`

---

<a id="item-10"></a>
## [AI recreates 1983 game 'Mad House' from PDF in minutes](https://simonwillison.net/2026/May/24/usborne-mad-house/#atom-everything) ⭐️ 6.0/10

Simon Willison fed a PDF of the 1983 Usborne book 'Creepy Computer Games' into Anthropic's Claude AI, which then generated a fully interactive JavaScript and HTML version of the 'Mad House' game. This demonstrates how large language models can rapidly modernize legacy software and make historical games playable again without manual programming, lowering the barrier for retro game preservation. Willison used a single prompt to Claude: 'Build a vanilla JS artifact that exactly recreates the game Mad House from this book, make sure it's mobile friendly and has a suitable retro aesthetic.' He also asked it to credit the book and link to Usborne's free PDFs.

rss · Simon Willison · May 24, 17:14

**Background**: Usborne published a series of computer books in the 1980s containing type-in games for various home computers like the ZX81 and Commodore 64. In recent years, Usborne made free PDFs of these books available online. Claude is a large language model developed by Anthropic, known for its code generation capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_AI">Claude AI</a></li>
<li><a href="https://archive.org/details/Creepy_Computer_Games_1983_Usborne_Publishing">Usborne creepy computer games : Reynolds, Colin... : Internet Archive</a></li>

</ul>
</details>

**Discussion**: On Hacker News, users expressed nostalgia for Usborne books and interest in using AI to recreate other classic games from PDFs. Some discussed the accuracy of the recreation and limitations of AI-generated code.

**Tags**: `#retro computing`, `#AI`, `#game recreation`, `#javascript`, `#claude`

---