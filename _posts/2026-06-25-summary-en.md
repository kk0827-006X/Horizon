---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 45 items, 18 important content pieces were selected

---

1. [OpenAI unveils first custom AI chip with Broadcom](#item-1) ⭐️ 9.0/10
2. [Krea 2: SOTA open-weights 12B image model](#item-2) ⭐️ 9.0/10
3. [Qualcomm Acquires Modular for $4 Billion](#item-3) ⭐️ 8.0/10
4. [Bunny DNS goes free, eliminates query fees](#item-4) ⭐️ 8.0/10
5. [PR spam today mirrors early 2000s email spam](#item-5) ⭐️ 8.0/10
6. [NVIDIA's 45°C Liquid Cooling Cuts Data Center Water Use to Near Zero](#item-6) ⭐️ 8.0/10
7. [Carmack Regrets Pushing Team Too Hard at id Software](#item-7) ⭐️ 8.0/10
8. [Nub: A Bun-like all-in-one toolkit for Node.js](#item-8) ⭐️ 8.0/10
9. [Rust community seeks to decouple crates.io from GitHub](#item-9) ⭐️ 8.0/10
10. [Tom MacWright Criticizes AI-Generated Job Applications](#item-10) ⭐️ 8.0/10
11. [Anthropic accuses Alibaba of illicitly extracting Claude AI capabilities](#item-11) ⭐️ 8.0/10
12. [RubyLLM: Unified Ruby Framework for Major AI Providers](#item-12) ⭐️ 7.0/10
13. [GLM-5.2: Open-Weight Model Gains Traction but Spurs Pricing Concerns](#item-13) ⭐️ 7.0/10
14. [SQLite database from Mozilla browser-compat-data](#item-14) ⭐️ 7.0/10
15. [Google Launches Computer Use in Gemini 3.5 Flash](#item-15) ⭐️ 6.0/10
16. [Xteink X4 E-Ink Reader: Tiny, Hackable, but Flawed](#item-16) ⭐️ 6.0/10
17. [Datasette 1.0a35 Alpha Adds Table Creation and Alteration APIs](#item-17) ⭐️ 6.0/10
18. [OPFS + Pyodide test harness for Datasette Lite](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI unveils first custom AI chip with Broadcom](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI, in partnership with Broadcom, announced its first custom AI inference chip named 'Jalapeño', developed from design to production in nine months using AI-assisted design. The chip is manufactured by TSMC and focuses on accelerating large language model inference. This marks a major shift as OpenAI moves from relying solely on GPUs to owning custom hardware, potentially reducing costs and improving efficiency for running ChatGPT and future AI systems. It also intensifies competition in the AI chip market, challenging incumbents like NVIDIA. The Jalapeño chip is an inference-optimized design co-developed with Broadcom and fabricated by TSMC. OpenAI claims it was completed in nine months, accelerated by their own AI models, though some commentators remain skeptical about the extent of AI involvement.

hackernews · jamdesk · Jun 24, 17:47 · [Discussion](https://news.ycombinator.com/item?id=48663324)

**Background**: AI inference chips are specialized processors designed to run trained AI models efficiently, as opposed to training chips which handle the computationally intensive training process. OpenAI has historically relied on NVIDIA GPUs for both training and inference, but increasing demand and costs have driven the company to develop custom silicon, similar to Google's TPUs or AWS's Trainium chips.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip | OpenAI</a></li>
<li><a href="https://wccftech.com/openai-first-custom-chip-is-as-hot-as-a-jalapeno-the-best-inference-platform-for-llms/">OpenAI 's First Custom Chip Is As Hot As A Jalapeño For AI, As The...</a></li>
<li><a href="https://www.datacenterdynamics.com/en/news/openai-and-broadcom-unveil-jalapeño-intelligence-processor-for-llm-inference/">OpenAI and Broadcom unveil ' Jalapeño ' Intelligence Processor for...</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some express skepticism about the AI-assisted design claims, questioning whether it's marketing hype. Others confirm the TSMC manufacturing and discuss potential architectural innovations, while a few compare the move to Google's TPUs and question when OpenAI will release performance benchmarks.

**Tags**: `#AI hardware`, `#custom chip`, `#OpenAI`, `#Broadcom`, `#inference`

---

<a id="item-2"></a>
## [Krea 2: SOTA open-weights 12B image model](https://www.krea.ai/blog/krea-2-technical-report) ⭐️ 9.0/10

Krea released open-weights of its 12B parameter image generation model, Krea 2, along with a comprehensive technical report detailing data curation, model architecture, and training infrastructure. Krea 2 achieves top scores among locally hostable models, offering state-of-the-art performance that can run on consumer hardware, challenging proprietary models and enabling broader access to advanced image generation. Two model variants are released: Krea 2 Turbo, which is both guidance- and timestep-distilled for faster inference (8 steps), and the standard model. The report includes details on RL pipelines, prompt expansion, and style references.

hackernews · mattnewton · Jun 23, 15:31 · [Discussion](https://news.ycombinator.com/item?id=48646659)

**Background**: Open-weights models make trained parameters publicly available, allowing users to download and run the model locally, study it, and modify it. Krea 2 is a 12B parameter text-to-image model that follows this approach, enabling usage on personal hardware without relying on cloud APIs.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model?</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed with the model's speed and performance, noting that Turbo at 8 steps outperformed most locally hostable models, though it still fell to common benchmark 'killers.' The detailed technical report and commitment to openness were highly appreciated.

**Tags**: `#AI`, `#image generation`, `#open-weights`, `#deep learning`, `#text-to-image`

---

<a id="item-3"></a>
## [Qualcomm Acquires Modular for $4 Billion](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 8.0/10

Qualcomm announced the acquisition of Modular, the AI startup behind the Mojo programming language and modular AI infrastructure, for $4 billion on June 24, 2026. This acquisition signals Qualcomm's strategic push into AI hardware and software integration, potentially positioning it to compete with NVIDIA in high-performance AI inference and training markets. Modular's Mojo language is built on MLIR, enabling high-performance code for CPUs, GPUs, and other accelerators. The deal values Modular at $4 billion, and Mojo is slated to become open source in fall 2026.

hackernews · timmyd · Jun 24, 13:49 · [Discussion](https://news.ycombinator.com/item?id=48659798)

**Background**: Mojo is a programming language designed to combine Python-like syntax with system-level performance, targeting AI infrastructure. It leverages the MLIR compiler framework to optimize across diverse hardware, including GPUs and TPUs. Modular, founded by Chris Lattner (creator of LLVM and Swift), has been developing the language and a modular AI platform.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://grokipedia.com/page/Mojo_(programming_language)">Mojo (programming language)</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some express surprise at the early acquisition and concern about Mojo's direction under Qualcomm, while others question Qualcomm's ability to compete in the high-end AI inference market. There is also irony noted given Lattner's past criticism of hardware companies' AI stacks.

**Tags**: `#AI`, `#acquisition`, `#Qualcomm`, `#Modular`, `#Mojo`

---

<a id="item-4"></a>
## [Bunny DNS goes free, eliminates query fees](https://bunny.net/blog/were-making-bunny-dns-free/) ⭐️ 8.0/10

Bunny DNS has announced that it is eliminating all DNS query fees and offering free DNS hosting for up to 500 domains per account, effective immediately. This move provides a compelling European-based alternative to Cloudflare, addressing growing demand for EU-hosted services amid geopolitical tensions, and lowers the cost barrier for DNS management. Users no longer face per-request billing or query limits, and advanced features like smart records and health monitoring are included for free with no hidden enterprise restrictions.

hackernews · dabinat · Jun 24, 08:50 · [Discussion](https://news.ycombinator.com/item?id=48657030)

**Background**: DNS (Domain Name System) translates human-readable domain names into IP addresses. Many DNS providers charge based on the number of queries or monthly active zones. Bunny.net is a European cloud infrastructure company offering CDN, storage, and DNS services, positioning itself as a privacy-conscious alternative to US providers.

<details><summary>References</summary>
<ul>
<li><a href="https://bunny.net/dns/">Bunny DNS | The #1 Scriptable DNS Platform | bunny .net</a></li>
<li><a href="https://euroalternative.eu/bunny-dns">Bunny DNS : European Alternative to Amazon Route 53 and...</a></li>

</ul>
</details>

**Discussion**: Comments on Hacker News are largely positive, with users like Lucasoato praising Bunny as an EU-based Cloudflare alternative and khurs noting its organic growth strategy. However, Diti expresses concern about sudden cost spikes from unexpected traffic for other Bunny products.

**Tags**: `#DNS`, `#free`, `#cloud infrastructure`, `#EU`, `#alternative`

---

<a id="item-5"></a>
## [PR spam today mirrors early 2000s email spam](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 8.0/10

The article and its comment thread compare the surge of unsolicited pull requests on GitHub to early email spam, highlighting a growing problem for open-source maintainers. Community members discuss potential solutions including new PR limits from GitHub and requiring non-textual introductions. This matters because unsolicited PRs waste maintainers' time and degrade the quality of open-source contributions. The discussion may lead to better tools and norms for managing project contributions. GitHub recently added configurable PR limits for maintainers (as mentioned in a comment). Unlike email spam, PR spam lacks per-user reputation systems tied to organizations, making it harder to filter automatically.

hackernews · dakshgupta · Jun 24, 14:32 · [Discussion](https://news.ycombinator.com/item?id=48660579)

**Background**: Pull request spam refers to low-quality or automated PRs submitted to open-source projects, often to game contribution metrics or for self-promotion. Open-source maintainers have to review all PRs, so spam adds significant overhead. This issue gained attention during events like Hacktoberfest, where participants submit trivial PRs. The comparison to early email spam highlights the need for systemic solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/shitoberfest/spam-pullrequests">GitHub - shitoberfest/ spam - pullrequests : Show the world how many...</a></li>
<li><a href="https://garvitasood.medium.com/github-clean-up-spam-babc5e5b5ab0">GitHub Clean-up Spam . by Garvita Sood, Anuj Bansal, Garima | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters share varied perspectives: one notes GitHub's new PR limits, another highlights the lack of organizational reputation in PR spam compared to email, a third shares historical email spam-fighting experience, and a fourth suggests requiring non-textual introductions or token donations to filter contributors.

**Tags**: `#open-source`, `#spam`, `#pull-requests`, `#maintainer-tools`

---

<a id="item-6"></a>
## [NVIDIA's 45°C Liquid Cooling Cuts Data Center Water Use to Near Zero](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA has introduced a novel liquid cooling design for AI data centers that operates at a coolant temperature of 45°C, enabling near-zero water usage by eliminating the need for chillers and evaporative cooling. This innovation significantly reduces the environmental impact of AI infrastructure, as data centers consume vast amounts of water for cooling. It also lowers energy costs because higher coolant temperatures reduce cooling energy requirements. The coolant is a mixture of 75% water and 25% propylene glycol, entering at 45°C and exiting at roughly 55°C. The design achieves full liquid cooling of all server components, not just GPUs and CPUs, requiring a complete redesign of thermal management for other parts.

hackernews · nitin_flanker · Jun 24, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48660178)

**Background**: Traditional data centers use air cooling or chilled water systems that rely on evaporative cooling, consuming large volumes of water. Liquid cooling is more efficient but typically requires lower coolant temperatures. NVIDIA's approach raises the coolant temperature to 45°C, which allows for dry cooling or waste heat reuse without water-intensive evaporation.

<details><summary>References</summary>
<ul>
<li><a href="https://beyondtmrw.org/article/45c-breakthrough-to-cool-ai-data-center-machines">AI Data Center Liquid Cooling 45C: Hotter Than a Hot Tub</a></li>
<li><a href="https://icharles.com/articles/nvidia-rubin-45c-liquid-cooling-zero-water">NVIDIA Rubin: 45°C Cooling, Near-Zero Water · iCharles</a></li>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45°C Liquid Cooling Design for AI Data Centers</a></li>

</ul>
</details>

**Discussion**: Commenters question the novelty of the approach, noting that higher coolant temperatures have been explored before, but acknowledge the full liquid cooling redesign is challenging. Discussions also highlight the potential for district heating and concerns about maintenance complexity in fully liquid-cooled servers.

**Tags**: `#data center`, `#cooling`, `#sustainability`, `#AI infrastructure`, `#NVIDIA`

---

<a id="item-7"></a>
## [Carmack Regrets Pushing Team Too Hard at id Software](https://twitter.com/ID_AA_Carmack/status/2069799283369345247) ⭐️ 8.0/10

John Carmack publicly reflected on his early mistakes at id Software, admitting he pushed his team too hard without allowing for slack as the company matured. This reflection offers valuable lessons for startup leaders about sustainable work culture and the need to adjust management style as a company grows. Carmack specifically linked the intense push to the development of Quake, noting that such intensity can wear out employees and ruin a company over time.

hackernews · shadowtree · Jun 24, 15:56 · [Discussion](https://news.ycombinator.com/item?id=48661825)

**Background**: John Carmack is a legendary game programmer known for his work at id Software on titles like Doom and Quake. id Software was known for its intense, startup-like work environment during the early 1990s, which produced groundbreaking games but also led to employee burnout and turnover.

**Discussion**: The community largely agreed with Carmack's self-criticism, citing Sandy Petersen's accounts of burnout during Quake's development. Some argued that despite the human cost, the resulting games like Quake were worth it, while others noted that id's creative talent left after Doom 2, impacting later titles.

**Tags**: `#software engineering`, `#game development`, `#leadership`, `#company culture`, `#retrospective`

---

<a id="item-8"></a>
## [Nub: A Bun-like all-in-one toolkit for Node.js](https://github.com/nubjs/nub) ⭐️ 8.0/10

Nub is a new toolkit that enhances Node.js with built-in TypeScript transpilation using the oxc transpiler and polyfills for APIs like Worker and Temporal, all via a --require preload hook and module resolution hook. It improves Node.js developer experience by offering seamless TypeScript support and modern APIs without replacing Node's runtime, bridging the gap between Node.js and Bun's convenience. This could save developers significant configuration time. Nub uses the oxc transpiler packaged as a Node-API add-on for performance, and registers a module resolution hook to handle TypeScript imports. It is purely additive and relies on Node's existing engine and standard library implementations.

hackernews · colinmcd · Jun 24, 14:14 · [Discussion](https://news.ycombinator.com/item?id=48660267)

**Background**: Node.js traditionally requires a separate transpilation step (e.g., with tsc or esbuild) to run TypeScript. Bun is an alternative runtime that includes built-in TypeScript support and many modern APIs. Nub aims to bring similar features to Node.js via hooks and polyfills. Oxc is a high-performance JavaScript tooling collection written in Rust, and Node-API allows native add-ons to be written in C/C++.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance JavaScript tools.</a></li>
<li><a href="https://github.com/nodejs/node-addon-api">GitHub - nodejs/node-addon-api: Module for using Node-API from C++ · GitHub</a></li>
<li><a href="https://github.com/guybedford/node-resolve-hook/blob/master/README.md">node-resolve-hook/README.md at master · guybedford/node-resolve-hook</a></li>

</ul>
</details>

**Discussion**: Comments are generally positive; users like the idea and some have already migrated monorepos without issues. A few users question the need for a transpiler given recent Node.js TypeScript support, while others discuss the choice of --require over --import and note potential ESM edge cases.

**Tags**: `#Node.js`, `#TypeScript`, `#Bun`, `#Developer Tools`, `#Transpiler`

---

<a id="item-9"></a>
## [Rust community seeks to decouple crates.io from GitHub](https://infosec.exchange/@mttaggart/116806641273303255) ⭐️ 8.0/10

A recently merged RFC (RFC 3963) and ongoing implementation aim to reduce reliance on GitHub for publishing crates on crates.io, improving supply-chain security and decentralization. Currently, crates.io uses GitHub OAuth for authentication, creating a single point of failure and potential supply-chain risk. Decoupling would allow alternative authentication methods and reduce the ecosystem's dependency on a single commercial platform. The effort includes implementing trusted publishing via OpenID Connect (OIDC) and other authentication methods, but progress is slow due to volunteer-driven development. The crates.io issue #326 tracks the roadmap.

hackernews · speckx · Jun 24, 19:40 · [Discussion](https://news.ycombinator.com/item?id=48664733)

**Background**: crates.io is the official Rust package registry, and currently requires a GitHub account for authentication when publishing crates. This centralization around GitHub has been a long-standing concern for supply-chain security, as it creates a dependency on a single provider. The Rust project is aware of this and has been working on solutions, but the work is largely volunteer-driven and complex.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/rust-lang/crates.io">GitHub - rust-lang/crates.io: The Rust package registry crates.io: Rust Package Registry 3691-trusted-publishing-cratesio - The Rust RFC Book crates.io: development update | Rust Blog Registries - The Cargo Book - Learn Rust</a></li>

</ul>
</details>

**Discussion**: The community largely agrees on the importance of decoupling, but acknowledges the challenges: it's a lot of work, volunteer-driven, and unglamorous. Comments reference RFC 3963, issue #326, and a talk by Jon Gjengset, highlighting both the progress and the difficulty of 'rebuilding the track while the train is running.' Some emphasize that the entire Rust ecosystem still faces broad supply-chain risks similar to npm and PyPI.

**Tags**: `#rust`, `#supply-chain`, `#crates.io`, `#open-source`, `#decentralization`

---

<a id="item-10"></a>
## [Tom MacWright Criticizes AI-Generated Job Applications](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 8.0/10

Tom MacWright, a well-known developer, published a blog post arguing that AI-generated job applications and portfolios make candidates seem generic and impersonal, eroding trust in the hiring process. This critique highlights a growing trend where job seekers use LLMs to generate application materials, leading to a loss of authentic signals that recruiters rely on. It may prompt discussions on how to evaluate candidates in an AI-saturated hiring landscape. MacWright observes that LLM-generated portfolios, GitHub projects, and commit messages are increasingly common, making it difficult to discern a candidate's genuine skills and personality. He notes that such applications tell him nothing about the person except their tool usage.

rss · Simon Willison · Jun 24, 18:13

**Background**: Large language models (LLMs) like GPT-4 are widely used to generate text, including resumes and cover letters. While they can help applicants save time, over-reliance on AI can produce content that lacks personal voice and authenticity. In technical hiring, recruiters often look for signals of genuine interest and skill through portfolios and open-source contributions.

**Tags**: `#ai`, `#careers`, `#hiring`, `#llm`, `#authenticity`

---

<a id="item-11"></a>
## [Anthropic accuses Alibaba of illicitly extracting Claude AI capabilities](https://www.investing.com/news/stock-market-news/anthropic-says-alibaba-illicitly-extracted-claude-ai-model-capabilities-4759021) ⭐️ 8.0/10

Anthropic publicly accused Alibaba of illicitly extracting capabilities from its Claude AI model through a model extraction attack, raising concerns about intellectual property theft in the AI industry. This allegation highlights critical intellectual property and security risks in the AI industry, potentially impacting how companies protect their models and share APIs. It could also affect competition and trust between major AI players. Model extraction attacks involve systematically querying a target model's API and using the outputs to train a replica model that mimics the original's behavior. As of now, Alibaba has not publicly responded to the allegations.

rss · Investing.com All News · Jun 24, 23:55

**Background**: Anthropic is a US-based AI safety company founded in 2021 by former OpenAI members, known for developing the Claude series of large language models focused on safety and reliability. A model extraction attack is a common AI security threat where an adversary with API access steals a model's functionality by querying it extensively.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude ( AI ) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.praetorian.com/blog/stealing-ai-models-through-the-api-a-practical-model-extraction-attack/">Stealing AI Models Through the API: A Practical Model Extraction Attack | Praetorian</a></li>

</ul>
</details>

**Tags**: `#AI`, `#intellectual property`, `#security`, `#Anthropic`, `#Alibaba`

---

<a id="item-12"></a>
## [RubyLLM: Unified Ruby Framework for Major AI Providers](https://rubyllm.com/) ⭐️ 7.0/10

RubyLLM is a new open-source Ruby gem that provides a unified interface for major AI providers such as OpenAI, Anthropic, and local Ollama models. It aims to simplify AI integration in Ruby applications with a single API. RubyLLM reduces the friction of switching between AI providers and lowers the barrier for Ruby developers to incorporate LLMs into their projects. It strengthens the Ruby AI ecosystem, making it more competitive with Python for AI development. RubyLLM has only three dependencies: Faraday, Zeitwerk, and Marcel. However, community members have noted issues with caching (e.g., for xAI) and lack of native support for the responses API, though a recent update appears to have added it.

hackernews · doener · Jun 24, 14:41 · [Discussion](https://news.ycombinator.com/item?id=48660711)

**Background**: Ruby is a popular scripting language, but until now lacked a unified SDK for interacting with multiple large language model providers. Many Ruby developers had to use provider-specific gems or raw HTTP calls. RubyLLM fills this gap by offering a consistent API similar to Vercel's AI SDK for JavaScript.

<details><summary>References</summary>
<ul>
<li><a href="https://rubyllm.com/">RubyLLM | One beautiful Ruby framework for all major AI providers.</a></li>
<li><a href="https://medium.com/@raviskit2012/rubyllm-the-ruby-gem-that-makes-ai-feel-right-at-home-a34a1d18def4">RubyLLM : The Ruby Gem That Makes AI Feel Right at Home | Medium</a></li>

</ul>
</details>

**Discussion**: Community feedback is largely positive, praising RubyLLM's ease of use and clean design. However, several users reported issues with caching not working reliably, missing native responses API support, and difficulty in achieving full trace observability. Some contributors are actively developing extensions to address these gaps.

**Tags**: `#Ruby`, `#AI`, `#framework`, `#LLM`, `#open source`

---

<a id="item-13"></a>
## [GLM-5.2: Open-Weight Model Gains Traction but Spurs Pricing Concerns](https://www.interconnects.ai/p/glm-52-is-the-step-change-for-open) ⭐️ 7.0/10

GLM-5.2, an open-weight model from Z.AI, offers competitive performance on par with proprietary models like GPT-5.5 at a lower cost, but users report excessive token consumption and unclear pricing structures. This model represents a step change for open-source agents, potentially democratizing access to high-performance AI, but its high token usage could limit its practical adoption and raise fairness concerns in the AI ecosystem. GLM-5.2 employs multi-token prediction, achieving top scores on design benchmarks, but users on the Max plan report burning through 700M tokens in two days, far exceeding typical usage of Claude or Codex models.

hackernews · vantareed · Jun 23, 03:23 · [Discussion](https://news.ycombinator.com/item?id=48639840)

**Background**: Open-weight models allow developers to inspect, modify, and self-host the model weights, offering greater transparency and control compared to closed APIs. Token pricing is a common billing method for LLM APIs, where each token (roughly 0.75 words) costs a fraction of a cent. GLM-5.2 is the latest in the GLM series from Z.AI, a Chinese AI lab, and claims to outperform many proprietary models while being significantly cheaper per token.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM-5.2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-glm-5-2-open-weight-model">What Is GLM 5.2? The Open-Weight Model Beating GPT 5.5 on Design Benchmarks | MindStudio</a></li>
<li><a href="https://www.reddit.com/r/technology/comments/1uc5hjh/what_is_glm52_another_opensource_chinese_ai_model/">r/technology on Reddit: What is GLM-5.2? Another open-source Chinese AI model has Silicon Valley's attention.</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some praise the model's performance and affordability (e.g., jerojero and fraywing), but others strongly criticize excessive token consumption and billing issues. Guybedo reports draining a 700M token weekly quota in under two days, while aunty_helen struggles with API errors and a denied refund.

**Tags**: `#open-source AI`, `#GLM-5.2`, `#LLM`, `#pricing`, `#AI agents`

---

<a id="item-14"></a>
## [SQLite database from Mozilla browser-compat-data](https://simonwillison.net/2026/Jun/24/browser-compat-db/#atom-everything) ⭐️ 7.0/10

Simon Willison used AI-generated scripts (Claude Code and Codex Desktop) to convert Mozilla's mdn/browser-compat-data repository into a ~66MB SQLite database, which is now available via GitHub CDN with open CORS headers. This makes browser compatibility data easily queryable for developers, enabling faster integration into tools and workflows, and showcases the practical use of AI-assisted programming for data conversion and deployment. The database is built using sqlite-utils and hosted on an orphan branch ('db') to leverage GitHub's open CORS headers for direct access. It can be explored immediately via Datasette Lite without any setup.

rss · Simon Willison · Jun 24, 23:59

**Background**: Mozilla's browser-compat-data repository contains detailed browser compatibility information for web features, commonly used by developers to ensure cross-browser support. SQLite is a lightweight, serverless database engine. The GitHub CDN serves files from repositories with open CORS headers, allowing client-side web applications to fetch the database. Datasette Lite is a browser-based tool for exploring SQLite databases.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/blog/introducing-mdn-mcp-server/?ref=weeklyfoo">Introducing the MDN MCP server - MDN Web Docs</a></li>
<li><a href="https://pypi.org/project/sqlite-utils/">sqlite - utils · PyPI</a></li>
<li><a href="https://code.claude.com/docs/en/claude-code-on-the-web">Use Claude Code on the web - Claude Code Docs</a></li>

</ul>
</details>

**Tags**: `#browser-compat-data`, `#SQLite`, `#developer tools`, `#Mozilla`, `#data conversion`

---

<a id="item-15"></a>
## [Google Launches Computer Use in Gemini 3.5 Flash](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/) ⭐️ 6.0/10

Google has introduced a 'computer use' feature in its Gemini 3.5 Flash model, enabling the AI to interact with graphical user interfaces and analyze on-screen content. The feature is now available to developers via the Gemini API. This marks a significant step toward more autonomous AI agents capable of performing tasks across applications. However, user reports of errors and missing support for key protocols like MCP highlight that the feature is still immature compared to competitors. The computer use feature works by analyzing screenshots and simulating clicks or inputs, but early testers have encountered frequent failures, such as Gemini giving up on simple data extraction tasks. Additionally, the Gemini app still lacks MCP (Model Context Protocol) support, which would allow it to connect to external tools like search engines or databases.

hackernews · swolpers · Jun 24, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48662999)

**Background**: Computer use is a capability that allows AI models to perceive and interact with a computer's graphical interface, similar to how a human would use a mouse and keyboard. MCP (Model Context Protocol) is an open standard developed by Anthropic that enables AI agents to connect to external data sources and tools, enhancing their functionality. Google's Gemini 3.5 Flash is a fast and efficient model designed for high-throughput applications.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/">Introducing computer use in Gemini 3 . 5 Flash</a></li>
<li><a href="https://9to5google.com/2026/06/24/gemini-chrome-select-screen/">Gemini in Chrome adds ‘Select from screen’ tool</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3 . 5 Flash — Google DeepMind</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed but largely critical. A user reported that Gemini gave up on a simple table extraction task after many iterations, admitting it 'invents data instead of doing a simple data copy/reformat.' Another user lamented the lack of MCP support, which forced them to use Codex for tasks requiring external info. Some also pointed out that in Google's own benchmark graph, Gemini 3.5 Flash was outperformed by competitors like Opus 4.8 and GPT 5.5.

**Tags**: `#Gemini`, `#AI`, `#language models`, `#computer use`, `#LLM limitations`

---

<a id="item-16"></a>
## [Xteink X4 E-Ink Reader: Tiny, Hackable, but Flawed](https://blog.omgmog.net/post/xteink-x4-e-ink-reader/) ⭐️ 6.0/10

A blog review of the Xteink X4 e-ink reader highlights its tiny size, ease of use with custom firmware like CrossPoint, and USB-C charging, but also points out the small screen and a reported risk of credit card fraud from the purchase process. The X4 demonstrates that a microcontroller-based e-reader can be sufficient for basic reading and highlights the appeal of open, hackable devices compared to locked-down competitors like Kindle. However, the screen size and fraud concerns limit its mass appeal, making it a niche product for enthusiasts. The X4 runs custom firmware (e.g., CrossPoint) accessible via a WiFi-based HTTP server for easy book transfers, uses a USB-C port, and includes a magnetic cover. Community reports note potential credit card fraud when purchasing from the manufacturer or website.

hackernews · felixdoerp · Jun 24, 16:35 · [Discussion](https://news.ycombinator.com/item?id=48662381)

**Background**: Custom firmware (CFW) is third-party software that replaces or modifies the original firmware of a device, adding features like improved emulator support or custom themes. E-ink displays are low-power screens that mimic paper, ideal for long reading sessions but typically lack backlighting. The Xteink X4 is a compact, open e-reader that appeals to hackers and tinkerers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Custom_firmware">Custom firmware</a></li>
<li><a href="https://handhelds.wiki/Custom_Firmware">Custom Firmware - Handhelds Wiki</a></li>

</ul>
</details>

**Discussion**: Community comments are generally positive, praising the X4's custom firmware and small form factor, with users noting it fits easily in a pocket. However, several users express disappointment with the tiny screen (especially for older eyes) and report credit card fraud issues, which tempers overall enthusiasm.

**Tags**: `#e-ink`, `#reader`, `#hardware`, `#review`, `#hackernews`

---

<a id="item-17"></a>
## [Datasette 1.0a35 Alpha Adds Table Creation and Alteration APIs](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 6.0/10

Datasette 1.0a35 introduces a 'Create table' interface and 'Alter table' action, both backed by JSON APIs, allowing users to define columns, constraints, and foreign keys, and to modify existing tables including renaming, reordering, and dropping columns. This release significantly extends Datasette's functionality from read-only to include schema management, making it a more complete data publishing tool. It empowers users to manage SQLite databases directly through the web UI and API, reducing reliance on external database tools. The 'Create table' API supports custom column types, NOT NULL constraints, literal and expression defaults, and single-column foreign keys. The 'Alter table' API allows adding, renaming, reordering, and dropping columns, as well as changing column types, defaults, constraints, primary keys, and foreign keys.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing data, especially SQLite databases. It provides a web interface and JSON API for querying data. Prior to this release, Datasette focused on read-only access; schema changes required external tools. This alpha adds write capabilities for schema management.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#JSON API`, `#database`, `#sqlite`

---

<a id="item-18"></a>
## [OPFS + Pyodide test harness for Datasette Lite](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison created a test harness to explore using the Origin Private File System (OPFS) with Pyodide in the browser, aiming to enable persistent storage of SQLite files in Datasette Lite. This tool provides a practical way to test persistent browser-based storage for Python web applications, potentially allowing Datasette Lite to save and edit SQLite databases locally without a server. The harness is a playground UI built with Claude Code for web, allowing experimentation across different browsers with OPFS and Pyodide.

rss · Simon Willison · Jun 23, 18:58

**Background**: Datasette Lite runs the full Datasette Python application in the browser using Pyodide, a port of CPython to WebAssembly. OPFS is a browser storage API providing a sandboxed, origin-specific virtual filesystem optimized for performance, which could enable local file persistence for web apps.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN</a></li>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.0</a></li>
<li><a href="https://lite.datasette.io/">Datasette</a></li>

</ul>
</details>

**Discussion**: No comments were provided with this news item.

**Tags**: `#browsers`, `#pyodide`, `#datasette-lite`, `#OPFS`

---