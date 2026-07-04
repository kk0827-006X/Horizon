---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 55 items, 12 important content pieces were selected

---

1. [Pegasus Spyware Hits EU Parliament Spy Investigators](#item-1) ⭐️ 8.0/10
2. [SearXNG: A Free Privacy-Respecting Metasearch Engine](#item-2) ⭐️ 7.0/10
3. [Guide to running SOTA LLMs locally at $40k+ cost](#item-3) ⭐️ 7.0/10
4. [Costco: The Anti-Amazon Business Model](#item-4) ⭐️ 7.0/10
5. [Open Source AI Gap Map Indexes 426 Products](#item-5) ⭐️ 7.0/10
6. [Josh Comeau Reports AI-Driven Drop in Course Sales](#item-6) ⭐️ 7.0/10
7. [Let AI Coding Assistants Use Their Own Judgement to Save Tokens](#item-7) ⭐️ 7.0/10
8. [Using DSPy to Evaluate and Improve Datasette Agent Prompts](#item-8) ⭐️ 7.0/10
9. [Understand to Participate: Deep Code Understanding for AI Collaboration](#item-9) ⭐️ 7.0/10
10. [Factories Are Just Rooms](#item-10) ⭐️ 6.0/10
11. [Simon Willison's June Newsletter: AI Models and Tool Updates](#item-11) ⭐️ 6.0/10
12. [Simon Willison Releases llm-coding-agent 0.1a0 Alpha](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Pegasus Spyware Hits EU Parliament Spy Investigators](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

Citizen Lab discovered that Pegasus spyware infected the iPhone of European Parliament member Stelios Kouloglou, who serves on a committee investigating spyware, with infections occurring in October 2022 and March 2023. This infection indicates that a state actor with cross-European authorization is actively spying on the very committee investigating spyware abuse, undermining democratic oversight and raising severe cybersecurity concerns for EU institutions. The infections were detected through forensic analysis of Kouloglou's iPhone, and the first infection overlaps with a Pegasus campaign targeting Russian and Belarusian-speaking exiled journalists in Europe, suggesting a coordinated campaign.

hackernews · ledoge · Jul 3, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48779683)

**Background**: Pegasus is spyware developed by Israeli company NSO Group, capable of remotely accessing a mobile device's data and sensors. It is sold only to governments, but has been widely abused to target journalists, activists, and politicians. Citizen Lab is a University of Toronto research group that investigates digital threats.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about consequences, noting past scandals in Greece where Pegasus was used against politicians without resolution. Some questioned the separation of work and personal devices for EU parliament members, while others highlighted the need for better oversight.

**Tags**: `#cybersecurity`, `#surveillance`, `#Pegasus`, `#espionage`, `#European Parliament`

---

<a id="item-2"></a>
## [SearXNG: A Free Privacy-Respecting Metasearch Engine](https://github.com/searxng/searxng) ⭐️ 7.0/10

SearXNG is a free internet metasearch engine that aggregates results from multiple sources while respecting user privacy. It provides a privacy-centric alternative to mainstream search engines, enabling users to avoid tracking and profiling. Its open-source nature and active community support make it a valuable tool for privacy-conscious individuals and developers building AI agents. SearXNG supports JSON results and can be used for internal document search or RAG applications. However, it may be slower than direct search engines and occasionally require CAPTCHA solving.

hackernews · theanonymousone · Jul 3, 20:15 · [Discussion](https://news.ycombinator.com/item?id=48779454)

**Background**: A metasearch engine aggregates results from multiple underlying search engines into a single list. SearXNG is a fork of Searx, which itself was inspired by the Seeks project. It allows users to self-host the engine, giving them control over their search data. The project is actively maintained on GitHub with over 15,000 stars.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Metasearch_engine">Metasearch engine - Wikipedia</a></li>
<li><a href="https://github.com/searxng/searxng">GitHub - searxng/searxng: SearXNG is a free internet metasearch engine which aggregates results from various search services and databases. Users are neither tracked nor profiled. · GitHub</a></li>
<li><a href="https://docs.searxng.org/user/about.html">About SearXNG - SearXNG Documentation (2026.7.3+21773bbb2)</a></li>

</ul>
</details>

**Discussion**: Community comments highlight both benefits and trade-offs. The original creator noted the limitations of the metasearch concept and moved on to a new full-text indexing project. Users appreciate the privacy gain but acknowledge it's slower and may get blocked by some search engines. One commenter noted that SearXNG is a key tool for providing search to local models.

**Tags**: `#privacy`, `#search engine`, `#open source`, `#metasearch`

---

<a id="item-3"></a>
## [Guide to running SOTA LLMs locally at $40k+ cost](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob has published a comprehensive guide on building expensive local setups (budget $40k+) for running state-of-the-art LLMs like GLM-5.2 and Qwen3.6, with detailed hardware recommendations and quantization techniques. This guide highlights the massive cost barrier to achieving near-cloud-quality LLM inference locally, sparking debate about whether local setups are economically viable compared to subscription services like Claude Opus at $200/month. The recommended build uses four $12k GPUs (e.g., H200s) totaling ~$50k, relying on heavy quantization like NVFP4 and REAP pruning to reduce model size from ~1T to ~594B parameters. However, community members note that even quantized models may suffer from quality degradation or reasoning loops.

hackernews · livestyle · Jul 3, 15:03 · [Discussion](https://news.ycombinator.com/item?id=48775921)

**Background**: Running large language models locally requires significant GPU VRAM — for example, a 70B parameter model in FP16 needs ~140GB VRAM. Quantization reduces memory by using lower-precision numbers (e.g., 4-bit), but may impair performance. Many enthusiasts opt for cheaper setups like 2x RTX 3090s (48GB VRAM) to run smaller models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/deep-learning/recommended-hardware-for-running-llms-locally/">Recommended Hardware for Running LLMs Locally</a></li>
<li><a href="https://epoch.ai/data-insights/llm-inference-price-trends">LLM inference prices have fallen rapidly but unequally across ...</a></li>
<li><a href="https://localllm.in/blog/quantization-explained">The Complete Guide to LLM Quantization | LocalLLM.in</a></li>

</ul>
</details>

**Discussion**: Commenters are skeptical about the cost, with jacobgold noting that $50k equals 16.8 years of Claude Opus subscription. Aurornis warns about inflated expectations and hidden costs. GTP suggests an intermediate option using 128GB unified memory (e.g., Apple M-series) to run DeepSeek V4 flash via DwarfStar as a more practical compromise.

**Tags**: `#local-llm`, `#hardware`, `#cost-analysis`, `#guide`, `#llm-inference`

---

<a id="item-4"></a>
## [Costco: The Anti-Amazon Business Model](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

An analysis argues that Costco's business model deliberately avoids the complexities of last-mile delivery, instead optimizing for bulk, in-person shopping, making it the strategic opposite of Amazon. This analysis highlights the strategic trade-offs in logistics and business model design, offering valuable insights for software engineers and entrepreneurs about the wisdom of avoiding unnecessary complexity. Costco uses a membership model, limited product selection, and bulk packaging to minimize logistical costs, while Amazon invests heavily in last-mile delivery infrastructure.

hackernews · bookofjoe · Jul 3, 15:14 · [Discussion](https://news.ycombinator.com/item?id=48776044)

**Background**: Last-mile delivery refers to the final leg of the supply chain where goods are transported from a distribution hub to the end customer's doorstep. It is notoriously expensive and complex due to traffic, failed deliveries, and fragmentation. Costco's model sidesteps these challenges entirely by relying on customers to transport their own purchases in bulk.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dhl.com/discover/en-global/logistics-advice/import-export-advice/last-mile-solutions">What Is Last Mile Delivery & How Can You Improve It? - DHL</a></li>
<li><a href="https://www.ascm.org/topics/last-mile-delivery/">Understanding Last-Mile Delivery in Supply Chain | ASCM</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with the article's premise, with one likening Costco's approach to the engineering proverb 'a wise person avoids a problem.' Another praised Costco as an example of American greatness. Some noted regional differences, such as UK Costco's membership requirements.

**Tags**: `#business-strategy`, `#logistics`, `#costco`, `#amazon`, `#ecommerce`

---

<a id="item-5"></a>
## [Open Source AI Gap Map Indexes 426 Products](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 7.0/10

Current AI launched the Open Source AI Gap Map v0.1, indexing 421 products (later updated to 426) across the open source AI stack, including software tools, models, datasets, and hardware projects. This comprehensive map helps identify gaps in the open source AI ecosystem, guiding investment and collaboration to strengthen public interest AI, especially given Current AI's $400M backing. The map covers 266 software tools, 85 models, 50 datasets, and 20 hardware projects from 228 organizations, with the underlying data released under an MIT license on GitHub.

rss · Simon Willison · Jul 3, 22:04

**Background**: Current AI is a non-profit global partnership launched at the AI Action Summit in Paris in February 2025, aiming to build public interest AI. The Gap Map builds on work from Columbia Convening, MOF, Hugging Face, and others to catalog the open source AI stack and identify missing components.

<details><summary>References</summary>
<ul>
<li><a href="https://www.currentai.org/">Current AI | Building Public Interest AI Technology Together</a></li>
<li><a href="https://map.currentai.org/">Current AI – Open Source AI Gap Map</a></li>

</ul>
</details>

**Tags**: `#open source`, `#artificial intelligence`, `#ecosystem mapping`, `#Current AI`, `#Gap Map`

---

<a id="item-6"></a>
## [Josh Comeau Reports AI-Driven Drop in Course Sales](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

Josh W. Comeau reports that his new course 'Whimsical Animations' is on track to sell only one-third as many copies as typical, and his existing courses have seen sales drop by over 50% compared to last year, attributing the decline primarily to AI concerns. This highlights a growing trend where AI, particularly large language models (LLMs), is disrupting developer education by creating job uncertainty and offering free or low-cost personalized tutoring, threatening the business model of paid course creators. Josh W. Comeau, a prominent front-end developer educator, launched his third course and saw sales roughly ⅓ of a typical launch; he notes that multiple course creators he spoke to report similar revenue declines of 50% or more.

rss · Simon Willison · Jul 3, 21:25

**Background**: Large language models (LLMs) like GPT-4 are AI systems trained on vast text data that can generate, summarize, and analyze text. They are increasingly used for code generation, debugging, and even personalized tutoring, which competes with traditional paid courses. Many developers fear that AI might replace their jobs, reducing incentive to invest in learning new skills.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/large-language-models">What Are Large Language Models (LLMs)? | IBM</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/large-language-model-llm/">Large Language Model (LLM) - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: In the discussion, Josh W. Comeau laments that AI not only reduces course sales but also ingests creators' work without consent or compensation. Other course creators echo similar experiences, showing a consensus that AI is significantly hurting their revenue.

**Tags**: `#AI impact`, `#developer education`, `#online courses`, `#job market`

---

<a id="item-7"></a>
## [Let AI Coding Assistants Use Their Own Judgement to Save Tokens](https://simonwillison.net/2026/Jul/3/judgement/#atom-everything) ⭐️ 7.0/10

Simon Willison shares tips from the Claude Code team: let Fable use its own judgement on testing, and delegate smaller coding tasks to cheaper models like Sonnet or Haiku to conserve expensive Fable tokens. This practical approach helps developers maximize token efficiency and reduce costs when using high-end AI coding assistants like Claude Fable, especially as token prices are about to increase. Willison implemented a memory file instructing Claude Code to spawn subagents with model overrides: Sonnet for substantive implementation, Haiku for trivial edits, while keeping judgement-heavy tasks on the main model.

rss · Simon Willison · Jul 3, 18:51

**Background**: Claude Fable is Anthropic's most capable model, optimized for complex agentic coding but expensive to run per token. The Claude Code tool supports model aliases like Opus for planning and Sonnet for execution to balance cost and capability. Token optimization techniques are becoming essential as AI coding assistants are widely adopted for everyday development tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/model-config">Model configuration - Claude Code Docs</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://www.c-sharpcorner.com/article/ai-token-optimization-techniques-every-developer-should-know/">AI Token Optimization Techniques Every Developer Should Know</a></li>

</ul>
</details>

**Tags**: `#AI coding assistant`, `#Claude Code`, `#software development`, `#productivity`

---

<a id="item-8"></a>
## [Using DSPy to Evaluate and Improve Datasette Agent Prompts](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison used the DSPy framework to automatically evaluate and improve the SQL system prompts of Datasette Agent, a task he delegated to Claude Code with Claude Fable 5. The optimization identified issues like missing column names in schema listings that caused incorrect SQL queries. This demonstrates a practical, automated approach to prompt engineering for AI agents, reducing reliance on manual trial-and-error. It highlights how DSPy can systematically improve agent behavior in real-world applications like data querying. The evaluation used GPT-4.1 mini and nano models for testing, and identified that the schema listing lacked column names, leading to column-name guessing and error-retry loops. The fix involves either including column names in the prompt or softening the advice against calling describe_table.

rss · Simon Willison · Jul 2, 18:25

**Background**: DSPy is a framework from Stanford NLP that emphasizes programming language models rather than prompting them, allowing for modular and optimizable AI systems. Datasette Agent is an AI assistant for Datasette, a tool for exploring and publishing SQLite databases; it can generate and execute read-only SQL queries to answer user questions.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp / dspy : DSPy : The framework for...</a></li>
<li><a href="https://simonw.substack.com/p/datasette-agent-an-ai-assistant-for">Datasette Agent: an AI assistant for Datasette built on LLM</a></li>

</ul>
</details>

**Tags**: `#DSPy`, `#Datasette`, `#prompt engineering`, `#AI agents`, `#SQL`

---

<a id="item-9"></a>
## [Understand to Participate: Deep Code Understanding for AI Collaboration](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 7.0/10

Geoffrey Litt introduced the concept of 'understand to participate' at the AI Engineer World's Fair 2026, arguing that developers must deeply understand AI agent code changes to maintain creative participation and avoid cognitive debt. As AI coding agents produce larger and more complex code changes, developers risk accumulating cognitive debt if they do not keep up with understanding. This concept provides a framework for staying engaged and creative, which is crucial for maintaining code quality and developer agency. Litt's approach emphasizes building a rich mental model of code changes before diving into details, and using AI tools to efficiently catch up on understanding. He argues that without deep understanding, developers become limited in their ability to think creatively about the project.

rss · Simon Willison · Jul 2, 17:07

**Background**: Cognitive debt refers to the accumulation of mental overhead when developers rely on AI without fully understanding the code, similar to technical debt but in the developer's mind. As AI agents become more capable, there is a growing need for methods to help humans stay in the loop and maintain comprehension.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck.html">Understanding is the new bottleneck</a></li>
<li><a href="https://twitter.com/geoffreylitt/status/2072522251300409556">Geoffrey Litt on X: "Hot take: I think it's still important to understand the code that our agents write! In this mega thread (based on my AIE talk today), I will explain why that's the case, and show some ideas for how to efficiently understand code. Alright, let's dive in. 1/ https://t.co/765DNZh6LN" / X</a></li>
<li><a href="https://www.linkedin.com/pulse/cognitive-debt-when-ai-becomes-our-google-maps-k-subramanian-vnguc">Cognitive Debt : When AI Becomes Our Google Maps for Software...</a></li>

</ul>
</details>

**Tags**: `#AI-assisted coding`, `#cognitive debt`, `#software engineering`, `#developer experience`

---

<a id="item-10"></a>
## [Factories Are Just Rooms](https://interconnected.org/home/2026/07/03/factories) ⭐️ 6.0/10

An essay argues that factories are fundamentally just rooms, challenging the perception of manufacturing as complex and capital-intensive. The author uses this perspective to advocate for a simpler, more accessible view of production. This reframing encourages entrepreneurs and hobbyists to reconsider barriers to entry in manufacturing, potentially fostering more small-scale, local production. It highlights that the simplicity of the concept can democratize making. The essay is reflective rather than technical, with high community engagement (73 comments) sharing personal experiences in small factories and manufacturing. The discussion adds depth to the core argument, revealing both opportunities and challenges.

hackernews · arbesman · Jul 3, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48776035)

**Background**: Factories are often perceived as large, automated facilities requiring significant capital investment. The essay posits that at their core, factories are merely rooms where things are made, emphasizing that the key ingredients are people and processes, not expensive machinery. This perspective aligns with movements like DIY culture and small-batch manufacturing.

**Discussion**: Commenters share personal anecdotes about running small factories, the value of hands-on work, and comparisons to fast-food kitchens as efficient factories. There is appreciation for the simplicity of manufacturing, but also recognition of challenges like business consistency and the need for process improvement.

**Tags**: `#manufacturing`, `#mindset`, `#small business`, `#making things`

---

<a id="item-11"></a>
## [Simon Willison's June Newsletter: AI Models and Tool Updates](https://simonwillison.net/2026/Jul/3/june-newsletter/#atom-everything) ⭐️ 6.0/10

Simon Willison released his June 2026 sponsors-only newsletter covering new AI models including Claude Fable 5, GPT-5.6, and GLM-5.2, as well as US export restrictions and updates to Datasette and related tools. This newsletter provides a curated overview of the latest developments in AI and developer tools, helping readers stay informed about rapidly evolving technologies. The spotlight on Claude Fable 5 and GLM-5.2 reflects the ongoing competition between proprietary and open-weight models. Claude Fable 5, released by Anthropic on June 9, 2026, is described as state-of-the-art for coding and autonomous tasks, while GLM-5.2 from Z.AI has become the leading open weights model on the Artificial Analysis Intelligence Index. Tokenmaxxing, a trend of maximizing AI token usage, is declared over, shifting toward valuemaxxing.

rss · Simon Willison · Jul 3, 14:50

**Background**: Simon Willison is a well-known developer and creator of Datasette, an open-source tool for exploring and publishing data. His monthly newsletter, available to sponsors, aggregates notable news in AI, LLMs, and developer tools. Tokenmaxxing refers to the practice of maximizing AI token usage, often associated with coding agents like Claude Code.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://artificialanalysis.ai/articles/glm-5-2-is-the-new-leading-open-weights-model-on-the-artificial-analysis-intelligence-index">GLM-5.2 is the new leading open weights model on the Artificial Analysis Intelligence Index</a></li>
<li><a href="https://www.forbes.com/sites/timkeary/2026/06/02/why-tokenmaxxing-is-out-and-valuemaxxing-is-in/">Why ‘Tokenmaxxing’ Is Out And ‘Valuemaxxing’ Is In</a></li>

</ul>
</details>

**Tags**: `#newsletter`, `#AI`, `#LLM`, `#datasette`, `#tools`

---

<a id="item-12"></a>
## [Simon Willison Releases llm-coding-agent 0.1a0 Alpha](https://simonwillison.net/2026/Jul/2/llm-coding-agent/#atom-everything) ⭐️ 6.0/10

Simon Willison has released an early alpha version (0.1a0) of llm-coding-agent, a coding agent built on his LLM library. The agent includes tools for reading and editing files, executing commands, and searching code, and can be run via the command line or used as a Python API. This release demonstrates how the LLM library has evolved into an agent framework, enabling the creation of coding assistants similar to Claude Code. It showcases the potential for open-source, customizable coding agents that can be tailored to specific workflows. The agent was built using Claude Code for web, writing a spec and then implementing it via test-driven development with the help of Fable 5. It ships with tools like edit_file, execute_command, list_files, read_file, and search_files, and supports a `--yolo` flag for automatic approval of all actions.

rss · Simon Willison · Jul 2, 19:33

**Background**: Simon Willison's LLM library is a CLI tool and Python library for accessing many large language models. The library has recently undergone a major refactor (version 0.32a0) to become more of an agent framework. This coding agent is an experiment to see what a simple coding agent built on that framework would look like, following patterns from tools like Claude Code.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#coding agent`, `#Python`, `#Simon Willison`

---