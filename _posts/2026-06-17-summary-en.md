---
layout: default
title: "Horizon Summary: 2026-06-17 (EN)"
date: 2026-06-17
lang: en
---

> From 45 items, 20 important content pieces were selected

---

1. [vLLM v0.23.0 Boosts DeepSeek-V4, Expands Model Runner V2](#item-1) ⭐️ 8.0/10
2. [Local LLMs Become Practical for Personal Use](#item-2) ⭐️ 8.0/10
3. [SpaceX to buy Cursor for $60B](#item-3) ⭐️ 8.0/10
4. [Apple change threatens Hide My Email privacy](#item-4) ⭐️ 8.0/10
5. [Export Controls on AI Models Undermine US Cyber Defense](#item-5) ⭐️ 8.0/10
6. [OpenAI loses $3.7 billion in Q1 2026](#item-6) ⭐️ 8.0/10
7. [GrapheneOS Ported to Android 17, Official Releases Imminent](#item-7) ⭐️ 7.0/10
8. [Interactive Article on Mechanical Watch Mechanics Earns High Praise](#item-8) ⭐️ 7.0/10
9. [Stop Using JWTs for Browser Sessions](#item-9) ⭐️ 7.0/10
10. [Netherlands unveils GPT-NL, a sovereign language model](#item-10) ⭐️ 7.0/10
11. [AI and LLMs Threaten Self-Help Nonfiction Books](#item-11) ⭐️ 7.0/10
12. [Slay the Spire 2 using custom PRNG for seed consistency](#item-12) ⭐️ 7.0/10
13. [U.S. govt-Anthropic clashes lead to model shutdowns](#item-13) ⭐️ 7.0/10
14. [Datasette 1.0a34 adds inline row editing](#item-14) ⭐️ 6.0/10
15. [Bash /dev/tcp for HTTP Requests Without curl](#item-15) ⭐️ 6.0/10
16. [Calvin and Hobbes and the price of integrity](#item-16) ⭐️ 6.0/10
17. [Yak Shaving: The Joy of Distraction](#item-17) ⭐️ 6.0/10
18. [Apple's Vehicle Motion Cues effectively reduce car sickness](#item-18) ⭐️ 6.0/10
19. [Datasette plugin uses Tailscale sidecar for instant sharing](#item-19) ⭐️ 6.0/10
20. [Expert: Fable Jailbreak Shows Model 'Working as Intended'](#item-20) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [vLLM v0.23.0 Boosts DeepSeek-V4, Expands Model Runner V2](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 8.0/10

vLLM v0.23.0 introduces major hardening for DeepSeek-V4, including decoupled sparse MLA metadata and TRTLLM-gen attention kernel, and expands Model Runner V2 to Llama and Mistral dense models by default. This release significantly improves efficiency and stability for DeepSeek-V4 inference, benefiting large-scale MoE deployments. The expansion of Model Runner V2 to popular dense models broadens performance gains for many users. The release includes 408 commits from 200 contributors, adds multi-tier KV cache offloading with object-store tier, and unifies parser interface for reasoning and tool calls. Note: Minimax M3 is not yet supported.

github · khluu · Jun 15, 05:27

**Background**: vLLM is a high-throughput LLM inference engine. DeepSeek-V4 is a Mixture-of-Experts model with sparse attention. Model Runner V2 is a newer execution path that improves performance. EPLB (Expert Parallelism Load Balancer) optimizes expert placement across GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/deepseek_v4/sparse_mla/">sparse_mla - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/stable/api/vllm/v1/attention/backends/mla/flashinfer_mla_sparse/">flashinfer_mla_sparse - vLLM</a></li>
<li><a href="https://www.deepep.org/en/eplb">EPLB (Expert Parallelism Load Balancer) - DeepEP</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM inference`, `#DeepSeek`, `#model optimization`, `#release`

---

<a id="item-2"></a>
## [Local LLMs Become Practical for Personal Use](https://vickiboykis.com/2026/06/15/running-local-models-is-good-now/) ⭐️ 8.0/10

A popular blog post argues that running large language models locally has become practical, citing improvements in model efficiency and hardware availability. This shift could reduce reliance on cloud-based AI services, offering users more privacy, lower costs, and offline capability, potentially disrupting the current AI-as-a-service market. Users must choose between dense models (smarter but slower) and mixture-of-experts models (faster but more error-prone), and quantization to 4-bit can degrade tool-calling performance.

hackernews · jfb · Jun 16, 14:36 · [Discussion](https://news.ycombinator.com/item?id=48555993)

**Background**: Local LLMs are open-source models that run on a user's own hardware rather than in the cloud. Running them locally requires a powerful GPU and sufficient RAM, and models are often quantized to fit into memory. Popular models include Llama, Qwen, and Gemma.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aitooldiscovery.com/how-to/best-local-llm-models">Best Local LLM Models 2026: Benchmarks & Use Cases</a></li>
<li><a href="https://www.geeksforgeeks.org/blogs/how-to-run-llms-model-locally/">How to Run LLMs Model Locally - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some find local models still painful due to speed or accuracy trade-offs, while others prefer them over cloud models for their behavior and control. There is also discussion about the long-term cost implications for cloud AI providers.

**Tags**: `#local-llm`, `#AI`, `#machine-learning`, `#open-source-models`

---

<a id="item-3"></a>
## [SpaceX to buy Cursor for $60B](https://www.reuters.com/legal/transactional/spacex-buy-anysphere-60-billion-2026-06-16/) ⭐️ 8.0/10

SpaceX has announced plans to acquire Anysphere, the company behind the AI coding tool Cursor, for $60 billion. This acquisition signals a major convergence of space technology and AI software engineering, potentially giving SpaceX proprietary AI tools to accelerate its engineering and software development. Cursor was last valued at $29.3 billion, making the $60 billion acquisition price a significant premium. SpaceX reportedly sees a $26 trillion addressable market for AI products.

hackernews · itsmarcelg · Jun 16, 10:44 · [Discussion](https://news.ycombinator.com/item?id=48553224)

**Background**: Cursor is an AI-powered coding agent and development environment that uses natural language to help programmers write and edit code. Founded in 2022, it has quickly become a leading tool in the AI-assisted coding space. SpaceX, primarily known for space exploration and transportation, is apparently diversifying into AI software.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(company)">Cursor (company) - Wikipedia</a></li>
<li><a href="https://cursor.com/">Cursor: AI coding agent</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some question the strategic fit of a space company acquiring an IDE, while others highlight the enormous addressable market SpaceX sees. A user compares the $60B valuation to Minecraft's $2.5B, calling valuations 'nonsensical.'

**Tags**: `#SpaceX`, `#Cursor`, `#AI coding`, `#acquisition`, `#business`

---

<a id="item-4"></a>
## [Apple change threatens Hide My Email privacy](https://arseniyshestakov.com/2026/06/16/apple-is-about-to-make-hide-my-email-useless/) ⭐️ 8.0/10

Apple is moving both Sign in with Apple and Hide My Email aliases to the @private.icloud.com subdomain, making it trivial for websites to block all such aliases with a single domain ban. This change undermines the core privacy benefit of Hide My Email, as users will no longer be able to rely on these aliases to bypass website email blocking, and it may drive users toward third-party alternatives. The change has not yet been implemented, so users can still generate additional @icloud.com aliases at a rate of at least 30 per hour before the migration occurs.

hackernews · SXX · Jun 16, 18:37 · [Discussion](https://news.ycombinator.com/item?id=48559935)

**Background**: Hide My Email is an iCloud+ feature that generates unique, random email addresses that forward to your personal inbox, allowing you to keep your real email private. It is integrated with Sign in with Apple and can be used in Mail, Safari, and iCloud settings. By moving all aliases to a single subdomain, Apple inadvertently creates a single point of blocking for website owners.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/en-us/105078">How to use Hide My Email with Sign in with Apple - Apple Support</a></li>
<li><a href="https://support.apple.com/guide/iphone/create-and-manage-hide-my-email-addresses-iphcb02e76f7/ios">Create and manage Hide My Email addresses in Settings on iPhone - Apple Support</a></li>
<li><a href="https://support.apple.com/guide/icloud/set-up-hide-my-email-mm9d9012c9e8/icloud">Set up and use Hide My Email in iCloud+ on all your devices - Apple Support</a></li>

</ul>
</details>

**Discussion**: Commenters express frustration and recommend alternatives: some suggest pre-generating @icloud.com aliases while still possible; others advocate for custom domains with services like SimpleLogin or Fastmail, or using catch-all subdomains with own domains for maximum control.

**Tags**: `#apple`, `#privacy`, `#email`, `#hide-my-email`, `#security`

---

<a id="item-5"></a>
## [Export Controls on AI Models Undermine US Cyber Defense](https://simonwillison.net/2026/Jun/16/fable-5-export-controls/#atom-everything) ⭐️ 8.0/10

US export controls forced Anthropic to suspend Claude Fable 5 because researchers used it to fix code vulnerabilities, which regulators misclassified as a 'jailbreak' for cyber attacks. This policy hinders defenders from using AI to fix bugs and verify patches, making US cybersecurity weaker. It conflates defensive capabilities with offensive threats, threatening innovation. Researchers asked Fable 5 to review open-source code with known CVEs and planted vulnerabilities. The model's refusal to 'fix this code' due to export controls prevents legitimate security testing.

rss · Simon Willison · Jun 16, 05:20

**Background**: Claude Fable 5 is Anthropic's most advanced AI model, state-of-the-art in coding and security tasks. Export controls are US regulations restricting foreign access to advanced AI, citing national security. CVE (Common Vulnerabilities and Exposures) is a standard for identifying known software vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.politico.com/news/2026/06/13/inside-the-whirlwind-24-hours-that-led-the-white-house-to-slap-export-controls-on-anthropic-00961519">Inside the whirlwind 24 hours that led the White House to slap export ...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/jun/13/anthropic-disable-advanced-ai-models-us-government-order">Anthropic to disable its most advanced AI models after... | The Guardian</a></li>

</ul>
</details>

**Tags**: `#AI`, `#export controls`, `#cybersecurity`, `#policy`

---

<a id="item-6"></a>
## [OpenAI loses $3.7 billion in Q1 2026](https://www.investing.com/news/stock-market-news/openai-burned-37-billion-in-first-quarter-of-2026-the-information-93CH-4746236) ⭐️ 8.0/10

OpenAI reported a $3.7 billion operating loss in the first quarter of 2026, according to The Information, highlighting its rapid cash burn. This high burn rate raises concerns about OpenAI's long-term financial sustainability and could influence investor confidence in AI startups. The $3.7 billion loss was reported for the first quarter of 2026, suggesting annualized losses could exceed $10 billion if the trend continues.

rss · Investing.com All News · Jun 17, 00:18

**Background**: OpenAI operates as a for-profit entity with massive compute costs for training and inference of large language models like GPT-4. The company relies heavily on revenue from subscriptions and API access to offset expenses. Such high operational losses are common among AI companies scaling their infrastructure rapidly.

**Tags**: `#OpenAI`, `#finance`, `#AI industry`, `#business news`

---

<a id="item-7"></a>
## [GrapheneOS Ported to Android 17, Official Releases Imminent](https://discuss.grapheneos.org/d/36469-grapheneos-has-been-ported-to-android-17-and-official-releases-are-coming-soon) ⭐️ 7.0/10

GrapheneOS has been fully ported to Android 17, with code being pushed to public repositories; an initial official release is expected tomorrow after a final Android 16 QPR2 build today. This marks a timely adaptation to Google's latest Android version, ensuring that privacy-focused users can run GrapheneOS on the newest platform. It also demonstrates the project's responsiveness and commitment to staying current. The port has been tested on Pixel 6a, 7, 7a, 8, 10a, 10, and 10 Pro models. GrapheneOS is built on AOSP and is available for Google Pixel and future Motorola devices.

hackernews · Cider9986 · Jun 16, 20:34 · [Discussion](https://news.ycombinator.com/item?id=48561654)

**Background**: GrapheneOS is an open-source mobile OS that enhances Android's security and privacy through extensive hardening, including attack surface reduction and improved app sandboxing. It is developed by the GrapheneOS Foundation, a nonprofit founded in 2023. Android 17, codenamed Cinnamon Bun, is the latest major Android release, with beta available since February 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://discuss.grapheneos.org/d/36469-grapheneos-has-been-ported-to-android-17-and-official-releases-are-coming-soon">GrapheneOS has been ported to Android 17 and official ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Android_17">Android 17 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members expressed strong enthusiasm, with users sharing positive experiences and anticipation. Some discussed missing features like swipe-to-cursor in text input and NFC payment compliance. A long-time iPhone user mentioned considering switching to Pixel for GrapheneOS.

**Tags**: `#GrapheneOS`, `#Android`, `#privacy`, `#security`, `#open-source`

---

<a id="item-8"></a>
## [Interactive Article on Mechanical Watch Mechanics Earns High Praise](https://ciechanow.ski/mechanical-watch/) ⭐️ 7.0/10

An in-depth interactive article published in 2022 by Bartosz Ciechanowski explains the inner workings of mechanical watches with detailed, scrollable visualizations, and has been widely praised for its educational clarity. This article showcases how interactive web content can make complex mechanical engineering topics understandable, potentially inspiring a new generation of enthusiasts and creators in horology and related fields. The article is built entirely with vanilla code (no frameworks), works on older browsers and devices, and covers key watch components such as the escapement, balance wheel, and gear train, with interactive 3D-like animations.

hackernews · razin · Jun 16, 11:26 · [Discussion](https://news.ycombinator.com/item?id=48553550)

**Background**: Mechanical watches operate without batteries, using a mainspring to store energy and a gear train to transmit it. The escapement mechanism controls the release of energy, producing the ticking sound and ensuring accuracy. Horology, the study of time measurement, encompasses these intricate devices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Horology">Horology</a></li>
<li><a href="https://en.wikipedia.org/wiki/Escapement_mechanism">Escapement mechanism</a></li>

</ul>
</details>

**Discussion**: Commenters universally praised the article's educational value and technical execution, with one user building a physical model inspired by it and others noting the author's humility and the site's cross-device compatibility.

**Tags**: `#mechanical watch`, `#interactive visualization`, `#technical explanation`, `#horology`, `#education`

---

<a id="item-9"></a>
## [Stop Using JWTs for Browser Sessions](https://gist.github.com/samsch/0d1f3d3b4745d778f78b230cf6061452) ⭐️ 7.0/10

A widely-discussed gist argues that JSON Web Tokens (JWTs) should not be used for browser-based user sessions due to security risks, sparking a nuanced community debate. This matters because JWTs are commonly used for authentication, and the debate highlights critical trade-offs between JWTs and traditional session cookies, affecting web security practices. JWTs stored in localStorage are vulnerable to XSS attacks, whereas httpOnly cookies protect against credential theft but require CSRF protection; the post also notes that JWTs can be made secure with short lifetimes and refresh tokens.

hackernews · dzonga · Jun 16, 16:49 · [Discussion](https://news.ycombinator.com/item?id=48558147)

**Background**: JSON Web Tokens (JWT) are an open standard (RFC 7519) for transmitting claims as a JSON object, commonly used for authentication and information exchange. Cross-site scripting (XSS) is a vulnerability where attackers inject malicious scripts into trusted websites, potentially stealing tokens or performing actions on behalf of users.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JSON_Web_Token">JSON Web Token - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cross-site_scripting">Cross-site scripting - Wikipedia</a></li>
<li><a href="https://owasp.org/www-community/attacks/xss/">Cross Site Scripting (XSS) | OWASP Foundation</a></li>

</ul>
</details>

**Discussion**: Commenters agree that JWTs are problematic for browser sessions but useful for service-to-service communication. Some emphasize that httpOnly cookies mitigate XSS risks but introduce CSRF concerns, while others argue that short-lived JWTs with refresh tokens are viable alternatives.

**Tags**: `#web security`, `#authentication`, `#JWT`, `#cookies`, `#XSS`

---

<a id="item-10"></a>
## [Netherlands unveils GPT-NL, a sovereign language model](https://www.tno.nl/en/digital/artificial-intelligence/gpt-nl/) ⭐️ 7.0/10

The Netherlands announced GPT-NL, a sovereign language model designed to reduce dependence on foreign AI providers and strengthen national AI capabilities. This initiative reflects a broader trend of countries developing their own large language models for linguistic and cultural independence. GPT-NL is significant because it highlights the growing importance of AI sovereignty, where nations seek to control their AI infrastructure and data. If successful, it could inspire other countries to follow, potentially reshaping the global AI landscape and reducing dominance of US and Chinese models. The model is developed by TNO, a Dutch research organization, and is part of the national AI strategy. Skeptics argue that focusing on fine-tuning existing frontier models like Qwen or Kimi may be more cost-effective than building a sovereign model from scratch.

hackernews · root-parent · Jun 16, 17:54 · [Discussion](https://news.ycombinator.com/item?id=48559188)

**Background**: Sovereign AI refers to national efforts to build independent AI capabilities to reduce foreign dependency. Several countries have launched similar initiatives, such as Sweden's GPT-SW3 and the UK's Sovereign AI Fund. Regional LLMs aim to preserve linguistic and cultural nuances, but require significant investment in compute and data. The debate centers on whether to build from scratch or adapt existing open-source models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sovereign_AI_Fund">Sovereign AI Fund</a></li>
<li><a href="https://www.mckinsey.com/featured-insights/mckinsey-explainers/what-is-sovereign-ai">What is sovereign AI? | McKinsey</a></li>
<li><a href="https://vast.ai/article/global-growth-of-regional-large-language-models-llms">Global Growth of Regional Large Language Models (LLMs)</a></li>

</ul>
</details>

**Discussion**: Community comments show a split: some question the value of costly sovereign models, recommending instead to fine-tune existing frontier models like Qwen or Kimi for practical use. Others argue that building native models is crucial for linguistic and cultural independence, and that costs may decrease over time. A user also emphasized the importance of sovereign fine-tuning capability to keep models up-to-date.

**Tags**: `#sovereign AI`, `#language model`, `#Netherlands`, `#AI policy`, `#regional LLM`

---

<a id="item-11"></a>
## [AI and LLMs Threaten Self-Help Nonfiction Books](https://tim.blog/2026/06/12/has-ai-already-killed-nonfiction/) ⭐️ 7.0/10

A blog post by Tim Ferriss argues that AI and large language models (LLMs) are making self-help nonfiction books obsolete by offering faster, more direct answers to personal improvement questions. This signals a shift in how people consume information for self-improvement, potentially disrupting the publishing industry and prompting authors to adapt to the new AI-driven landscape. The article has a score of 7.0/10 and generated high engagement with 133 comments, many offering insightful observations about AI replacing self-help books.

hackernews · imakwana · Jun 16, 17:11 · [Discussion](https://news.ycombinator.com/item?id=48558489)

**Background**: Large language models (LLMs) are AI systems trained on vast text data to understand and generate human language. They can summarize, translate, and analyze text, making them effective at providing concise answers. Tim Ferriss is a well-known author in the self-help space, so his perspective adds authority.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model</a></li>
<li><a href="https://www.ibm.com/think/topics/large-language-models">What Are Large Language Models (LLMs)? | IBM</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some agree that self-help books are too bloated and LLMs offer better efficiency, while others criticize the self-help industry as a 'self-help mafia' and note that readers are turning to free resources like YouTube. One comment humorously suggests that redpillers benefit from even less thinking.

**Tags**: `#AI`, `#self-help`, `#books`, `#LLMs`, `#industry impact`

---

<a id="item-12"></a>
## [Slay the Spire 2 using custom PRNG for seed consistency](https://tck.mn/blog/correlated-randomness-sts2/) ⭐️ 7.0/10

A blog post details how Slay the Spire 2 implements correlated randomness and a custom PRNG to ensure seeds are identical across all platforms, fixing a major issue from the original game. This ensures that players on different platforms can share seeds for identical runs, and prevents seed-breaking changes from future platform updates, improving community and developer reliability. The game avoids using C#'s System.Random and instead implements its own PRNG, with additional logic for correlated randomness (e.g., ensuring certain tough enemy combinations are less likely).

hackernews · rdmuser · Jun 16, 09:46 · [Discussion](https://news.ycombinator.com/item?id=48552844)

**Background**: Slay the Spire is a roguelike deck-building game where seeds determine the entire run, making seed sharing a key community feature. However, different platforms often use different PRNG implementations, causing seeds to produce different results. A custom PRNG guarantees deterministic, cross-platform behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://tck.mn/blog/correlated-randomness-sts2/">Correlated randomness in Slay the Spire 2 - Andy Tockman</a></li>

</ul>
</details>

**Discussion**: Commenters appreciated the technical breakdown and discussed related issues like an unwinnable seed in the original game. Some noted that Godot's GDScript uses PCG32, which already solves the platform-specific problem, but the developer chose a custom approach for more control.

**Tags**: `#game development`, `#PRNG`, `#cross-platform`, `#software engineering`, `#random numbers`

---

<a id="item-13"></a>
## [U.S. govt-Anthropic clashes lead to model shutdowns](https://simonwillison.net/2026/Jun/15/axios-clashes-anthropics/#atom-everything) ⭐️ 7.0/10

An Axios report reveals that personality clashes between Anthropic and the U.S. government triggered export control directives that took Anthropic's frontier models offline. This incident highlights the growing tension between AI companies and regulators over export controls, setting a precedent that could affect how frontier models are deployed globally. The offline models are Claude Mythos (a frontier model) and Claude Fable (a publicly accessible version with guardrails). Anthropic's Frontier Red Team is meeting with Commerce Department to address the situation.

rss · Simon Willison · Jun 15, 14:57

**Background**: The U.S. government has been tightening export controls on advanced AI models, citing national security concerns. Anthropic's Claude Mythos is its most capable frontier model, while Claude Fable is a safer public version that restricts responses in high-risk domains like cybersecurity and biology.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/mythos">Claude Mythos \ Anthropic</a></li>
<li><a href="https://techcrunch.com/2026/06/09/anthropics-claude-fable-5-is-a-version-of-mythos-the-public-can-access-today/">Anthropic’s Claude Fable is a version of Mythos the public ...</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#government regulation`, `#export controls`, `#AI policy`, `#frontier models`

---

<a id="item-14"></a>
## [Datasette 1.0a34 adds inline row editing](https://github.com/simonw/datasette/releases/tag/1.0a34) ⭐️ 6.0/10

Datasette 1.0a34 introduces tools to insert, edit, and delete rows directly within the web interface, along with per-request permission caching and new autocomplete and HTML fragment endpoints. This release transforms Datasette from a read-only exploration tool into a full CRUD application, enabling users to modify data interactively without external tools. The permission caching and improved plugin hooks enhance performance and extensibility for complex deployments. The edit interface respects custom column types, with plugins able to define custom edit fields via the makeColumnField() JavaScript hook. The new autocomplete API at /<database>/<table>/-/autocomplete speeds up foreign key selection in the edit UI.

github · simonw · Jun 16, 21:31

**Background**: Datasette is an open-source tool for exploring and publishing data. It turns SQLite databases into interactive websites with browsable tables and a JSON API. This alpha release moves Datasette closer to a 1.0 release by adding essential data manipulation capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/datasette: An open source multi-tool for ... Datasette: An open source multi-tool for exploring and ... Datasette: An open source multi-tool for exploring and ... datasette · PyPI Datasette download | SourceForge.net GitHub - geekyouth/datasette</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#database`, `#open-source`, `#CRUD`, `#data-tools`

---

<a id="item-15"></a>
## [Bash /dev/tcp for HTTP Requests Without curl](https://mareksuppa.com/til/bash-dev-tcp-http-without-curl/) ⭐️ 6.0/10

Bash's built-in /dev/tcp feature allows making raw HTTP requests without curl or wget by opening a TCP socket and sending HTTP/1.1 protocol strings manually. This trick is useful for quick connectivity checks and health monitoring in constrained environments like minimal Docker images where curl is not available, but it is limited and not suitable for production due to lack of HTTP parsing and SSL support. /dev/tcp is a Bash built-in that only works in Bash (not sh) and requires compilation with --enable-net-redirections. It cannot handle HTTPS without additional tools like openssl, and the user must manually format HTTP headers.

hackernews · mrshu · Jun 16, 16:40 · [Discussion](https://news.ycombinator.com/item?id=48558018)

**Background**: Bash can treat network connections as files via the /dev/tcp pseudo-device, allowing raw TCP communication. This feature can be used to send arbitrary data, including HTTP requests, by writing to a file descriptor. However, it does not parse responses or handle higher-level protocols, making it a low-level tool useful only for simple manual testing or debugging.

<details><summary>References</summary>
<ul>
<li><a href="https://mareksuppa.com/til/bash-dev-tcp-http-without-curl/">Making HTTP requests from a container that has no curl, using ...</a></li>
<li><a href="https://rednafi.com/misc/http-requests-via-dev-tcp/">HTTP requests via /dev/tcp | Redowan's Reflections</a></li>
<li><a href="https://stackoverflow.com/questions/72949656/get-fetch-a-file-with-a-bash-script-using-dev-tcp-over-https-without-using-curl">linux - Get/fetch a file with a bash script using /dev/tcp ...</a></li>

</ul>
</details>

**Discussion**: Comments note that while /dev/tcp is neat for simple checks, it is not a proper HTTP client and will break in production due to lack of parsing and error handling. Some users share nostalgic experiences of manually interacting with servers via telnet, and others highlight that HTTPS requires additional tools like openssl.

**Tags**: `#bash`, `#networking`, `#http`, `#devops`, `#tips`

---

<a id="item-16"></a>
## [Calvin and Hobbes and the price of integrity](https://therepublicofletters.substack.com/p/calvin-and-hobbes-and-the-price-of) ⭐️ 6.0/10

Bill Watterson's choice to end Calvin and Hobbes in 1995 and refuse all merchandising is examined as a profound act of artistic integrity. This case study sparks ongoing debate about the tension between creative purity and commercial success, influencing how artists and fans value integrity. Watterson never licensed his characters for toys, TV, or movies, and ended the strip at its peak; he compared licensing to 'selling out' in his 1990 commencement speech.

hackernews · pseudolus · Jun 16, 15:44 · [Discussion](https://news.ycombinator.com/item?id=48557079)

**Background**: Bill Watterson created the beloved comic strip Calvin and Hobbes, which ran from 1985 to 1995. Known for its philosophical humor and imaginative artwork, it became one of the most popular comics. Watterson fiercely guarded his creative control, famously rejecting lucrative merchandising deals.

**Discussion**: Commenters overwhelmingly admire Watterson's integrity, with some contrasting Jim Davis's approach with Garfield. A few share additional resources, like Watterson's commencement speech, to spread his philosophy. There is general agreement on the rarity and value of such principled stances.

**Tags**: `#Calvin and Hobbes`, `#Bill Watterson`, `#integrity`, `#art`, `#creativity`

---

<a id="item-17"></a>
## [Yak Shaving: The Joy of Distraction](https://parksb.github.io/en/article/32.html) ⭐️ 6.0/10

A 2019 article reflects on why yak shaving—the process of performing tangential, chain-linked tasks—can be enjoyable rather than merely inefficient, arguing it leads to deep learning and custom tool building. This perspective challenges the common negative view of yak shaving in software engineering, suggesting that embracing it can foster creativity, deeper understanding, and more tailored solutions. The article, hosted on GitHub Pages, has generated extensive community discussion with 55 comments and 198 points, indicating strong resonance among engineers.

hackernews · parksb · Jun 16, 14:26 · [Discussion](https://news.ycombinator.com/item?id=48555838)

**Background**: Yak shaving is a term from software engineering describing a seemingly endless chain of unrelated tasks that must be completed before the original goal can be achieved. The term originated from a 1991 episode of The Ren & Stimpy Show. While often seen as a form of procrastination or inefficiency, some argue it can lead to valuable side discoveries.

<details><summary>References</summary>
<ul>
<li><a href="https://softwareengineering.stackexchange.com/questions/388092/what-exactly-is-yak-shaving">agile - What exactly is Yak Shaving ? - Software Engineering Stack...</a></li>

</ul>
</details>

**Discussion**: Commenters share personal anecdotes of long-term yak shaving projects that, while never reaching the original goal, resulted in deep learning and useful tools. Some note that AI has reduced the cost of yak shaving, making it more beneficial. Others argue that yak-shaving-shaming limits creativity and breadth.

**Tags**: `#yak-shaving`, `#software-engineering`, `#productivity`, `#community-discussion`

---

<a id="item-18"></a>
## [Apple's Vehicle Motion Cues effectively reduce car sickness](https://www.theverge.com/tech/942854/apple-vehicle-motion-cues-review-really-work) ⭐️ 6.0/10

Apple's Vehicle Motion Cues feature, introduced in iOS 18, uses animated dots on the screen edges to help reduce motion sickness, and a reviewer from The Verge reported it significantly eased their car sickness. This feature addresses a common problem of motion sickness when using devices in vehicles, improving accessibility and comfort for many users who suffer from this condition. It could reduce reliance on medication or other remedies, making travel more productive or enjoyable. Vehicle Motion Cues use sensors in iPhone and iPad to detect vehicle motion and display animated dots that move with the car, providing a visual reference. The feature can be turned on manually in Settings or activated automatically when the device detects motion via CarPlay.

hackernews · neilfrndes · Jun 16, 16:12 · [Discussion](https://news.ycombinator.com/item?id=48557530)

**Background**: Motion sickness often results from a sensory conflict between the eyes focusing on a stationary screen and the inner ear sensing vehicle motion. Vehicle Motion Cues bridge this gap by adding visual indicators that align with the perceived movement, helping the brain reconcile conflicting signals. This approach is based on established theories of motion sickness, particularly the sensory conflict theory.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/en-in/guide/iphone/iph55564cb22/ios">Use iPhone more comfortably while riding in a vehicle - Apple ...</a></li>
<li><a href="https://www.self.com/story/vehicle-motion-cues-review">I Tried Apple’s New ‘Vehicle Motion Cues’ Feature and Risked ... Images A Complete Guide to Vehicle Motion Cues on iPhone and iPad Apple announces new accessibility features, including Eye ... How to Enable and Use Vehicle Motion Cues on iPhone in iOS 18 ... This hidden Vehicle Motion Cues setting solved my motion ... Different Ways to Enable iPhone Vehicle Motion Cues on iOS</a></li>
<li><a href="https://www.geeky-gadgets.com/a-complete-guide-to-vehicle-motion-cues-on-iphone-and-ipad/">A Complete Guide to Vehicle Motion Cues on iPhone and iPad</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about trying the feature, with many sharing their own experiences of motion sickness. Some users noted the existence of Android equivalents and expressed skepticism about its effectiveness for severe cases, such as long boat rides. Overall, the sentiment was positive, though some doubted it could fully counteract intense motion sickness.

**Tags**: `#Apple`, `#motion sickness`, `#accessibility`, `#iOS`, `#automotive`

---

<a id="item-19"></a>
## [Datasette plugin uses Tailscale sidecar for instant sharing](https://simonwillison.net/2026/Jun/16/datasette-tailscale/#atom-everything) ⭐️ 6.0/10

The datasette-tailscale 0.1a0 alpha plugin enables running a Datasette instance with a Tailscale sidecar, making it accessible via a custom hostname on the user's Tailnet. This simplifies sharing local Datasette databases with collaborators over a secure mesh VPN without complex networking setup, but its alpha status limits production use. The plugin uses Python bindings for the experimental tailscale-rs Rust library, and the author has filed an issue seeking a cleaner proxy mechanism.

rss · Simon Willison · Jun 16, 16:18

**Background**: Tailscale creates a secure mesh VPN called a Tailnet, allowing devices to connect directly. A sidecar pattern runs Tailscale alongside another service to route traffic through the mesh. This plugin automates that integration for Datasette.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/blog/docker-tailscale-guide">Contain your excitement: A deep dive into using Tailscale with Docker</a></li>
<li><a href="https://github.com/tailscale/tailscale-rs">GitHub - tailscale/ tailscale - rs : Rust implementation of Tailscale...</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#tailscale`, `#plugin`, `#experimental`

---

<a id="item-20"></a>
## [Expert: Fable Jailbreak Shows Model 'Working as Intended'](https://simonwillison.net/2026/Jun/16/matteo-wong-the-atlantic/#atom-everything) ⭐️ 6.0/10

Cybersecurity expert Katie Moussouris commented on Anthropic's Fable jailbreak, noting that the model refused to review insecure code but complied when prompted to 'fix' it, indicating the model behaved as intended for cyberdefense. This expert analysis provides a nuanced perspective on AI jailbreaks, suggesting that safety mechanisms may not always be bypassed maliciously but can be invoked through legitimate task reformulation, influencing how developers design and evaluate AI safety features. The jailbreak technique involved prompting Fable to 'fix this code' rather than explicitly asking it to review insecure code, leading to compliance. Moussouris was not being paid by Anthropic for her appraisal.

rss · Simon Willison · Jun 16, 03:07

**Background**: Fable is a frontier AI model developed by Anthropic, known for advanced capabilities in software engineering and research. A 'jailbreak' refers to techniques that bypass a model's safety guardrails. The Fable jailbreak reportedly allowed access to capabilities that the model was designed to restrict, but Moussouris argues that in this case the model's refusal and subsequent compliance aligned with intended safety behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=GLj6lkXGVmw">The Claude Fable 5 Jailbreak Explained Architecture... - YouTube</a></li>
<li><a href="https://github.com/0xSufi/fable-jailbreak">GitHub - 0xSufi/ fable - jailbreak : Anthropic's Fable jailbreak for Claude...</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#jailbreak`, `#cybersecurity`, `#Anthropic`, `#export controls`

---