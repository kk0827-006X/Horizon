---
layout: default
title: "Horizon Summary: 2026-05-19 (EN)"
date: 2026-05-19
lang: en
---

> From 37 items, 8 important content pieces were selected

---

1. [Elon Musk Loses Lawsuit Against Sam Altman and OpenAI](#item-1) ⭐️ 8.0/10
2. [FBI Seeks Nationwide License Plate Reader Data Access](#item-2) ⭐️ 8.0/10
3. [GDS Opposes NHS Retreat from Open Source](#item-3) ⭐️ 8.0/10
4. [Anthropic acquires Stainless, shuts down SDK generator](#item-4) ⭐️ 7.0/10
5. [Hyperpolyglot Lisp: Cross-Dialect Reference](#item-5) ⭐️ 7.0/10
6. [Using Git's --author flag to block AI bot spam on GitHub](#item-6) ⭐️ 7.0/10
7. [Files.md: Open-source Obsidian alternative with chat UI](#item-7) ⭐️ 7.0/10
8. [Letting AIs Run Radio Stations: A Hilarious Experiment](#item-8) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Elon Musk Loses Lawsuit Against Sam Altman and OpenAI](https://techcrunch.com/2026/05/18/elon-musk-has-lost-his-lawsuit-against-sam-altman-and-openai/) ⭐️ 8.0/10

A jury found that Elon Musk's lawsuit against OpenAI and Sam Altman was filed too late, dismissing all claims due to the statute of limitations. This verdict reinforces legal protections for OpenAI's transition from non-profit to for-profit, and may discourage future lawsuits on similar grounds. The jury determined that Musk's claims were untimely because similar events occurred in 2019 and 2021, and Musk could have sued then. The court only answered yes/no questions, so the exact reasoning is not public.

hackernews · nycdatasci · May 18, 17:38 · [Discussion](https://news.ycombinator.com/item?id=48182754)

**Background**: Elon Musk co-founded OpenAI in 2015 as a non-profit, but later left. In 2023, he sued OpenAI and its CEO Sam Altman, alleging they abandoned the non-profit mission by partnering with Microsoft. The statute of limitations requires lawsuits to be filed within a set time after the alleged harm.

**Discussion**: Commenters noted that the jury's finding of untimeliness was expected, but some raised concerns about the precedent for non-profits transferring assets to for-profits. Musk's counsel indicated an appeal, but the grounds remain unclear.

**Tags**: `#AI`, `#OpenAI`, `#lawsuit`, `#Elon Musk`, `#legal`

---

<a id="item-2"></a>
## [FBI Seeks Nationwide License Plate Reader Data Access](https://www.404media.co/the-fbi-wants-to-buy-nationwide-access-to-license-plate-readers/) ⭐️ 8.0/10

The FBI is seeking to purchase nationwide access to automatic license plate reader (ALPR) data, enabling broad surveillance of vehicle movements across the United States. This raises significant privacy and civil liberties concerns, as it could allow the government to track individuals' locations without warrants. The move reflects a growing trend of government agencies acquiring mass surveillance capabilities. The purchase would likely involve aggregating data from private and public ALPR systems, creating a massive database of vehicle location histories. Legal frameworks regulating such data are inconsistent across states.

hackernews · cdrnsf · May 18, 19:28 · [Discussion](https://news.ycombinator.com/item?id=48184350)

**Background**: Automatic license plate readers (ALPR) use cameras and software to automatically capture and store license plate numbers, often used by law enforcement to track vehicles of interest. The FBI's proposal would expand access beyond local operations, centralizing data for federal use. Only three states passed laws regulating ALPR data in 2025, highlighting the regulatory gap.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dhs.gov/science-and-technology/saver/automatic-license-plate-readers">Automatic License Plate Readers - Homeland Security</a></li>
<li><a href="https://stateline.org/2025/10/10/despite-widespread-interest-only-3-states-passed-license-plate-reader-laws-this-year/">Despite widespread interest, only 3 states passed license ...</a></li>

</ul>
</details>

**Discussion**: Comments express skepticism about privacy protections, with some suggesting that personal data should be considered a liability rather than an asset. Others discuss methods to evade plate readers, indicating a lack of trust in government surveillance. There is also debate about jurisdictional challenges and the effectiveness of such data collection.

**Tags**: `#privacy`, `#surveillance`, `#government`, `#data-collection`, `#civil-liberties`

---

<a id="item-3"></a>
## [GDS Opposes NHS Retreat from Open Source](https://simonwillison.net/2026/May/17/gds-weighs-in/#atom-everything) ⭐️ 8.0/10

On May 14, 2026, the UK Government Digital Service (GDS) published guidance recommending that public sector organizations keep open source repositories public by default, pushing back against the NHS's decision to close access due to vulnerabilities reported via Project Glasswing. This highlights a policy conflict between security and openness in government technology, and GDS's stance reaffirms the cost-saving and scrutiny benefits of open source, potentially influencing other public bodies worldwide. GDS's guidance, titled "AI, open code and vulnerability risk in the public sector," emphasizes "open by default" with closure used only sparingly and deliberately, and Terence Eden interprets this as a rare public internal civil service disagreement.

rss · Simon Willison · May 17, 15:59

**Background**: Project Glasswing is a cybersecurity initiative launched by Anthropic on April 7, 2026, that uses advanced AI to find vulnerabilities in critical software. The NHS closed its open source repositories after vulnerabilities were reported via this project. GDS's response is notable because it publicly counters the NHS's move, signaling a significant policy debate within the UK government.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Glasswing">Project Glasswing</a></li>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era</a></li>

</ul>
</details>

**Tags**: `#open source`, `#government policy`, `#security`, `#NHS`, `#GDS`

---

<a id="item-4"></a>
## [Anthropic acquires Stainless, shuts down SDK generator](https://www.anthropic.com/news/anthropic-acquires-stainless) ⭐️ 7.0/10

Anthropic has acquired Stainless, a platform for generating SDKs from OpenAPI specs, and will wind down all hosted Stainless products including the SDK generator, effective immediately. This acquisition reflects Anthropic's strategic focus on enhancing the Claude platform and developer experience, but it also raises concerns about tool consolidation and walled gardens in the AI ecosystem. New signups, projects, and SDK generation on Stainless are no longer available. The deal is primarily an acqui-hire, bringing Stainless's engineering talent to Anthropic to improve Claude's API tooling.

hackernews · tomeraberbach · May 18, 17:01 · [Discussion](https://news.ycombinator.com/item?id=48182281)

**Background**: SDK generators automatically create language-specific client libraries from API specifications like OpenAPI, saving developers time and reducing errors. Stainless was a popular tool that also provided hosted documentation and MCP servers. Anthropic's decision to shut down the product suggests it plans to integrate the team's expertise internally rather than continue offering a standalone service.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stainless.com/">Stainless - Best-in-class developer interfaces for your API</a></li>
<li><a href="https://www.everydev.ai/tools/stainless">Stainless - SDK Generator from OpenAPI Spec | EveryDev.ai</a></li>
<li><a href="https://aidirectory.com/news/anthropic-acquires-stainless-shuts-down-hosted-products">Anthropic acquires Stainless and plans to shut down its ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed feelings: some congratulated the Stainless team but lamented the loss of a useful product, calling it a typical acqui-hire; others criticized the sudden shutdown and worried about the trend of AI companies creating walled gardens through acquisitions.

**Tags**: `#acquisition`, `#anthropic`, `#stainless`, `#api-tools`, `#developer-experience`

---

<a id="item-5"></a>
## [Hyperpolyglot Lisp: Cross-Dialect Reference](https://hyperpolyglot.org/lisp) ⭐️ 7.0/10

A comprehensive side-by-side reference comparing syntax and features of Common Lisp, Racket, Clojure, and Emacs Lisp has been published on Hyperpolyglot.org. This reference helps Lisp programmers quickly understand differences between dialects, promoting cross-pollination and easing transition between dialects. The page covers syntax, data types, functions, macros, and more, with examples. Community members have pointed out non-idiomatic examples and missing documentation features.

hackernews · veqq · May 18, 19:27 · [Discussion](https://news.ycombinator.com/item?id=48184322)

**Background**: Lisp is a family of programming languages with a long history. Common Lisp, Racket, Clojure, and Emacs Lisp are major dialects, each with unique features. Hyperpolyglot.org provides side-by-side comparisons of programming languages.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyperpolyglot">Hyperpolyglot</a></li>
<li><a href="https://en.wikipedia.org/wiki/Clojure">Clojure</a></li>
<li><a href="https://clojure.org/">Clojure</a></li>

</ul>
</details>

**Discussion**: Comments include corrections to idiomatic Common Lisp code, suggestions for documenting functions, and notes on compilation behavior in SBCL. Overall sentiment is positive, with users appreciating the resource and offering improvements.

**Tags**: `#Lisp`, `#programming-languages`, `#reference`, `#comparison`

---

<a id="item-6"></a>
## [Using Git's --author flag to block AI bot spam on GitHub](https://archestra.ai/blog/only-responsible-ai) ⭐️ 7.0/10

A blog post describes using Git's --author flag to filter out AI-generated pull request spam in a GitHub repository. This allows maintainers to automatically reject commits from suspicious bot authors. AI bot spam is overwhelming open-source maintainers, especially in repos with bounties, causing wasted time and reduced trust. This simple technique offers a low-cost defense, but also highlights security gaps in GitHub's contributor approval system. The --author flag filters commits by author name or email pattern, enabling maintainers to reject PRs from known bot accounts. However, malicious actors can spoof author information, and GitHub's approval settings may allow bots to bypass restrictions after a single accepted PR.

hackernews · ildari · May 18, 15:24 · [Discussion](https://news.ycombinator.com/item?id=48181125)

**Background**: Git records both author and committer fields for each commit; the --author flag can be used with git log or git rev-list to search for specific authors. GitHub provides settings to require approval for first-time contributors, but a user who has had any PR merged is no longer considered a first-time contributor. This design can be exploited by bots to gain elevated privileges after a trivial accepted PR.

<details><summary>References</summary>
<ul>
<li><a href="https://labex.io/tutorials/git-how-to-use-git-author-flag-correctly-419252">How to use Git author flag correctly - LabEx</a></li>
<li><a href="https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/filtering-and-searching-issues-and-pull-requests">Filtering and searching issues and pull requests - GitHub Docs</a></li>
<li><a href="https://www.linkedin.com/pulse/githubs-kill-switch-pull-requests-why-ai-spam-now-workflow-kumar-l-la0yc">Stop AI Spam Breaking Your GitHub PRs - LinkedIn</a></li>

</ul>
</details>

**Discussion**: Commenters raised security implications, noting that contributor approval bypass can be exploited. They also criticized GitHub for not implementing basic anti-spam measures, and proposed alternative solutions like ELO-based quality scoring, deleting PRs, and blocking accounts with high rejection rates. Some blamed the AI hype for encouraging low-effort spam.

**Tags**: `#AI spam`, `#GitHub`, `#open source`, `#security`, `#community management`

---

<a id="item-7"></a>
## [Files.md: Open-source Obsidian alternative with chat UI](https://github.com/zakirullin/files.md) ⭐️ 7.0/10

Files.md is a newly released open-source note-taking app that positions itself as an alternative to Obsidian, featuring a unique chat-based interface for interacting with Markdown files. This matters because it introduces a novel chat interface that could change how users interact with notes, while also highlighting the demand for open-source alternatives to popular but proprietary tools like Obsidian. Files.md is hosted on GitHub (zakirullin/files.md) and uses Markdown files stored locally. Its chat interface allows users to query or update notes through natural language, potentially leveraging AI assistants.

hackernews · zakirullin · May 18, 13:33 · [Discussion](https://news.ycombinator.com/item?id=48179677)

**Background**: Obsidian is a popular note-taking application that works with local Markdown files but is not open-source. Many users desire open-source alternatives for transparency and customization. Files.md offers a different paradigm by replacing the traditional folder/file view with a conversational interface.

**Discussion**: Community comments express surprise that Obsidian is not open-source, interest in the chat interface, and debates on whether it qualifies as an alternative to Obsidian. Some users also mention Joplin as another open-source option. Overall sentiment is positive, with curiosity about how the chat interface could change note-taking workflows.

**Tags**: `#open-source`, `#note-taking`, `#obsidian`, `#markdown`

---

<a id="item-8"></a>
## [Letting AIs Run Radio Stations: A Hilarious Experiment](https://andonlabs.com/blog/andon-fm) ⭐️ 6.0/10

Andon Labs gave four AI agents (Claude, GPT, Gemini, Grok) $20 each and full autonomy to run 24/7 radio stations, including live broadcasting and business tasks, for six months. This experiment reveals both the promise and pitfalls of autonomous AI agents in creative and business roles, showing they can produce engaging content but often fail at reliability and profitability. Each AI agent used a different model: Claude Opus 4.7, GPT-5.5, Gemini 3.1 Pro, and Grok 4.3. Revenue was terrible, but shows were sometimes hilarious; one station (Grok and Roll) got stuck replaying a single phrase.

hackernews · lukaspetersson · May 18, 18:12 · [Discussion](https://news.ycombinator.com/item?id=48183301)

**Background**: Andon Labs builds 'Safe Autonomous Organizations' and previously ran experiments in retail with vending machines and stores. They let AI agents operate without human intervention to study failure modes. This experiment continues their tradition of publicly testing AI autonomy in real-world scenarios.

<details><summary>References</summary>
<ul>
<li><a href="https://andonlabs.com/blog/andon-fm">We let four AIs run radio stations. Here's what happened. | Andon Labs</a></li>
<li><a href="https://the-decoder.com/four-ai-models-ran-radio-stations-for-six-months-and-the-results-ranged-from-competent-to-unhinged/">Four AI models ran radio stations for six months and the results ranged from competent to unhinged</a></li>

</ul>
</details>

**Discussion**: Commenters noted glitches like Grok and Roll's stuck loop, found it amusing, and appreciated the transparency about failures. Some asked about revenue and technical details, while others shared similar projects.

**Tags**: `#AI`, `#experiment`, `#media`, `#automation`

---