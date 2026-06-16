---
layout: default
title: "Horizon Summary: 2026-06-16 (EN)"
date: 2026-06-16
lang: en
---

> From 40 items, 16 important content pieces were selected

---

1. [vLLM v0.23.0 Released with DeepSeek-V4 and MRv2 Enhancements](#item-1) ⭐️ 8.0/10
2. [Backdoor in LinkedIn Job Offer via npm Prepare Script](#item-2) ⭐️ 8.0/10
3. [Iroh 1.0: Peer-to-Peer Networking Library Released](#item-3) ⭐️ 8.0/10
4. [Ask HN: Users share local model setups for coding](#item-4) ⭐️ 8.0/10
5. [Fox to Acquire Roku](#item-5) ⭐️ 8.0/10
6. [How TimescaleDB Compresses Time-Series Data](#item-6) ⭐️ 8.0/10
7. [Salesforce Acquires Fin for $3.6B to Boost AI Customer Support](#item-7) ⭐️ 8.0/10
8. [AI hasn't replaced software engineers, and likely won't, argue researchers](#item-8) ⭐️ 8.0/10
9. [Banned Book Library in a Wi-Fi Smart Light Bulb](#item-9) ⭐️ 7.0/10
10. [Homelab AI Dev Platform: Forgejo + Opencode Walkthrough](#item-10) ⭐️ 7.0/10
11. [Hetzner Announces Major Price Hikes for Cloud Servers](#item-11) ⭐️ 7.0/10
12. [Commander Keen Engine White Paper: Smooth Scrolling Revolution](#item-12) ⭐️ 7.0/10
13. [Copper transport drug restores memory in Alzheimer's mice](#item-13) ⭐️ 7.0/10
14. [Anthropic models offline due to personality clashes, export controls](#item-14) ⭐️ 7.0/10
15. [TinyWind Game Criticized for Inaccurate Wind Physics](#item-15) ⭐️ 6.0/10
16. [US battery output hits record, but lags China and may include primary batteries](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [vLLM v0.23.0 Released with DeepSeek-V4 and MRv2 Enhancements](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 8.0/10

vLLM v0.23.0 is now available, featuring major improvements for DeepSeek-V4 including sparse MLA metadata decoupling, EPLB support, and multi-token prediction enhancements, alongside the expansion of Model Runner V2 to Llama and Mistral dense models by default. This release significantly boosts inference efficiency and scalability for state-of-the-art models like DeepSeek-V4 and popular dense architectures, directly benefiting developers and organizations deploying large language models in production with lower latency and higher throughput. DeepSeek-V4 gains TRTLLM-gen attention kernel, selective prefix-cache retention, and index-share for DSA MTP; Model Runner V2 adds FlashInfer sampler and breakable CUDA graphs, and the experimental Rust frontend now supports streaming generate and dynamic LoRA endpoints.

github · khluu · Jun 15, 05:27

**Background**: vLLM is a high-throughput, memory-efficient LLM inference and serving engine. DeepSeek-V4 is a large Mixture-of-Experts (MoE) model with Multi-Head Latent Attention (MLA) and Multi-Token Prediction (MTP). Model Runner V2 (MRv2) is vLLM's next-generation execution framework for optimized inference. EPLB (Expert Parallelism Load Balancer) helps balance expert distribution across GPUs for MoE models.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/deepseek_v4/sparse_mla/">sparse _ mla - vLLM</a></li>
<li><a href="https://github.com/deepseek-ai/EPLB">GitHub - deepseek-ai/EPLB: Expert Parallelism Load Balancer</a></li>
<li><a href="https://medium.com/@bingqian/understanding-multi-token-prediction-mtp-in-deepseek-v3-ed634810c290">Understanding Multi - Token Prediction ( MTP ) in DeepSeek -V3 | by Bing</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM`, `#inference`, `#deepseek`, `#model runner`

---

<a id="item-2"></a>
## [Backdoor in LinkedIn Job Offer via npm Prepare Script](https://roman.pt/posts/linkedin-backdoor/) ⭐️ 8.0/10

A LinkedIn recruiter from a crypto startup sent a GitHub repository for review that contained a backdoor executed automatically via the npm 'prepare' script during dependency installation. This incident highlights a novel social engineering vector combining LinkedIn job scams with npm supply chain attacks, potentially compromising many developers who trust job-related code reviews. The backdoor was hidden in commented-out test code and executed via npm's 'prepare' script, which runs automatically after 'npm install' without user interaction.

hackernews · lwhsiao · Jun 15, 20:00 · [Discussion](https://news.ycombinator.com/item?id=48546294)

**Background**: The npm 'prepare' script is a lifecycle hook that runs before publishing a package and after 'npm install' to prepare the package. A supply chain attack targets less secure elements in the software supply chain, such as dependencies, to infiltrate a target system. This attack exploited developers' trust in recruiter-sent code and the automatic execution of npm scripts.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.npmjs.com/cli/v8/using-npm/scripts/?v=true">scripts | npm Docs</a></li>
<li><a href="https://stackoverflow.com/questions/44499912/why-is-npm-running-prepare-script-after-npm-install-and-how-can-i-stop-it">node.js - Why is npm running prepare script after npm install, and how ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack</a></li>

</ul>
</details>

**Discussion**: Commenters described the act as criminal and called for better cybercrime reporting channels. Some shared similar experiences, while others criticized LinkedIn's requirement for job applications. One commenter noted that antivirus might not catch such a backdoor.

**Tags**: `#security`, `#backdoor`, `#npm`, `#linkedin`, `#supply chain attack`

---

<a id="item-3"></a>
## [Iroh 1.0: Peer-to-Peer Networking Library Released](https://www.iroh.computer/blog/v1) ⭐️ 8.0/10

Iroh 1.0 has been released as a stable version of the Rust library that enables peer-to-peer QUIC connections identified by public keys instead of IP addresses. This release provides application developers with a decentralized networking primitive, reducing reliance on central servers and making it easier to build peer-to-peer applications with direct connections. Iroh natively supports IPv4, IPv6, and relay transports, and allows custom transport implementations. It offers opt-in observability and network diagnostics, and includes composable protocols.

hackernews · chadfowler · Jun 15, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48542480)

**Background**: Traditional networking relies on IP addresses and DNS, which require central infrastructure. Iroh uses public keys for addressing, enabling direct connections even when devices change networks. It builds on QUIC and can use relays for NAT traversal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.iroh.computer/">Iroh</a></li>
<li><a href="https://github.com/n0-computer/iroh">GitHub - n0-computer/ iroh : IP addresses break, dial keys ...</a></li>
<li><a href="https://deepwiki.com/n0-computer/iroh">n0-computer/ iroh | DeepWiki</a></li>

</ul>
</details>

**Discussion**: Community members described Iroh as 'Tailscale at the application layer' and debated its advantages over embedding Tailscale. Developers appreciated the custom transport support, while some questioned the need for yet another networking approach over existing IP-based solutions.

**Tags**: `#peer-to-peer`, `#networking`, `#library`, `#release`, `#distributed-systems`

---

<a id="item-4"></a>
## [Ask HN: Users share local model setups for coding](https://news.ycombinator.com/item?id=48542100) ⭐️ 8.0/10

An Ask HN post has garnered extensive community responses detailing how developers have replaced cloud-based coding assistants like Claude and GPT with local models such as Qwen, achieving satisfactory performance and privacy benefits. This discussion highlights a growing trend toward local LLMs for coding, driven by privacy concerns and cost savings, and provides practical benchmarks and configurations that can guide others considering the switch. Common setups include using Qwen 3.6 35B models with a Pi coding harness or llama.cpp, achieving around 150 tokens per second on dual RTX 3090s, though users note that local models are not as capable as frontier models like Codex.

hackernews · cloudking · Jun 15, 14:46

**Background**: Local LLMs run on personal hardware without internet connectivity, offering privacy and avoiding subscription fees. Tools like Ollama, llama.cpp, and Continue extension enable integration with code editors. Tokens per second (tok/s) is a key performance metric for inference speed.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@walterdeane/running-a-local-llm-for-code-assistance-dea64748041a">Running a Local LLM for Code Assistance | by Walter Deane | Medium</a></li>
<li><a href="https://dev.to/anita_ihuman/best-offline-ai-coding-assistant-how-to-run-llms-locally-without-internet-2bah">Best Offline AI Coding Assistant: How to Run LLMs Locally Without Internet - DEV Community</a></li>
<li><a href="https://www.baseten.co/blog/comparing-tokens-per-second-across-llms/">Comparing tokens per second across LLMs</a></li>

</ul>
</details>

**Discussion**: The community is largely positive, with many sharing successful swaps and specific hardware setups. Some emphasize that local models still lag behind the best cloud models in intelligence but are sufficient for many tasks. A few commenters express skepticism about the true extent of replacement.

**Tags**: `#local LLM`, `#coding assistant`, `#AI`, `#privacy`, `#Qwen`

---

<a id="item-5"></a>
## [Fox to Acquire Roku](https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9) ⭐️ 8.0/10

Fox Corporation is reportedly in talks to acquire Roku, the popular streaming platform that powers millions of smart TVs and streaming devices. This acquisition would give Fox direct access to Roku's large user base (roughly 30-50% of US households), raising concerns about media consolidation and potential harm to the service-agnostic nature of the platform. Roku has historically maintained a hardware-agnostic approach, but recent moves into original content and in-platform ads have already strained that neutrality; a Fox acquisition could accelerate bias toward Fox-owned content.

hackernews · thm · Jun 15, 12:50 · [Discussion](https://news.ycombinator.com/item?id=48540499)

**Background**: Roku is a leading streaming platform that provides hardware (streaming sticks, smart TVs) and a software interface to access various streaming services. Fox is a major media conglomerate owning news, sports, and entertainment networks. Media consolidation in the streaming space has been a growing trend, with companies like Disney and Warner Bros. Discovery also pursuing vertical integration.

**Discussion**: Commenters express strong pessimism, fearing Fox will compromise Roku's neutral platform by pushing Fox News and other Fox content. Many have already moved to alternative devices like Nvidia Shield with custom launchers to avoid ads and bias.

**Tags**: `#acquisition`, `#streaming`, `#Roku`, `#Fox`, `#media consolidation`

---

<a id="item-6"></a>
## [How TimescaleDB Compresses Time-Series Data](https://roszigit.com/en/blog/timescaledb-compression-hypercore) ⭐️ 8.0/10

TimescaleDB achieves high compression ratios for time-series data by using a hybrid row-columnar storage engine called Hypercore and type-aware compression algorithms such as delta-of-delta and Simple-8b with run-length encoding. This compression method can reduce storage costs by up to 98% for time-series workloads, making PostgreSQL viable for large-scale IoT, monitoring, and analytics applications where storage efficiency is critical. The compression is not automatic; users must configure compression settings and add a compression policy to schedule it. Different algorithms are applied based on data type: delta-of-delta for timestamps, Simple-8b for integers, etc.

hackernews · lkanwoqwp · Jun 15, 17:29 · [Discussion](https://news.ycombinator.com/item?id=48544451)

**Background**: TimescaleDB is an open-source time-series database built as a PostgreSQL extension. Time-series data, like sensor readings or server metrics, often arrives in high volume and benefits from compression to save storage. Traditional row-based storage is inefficient for such data, so TimescaleDB uses Hypercore, a hybrid row-columnar engine, to switch between row-oriented (for fast inserts) and column-oriented (for efficient compression and analytics) storage. Type-aware compression further optimizes by applying the best algorithm for each data type.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.timescale.com/use-timescale/latest/compression/compression-methods/">Timescale Documentation | About compression methods</a></li>
<li><a href="https://www.tigerdata.com/blog/time-series-compression-algorithms-explained">Time-series compression algorithms , explained | Tiger Data</a></li>

</ul>
</details>

**Discussion**: Community members discussed query performance trade-offs (gopalv noted no silver bullet), with tudorg comparing his own extension deltaX. Robocat criticized the use of 'up to' in the title as misleading. Others referenced historical algorithms like swinging-door and Facebook's Gorilla.

**Tags**: `#TimescaleDB`, `#compression`, `#time-series`, `#PostgreSQL`, `#database`

---

<a id="item-7"></a>
## [Salesforce Acquires Fin for $3.6B to Boost AI Customer Support](https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/?bc=HL) ⭐️ 8.0/10

Salesforce announced its definitive agreement to acquire Fin, formerly Intercom, for approximately $3.6 billion on June 15, 2026. Fin provides an AI-powered customer agent that handles sales and support across the customer journey. This acquisition consolidates the AI customer support agent market and signals Salesforce's intent to compete directly with Sierra, founded by its former co-CEO Bret Taylor. It also prevents independent AI agents from becoming a control point outside the CRM ecosystem. Fin rebranded from Intercom just a month ago, narrowing its focus to AI-powered customer service agents. The deal is Salesforce's largest in the agentic customer experience space, valued at $3.6 billion subject to customary adjustments.

hackernews · colesantiago · Jun 15, 12:08 · [Discussion](https://news.ycombinator.com/item?id=48540126)

**Background**: Intercom was originally a messaging-first customer communication platform, but pivoted to AI agents under the Fin brand. Salesforce is a leading CRM provider that has been expanding its AI capabilities, including through its Einstein platform. The customer support AI agent market is heating up with competitors like Sierra (valued at $15.8B) and Decagon ($4.5B).

<details><summary>References</summary>
<ul>
<li><a href="https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/">Salesforce Signs Definitive Agreement to Acquire Fin</a></li>
<li><a href="https://techcrunch.com/2026/06/15/salesforce-acquires-ai-customer-service-platform-fin-for-3-6b/">Salesforce acquires AI customer service platform Fin for $3.6B</a></li>
<li><a href="https://www.cmswire.com/customer-experience/salesforce-acquires-fin/">Salesforce Agrees to Buy Fin for $3.6 Billion, Largest Agentic CX Deal ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News community expressed mixed feelings: some praised AI customer service when done right (e.g., Starlink example), while others questioned the long-term viability of helpdesk companies given that businesses can now train their own AI agents. One comment noted the timing of the sale after Fin's rebrand, and others pointed out the rivalry with Sierra.

**Tags**: `#acquisition`, `#AI customer support`, `#Salesforce`, `#SaaS`, `#CRM`

---

<a id="item-8"></a>
## [AI hasn't replaced software engineers, and likely won't, argue researchers](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan and Sayash Kapoor published an essay arguing that AI has not caused mass unemployment among software engineers, citing that in the first year of New York's AI disclosure checkbox on WARN Act filings, not a single company checked the box. This challenges the dominant narrative that AI will soon render software engineers obsolete, providing data-driven evidence that the profession's core value — deep human understanding of codebase, business, and environment — remains irreplaceable by current AI tools. The authors identify three real bottlenecks in software engineering that resist automation: deciding what to build, verifying delivered output, and the deep human understanding required for both. AI can assist but not replace these activities.

rss · Simon Willison · Jun 14, 23:54

**Background**: The WARN Act (Worker Adjustment and Retraining Notification Act) requires U.S. employers with 100+ employees to provide 60 days' notice before mass layoffs. In March 2025, New York added an AI disclosure checkbox to these filings, requiring companies to indicate if layoffs are AI-related. The fact that no company checked the box in the first full year provides concrete evidence that AI is not yet driving mass layoffs in software engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WARN_Act">WARN Act</a></li>
<li><a href="https://en.wikipedia.org/wiki/Worker_Adjustment_and_Retraining_Notification_Act_of_1988">Worker Adjustment and Retraining Notification Act of 1988 - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#job market`, `#narrative`, `#data`

---

<a id="item-9"></a>
## [Banned Book Library in a Wi-Fi Smart Light Bulb](https://www.richardosgood.com/posts/banned-book-library/) ⭐️ 7.0/10

A hacker repurposed a Wi-Fi smart light bulb by flashing it with custom firmware to host a library of banned books, accessible via a local web server. This project demonstrates a creative and low-cost method to circumvent censorship by hiding content in everyday IoT devices, potentially empowering free speech in restrictive environments. The bulb uses an ESP8266 chip with SPIFFS storage, allowing it to serve text files like ebooks over Wi-Fi. The firmware is likely based on Tasmota or similar open-source IoT firmware.

hackernews · sohkamyung · Jun 15, 22:37 · [Discussion](https://news.ycombinator.com/item?id=48547985)

**Background**: Many cheap Wi-Fi smart bulbs use the ESP8266 microcontroller, which can be flashed with custom firmware like Tasmota to remove cloud dependency. ESP8266 can also act as a web server serving files from its SPIFFS file system, enabling local file sharing without internet access.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mbreviews.com/how-to-flash-tuya-with-tasmota/">How to flash a Gosund (or other Tuya) smart bulb with ... - MBReviews</a></li>
<li><a href="https://shepherdingelectrons.blogspot.com/2019/04/esp8266-as-spiffs-http-server.html">ESP8266 as a SPIFFs File Server</a></li>
<li><a href="https://tttapa.github.io/ESP8266/Chap12+-+Uploading+to+Server.html">Uploading files to the server</a></li>

</ul>
</details>

**Discussion**: Comments are positive, praising the creativity and comparing the project to PirateBox and LibraryBox. Some discuss the potential for mesh networking and note the importance of such tools as censorship increases.

**Tags**: `#embedded systems`, `#censorship`, `#free speech`, `#IoT`, `#hacking`

---

<a id="item-10"></a>
## [Homelab AI Dev Platform: Forgejo + Opencode Walkthrough](https://rsgm.dev/post/ai-dev-platform/) ⭐️ 7.0/10

A developer published a detailed walkthrough of building a personal AI development platform that integrates local AI models with a self-hosted Git forge (Forgejo) and the opencode coding agent. This demonstrates how developers can create privacy-preserving, local AI-infused development workflows without relying on external cloud services, highly relevant for the homelab and self-hosting communities. The platform uses a persistent opencode server running locally, integrated with Forgejo for issue tracking and pull requests. Community comments highlight alternative approaches like running opencode inside Forgejo action runners.

hackernews · rsgm · Jun 15, 15:09 · [Discussion](https://news.ycombinator.com/item?id=48542433)

**Background**: Forgejo is a self-hosted, lightweight software forge for Git repositories, issue tracking, and CI/CD. Opencode is an open-source AI coding agent that can assist with code generation and review. Combining them allows developers to have an AI assistant integrated into their version control workflow.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Forgejo">Forgejo</a></li>
<li><a href="https://forgejo.org/">Forgejo – Beyond coding. We forge .</a></li>
<li><a href="https://github.com/anomalyco/opencode/">GitHub - anomalyco/ opencode : The open source coding agent.</a></li>

</ul>
</details>

**Discussion**: The community responded enthusiastically, with several users sharing similar setups. One user described running opencode inside Forgejo action runners, while another mentioned using n8n and k3s. Some users raised concerns about context management in multi-round interactions.

**Tags**: `#homelab`, `#AI`, `#development platform`, `#Forgejo`, `#opencode`

---

<a id="item-11"></a>
## [Hetzner Announces Major Price Hikes for Cloud Servers](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers) ⭐️ 7.0/10

Hetzner has announced significant price increases for its cloud server products, with some configurations seeing up to a 3x rise, citing rising hardware costs driven by AI demand. This price hike affects a large community of developers and businesses who rely on Hetzner for affordable cloud hosting, and it reflects a broader industry trend where AI demand is driving up hardware costs, potentially increasing inequality between large and small cloud providers. The adjustments apply to cloud servers specifically, with some configurations tripling in price compared to previous rates. Hetzner attributes the increases to higher costs for RAM and storage components.

hackernews · tuhtah · Jun 15, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48540844)

**Background**: Hetzner is a popular German hosting provider known for offering low-cost dedicated and cloud servers. The surge in AI workloads has increased demand for GPUs and high-bandwidth memory, leading to global hardware shortages and price hikes. Similar price adjustments have been seen across the industry.

**Discussion**: Commenters expressed shock at the magnitude of the increase, with some questioning the justification for a 3x rise. Others linked the trend to AI-driven wealth inequality and noted that hyperscalers like AWS may have better supply chain leverage to keep costs down.

**Tags**: `#cloud hosting`, `#price increase`, `#hardware costs`, `#Hetzner`, `#AI impact`

---

<a id="item-12"></a>
## [Commander Keen Engine White Paper: Smooth Scrolling Revolution](https://forgottenbytes.net/commander_keen.html) ⭐️ 7.0/10

ForgottenBytes has published a detailed white paper analyzing the Commander Keen game engine, focusing on the adaptive tile refresh technique that enabled smooth scrolling on early PC hardware. This white paper matters because it documents a groundbreaking technique that allowed PCs to rival consoles in side-scrolling games, paving the way for future PC games and showcasing John Carmack's early innovation. The white paper explains how adaptive tile refresh used EGA hardware features to perform scrolling in hardware, overcoming the PC's lack of dedicated sprite hardware and achieving smooth movement.

hackernews · mfiguiere · Jun 15, 17:52 · [Discussion](https://news.ycombinator.com/item?id=48544781)

**Background**: In the early 1990s, PCs struggled with side-scrolling games due to limited graphics capabilities compared to consoles like the SNES, which had dedicated sprite processors. John Carmack developed adaptive tile refresh for Commander Keen, cleverly using EGA video memory to achieve smooth scrolling on standard PC hardware. This innovation helped establish id Software as a leading game developer.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Commander_Keen">Commander Keen - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adaptive_tile_refresh">Adaptive tile refresh - Wikipedia</a></li>
<li><a href="https://www.howtogeek.com/704727/30-years-of-vorticons-how-commander-keen-changed-pc-gaming/">30 Years of Vorticons: How Commander Keen Changed PC Gaming</a></li>

</ul>
</details>

**Discussion**: Community members praised the white paper, with references to the book 'Masters of Doom' for historical context and a discussion on the contrast between PC and SNES hardware capabilities. A link to play Commander Keen 4 online was also shared, and the site was compared to the Cosmodoc project.

**Tags**: `#game development`, `#retro computing`, `#video game history`, `#programming`

---

<a id="item-13"></a>
## [Copper transport drug restores memory in Alzheimer's mice](https://www.monash.edu/news/articles/copper-drug-restores-memory-and-clears-toxic-alzheimers-proteins) ⭐️ 7.0/10

Monash University researchers demonstrated that a copper transport drug restores memory and clears toxic amyloid-beta proteins in a mouse model of Alzheimer's disease, suggesting a novel therapeutic mechanism. This finding offers a potential new avenue for Alzheimer's treatment that bypasses the repeated failures of direct amyloid-targeting drugs, by addressing underlying copper dysregulation in the brain. The compound, a mutant copper transporter, corrects abnormal copper distribution—copper accumulation in plaques and deficiency in neurons—and the drug has already undergone safety evaluations for other diseases, facilitating potential rapid translation to human trials.

hackernews · bookofjoe · Jun 15, 14:48 · [Discussion](https://news.ycombinator.com/item?id=48542132)

**Background**: Alzheimer's disease is characterized by amyloid-beta plaques and abnormal copper homeostasis, with copper accumulating in plaques while neurons become copper-deficient. The amyloid hypothesis, which posits that amyloid-beta buildup drives the disease, has been challenged by repeated clinical failures of amyloid-clearing drugs. This study explores correcting copper distribution as an alternative strategy, potentially affecting amyloid production or clearance indirectly.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48542132">Copper transport drug restores memory and clears... | Hacker News</a></li>
<li><a href="https://www.academia.edu/115715222/In_vivo_reduction_of_amyloid_β_by_a_mutant_copper_transporter">(PDF) In vivo reduction of amyloid-β by a mutant copper transporter</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some commenters express caution, noting that amyloid plaque may be a tombstone rather than a cause, and that results are only in mice. Others appreciate the novel mechanism, while a few point out that the drug's safety in humans for other conditions is a promising sign. Personal stories from caregivers highlight the urgency and complexity of the disease.

**Tags**: `#Alzheimer's`, `#copper transport`, `#amyloid-beta`, `#preclinical`, `#neurodegeneration`

---

<a id="item-14"></a>
## [Anthropic models offline due to personality clashes, export controls](https://simonwillison.net/2026/Jun/15/axios-clashes-anthropics/#atom-everything) ⭐️ 7.0/10

An Axios article reveals that personality clashes between Anthropic and the US government led to the suspension of access to its advanced models, Mythos and Fable. Key Anthropic figures including Logan Graham are meeting with the Commerce Department today to address the situation. This incident highlights growing tensions between AI companies and regulators over national security, potentially setting a precedent for how advanced AI models are governed. The outcome could affect global AI development and the balance between innovation and safety. The shutdown was triggered by a jailbreak that the US government deemed a national security risk, though Anthropic classified it as a narrow, non-universal attack. Anthropic's Constitutional Classifiers aim to prevent such jailbreaks, but perfect resistance may be impossible.

rss · Simon Willison · Jun 15, 14:57

**Background**: Anthropic's Mythos is a state-of-the-art model released in April through Project Glasswing, with limited partner access to select organizations like Apple and NVIDIA. Fable is a Mythos-class model made generally available, representing a significant leap in capabilities. The US government issued a directive to suspend access due to export control concerns after a reported jailbreak. Anthropic's Frontier Red Team, led by Logan Graham, evaluates AI safety risks and publicizes findings.

<details><summary>References</summary>
<ul>
<li><a href="https://www.engadget.com/2190934/anthropic-fable-ai-brings-the-capabilities-of-its-unreleased-mythos-model-to-regular-users/">Anthropic's Fable AI brings the capabilities of its unreleased Mythos model to regular users - Engadget</a></li>
<li><a href="https://aimagazine.com/news/fable-5-and-mythos-5-anthropics-mythos-class-models-explained">What Happens When Anthropic's Mythos Class Models go Public? | AI Magazine</a></li>
<li><a href="https://fortune.com/2025/09/04/anthropic-red-team-pushes-ai-models-into-the-danger-zone-and-burnishes-companys-reputation-for-safety/">Anthropic ’s ‘ Red Team ’ pushes its AI models into the danger... | Fortune</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#AI safety`, `#government regulation`, `#export controls`, `#AI policy`

---

<a id="item-15"></a>
## [TinyWind Game Criticized for Inaccurate Wind Physics](https://tinywind.io/) ⭐️ 6.0/10

TinyWind, a pixel-art pirate sailing game, has gained over 380,000 km sailed by players but faces community criticism that its wind physics are not realistic and sailing mechanics lack depth. This highlights the challenge indie developers face in balancing accessibility with realistic simulation, especially for niche topics like sailing. The feedback can guide improvements in physics-based game design. The game claims real wind physics, but players note that sail trim and wind direction interaction is oversimplified, with ships sailing upwind unrealistically fast. The developer has not yet addressed these specific concerns publicly.

hackernews · tinywind · Jun 15, 16:15 · [Discussion](https://news.ycombinator.com/item?id=48543475)

**Background**: Realistic sailing physics in games is notoriously difficult to implement, often requiring complex fluid dynamics and sail models. Many games simplify by using approximate formulas for wind force and sail efficiency, sacrificing accuracy for playability. Indie titles especially struggle to achieve both realism and fun. The community's detailed feedback on TinyWind reflects the nuanced expectations of sailing enthusiasts.

<details><summary>References</summary>
<ul>
<li><a href="https://shaaaanya.medium.com/sailing-game-in-unity-4b2c109469c4">Sailing Game in Unity. Part 1: Buoyancy Physics | by Ivan... | Medium</a></li>
<li><a href="https://gamedev.net/forums/topic/166648-simplified-sail-physics/">(Simplified) Sail physics - Math and Physics - GameDev.net | Forum</a></li>

</ul>
</details>

**Discussion**: The community is divided: some praise the game as a fun and accessible introduction to sailing concepts, while others, especially experienced sailors, find the physics too simplistic and unrealistic. Key criticisms include unclear wind indicators and linear sail angle mechanics that don't reflect real upwind/downwind behavior.

**Tags**: `#gaming`, `#sailing`, `#physics simulation`, `#indie game`, `#hackernews`

---

<a id="item-16"></a>
## [US battery output hits record, but lags China and may include primary batteries](https://fred.stlouisfed.org/series/IPG33591S) ⭐️ 6.0/10

US battery manufacturing output reached record highs according to FRED data, but community comments indicate that China's cell production capacity in 2025 is 1755 GWh compared to the US's 70 GWh, and the data may include primary (non-rechargeable) batteries. While record output is a positive sign for US industrial capacity, the massive gap with China and the inclusion of primary batteries limits its significance for the electric vehicle boom, highlighting the need for accelerated domestic battery production. The FRED series IPG33591S is described as 'durable goods' but may include primary batteries from companies like Energizer; community estimates show US cell production capacity at 70 GWh vs China's 1755 GWh in 2025.

hackernews · epistasis · Jun 15, 20:28 · [Discussion](https://news.ycombinator.com/item?id=48546616)

**Background**: Primary batteries are non-rechargeable batteries used in household items like flashlights, while secondary (rechargeable) batteries power EVs and electronics. The US has historically dominated primary battery production, but the EV boom requires massive scaling of secondary battery manufacturing, in which China leads significantly.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Primary_batteries">Primary batteries</a></li>

</ul>
</details>

**Discussion**: Commenters highlight the stark US-China capacity gap (70 GWh vs 1755 GWh) and question whether the data reflects primary batteries, with one noting that Energizer may account for much of the output. Another suggests the production increase is insufficient for EV needs, while another views it positively for national security.

**Tags**: `#battery manufacturing`, `#energy storage`, `#EVs`, `#industrial output`, `#US-China comparison`

---