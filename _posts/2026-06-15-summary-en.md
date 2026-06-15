---
layout: default
title: "Horizon Summary: 2026-06-15 (EN)"
date: 2026-06-15
lang: en
---

> From 31 items, 9 important content pieces were selected

---

1. [US Government Orders Anthropic to Suspend Fable 5 and Mythos 5](#item-1) ⭐️ 9.0/10
2. [Rio LLM revealed as weighted merge of existing models](#item-2) ⭐️ 8.0/10
3. [Anthropic's Dual Role in AI Safety Questioned](#item-3) ⭐️ 8.0/10
4. [Jane Street on Formal Methods in AI-Assisted Programming](#item-4) ⭐️ 8.0/10
5. [Essay: AI Won't Replace Software Engineers](#item-5) ⭐️ 8.0/10
6. [WASM Python wheels now publishable to PyPI](#item-6) ⭐️ 8.0/10
7. [Kage Mirrors Websites into Single Offline Binary](#item-7) ⭐️ 7.0/10
8. [Zeroserve's Caddy compatibility boosts performance 3x, but lacks ACME](#item-8) ⭐️ 7.0/10
9. [Mapping SQLite Result Columns to Source Tables](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [US Government Orders Anthropic to Suspend Fable 5 and Mythos 5](https://simonwillison.net/2026/Jun/13/us-government-directive-to-suspend-access/#atom-everything) ⭐️ 9.0/10

The US government issued an export control directive citing national security concerns, ordering Anthropic to immediately suspend all access to its advanced AI models Fable 5 and Mythos 5 for all customers, including foreign national employees. This marks a landmark escalation in government intervention over AI safety, potentially setting a precedent for future regulation of advanced models based on unverified jailbreak claims. Anthropic stated the government's concern was based on a reported jailbreak technique that allowed the model to identify minor, previously known vulnerabilities—capabilities Anthropic argues are also available in other models like OpenAI's GPT-5.5.

rss · Simon Willison · Jun 13, 01:01

**Background**: Fable 5 is Anthropic's most capable model to date, state-of-the-art on many benchmarks. AI jailbreaking involves crafting inputs to bypass safety guardrails. The US government invoked national security export controls, despite Anthropic's objection and lack of specific details.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://aisecurityandsafety.org/en/guides/jailbreaking-attacks/">Jailbreaking AI Models: Attack Patterns, Examples & Defenses (2026)</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#national security`, `#Anthropic`, `#export controls`, `#jailbreak`

---

<a id="item-2"></a>
## [Rio LLM revealed as weighted merge of existing models](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

A GitHub issue reveals that the Rio-3.5-Open-397B model, presented as a homegrown fine-tune by the municipality of Rio de Janeiro, is actually a weighted merge of 60% Nex-N2 Pro and 40% Qwen3.5, with no additional training. This controversy highlights the importance of transparency and proper attribution in open-source AI development, as model merging can produce strong results without disclosure. The model's weight tensors are a 0.6/0.4 blend of Nex and Qwen across all 60 layers and components, and the claimed improvement may stem from on-policy distillation that was not included in the uploaded model.

hackernews · unrvl22 · Jun 14, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48528371)

**Background**: Model merging combines the weights of multiple trained models into a single model without additional training, using techniques like SLERP or TIES. It is a cost-effective alternative to joint training and can improve performance, but it raises issues of disclosure when presented as original work.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs - NVIDIA Developer</a></li>
<li><a href="https://sahilchachra.medium.com/merged-fine-tuned-a-case-study-on-qwen3-and-domain-fusion-192ffcdef6aa">Merged > Fine-Tuned? A Case Study on Qwen3 and Domain... | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters note that while model merging is a valid technique, the lack of disclosure is problematic. One user observes that the weights are a linear combination across all layers, which is unusual for fine-tunes and suggests a simple merge. Another expresses frustration about profiting from others' work without attribution.

**Tags**: `#AI`, `#open-source`, `#ethics`, `#model merging`, `#controversy`

---

<a id="item-3"></a>
## [Anthropic's Dual Role in AI Safety Questioned](https://www.verysane.ai/p/did-anthropic-ask-for-this) ⭐️ 8.0/10

A critical analysis compares Anthropic to a 'Doomsday Device Company' for promoting powerful AI while simultaneously advocating for regulation, highlighting a perceived contradiction in their AI safety stance. This critique challenges the credibility of Anthropic's safety advocacy, raising important questions about the ethics of AI development and the potential for corporate hypocrisy in the AI industry. The analysis, published on verysane.ai, garnered 99 comments and 132 points, indicating high engagement. It specifically likens Anthropic to a company that both sells doomsday devices and calls for their regulation.

hackernews · ad8e · Jun 14, 22:23 · [Discussion](https://news.ycombinator.com/item?id=48533504)

**Background**: Anthropic is an artificial intelligence company focused on safety research, founded by former OpenAI employees. The company has been vocal about the risks of AI and the need for regulation, while also developing powerful AI models like Claude. This analysis points out the potential contradiction in promoting powerful AI while warning about its dangers.

**Discussion**: Community comments reflect a mix of skepticism and nuanced views. Some commenters argue that Anthropic's leadership suffers from hubris and is detached from consequences, while others suggest that Anthropic genuinely believes in existential risks and is trying to steer regulation in a responsible manner.

**Tags**: `#AI safety`, `#Anthropic`, `#ethics`, `#regulation`, `#hubris`

---

<a id="item-4"></a>
## [Jane Street on Formal Methods in AI-Assisted Programming](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street published a blog post arguing that formal methods, such as type systems and proof assistants, are becoming essential for ensuring correctness in an era of AI-generated code. The post highlights their practical experience using formal techniques to improve verification and provide better feedback for AI development agents. As AI-assisted programming grows, the bottleneck shifts from writing code to verifying it; formal methods offer mathematically rigorous guarantees that complement testing. This could lead to more reliable software and change how developers and AI agents collaborate. The post is part of a series on formal methods at Jane Street, emphasizing that even lightweight formal techniques like strong type systems provide significant benefits for agentic programming. They note that more powerful proof techniques could further uplift AI-assisted development.

hackernews · eatonphil · Jun 14, 12:35 · [Discussion](https://news.ycombinator.com/item?id=48526633)

**Background**: Formal methods are mathematical approaches to specifying, developing, and verifying software, including type systems, model checking, and theorem proving. Historically, they were seen as difficult and time-consuming, but advances in automation and growing software complexity have revived interest. Jane Street uses formal methods in production, notably in their OCaml codebase, to improve reliability.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.janestreet.com/formal-methods-at-jane-street-index/">Jane Street Blog - Formal methods and the future of programming</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters shared mixed perspectives: some recalled early proof automation tools and the human effort required to guide theorem provers, while others praised modern expressive type systems for catching errors and improving AI agent behavior. A few questioned whether formal specs merely duplicate tests or code, but overall the discussion recognized formal methods as increasingly relevant with AI.

**Tags**: `#formal methods`, `#verification`, `#programming languages`, `#AI-assisted programming`, `#types`

---

<a id="item-5"></a>
## [Essay: AI Won't Replace Software Engineers](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

An essay by Arvind Narayanan and Sayash Kapoor argues that current data, including New York's WARN Act filings with zero AI-related layoffs, does not support the narrative that AI will cause mass unemployment among software engineers. 这挑战了当前关于AI导致岗位流失的主流炒作，尤其对最易受AI自动化影响的软件工程行业而言，暗示其他行业可能更具缓冲能力。 The essay identifies three real bottlenecks in software engineering: deciding what to build, verifying and being accountable for delivery, and deep human understanding of codebases, business, and environment.

rss · Simon Willison · Jun 14, 23:54

**Background**: The WARN Act (Worker Adjustment and Retraining Notification Act) is a U.S. law requiring employers with 100+ employees to give 60 days' notice of mass layoffs. In March 2025, New York added an AI disclosure checkbox to WARN filings; in its first year, not a single company checked it.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WARN_Act">WARN Act</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#employment`, `#automation`

---

<a id="item-6"></a>
## [WASM Python wheels now publishable to PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 8.0/10

Pyodide 314.0 and a PR to PyPI (merged April 21st) enable publishing Python packages built for WebAssembly (WASM) directly to PyPI using the new 'pyemscripten' platform tag defined in PEP 783. Maintainers can now build and upload WASM wheels just like native wheels. This eliminates the major bottleneck where Pyodide maintainers had to manually build and host over 300 packages, empowering the broader Python community to distribute WASM-compatible packages independently. It significantly expands the ecosystem of Python-in-the-browser tools and libraries. The new platform tag is 'pyemscripten_YYYY_P_wasm32', as specified in PEP 783. Author Simon Willison successfully published a 'luau-wasm' package as a proof of concept, which compiles the Luau scripting language (C++) to WASM and can be installed via micropip in Pyodide.

rss · Simon Willison · Jun 13, 23:55

**Background**: Pyodide is a WebAssembly-based Python runtime for the browser. Previously, packages with C/Rust extensions needed to be specially compiled to WASM, but there was no official way to distribute them via PyPI. PEP 783 standardized the 'pyemscripten' platform tag, and PyPI now accepts wheels with that tag.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/">Publishing WASM wheels to PyPI for use with Pyodide</a></li>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 - Emscripten Packaging | peps.python.org</a></li>

</ul>
</details>

**Tags**: `#Pyodide`, `#WASM`, `#PyPI`, `#Python`, `#WebAssembly`

---

<a id="item-7"></a>
## [Kage Mirrors Websites into Single Offline Binary](https://github.com/tamnd/kage) ⭐️ 7.0/10

Kage is a new open-source tool that clones any website into a single binary file for offline viewing by driving a real browser and stripping JavaScript. This simplifies offline access to web content, making it easy to share and version control entire websites without requiring a server or network connection. Kage uses a three-step process: clone, serve, and pack, with the pack step creating a single .zim file. It requires a separate serve process for viewing, though the author mentions potential for a standalone HTML entrypoint.

hackernews · tamnd · Jun 14, 17:25 · [Discussion](https://news.ycombinator.com/item?id=48529990)

**Background**: Traditional 'Save As' captures only static HTML and misses dynamically loaded content. Kage drives a real headless browser, captures the page as seen by a human, and makes it inert by stripping JavaScript, resulting in a faithful offline replica.

<details><summary>References</summary>
<ul>
<li><a href="https://kage.tamnd.com/">kage</a></li>
<li><a href="https://github.com/tamnd/kage">GitHub - tamnd/kage: Shadow any website for offline viewing, with the JavaScript stripped out · GitHub</a></li>

</ul>
</details>

**Discussion**: Community feedback is positive, with interest in use cases like offline company wikis and AI prototypes. Users reported issues with HTTP sites not resolving, and there is discussion about eliminating the need for a separate server process.

**Tags**: `#offline`, `#web-mirror`, `#binary`, `#tools`, `#open-source`

---

<a id="item-8"></a>
## [Zeroserve's Caddy compatibility boosts performance 3x, but lacks ACME](https://su3.io/posts/zeroserve-caddy-compat) ⭐️ 7.0/10

Zeroserve announced Caddy compatibility, achieving 3x throughput and 70% lower latency compared to Caddy, but the implementation does not include ACME automatic certificate management or plugin support. This demonstrates the potential of io_uring and eBPF in web servers, but the missing ACME support and security concerns around io_uring limit its practical usability for production environments. The performance claims are based on benchmarks comparing zeroserve with Caddy; however, zeroserve lacks ACME support and plugin compatibility, making it incompatible with Caddy's ecosystem, and the io_uring interface has been flagged for potential safety issues in network I/O.

hackernews · losfair · Jun 14, 13:43 · [Discussion](https://news.ycombinator.com/item?id=48527145)

**Background**: Zeroserve is a zero-configuration web server that uses eBPF scripting and io_uring for high performance. io_uring is a Linux kernel interface for asynchronous I/O, offering lower latency and higher throughput than traditional syscalls, but it has raised security concerns for network applications. ACME is the protocol used by Let's Encrypt to automate SSL/TLS certificate management, a critical feature for modern HTTPS servers.

<details><summary>References</summary>
<ul>
<li><a href="https://su3.io/posts/introducing-zeroserve">zeroserve: a zero-config web server you can script with eBPF</a></li>
<li><a href="https://en.wikipedia.org/wiki/Io_uring">io_uring - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Automatic_Certificate_Management_Environment">Automatic Certificate Management Environment - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members expressed disappointment over the missing ACME support, calling it a dealbreaker, and questioned the safety of using io_uring for network servers. Some also noted that nginx still holds up well in benchmarks despite being older technology.

**Tags**: `#performance`, `#web-server`, `#io-uring`, `#acme`, `#caddy`

---

<a id="item-9"></a>
## [Mapping SQLite Result Columns to Source Tables](https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/#atom-everything) ⭐️ 7.0/10

Simon Willison documented a research project using Claude Code to programmatically identify the source `table.column` for each result column in arbitrary SQL queries, including joins and CTEs. This capability could enable Datasette and other SQL analysis tools to display richer metadata about query results, improving data lineage understanding and debugging efficiency. Claude Code found three promising approaches: using the `apsw` library, using `ctypes` to call SQLite's `sqlite3_column_table_name()` C function, and parsing `EXPLAIN` output.

rss · Simon Willison · Jun 13, 23:05

**Background**: SQLite is a widely-used embedded database engine. When executing a query, SQLite internally tracks provenance of columns but does not expose it through the standard Python `sqlite3` module. Claude Code is Anthropic's AI coding agent that can understand codebases and assist with development tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#Datasette`, `#Query Analysis`, `#Column Provenance`, `#AI-assisted Programming`

---