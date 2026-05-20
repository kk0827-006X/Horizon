---
layout: default
title: "Horizon Summary: 2026-05-20 (EN)"
date: 2026-05-20
lang: en
---

> From 50 items, 15 important content pieces were selected

---

1. [Google Search Box Gets AI Overhaul with Gemini](#item-1) ⭐️ 9.0/10
2. [CISA Admin Leaks AWS GovCloud Keys on GitHub](#item-2) ⭐️ 9.0/10
3. [Google Launches Gemini 3.5 Flash Model](#item-3) ⭐️ 8.0/10
4. [Virtual Museum Showcases Nearly Every Operating System](#item-4) ⭐️ 8.0/10
5. [Forge: Guardrails Boost Local LLM to 99% Accuracy](#item-5) ⭐️ 8.0/10
6. [Common Ways Open Source Projects Die](#item-6) ⭐️ 8.0/10
7. [Apple unveils AI-powered accessibility features](#item-7) ⭐️ 8.0/10
8. [Minnesota becomes first state to ban prediction markets](#item-8) ⭐️ 8.0/10
9. [Andrej Karpathy Joins Anthropic to Lead Pre-training](#item-9) ⭐️ 8.0/10
10. [Gentoo Warns of Three Linux Kernel Vulnerabilities](#item-10) ⭐️ 8.0/10
11. [OpenAI Adopts Google's SynthID Watermark for AI Images](#item-11) ⭐️ 7.0/10
12. [Mistral AI Acquires Emmi AI to Build Industrial AI Stack](#item-12) ⭐️ 7.0/10
13. [Simon Willison Summarizes LLM Developments at PyCon US 2026](#item-13) ⭐️ 7.0/10
14. [Tesla Lithium Refinery Discharges Polluted Wastewater Beyond Permit Limits](#item-14) ⭐️ 6.0/10
15. [llm-gemini 0.32 Adds Gemini 3.5 Flash Support](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Google Search Box Gets AI Overhaul with Gemini](https://blog.google/products-and-platforms/products/search/search-io-2026/) ⭐️ 9.0/10

At Google I/O 2026, Google announced a major redesign of its search box that directly integrates the Gemini AI model into the search experience, generating conversational answers instead of traditional links. This shift could fundamentally change how users access information, potentially reducing web traffic to external sites and raising concerns about accuracy and primary source verification. The new search box uses Gemini to provide synthesized answers with citations, but critics warn it may favor AI summaries over original content, leading to a 'Google Zero' scenario where clicks to publishers drop sharply.

hackernews · berkeleyjunk · May 19, 18:34 · [Discussion](https://news.ycombinator.com/item?id=48197370)

**Background**: Google Search has traditionally returned a list of links to web pages. Gemini is a family of multimodal large language models developed by Google DeepMind, announced in 2023, capable of understanding text, images, and more. This redesign marks a shift from providing links to generating answers directly, similar to AI chatbots but within the core search interface.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(AI_model)">Gemini (AI model)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(language_model)">Gemini (language model) - Wikipedia</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models">Models | Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**Discussion**: Community comments express strong distrust of AI-generated facts, with users emphasizing the importance of primary sources and pointing out that LLMs can combine information from different eras incorrectly. The concept of 'Google Zero' is also discussed, where Google stops sending traffic to other sites, sparking debate about the ecosystem's future.

**Tags**: `#Google`, `#AI`, `#Search`, `#Technology`, `#Web`

---

<a id="item-2"></a>
## [CISA Admin Leaks AWS GovCloud Keys on GitHub](https://krebsonsecurity.com/2026/05/cisa-admin-leaked-aws-govcloud-keys-on-github/) ⭐️ 9.0/10

A CISA administrator publicly exposed AWS GovCloud access keys on a GitHub repository, along with a CSV file containing plaintext usernames and passwords for internal CISA systems. This incident exposes highly sensitive government credentials on a public platform, undermining cloud security for a critical federal agency and highlighting systemic failures in credential management and automated monitoring. The leaked keys were for AWS GovCloud, an isolated AWS region designed for sensitive government workloads, and the repository also contained a file named “AWS-Workspace-Firefox-Passwords.csv” with dozens of internal system credentials. The owner failed to respond to notification attempts by security researchers.

hackernews · LelouBil · May 19, 07:45 · [Discussion](https://news.ycombinator.com/item?id=48190454)

**Background**: AWS GovCloud (US) is a physically and logically isolated AWS region that complies with U.S. government regulations for hosting sensitive and controlled unclassified information (CUI). AWS access keys are long-term credentials used by IAM users to authenticate programmatic requests to AWS services. Leaking such keys can lead to unauthorized access to government infrastructure and data.

<details><summary>References</summary>
<ul>
<li><a href="https://aws.amazon.com/govcloud-us/">AWS GovCloud (US) - Amazon Web Services</a></li>
<li><a href="https://docs.aws.amazon.com/govcloud-us/latest/UserGuide/whatis.html">What Is AWS GovCloud (US)? - AWS GovCloud (US)</a></li>
<li><a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html">Manage access keys for IAM users - AWS Identity and Access ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed shock at the leak and the administrator's lack of response, with some suspecting it could be a honeypot due to the blatant exposure. Others criticized the failure to use AWS security services like Secrets Manager or automated scanners, and noted that similar sensitive documents were also uploaded to ChatGPT.

**Tags**: `#cybersecurity`, `#AWS`, `#government`, `#data breach`, `#cloud security`

---

<a id="item-3"></a>
## [Google Launches Gemini 3.5 Flash Model](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5/) ⭐️ 8.0/10

Google announced the general availability of Gemini 3.5 Flash, a new AI model that skips the preview stage and is being integrated into key Google products. This release signals Google's aggressive push in the AI model race, with Gemini 3.5 Flash offering improved performance but at a significantly higher price point, which could influence developer adoption and competitive dynamics. Pricing for Gemini 3.5 Flash is $1.50 per million input tokens and $9.00 per million output tokens, which is roughly 3x the cost of Gemini 2.5 Flash. The model is available immediately through the Gemini API and powers various Google products.

hackernews · spectraldrift · May 19, 17:43 · [Discussion](https://news.ycombinator.com/item?id=48196570)

**Background**: Gemini is Google's family of large language models. The 'Flash' variants are designed for faster, cost-effective inference. Google I/O is the company's annual developer conference where major product announcements are made. This release is notable as it skips the usual 'preview' phase, indicating confidence in the model's readiness.

**Discussion**: Commenters noted the significant price increase, with one pointing out that Gemini 3.5 Flash costs as much as Gemini 2.5 Pro. Others reported high token usage and quota exhaustion. Some humorous remarks compared the name 'Flash' to Adobe Flash, suggesting to consider HTML5 instead.

**Tags**: `#AI`, `#Google`, `#Gemini`, `#pricing`, `#model release`

---

<a id="item-4"></a>
## [Virtual Museum Showcases Nearly Every Operating System](https://virtualosmuseum.org/) ⭐️ 8.0/10

A new virtual museum, virtualosmuseum.org, has been launched, featuring an extensive collection of historical and obscure operating systems spanning decades. It curates them in an interactive, browsable gallery that allows users to explore OS history. This project serves as a vital resource for preserving and understanding the evolution of operating systems, which are foundational to modern computing. It offers enthusiasts and researchers a unique way to experience and compare systems that are otherwise difficult to access. The museum includes not only major systems like Windows and macOS but also rare ones like Domain/OS and Pick, showcasing both their visual interfaces and some interactive elements. However, as noted in community comments, emulation may not capture the full original user experience, such as hardware-specific feedback or latency.

hackernews · andreww591 · May 19, 15:53 · [Discussion](https://news.ycombinator.com/item?id=48195009)

**Background**: Operating systems have evolved dramatically since the early days of computing, with many now defunct or obscure systems offering unique features and design philosophies. Emulation allows modern users to run these old systems on current hardware, but it often cannot replicate the tactile and sensory experience of original hardware. The museum leverages emulation to make these systems accessible, while also highlighting the differences between emulated and real experiences.

**Discussion**: Community comments praise the curation effort but note that some featured versions may not be the most interesting or representative. Others discuss how emulation loses the 'feel' of original hardware, such as keyboard latency, mouse acceleration, and CRT display characteristics. A few users mention missing systems like Pick and recall obscure Unix features.

**Tags**: `#retro computing`, `#operating systems`, `#emulation`, `#curation`, `#history`

---

<a id="item-5"></a>
## [Forge: Guardrails Boost Local LLM to 99% Accuracy](https://github.com/antoinezambelli/forge) ⭐️ 8.0/10

Forge is an open-source reliability layer that boosts small local LLMs from ~53% to ~99% accuracy on multi-step agentic tasks using guardrails and a harness, without modifying the model itself. This dramatically closes the reliability gap between free local models and expensive frontier APIs, enabling cost-effective, always-on agentic systems on consumer hardware. It also reveals that infrastructure choices (e.g., serving backend) can cause larger accuracy swings than model selection. The guardrail stack includes five layers: retry nudges, step enforcement, error recovery, rescue parsing, and VRAM-aware context compaction. In ablation studies, retry nudges caused a 24-49 point accuracy drop when disabled, and error recovery caused ~10 point drops. Forge also introduces a ToolResolutionError exception to distinguish tool success with no results from failure.

hackernews · zambelli · May 19, 12:23 · [Discussion](https://news.ycombinator.com/item?id=48192383)

**Background**: LLM agentic tasks involve multi-step workflows where the model calls tools and processes results. Even 90% per-step accuracy compounds to a high failure rate over multiple steps. Guardrails are validation layers that catch errors, enforce structure, and retry failures. VRAM management is critical for local models on consumer GPUs, as silent CPU fallback can drastically slow inference.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/guardrails-ai/guardrails">GitHub - guardrails-ai/guardrails: Adding guardrails to large language models. · GitHub</a></li>
<li><a href="https://labs.adaline.ai/p/what-are-agentic-llms-a-comprehensive">What Are Agentic LLMs? Use Cases, Risks, and How They Work</a></li>
<li><a href="https://medium.com/@lyx_62906/context-kills-vram-how-to-run-llms-on-consumer-gpus-a785e8035632">Context Kills VRAM: How to Run LLMs on consumer GPUs | by Lyx | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters agreed with the tool-call ambiguity point, noting similar issues with frontier models. One user mentioned their own harness system improved token efficiency 2-10x on math tasks. Another highlighted the importance of appropriate scaling, suggesting we don't always need large frontier models.

**Tags**: `#llm`, `#guardrails`, `#agentic`, `#open-source`, `#reliability`

---

<a id="item-6"></a>
## [Common Ways Open Source Projects Die](https://nesbitt.io/2026/05/19/dumb-ways-for-an-open-source-project-to-die.html) ⭐️ 8.0/10

A blog post titled 'Dumb Ways for an Open Source Project to Die' lists common failure modes such as bus factor, bikeshedding, and scope creep. The community discussion enriches the list with additional patterns like overconfident forks and maintainer burnout. This post serves as a practical checklist for open source maintainers to recognize and avoid pitfalls that kill projects. The high community engagement (124 points, 59 comments) underscores the relevance and urgency of these issues in the open source ecosystem. Notable failure modes include the bus factor (single point of failure), bikeshedding (focusing on trivial matters), and scope creep driven by vocal users. Community comments also highlight overconfident forks, maintainer burnout, and the unrealistic expectation of weekly maintenance.

hackernews · chmaynard · May 19, 19:22 · [Discussion](https://news.ycombinator.com/item?id=48198127)

**Background**: Open source projects rely on volunteer or under-resourced maintainers, making them vulnerable to various risks. The bus factor measures risk from key developer unavailability; bikeshedding describes triviality bias in discussions; governance models define decision-making structures. Understanding these concepts helps contextualize why projects fail.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bus_factor">Bus factor</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bikeshedding">Bikeshedding</a></li>
<li><a href="https://www.redhat.com/en/blog/understanding-open-source-governance-models">Understanding open source governance models</a></li>

</ul>
</details>

**Discussion**: Comments generally agree with the listed failure modes and add missing ones. Some nostalgia for when open source was simpler, while others note that maintainer burnout and overconfident forks are common. A few comments suggest the need for clear contributing guidelines to prevent scope creep.

**Tags**: `#open source`, `#software engineering`, `#project maintenance`, `#community best practices`

---

<a id="item-7"></a>
## [Apple unveils AI-powered accessibility features](https://www.apple.com/newsroom/2026/05/apple-unveils-new-accessibility-features-and-updates-with-apple-intelligence/) ⭐️ 8.0/10

Apple announced a suite of accessibility updates powered by Apple Intelligence, including enhanced VoiceOver, Magnifier, Voice Control, and a new Accessibility Reader for customized reading experiences. This integration of generative AI into accessibility tools shows Apple's commitment to inclusive design and privacy-focused on-device processing, potentially setting a new standard for AI in assistive technology. The features leverage Apple Intelligence, which combines on-device and server processing, and are available on iPhone 16 series, iPhone 15 Pro, and devices with M1 or later chips. Accessibility Reader uses AI to adapt text for users with dyslexia or low vision.

hackernews · interpol_p · May 19, 12:04 · [Discussion](https://news.ycombinator.com/item?id=48192224)

**Background**: Apple Intelligence is Apple's generative AI system announced in June 2024, integrated into iOS 18, iPadOS 18, and macOS Sequoia. It offers writing tools, image generation, notification summaries, and ChatGPT integration, with a strong emphasis on privacy through on-device processing. Accessibility features have long been a focus for Apple, and this update brings AI to improve usability for people with disabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/05/apple-unveils-new-accessibility-features-and-updates-with-apple-intelligence/">Apple unveils new accessibility features, and updates with Apple ...</a></li>
<li><a href="https://www.macrumors.com/2026/05/19/new-accessibility-features-with-apple-intelligence/">Apple Previews New Accessibility Features Powered by Apple Intelligence</a></li>
<li><a href="https://9to5mac.com/2026/05/19/apple-announces-ai-powered-accessibility-features-and-eye-controlled-wheelchair-functionality/">Apple announces AI-powered accessibility features and eye ... - 9to5Mac</a></li>

</ul>
</details>

**Discussion**: Community comments highlight mixed reactions: some praise the practical use of AI for accessibility, while others criticize Apple's speech-to-text accuracy and note that the company often stealth-tests new technologies (like agentic AI) through accessibility features. There is also appreciation for how blind users can listen at high speeds, demonstrating advanced assistive techniques.

**Tags**: `#accessibility`, `#Apple`, `#artificial intelligence`, `#speech-to-text`, `#user experience`

---

<a id="item-8"></a>
## [Minnesota becomes first state to ban prediction markets](https://www.npr.org/2026/05/19/nx-s1-5821265/minnesota-ban-prediction-markets) ⭐️ 8.0/10

Minnesota has enacted a law banning prediction markets, becoming the first U.S. state to do so. The ban targets platforms like Polymarket that allow users to bet on event outcomes. This sets a precedent for state-level regulation of prediction markets, raising questions about federal preemption by the CFTC. It could embolden other states to follow suit, impacting the growing industry of event-based betting. Minnesota currently also has a complete ban on sports betting, which may strengthen its legal position against prediction markets. The ban is likely to face legal challenges on federal preemption grounds, as prediction markets are regulated by the CFTC as commodity futures.

hackernews · ortusdux · May 19, 19:13 · [Discussion](https://news.ycombinator.com/item?id=48197980)

**Background**: Prediction markets are platforms where participants bet on the outcome of future events, with prices reflecting collective probability estimates. They have been used for forecasting everything from election results to movie openings. In the U.S., the Commodity Futures Trading Commission (CFTC) has authority over prediction markets as futures contracts, but state laws can also apply. This tension between state and federal oversight is central to the current debate.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prediction_market">Prediction market - Wikipedia</a></li>
<li><a href="https://help.polymarket.com/en/articles/13364272-what-is-a-prediction-market">What is a Prediction Market? | Polymarket Help Center</a></li>

</ul>
</details>

**Discussion**: Commenters debate whether the ban can survive federal preemption, with some noting the CFTC typically regulates futures markets. Others argue prediction markets often devolve into sports betting or insider trading, questioning their societal value. A few express skepticism that the ban will last, citing potential legal challenges.

**Tags**: `#regulations`, `#prediction-markets`, `#crypto`, `#politics`, `#finance`

---

<a id="item-9"></a>
## [Andrej Karpathy Joins Anthropic to Lead Pre-training](https://twitter.com/karpathy/status/2056753169888334312) ⭐️ 8.0/10

Andrej Karpathy has joined Anthropic to lead the pre-training team for Claude, responsible for the massive training runs that give Claude its core knowledge and capabilities. As a highly respected AI researcher and former head of AI at Tesla and OpenAI, Karpathy's move to Anthropic underscores the importance of pre-training and may accelerate Anthropic's development of Claude, potentially reshaping the frontier of AI language models. Karpathy will start on Anthropic's pre-training team this week, and he had hinted at this move in a recent interview, saying he might fall out of touch with evolving approaches and would be interested if a frontier lab would have him.

hackernews · dmarcos · May 19, 15:07 · [Discussion](https://news.ycombinator.com/item?id=48194352)

**Background**: Andrej Karpathy is a renowned AI researcher known for his work at OpenAI and Tesla, and for his popular educational content on deep learning. Anthropic is a leading AI company focused on building safe and capable AI systems, particularly its Claude model series. Pre-training is the initial large-scale training phase that gives a language model its broad knowledge and capabilities, typically using massive amounts of text data.

**Discussion**: The community largely expressed excitement about Karpathy joining Anthropic, with some hoping he continues his educational work. Others voiced concerns about Anthropic's growing influence in the AI industry, drawing parallels to a monopoly. Overall, the discussion reflected a mix of admiration for Karpathy and wariness of Anthropic's consolidation of talent.

**Tags**: `#AI`, `#Anthropic`, `#Andrej Karpathy`, `#Claude`, `#industry news`

---

<a id="item-10"></a>
## [Gentoo Warns of Three Linux Kernel Vulnerabilities](https://www.gentoo.org/news/2026/05/19/copy-fail-fragnesia-vulnerabilities.html) ⭐️ 8.0/10

Gentoo has announced three kernel privilege escalation vulnerabilities: Copy Fail (CVE-2026-31431), Dirty Frag, and Fragnesia (CVE-2026-46300), urging users to upgrade or apply live patches. These vulnerabilities allow unprivileged local users to gain root access, posing a critical risk to Linux systems including cloud and Kubernetes environments, and require urgent patching. Copy Fail was discovered in the crypto subsystem and already has an exploit in the wild; Fragnesia does not require a race condition, making it more reliable for privilege escalation.

hackernews · akhuettel · May 19, 15:27 · [Discussion](https://news.ycombinator.com/item?id=48194614)

**Background**: The Linux kernel is the core of the operating system, managing hardware and security. Privilege escalation vulnerabilities allow attackers to bypass restrictions and gain full control. Live patching (e.g., kpatch) enables applying security fixes without rebooting, but carries risks of system instability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gentoo.org/news/2026/05/19/copy-fail-fragnesia-vulnerabilities.html">Copy Fail, Dirty Frag, and Fragnesia kernel vulnerabilities</a></li>
<li><a href="https://en.wikipedia.org/wiki/Copy_Fail">Copy Fail - Wikipedia</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/new-fragnesia-linux-flaw-lets-attackers-gain-root-privileges/">New Fragnesia Linux flaw lets attackers gain root privileges</a></li>

</ul>
</details>

**Discussion**: Community comments debate the adoption of automated live patching, with some concerned about reliability and security. Others question whether Gentoo is unique in facing such challenges, and one sarcastically suggests LLM-generated patches without review.

**Tags**: `#kernel`, `#vulnerability`, `#linux`, `#security`, `#gentoo`

---

<a id="item-11"></a>
## [OpenAI Adopts Google's SynthID Watermark for AI Images](https://openai.com/index/advancing-content-provenance/) ⭐️ 7.0/10

OpenAI announced it is integrating Google DeepMind's SynthID digital watermark into images generated by its DALL-E and other AI image tools, and released an open verification tool to check for the watermark. This move standardizes content provenance across major AI platforms, helping to distinguish AI-generated images from human-created ones and combat misinformation, though the watermark's robustness is debated. SynthID embeds an imperceptible watermark directly into the pixel data, designed to survive common edits like cropping and compression; however, community members have reported methods to remove or distort the watermark.

hackernews · smooke · May 19, 19:34 · [Discussion](https://news.ycombinator.com/item?id=48198291)

**Background**: SynthID was developed by Google DeepMind and is an invisible digital watermarking technology for AI-generated images and videos. It works by modifying pixel values in a way that is imperceptible to humans but detectable by a proprietary algorithm. The goal is to provide a means of tracing AI-generated content to its source.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/synthid/">SynthID — Google DeepMind</a></li>
<li><a href="https://ai.google.dev/responsible/docs/safeguards/synthid">SynthID: Tools for watermarking and detecting LLM-generated Text | Responsible Generative AI Toolkit | Google AI for Developers</a></li>

</ul>
</details>

**Discussion**: Comments are mixed: some users claim to have successfully removed the watermark using off-the-shelf models, while others question its robustness and compare it to DRM. There is skepticism about its long-term effectiveness, but some appreciate the effort to improve content provenance.

**Tags**: `#watermark`, `#AI images`, `#content provenance`, `#OpenAI`, `#SynthID`

---

<a id="item-12"></a>
## [Mistral AI Acquires Emmi AI to Build Industrial AI Stack](https://www.emmi.ai/news/mistral-ai-acquires-emmi-ai) ⭐️ 7.0/10

Mistral AI has acquired Emmi AI, a startup specializing in AI for engineering simulations, with the goal of creating a leading AI stack tailored for industrial engineering applications. This acquisition targets a less-covered vertical—industrial engineering—where AI can optimize complex simulations and design processes. With ASML as a strategic investor, Mistral AI gains credibility and potential access to the semiconductor manufacturing ecosystem. Emmi AI has released Noether, an open-source deep learning framework for engineering AI, built for reproducible and extensible workflows. The acquisition leverages ASML's investment in Mistral AI, announced in September 2025, which gave ASML a seat on Mistral AI's Strategic Committee.

hackernews · doener · May 19, 19:14 · [Discussion](https://news.ycombinator.com/item?id=48197995)

**Background**: Mistral AI is a French startup known for developing large language models and AI solutions. Emmi AI focuses on applying deep learning to engineering and physics simulations, an area often neglected by mainstream AI companies. ASML, a leading supplier of photolithography systems for chip manufacturing, invested in Mistral AI to explore AI-driven industrial applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emmi.ai/">Emmi AI | Home</a></li>
<li><a href="https://www.asml.com/en/news/press-releases/2025/asml-mistral-ai-enter-strategic-partnership">ASML, Mistral AI enter strategic partnership</a></li>

</ul>
</details>

**Discussion**: Commenters noted that ASML's investment makes the industrial AI ambitions more credible, but some expressed skepticism about Mistral AI's competitive position against giants like Google, Anthropic, and OpenAI. Others questioned what Emmi AI has actually built, as no concrete demos were found.

**Tags**: `#AI`, `#acquisition`, `#industrial engineering`, `#Mistral`, `#Emmi`

---

<a id="item-13"></a>
## [Simon Willison Summarizes LLM Developments at PyCon US 2026](https://simonwillison.net/2026/May/19/5-minute-llms/#atom-everything) ⭐️ 7.0/10

Simon Willison presented a five-minute lightning talk at PyCon US 2026 summarizing the major LLM developments from the past six months, using his annotated presentation tool. The talk highlighted a November 2025 inflection point where the best model changed hands five times among top AI labs. This summary provides a concise, high-level overview of the rapidly evolving LLM landscape, particularly for coding models, helping practitioners stay updated. The annotated presentation tool itself is a notable technical innovation for creating accessible slide content. The talk used a 'pelican riding a bicycle' SVG generation test to illustrate model differences. The 'best' model designation shifted five times between November 2025 and May 2026, among Anthropic, OpenAI, and Google.

rss · Simon Willison · May 19, 01:09

**Background**: The 'November 2025 inflection point' refers to a period of intense competition in large language models, marked by rapid releases of new models that overtook each other in benchmarks. Simon Willison's annotated presentation tool allows speakers to add alt text and notes to slides, improving accessibility and reproducibility.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2025/May/15/annotated-presentation-creator/">Annotated Presentation Creator | Simon Willison ’s Weblog</a></li>
<li><a href="https://simonwillison.net/2025/may/15/annotated-presentations/">Tool : Annotated Presentation Creator | Simon Willison ’s Weblog</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#AI`, `#PyCon`, `#Simon Willison`, `#lightning talk`

---

<a id="item-14"></a>
## [Tesla Lithium Refinery Discharges Polluted Wastewater Beyond Permit Limits](https://www.autonocion.com/us/tesla-lithium-refinery-texas/) ⭐️ 6.0/10

Tesla's lithium refinery in Robstown, Texas, discharged up to 231,000 gallons of treated wastewater per day under a TPDES permit, but the discharge exceeded permit limits for pollutants like hexavalent chromium and arsenic, and the company lacked legal rights to use the drainage ditch. This incident highlights environmental compliance risks for lithium refining operations, which are critical for battery supply chains. It could lead to stricter regulations and public scrutiny of Tesla's and other companies' environmental practices. Hexavalent chromium was detected at 0.0104 mg/L, just above the lab's reporting limit of 0.01 mg/L, and arsenic at 0.0025 mg/L, below federal drinking water standards. The TPDES permit did not grant Tesla the right to use the county-owned ditch for wastewater conveyance.

hackernews · atombender · May 19, 19:52 · [Discussion](https://news.ycombinator.com/item?id=48198551)

**Background**: Lithium refining processes extract lithium from ores or brines to produce battery-grade compounds, often generating wastewater containing heavy metals and other pollutants. Wastewater discharge permits like TPDES set limits on pollutant concentrations, but do not automatically grant rights to use third-party infrastructure for conveyance.

<details><summary>References</summary>
<ul>
<li><a href="https://energyx.com/blog/what-is-lithium-refining-a-deep-dive-from-energyx/">What is Lithium Refining ? A Deep Dive from EnergyX - EnergyX</a></li>
<li><a href="https://www.usgs.gov/news/featured-story/trash-treasure-could-energy-wastewaters-be-a-viable-source-lithium">Trash to Treasure: Could energy wastewaters be a viable ...</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the legal case focuses more on Tesla's lack of rights to use the drainage ditch than on the pollution itself, with some arguing the pollutant levels were not extremely high. Others criticized Tesla's statement claiming full compliance while exceeding permit limits.

**Tags**: `#environment`, `#Tesla`, `#pollution`, `#regulation`, `#lithium`

---

<a id="item-15"></a>
## [llm-gemini 0.32 Adds Gemini 3.5 Flash Support](https://simonwillison.net/2026/May/19/llm-gemini-2/#atom-everything) ⭐️ 6.0/10

The llm-gemini plugin version 0.32 has been released, adding support for the new gemini-3.5-flash model from Google DeepMind. This update allows users of the LLM command-line tool to easily access the latest Gemini 3.5 Flash model, which offers faster inference and lower cost for agentic and multi-step tasks. The release only adds a single new model, gemini-3.5-flash, and no other changes are mentioned. Users can upgrade the plugin and start using the model immediately.

rss · Simon Willison · May 19, 23:46

**Background**: LLM is a command-line tool and Python library by Simon Willison that provides a unified interface to interact with many large language models, including OpenAI, Anthropic, and Google Gemini. Gemini 3.5 Flash is a multimodal model from Google DeepMind designed for high-speed, cost-efficient performance, especially for complex multi-step workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the ...</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models/gemini-3.5-flash">Gemini 3 . 5 Flash | Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**Tags**: `#gemini`, `#llm`, `#llm-gemini`, `#release`

---