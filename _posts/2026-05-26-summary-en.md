---
layout: default
title: "Horizon Summary: 2026-05-26 (EN)"
date: 2026-05-26
lang: en
---

> From 31 items, 9 important content pieces were selected

---

1. [Microsoft Copilot Cowork Feature Vulnerable to Prompt Injection Data Exfiltration](#item-1) ⭐️ 8.0/10
2. [California proposes Linux exemption from age-verification law](#item-2) ⭐️ 8.0/10
3. [Armin Ronacher Slams AI-Generated Bug Reports](#item-3) ⭐️ 8.0/10
4. [Mullvad Rolls Out Exit IP Fingerprinting Mitigation](#item-4) ⭐️ 7.0/10
5. [Magnifica Humanitas: Vatican Encyclical on Tech Ethics](#item-5) ⭐️ 7.0/10
6. [C Extensions and Portability Challenges](#item-6) ⭐️ 7.0/10
7. [Datasette 1.0a30 Introduces Customizable Jump to Menu](#item-7) ⭐️ 7.0/10
8. [LLM recreates 1983 game 'Mad House' from PDF](#item-8) ⭐️ 7.0/10
9. [Norway Uses 2 PB Huawei Flash & HPE Cray for Sovereign LLM](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Microsoft Copilot Cowork Feature Vulnerable to Prompt Injection Data Exfiltration](https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files) ⭐️ 8.0/10

Researchers at PromptArmor demonstrated a prompt injection attack on Microsoft Copilot's 'cowork' feature, where a malicious skill can exfiltrate sensitive user data to an attacker-controlled server. This vulnerability poses a serious security risk for enterprises widely adopting Copilot, as it undermines trust in AI agents handling sensitive data. It highlights the dangers of rushing AI features to production without adequate security measures. The attack uses a crafted skill with only five lines of innocuous-looking code that, when uploaded, triggers Copilot to execute 'curl | bash' commands via prompt injection, sending data to an external server. The cowork feature is still in beta/preview and rolling out gradually.

hackernews · Kneenex · May 25, 21:45 · [Discussion](https://news.ycombinator.com/item?id=48272354)

**Background**: Prompt injection is a security exploit where malicious inputs cause large language models to behave unexpectedly. Microsoft Copilot's cowork feature is an AI automation layer that can execute multi-step tasks across Office applications. Skills are user-uploaded programs that extend Copilot's capabilities, similar to plugins, but this one contains a hidden prompt that hijacks the assistant.

<details><summary>References</summary>
<ul>
<li><a href="https://support.microsoft.com/en-us/microsoft-365-copilot/get-started-with-cowork-frontier">Get started with Cowork (Frontier) | Microsoft Support</a></li>
<li><a href="https://fortune.com/2026/03/09/microsoft-copilot-cowork-ai-agents-anthropic-e7-m365-saas/">Microsoft debuts Copilot Cowork built with Anthropic’s help... | Fortune</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some argue that the attack is 'works as expected' since skills are programs with full access, while others criticize Microsoft for rushing the feature to production without proper security hardening. One commenter notes that the title is misleading and rage-baity, though the technical finding is valid.

**Tags**: `#security`, `#prompt injection`, `#AI agents`, `#Microsoft`, `#exfiltration`

---

<a id="item-2"></a>
## [California proposes Linux exemption from age-verification law](https://www.tomshardware.com/software/linux/california-moves-to-exempt-linux-from-its-upcoming-age-verification-law-after-backlash-over-forcing-operating-systems-to-collect-users-ages-amendment-proposed-by-the-same-lawmaker-who-wrote-the-original-law) ⭐️ 8.0/10

California lawmaker proposed an amendment to exempt Linux from the state's upcoming age-verification law after widespread backlash from the open-source community. This move protects open-source operating systems from intrusive age-verification requirements, setting a significant precedent for tech regulation and preserving user privacy and software freedom. The amendment was introduced by the same lawmaker who authored the original law, and it specifically exempts Linux and potentially other open-source operating systems from collecting users' ages.

hackernews · rbanffy · May 25, 18:19 · [Discussion](https://news.ycombinator.com/item?id=48269961)

**Background**: California's age-verification law requires platforms to implement age checks to protect minors online. Critics argued that applying it to Linux would force the open-source OS to implement user surveillance, violating core principles of privacy and freedom.

**Discussion**: Comments highlight a political win for the open-source community but express broader concerns about the law's burden shifting to consumers rather than regulating companies. Some note the irony that nerds using Linux can access more content while others remain restricted.

**Tags**: `#Linux`, `#age-verification`, `#California law`, `#open source`, `#privacy`

---

<a id="item-3"></a>
## [Armin Ronacher Slams AI-Generated Bug Reports](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher published a blog post criticizing AI-generated bug reports for their inaccuracy and overconfidence, advocating for a simple four-step format that captures only what the human directly observed. This critique highlights a growing challenge in open-source maintenance where low-quality AI-generated issues waste maintainers' time and introduce noise, threatening the efficiency of collaborative software development. Ronacher's proposed format asks reporters to state the command run, the expected result, the actual result, and the exact error or log, stripping away any AI-generated speculation or rephrasing.

rss · Simon Willison · May 24, 18:46

**Background**: AI tools like large language models (LLMs) are increasingly used to compose or rephrase bug reports, but they often produce plausible-sounding but incorrect analyses. This phenomenon, sometimes called 'slop,' burdens open-source maintainers who must sift through misleading information.

**Tags**: `#AI`, `#open source`, `#bug reports`, `#software engineering`, `#LLM`

---

<a id="item-4"></a>
## [Mullvad Rolls Out Exit IP Fingerprinting Mitigation](https://mullvad.net/en/help/exit-ip-vpn-servers-mitigation-rollout) ⭐️ 7.0/10

Mullvad has announced a mitigation rollout against exit IP fingerprinting for its VPN servers, which will regenerate WireGuard keys and change internal IP addresses to prevent linking users across different servers. This mitigation addresses a privacy vulnerability that could allow attackers to track VPN users across servers, enhancing user anonymity and setting a privacy standard for the VPN industry. The new method assigns exit IP addresses randomly per session, eliminating correlation between servers, and automatically regenerates WireGuard keys to prevent long-term tracking.

hackernews · Cider9986 · May 25, 17:45 · [Discussion](https://news.ycombinator.com/item?id=48269580)

**Background**: Exit IP fingerprinting is a technique where an attacker observes which exit IP addresses a user is assigned on different VPN servers to track their activity. Mullvad's new mitigation breaks this correlation by ensuring that assignments are random and independent per server, making it harder to link a user across sessions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TCP/IP_stack_fingerprinting">TCP/IP stack fingerprinting - Wikipedia</a></li>
<li><a href="https://mullvad.net/en/blog/exit-ip-fingerprinting-between-vpn-servers">Exit IP fingerprinting between VPN servers | Mullvad VPN</a></li>

</ul>
</details>

**Discussion**: Community comments highlight features like Mullvad Browser's built-in proxy and random mode for IP rotation, with overall positive sentiment. Some users express interest in broader anti-fingerprinting measures, such as spoofing consistent yet standardized device profiles.

**Tags**: `#VPN`, `#privacy`, `#fingerprinting`, `#Mullvad`, `#security`

---

<a id="item-5"></a>
## [Magnifica Humanitas: Vatican Encyclical on Tech Ethics](https://www.vatican.va/content/leo-xiv/en/encyclicals/documents/20260515-magnifica-humanitas.html) ⭐️ 7.0/10

Pope Leo XIV issued an encyclical titled Magnifica Humanitas, which addresses the ethical and societal implications of technology and the concentration of power. This encyclical from the Vatican, a major moral authority, offers a significant framework for discussing technology ethics, influencing global discourse on AI and power dynamics. The encyclical asserts that 'technology is never neutral' and that builders bear ethical responsibility, warning against the concentration of power via nuclear energy, biotechnology, and information technology.

hackernews · theletterf · May 25, 10:11 · [Discussion](https://news.ycombinator.com/item?id=48265206)

**Background**: An encyclical is a formal papal letter addressing contemporary issues. This document, Magnifica Humanitas, continues the Vatican's focus on technology's moral dimensions, building on previous warnings by Pope Francis about technology's impact on humanity.

**Discussion**: Commenters generally praise the Vatican's perspective on technology, with some noting it raises important questions about power and responsibility. An atheist commenter remarked that the Vatican has some of the best takes on technology, while others question whether technology can be tamed for societal good.

**Tags**: `#ethics`, `#technology`, `#society`, `#AI`, `#Vatican`

---

<a id="item-6"></a>
## [C Extensions and Portability Challenges](https://lemon.rip/w/6-c-extensions-compilers/) ⭐️ 7.0/10

The article examines how compiler-specific extensions (like __attribute__) cause portability issues when moving code between GCC, Clang, TinyCC, and other compilers, and discusses workarounds. This matters because C is widely used in systems programming, and poor portability forces developers to maintain fragile workarounds, hindering adoption of alternative compilers and platforms. Common workarounds include conditional #ifdef guards (e.g., checking for __GNUC__), but they often fail when a compiler doesn't pretend to be GCC but still uses similar extensions. The article also highlights efforts like slimcc's platform header hacks to improve compatibility.

hackernews · xngbuilds · May 25, 14:15 · [Discussion](https://news.ycombinator.com/item?id=48267126)

**Background**: C extensions are non-standard features added by compilers to provide low-level functionality, such as __attribute__ for aligning variables or specifying function attributes. Each compiler (GCC, Clang, MSVC, etc.) has its own set of extensions, and code relying on them may fail to compile on another compiler. Standard C (ISO C) avoids these extensions, but real-world projects often depend on them for performance or hardware access.

**Discussion**: Community comments from developers like ndesaulniers (kernel developer) and WalterBright (D language creator) confirm the pain, with WalterBright sharing his experience implementing ImportC and encountering 'nutburger nonsense' in header files. Others suggest that the Common Lisp ecosystem's approach of letting portability libraries emerge could serve as a model.

**Tags**: `#C programming`, `#portability`, `#compilers`, `#systems programming`, `#extensions`

---

<a id="item-7"></a>
## [Datasette 1.0a30 Introduces Customizable Jump to Menu](https://simonwillison.net/2026/May/24/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a30, released on May 24, 2026, adds a new customizable 'Jump to' menu that can be activated by pressing '/' on the latest demo site. It also introduces the jump_items_sql() plugin hook, allowing plugins to contribute items to the menu's search results. This enhancement improves navigation within Datasette instances, making it easier for users to quickly find databases, tables, and debug options. The plugin hook opens up extensibility, enabling the community to build custom navigation shortcuts tailored to their data publishing needs. The 'Jump to' menu is described in detail on the Datasette blog, and the jump_items_sql() hook is documented in the official plugin hooks documentation. The menu can be tried on the latest.datasette.io demo site.

rss · Simon Willison · May 24, 23:52

**Background**: Datasette is an open-source tool for exploring and publishing data, particularly SQLite databases, created by Simon Willison. It provides a web interface for browsing and querying datasets, and supports a plugin system for extending its functionality. This alpha release continues development toward the 1.0 stable release.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/May/21/datasette-agent/">Datasette Agent | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#opensource`, `#plugin`, `#sqlite`, `#datapublishing`

---

<a id="item-8"></a>
## [LLM recreates 1983 game 'Mad House' from PDF](https://simonwillison.net/2026/May/24/usborne-mad-house/#atom-everything) ⭐️ 7.0/10

Simon Willison used Claude to build an interactive JavaScript version of the 1983 game 'Mad House' from Usborne's Creepy Computer Games PDF. This demonstrates how large language models can efficiently recreate historical software from scanned documents, preserving retro gaming experiences. The game was created by feeding the PDF into Claude with a prompt requesting a mobile-friendly vanilla JS artifact with a retro aesthetic.

rss · Simon Willison · May 24, 17:14

**Background**: Usborne published free PDFs of their 1980s computer books, including 'Creepy Computer Games' from 1983. Claude is an AI assistant by Anthropic capable of coding and understanding documents. 'Mad House' is a text-based maze horror game originally written for home computers like the Commodore 64.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/introducing-claude">Introducing Claude \ Anthropic</a></li>
<li><a href="https://archive.org/details/Creepy_Computer_Games_1983_Usborne_Publishing">Usborne creepy computer games : Reynolds, Colin : Free Download, Borrow, and Streaming : Internet Archive</a></li>

</ul>
</details>

**Tags**: `#retro computing`, `#AI-assisted development`, `#JavaScript`, `#game recreation`, `#Claude`

---

<a id="item-9"></a>
## [Norway Uses 2 PB Huawei Flash & HPE Cray for Sovereign LLM](https://www.blocksandfiles.com/flash/2026/05/22/norways-2-petabytes-of-huawei-flash-storage-and-llm-training/5244910) ⭐️ 6.0/10

Norway has deployed 2 petabytes of Huawei flash storage and an HPE Cray Supercomputing EX system to train a sovereign large language model (LLM) dedicated to the Norwegian language and culture. This initiative underscores the growing trend of sovereign AI, where countries invest in independent AI infrastructure to reduce reliance on foreign technologies and preserve cultural and linguistic data. It also highlights the use of HPC systems for LLM training at a more modest scale, challenging assumptions about the required resources. The HPE Cray system, named Olivia, features 448 GPUs and 64,512 CPU cores, which some commenters consider modest for training a fully fledged LLM. The 2 PB of flash storage from Huawei is relatively affordable, potentially costing around $200,000.

hackernews · rbanffy · May 25, 19:37 · [Discussion](https://news.ycombinator.com/item?id=48270770)

**Background**: Sovereign AI refers to national strategies aimed at developing independent AI capabilities, including models, data, and hardware, to reduce dependence on foreign providers. Norway's effort is part of this trend, focusing on creating an LLM that understands its unique language and culture, which general English-centric models may not cover. The Norwegian National Library's extensive digitized text collection provides a rich training dataset.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hpe.com/us/en/collaterals/collateral.a00094635enw.html">HPE Cray Supercomputing EX QuickSpecs | HPE</a></li>
<li><a href="https://grokipedia.com/page/Sovereign_AI">Sovereign AI</a></li>
<li><a href="https://e.huawei.com/en/products/storage/hybrid-flash-storage">OceanStor Hybrid Flash Storage | Huawei Enterprise</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the sufficiency of the hardware, with one calling it a potential waste of resources and suggesting fine-tuning an open-source model instead. Others proposed sharing Norwegian training data with all model builders rather than building a custom LLM. A few noted the low cost of flash storage, questioning the project's scale.

**Tags**: `#LLM`, `#Norway`, `#sovereign AI`, `#flash storage`, `#HPC`

---