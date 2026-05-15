---
layout: default
title: "Horizon Summary: 2026-05-15 (EN)"
date: 2026-05-15
lang: en
---

> From 46 items, 15 important content pieces were selected

---

1. [First public macOS kernel exploit on Apple M5 bypasses MTE](#item-1) ⭐️ 9.0/10
2. [vLLM 0.21.0 Released with Breaking Changes and New Backend](#item-2) ⭐️ 8.0/10
3. [Removing RAV4 Modem and GPS Stops Telemetry](#item-3) ⭐️ 8.0/10
4. [RTX 5090 eGPU on M4 MacBook Air: Gaming and LLM Breakthrough](#item-4) ⭐️ 8.0/10
5. [New Nginx Exploit with ASLR Bypass](#item-5) ⭐️ 8.0/10
6. [arXiv Bans Authors for AI-Hallucinated References](#item-6) ⭐️ 8.0/10
7. [HDD Firmware Hacking Deep Dive](#item-7) ⭐️ 8.0/10
8. [Amazonbot Finally Respects robots.txt](#item-8) ⭐️ 7.0/10
9. [AI Coding Agents Reduce Technology Lock-In Risk](#item-9) ⭐️ 7.0/10
10. [Criticizing '11 AI agents' as Meaningless Counting](#item-10) ⭐️ 7.0/10
11. [Anthropic's $1.5B Copyright Settlement Under Review](#item-11) ⭐️ 7.0/10
12. [Codex Now in ChatGPT Mobile App](#item-12) ⭐️ 6.0/10
13. [Mitchell Hashimoto: Programming languages are now fungible](#item-13) ⭐️ 6.0/10
14. [Datasette IP Rate-Limit Plugin 0.1a0 Released](#item-14) ⭐️ 6.0/10
15. [CSP Allow-list Experiment by Simon Willison](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [First public macOS kernel exploit on Apple M5 bypasses MTE](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

Calif disclosed the first public kernel memory corruption exploit for Apple's M5 chip, successfully bypassing the Memory Tagging Extension (MTE) security feature. This exploit demonstrates a significant security weakness in Apple's latest M5 chip, potentially affecting millions of macOS users and challenging the effectiveness of MTE as a mitigation. The exploit targets memory corruption in the macOS kernel and bypasses MTE, a hardware security feature designed to prevent such attacks. A 55-page report details the findings.

hackernews · quadrige · May 14, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48139219)

**Background**: Memory Tagging Extension (MTE) is an ARM hardware security feature that assigns tags to memory allocations to detect buffer overflows and use-after-free errors. Apple's M5 chip is the latest ARM-based SoC for Macs, succeeding the M4. This exploit is the first to demonstrate a practical bypass of MTE on Apple silicon.

<details><summary>References</summary>
<ul>
<li><a href="https://source.android.com/docs/security/test/memory-safety/arm-mte">Arm memory tagging extension | Android Open Source Project</a></li>
<li><a href="https://8ksec.io/arm64-reversing-and-exploitation-part-10-intro-to-arm-memory-tagging-extension-mte/">ARM64 Reversing Part 10: Intro to ARM MTE | 8kSec</a></li>
<li><a href="https://grokipedia.com/page/Apple_M5">Apple M5</a></li>

</ul>
</details>

**Discussion**: Commenters expressed a mix of awe and skepticism: some praised the technical achievement and speculated about bug bounty payouts (up to $1.5 million), while others questioned the lack of public technical details. A sarcastic comment compared the disclosure to fake vulnerabilities, and one user regretted buying the M5 for its security features.

**Tags**: `#macOS`, `#kernel exploit`, `#Apple M5`, `#memory corruption`, `#security`

---

<a id="item-2"></a>
## [vLLM 0.21.0 Released with Breaking Changes and New Backend](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

vLLM 0.21.0 has been released with 367 commits from 202 contributors. It deprecates transformers v4, requires C++20, integrates KV offload with Hybrid Memory Allocator, and introduces the TOKENSPEED_MLA attention backend for Blackwell GPUs. This is a significant release for the widely-used LLM inference library, introducing major performance and memory improvements. The breaking changes require migration efforts but enable support for newer hardware and larger models. The KV offloading subsystem now uses the Hybrid Memory Allocator with sliding window group support, improving memory efficiency. The TOKENSPEED_MLA backend leverages proprietary kernels for optimal performance on Blackwell GPUs with DeepSeek-R1/Kimi-K25 models.

github · khluu · May 14, 23:15

**Background**: KV cache offloading moves attention key-value data from GPU to CPU memory to free GPU resources. The Hybrid Memory Allocator reduces memory waste compared to fixed-block allocators. TOKENSPEED is a high-performance inference engine with optimized MLA kernels for Blackwell.

<details><summary>References</summary>
<ul>
<li><a href="https://bentoml.com/llm/inference-optimization/kv-cache-offloading">KV cache offloading | LLM Inference Handbook</a></li>
<li><a href="https://github.com/lightseekorg/tokenspeed">GitHub - lightseekorg/tokenspeed: TokenSpeed is a speed-of-light LLM inference engine. · GitHub</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM inference`, `#GPU`, `#transformers`, `#release`

---

<a id="item-3"></a>
## [Removing RAV4 Modem and GPS Stops Telemetry](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/) ⭐️ 8.0/10

A detailed guide was published on removing the cellular modem and GPS receiver from a 2024 Toyota RAV4 hybrid to prevent the vehicle from sending telemetry data to Toyota. This matters because modern cars increasingly collect and share driver data, often without explicit consent; the guide provides a practical DIY method for privacy-conscious owners to stop data transmission. After removing the modem, connecting a phone via Bluetooth still allows the car to use the phone's internet connection to send telemetry; however, using wired USB CarPlay does not trigger this behavior.

hackernews · arkadiyt · May 14, 17:08 · [Discussion](https://news.ycombinator.com/item?id=48138136)

**Background**: Modern vehicles contain a telematics control unit (TCU) with a cellular modem and GPS that continuously collect data such as location, speed, and driving behavior. This data is often shared with manufacturers and third parties, raising privacy concerns. Physical removal or disconnection of the TCU is one way to achieve an air-gapped vehicle that cannot transmit telemetry.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rav4world.com/threads/how-to-fully-disable-telemetry-and-have-an-air-gapped-car.343029/">How to fully disable telemetry and have an "air-gapped" car | Toyota RAV4 Forums</a></li>
<li><a href="https://en.wikipedia.org/wiki/Telemetry">Telemetry - Wikipedia</a></li>
<li><a href="https://disappearme.ai/blog/car-reporting-complete-guide-disabling-vehicle-telemetry-data-collection-2025">Disable Car Data Collection: Complete Brand-by-Brand Guide to Vehicle Telemetry</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Bluetooth connectivity after modem removal can still leak data via the phone, and that CarPlay itself collects vehicle telemetry. One user wanted to perform this modification to fix a GPS compass issue in CarPlay, which Toyota refused to address. Another pointed out that the 2024 Ford Maverick has a simple fuse removal option for its telematics unit.

**Tags**: `#privacy`, `#car telemetry`, `#Toyota RAV4`, `#DIY`, `#GPS`

---

<a id="item-4"></a>
## [RTX 5090 eGPU on M4 MacBook Air: Gaming and LLM Breakthrough](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 8.0/10

A developer successfully connected an NVIDIA RTX 5090 eGPU to an M4 MacBook Air, demonstrating functional gaming and significant improvements in LLM inference performance via a custom VM setup. This achievement challenges Apple's official stance that eGPUs are unsupported on Apple Silicon, opening new possibilities for Mac gaming and local AI workloads, particularly for users needing high GPU performance on a portable device. The setup relies on a virtual machine with GPU passthrough, bypassing macOS limitations; however, it is constrained by Apple's 1.5 GB memory window for DMA transfers. The eGPU dramatically accelerates LLM prompt prefill, a known bottleneck on Apple Silicon.

hackernews · allenleee · May 14, 15:47 · [Discussion](https://news.ycombinator.com/item?id=48137145)

**Background**: An eGPU (external GPU) connects a desktop graphics card to a laptop via Thunderbolt, typically boosting graphics performance. Apple officially supported eGPUs only for Intel-based Macs, and only with AMD cards. Apple Silicon Macs lack official eGPU support due to unified memory architecture. LLM inference involves two phases: prefill (prompt processing) and decode (token generation); prefill is memory-bandwidth intensive and often slow on Macs.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/en-us/102363">Use an external graphics processor with your Mac - Apple Support</a></li>
<li><a href="https://www.linkedin.com/pulse/external-graphics-processing-unit-egpu-real-world-5-uses-zpfff">External Graphics Processing Unit Egpu in the Real World: 5 Uses...</a></li>
<li><a href="https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/">Mastering LLM Techniques: Inference Optimization | NVIDIA Technical...</a></li>

</ul>
</details>

**Discussion**: Community reaction is highly positive, with praise for the technical achievement and practical implications for LLM workloads. Commenters note the workaround's complexity and express hope for official Apple support, while also highlighting the remaining 1.5 GB window limitation.

**Tags**: `#eGPU`, `#Apple Silicon`, `#Mac gaming`, `#RTX 5090`, `#LLM inference`

---

<a id="item-5"></a>
## [New Nginx Exploit with ASLR Bypass](https://github.com/DepthFirstDisclosures/Nginx-Rift) ⭐️ 8.0/10

A memory corruption exploit in nginx, named Nginx-Rift, has been disclosed that uses the rewrite and set directives, with a claimed ASLR bypass. As nginx powers a large portion of the web, this exploit poses a significant security risk, though mitigations like using named capture groups reduce its severity. The exploit requires specific preconditions: a rewrite directive with a question mark in the replacement string and a subsequent set directive referencing a regex capture group (e.g., set $var $1). The proof-of-concept assumes ASLR is disabled, but the writeup claims a reliable ASLR bypass exists.

hackernews · hetsaraiya · May 14, 17:17 · [Discussion](https://news.ycombinator.com/item?id=48138268)

**Background**: Nginx is a popular web server that uses directives like rewrite and set for URL manipulation. Rewrite rules can include regular expression capture groups (e.g., $1, $2) to capture parts of the URL. Named capture groups (e.g., $name) are an alternative that are not vulnerable to this exploit. ASLR (Address Space Layout Randomization) is a memory protection technique that randomizes memory addresses to make exploitation harder.

<details><summary>References</summary>
<ul>
<li><a href="https://www.digitalocean.com/community/tutorials/nginx-rewrite-url-rules">Nginx Rewrite URL Rules Examples | DigitalOcean</a></li>
<li><a href="https://nickjanetakis.com/blog/using-nginx-regex-capture-groups-to-redirect-url-paths">Using NGINX Regex Capture Groups to Redirect... — Nick Janetakis</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights that ASLR is a defense-in-depth mechanism and discounting the exploit because the POC disables ASLR is misguided. Commenters emphasize that the vulnerabilities are real and preconditions are significant, but F5 has released patches for versions 1.31.0 and 1.30.1.

**Tags**: `#nginx`, `#exploit`, `#security`, `#vulnerability`, `#ASLR`

---

<a id="item-6"></a>
## [arXiv Bans Authors for AI-Hallucinated References](https://twitter.com/tdietterich/status/2055000956144935055) ⭐️ 8.0/10

arXiv announced a new policy imposing a one-year ban on authors who submit papers containing hallucinated references, likely generated by AI, effective for future submissions. This policy directly addresses the growing problem of AI-generated slop polluting scientific literature, helping preserve academic integrity and trust in preprints. The ban lasts one year, after which authors must first have a paper accepted at a reputable peer-reviewed venue before resubmitting to arXiv. The policy targets easily detectable hallucinations, not honest errors.

hackernews · gjuggler · May 14, 20:39 · [Discussion](https://news.ycombinator.com/item?id=48140922)

**Background**: Hallucinated references are fabricated citations that appear real but do not exist, often generated by AI language models like ChatGPT. A Nature analysis found tens of thousands of publications from 2025 may contain such invalid references. arXiv, a free preprint repository, aims to curb this trend with punitive measures.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)">Hallucination (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://www.nature.com/articles/d41586-026-00969-z">Hallucinated citations are polluting the scientific literature. What can be done?</a></li>

</ul>
</details>

**Discussion**: The community broadly supports the policy, with comments like 'incredibly good for science' and 'forcing consequences on easily-detectable hallucinations can only be a good thing.' However, some commenters urge careful vetting before imposing bans and note the policy may not yet be live.

**Tags**: `#arXiv`, `#academic integrity`, `#AI hallucination`, `#scientific publishing`

---

<a id="item-7"></a>
## [HDD Firmware Hacking Deep Dive](https://icode4.coffee/?p=1465) ⭐️ 8.0/10

A detailed technical article series explains how to dump, reverse engineer, and modify HDD firmware, including using JTAG for live debugging and AI for analysis of unknown architectures. This work exposes serious firmware-level vulnerabilities in HDDs and SSDs, highlighting risks for security researchers and potential exploitation by threat actors. It also provides valuable techniques for data recovery and forensic analysis. The series covers live debugging via JTAG, modifying firmware, and using AI to classify unknown microcontroller architectures. The first part focuses on dumping and modifying firmware without AI, while later parts incorporate AI assistance.

hackernews · jsploit · May 14, 16:19 · [Discussion](https://news.ycombinator.com/item?id=48137553)

**Background**: Hard disk drive firmware is low-level software that controls the physical operation of the drive. Hacking this firmware can allow attackers to hide malicious code or alter drive behavior. Historically, researchers have demonstrated firmware-level attacks on both HDDs and SSDs, and techniques like JTAG debugging have been used to extract firmware.

<details><summary>References</summary>
<ul>
<li><a href="https://icode4.coffee/?p=1465">HDD Firmware Hacking Part 1 – I Code 4 Coffee</a></li>
<li><a href="https://malwaretech.com/2015/04/hard-disk-firmware-hacking-part-1.html">Hard Disk Firmware Hacking (Part 1)</a></li>
<li><a href="https://spritesmods.com/?art=hddhack&page=6">Sprites mods - Hard disk hacking - Software flashing</a></li>

</ul>
</details>

**Discussion**: Commenters shared related work, including decompilation of Samsung 840 EVO SSD firmware and a similar HDD hack that modified /etc/shadow passwords. Some referenced NSA firmware hacking capabilities, highlighting the real-world implications of such research.

**Tags**: `#firmware hacking`, `#HDD`, `#reverse engineering`, `#security`, `#hardware hacking`

---

<a id="item-8"></a>
## [Amazonbot Finally Respects robots.txt](https://xeiaso.net/notes/2026/amazonbot-respecting-robots-txt/) ⭐️ 7.0/10

Amazonbot, Amazon's web crawler, has started respecting robots.txt directives after previously ignoring them, as reported by users experiencing excessive traffic. This change is significant because many website operators had to block Amazonbot manually, consuming bandwidth and resources. It sets a precedent for AI crawlers to follow ethical scraping practices. The change was observed following user complaints about high traffic from Amazonbot, including violations of disallowed paths. Amazon appears to have updated the crawler behavior without a public announcement.

hackernews · xena · May 14, 20:22 · [Discussion](https://news.ycombinator.com/item?id=48140730)

**Background**: Robots.txt is a standard file that tells web crawlers which parts of a site they may access. While voluntary, many reputable bots follow it. Amazonbot is Amazon's crawler used for indexing search results and powering the Alexa AI assistant.

<details><summary>References</summary>
<ul>
<li><a href="https://datadome.co/bots/amazonbot/">What is Amazonbot ? How to block it ?</a></li>

</ul>
</details>

**Discussion**: Comments reveal that users have experienced massive data usage from Amazonbot, such as 750 GiB of traffic to public repos. Some users remain skeptical, noting that robots.txt is merely a gentleman's agreement and other AWS user agents continue to pose issues.

**Tags**: `#robots.txt`, `#web scraping`, `#Amazonbot`, `#AI crawlers`, `#Hacker News`

---

<a id="item-9"></a>
## [AI Coding Agents Reduce Technology Lock-In Risk](https://simonwillison.net/2026/May/14/not-so-locked-in/#atom-everything) ⭐️ 7.0/10

Simon Willison reflects on how AI coding agents lower the cost of rewriting software, making platform and language lock-in less of a concern. He highlights a company that used coding agents to rewrite their iPhone and Android apps to React Native, confident they could port back if needed, and references Bun's migration from Zig to Rust. This development matters because it reduces the strategic risk of choosing a particular technology stack, giving organizations more flexibility and the ability to adapt to future changes. It could accelerate adoption of newer languages and frameworks by lowering the switching cost. The React Native rewrite was driven by AI coding agents, and the company explicitly stated they could reverse the decision if needed. Mitchell Hashimoto's quote about Bun migrating from Zig to Rust underscores the broader trend that programming languages are no longer irreversible lock-in.

rss · Simon Willison · May 14, 22:53

**Background**: AI coding agents are tools that use large language models to assist in writing, refactoring, and rewriting code, often automating complex tasks. Technology lock-in refers to the difficulty and cost of switching away from a platform or language once it is deeply embedded in a project. React Native is a framework for building cross-platform mobile apps, while Bun is a JavaScript runtime that originally used Zig and is now being ported to Rust.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/jtorchia/bun-migrates-from-zig-to-rust-what-my-real-benchmarks-say-about-whether-it-matters-3fm7">Bun Migrates from Zig to Rust : What My Real... - DEV Community</a></li>
<li><a href="https://www.theregister.com/2026/05/05/bun_rust_port/">Anthrophic's Bun team trials port from Zig to Rust • The Register</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#React Native`, `#software engineering`, `#lock-in`, `#programming languages`

---

<a id="item-10"></a>
## [Criticizing '11 AI agents' as Meaningless Counting](https://simonwillison.net/2026/May/13/boris-mann/#atom-everything) ⭐️ 7.0/10

Boris Mann, a well-known figure in the tech community, criticized the phrase '11 AI agents' as meaningless, comparing it to counting spreadsheets or browser tabs without context. This critique highlights how the term 'AI agent' is often used vaguely in industry hype, potentially confusing discussions about AI capabilities and deployments. Mann's post on Bluesky received attention for its concise analogy, and it was shared by Simon Willison on his blog, adding to ongoing conversations about defining AI agents.

rss · Simon Willison · May 13, 16:15

**Background**: The term 'AI agent' has become popular in recent years, often used to describe autonomous software that can perform tasks. However, its meaning can vary widely, from simple chatbots to complex multi-step reasoning systems. Without clear definitions, phrases like '11 AI agents' obscure more than they clarify.

**Tags**: `#ai-agents`, `#ai`, `#terminology`, `#criticism`

---

<a id="item-11"></a>
## [Anthropic's $1.5B Copyright Settlement Under Review](https://www.investing.com/news/stock-market-news/us-judge-considers-anthropics-15-billion-settlement-of-authors-lawsuit-4690939) ⭐️ 7.0/10

A US judge is reviewing Anthropic's proposed $1.5 billion settlement to resolve a copyright infringement lawsuit filed by authors over the use of their works in training AI models. This settlement sets a major precedent for AI companies using copyrighted works for training, potentially influencing future litigation and licensing practices in the AI industry. The settlement amount is at least $1.5 billion, compensating creators whose copyrighted works were used without permission to train Anthropic's Claude AI model.

rss · Investing.com All News · May 14, 23:49

**Background**: Generative AI models like Claude require vast amounts of text data for training, often including copyrighted books. Authors have sued for copyright infringement, arguing that using their works without consent violates their rights. This case is among the first major settlements in such disputes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wvtf.org/2025-09-05/anthropic-settles-with-authors-in-first-of-its-kind-ai-copyright-infringement-lawsuit">Anthropic settles with authors in first-of-its-kind AI copyright ... | WVTF</a></li>
<li><a href="https://biz.chosun.com/en/en-it/2025/09/07/C3PX7HJJKJFXLLUAGJNLB5KWI4/">Anthropic settles AI copyright lawsuit , agrees to pay... - CHOSUNBIZ</a></li>

</ul>
</details>

**Tags**: `#AI`, `#litigation`, `#copyright`, `#Anthropic`, `#settlement`

---

<a id="item-12"></a>
## [Codex Now in ChatGPT Mobile App](https://openai.com/index/work-with-codex-from-anywhere/) ⭐️ 6.0/10

OpenAI has integrated its AI coding assistant Codex into the ChatGPT mobile app, making it available for free to all users who sign in with a ChatGPT account. This expands access to AI-assisted coding to mobile devices, allowing developers to work on code from anywhere, but mobile usability constraints may limit its effectiveness for complex tasks. Codex in the mobile app includes a remote control feature that connects to the desktop Codex app, but it does not include Codex Cloud or the CLI version. All interactions on the free plan may be used for training data.

hackernews · mikeevans · May 14, 20:06 · [Discussion](https://news.ycombinator.com/item?id=48140529)

**Background**: Codex is OpenAI's developer-focused AI assistant that can understand, generate, and modify code in dozens of programming languages. It runs on advanced GPT models and allows users to describe software in plain English to have the AI write the code and push it to GitHub. Previously, Codex was only available on desktop or via CLI.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/getting-started-openai-codex-tpms-diving-deep-guide-vibe-doron-katz-a5fdc">Getting Started with OpenAI Codex : A TPM’s Diving Deep Guide to...</a></li>
<li><a href="https://techglimmer.io/openai-codex-review-2026/">OpenAI Codex 2026: The New macOS App Turns AI into Your Coding ...</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some users are excited about free access to Codex, while others find mobile usage less effective due to screen size and lack of keyboard. Several users note limitations such as the absence of Linux CLI support and that the mobile version lacks Codex Cloud integration.

**Tags**: `#Codex`, `#ChatGPT`, `#mobile`, `#AI coding`, `#OpenAI`

---

<a id="item-13"></a>
## [Mitchell Hashimoto: Programming languages are now fungible](https://simonwillison.net/2026/May/14/mitchell-hashimoto/#atom-everything) ⭐️ 6.0/10

Mitchell Hashimoto, co-founder of HashiCorp, posted on Twitter that programming languages are increasingly fungible, citing Bun's quick rewrite from Zig to Rust as evidence that languages are no longer a lock-in. This observation challenges the traditional belief that choosing a programming language leads to long-term lock-in, suggesting that with modern tooling and AI assistance, migrating between languages can be done rapidly. It impacts how developers and companies evaluate language decisions for new projects. Bun is a JavaScript runtime originally written in Zig, and has been experimentally rewritten in Rust by its new owner Anthropic. Hashimoto claims the rewrite took roughly a week or two, highlighting the fungibility of languages.

rss · Simon Willison · May 14, 22:31

**Background**: Bun is a high-performance JavaScript runtime and toolkit designed as a drop-in replacement for Node.js, using JavaScriptCore engine. Zig is a systems programming language focused on simplicity and performance, often compared to C. Rust is a memory-safe systems language gaining popularity for performance-critical applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig ( programming language ) - Wikipedia</a></li>
<li><a href="https://www.stork.ai/blog/buns-rust-rewrite-the-betrayal-that-killed-zig">Bun 's Rust Rewrite : An Analysis of the Zig vs. Rust Debate | Stork.AI</a></li>

</ul>
</details>

**Tags**: `#programming-languages`, `#rust`, `#zig`, `#bun`, `#mitchell-hashimoto`

---

<a id="item-14"></a>
## [Datasette IP Rate-Limit Plugin 0.1a0 Released](https://simonwillison.net/2026/May/14/datasette-ip-rate-limit/#atom-everything) ⭐️ 6.0/10

Simon Willison released version 0.1a0 of datasette-ip-rate-limit, a plugin for Datasette that blocks aggressive crawlers by rate-limiting IP addresses. The plugin was built with assistance from OpenAI's Codex AI agent. This plugin addresses a common operational challenge for Datasette users facing abusive crawlers, making it easier to protect site performance without complex infrastructure. It also demonstrates practical use of AI-assisted development for real-world software tools. The plugin allows configurable rate-limiting rules per path, with a maximum of 10,000 tracked IPs and exempt paths for static files. In the production configuration, it limits certain demo database paths to 60 requests per 60-second window, blocking offending IPs for 20 seconds.

rss · Simon Willison · May 14, 04:10

**Background**: Datasette is an open-source Python tool for exploring and publishing structured data, often used to share datasets online. Rate limiting is a technique to control the number of requests a client can make in a given time period, preventing server overload. Codex is an AI coding agent by OpenAI, designed to automate software engineering tasks like writing features and fixing bugs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex ( AI agent) - Wikipedia</a></li>
<li><a href="https://faceprep.medium.com/what-is-codex-openais-latest-ai-coding-agent-3e487915d486">What is Codex ? OpenAI’s latest AI coding agent | by FACE... | Medium</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#rate-limiting`, `#python`, `#ai-assisted`

---

<a id="item-15"></a>
## [CSP Allow-list Experiment by Simon Willison](https://simonwillison.net/2026/May/13/csp-allow/#atom-everything) ⭐️ 6.0/10

Simon Willison built a tool that loads an app in a CSP-protected sandboxed iframe and intercepts fetch errors to prompt users to add blocked domains to an allow-list, then refreshes the page. This experiment demonstrates a novel user-friendly approach to managing Content Security Policy (CSP) restrictions without breaking functionality, potentially improving web security adoption by reducing friction. The tool uses a custom fetch() that intercepts CSP errors and passes them to the parent window, which then shows a dialog asking whether to add the origin to the connect-src allow-list. The implementation was built with GPT-5.5 xhigh in the Codex desktop app.

rss · Simon Willison · May 13, 04:50

**Background**: Content Security Policy (CSP) is a security standard that restricts which resources a web page can load, preventing cross-site scripting attacks. A sandboxed iframe has limited capabilities and can be used to isolate untrusted content. CSP violations typically result in blocked requests, which can break functionality; this experiment offers a way to dynamically update the policy based on user consent.

**Tags**: `#CSP`, `#web security`, `#sandbox`, `#iframe`, `#JavaScript`

---