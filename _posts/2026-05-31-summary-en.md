---
layout: default
title: "Horizon Summary: 2026-05-31 (EN)"
date: 2026-05-31
lang: en
---

> From 44 items, 14 important content pieces were selected

---

1. [vLLM v0.22.0 Released with DeepSeek V4 and Rust Frontend](#item-1) ⭐️ 9.0/10
2. [Accenture to Acquire Ookla for $1.2 Billion](#item-2) ⭐️ 8.0/10
3. [Zig's ELF Linker Advances Towards C Replacement](#item-3) ⭐️ 8.0/10
4. [Openrsync becomes default rsync in macOS 15.0](#item-4) ⭐️ 8.0/10
5. [How Anthropic Sandboxes Claude Across Products](#item-5) ⭐️ 8.0/10
6. [Anthropic's run-rate revenue hits $47 billion](#item-6) ⭐️ 8.0/10
7. [SoftBank to Invest €75B in French AI Data Centers](#item-7) ⭐️ 8.0/10
8. [Domain expertise, not AI tools, is the real advantage](#item-8) ⭐️ 7.0/10
9. [Voxel Space Rendering Technique Demystified](#item-9) ⭐️ 7.0/10
10. [Python ASGI Apps Run in Browser via Pyodide + Service Worker](#item-10) ⭐️ 7.0/10
11. [Datasette 1.0a31 adds write queries and stored queries](#item-11) ⭐️ 7.0/10
12. [Nvidia-Powered Windows PC Debuts Next Week](#item-12) ⭐️ 7.0/10
13. [Pandoc Templates Directory Offers Community-Curated Resources](#item-13) ⭐️ 6.0/10
14. [Chad Whitacre Retires from Tech to Live Offline](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [vLLM v0.22.0 Released with DeepSeek V4 and Rust Frontend](https://github.com/vllm-project/vllm/releases/tag/v0.22.0) ⭐️ 9.0/10

vLLM v0.22.0 has been released with 459 commits from 230 contributors, introducing major improvements for DeepSeek V4 including NVFP4 fused MoE and MTP speculative decoding, advancing Model Runner V2 toward default, and adding an experimental Rust frontend. This release significantly enhances the efficiency and scalability of LLM inference, especially for DeepSeek V4 models, and the experimental Rust frontend points to future performance improvements. The maturation of Model Runner V2 will benefit all vLLM users with cleaner and faster execution. DeepSeek V4 now has a dedicated package, NVFP4 fused MoE support, full and piecewise CUDA graph, and MTP speculative decoding. Model Runner V2 adds an oracle that selects it for Qwen3 dense models by default and sleep-mode weight reload, with auto-fallback to MRv1 when a KV connector is present.

github · khluu · May 29, 10:28

**Background**: vLLM is a high-throughput and memory-efficient inference engine for large language models. DeepSeek V4 is a MoE architecture, and NVFP4 is a quantization format. MTP (Multi-Token Prediction) is a speculative decoding technique. Model Runner V2 is a ground-up redesign of vLLM's model runner for better modularity and performance.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>
<li><a href="https://deepwiki.com/vllm-project/vllm/7.4-moe-quantization-and-backend-selection">MoE Quantization and Backend Selection | vllm-project/vllm ...</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#DeepSeek V4`, `#Rust frontend`, `#Model Runner V2`

---

<a id="item-2"></a>
## [Accenture to Acquire Ookla for $1.2 Billion](https://newsroom.accenture.com/news/2026/accenture-to-acquire-ookla-to-strengthen-network-intelligence-and-experience-with-data-and-ai-for-enterprises) ⭐️ 8.0/10

Accenture announced its intent to acquire Ookla, the company behind Speedtest and Downdetector, for $1.2 billion, aiming to strengthen its network intelligence and data capabilities for enterprises. This acquisition combines Accenture's consulting scale with Ookla's massive network data from millions of consumer tests, potentially reshaping how telecoms and enterprises optimize 5G and Wi-Fi networks. It also raises concerns about data privacy and trust, as a consulting firm serving telcos now controls independent network monitoring tools. Ookla collects over 250 million consumer-initiated tests per month and serves almost every major telco through its data subscription programs. The deal includes Ookla's full portfolio: Speedtest, Downdetector, Ekahau, and RootMetrics.

hackernews · Garbage · May 30, 16:28 · [Discussion](https://news.ycombinator.com/item?id=48337987)

**Background**: Ookla's Speedtest is a widely used internet speed measurement tool, and Downdetector tracks service outages for websites and apps. Their primary revenue comes from selling aggregated network performance data to telecom operators, who use it to inform infrastructure investments. Accenture is a global professional services firm offering strategy, consulting, and technology services.

**Discussion**: Community members expressed skepticism about the deal's value, noting that Ookla's core products are technically straightforward, and the real value lies in its data business. Some raised trust concerns, questioning whether Downdetector would remain impartial when owned by a consulting firm that also advises the companies being monitored.

**Tags**: `#acquisition`, `#network intelligence`, `#Accenture`, `#Ookla`, `#data privacy`

---

<a id="item-3"></a>
## [Zig's ELF Linker Advances Towards C Replacement](https://ziglang.org/devlog/2026/#2026-05-30) ⭐️ 8.0/10

The Zig language team has made significant improvements to its ELF linker, bringing it closer to serving as a drop-in replacement for C with fast incremental compilation and high performance. These changes are documented in the latest devlog. These linker enhancements are crucial for Zig's goal of enabling rapid development iteration akin to interpreted languages while maintaining C-level performance. This could expand Zig's adoption beyond niche systems programming into broader application development. The improvements focus on incremental linking, which speeds up the edit-compile-test cycle significantly. Notably, incremental linking may be mutually exclusive with link-time optimization (LTO), so developers would use it for development builds and full LTO for release builds.

hackernews · kristoff_it · May 30, 17:29 · [Discussion](https://news.ycombinator.com/item?id=48338673)

**Background**: The ELF (Executable and Linkable Format) is the standard binary format for executables and shared libraries on Linux and many Unix-like systems. A linker combines object files into a final executable or library; faster linking reduces development wait times. Zig has been developing its own linker to replace the LLVM LLD linker, aiming for better performance and integration with Zig's build system.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ziglang/zig/issues/8755">zig ld: a drop-in linker replacement · Issue #8755 · ziglang/zig</a></li>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about Zig's linker progress, with one user noting it makes Zig a viable C replacement with iteration speed like Python or JavaScript. Another developer building a memory-safe language that transpiles to Zig praised the build system. Some questioned whether incremental linking is compatible with LTO, and others discussed potential use cases like porting Raku's VM from C to Zig.

**Tags**: `#Zig`, `#linker`, `#programming languages`, `#systems programming`, `#ELF`

---

<a id="item-4"></a>
## [Openrsync becomes default rsync in macOS 15.0](https://github.com/kristapsdz/openrsync) ⭐️ 8.0/10

Openrsync, a BSD-licensed reimplementation of rsync by the OpenBSD team, has been adopted as the default rsync utility in macOS 15.0, replacing the original GPL-licensed rsync. This matters because rsync is a critical tool for file synchronization and backups; its adoption in macOS signals growing trust in security-focused, permissively licensed implementations and may encourage wider use across other platforms. Openrsync is developed by Kristaps Dzonsons and emphasizes code correctness and security. Some users report minor incompatibilities, such as with the --rsync-path option creating unexpected directory structures.

hackernews · sph · May 30, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48334854)

**Background**: rsync is a widely used utility for efficiently transferring and synchronizing files across systems, commonly used for backups and mirroring. OpenBSD is known for its proactive security and code auditing. Openrsync is a clean-room implementation under a BSD license, avoiding the GPL license of the original rsync, which may appeal to commercial users and projects.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Openrsync">Openrsync</a></li>
<li><a href="https://github.com/kristapsdz/openrsync">GitHub - kristapsdz/openrsync: BSD-licensed implementation of rsync</a></li>
<li><a href="https://www.openrsync.org/">OpenRsync</a></li>

</ul>
</details>

**Discussion**: Users have positive experiences with openrsync, noting improvements over time. However, some report behavioral differences, like the --rsync-path issue described by one user. Others mention alternative implementations, such as a Go version by the Gokrazy team, and express hope that openrsync will fully replace the original rsync.

**Tags**: `#openrsync`, `#openbsd`, `#rsync`, `#utility`, `#security`

---

<a id="item-5"></a>
## [How Anthropic Sandboxes Claude Across Products](https://simonwillison.net/2026/May/30/how-we-contain-claude/#atom-everything) ⭐️ 8.0/10

Anthropic published a detailed engineering blog explaining how they sandbox Claude across Claude.ai, Claude Code, and Claude Cowork using gVisor, Seatbelt, Bubblewrap, and full virtual machines. The post also discloses a previously missed exfiltration vector via the /v1/files endpoint. As AI agents gain more autonomy, robust sandboxing is critical to prevent data exfiltration and misuse. Anthropic's transparency in documenting their security measures sets a precedent for the industry and addresses a common complaint about insufficient sandbox documentation. Claude.ai uses gVisor, an application kernel that intercepts Linux system calls in userspace. Claude Code uses Seatbelt on macOS and Bubblewrap on Linux for filesystem and process isolation. Claude Cowork runs full virtual machines—Apple's Virtualization framework on macOS and Windows Hypervisor Platform (HCS) on Windows.

rss · Simon Willison · May 30, 21:36

**Background**: Sandboxing is a security technique that restricts what resources an application can access. gVisor is an open-source container sandbox from Google that implements Linux syscalls in userspace using Go. Seatbelt is Apple's built-in sandbox framework for macOS, while Bubblewrap is a lightweight Linux sandbox using user namespaces. Anthropic also maintains an open-source Sandbox Runtime (srt) tool on GitHub.

<details><summary>References</summary>
<ul>
<li><a href="https://gvisor.dev/">The Container Security Platform - gVisor</a></li>
<li><a href="https://github.com/containers/bubblewrap">GitHub - containers/bubblewrap: Low-level unprivileged ...</a></li>
<li><a href="https://watchfire.io/docs/concepts/sandboxing">Sandboxing | Watchfire Docs</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#sandboxing`, `#Anthropic`, `#Claude`, `#security`

---

<a id="item-6"></a>
## [Anthropic's run-rate revenue hits $47 billion](https://simonwillison.net/2026/May/29/anthropic/#atom-everything) ⭐️ 8.0/10

Anthropic announced in its Series H announcement that its run-rate revenue has crossed $47 billion as of May 2026, up from $30 billion in April 2026 and $9 billion at the end of 2025. This rapid revenue growth highlights the accelerating adoption of AI in enterprise, positioning Anthropic as one of the fastest-growing companies in history and validating the market demand for large language models. Run-rate revenue is an annualized projection calculated by multiplying the most recent month's revenue by 12. Anthropic has disclosed these figures during fundraising announcements, where misrepresentation would constitute securities fraud.

rss · Simon Willison · May 29, 01:23

**Background**: Run-rate revenue is a financial metric that extrapolates current short-term revenue to estimate annual performance. It is commonly used by fast-growing companies to give investors a sense of trajectory, but it can be misleading if revenue is seasonal or not sustainable. Anthropic, an AI company behind the Claude model family, has been rapidly scaling its enterprise customer base.

<details><summary>References</summary>
<ul>
<li><a href="https://corporatefinanceinstitute.com/resources/accounting/revenue-run-rate/">Revenue Run Rate - Definition, Calculation, Examples</a></li>
<li><a href="https://www.investopedia.com/terms/r/runrate.asp">Run Rate Explained: Benefits, Risks, and Business Insights</a></li>

</ul>
</details>

**Discussion**: The article notes skepticism from some, like Ed Zitron who questioned the $30 billion figure, but the author argues the numbers are credible as they are disclosed in fundraising announcements where lying would be securities fraud. Some readers dismiss the figures as self-reported, but the author counters that the risk of legal consequences makes them trustworthy.

**Tags**: `#AI`, `#Anthropic`, `#revenue`, `#funding`, `#industry news`

---

<a id="item-7"></a>
## [SoftBank to Invest €75B in French AI Data Centers](https://www.investing.com/news/stock-market-news/softbank-to-invest-up-to-75-bln-in-french-ai-data-centers-4717783) ⭐️ 8.0/10

SoftBank announced plans to invest up to €75 billion in AI data centers in France, signaling a major push into European AI infrastructure. This massive investment underscores the growing importance of data center capacity for AI development and positions France as a key hub for AI infrastructure in Europe. The investment amount of €75 billion is one of the largest single commitments to AI infrastructure globally, though specific timelines and project details have not been disclosed.

rss · Investing.com All News · May 30, 20:42

**Background**: SoftBank is a Japanese multinational conglomerate known for its Vision Fund investments in technology companies. AI data centers require enormous capital expenditure for land, construction, and advanced computing hardware like GPUs. This investment reflects the race among nations and companies to build AI computing capacity.

**Tags**: `#AI`, `#data centers`, `#SoftBank`, `#investment`, `#infrastructure`

---

<a id="item-8"></a>
## [Domain expertise, not AI tools, is the real advantage](https://www.brethorsting.com/blog/2026/05/domain-expertise-has-always-been-the-real-moat/) ⭐️ 7.0/10

An opinion essay argues that domain expertise remains the true competitive advantage in software development, even as AI tools like vibe coding gain popularity. This perspective challenges the hype around AI replacing developers, emphasizing that deep domain knowledge is irreplaceable for building robust, useful software. The essay sparked over 129 comments, with many sharing real-world examples of domain experts struggling to build reliable software without engineering support.

hackernews · aaronbrethorst · May 30, 20:40 · [Discussion](https://news.ycombinator.com/item?id=48340411)

**Background**: Vibe coding is a term coined by Andrej Karpathy in February 2025, describing AI-assisted programming where developers accept AI-generated code with minimal review. The practice has sparked debate about the future of software engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>

</ul>
</details>

**Discussion**: Commenters generally agree that domain expertise alone is insufficient without software engineering skills. Some argue that the narrative around AI's impact keeps shifting, making it hard to know what truly matters.

**Tags**: `#AI`, `#domain expertise`, `#software engineering`, `#vibe coding`

---

<a id="item-9"></a>
## [Voxel Space Rendering Technique Demystified](https://s-macke.github.io/VoxelSpace/) ⭐️ 7.0/10

In 2017, a detailed article by s-macke explained the Voxel Space heightmap-based rendering technique used in the 1992 game Comanche, including a JavaScript demo and Python pseudocode. This article is significant because it preserves and explains an innovative rendering technique that allowed Comanche to render detailed terrain in real-time on 1992 hardware, influencing later game engines and inspiring modern implementations. Technically, Voxel Space is not true voxel rendering but a heightmap-based approach where each column is a prism. The core algorithm can be implemented in fewer than 20 lines of code.

hackernews · davikr · May 30, 14:25 · [Discussion](https://news.ycombinator.com/item?id=48336564)

**Background**: Voxel Space is a terrain rendering engine invented by Kyle Freeman at NovaLogic for the 1992 game Comanche: Maximum Overkill. It stores height values in a 2D grid and renders by scanning columns from far to near, achieving realistic terrain on low-end hardware. The engine was written entirely in x86 assembly for speed, and it was the first commercial use of voxel-like terrain in a flight simulator.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Voxel">Voxel - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Comanche_(video_game_series)">Comanche (video game series) - Wikipedia</a></li>
<li><a href="https://www.youtube.com/watch?v=bQBY9BM9g_Y">Voxel Space (Comanche Terrain Rendering) - YouTube Inspire » Voxel Space Comanche (video game series) - Wikipedia VoxelSpace - Simon Willison s-macke/VoxelSpace: Terrain Rendering Algorithm in Less Than ...</a></li>

</ul>
</details>

**Discussion**: Comments on the article noted that Voxel Space is technically a heightmap rather than true voxels (nine_k). Others shared fond memories of Comanche and linked to modern reimplementations in C++ and AGS (superjan, snickerer, a1o), reflecting the enduring interest in retro rendering techniques.

**Tags**: `#voxel-space`, `#rendering`, `#game-development`, `#retro-programming`, `#heightmap`

---

<a id="item-10"></a>
## [Python ASGI Apps Run in Browser via Pyodide + Service Worker](https://simonwillison.net/2026/May/30/pyodide-asgi-browser/#atom-everything) ⭐️ 7.0/10

Simon Willison demonstrated that Python ASGI applications can run entirely in the browser by using Pyodide (WebAssembly) combined with a service worker, replacing the previous web worker approach. This allows JavaScript in <script> tags to be executed, overcoming a key limitation of the earlier method. This innovation unlocks full support for Datasette plugins that rely on JavaScript, which were previously broken in Datasette Lite. It demonstrates a practical path for running complex Python web frameworks (like FastAPI, Starlette) entirely client-side, expanding the possibilities of serverless Python in the browser. The prototype uses Claude Opus 4.8 via Claude Code to refactor the code. A demo runs Datasette 1.0a31, and the source code is available on GitHub under simonw/research/pyodide-asgi-browser.

rss · Simon Willison · May 30, 21:02

**Background**: Pyodide is a port of CPython to WebAssembly, enabling Python execution in the browser without a server. ASGI (Asynchronous Server Gateway Interface) is a standard for Python async web apps, successor to WSGI. Datasette is a tool for exploring and publishing tabular data, and Datasette Lite is its browser-only version. Previously, Datasette Lite used Web Workers to run Python, but Web Workers cannot execute inline JavaScript, breaking some functionality.

<details><summary>References</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 0.29.4</a></li>
<li><a href="https://github.com/pyodide/pyodide">GitHub - pyodide/pyodide: Pyodide is a Python distribution ... Home - Pyodide pyodide | Pyodide is a Python distribution for the browser ... Online Python (Pyodide) - Run Python in Browser via WebAssembly Pyodide — Version 0.17.0 pyodide · PyPI</a></li>
<li><a href="https://en.wikipedia.org/wiki/ASGI">ASGI</a></li>

</ul>
</details>

**Tags**: `#Pyodide`, `#ASGI`, `#Service Workers`, `#WebAssembly`, `#Datasette`

---

<a id="item-11"></a>
## [Datasette 1.0a31 adds write queries and stored queries](https://simonwillison.net/2026/May/29/datasette/#atom-everything) ⭐️ 7.0/10

Datasette version 1.0a31 introduces two major features: the ability to execute write queries (insert, update, delete) and to save stored queries (renamed from 'canned queries') for private or shared use. This alpha release significantly expands Datasette's interactive database capabilities, making it useful for users who need to modify data directly through the web interface. It also enhances collaboration by allowing saved queries to be shared among instance members. Write queries are permission-controlled, allowing only users with the necessary permissions to execute inserts, updates, or deletes. The stored queries feature replaces the previous 'canned queries' and supports both private and public sharing within the Datasette instance.

rss · Simon Willison · May 29, 03:32

**Background**: Datasette is an open-source tool for exploring and publishing data as interactive websites and APIs. It is built on SQLite and allows users to run SQL queries on uploaded datasets. Prior to this release, Datasette only supported read-only queries, limiting its use for data entry or editing tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#sql`, `#database`, `#open-source`, `#alpha-release`

---

<a id="item-12"></a>
## [Nvidia-Powered Windows PC Debuts Next Week](https://www.investing.com/news/stock-market-news/first-windows-pc-powered-by-nvidia-chips-to-debut-next-week-axios-reports-4717762) ⭐️ 7.0/10

Microsoft and Nvidia have teased a major announcement expected to unveil the first Windows PC powered by Nvidia's custom Arm-based chip, likely the N1X, at Computex next week. This marks Nvidia's entry into the PC CPU market, challenging Intel and AMD's x86 dominance and potentially accelerating the adoption of Arm-based Windows PCs with superior AI and power efficiency. The Nvidia chip is rumored to be an Arm-based SoC developed in collaboration with MediaTek, featuring a 20-core CPU design for high-performance gaming laptops, and is expected to deliver twice the power efficiency of current x86 processors.

rss · Investing.com All News · May 30, 23:54

**Background**: Windows on Arm has historically been limited by software compatibility and performance, with Qualcomm holding a near-monopoly on Arm chips for Windows PCs. Nvidia's entry, backed by its GPU and AI expertise, could bring significant performance and efficiency gains, while Microsoft is positioning this as a 'new era of PC' with AI capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomsguide.com/computing/cpus/nvidia-n1x-cpu-everything-we-know-so-far">Nvidia N1X and N1 CPU: Everything we know so far - Tom's Guide</a></li>
<li><a href="https://www.forbes.com/sites/jonmarkman/2026/03/16/the-arm-invasion-nvidia-targets-200-billion-pc-market-with-n1x-chips/">The Arm Invasion: Nvidia Targets $200 Billion PC ... - Forbes</a></li>
<li><a href="https://www.pcmag.com/news/nvidia-microsoft-tease-is-arm-powered-windows-pc-chip-coming-computex-2026">Nvidia Joins Microsoft's Windows To Tease 'New Era of PC'</a></li>
<li><a href="https://www.windowscentral.com/hardware/surface/a-new-era-of-pc-microsoft-and-nvidia-tease-major-announcement-experts-predict-to-be-the-fabled-n1x-chip">"A new era of PC": Microsoft and NVIDIA tease major announcement experts predict to be the fabled N1X chip | Windows Central</a></li>
<li><a href="https://www.reddit.com/r/nvidia/comments/1m950a9/nvidias_arm_soc_hits_a_wall_microsofts_os_isnt/">r/nvidia on Reddit: NVIDIA’s ARM SoC Hits a Wall: Microsoft’s OS Isn’t Ready Yet</a></li>

</ul>
</details>

**Discussion**: On Reddit, users expressed excitement about Nvidia's potential in the PC CPU space but raised concerns about Microsoft's readiness for Windows on Arm, citing slow progress and compatibility issues. Some believe Nvidia's AI expertise could be a game-changer, while others remain skeptical about software ecosystem maturity.

**Tags**: `#Nvidia`, `#Windows PC`, `#hardware`, `#chip announcement`

---

<a id="item-13"></a>
## [Pandoc Templates Directory Offers Community-Curated Resources](https://pandoc-templates.org/) ⭐️ 6.0/10

A new website, pandoc-templates.org, serves as a directory of Pandoc templates for document conversion, providing users with easy access to community-contributed templates. This resource lowers the barrier for Pandoc users to create polished documents by offering ready-made templates, expanding the utility of Pandoc in academic and professional writing. The templates cover various output formats including PDF, HTML, and DOCX, and the website is explicitly stated as a community effort. Some users note that Pandoc's PDF generation can have issues with tables and Unicode fonts.

hackernews · ankitg12 · May 30, 09:56 · [Discussion](https://news.ycombinator.com/item?id=48334515)

**Background**: Pandoc is a versatile open-source document converter that can transform files between many markup formats. It is widely used for converting Markdown to PDF, Word, HTML, and more. Quarto, mentioned in comments, is another publishing system built on Pandoc that provides a more integrated experience.

<details><summary>References</summary>
<ul>
<li><a href="https://pandoc.org/">Pandoc - index</a></li>
<li><a href="https://quarto.org/">Quarto</a></li>

</ul>
</details>

**Discussion**: Commenters praise Pandoc's capabilities and the new template directory, with one user sharing their experience using Pandoc for a novel and GitHub Actions. Another user appreciates the variety of templates but notes past difficulties with PDF generation, including table layouts and font fallback. Some suggest Quarto as a more modern alternative.

**Tags**: `#pandoc`, `#markdown`, `#templates`, `#document-conversion`

---

<a id="item-14"></a>
## [Chad Whitacre Retires from Tech to Live Offline](https://simonwillison.net/2026/May/30/retiring-from-tech-to-live-offline/#atom-everything) ⭐️ 6.0/10

Chad Whitacre, known for his work on open source sustainability, announced he is retiring from tech and open source, citing AI as the final catalyst, and plans to live an offline life reminiscent of the 1980s. This personal decision highlights a growing unease among tech workers about AI's impact on human agency and culture, potentially signaling a broader trend of professionals stepping away from technology. Whitacre's retirement was announced via a typewritten, scanned letter, and he plans to be 'AI Amish' or 'Internet Amish,' accepting modern amenities like cars but rejecting AI and doomscrolling. He previously spent three 12-hour days using Claude Code with Opus 4.5, which he found intoxicating and unsettling.

rss · Simon Willison · May 30, 19:39

**Background**: Chad Whitacre is a prominent figure in the open source community, known for founding Gratipay and advocating for open source sustainability. The rise of generative AI has caused many in tech to question their relationship with technology, with some choosing to reduce digital exposure. Whitacre's concept of being 'AI Amish' draws a parallel to the Amish, who selectively adopt technology while preserving a simpler way of life.

**Tags**: `#tech retirement`, `#AI impact`, `#offline living`, `#open source`

---