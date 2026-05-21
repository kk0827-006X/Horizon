---
layout: default
title: "Horizon Summary: 2026-05-21 (EN)"
date: 2026-05-21
lang: en
---

> From 42 items, 13 important content pieces were selected

---

1. [OpenAI Model Disproves Discrete Geometry Conjecture](#item-1) ⭐️ 9.0/10
2. [GitHub confirms breach of 3,800 repos via malicious VSCode extension](#item-2) ⭐️ 9.0/10
3. [Qwen3.7-Max: A New Agent-Focused LLM Claims SOTA](#item-3) ⭐️ 9.0/10
4. [SpaceX S-1 Reveals Starlink Profitability and $1.25B/Month AI Deal with Anthropic](#item-4) ⭐️ 9.0/10
5. [Google Declaring War on the Web: AI Threatens Symbiosis](#item-5) ⭐️ 8.0/10
6. [Mozilla Deprecates asm.js as WebAssembly Takes Over](#item-6) ⭐️ 8.0/10
7. [Railway GCP Account Suspension Incident Report Highlights Reliability Risks](#item-7) ⭐️ 8.0/10
8. [Gemini 3.5 Flash Launches with Higher Price, Broader Integration](#item-8) ⭐️ 8.0/10
9. [Interactive Map of Metal Music Subgenres](#item-9) ⭐️ 6.0/10
10. [SBCL as Assembly Code Breadboard](#item-10) ⭐️ 6.0/10
11. [Simulating LLM Token Speeds: 5 to 800 per Second](#item-11) ⭐️ 6.0/10
12. [Simon Willison on Google I/O: Gemini Spark and Antigravity](#item-12) ⭐️ 6.0/10
13. [Six Months of LLM Progress in Five Minutes](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI Model Disproves Discrete Geometry Conjecture](https://openai.com/index/model-disproves-discrete-geometry-conjecture/) ⭐️ 9.0/10

OpenAI's model has found a counterexample to a long-standing conjecture by Paul Erdős in discrete geometry, demonstrating AI's ability to perform novel mathematical reasoning. This achievement shows that AI can contribute to pure mathematics by discovering new knowledge, challenging the view that AI merely recombines existing data and potentially accelerating mathematical research. The disproof was achieved by finding a counterexample rather than a general proof, and some mathematicians note that disproving a conjecture via counterexample is often considered less insightful than proving it true.

hackernews · tedsanders · May 20, 19:05 · [Discussion](https://news.ycombinator.com/item?id=48212493)

**Background**: Discrete geometry studies combinatorial properties of finite geometric objects, such as points and lines. The conjecture involved point-line incidences, a classic area in discrete geometry. AI models like LLMs are now being applied to explore mathematical conjectures systematically.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Discrete_geometry">Discrete geometry</a></li>

</ul>
</details>

**Discussion**: The community discussion is mixed: some are excited about AI's potential in mathematics, while others debate whether LLMs truly discover or merely recombine. Tim Gowers' remarks are highly recommended, and some find the counterexample approach less impactful than a proof would be.

**Tags**: `#AI`, `#mathematics`, `#discrete geometry`, `#LLM`, `#research`

---

<a id="item-2"></a>
## [GitHub confirms breach of 3,800 repos via malicious VSCode extension](https://www.bleepingcomputer.com/news/security/github-confirms-breach-of-3-800-repos-via-malicious-vscode-extension/) ⭐️ 9.0/10

GitHub confirmed that over 3,800 internal repositories were compromised through a malicious VSCode extension, part of a supply chain attack that also impacted Microsoft's Python SDK. This breach underscores the critical security risk in the developer toolchain, especially VSCode extensions, which are often trusted without scrutiny. It could lead to widespread code theft or further supply chain attacks. The malicious extension was sourced from the VSCode Marketplace and appears to be a worm that targeted Microsoft's Python SDK. The compromised repositories were internal to GitHub, but the extension had a large install base of up to 150,000.

hackernews · Timofeibu · May 20, 13:43 · [Discussion](https://news.ycombinator.com/item?id=48207660)

**Background**: VSCode extensions are add-ons that provide additional functionality but can execute arbitrary code, making them a prime vector for supply chain attacks. The VSCode Marketplace has previously been targeted by malicious extensions, and this incident highlights the need for better vetting and security measures.

<details><summary>References</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pIXy1HWEVSRWQya05EVXpvb0hTZ0FQAQ?hl=en-IN&gl=IN&ceid=IN:en">GitHub internal repositories breached via malicious extension ...</a></li>
<li><a href="https://www.stepsecurity.io/blog/malicious-iolitelabs-vscode-extensions-target-solidity-developers-on-windows-macos-and-linux-with-backdoor">Malicious IoliteLabs VSCode Extensions Target Solidity... - StepSecurity</a></li>
<li><a href="https://www.linkedin.com/posts/abhishek-chatrath1_12-malicious-extension-in-vscode-marketplace-activity-7390035070603956225-KHXz">Malicious VSCode extensions discovered, posing data risk | LinkedIn</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern about the VSCode extension attack vector, with one noting the risk of pop-ups prompting installations of unverified extensions. Another speculated that the attack might involve the compromised nx console extension. Overall sentiment was fear and criticism of the lack of security in the extension ecosystem.

**Tags**: `#security`, `#github`, `#vscode`, `#supply-chain`, `#breach`

---

<a id="item-3"></a>
## [Qwen3.7-Max: A New Agent-Focused LLM Claims SOTA](https://qwen.ai/blog?id=qwen3.7) ⭐️ 9.0/10

Alibaba's Tongyi Lab released Qwen3.7-Max, a proprietary large language model optimized for AI agent tasks, claiming state-of-the-art performance on benchmarks like non-hallucination rate. This release signals the rapid advancement of open-source-aligned models in the agent domain, challenging closed-source leaders like GPT-5 and Gemini. The strong community engagement (594 points, 236 comments) highlights its significance for developers and enterprises seeking cost-effective, high-performance alternatives. Qwen3.7-Max features a 1 million token context window and explicit chain-of-thought reasoning, and integrates office productivity tools via the Model Context Protocol (MCP). It supports multi-agent orchestration and embodied intelligence, but remains proprietary with no confirmed open-source release.

hackernews · kevinsimper · May 20, 10:35 · [Discussion](https://news.ycombinator.com/item?id=48205626)

**Background**: An AI agent is a large language model structured to perform reasoning and complete tasks autonomously, often using tools. Qwen3.7-Max is built on this concept, leveraging chain-of-thought to improve reasoning. The model is developed by Tongyi Lab under Alibaba Cloud, continuing the Qwen series that has been influential in open-source AI, though this version is proprietary.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-7-max">Qwen 3 . 7 Max - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://ar5iv.labs.arxiv.org/html/2401.03568">[2401.03568] Agent AI : Surveying the Horizons of Multimodal Interaction</a></li>
<li><a href="https://news.aibase.com/news/28161">Tongyi Lab Launches Qwen 3 . 7 - Max with Orthogonal Decoupling...</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some users praise the SOTA non-hallucination rate and see it as a great free alternative to Claude Code, while others express disappointment that the model is proprietary rather than open-source. There are also calls for partnerships with US hyperscalers to enable wider enterprise adoption.

**Tags**: `#AI`, `#large language models`, `#open source`, `#Qwen`, `#agents`

---

<a id="item-4"></a>
## [SpaceX S-1 Reveals Starlink Profitability and $1.25B/Month AI Deal with Anthropic](https://www.sec.gov/Archives/edgar/data/1181412/000162828026036936/spaceexplorationtechnologi.htm) ⭐️ 9.0/10

SpaceX's S-1 filing with the SEC shows Starlink turned profitable with $4.4B operating income in 2025, and reveals a $1.25 billion per month cloud services agreement with AI company Anthropic through May 2029. This filing signals that Starlink has become a cash-generating business capable of funding SpaceX's ambitious AI infrastructure bets, and the massive Anthropic deal underscores the growing demand for AI compute capacity, potentially reshaping the space and AI industries. Starlink generated $11.4B in revenue and $4.4B in operating income in 2025, while SpaceX overall reported a net loss of $4.9B due to $20.7B in capital expenditures, primarily for Starlink satellite manufacturing and launch costs.

hackernews · cachecow · May 20, 20:49 · [Discussion](https://news.ycombinator.com/item?id=48213933)

**Background**: An S-1 filing is a registration statement required by the SEC for companies planning to go public, providing detailed financial information. Starlink is SpaceX's satellite internet constellation providing broadband globally. Anthropic is an AI research company known for its Claude model. The deal involves SpaceX providing compute capacity from its Colossus data centers to Anthropic.

**Discussion**: Commenters highlight the surprising profitability of Starlink and the enormous scale of the Anthropic deal, with some questioning the feasibility of space-based data centers and the high valuation given SpaceX's relatively low revenue compared to other tech giants. Others note the company's heavy capital expenditures and net losses despite strong operational cash flow.

**Tags**: `#SpaceX`, `#IPO`, `#Starlink`, `#Anthropic`, `#AI`

---

<a id="item-5"></a>
## [Google Declaring War on the Web: AI Threatens Symbiosis](https://tante.cc/2026/05/20/on-google-declaring-war-on-the-web/) ⭐️ 8.0/10

A critical analysis argues that Google is shifting towards AI-generated content, breaking the traditional symbiotic relationship where websites provide content for crawling in exchange for traffic. This threatens the economic model of web publishers and could lead to a monopolized, low-quality web environment where only large corporations profit from content. AI-generated summaries often contain errors, and website owners report major shifts in viewership, with some seeing upticks but others harmed by incorrect AI summaries.

hackernews · cdrnsf · May 20, 21:33 · [Discussion](https://news.ycombinator.com/item?id=48214449)

**Background**: Traditionally, Google's search engine relies on crawling and indexing web content, providing traffic to websites in return. This symbiotic relationship incentivizes content creation. Google's new focus on AI-generated answers threatens to bypass websites entirely, removing that incentive.

**Discussion**: Commenters express fear that only large corporations can profit from creativity, while individuals are excluded. Some worry that AI summaries often contain errors, and suggest alternatives like StumbleUpon for traffic. Others note that the symbiotic relationship is being broken, and websites may block Google crawlers.

**Tags**: `#Google`, `#AI`, `#Web`, `#Monopoly`, `#Content Creation`

---

<a id="item-6"></a>
## [Mozilla Deprecates asm.js as WebAssembly Takes Over](https://spidermonkey.dev/blog/2026/05/20/saying-goodbye-to-asmjs.html) ⭐️ 8.0/10

Mozilla has announced the deprecation of asm.js, a JavaScript subset for near-native performance. WebAssembly has fully matured and replaced its role in web performance optimization. This marks the end of a foundational era in web technology, where asm.js blazed the trail for running native code in the browser. Developers who relied on asm.js will transition fully to WebAssembly, which offers better performance and smaller bundle sizes. asm.js was a strict subset of JavaScript used as a compilation target for C/C++ via Emscripten, enabling near-native performance. WebAssembly, first released in 2017 and now a W3C standard, supersedes asm.js with a binary format that avoids JavaScript parsing overhead.

hackernews · eqrion · May 20, 12:01 · [Discussion](https://news.ycombinator.com/item?id=48206340)

**Background**: asm.js was introduced by Mozilla in 2013 as a response to Google's NaCl and PNaCl, aiming to bring near-native performance to the web. It works by restricting JavaScript to a subset that can be aggressively optimized by the browser's JavaScript engine. However, asm.js is still JavaScript, leading to larger bundle sizes and parsing overhead. WebAssembly (Wasm) was designed as a true binary format, becoming a W3C recommendation in 2019, and is now supported by all major browsers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asm.js">Asm.js</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="http://asmjs.org/">asm . js</a></li>

</ul>
</details>

**Discussion**: The community comments express a mix of nostalgia and approval. Users recall asm.js's role in making web apps like Figma possible, and reference Gary Bernhardt's famous talk "The Birth and Death of JavaScript" as prophetic. Some note the bittersweet end, but acknowledge WebAssembly is a clear improvement.

**Tags**: `#asm.js`, `#WebAssembly`, `#JavaScript`, `#browser`, `#Mozilla`

---

<a id="item-7"></a>
## [Railway GCP Account Suspension Incident Report Highlights Reliability Risks](https://blog.railway.com/p/incident-report-may-19-2026-gcp-account-outage) ⭐️ 8.0/10

Railway published a detailed incident report on May 19, 2026, regarding a GCP account suspension that caused an outage for its customers, and announced plans to reduce reliance on Google Cloud services in the data plane's hot path. This incident underscores significant reliability and trust concerns with Google Cloud as a B2B provider, serving as a warning for businesses that rely on GCP for critical infrastructure. Railway's architectural decision to re-architect away from GCP reflects growing industry sentiment about cloud provider lock-in risks. The outage was caused by Google Cloud suspending Railway's account without prior warning, affecting Railway's entire platform for an unspecified duration. Railway acknowledged architectural failure in relying solely on GCP and is planning to keep GCP only for secondary or failover purposes.

hackernews · 0xedb · May 20, 08:37 · [Discussion](https://news.ycombinator.com/item?id=48204770)

**Background**: Railway is an all-in-one intelligent cloud platform (PaaS) that enables developers to deploy web apps, databases, and other services by connecting a GitHub repo. Google Cloud Platform (GCP) is a major cloud provider, but has faced criticism for opaque account suspension practices. This incident is part of a broader pattern where GCP customers have experienced sudden service disruptions due to automated or human-driven account flags.

<details><summary>References</summary>
<ul>
<li><a href="https://railway.com/">Railway | The all-in-one intelligent cloud provider</a></li>

</ul>
</details>

**Discussion**: Community comments were highly critical of GCP's reliability, with users warning others about Google's B2B trustworthiness. Some commenters noted the lack of root cause explanation from Google and pointed to past incidents, while praising Railway for taking responsibility and planning to reduce GCP dependency.

**Tags**: `#Google Cloud`, `#incident report`, `#cloud reliability`, `#B2B trust`, `#Railway`

---

<a id="item-8"></a>
## [Gemini 3.5 Flash Launches with Higher Price, Broader Integration](https://simonwillison.net/2026/May/19/gemini-35-flash/#atom-everything) ⭐️ 8.0/10

Google released Gemini 3.5 Flash to general availability at Google I/O, skipping the preview phase, and is integrating it across key products including the Gemini app, Google Search, Google Antigravity, and Gemini Enterprise Agent Platform. This marks a significant step in Google's AI strategy, deploying a more capable but pricier model across free consumer products, signaling a trend of major AI labs testing customer price tolerance. The model ID is gemini-3.5-flash, with a knowledge cutoff of January 2025, supporting 1,048,576 input tokens and 65,536 output tokens. It costs $1.50 per million input tokens and $9 per million output tokens, roughly 3x the price of Gemini 3 Flash Preview.

rss · Simon Willison · May 19, 22:40

**Background**: Gemini 3.5 Flash is part of Google's latest family of large language models. The new Interactions API, in beta, offers server-side history management similar to OpenAI Responses. Google's agent-first development platform Antigravity and Gemini Enterprise Agent Platform are designed for building AI agents.

<details><summary>References</summary>
<ul>
<li><a href="https://www.googleantigravity.org/">AI IDE with Gemini 3 Pro | Agentic Software Development Platform</a></li>
<li><a href="https://cloud.google.com/products/gemini-enterprise-agent-platform">Gemini Enterprise Agent Platform (formerly Vertex AI) | Google Cloud</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#Machine Learning`

---

<a id="item-9"></a>
## [Interactive Map of Metal Music Subgenres](https://mapofmetal.com/) ⭐️ 6.0/10

The Map of Metal, an interactive visualization of metal music subgenres and their evolution, has been ported from Flash to HTML5 by its creator, keeping the project alive for old fans and new visitors. This project preserves a unique and culturally significant historical resource for metal music enthusiasts, demonstrating how legacy Flash-based creative works can be modernized to remain accessible on the modern web. The site was originally built in Flash within about two weeks by the creator and a friend, and later ported to HTML5. The source code is available on GitHub.

hackernews · robin_reala · May 20, 10:47 · [Discussion](https://news.ycombinator.com/item?id=48205699)

**Background**: The Map of Metal is an interactive visualization that charts the evolution and relationships of heavy metal subgenres, from early influences like Led Zeppelin and Black Sabbath to dozens of modern styles. Originally created in Adobe Flash, it became a beloved reference for metal fans. The recent port to HTML5 ensures it works without Flash Player, which is no longer supported by browsers.

**Discussion**: Commenters praised the map's historical accuracy and nostalgic value, with some noting similarities to other music maps like Ishkur's Guide to Electronic Music. Users also expressed interest in similar visualizations for other genres such as jazz, classical, or hip-hop, and requested features like showing spiritual successors of bands.

**Tags**: `#music`, `#visualization`, `#HTML5`, `#interactive`, `#niche`

---

<a id="item-10"></a>
## [SBCL as Assembly Code Breadboard](https://pvk.ca/Blog/2014/03/15/sbcl-the-ultimate-assembly-code-breadboard/) ⭐️ 6.0/10

A 2014 article demonstrates using Steel Bank Common Lisp (SBCL) as a macro-assembler to prototype VM instructions on x86_64, directly mapping VM registers to hardware registers and automatically handling instruction alignment and padding. This technique showcases a creative bridge between high-level Lisp and low-level assembly, enabling rapid prototyping of efficient VM instruction sets without traditional assembler tedium. It remains relevant for compiler and VM developers exploring code generation strategies. The approach uses 8 x86_64 registers as stack slots for a custom VM, and SBCL's compiler macros calculate instruction alignments automatically. The article is a repost from 2014 and is not a new breakthrough, but it continues to attract interest on Hacker News.

hackernews · yacin · May 20, 15:39 · [Discussion](https://news.ycombinator.com/item?id=48209558)

**Background**: SBCL is a high-performance, open-source Common Lisp implementation with a native compiler that can generate efficient machine code. Common Lisp macros allow code transformation at compile time, making SBCL suitable for use as a macro-assembler. A 'breadboard' in electronics is a prototyping board, metaphorically referring to a flexible environment for trying out assembly code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SBCL">SBCL</a></li>
<li><a href="https://archlinux.org/packages/extra/x86_64/sbcl/">Arch Linux - sbcl 2.6.4-1 (x86_64)</a></li>

</ul>
</details>

**Discussion**: Community comments on Hacker News show repeated interest over the years. User snazz finds the article challenging but appreciates the register mapping and alignment calculations; BoingBoomTschak recommends a related article on sb-simd. The discussion highlights the article's enduring educational value.

**Tags**: `#lisp`, `#sbcl`, `#assembly`, `#compiler`, `#low-level`

---

<a id="item-11"></a>
## [Simulating LLM Token Speeds: 5 to 800 per Second](https://simonwillison.net/2026/May/20/tokens-per-second/#atom-everything) ⭐️ 6.0/10

Mike Veerman created a simple HTML app that visually simulates LLM token output at speeds ranging from 5 to 800 tokens per second, helping users grasp real-world reading pace of advertised rates. This tool makes abstract token-per-second metrics tangible, enabling developers and users to better evaluate and compare LLM performance claims. The app simulates speeds from 5 to 800 tokens per second, and its source code is available on GitHub for inspection or modification.

rss · Simon Willison · May 20, 17:57

**Background**: In large language models (LLMs), text is broken into tokens — small units like words or subwords. Tokens per second (TPS) is a common performance metric indicating how quickly a model generates output. However, raw TPS numbers can be hard to interpret without a sense of how fast that actually reads.

<details><summary>References</summary>
<ul>
<li><a href="https://www.baseten.co/blog/comparing-tokens-per-second-across-llms/">Comparing tokens per second across LLMs</a></li>
<li><a href="https://rumn.medium.com/benchmarking-llm-performance-token-per-second-tps-time-to-first-token-ttft-and-gpu-usage-8c50ee8387fa">Benchmarking LLM Performance: Token Per Second (TPS), Time to First Token (TTFT), and GPU Usage</a></li>
<li><a href="https://www.cognativ.com/blogs/post/what-is-a-token-in-llm-a-clear-guide-to-understanding-their-role/314">What is a Token in LLM A Clear Guide to Understanding Their Role</a></li>

</ul>
</details>

**Tags**: `#ai`, `#llms`, `#tools`, `#visualization`

---

<a id="item-12"></a>
## [Simon Willison on Google I/O: Gemini Spark and Antigravity](https://simonwillison.net/2026/May/20/google-io/#atom-everything) ⭐️ 6.0/10

Simon Willison discusses Google I/O 2026 announcements, focusing on the Gemini Spark AI agent and the Antigravity platform, while adhering to his policy of only writing about generally available products. Gemini Spark marks Google's entry into the personal AI agent space, directly competing with OpenClaw, and raises critical questions about agent security and prompt injection risks as users entrust sensitive data to the agent. Gemini Spark runs on Gemini 3.5 Flash and Antigravity, where Antigravity is a Go-based CLI tool and SDK; the open-source Gemini CLI will be deprecated on June 18, replaced by the closed-source Antigravity CLI.

rss · Simon Willison · May 20, 15:32

**Background**: Gemini Spark is a 24/7 personal AI agent that connects with Google apps like Gmail, Calendar, and Drive. Antigravity is a platform comprising a desktop app, CLI tool, SDK (Python wrapper around a Go binary), and an IDE (VS Code fork). OpenClaw is an open-source personal AI assistant that serves as a competitor, running locally and integrating with LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/products/gemini-app/next-evolution-gemini-app/">The Gemini app becomes more agentic, delivering proactive, 24/7 help</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5/">Gemini 3.5: frontier intelligence with action</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#google-io`, `#ai-agent`, `#gemini`, `#google`, `#personal-blog`

---

<a id="item-13"></a>
## [Six Months of LLM Progress in Five Minutes](https://simonwillison.net/2026/May/19/5-minute-llms/#atom-everything) ⭐️ 6.0/10

Simon Willison delivered a lightning talk at PyCon US 2026, summarizing key LLM developments from November 2025 to May 2026 with annotated slides. He highlighted the 'November 2025 inflection point' and noted that the 'best' model changed hands five times among Anthropic, OpenAI, and Google. This talk provides a concise, curated snapshot of the rapidly evolving LLM landscape, helping developers and AI enthusiasts quickly grasp the pace of progress. Willison's unique 'pelican on a bicycle' test offers a creative, unbiased benchmark for comparing model capabilities. The talk covers the period from November 2025 to May 2026, including the release of models like Claude Sonnet 4.5, GPT-5.1, Gemini 3, GPT-5.1 Codex Max, and Claude Opus. Willison used his annotated presentation tool, which runs entirely in the browser without uploading images to a server, to create the slides.

rss · Simon Willison · May 19, 01:09

**Background**: Simon Willison is a well-known Python developer and creator of Datasette. His annotated presentation tool allows users to add textual annotations to slide images, making talks more accessible and shareable. The 'pelican riding a bicycle' test is his personal benchmark for evaluating LLM image generation quality, chosen because it's a task unlikely to be in training data.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2023/Aug/6/annotated-presentations/">How I make annotated presentations | Simon Willison ’s Weblog</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#PyCon`, `#AI developments`, `#lightning talk`

---