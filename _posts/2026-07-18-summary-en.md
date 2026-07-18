---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 51 items, 17 important content pieces were selected

---

1. [First atmosphere detected on rocky exoplanet LHS 1140b](#item-1) ⭐️ 9.0/10
2. [Kimi K3: 2.8 Trillion Parameter Open-Weight Model](#item-2) ⭐️ 9.0/10
3. [Firefox Runs Inside a Browser via WebAssembly](#item-3) ⭐️ 9.0/10
4. [Inkling: 975B MoE Open-Weights Model from Mira Murati's Lab](#item-4) ⭐️ 9.0/10
5. [Open Source AI Landscape Shows Rapid Growth](#item-5) ⭐️ 8.0/10
6. [GPT-5.6 Codex Bug Deletes Files in Unsandboxed Mode](#item-6) ⭐️ 8.0/10
7. [Linus Torvalds Declares Linux Is Not Anti-AI](#item-7) ⭐️ 8.0/10
8. [xAI Open-Sources Grok Build After Privacy Backlash](#item-8) ⭐️ 8.0/10
9. [Kaiser Nurses: AI and Surveillance Undermining Care Quality](#item-9) ⭐️ 7.0/10
10. [Zilog Z80 Microprocessor Celebrates 50th Anniversary](#item-10) ⭐️ 7.0/10
11. [Julia Evans' practical SQLite tips: .expert and backups](#item-11) ⭐️ 7.0/10
12. [Honeypot Live: Real-Time SSH Bot Interaction Visualization](#item-12) ⭐️ 7.0/10
13. [Project Orion Nuclear Pulse Rocket Revisited](#item-13) ⭐️ 7.0/10
14. [Mermaid Diagrams Rendered as Colorful ASCII Art in Browser via WebAssembly](#item-14) ⭐️ 7.0/10
15. [Recurse Center Founder Thanks HN for 15 Years of Support](#item-15) ⭐️ 6.0/10
16. [LLM Cliché Highlighter Spots AI Writing Patterns](#item-16) ⭐️ 6.0/10
17. [New Tool Renders Mermaid Diagrams as Unicode Box Art via WASM](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [First atmosphere detected on rocky exoplanet LHS 1140b](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 9.0/10

Using the James Webb Space Telescope, astronomers have detected an atmosphere on LHS 1140b, a super-Earth located in the habitable zone of the red dwarf star LHS 1140. This marks the first confirmed atmosphere on a rocky exoplanet in the habitable zone. This discovery is a milestone in exoplanet research, offering the first opportunity to study the atmosphere of a potentially habitable Earth-sized world. It paves the way for future searches for biosignatures and understanding planetary habitability. LHS 1140b is about 5.6 times Earth's mass and 70% larger in radius, likely an ocean world with 9-19% water by mass. The atmosphere was detected via transmission spectroscopy, and the planet orbits its star every 24.7 days at 0.0946 AU.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: Exoplanet atmospheres are studied using transit spectroscopy, where starlight filters through a planet's atmosphere during a transit, revealing absorption signatures. LHS 1140b was discovered in 2017 by the MEarth Project. Red dwarfs like LHS 1140 are known for intense flares that can strip atmospheres, making this detection significant for planet habitability studies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - NASA Science</a></li>
<li><a href="https://www.science.org/content/article/astronomers-spot-first-atmosphere-around-potentially-habitable-alien-world">Astronomers spot first atmosphere around a potentially ... - Science</a></li>

</ul>
</details>

**Discussion**: Comments express mixed reactions: some speculate about silicon-based life, while others debate whether LHS 1140b is truly Earth-like or more like a mini-Neptune. One user references a arXiv paper showing JWST emission spectroscopy rules out a mini-Neptune, and others discuss the Fermi paradox and suggest building a solar lens telescope.

**Tags**: `#exoplanets`, `#atmosphere`, `#JWST`, `#astrobiology`, `#habitable zone`

---

<a id="item-2"></a>
## [Kimi K3: 2.8 Trillion Parameter Open-Weight Model](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 9.0/10

Moonshot AI announced Kimi K3, a 2.8 trillion parameter open-weight model, claiming it surpasses GPT-5.5 and Claude Opus 4.8 on several benchmarks, with open weights promised by July 27, 2026. This marks a milestone in open-weight AI, as K3 is the largest openly available model to date, potentially accelerating research and applications while intensifying competition among AI labs. K3 costs $3 per million input tokens and $15 per million output tokens, making it the most expensive model from a Chinese lab. It also uses 21% fewer output tokens than its predecessor K2.6, as reported by Artificial Analysis.

rss · Simon Willison · Jul 16, 20:19 · [Discussion](https://news.ycombinator.com/item?id=48947717)

**Background**: The pelican benchmark is an informal test created by developer Simon Willison, asking LLMs to generate an SVG of a pelican riding a bicycle. It has been used for over 21 months to qualitatively compare models, but its validity as a benchmark is debated due to potential data contamination. Kimi K3 produced a pelican SVG costing 25 cents.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/16/kimi-k3/">Kimi K3, and what we can still learn from the pelican benchmark</a></li>
<li><a href="https://fortune.com/2026/07/16/moonshots-kimi-k3-pushes-chinese-ai-into-fable-level-territory/">Moonshot’s Kimi K3 pushes Chinese AI into Fable-level territory | Fortune</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>

</ul>
</details>

**Discussion**: Commenters questioned the pelican benchmark's reliability, with OsrsNeedsf2P noting that pelican examples likely exist in training data. btown proposed a more adversarial variant incorporating tool calls. Others discussed tokenizer quirks, such as devttyeu's observation that Kimi K3's token count for the prompt suggests a hidden 85-token system prompt.

**Tags**: `#large language models`, `#open-weight models`, `#AI benchmarks`, `#Kimi K3`, `#model evaluation`

---

<a id="item-3"></a>
## [Firefox Runs Inside a Browser via WebAssembly](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter successfully compiled the full Firefox/Gecko engine to WebAssembly, enabling the browser to run inside another browser tab. The project used approximately $25,000 worth of AI-generated code from Claude Opus and Fable tokens to overcome engineering challenges. This demonstration proves that a full modern browser engine can be compiled to WebAssembly and run in a sandboxed browser environment, opening possibilities for secure isolation, browser-based IDE sandboxes, and cross-platform applications. It also showcases the potential of AI-assisted engineering to tackle previously intractable porting tasks. The demo uses the Wisp protocol to proxy all network traffic over a WebSocket connection through Puter's server, since WebAssembly code in browsers cannot open arbitrary network connections. The project claims end-to-end encryption: traffic to HTTPS sites was encrypted, while HTTP traffic was in cleartext when inspected.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (Wasm) is a low-level binary instruction format that allows code written in languages like C++ to run in web browsers at near-native speed. The Wisp protocol is an open standard for proxying multiple TCP/UDP sockets over a single WebSocket connection, enabling network access for Wasm modules that cannot directly use raw sockets. Compiling a full browser engine like Gecko (Firefox's rendering engine) to Wasm is an extremely complex task due to the sheer size of the codebase and dependencies on system-level features.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>
<li><a href="https://developer.puter.com/labs/firefox-wasm/">Firefox in WebAssembly</a></li>
<li><a href="https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/">Firefox in WebAssembly</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was highly enthusiastic, with many commenters impressed by the technical achievement and the clever use of AI. Some raised concerns about the cost and efficiency of proxying all traffic through Puter's server, and the team confirmed they had to scale up servers to handle the traffic spike. There was also curiosity about performance compared to native Firefox.

**Tags**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Wasm`, `#AI-assisted engineering`

---

<a id="item-4"></a>
## [Inkling: 975B MoE Open-Weights Model from Mira Murati's Lab](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

Mira Murati's Thinking Machines Lab released Inkling, a 975B-parameter Mixture-of-Experts multimodal model with 41B active parameters, under the Apache-2.0 license. This release adds a strong US-based open-weights contender to the ecosystem, potentially boosting competition and innovation in open-source AI. Inkling is not a frontier model but is designed as a strong base for fine-tuning, especially via Thinking Machines' Tinker platform; a smaller Inkling-Small (276B/12B active) is promised once testing completes.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) is a neural architecture that uses a gating mechanism to selectively activate only a subset of expert subnetworks per input token, enabling efficient scaling. Open-weights models release trained parameters but not full training details, allowing customization and inspection. This release is notable because it comes from a new lab led by former OpenAI CTO Mira Murati.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/mixture-of-experts-transformer">Mixture - of - Experts Transformer</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you've been told</a></li>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our open-weights model - Thinking Machines Lab</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#multimodal`, `#Mira Murati`, `#Thinking Machines Lab`

---

<a id="item-5"></a>
## [Open Source AI Landscape Shows Rapid Growth](https://stateofopensource.ai/) ⭐️ 8.0/10

The report 'State of Open Source AI' presents data showing that open models have overtaken closed models in token processing on OpenRouter, with open models processing 4.19 trillion tokens daily and holding 63% market share. This marks a significant shift from four months ago when closed models held a 60% majority. This trend suggests that open models are becoming the dominant force in AI inference, potentially challenging the business models of companies like Anthropic and OpenAI. The rapid adoption could accelerate innovation and reduce costs for AI deployment. The data is derived from OpenRouter API usage, and a dashboard tracking daily updates is available. Critics note that the report's presentation appears to be AI-generated, with charts loosely connected to text.

hackernews · rellem · Jul 17, 14:31 · [Discussion](https://news.ycombinator.com/item?id=48947825)

**Background**: Open source AI models, such as Meta's Llama and Mistral, are freely available for use and modification, unlike closed models from OpenAI and Anthropic. The debate centers on whether open models can match the performance of frontier closed models while offering lower cost and greater customizability.

**Discussion**: Comments on Hacker News express both excitement and skepticism. Some see open models as a threat to closed providers, citing usage data. Others criticize the report's AI-generated prose and lack of deep analysis, with one commenter calling it 'an LLM's idea of a CTO presentation.'

**Tags**: `#open source`, `#AI`, `#large language models`, `#community debate`

---

<a id="item-6"></a>
## [GPT-5.6 Codex Bug Deletes Files in Unsandboxed Mode](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

Thibault Sottiaux reported a bug in GPT-5.6 (Codex) where the AI coding agent can delete user files when running in full access mode without sandboxing and with the HOME environment variable misconfigured. This bug highlights a critical safety risk in AI coding agents, as file deletion can cause irreversible data loss. It underscores the need for mandatory sandboxing and review features before deploying autonomous agents. The bug occurs specifically when full access mode is enabled, sandboxing is off, and auto review is disabled; the model attempts to override the $HOME env var to define a temporary directory, but mistakenly deletes $HOME instead.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is a lightweight coding agent from OpenAI that runs locally in the terminal, capable of executing code and managing files. Coding agents like Codex operate with varying levels of autonomy and can perform actions on the user's system. Sandboxing isolates the agent's operations to prevent damage, and auto review requires user confirmation before critical actions. This bug demonstrates the risks when both protections are disabled.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/openai/codex">GitHub - openai/codex: Lightweight coding agent that runs in your terminal · GitHub</a></li>
<li><a href="https://crabtalk.ai/blog/agent-sandbox-permissions">Sandboxing AI agents: beyond Docker and WASM | CrabTalk</a></li>

</ul>
</details>

**Tags**: `#ai-safety`, `#codex`, `#bug`, `#generative-ai`, `#coding-agents`

---

<a id="item-7"></a>
## [Linus Torvalds Declares Linux Is Not Anti-AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds, the creator of Linux, publicly stated on the Linux kernel mailing list that Linux is not an anti-AI project and that AI is a clearly useful tool. He warned that those who disagree can fork the project or walk away. This firm stance from the top-level maintainer signals a strong endorsement of AI within the Linux kernel ecosystem, likely encouraging integration of AI tools and reducing resistance among developers. It may also influence the broader open-source community's acceptance of AI. Torvalds emphasized that AI's usefulness was unclear a year ago but is now beyond question, though he acknowledged other open questions remain, such as AI's economic impact. The statement was made on the linux-media mailing list in response to kernel development discussions.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linux is the world's largest open-source operating system kernel, overseen by Linus Torvalds. AI, particularly large language models (LLMs), has sparked debates in open-source communities regarding ethics and practical value. Torvalds' stance represents a pragmatic acceptance of AI as a development tool.

**Tags**: `#Linux`, `#AI`, `#open source`, `#Linus Torvalds`

---

<a id="item-8"></a>
## [xAI Open-Sources Grok Build After Privacy Backlash](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 8.0/10

After it was discovered that the grok CLI tool uploaded entire directories to xAI's cloud storage, xAI disabled the feature, deleted retained data, and open-sourced the entire Grok Build codebase under the Apache 2.0 license. This incident highlights critical privacy risks in AI-powered developer tools and the importance of transparency. By open-sourcing the code, xAI aims to rebuild trust and allows the community to audit the software. The Grok Build repository contains over 844,000 lines of Rust code in a single initial commit, with notable components including a system prompt and a Mermaid diagram renderer. xAI also disabled default data retention starting July 12, 2026, and deleted previously retained coding data.

rss · Simon Willison · Jul 15, 23:59

**Background**: Grok Build is a terminal-based AI coding agent developed by xAI that can edit files, run commands, and manage tasks. The recent privacy breach occurred because the tool automatically uploaded entire directories, including sensitive files like SSH keys and password databases, to xAI's cloud servers without clear user consent.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xai-org/grok-build">Grok Build - GitHub</a></li>
<li><a href="https://thehackernews.com/2026/07/grok-build-uploads-entire-git.html">Grok Build Uploaded Entire Git Repositories to xAI Storage, Not Just ...</a></li>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>

</ul>
</details>

**Discussion**: One user reported that running grok in their home directory uploaded 'SSH keys, my password manager database, my documents, photos, videos, everything,' sparking widespread outrage. In response, xAI and Elon Musk assured users that all uploaded data would be deleted and that retention is now disabled by default, but many remain skeptical about the company's data practices.

**Tags**: `#privacy`, `#open source`, `#CLI tool`, `#security incident`, `#xAI`

---

<a id="item-9"></a>
## [Kaiser Nurses: AI and Surveillance Undermining Care Quality](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

Kaiser Permanente nurses report that AI-powered workplace surveillance tools, including call-center metrics and empathy scoring, are harming patient care and increasing job stress. Community commenters note that the core problems stem from misuse of metrics rather than AI itself, and some AI tools like medical LLMs are beneficial. This debate highlights real-world tensions between AI-based efficiency metrics and healthcare quality, affecting millions of patients and healthcare workers. The outcome could influence how healthcare organizations deploy AI surveillance and whether patient care is prioritized over cost savings. The article mentions an AI empathy pilot that was discontinued in 2024, and nurses are penalized for giving more than three pieces of advice per call. Some commenters note that AI tools for translation and note-taking actually improve care, but metric-driven pressure to minimize call times reduces quality.

hackernews · gnabgib · Jul 17, 22:26 · [Discussion](https://news.ycombinator.com/item?id=48952880)

**Background**: AI in healthcare call centers is increasingly used to monitor performance and cost efficiency. Empathy scoring AI attempts to evaluate the emotional quality of patient interactions. Critics argue that such metrics can incentivize rushed care and penalize thoroughness, while proponents highlight AI's potential to reduce clinician burnout through automation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2025.1680552/full">Empathy AI in healthcare - Frontiers</a></li>
<li><a href="https://bmjopen.bmj.com/content/16/6/e118515">Impact of artificial intelligence integrations on empathy in healthcare ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that metric misuse is the real issue, not AI itself. Some share positive experiences with AI tools that aid documentation and translation, while others criticize the empathy scoring concept. A few commenters highlight a cycle of insurers and providers both using AI to justify billing, which ultimately harms patients.

**Tags**: `#AI`, `#healthcare`, `#workplace surveillance`, `#ethics`, `#Kaiser`

---

<a id="item-10"></a>
## [Zilog Z80 Microprocessor Celebrates 50th Anniversary](https://goliath32.com/blog/z80.html) ⭐️ 7.0/10

A blog post and community comments celebrate the 50th anniversary of the Zilog Z80 microprocessor, reflecting on its profound impact on early personal computing and assembly programming. The Z80 was a cornerstone of the home computer revolution, powering iconic systems like the ZX Spectrum and TRS-80, and its longevity in embedded systems underscores its engineering legacy. Designed by Zilog and released in 1976, the Z80 is binary compatible with the Intel 8080 but uses a different flag register behavior, and it introduced new instructions not found in the 8080.

hackernews · st_goliath · Jul 17, 19:41 · [Discussion](https://news.ycombinator.com/item?id=48951461)

**Background**: The Zilog Z80 is an 8-bit microprocessor that played a crucial role in the late 1970s and 1980s home computer era. It was designed by former Intel engineers and offered a superset of the 8080 instruction set, making it easier to integrate into systems. Its low cost and high performance led to widespread adoption in computers, game consoles, and embedded devices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zilog_Z80">Zilog Z80 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zilog">Zilog - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters fondly recalled learning assembly programming on Z80-based machines like the TRS-80 and ZX-81, with some noting technical nuances such as the flag register differences between the Z80 and 8080. The discussion reflects deep nostalgia and appreciation for the CPU's role in their early computing experiences.

**Tags**: `#Z80`, `#microprocessor`, `#retrocomputing`, `#vintage hardware`, `#history`

---

<a id="item-11"></a>
## [Julia Evans' practical SQLite tips: .expert and backups](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 7.0/10

Julia Evans published a blog post sharing practical tips for running SQLite, including using the .expert command for automatic index recommendations and efficient backup strategies like piping .dump through zstd compression. These tips help developers and database administrators optimize SQLite performance and backups, which is crucial for lightweight applications and embedded systems. The high community engagement reflects the demand for practical SQLite advice. The .expert command analyzes SQL queries and suggests indexes to improve performance. For backups, using .dump piped through zstd with --rsyncable produces compressed dumps that are easy to sync and don't block writers when SQLite uses WAL mode.

hackernews · surprisetalk · Jul 17, 17:45 · [Discussion](https://news.ycombinator.com/item?id=48950122)

**Background**: SQLite is a popular embedded SQL database engine that runs in-process, commonly used in mobile apps and small websites. The .expert command, available in the SQLite CLI, provides index recommendations based on query analysis. WAL (Write-Ahead Log) mode allows concurrent reads and writes, making live backups safer. Understanding these tools helps users get more out of SQLite without migrating to heavier databases.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/cli.html">Command Line Shell For SQLite</a></li>
<li><a href="https://oldmoe.blog/2024/04/30/backup-strategies-for-sqlite-in-production/">Backup strategies for SQLite in production – Oldmoe's blog</a></li>
<li><a href="https://sqliteexpert.com/">SQLite administration | SQLite Expert</a></li>

</ul>
</details>

**Discussion**: Commenters shared alternative backup methods, such as Simon Willison's s3-credentials tool for scoped AWS credentials and ZFS snapshots for point-in-time consistency. Some debated using PostgreSQL for complex queries, while others recommended batch deletion for large DELETE operations. Overall, the discussion added valuable practical insights.

**Tags**: `#SQLite`, `#database administration`, `#backup`, `#performance tuning`, `#developer tools`

---

<a id="item-12"></a>
## [Honeypot Live: Real-Time SSH Bot Interaction Visualization](https://honeypotlive.cc/) ⭐️ 7.0/10

A new website, honeypotlive.cc, visualizes SSH honeypot interactions in real time, showing actual bot commands and behaviors. This provides a unique window into automated cyberattacks, helping security researchers and enthusiasts understand common attack patterns and the scale of internet background noise. The site appears to be a live feed from a low-interaction SSH honeypot; however, some users have abused the web interface to spam large amounts of text, obscuring real bot activity.

hackernews · tusksm · Jul 17, 14:05 · [Discussion](https://news.ycombinator.com/item?id=48947548)

**Background**: An SSH honeypot is a fake SSH server designed to attract and log malicious login attempts. Low-interaction honeypots simulate a limited set of services without allowing full access, while high-interaction ones allow attackers to interact more freely for deeper analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://securehoney.net/">Secure Honey | SSH Honeypot</a></li>
<li><a href="https://github.com/jaksi/sshesame">GitHub - jaksi/sshesame: An easy to set up and use SSH honeypot, a fake ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed reactions: some found the project interesting and timely, but others noted immediate spam abuse of the web interface. There was also mention of a related honeypot project using LLMs, and general appreciation for the visibility into background noise on public IPs.

**Tags**: `#security`, `#honeypot`, `#SSH`, `#visualization`, `#cybersecurity`

---

<a id="item-13"></a>
## [Project Orion Nuclear Pulse Rocket Revisited](https://mceglowski.substack.com/p/more-bounce-to-the-ounce) ⭐️ 7.0/10

A Substack article re-examining Project Orion, the 1950s nuclear pulse propulsion concept, sparked a detailed Hacker News discussion comparing it to alternatives like NERVA. This discussion brings renewed attention to historical nuclear rocket concepts, highlighting their potential for interplanetary travel and the technical and political challenges that led to their abandonment. Commenters noted that NERVA and its Soviet counterpart RD-0410 reached ground test prototype stages, unlike Orion which remained conceptual, and raised concerns about delivering nuclear charges into a blast zone.

hackernews · pavel_lishin · Jul 17, 13:32 · [Discussion](https://news.ycombinator.com/item?id=48947201)

**Background**: Project Orion was a U.S. study in the 1950s-60s for a spacecraft propelled by nuclear explosions behind a pusher plate. It was abandoned partly due to the 1963 Partial Test Ban Treaty. NERVA was a nuclear thermal rocket program that successfully tested engines. Both represent different approaches to nuclear propulsion.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Orion_(nuclear_propulsion)">Project Orion (nuclear propulsion)</a></li>
<li><a href="https://en.wikipedia.org/wiki/NERVA">NERVA - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nuclear_pulse_propulsion">Nuclear pulse propulsion - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters generally agreed that NERVA was more practical, with one stating it 'was much more practical and plausible' than Orion. Another questioned the logistics of delivering bombs into a nuclear blast, calling it an 'implementation detail.' Some referenced the concept's appearance in Neal Stephenson's novel 'Anathem.'

**Tags**: `#space propulsion`, `#nuclear rockets`, `#Project Orion`, `#engineering history`, `#NERVA`

---

<a id="item-14"></a>
## [Mermaid Diagrams Rendered as Colorful ASCII Art in Browser via WebAssembly](https://simonwillison.net/2026/Jul/16/mermaid-ascii/#atom-everything) ⭐️ 7.0/10

Simon Willison compiled the AlexanderGrooff/mermaid-ascii Go library to WebAssembly, creating an in-browser tool that renders Mermaid diagram source into ASCII/Unicode box-drawing art with color support. This tool provides developers with a lightweight, client-side way to preview Mermaid diagrams as ASCII art directly in the browser, enabling quick sharing and embedding without server dependencies. It also demonstrates the cross-language compilation pattern of Go to WebAssembly, expanding the ecosystem of web tools. The tool supports 22 diagram types and includes color rendering via ANSI escape codes or Unicode box-drawing characters. Users can adjust padding, box padding, and toggle ASCII-only mode. It also offers "Copy as text" and "Copy link to this diagram" features.

rss · Simon Willison · Jul 16, 14:57

**Background**: Mermaid is a popular JavaScript-based diagramming tool that uses a Markdown-like syntax to define flowcharts, sequence diagrams, and more. ASCII art rendering of these diagrams is useful for terminal display or inclusion in plain-text environments. WebAssembly (Wasm) allows code written in languages like Go to run in the browser at near-native speed, enabling reuse of existing libraries without rewriting them in JavaScript.

<details><summary>References</summary>
<ul>
<li><a href="https://tools.simonwillison.net/mermaid-ascii">Mermaid to ASCII art ( mermaid - ascii )</a></li>
<li><a href="https://pkg.go.dev/github.com/pgavlin/mermaid-ascii">mermaid - ascii command - github.com/pgavlin/ mermaid - ascii - Go ...</a></li>
<li><a href="https://go.dev/wiki/WebAssembly">Go Wiki: WebAssembly - The Go Programming Language</a></li>

</ul>
</details>

**Tags**: `#mermaid`, `#ascii`, `#webassembly`, `#tool`, `#developer-tools`

---

<a id="item-15"></a>
## [Recurse Center Founder Thanks HN for 15 Years of Support](https://news.ycombinator.com/item?id=48949551) ⭐️ 6.0/10

The founder of the Recurse Center posted a heartfelt retrospective on Hacker News, thanking the community for 15 years of support that helped launch and sustain the free self-directed programming retreat. This news underscores how community platforms like Hacker News can catalyze meaningful, non-commercial educational initiatives that have a lasting impact on thousands of programmers. The Recurse Center has hosted over 3,000 participants since 2010, operating as a free retreat funded by a built-in recruiting agency. Paul Graham's prescient comment at launch noted it might not be a billion-dollar business but is a benevolent endeavor.

hackernews · nicholasjbs · Jul 17, 16:57

**Background**: The Recurse Center (originally Hacker School) is a self-directed, community-driven educational retreat for programmers in New York City. It has no fixed curriculum; participants work on their own projects and help each other improve. The program is free because an integrated recruiting agency charges companies to hire alumni, ensuring no cost to participants.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recurse_Center">Recurse Center - Wikipedia</a></li>
<li><a href="https://www.recurse.com/">The Recurse Center</a></li>
<li><a href="https://www.ycombinator.com/companies/recurse-center">Recurse Center : The retreat where curious programmers recharge...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed gratitude and shared personal stories of attending the Recurse Center, praising its impact on their careers. Some discussed the social rules and the free funding model, while others thanked HN for its role in their own lives.

**Tags**: `#programming community`, `#hacker news`, `#recurse center`, `#education`, `#retrospective`

---

<a id="item-16"></a>
## [LLM Cliché Highlighter Spots AI Writing Patterns](https://simonwillison.net/2026/Jul/17/llm-cliche-highlighter/#atom-everything) ⭐️ 6.0/10

Simon Willison launched a web app that highlights ten common clichéd phrases frequently appearing in LLM-generated text, such as 'no fluff, no filler, no jargon.' The tool was built using vibe coding via Fable 5. As LLM-generated content proliferates, this tool helps readers detect AI-authored text by flagging repetitive patterns, promoting more critical consumption of online writing. It also highlights the growing need for transparency and authenticity in AI-assisted content creation. The tool targets ten specific cliché patterns common in LLM outputs, including 'no X, no Y' chains and other repetitive structures. It is a simple web-based highlighter that requires no installation—users just paste text into the analyzer.

rss · Simon Willison · Jul 17, 12:11

**Background**: Vibe coding, a term coined by Andrej Karpathy in February 2025, refers to AI-assisted software development where developers describe a project in a prompt and the LLM generates the code. This approach lowers the barrier for non-programmers but raises concerns about code quality and maintainability. The LLM cliché highlighter is a demonstration of how vibe coding can quickly produce useful tools.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_code">Vibe code</a></li>

</ul>
</details>

**Tags**: `#tools`, `#ai`, `#generative-ai`, `#llms`

---

<a id="item-17"></a>
## [New Tool Renders Mermaid Diagrams as Unicode Box Art via WASM](https://simonwillison.net/2026/Jul/16/grok-mermaid/#atom-everything) ⭐️ 6.0/10

Simon Willison extracted a Rust-based terminal renderer for Mermaid diagrams from the open-sourced Grok CLI and compiled it to WebAssembly, creating a browser tool that converts Mermaid text to Unicode box art. This demonstrates practical reuse of a specialized Rust component in the browser via WebAssembly, enabling terminal-style diagram rendering without external dependencies. It expands the accessibility of Mermaid diagrams to plain-text environments. The tool was built using a prompt in Claude Code for web (Fable 5), and the original Rust code was found in the xai-grok-markdown crate. The output uses Unicode box-drawing characters (U+2500–U+257F) to create flowcharts and other diagrams.

rss · Simon Willison · Jul 16, 00:33

**Background**: Mermaid is a popular open-source diagramming tool that uses text-based syntax to generate charts. Unicode box-drawing characters are a set of symbols used in text user interfaces to draw geometric frames and boxes, commonly seen in terminal applications.

<details><summary>References</summary>
<ul>
<li><a href="https://mermaid.js.org/">Mermaid | Diagramming and charting tool</a></li>
<li><a href="https://en.wikipedia.org/wiki/Box-drawing_characters">Box -drawing characters - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#mermaid`, `#unicode`, `#webassembly`, `#tools`

---