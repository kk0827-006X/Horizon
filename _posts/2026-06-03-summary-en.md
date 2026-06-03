---
layout: default
title: "Horizon Summary: 2026-06-03 (EN)"
date: 2026-06-03
lang: en
---

> From 52 items, 11 important content pieces were selected

---

1. [Microsoft unveils MAI-Thinking-1 and MAI-Code-1-Flash LLMs](#item-1) ⭐️ 8.0/10
2. [Hackers Hijack Instagram Accounts by Asking Meta AI Bot to Change Email](#item-2) ⭐️ 8.0/10
3. [CT Scans Reveal BYD Car Parts' Inner Secrets](#item-3) ⭐️ 7.0/10
4. [User ditches Gmail for Fastmail over intrusive AI features](#item-4) ⭐️ 7.0/10
5. [Seattle Surveillance Tour Maps City's Camera Network](#item-5) ⭐️ 7.0/10
6. [Adafruit Receives Demand Letter from Flux.ai Legal Counsel](#item-6) ⭐️ 7.0/10
7. [Trump signs downsized AI order with voluntary review](#item-7) ⭐️ 7.0/10
8. [Nvidia GPU VRAM as Linux swap with nbd-vram](#item-8) ⭐️ 6.0/10
9. [Clojure Reflections: Composability and Dialect Diversity](#item-9) ⭐️ 6.0/10
10. [HP re-releases classic HP-16C calculator as collector's edition](#item-10) ⭐️ 6.0/10
11. [datasette-agent-micropython 0.1a0 Released](#item-11) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Microsoft unveils MAI-Thinking-1 and MAI-Code-1-Flash LLMs](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

Microsoft announced two new text LLMs: MAI-Thinking-1, a reasoning model with 1 trillion total parameters but only 35 billion active, and MAI-Code-1-Flash, a code-specialist model with 137 billion total parameters and 5 billion active. The models are built on clean, licensed data and are being integrated into GitHub Copilot and VS Code. These models demonstrate progress in efficient LLM architectures with low active parameter counts, potentially reducing inference costs. MAI-Thinking-1 claims to be preferred over Claude Sonnet 4.6 in blind evaluations, challenging larger, more expensive models. MAI-Thinking-1 is a 1-trillion-parameter model with 35 billion active parameters using a Mixture-of-Experts architecture, while MAI-Code-1-Flash has 137 billion total parameters and 5 billion active. Despite initial claims of clean data, the technical paper reveals training included proprietary web crawls and Common Crawl data, similar to other major LLMs.

rss · Simon Willison · Jun 2, 22:21

**Background**: Large language models (LLMs) are AI systems trained on vast text data to generate human-like text. Mixture-of-Experts (MoE) architectures activate only a subset of parameters per token, enabling large models with lower computational cost. Active parameters refer to the number of parameters used during inference, while total parameters include all weights in the model. Microsoft's new models use MoE to achieve high performance with low active parameter counts.

<details><summary>References</summary>
<ul>
<li><a href="https://microsoft.ai/news/two-new-in-house-models/">Two in-house models in support of our mission | Microsoft AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/claude-sonnet-4-6">Introducing Claude Sonnet 4.6</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the models' performance, noting that MAI-Code-1-Flash's SWE-bench pro score (51%) is only slightly better than a cheaper open model (Qwen3.6-35B-A3B at 49.5%). Some criticized Microsoft's comparison to older, smaller Anthropic models like Haiku 4.5, and questioned the value of small cloud models for serious coding tasks. There was also frustration with GitHub Copilot's recent pricing changes.

**Tags**: `#LLM`, `#Microsoft`, `#AI`, `#efficiency`, `#code generation`

---

<a id="item-2"></a>
## [Hackers Hijack Instagram Accounts by Asking Meta AI Bot to Change Email](https://simonwillison.net/2026/Jun/1/hackers-simply-asked-meta-ai/#atom-everything) ⭐️ 8.0/10

Hackers exploited Meta's AI support chatbot by simply asking it to link a new email address to high-profile Instagram accounts, successfully hijacking them without needing passwords or two-factor authentication. The attackers used a VPN to spoof the target's location to avoid triggering security alerts. This incident reveals a critical security flaw in deploying AI chatbots for sensitive account management, as the bot bypassed standard account recovery procedures. It undermines trust in AI-driven support systems and highlights the need for strict guardrails to prevent prompt injection attacks. The attack did not require sophisticated prompt injection—the hackers simply made a direct request, and the bot complied without verifying identity or demanding additional authentication. Multiple high-profile accounts were affected, and Meta has not yet commented on a fix.

rss · Simon Willison · Jun 1, 21:14

**Background**: Prompt injection is a type of cybersecurity attack where malicious inputs cause a large language model (LLM) to behave unexpectedly, often bypassing its intended safeguards. In this case, the AI support bot was granted the ability to perform account recovery actions—like changing linked emails—without proper human oversight. Such bots are increasingly used by companies to automate customer support, but without strict access controls, they can become a powerful attack vector.

<details><summary>References</summary>
<ul>
<li><a href="https://www.404media.co/hackers-simply-asked-meta-ai-to-give-them-access-to-high-profile-instagram-accounts-it-worked/">Hackers Simply Asked Meta AI to Give Them Access to High-Profile Instagram Accounts. It Worked</a></li>
<li><a href="https://techcrunch.com/2026/06/01/hackers-hijacked-instagram-accounts-by-tricking-meta-ai-support-chatbot-into-granting-access/">Hackers hijacked Instagram accounts by tricking Meta AI support chatbot into granting access | TechCrunch</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI safety`, `#account takeover`, `#Meta`

---

<a id="item-3"></a>
## [CT Scans Reveal BYD Car Parts' Inner Secrets](https://www.lumafield.com/scan-of-the-month/byd) ⭐️ 7.0/10

Lumafield published industrial CT scans of BYD car parts, including a key fob and a prismatic battery cell, revealing internal structures and sparking detailed technical discussion on design and manufacturing. This provides rare, non-destructive insight into BYD's engineering and vertical integration strategy, which is a key competitive advantage in the EV market. The scans help the community understand how BYD achieves high component self-sufficiency. Community members corrected that the mechanical key in the fob is not hinged but pulls out after unlatching a clip, and noted that the scanned prismatic cell is not the famous Blade battery but shares the same chemistry.

hackernews · viasfo · Jun 2, 20:30 · [Discussion](https://news.ycombinator.com/item?id=48375824)

**Background**: Industrial CT scanning uses X-rays to create 3D internal images of objects without disassembly, commonly used for quality control and reverse engineering. Vertical integration means a company controls multiple stages of production; BYD reportedly produces around 75% of its vehicle components, similar to Tesla's claim and far above Ford's 25%.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lumafield.com/scan-of-the-month/car-parts">Explore familiar car parts with the help of CT scans</a></li>

</ul>
</details>

**Discussion**: Commenters provided corrections (the key is not hinged but clipped), shared links to Munro teardown videos for deeper analysis, and expressed slight disappointment that the scanned cell was not the Blade battery, though they noted shared chemistry.

**Tags**: `#CT scanning`, `#BYD`, `#electric vehicles`, `#manufacturing`, `#teardown`

---

<a id="item-4"></a>
## [User ditches Gmail for Fastmail over intrusive AI features](https://moddedbear.com/gmail-thinks-im-stupid-so-i-left) ⭐️ 7.0/10

The author of a blog post switched from Gmail to Fastmail, citing frustration with Gmail's AI-powered features like Smart Compose that feel intrusive and assume user incompetence. This highlights growing user pushback against AI-assisted features in productivity tools, raising questions about user autonomy and the balance between helpful automation and unwanted interference. Fastmail is a subscription-based email service offering features similar to Gmail including app passwords, masked emails, and iOS integration, but with faster performance and no AI intrusions. The author also notes that Fastmail's calendar lacks autocomplete for addresses.

hackernews · speckx · Jun 2, 19:27 · [Discussion](https://news.ycombinator.com/item?id=48375016)

**Background**: Gmail's Smart Compose uses machine learning to predict and suggest text as users type emails. While intended to speed up writing, some users find these suggestions distracting or presumptuous. Fastmail is a paid, independent email provider that emphasizes privacy and simplicity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fastmail">Fastmail - Wikipedia</a></li>
<li><a href="https://support.google.com/mail/answer/9116836?hl=en&co=GENIE.Platform=Desktop">Use Smart Compose in Gmail - Computer - Gmail Help</a></li>

</ul>
</details>

**Discussion**: Comments generally agree with the author's frustration, with many expressing annoyance at AI email suggestions that are often unhelpful or overly verbose. Some users also criticize Google's aggressive promotion of AI features, such as Windows notifications from Chrome.

**Tags**: `#email`, `#AI`, `#productivity`, `#Gmail`, `#Fastmail`

---

<a id="item-5"></a>
## [Seattle Surveillance Tour Maps City's Camera Network](https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/) ⭐️ 7.0/10

A walking tour documented and illustrated Seattle's extensive surveillance infrastructure, including automatic license plate readers, ShotSpotter sensors, and police cameras, to reveal the density of public monitoring. This visual documentation raises critical questions about privacy and the normalization of surveillance in urban spaces, empowering citizens to understand and debate the extent of monitoring by government and corporations. The tour highlights automatic license plate readers (ALPRs) mounted on street poles and police cars, ShotSpotter acoustic gunshot detection sensors, and multiple police cameras. The project combines photography and mapping to show their dense distribution.

hackernews · eustoria · Jun 2, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48369980)

**Background**: Surveillance cameras have become common in cities for law enforcement and traffic management. ALPRs capture license plate numbers and track vehicle movements, while ShotSpotter uses acoustic sensors to detect gunfire. Privacy advocates warn about the erosion of anonymity and potential misuse of collected data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dhs.gov/science-and-technology/saver/automatic-license-plate-readers">Automatic License Plate Readers - Homeland Security</a></li>
<li><a href="https://sls.eff.org/technologies/automated-license-plate-readers-alprs">Automated license plate readers - Electronic Frontier Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/ShotSpotter">ShotSpotter - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments show divided views: some support surveillance for solving crimes like auto theft, while others criticize the project's academic language as inaccessible. A user argues that without video evidence, prosecutors often decline to press charges, while another expresses willingness to trade privacy for safety.

**Tags**: `#surveillance`, `#privacy`, `#seattle`, `#ethics`, `#infrastructure`

---

<a id="item-6"></a>
## [Adafruit Receives Demand Letter from Flux.ai Legal Counsel](https://blog.adafruit.com/) ⭐️ 7.0/10

Adafruit, a leading open-source hardware company, received a demand letter from legal counsel representing Flux.ai, an AI-powered PCB design tool startup, following negative coverage or reviews. Ladyada, Adafruit's founder, expressed hope to resolve the matter publicly, possibly through a podcast. This legal action underscores growing tensions between open-source hardware communities and emerging AI-based PCB tools, potentially setting a precedent for how such disputes are handled. It also affects trust and transparency in the hardware ecosystem, where community reviews are highly valued. Flux.ai recently received funding from Bain Capital, and the demand letter likely relates to intellectual property or defamation claims. Ladyada reached out to Flux.ai's CEO Matthias Wagner to seek a collaborative resolution, aiming to set a positive example for the community.

hackernews · semanser · Jun 2, 10:00 · [Discussion](https://news.ycombinator.com/item?id=48368121)

**Background**: Flux.ai is a browser-based, cloud EDA platform for PCB design that leverages AI to assist with schematic capture and layout. Adafruit is a well-known open-source hardware company that frequently reviews and promotes tools for makers and engineers. Legal demands in the hardware community are unusual, and this incident has sparked debate about the quality and business practices of AI PCB tools.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Comparison_of_KiCad_and_Fluxai">Comparison of KiCad and Flux.ai</a></li>

</ul>
</details>

**Discussion**: Community comments overwhelmingly criticize Flux.ai, with users reporting poor experiences and high token costs. Many support Adafruit and view the legal letter as an attempt to suppress criticism. Some note Flux.ai's recent funding and suggest the company is sensitive about its reputation.

**Tags**: `#hardware`, `#PCB design`, `#legal`, `#open source`

---

<a id="item-7"></a>
## [Trump signs downsized AI order with voluntary review](https://www.politico.com/news/2026/06/02/trump-signs-downsized-ai-order-00946389) ⭐️ 7.0/10

President Trump signed a scaled-back AI executive order requiring companies to voluntarily submit powerful new AI models for government review 30 days before public release. This order marks a significant shift in U.S. AI policy, potentially slowing the release of frontier models and setting a precedent for future regulation. The order reduced the earlier draft's 90-day voluntary review window to 30 days, and applies only to the most powerful models. It also directs the Justice Department to pursue criminal cases against AI misuse.

hackernews · _alternator_ · Jun 2, 16:40 · [Discussion](https://news.ycombinator.com/item?id=48372628)

**Background**: Executive orders are directives issued by the U.S. president to manage federal operations. This order aims to balance innovation with national security by giving agencies a brief window to assess risks from advanced AI systems before public deployment.

**Discussion**: Community comments are largely skeptical, with many noting the order lacks substance and worrying it could be a step toward mandatory review for open-source or foreign models. Some appreciate the reduced 30-day window but question how the review will work in practice.

**Tags**: `#AI policy`, `#executive order`, `#regulation`, `#government`

---

<a id="item-8"></a>
## [Nvidia GPU VRAM as Linux swap with nbd-vram](https://github.com/c0dejedi/nbd-vram) ⭐️ 6.0/10

A new open-source tool called nbd-vram enables Linux users to utilize Nvidia GPU VRAM as swap space using CUDA and the NBD protocol. It is specifically designed for laptops with soldered, non-upgradable RAM. This tool provides a novel memory management option for systems with spare GPU VRAM, potentially improving performance for memory-constrained tasks. It highlights creative uses of GPU resources beyond graphics and AI workloads. On an RTX 3070 laptop, nbd-vram achieves sequential throughput of about 1.3 GB/s, which is slower than an NVMe SSD but has lower latency. The tool may cause desktop crashes under Wayland due to dynamic VRAM allocation and lacks backpressure handling.

hackernews · tanelpoder · Jun 2, 22:55 · [Discussion](https://news.ycombinator.com/item?id=48377404)

**Background**: Swap space is a portion of storage (typically a disk) used as overflow when RAM is full. Using GPU VRAM as swap is unusual because VRAM is normally reserved for graphics and compute; however, it can be repurposed via CUDA programming. The NBD protocol allows creating a block device that communicates with a userspace server, making the VRAM appear as a local device for swap.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/c0deJedi/nbd-vram">Use your Nvidia GPU's VRAM as swap space on Linux - GitHub</a></li>
<li><a href="https://www.phoronix.com/news/NVIDIA-NBD-VRAM">NBD-VRAM Provides Swap Space On Your NVIDIA GeForce GPUs</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-06-03-new-nbd-vram-tool-enables-linux-users-to-utilize-nvidia-gpu-vram-as-high-speed-swap-space">Use NVIDIA GPU VRAM as Swap Space on Linux with nbd-vram</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some users find it useful for laptops with soldered RAM and idle VRAM, while others note that NVMe swap is faster. There are concerns about Wayland stability and the lack of backpressure, with reports of desktop crashes when VRAM pressure is high.

**Tags**: `#Linux`, `#GPU`, `#swap`, `#memory management`, `#VRAM`

---

<a id="item-9"></a>
## [Clojure Reflections: Composability and Dialect Diversity](https://www.acdw.net/clojure/) ⭐️ 6.0/10

A programmer shares a month-long experience with Clojure, praising its composability and data structures, while the ensuing discussion delves into runtime trade-offs and alternative Clojure dialects such as ClojureScript and babashka. This discussion highlights a key tension in the Clojure ecosystem: the value of the JVM runtime versus the growing diversity of platforms that Clojure dialects support. It reflects ongoing debates about where Clojure's true strengths lie and could influence newcomers' adoption decisions. Commenters note that Clojure's syntax and semantics are portable across multiple runtimes via dialects like ClojureScript (JavaScript), ClojureDart, and babashka (SCI), and that most Clojure code without host interop works across dialects. However, one commenter argues the real value is in the JVM runtime, not the syntax, and that Java's concurrency model lags behind Erlang or Golang.

hackernews · speckx · Jun 2, 19:56 · [Discussion](https://news.ycombinator.com/item?id=48375393)

**Background**: Clojure is a modern Lisp dialect that runs primarily on the Java Virtual Machine (JVM) and emphasizes functional programming with immutable data structures. Its design allows for multiple dialects targeting alternative runtimes, such as ClojureScript for JavaScript, ClojureDart for Dart, and babashka for native scripts. This portability means developers can leverage Clojure's syntax across different platforms, though platform-specific features may require host interop.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Clojure">Clojure - Wikipedia</a></li>
<li><a href="https://programmingmentorship.github.io/docs/lessons/5-webdevelopment/3-clojuredialects/">Clojure Dialects | Programming Mentorship</a></li>

</ul>
</details>

**Discussion**: The community discussion shows a split: some echo the author's praise for composability and data structures, while others debate the runtime's importance. Notable points include Jeaye's list of dialects demonstrating Clojure's multi-platform reach, and pdimitar's assertion that the JVM runtime is the main value, not the syntax. There is also practical concern from zuzululu about limited job opportunities.

**Tags**: `#Clojure`, `#functional programming`, `#programming languages`, `#JVM`, `#static site generation`

---

<a id="item-10"></a>
## [HP re-releases classic HP-16C calculator as collector's edition](https://hpcalcs.com/product/hp-16c-collectors-edition/) ⭐️ 6.0/10

HP has re-released the HP-16C Computer Scientist calculator as a Collector's Edition, now available for ordering. The re-release of the HP-16C revives a beloved tool for programmers and retro enthusiasts, but concerns about build quality and value may affect its reception. The Collector's Edition retains the classic design of the original but includes modern programming functions; however, some community members question its build quality and suggest alternatives like the SwissMicros DM16L.

hackernews · dm319 · Jun 2, 19:02 · [Discussion](https://news.ycombinator.com/item?id=48374685)

**Background**: The original HP-16C was launched in 1982 and was unique for its support of multiple number bases and bitwise operations, making it a favorite among programmers. HP has been re-releasing classic calculators as Collector's Editions, including the HP-15C.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HP-16C">HP-16C - Wikipedia</a></li>
<li><a href="https://www.thecalculatorstore.com/c/hp16c-ce">HP16c CE - thecalculatorstore.com</a></li>
<li><a href="https://hpcalcs.com/product/hp-16c-collectors-edition/">HP 16c Collector’s Edition - HP Calc</a></li>

</ul>
</details>

**Discussion**: Community comments express strong nostalgia for the original HP-16C but mixed feelings about the Collector's Edition. Many users praise the durability of their original calculators while questioning the build quality of the new reissue. Some recommend alternatives like the SwissMicros DM16L as a more reliable modern option.

**Tags**: `#HP calculators`, `#retro computing`, `#collector's edition`, `#programming tools`

---

<a id="item-11"></a>
## [datasette-agent-micropython 0.1a0 Released](https://simonwillison.net/2026/Jun/2/datasette-agent-micropython/#atom-everything) ⭐️ 6.0/10

Simon Willison released version 0.1a0 of datasette-agent-micropython, an alpha tool that executes AI-generated Python code safely within a WebAssembly sandbox. Initial tests indicate GPT-5.5 has not yet managed to break out of the sandbox. This release addresses a critical safety need for AI-powered data analysis tools by providing a secure execution environment for untrusted code. It enables Datasette Agent to safely generate and run Python code, paving the way for more autonomous AI assistants in data exploration. The tool leverages WebAssembly as a sandboxing mechanism, using wasmtime-py and a Python WASM build from VMware Wasm Labs. It is still in early alpha, and the developer invites the community to test its security against AI-generated code.

rss · Simon Willison · Jun 2, 19:28

**Background**: Datasette Agent is an AI assistant for Datasette that helps users explore, query, and chart data. WebAssembly provides a lightweight, secure sandbox for running untrusted code by compiling it into a binary format that executes in a restricted environment. This combination allows AI models like GPT-4 (and newer) to generate code that runs safely without risking the host system.

<details><summary>References</summary>
<ul>
<li><a href="https://til.simonwillison.net/webassembly/python-in-a-wasm-sandbox">Run Python code in a WebAssembly sandbox - Simon Willison</a></li>
<li><a href="https://simonwillison.net/2026/May/21/datasette-agent/">Datasette Agent - simonwillison.net</a></li>
<li><a href="https://github.com/ciresnave/wasm-sandbox">GitHub - ciresnave/wasm-sandbox: A secure WebAssembly sandbox ...</a></li>

</ul>
</details>

**Tags**: `#python`, `#sandboxing`, `#datasette`, `#webassembly`, `#AI safety`

---