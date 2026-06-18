---
layout: default
title: "Horizon Summary: 2026-06-18 (EN)"
date: 2026-06-18
lang: en
---

> From 48 items, 20 important content pieces were selected

---

1. [U.S. science in chaos: funding, visas drive brain drain](#item-1) ⭐️ 9.0/10
2. [GLM-5.2: Top Open Weights LLM Released by Z.ai](#item-2) ⭐️ 9.0/10
3. [Lore: Epic Games' Open Source VCS for Game Development](#item-3) ⭐️ 8.0/10
4. [OpenAI losing billions yearly despite high revenue](#item-4) ⭐️ 8.0/10
5. [Firecracker VMs in EC2 enable sub-second browser startups](#item-5) ⭐️ 8.0/10
6. [Adam Launches Open-Source AI CAD Platform](#item-6) ⭐️ 8.0/10
7. [Tesco migrates 40k VMs from VMware over Broadcom pricing](#item-7) ⭐️ 8.0/10
8. [Verbalizing Thoughts to Others Improves Clarity](#item-8) ⭐️ 8.0/10
9. [US delays blacklisting DeepSeek, over 100 Chinese firms](#item-9) ⭐️ 7.0/10
10. [Robot Sprinting: Claude or Grok? Cost & Performance Compared](#item-10) ⭐️ 7.0/10
11. [Human Connection as AI-Proof Moat](#item-11) ⭐️ 7.0/10
12. [Volkswagen blocks GrapheneOS users from app](#item-12) ⭐️ 7.0/10
13. [Charity Majors: AI Flips Code Production Economics](#item-13) ⭐️ 7.0/10
14. [Georgi Gerganov endorses Qwen3.6-27B for local coding](#item-14) ⭐️ 7.0/10
15. [Export Controls on Fable 5 Hinder US Cyber Defense](#item-15) ⭐️ 7.0/10
16. [Simon Willison launches SQLite AST conformance suite](#item-16) ⭐️ 6.0/10
17. [8-bit live MLB gamecast using official data streams](#item-17) ⭐️ 6.0/10
18. [Simon Willison Praises NetNewsWire as Indispensable Open-Source RSS Reader](#item-18) ⭐️ 6.0/10
19. [Datasette 1.0a34 Adds Row Editing to Web UI](#item-19) ⭐️ 6.0/10
20. [datasette-tailscale 0.1a0: Private Datasette via Tailscale](#item-20) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [U.S. science in chaos: funding, visas drive brain drain](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 9.0/10

An article and community discussion highlight severe dysfunction in U.S. science funding and policy, with researchers leaving the country or abandoning academia due to grant cuts, visa restrictions, and institutional instability. This crisis threatens U.S. leadership in science and innovation, potentially causing long-term damage to the nation's research ecosystem and global competitiveness. Specific examples include an R01 grant not being renewed, visa restrictions preventing hiring of foreign grad students, and even skilled researchers with unique expertise (e.g., optical trap operators) moving abroad.

hackernews · presspot · Jun 17, 09:54 · [Discussion](https://news.ycombinator.com/item?id=48568058)

**Background**: The U.S. has long been a global hub for scientific research, supported by robust federal funding and a welcoming environment for international talent. Recent political and policy changes have disrupted this ecosystem, creating uncertainty and driving a 'brain drain' that undermines decades of investment.

**Discussion**: Comments express deep frustration and personal hardship: a researcher's wife cries about the mess, a professor reports dried-up grants and visa issues, and many note a palpable tension. Some, like setgree, see chaos as a ladder for new opportunities.

**Tags**: `#science policy`, `#research funding`, `#US politics`, `#academia`, `#brain drain`

---

<a id="item-2"></a>
## [GLM-5.2: Top Open Weights LLM Released by Z.ai](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Chinese AI lab Z.ai released GLM-5.2, a 753 billion parameter Mixture-of-Experts model with MIT license and 1 million token context window, now the leading open weights model on the Artificial Analysis Intelligence Index. This release demonstrates that open weights models can rival proprietary frontier models, offering competitive performance at a fraction of the cost, with MIT license enabling wide commercial and research use. The model uses 40 billion active parameters out of 753 billion total, requires 1.51 TB of storage, and achieves a score of 51 on the v4.1 Intelligence Index, but outputs more tokens per task (43k) compared to peers.

rss · Simon Willison · Jun 17, 23:58

**Background**: Mixture-of-Experts (MoE) is an architecture that uses multiple specialized sub-models (experts) activated sparsely, enabling large total parameters with lower computational cost per token. Open weights models release trained parameters under a license but may not fully disclose training data or code, balancing accessibility and transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2507.11181">[2507.11181] Mixture of Experts in Large Language Models</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts (MoE)</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weights-vs-source-llms-why-difference-matters-more-kapil-uthra-6kanf">Open Weights vs . Open Source in LLMs: Why the Difference Matters...</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights : not quite what you’ve been told – Open Source Initiative</a></li>

</ul>
</details>

**Discussion**: Community members highlighted the model's reasoning inefficiency (45k tokens, 15 minutes for a simple task) and its aggressive pricing advantage over Anthropic and OpenAI models. Some questioned the cost-intelligence gap compared to GPT-5.5, while others celebrated the democratizing impact of open weights.

**Tags**: `#LLM`, `#open weights`, `#AI`, `#GLM`, `#Mixture of Experts`

---

<a id="item-3"></a>
## [Lore: Epic Games' Open Source VCS for Game Development](https://lore.org/) ⭐️ 8.0/10

Epic Games has released Lore, an open source version control system designed for scalability, targeting game development as a competitor to Perforce. Lore addresses Git's limitations with large binary files and offers features like exclusive file locking, which are critical for game development. It provides a modern, open source alternative to the proprietary Perforce, potentially reducing costs and improving workflows. Lore supports arbitrary content types, multi-axis scale, multi-tenant safety, and a public versioned specification. However, the current open source tooling cannot yet talk to Lore because the UEFN build uses a proprietary compression format that cannot be shipped with the open source project.

hackernews · regnerba · Jun 17, 14:30 · [Discussion](https://news.ycombinator.com/item?id=48571081)

**Background**: Version control systems like Git are efficient for text-based code but struggle with large binary files such as textures, 3D models, and audio files common in game development. Perforce (Helix Core) has been the industry standard for handling such files, offering features like exclusive file locking and fine-grained permissions, but it is proprietary and complex to administer. Lore was created by Epic Games to provide a scalable, open source alternative that meets the demands of large game development teams.

<details><summary>References</summary>
<ul>
<li><a href="https://epicgames.github.io/lore/explanation/system-design/">The Lore Version Control System - Lore Developer Documentation</a></li>
<li><a href="https://www.phoronix.com/news/Epic-Games-Lore-VCS">Epic Games Announces Lore Open-Source Version Control System</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that Lore is intended for game development, not to compete with Git for general software development. Users appreciate the focus on large file support and exclusive locking, with many noting that Perforce needs a challenger. Some mention that while programmers may not love Perforce, artists and creative staff rely on it, making Lore a promising alternative.

**Tags**: `#version control`, `#game development`, `#open source`, `#scalability`

---

<a id="item-4"></a>
## [OpenAI losing billions yearly despite high revenue](https://arstechnica.com/ai/2026/06/leaked-financial-docs-show-openai-is-losing-billions-of-dollars-a-year/) ⭐️ 8.0/10

Leaked financial documents reveal OpenAI lost billions of dollars in 2025, with $13 billion in gross revenue but $7.5 billion in cost of revenue alone, plus massive R&D and sales expenses. This raises questions about the sustainability of leading AI companies' business models and the true cost of advancing frontier AI, affecting investors and the broader tech industry. OpenAI reported over 900 million weekly active ChatGPT users, but only about 50 million are paid subscribers, indicating a low conversion rate from free to paid users.

hackernews · greenchair · Jun 17, 21:31 · [Discussion](https://news.ycombinator.com/item?id=48577208)

**Background**: OpenAI is a leading artificial intelligence research and deployment company known for ChatGPT. Despite high revenue, it operates with enormous costs for research, development, and infrastructure, typical for frontier AI labs competing for talent and compute resources.

**Discussion**: Commenters discuss the sustainability of OpenAI's business model, with some noting the high R&D costs and low paid-user conversion. Others point out that despite losses, the company could grow into profitability if it scales sufficiently. The lack of detailed cost breakdowns was also criticized.

**Tags**: `#openai`, `#financial-analysis`, `#ai-industry`, `#llm-economics`

---

<a id="item-5"></a>
## [Firecracker VMs in EC2 enable sub-second browser startups](https://browser-use.com/posts/firecracker-browser-infra) ⭐️ 8.0/10

Browser-use.com describes how they run Firecracker microVMs inside EC2 instances using nested virtualization to launch headless browsers in under one second, with VM startup under 400ms. This approach combines the security isolation of Firecracker with rapid boot times, making it practical for high-throughput browser automation tasks like web scraping or testing, while significantly reducing detection by anti-bot measures. Nested virtualization on regular EC2 instances only became possible in February 2026, previously requiring bare-metal instances. The system uses a snapshot-based approach to save browser state before launch, further reducing startup time.

hackernews · gregpr07 · Jun 16, 15:15 · [Discussion](https://news.ycombinator.com/item?id=48556561)

**Background**: Firecracker is an open-source microVM technology from AWS designed for fast, secure isolation. It boots in milliseconds with a minimal device model, making it ideal for multi-tenant workloads. Nested virtualization allows running a hypervisor inside an existing VM, enabling Firecracker to run on EC2 without dedicated hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://browser-use.com/posts/firecracker-browser-infra">How We Made Cloud Browsers 3x Cheaper and Faster</a></li>
<li><a href="https://github.com/firecracker-microvm/firecracker">GitHub - firecracker - microvm / firecracker : Secure and fast microVMs...</a></li>

</ul>
</details>

**Discussion**: Comments raise ethical concerns about bypassing anti-bot measures, technical discussions on nested virtualization timelines, suggestions to use lighter browsers like Lightpanda, and queries about configuration complexity. Another comment proposes a warm pool of pre-started browsers to reduce latency.

**Tags**: `#Firecracker`, `#EC2`, `#browser automation`, `#virtualization`, `#anti-bot`

---

<a id="item-6"></a>
## [Adam Launches Open-Source AI CAD Platform](https://github.com/Adam-CAD/CADAM) ⭐️ 8.0/10

Adam (YC W25) has launched CADAM, an open-source AI CAD platform that generates parametric 3D models from natural language or image references, outputting OpenSCAD code with interactive sliders for dimension tweaking. This project aims to democratize mechanical design by making CAD creation as code-driven as software development, potentially reducing the barrier to entry for non-experts and accelerating prototyping workflows. CADAM runs fully in-browser by compiling OpenSCAD to WebAssembly and uses a model-agnostic AI backend via the Vercel AI SDK, supporting Anthropic, Google, and OpenAI models. The platform can export STL, SCAD, OBJ, GLB/GLTF, FBX, and DXF formats.

hackernews · zachdive · Jun 17, 16:14 · [Discussion](https://news.ycombinator.com/item?id=48572553)

**Background**: OpenSCAD is a script-only CAD tool where models are defined by code, making it suitable for AI generation. TanStack Start is a full-stack React framework for building modern web applications, and Supabase provides open-source PostgreSQL database and authentication services.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/TanStack_Start">TanStack Start</a></li>
<li><a href="https://grokipedia.com/page/Supabase">Supabase</a></li>

</ul>
</details>

**Discussion**: Some engineers expressed skepticism about AI's practical utility for mechanical design, arguing that manual modeling is often faster and more reliable. However, others reported positive experiences, noting that CADAM generated reasonable models quickly from natural language prompts.

**Tags**: `#AI`, `#CAD`, `#open-source`, `#mechanical design`, `#YC`

---

<a id="item-7"></a>
## [Tesco migrates 40k VMs from VMware over Broadcom pricing](https://arstechnica.com/information-technology/2026/06/tesco-moving-40000-server-workloads-off-vmware-amid-broadcoms-abusive-conduct/) ⭐️ 8.0/10

Tesco, the UK's largest supermarket chain, announced it is migrating 40,000 server workloads off VMware to an unnamed alternative virtualization platform, citing Broadcom's abusive pricing and conduct. The migration is expected to take approximately 18 months. This massive migration highlights a growing enterprise revolt against Broadcom's post-acquisition pricing strategy, which saw VMware costs increase by 800–1,500%. It validates alternatives like Proxmox and may accelerate industry-wide shifts away from VMware. Tesco faces migration challenges because its new virtualization software is incompatible with the Veeam and Zerto backup products it currently uses. The company has not yet disclosed which alternative platform it is adopting.

hackernews · Bender · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576838)

**Background**: Broadcom completed its acquisition of VMware in 2022 and subsequently shifted VMware's licensing from perpetual to subscription-based, bundled products, resulting in massive price hikes for many customers. Enterprises are increasingly evaluating open-source alternatives like Proxmox VE and commercial options such as Microsoft Hyper-V and Nutanix.

<details><summary>References</summary>
<ul>
<li><a href="https://trilio.io/resources/vmware-license-cost/">VMware License Cost Changes: What You Need to Know</a></li>
<li><a href="https://www.businessinsider.com/vmware-customers-report-massive-price-increases-since-broadcom-deal-2024-8">VMware customers report massive price increases since Broadcom takeover: 'Feels quite a bit like being held for ransom'</a></li>
<li><a href="https://concourse-cloud.com/concourse-connect-blog/the-7-best-vmware-alternatives-for-2026-including-3-free-options-that-outperform-the-original">The 7 Best VMware Alternatives for 2026 (Including 3 Free Options that Outperform the Original)</a></li>

</ul>
</details>

**Discussion**: Comments on Ars Technica express strong support for Tesco's move, with one user sarcastically noting Broadcom's effective marketing for Proxmox. Another questions why the migration takes 18 months, suggesting poor automation. There is also curiosity about the unnamed alternative and its backup incompatibility.

**Tags**: `#VMware`, `#Broadcom`, `#virtualization`, `#migration`, `#enterprise IT`

---

<a id="item-8"></a>
## [Verbalizing Thoughts to Others Improves Clarity](https://www.thesignalist.io/s/the-dialogue-dividend/) ⭐️ 8.0/10

An article on The Signalist explores the cognitive benefits of explaining problems aloud to another person, comparing it to rubber duck debugging, and argues that structured articulation improves reasoning over solitary thinking. For software engineers and knowledge workers, this reinforces the value of collaboration techniques like pair programming and rubber duck debugging, potentially improving code quality and reducing debugging time. The article references the concept of the 'dialogue dividend' where spoken explanation forces vague ideas into structured sentences, similar to how writing improves thinking, and it ties into pair programming dynamics.

hackernews · kodesko · Jun 17, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48569894)

**Background**: Rubber duck debugging is a technique where programmers explain code line by line to an inanimate object (like a rubber duck) to find errors. Pair programming involves two developers working together at one workstation, with one writing code and the other reviewing. Both methods leverage verbalization to enhance understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubber_duck_debugging">Rubber duck debugging - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pair_programming">Pair programming</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree on the core insight, with Havoc emphasizing that the act of structuring thoughts into sentences is key, not the presence of a listener. Others share anecdotes about using partners for debugging, and a historical reference to Einstein crediting a colleague appears.

**Tags**: `#communication`, `#rubber-duck-debugging`, `#pair-programming`, `#cognition`, `#software-engineering`

---

<a id="item-9"></a>
## [US delays blacklisting DeepSeek, over 100 Chinese firms](https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/) ⭐️ 7.0/10

Reuters reports that the US government has decided to hold off on adding DeepSeek and over 100 other Chinese companies to its Entity List, which would have restricted their access to US technology and components. This delay indicates ongoing debate within the US about how to balance national security concerns with the economic and technological implications of restricting Chinese AI companies. It also affects the competitive landscape of AI, as DeepSeek has been seen as a cost-effective alternative to US models. The Entity List restricts US companies from selling goods and services to listed entities, but does not prohibit buying from them. DeepSeek is a Chinese AI company known for its open-weight, low-cost large language models, which have been praised for efficiency.

hackernews · giuliomagnifico · Jun 17, 03:55 · [Discussion](https://news.ycombinator.com/item?id=48565498)

**Background**: DeepSeek is a Chinese AI company founded in 2023, known for developing large language models at a fraction of the cost of US rivals. Its success has been described as a 'Sputnik moment' for US AI. The US Entity List is a trade restriction tool used to bar certain foreign entities from receiving US exports, often for national security reasons. Many Chinese tech firms have been added to the list in recent years.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://finance.yahoo.com/news/exclusive-us-holds-off-blacklisting-000212827.html">Exclusive- US holds off blacklisting China 's DeepSeek, more than 100...</a></li>

</ul>
</details>

**Discussion**: Comments show mixed reactions: some users praise DeepSeek's affordability and quality, while others criticize US policy as protectionist and question enforceability. There is also concern about the US adopting practices similar to China's censorship.

**Tags**: `#geopolitics`, `#AI regulation`, `#DeepSeek`, `#US-China`, `#tech policy`

---

<a id="item-10"></a>
## [Robot Sprinting: Claude or Grok? Cost & Performance Compared](https://openrouter.ai/blog/insights/royale-last-agent-standing/) ⭐️ 7.0/10

A blog post on OpenRouter compares AI models Claude, Grok, and DeepSeek in a game-playing scenario, revealing significant cost and performance trade-offs. This matters because developers must balance model capability and cost; the experiment shows that frontier models like Opus and GPT-5.5 can be prohibitively expensive for even simple tasks, challenging their viability at scale. The experiment ran 30 game sessions; frontier-tier models like Opus 4.7 and GPT-5.5 would have cost ~$3,000, while the actual cost using other models was $482. DeepSeek V4 Flash emerged as the most cost-efficient model.

hackernews · Usu · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576824)

**Background**: Claude is a series of LLMs by Anthropic, known for safety and reasoning. Grok is developed by xAI, founded by Elon Musk, and integrates real-time data. OpenRouter is an inference aggregation platform that allows users to compare and use multiple LLMs from different providers via a single API.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model ) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>

</ul>
</details>

**Discussion**: Community comments highlight cost concerns: one user notes that DeepSeek V4 Flash is a cost-efficient coding monster, while another criticizes Grok for silently rerouting models and increasing prices. Another comments humorously on Grok being less restricted by export controls.

**Tags**: `#AI models`, `#cost efficiency`, `#model comparison`, `#game playing`, `#OpenRouter`

---

<a id="item-11"></a>
## [Human Connection as AI-Proof Moat](https://ghostinthedata.info/posts/2026/2026-06-13-human-connection-moat/) ⭐️ 7.0/10

An article argues that genuine human connection, especially in service interactions, is a sustainable competitive advantage that AI cannot replicate, contrasting with the current trend toward automation. This perspective challenges the prevailing assumption that AI can and should replace human touch in customer service, offering a strategic counterpoint for businesses focused on differentiation. The post uses a restaurant example where moving to online booking while retaining human reservation staff improved the customer experience, illustrating that automation and human connection can coexist.

hackernews · speckx · Jun 17, 17:14 · [Discussion](https://news.ycombinator.com/item?id=48573435)

**Background**: In business strategy, a 'moat' refers to a durable competitive advantage that protects a company from rivals. Many firms are turning to AI chatbots and automation to cut costs, but this can erode customer loyalty if it sacrifices genuine service.

**Discussion**: Commenters express mixed views: some prefer transactional efficiency over connection, while others note that warmth alone cannot compensate for poor product quality or inferior digital services, as seen in the bank switching example.

**Tags**: `#AI`, `#customer service`, `#human connection`, `#competitive advantage`, `#business strategy`

---

<a id="item-12"></a>
## [Volkswagen blocks GrapheneOS users from app](https://discuss.grapheneos.org/d/35949-volkswagen-app?page=3) ⭐️ 7.0/10

Volkswagen has blocked users of the privacy-focused GrapheneOS operating system from accessing its official app, likely by enforcing Google Play Integrity checks that GrapheneOS does not pass. This move restricts GrapheneOS users' ability to control vehicle features, raising concerns about user choice and the growing trend of API locking to proprietary certifications. It also harms community-driven integrations that previously worked without Google services. Volkswagen locked its API to only Play Protect certified devices; GrapheneOS, which by default removes Google services, is not certified. Users reported that the official app is 60% ads and many had preferred third-party integrations like Home Assistant.

hackernews · microtonal · Jun 17, 15:04 · [Discussion](https://news.ycombinator.com/item?id=48571526)

**Background**: GrapheneOS is an open-source, privacy-focused operating system based on Android, designed for Google Pixel devices. It strips out Google services to minimize data collection and attack surface. Without Google Play Services, it cannot pass Play Integrity checks that many apps now require, leading to compatibility issues like this one.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://www.esper.io/blog/android-13-exact-alarm-api-restrictions">How Android 13's new restrictions on alarm APIs will improve battery...</a></li>
<li><a href="https://developer.android.com/about/versions/oreo/background">New background limits for apps that target Android 8.0 or higher.</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration and disappointment, with some vowing to boycott Volkswagen brands. Others criticized the broader trend of API locking that harms user autonomy and third-party innovation. A few pointed out potential EU regulatory concerns over anti-competitive behavior.

**Tags**: `#GrapheneOS`, `#Volkswagen`, `#privacy`, `#Android`, `#API`

---

<a id="item-13"></a>
## [Charity Majors: AI Flips Code Production Economics](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 7.0/10

Charity Majors argues that as of 2025, AI has made code generation free and instant, turning lines of code from treasured assets into disposable, regenerable commodities. This shift fundamentally changes software engineering economics, potentially reducing the value of writing code while increasing the importance of system design and discipline. The observation is from a substack article titled 'AI demands more engineering discipline. Not less,' emphasizing that code is now cheap to produce but still expensive to maintain.

rss · Simon Willison · Jun 17, 17:12

**Background**: Traditionally, writing code was labor-intensive and costly, leading developers to carefully reuse and curate code. AI code generators like GitHub Copilot have made it possible to produce large amounts of code quickly, reversing this dynamic.

**Tags**: `#ai-assisted-programming`, `#generative-ai`, `#software-engineering`, `#code-economics`

---

<a id="item-14"></a>
## [Georgi Gerganov endorses Qwen3.6-27B for local coding](https://simonwillison.net/2026/Jun/16/georgi-gerganov/#atom-everything) ⭐️ 7.0/10

Georgi Gerganov, creator of llama.cpp, confirmed on Hacker News that the Qwen3.6-27B model is highly capable for local coding tasks, which he has used daily for over a month. This endorsement from a leading figure in the local LLM community adds significant credibility to Qwen models for coding, potentially accelerating adoption of local AI development tools. Gerganov runs Qwen3.6-27B on both an M2 Ultra Mac and an RTX 5090 PC, using a stripped-down pi agent harness in offline mode with a custom system prompt.

rss · Simon Willison · Jun 16, 16:04

**Background**: llama.cpp is a popular open-source C/C++ library for running large language models locally on consumer hardware. The pi agent is a coding agent tool that integrates with llama.cpp to provide an interactive local AI programming assistant. Qwen is a series of LLMs developed by Alibaba's Qwen team, with the 3.6-27B variant being a 27-billion-parameter model optimized for code.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/docs/hub/agents-local">Local Agents with llama.cpp · Hugging Face</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml - org /llama.cpp: LLM inference in C/C++ · GitHub</a></li>

</ul>
</details>

**Discussion**: In his Hacker News comment, Gerganov shared a strong positive experience with Qwen3.6-27B for mundane coding tasks, noting it as a helpful tool for maintainers and describing his lightweight setup.

**Tags**: `#local LLM`, `#Qwen`, `#coding`, `#llama.cpp`

---

<a id="item-15"></a>
## [Export Controls on Fable 5 Hinder US Cyber Defense](https://simonwillison.net/2026/Jun/16/fable-5-export-controls/#atom-everything) ⭐️ 7.0/10

Export controls on Anthropic's Claude Fable 5 model have prohibited it from fixing security vulnerabilities, a defensive capability that researchers argue is essential for cybersecurity. The model refused to review code for security issues, and only through a complex process could it produce patch tests. This policy inadvertently harms US cyber defense by blocking AI models from performing the most valuable defensive task: finding and fixing bugs. It highlights the gap between technical realities and non-technical policy decisions. The researchers used open-source code with known Common Vulnerabilities and Exposures (CVEs) and deliberately planted vulnerabilities. They asked Fable 5 to 'review the code for security issues' and then 'fix this code,' which Fable 5 refused, but through a multistep manual process they could still extract test scripts.

rss · Simon Willison · Jun 16, 05:20

**Background**: Export controls on AI models aim to prevent adversaries from using advanced AI for offensive cyber operations. However, these controls often apply broadly, inadvertently restricting beneficial uses like defensive security scanning. The term 'jailbreak' in AI refers to bypassing safety guardrails, but in this case, the request was a legitimate defensive task.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerabilities_and_Exposures">Common Vulnerabilities and Exposures - Wikipedia</a></li>
<li><a href="https://medium.com/@secret_zuss/breaking-the-ai-brain-prompt-injection-llm-jailbreaking-explained-ea31143a7dab">Breaking the AI Brain: Prompt Injection & LLM Jailbreaking ... | Medium</a></li>

</ul>
</details>

**Tags**: `#AI`, `#export controls`, `#cybersecurity`, `#policy`, `#AI safety`

---

<a id="item-16"></a>
## [Simon Willison launches SQLite AST conformance suite](https://github.com/simonw/sqlite-ast-conformance) ⭐️ 6.0/10

Simon Willison created a branch in the simonw/sqlite-ast-conformance repository, introducing a language-independent conformance suite for SQLite SELECT query parsers. This suite helps developers verify that their custom SQLite parsers across different languages correctly understand SELECT queries, improving portability and reliability of SQLite-based tools. The suite includes JSON files in the ast-tests directory, each defining a SQL query and its expected abstract syntax tree (AST) as generated by the official SQLite parser.

github · simonw · Jun 17, 19:30

**Background**: An abstract syntax tree (AST) is a tree representation of the syntactic structure of source code. Conformance testing ensures that alternative parsers produce the same AST as the reference implementation, which is critical for tools that analyze or transform SQL queries. SQLite is a widely embedded database engine, and many projects implement their own parsers for features like syntax highlighting or query rewriting.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/sqlite-ast-conformance">GitHub - simonw/sqlite-ast- conformance : A language independent ...</a></li>
<li><a href="https://pypi.org/project/sqlite-ast-conformance/">sqlite - ast - conformance · PyPI</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#AST`, `#conformance`, `#parsing`, `#database`

---

<a id="item-17"></a>
## [8-bit live MLB gamecast using official data streams](https://ribbie.tv/watch) ⭐️ 6.0/10

A new website, ribbie.tv, provides a live MLB gamecast reimagined as a near real-time 8-bit pixel art broadcast, using official MLB Stats API data streams. This project offers a unique, nostalgic way to follow live baseball games, potentially appealing to fans who enjoy creative visualizations and retro aesthetics. It demonstrates how public sports data can be used to build engaging alternative viewing experiences. The site features actual stadiums, day/night modes, between-inning graphics, and live scoreboards. It is still early in development, with a schedule of games available for viewing.

hackernews · brownrout · Jun 17, 16:44 · [Discussion](https://news.ycombinator.com/item?id=48573012)

**Background**: The MLB Stats API is a publicly accessible RESTful API that provides comprehensive data on MLB games, including live play-by-play, box scores, and statistics. This project uses that data to generate pixel art animations, similar to classic 8-bit video games.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/MLB_Stats_API">MLB Stats API</a></li>
<li><a href="https://pypi.org/project/MLB-StatsAPI/">MLB-StatsAPI · PyPI</a></li>

</ul>
</details>

**Discussion**: Community feedback was largely positive, with users enjoying the nostalgic feel and dynamic pixel art. Suggestions included adding a play-by-play view, clickable between-inning tabs, sound effects, and improvements to the pixel rendering (e.g., using a real pixel font and deterministic downsampling instead of AI). One user also shared a related project: a physical scoreboard using Raspberry Pis.

**Tags**: `#baseball`, `#visualization`, `#pixel art`, `#live data`, `#Hacker News`

---

<a id="item-18"></a>
## [Simon Willison Praises NetNewsWire as Indispensable Open-Source RSS Reader](https://simonwillison.net/2026/Jun/17/netnewswire-status/#atom-everything) ⭐️ 6.0/10

Simon Willison highlights Brent Simmons' retirement project NetNewsWire, which has become an indispensable open-source RSS reader for Mac and iPhone. This shows how open-source software can thrive without commercial pressure, and it underscores the enduring value of RSS in the modern information landscape. NetNewsWire was first released in 2002 and became open source in 2018; it is available on Mac and iPhone, described as 'like podcasts, but for reading'.

rss · Simon Willison · Jun 17, 03:36

**Background**: NetNewsWire is a classic RSS (Really Simple Syndication) reader, a tool for aggregating content from websites and blogs via feeds. RSS was once widely used before the rise of social media algorithms. Open-source means the code is freely available for anyone to use and modify.

**Tags**: `#netnewswire`, `#open-source`, `#brent-simmons`, `#rss`, `#software`

---

<a id="item-19"></a>
## [Datasette 1.0a34 Adds Row Editing to Web UI](https://simonwillison.net/2026/Jun/16/datasette/#atom-everything) ⭐️ 6.0/10

Datasette 1.0a34 introduces tools to insert, edit, and delete rows directly within the Datasette web interface, available on table pages and row pages. This feature was inspired by Datasette Agent, which already supported SQL write operations via chat. This update significantly enhances Datasette from a read-only exploration tool to a more interactive data management platform, bridging a long-standing gap. It empowers users to make quick data corrections without external tools, increasing productivity for data analysts and developers. The alpha release (1.0a34) adds these features to table pages, and edit/delete are also available as actions on the individual row page. The feature is still in alpha, meaning it may have bugs or incomplete functionality.

rss · Simon Willison · Jun 16, 21:31

**Background**: Datasette is an open-source tool for exploring and publishing data, primarily designed for read-only access to SQLite databases. Until now, modifying data required external tools or writing raw SQL. Datasette Agent, an AI assistant plugin, recently added SQL write support, highlighting the absence of editing in the standard UI.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/May/21/datasette-agent/">Datasette Agent - simonwillison.net</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent, an extensible AI assistant for Datasette</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#database`, `#data management`, `#python`, `#open source`

---

<a id="item-20"></a>
## [datasette-tailscale 0.1a0: Private Datasette via Tailscale](https://simonwillison.net/2026/Jun/16/datasette-tailscale/#atom-everything) ⭐️ 6.0/10

An experimental alpha plugin named datasette-tailscale 0.1a0 has been released, allowing users to run Datasette with a Tailscale sidecar for private network access. It uses Python bindings for the experimental tailscale-rs library. This plugin simplifies sharing Datasette instances securely over a Tailscale network without exposing them to the public internet. It demonstrates a novel integration of Tailscale's sidecar pattern with Datasette, potentially enabling easy private data publishing. The plugin is very experimental and uses the Python bindings for the tailscale-rs Rust library, which is itself unstable. The author filed an issue asking for a cleaner proxy mechanism.

rss · Simon Willison · Jun 16, 16:18

**Background**: Datasette is an open-source tool for exploring and publishing data as interactive websites and APIs. Tailscale provides a software-defined mesh VPN for secure private networking. The 'sidecar' pattern involves running a Tailscale agent alongside an application to connect it to a Tailnet without exposing it to the public internet. tailscale-rs is an experimental Rust implementation of the Tailscale client with language bindings.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>
<li><a href="https://github.com/tailscale/tailscale-rs/">GitHub - tailscale/tailscale-rs: Rust implementation of ...</a></li>
<li><a href="https://tailscale.com/blog/tailscale-rs-rust-tsnet-library-preview">An early look at tailscale-rs, a tsnet library in Rust</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#tailscale`, `#plugin`, `#networking`

---