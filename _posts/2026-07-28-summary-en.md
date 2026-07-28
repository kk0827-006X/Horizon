---
layout: default
title: "Horizon Summary: 2026-07-28 (EN)"
date: 2026-07-28
lang: en
---

> From 47 items, 8 important content pieces were selected

---

1. [vLLM v0.26.0: Inkling Support, DeepSeek-V4 Optimizations](#item-1) ⭐️ 9.0/10
2. [Moonshot AI Releases Kimi-K3 2.8 Trillion Parameter Weights](#item-2) ⭐️ 9.0/10
3. [Anthropic Advocates Mandatory Safety Testing for Open-Weights Models](#item-3) ⭐️ 8.0/10
4. [Python-build-standalone provides portable Python distributions used by uv](#item-4) ⭐️ 8.0/10
5. [Judge Rejects Google's DMCA Claim to Block Scraping](#item-5) ⭐️ 8.0/10
6. [React replaced by HTMX in forum software](#item-6) ⭐️ 8.0/10
7. [LLM Token Relay Market Exploits Free Trials and Stolen Credentials](#item-7) ⭐️ 8.0/10
8. [Ethan Mollick's guide shifts from chat to agentic AI](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0: Inkling Support, DeepSeek-V4 Optimizations](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 ships day-0 support for the Inkling 1T-parameter multimodal model family from Thinking Machines Lab, including novel architecture components like relative attention, short convolution, and shared expert sinks. It also delivers significant DeepSeek-V4 performance improvements across vendors, fp32 lm_head support, flexible attention backends, and matured KV offloading. This release marks a major milestone for open-source LLM inference, as vLLM now supports a cutting-edge 1T-parameter multimodal model on day zero, enabling efficient deployment of the latest architectures. The flexible attention backends and enhanced KV offloading improve support for hybrid models and long-context applications, benefiting the broader AI serving ecosystem. Inkling support includes base modeling, piecewise CUDA graphs, Hopper FA4 relative attention, MTP=1 speculative decoding, LoRA, and ModelOpt NVFP4 quantization. DeepSeek-V4 gains a specialized routing kernel (2.94% E2E TPOT improvement), fused_topk_bias (1.5–2x kernel), and redundant repeat/copy removal (1.8% E2E TPOT).

github · khluu · Jul 27, 01:06

**Background**: vLLM is a high-performance inference engine for large language models (LLMs), widely used for serving models in production. The Inkling model family from Thinking Machines Lab is a 1T-parameter multimodal model accepting text, image, and audio inputs with up to 1M context length. FlashAttention-4 (FA4) is an optimized attention kernel for Hopper GPUs, and NVFP4 is NVIDIA's 4-bit floating-point quantization format supported via ModelOpt.

<details><summary>References</summary>
<ul>
<li><a href="https://vllm.ai/blog/2026-07-15-inkling">TML Inkling on vLLM: Day-0 Support with Optimized Performance</a></li>
<li><a href="https://arxiv.org/html/2603.05451v1">FlashAttention-4: Algorithm and Kernel Pipelining Co-Design ...</a></li>
<li><a href="https://github.com/vllm-project/vllm/blob/main/vllm/models/inkling/nvidia/ops/fa4_rel_attention.py">vllm/vllm/models/inkling/nvidia/ops/fa4_rel_attention.py at ...</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#model optimization`, `#open-source release`, `#GPU performance`

---

<a id="item-2"></a>
## [Moonshot AI Releases Kimi-K3 2.8 Trillion Parameter Weights](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 9.0/10

Moonshot AI has released the weights for their 2.8 trillion parameter Kimi-K3 model on Hugging Face, weighing 1.56TB, under a new license that replaces the previous modified MIT license. The new license requires a separate agreement for large Model-as-a-Service businesses with over $20 million annual revenue. This release provides the open-weight community with one of the largest publicly available models, significantly advancing open AI research and competition. The licensing shift highlights ongoing tensions between openness and commercial control in the AI industry. The Kimi-K3 model has 2.8 trillion parameters and is available in FP16 format, requiring substantial hardware to run. The license explicitly requires large MaaS providers to enter a separate agreement with Moonshot, moving away from the 'modified MIT' label used for the earlier K2 model.

rss · Simon Willison · Jul 27, 23:39

**Background**: Moonshot AI is a Chinese company known for developing the Kimi line of large language models. In July 2025, they released Kimi-K2 under a modified MIT license that required attribution for large commercial entities. The new K3 license no longer calls itself modified MIT and imposes stricter commercial terms. Open-weight models release trained parameters but may not meet all Open Source Initiative definitions, as seen with this license.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(chatbot)">Kimi (chatbot) - Wikipedia</a></li>
<li><a href="https://localaimaster.com/models/kimi-k2">Kimi K 2 : 1T MoE Model (32B Active) — Local Setup... | Local AI Master</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Open Source`, `#Large Language Models`, `#Machine Learning`

---

<a id="item-3"></a>
## [Anthropic Advocates Mandatory Safety Testing for Open-Weights Models](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic published a position statement arguing against outright bans on open-weights AI models, instead calling for mandatory safety testing for all sufficiently capable models, both open and closed. Critics argue this stance effectively restricts open development by imposing costly or inaccessible testing requirements. As a leading AI company, Anthropic's policy stance could influence global AI regulation and the future of open-source AI. If adopted, mandatory safety testing may create barriers for small developers and researchers, potentially centralizing AI development among well-funded organizations. Anthropic's CEO Dario Amodei previously stated he does not regard bans as useful, yet the position supports banning chip sales to China and other measures, drawing accusations of hypocrisy. The statement does not specify who would conduct the safety tests or establish criteria, leaving implementation unclear.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open-weights AI models are models whose trained parameters (weights) are publicly released, allowing anyone to download, modify, and run them on their own hardware. This openness fosters innovation and accessibility but raises concerns about misuse, as the models can be used without oversight. The debate over regulating such models is central to AI safety policy, balancing openness with preventing harm.

<details><summary>References</summary>
<ul>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership - microsoft.com</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Discussion**: Community comments are highly critical, with users like cogman10 arguing that mandatory testing is effectively a ban due to cost and administrative barriers. Others point out contradictions in Anthropic's stance, such as supporting chip bans while claiming opposition to bans, and question the company's motives, suggesting it is protecting its own closed, expensive models.

**Tags**: `#AI safety`, `#open-weights`, `#AI policy`, `#artificial intelligence`, `#regulation`

---

<a id="item-4"></a>
## [Python-build-standalone provides portable Python distributions used by uv](https://gregoryszorc.com/docs/python-build-standalone/main/) ⭐️ 8.0/10

The python-build-standalone project produces self-contained, highly-portable Python distributions that are now the primary source of Python installations for many tools, including uv, pipx, Hatch, Poetry, and Bazel. These distributions simplify bundling Python into applications without requiring a system Python installation, making them critical for modern Python tooling and application distribution. The distributions include most standard library extension modules and are highly portable across platforms. Astral (the company behind uv) has taken over maintenance of the project, ensuring continued development.

hackernews · jcbhmr · Jul 27, 18:43 · [Discussion](https://news.ycombinator.com/item?id=49073942)

**Background**: Traditionally, Python applications required users to install Python separately, which could lead to version conflicts and complex setup. python-build-standalone provides fully self-contained Python builds that can be embedded directly into applications or downloaded on demand, eliminating dependency on a system Python. This approach is similar to how Rust's rustup manages toolchains.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/astral-sh/python-build-standalone">GitHub - astral-sh/ python - build - standalone : Produce redistributable...</a></li>
<li><a href="https://astral.sh/blog/python-build-standalone">A new home for python - build - standalone</a></li>
<li><a href="https://gregoryszorc.com/docs/python-build-standalone/main/">Python Standalone Builds — python - build - standalone documentation</a></li>

</ul>
</details>

**Discussion**: Community members, including charliermarsh (creator of uv) and simonw, praised the distributions for enabling easy Python bundling and noted that Astral now maintains the project. Others pointed to related projects like PyOxy for single-file executables and Cosmopolitan for cross-platform binaries, highlighting the broader ecosystem of portable Python solutions.

**Tags**: `#Python`, `#standalone`, `#portable`, `#distribution`, `#tooling`

---

<a id="item-5"></a>
## [Judge Rejects Google's DMCA Claim to Block Scraping](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

A federal judge rejected Google's attempt to use the Digital Millennium Copyright Act (DMCA) to prevent SerpAPI from scraping its search engine results pages. This ruling reaffirms that publicly accessible web data is generally free to scrape, which is vital for maintaining an open internet and for developers who rely on alternative search data access after Google deprecated its own search API. Google argued that its search results are copyrightable compilations and that scraping them violates the DMCA's anti-circumvention provisions, but the judge found the results lacked the minimal creativity required for copyright protection.

hackernews · cdrnsf · Jul 27, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49073513)

**Background**: The DMCA is a US copyright law that includes provisions against circumventing technological measures used to protect copyrighted works. Web scraping is the automated extraction of data from websites, a practice that has often been challenged legally. Google itself was built on crawling and indexing the open web, a fact that many see as ironic in this case.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eff.org/issues/dmca">DMCA | Electronic Frontier Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_scraping">Web scraping - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters widely noted the irony of Google using the DMCA to block scraping, given its own origins as a web crawler. Some criticized Google for removing its cheap search API while still opposing third-party scraping, calling it typical big company behavior that creates demand for the very activity it sues over.

**Tags**: `#legal`, `#web scraping`, `#Google`, `#DMCA`, `#copyright`

---

<a id="item-6"></a>
## [React replaced by HTMX in forum software](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 8.0/10

The Misago forum project removed React.js from its codebase and adopted HTMX for UI interactivity in 2023, detailed in a community discussion. This move reflects a growing trend away from heavy client-side frameworks toward simpler server-driven interactivity, reducing complexity and improving performance for content-focused websites. HTMX extends HTML with custom attributes for AJAX, WebSockets, and server-sent events, enabling dynamic partial updates without writing JavaScript. The discussion noted that for forum software, HTMX provides a lightweight alternative to SPAs.

hackernews · Ralfp · Jul 27, 09:58 · [Discussion](https://news.ycombinator.com/item?id=49067301)

**Background**: HTMX is an open-source JavaScript library that enables dynamic web pages using HTML attributes, following a hypermedia-driven approach. It sends HTTP requests for user actions and updates page regions with server responses, in contrast to client-side frameworks like React that use a virtual DOM.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>

</ul>
</details>

**Discussion**: Many commenters supported the switch, with some sharing practical experiences: James2doyle reported slow performance with large response payloads, while prologic uses HTMX for all web apps including PWAs. Others recommended alternatives like PyView for server-rendered interactivity.

**Tags**: `#HTMX`, `#React`, `#web development`, `#JavaScript frameworks`, `#server-side rendering`

---

<a id="item-7"></a>
## [LLM Token Relay Market Exploits Free Trials and Stolen Credentials](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

Matt Lenhard's investigation reveals a thriving relay market that resells LLM tokens at a discount by pooling API keys from free trials, stolen credentials, and chargeback attacks, primarily operating in China. This market poses significant risks for LLM vendors and developers, as it enables fraud, abuse of API keys, and potential model distillation, highlighting urgent need for better API security and cost controls. The proxies are built on open-source projects one-api and its fork new-api, legitimate tools that load-balance across pooled API credentials. Resellers offer discounts by exploiting unprotected support bots, stolen credit cards, or chargeback fraud.

rss · Simon Willison · Jul 26, 19:30

**Background**: LLM API providers like OpenAI charge per-token usage, and developers often set keys with limits. The relay market pools many keys to offer cheaper access, sometimes using fraudulent methods. Open-source API gateways such as one-api and new-api are designed for legitimate multi-model management but can be misused for this purpose.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/QuantumNous/new-api">GitHub - QuantumNous/new-api: A unified AI model hub for aggregation & distribution. It supports cross-converting various LLMs into OpenAI-compatible, Claude-compatible, or Gemini-compatible formats. A centralized gateway for personal and enterprise model management. 🍥</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#API security`, `#fraud`, `#proxy`, `#token reselling`

---

<a id="item-8"></a>
## [Ethan Mollick's guide shifts from chat to agentic AI](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 7.0/10

Ethan Mollick updated his opinionated AI guide, now focusing on agentic systems like ChatGPT Work and Claude Cowork that can autonomously perform hours of human work. This shift highlights a major industry trend from chat-based AI to autonomous agents, helping practitioners choose the right model for complex, multi-step tasks. The guide notes that Gemini is no longer listed because Google lacks a comparable Codex/ChatGPT Work/Cowork category. ChatGPT and Claude offer confusingly named modes like Work, Cowork, Codex, and Code, each with different capabilities.

rss · Simon Willison · Jul 27, 21:55

**Background**: Agentic AI refers to systems that can pursue goals, use tools, and take actions with limited human supervision. Earlier AI guides focused on chat interfaces, but newer models like GPT-4, Claude 4 Opus, and Gemini 2.5 Pro now support agentic capabilities beyond simple conversation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://chatgpt.com/ru-RU/work/">ChatGPT Work</a></li>

</ul>
</details>

**Tags**: `#AI`, `#agents`, `#opinion guide`, `#Ethan Mollick`

---