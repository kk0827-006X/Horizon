---
layout: default
title: "Horizon Summary: 2026-06-19 (EN)"
date: 2026-06-19
lang: en
---

> From 50 items, 14 important content pieces were selected

---

1. [Researcher discovers 10,000 GitHub repos distributing trojan malware](#item-1) ⭐️ 9.0/10
2. [Noam Shazeer Joins OpenAI](#item-2) ⭐️ 9.0/10
3. [GLM-5.2: Most Powerful Open-weights LLM Released](#item-3) ⭐️ 9.0/10
4. [Hospitals and universities repurpose drugs at 90% lower cost](#item-4) ⭐️ 8.0/10
5. [Consumer advocate's forced consent challenge leads to €1.8M GDPR fine](#item-5) ⭐️ 8.0/10
6. [Swiss parliament lifts ban on new nuclear plants](#item-6) ⭐️ 8.0/10
7. [W Social: European digital sovereignty or political theater?](#item-7) ⭐️ 8.0/10
8. [Charity Majors: AI Makes Code Disposable](#item-8) ⭐️ 8.0/10
9. [Cornell's CS 6120 Advanced Compilers Course Goes Self-Guided Online](#item-9) ⭐️ 7.0/10
10. [Site Checks LLM Recognition of Your Online Presence](#item-10) ⭐️ 7.0/10
11. [Master Git ignoring: beyond .gitignore](#item-11) ⭐️ 7.0/10
12. [Datasette Apps Plugin Launches with Sandboxed SQL Access](#item-12) ⭐️ 7.0/10
13. [Ubiquiti Launches Enterprise NAS with ZFS](#item-13) ⭐️ 6.0/10
14. [Datasette ACL Plugin Expands to General Resource Sharing](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Researcher discovers 10,000 GitHub repos distributing trojan malware](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 9.0/10

A security researcher has identified approximately 10,000 GitHub repositories that are distributing Trojan malware, likely part of a coordinated supply chain attack targeting automated agents and developers. This discovery reveals a large-scale, automated attack on the open-source ecosystem that can infect countless downstream projects and users, highlighting a critical vulnerability in software supply chains. The malicious repositories are frequently updated with new commits to appear in search results and avoid detection; they are specifically designed to be picked up by automated dependency resolvers and AI coding assistants.

hackernews · theorchid · Jun 18, 11:45 · [Discussion](https://news.ycombinator.com/item?id=48583928)

**Background**: Trojan malware disguises itself as legitimate software to trick users into installing it. Supply chain attacks target the relationship between developers and their dependencies, injecting malicious code into trusted sources. GitHub, hosting millions of repositories, is a prime vector for such attacks.

**Discussion**: Community members confirm similar experiences, with some finding their names attached to unknown repositories. The discussion highlights that the attack is automated and targets AI agents and automated tools, not human users directly, and references past real-world incidents like a Disney engineer being compromised via a GitHub tool.

**Tags**: `#security`, `#malware`, `#github`, `#supply-chain-attack`, `#open-source`

---

<a id="item-2"></a>
## [Noam Shazeer Joins OpenAI](https://twitter.com/NoamShazeer/status/2067400851438932297) ⭐️ 9.0/10

Noam Shazeer, co-author of the seminal 'Attention Is All You Need' paper and former co-lead of Google's Gemini, has left Google to join OpenAI. This high-profile talent move underscores the intense competition for AI research leadership, as Shazeer's transformer expertise is foundational to modern language models. Shazeer originally left Google in 2021 to co-found Character.AI, then returned in 2024 via a licensing deal reportedly worth $2.7 billion before now departing again for OpenAI.

hackernews · lukasgross · Jun 18, 00:26 · [Discussion](https://news.ycombinator.com/item?id=48578913)

**Background**: The transformer architecture, introduced in the 2017 paper 'Attention Is All You Need' co-authored by Shazeer, revolutionized natural language processing by replacing recurrent layers with self-attention mechanisms. Shazeer was a long-time Google researcher before co-founding Character.AI, and after returning to Google he served as co-lead of the Gemini AI model project.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.google.dev/gemini-api/docs/models">Models - Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**Discussion**: Commenters note Shazeer's legendary status within Google's engineering history and provide additional context about his career moves from Character.AI back to Google and now to OpenAI, with some expressing surprise at the rapid departure after his recent return.

**Tags**: `#AI`, `#transformers`, `#openai`, `#google`, `#talent`

---

<a id="item-3"></a>
## [GLM-5.2: Most Powerful Open-weights LLM Released](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai released GLM-5.2, a 753B-parameter Mixture-of-Experts LLM with 40B active parameters, a 1M token context window, and an MIT license on June 16, 2026. It is the leading open-weights model on the Artificial Analysis Intelligence Index v4.1 with a score of 51. GLM-5.2 sets a new benchmark for open-weights LLMs, outperforming models like DeepSeek V4 Pro and Kimi K2.6, and ranks second on the Code Arena WebDev leaderboard behind only Claude Fable 5. This release significantly advances open-source AI, making cutting-edge capabilities accessible under a permissive license. GLM-5.2 is a text-only model with a 1.51TB total size, using an MoE architecture with 40B active parameters per token. It is notably token-hungry, consuming 43k output tokens per task, higher than its predecessor GLM-5.1 (26k) and rivals. The model is available via OpenRouter at $1.40/1M input and $4.40/1M output tokens.

rss · Simon Willison · Jun 17, 23:58

**Background**: GLM-5.2 is part of Z.ai's GLM-5 family, developed by Zhipu AI, a Chinese company spun out from Tsinghua University. It is optimized for coding and agentic tasks, with a large context window of 1M tokens suitable for ultra-long-horizon tasks. The Mixture-of-Experts (MoE) architecture allows the model to have a huge total parameter count while only activating a subset per token, improving efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/blog/glm-5-2">GLM - 5 . 2 : Features, Setup, Benchmarks, and Model ... | DataCamp</a></li>
<li><a href="https://www.verdent.ai/guides/what-is-glm-5-2">What Is GLM - 5 . 2 ? A Developer's Guide to Z.ai's Coding Model</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#open-source`, `#AI`, `#natural-language-processing`, `#transformer`

---

<a id="item-4"></a>
## [Hospitals and universities repurpose drugs at 90% lower cost](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

Hospitals and universities are repurposing existing drugs for new indications, achieving up to 90% cost reduction compared to branded alternatives. This approach can significantly lower healthcare costs and improve access to treatments for diseases like macular degeneration and rare disorders, challenging the current pharmaceutical pricing model. A notable example is Avastin (bevacizumab) repurposed for macular degeneration at $50/dose versus Lucentis at $1,500/dose. However, off-label use lacks regulatory pathways without manufacturer consent or becoming a manufacturer.

hackernews · giuliomagnifico · Jun 18, 10:33 · [Discussion](https://news.ycombinator.com/item?id=48583386)

**Background**: Drug repurposing involves using an approved drug for a new medical indication, often at a fraction of the cost. This is common in ophthalmology and psychiatry, but regulatory and financial barriers hinder widespread adoption.

**Discussion**: Comments highlight real-world examples such as Avastin for macular degeneration and Spravato (esketamine) versus ketamine. Users note that Spravato is a patented modification of ketamine, though less effective, and criticize the broken incentives. One commenter mentions Cures Within Reach, a nonprofit funding repurposed drug studies.

**Tags**: `#drug repurposing`, `#healthcare costs`, `#pharmaceuticals`, `#macular degeneration`, `#ketamine`

---

<a id="item-5"></a>
## [Consumer advocate's forced consent challenge leads to €1.8M GDPR fine](https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/) ⭐️ 8.0/10

A Norwegian consumer advocate persisted in challenging Elkjop's forced consent practice in its customer club, resulting in a €1.8 million GDPR fine five years later. This case demonstrates that individuals can enforce GDPR rights against large corporations, and it sets a precedent that forced consent for marketing in loyalty programs is unlawful. The fine was issued by the Norwegian Data Protection Authority (Datatilsynet) after the advocate refused to consent and documented the violation. The company admitted that membership was required to receive marketing offers.

hackernews · speckx · Jun 18, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48589501)

**Background**: The General Data Protection Regulation (GDPR) requires that consent for data processing must be freely given, specific, informed, and unambiguous. Forced consent — making a service conditional on consent to unnecessary processing — violates Article 7(4) GDPR. Customer loyalty programs often collect personal data, but they must obtain valid consent without bundling.

<details><summary>References</summary>
<ul>
<li><a href="https://gdpr.eu/what-is-gdpr/">What is GDPR , the EU’s new data protection law? - GDPR .eu</a></li>
<li><a href="https://gdpr-info.eu/">General Data Protection Regulation ( GDPR ) – Legal Text</a></li>
<li><a href="https://martech.org/gdpr-day-1-google-and-facebook-sued-for-forced-consent/">GDPR day 1: Google and Facebook sued for ' forced consent '</a></li>

</ul>
</details>

**Discussion**: Community members praised the advocate's persistence, with some noting that similar pushback is rare, especially in the US. Others linked to the official decision and machine translation, providing technical resources. One commenter humorously observed the irony of suing the entity that won the case for him.

**Tags**: `#privacy`, `#GDPR`, `#consent`, `#regulation`, `#consumer rights`

---

<a id="item-6"></a>
## [Swiss parliament lifts ban on new nuclear plants](https://www.bluewin.ch/en/news/switzerland/parliament-lifts-ban-on-new-nuclear-power-plants-3257535.html) ⭐️ 8.0/10

The Swiss parliament voted to lift a ban on constructing new nuclear power plants, though the decision still requires approval in a public referendum before taking effect. This policy shift could significantly alter Switzerland's energy strategy, reigniting debates on energy security, safety, and the role of nuclear power in a clean energy future. The ban was originally introduced after the Fukushima disaster in 2011; the new decision must survive a likely referendum, with left-leaning and green parties strongly opposed.

hackernews · leonidasrup · Jun 18, 14:17 · [Discussion](https://news.ycombinator.com/item?id=48585746)

**Background**: Switzerland currently operates four nuclear reactors that provide about one-third of its electricity. The 2011 Fukushima accident led to a phase-out decision, banning new plants. Recent energy security concerns and climate goals have revived interest in nuclear power as a low-carbon source.

**Discussion**: Community comments reflect a polarized debate: some argue nuclear is safe and provides energy security, while others highlight cost, waste, and reliance on imported fuel. There is skepticism that new plants would be built in time and hope that renewables and hydro storage could fill the gap.

**Tags**: `#nuclear energy`, `#energy policy`, `#Switzerland`, `#clean energy`, `#energy security`

---

<a id="item-7"></a>
## [W Social: European digital sovereignty or political theater?](https://blog.elenarossini.com/w-social-public-institutions-and-the-theater-of-european-digital-sovereignty/) ⭐️ 8.0/10

A critical blog post by Elena Rossini examines W Social, a European social network branded as a digital sovereignty initiative, questioning its transparency and suggesting it is more about political theater than genuine open-source community building. This analysis raises important questions about the authenticity of European digital sovereignty projects and whether they truly serve public interest or are merely performative moves by politicians. The post highlights that W Social is closed-source, operates as an LLC with profit motives, and attracted high-profile EU politicians immediately, while an open-source alternative called Eurosky exists but received no media attention.

hackernews · nemoniac · Jun 18, 12:46 · [Discussion](https://news.ycombinator.com/item?id=48584497)

**Background**: European digital sovereignty refers to the EU's push to reduce dependence on non-European tech platforms. W Social was launched as a homegrown alternative to platforms like X, but its closed-source nature and corporate structure contrast with the open ideals often associated with digital sovereignty projects like the AT Protocol-based Eurosky.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bangkokpost.com/world/3272749/w-marks-the-xspot-european-social-network-takes-on-musk">W marks the X-spot: European social network takes on Musk</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism, comparing W Social to Truth Social and noting its corporate structure and lack of transparency. Some pointed out the existence of a transparent, open-source alternative (Eurosky) that was ignored by the press, while others highlighted the quick onboarding of EU politicians as a red flag.

**Tags**: `#digital sovereignty`, `#social media`, `#EU politics`, `#closed-source`, `#community critique`

---

<a id="item-8"></a>
## [Charity Majors: AI Makes Code Disposable](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors, a respected engineer, argues that the economics of code production have been fundamentally changed by AI, making code generation effectively free and instant, turning code from a treasured asset into a disposable commodity. This shift has profound implications for software engineering practices, project management, and the value of code itself. Developers may need to rethink how they design, maintain, and invest in codebases. Majors specifically notes that this change happened 'practically overnight' in 2025. She emphasizes that while code production is cheap, engineering discipline becomes more important, not less.

rss · Simon Willison · Jun 17, 17:12

**Background**: Traditionally, writing code is labor-intensive and time-consuming, so developers treat code as a valuable asset to be reused and carefully maintained. With AI-assisted programming tools like large language models (LLMs), generating code has become trivial, challenging this long-held assumption.

**Tags**: `#ai-assisted-programming`, `#generative-ai`, `#software-engineering`, `#economics-of-code`, `#charity-majors`

---

<a id="item-9"></a>
## [Cornell's CS 6120 Advanced Compilers Course Goes Self-Guided Online](https://www.cs.cornell.edu/courses/cs6120/2025fa/self-guided/) ⭐️ 7.0/10

Cornell University's advanced compilers course CS 6120 is now available as a self-guided online course with all materials, including lectures, notes, and assignments, freely accessible for self-study. This makes a high-quality, advanced compiler education accessible to anyone, helping to train the next generation of compiler engineers and researchers. The course covers fundamental concepts like SSA form and dynamic compilation, which are core to modern compiler design. The course covers topics such as dead code elimination, data flow analysis, dominator analysis, and SSA form, with a section on dynamic compilers that focuses on trace compilation. Community feedback notes that trace compilation is considered a dead end, and that the material might be more suitable for a first compilers course rather than an advanced one.

hackernews · ibobev · Jun 18, 11:04 · [Discussion](https://news.ycombinator.com/item?id=48583606)

**Background**: Static single assignment (SSA) form is an intermediate representation used in optimizing compilers where each variable is assigned exactly once, enabling efficient data-flow analysis. Dynamic compilation, including just-in-time compilation, optimizes code at runtime based on execution profiles, often used in modern programming language runtimes like Java's HotSpot.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Static_single-assignment_form">Static single-assignment form - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dynamic_compilation">Dynamic compilation</a></li>

</ul>
</details>

**Discussion**: Users like 'titzer' criticized the focus on trace compilation as a dead end, suggesting better coverage of type feedback, speculation, and deoptimization. 'j2kun' questioned the course's advanced label, noting that many topics are typical of a first compiler course. Despite these critiques, the overall sentiment was appreciative of the free resource.

**Tags**: `#compilers`, `#online-course`, `#academic`, `#systems`

---

<a id="item-10"></a>
## [Site Checks LLM Recognition of Your Online Presence](https://www.intheweights.com/) ⭐️ 7.0/10

A new website, intheweights.com, queries multiple LLMs in parallel to determine how strongly they recognize a person based on their online presence, scoring recognition and clustering responses. As traffic shifts from the web to LLMs, this tool reveals the extent to which individuals' digital footprints are encoded in model weights, raising privacy and awareness issues. The site queries frontier and small models, clusters responses for consistency, and attributes hallucinations when only a single model gives a plausible but likely incorrect answer.

hackernews · turtlesoup · Jun 18, 20:49 · [Discussion](https://news.ycombinator.com/item?id=48591348)

**Background**: LLM 'weights' are the learned parameters that store knowledge acquired during training. Tools like this probe whether a person's online data (e.g., Reddit history) is embedded in these weights, effectively making the person 'in the weights.'

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@tahirbalarabe2/llm-weights-context-and-memory-explained-simply-03685b6789c0">LLM Weights Context and Memory Explained Simply - Medium</a></li>
<li><a href="https://arxiv.org/pdf/2605.17110">Capturing LLM Capabilities via Evidence-Calibrated Query ...</a></li>

</ul>
</details>

**Discussion**: Users reported mixed results: some were correctly recognized, while others were hallucinations. One user noted non-determinism and score inflation with more keywords; another questioned privacy concerns.

**Tags**: `#LLM`, `#privacy`, `#training data`, `#recognition`, `#community discussion`

---

<a id="item-11"></a>
## [Master Git ignoring: beyond .gitignore](https://nelson.cloud/.gitignore-isnt-the-only-way-to-ignore-files-in-git/) ⭐️ 7.0/10

This article explains alternative Git ignore mechanisms such as .git/info/exclude and global .gitignore files, which are less known but powerful ways to ignore files in a Git repository. Understanding these alternatives helps developers keep their .gitignore files clean and project-specific, avoid committing unwanted files like IDE artifacts, and collaborate more effectively by using global excludes for personal workflows. The .git/info/exclude file is per-repository but not committed, ideal for local-only ignore rules. The global .gitignore (configured via core.excludesfile) applies to all repos on a machine, perfect for OS or editor-specific files. Additionally, .gitattributes can ignore diffs for certain files without preventing tracking.

hackernews · FergusArgyll · Jun 18, 10:29 · [Discussion](https://news.ycombinator.com/item?id=48583356)

**Background**: Git provides multiple ways to ignore files from being tracked. The most common is the .gitignore file, which is version-controlled and shared with the team. However, there are also local and global mechanisms: .git/info/exclude for repository-specific personal ignores, and a global .gitignore file configured via git config core.excludesfile. These are useful for ignoring files that should never be committed, like operating system or editor temporary files.

<details><summary>References</summary>
<ul>
<li><a href="https://git-scm.com/docs/gitignore">Git - gitignore Documentation</a></li>
<li><a href="https://docs.github.com/en/get-started/git-basics/ignoring-files">Ignoring files - GitHub Docs</a></li>
<li><a href="https://stackoverflow.com/questions/7335420/can-i-use-a-global-user-profile-scope-gitignore-file">Can I use a global (user-profile-scope) .gitignore file? Usage example</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article and added more insights. One highlighted .gitattributes for ignoring diffs on noisy files like package-lock.json. Another emphasized that global exclusion prevents cluttering project .gitignore with IDE/OS files. A user noted that ~/.config/git/ignore is a proper location for global Git config files. The overall sentiment is positive, with appreciation for uncovering lesser-known Git features.

**Tags**: `#git`, `#.gitignore`, `#version control`, `#best practices`

---

<a id="item-12"></a>
## [Datasette Apps Plugin Launches with Sandboxed SQL Access](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 7.0/10

The datasette-apps plugin was launched, allowing users to embed custom HTML+JavaScript applications inside Datasette that run in a sandboxed iframe and execute read-only SQL queries, with optional write access via stored queries. This plugin transforms Datasette from a data exploration tool into a platform for building and hosting interactive data-driven web applications, enabling secure third-party app embedding without compromising data privacy. Apps run in an iframe with sandbox="allow-scripts allow-forms" and a CSP header that blocks outgoing HTTP requests, preventing data exfiltration; write queries are allowed only if stored queries are configured with appropriate permissions.

rss · Simon Willison · Jun 18, 23:58

**Background**: Datasette is an open-source tool for exploring and publishing data as interactive websites and APIs, built on SQLite. It provides a JSON API for custom frontends. The datasette-apps plugin extends this by offering a secure sandbox for arbitrary HTML and JavaScript applications, inspired by Claude Artifacts and the author's earlier vibe-coded tools.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/datasette: An open source multi-tool for ... The Datasette Ecosystem Introduction to Datasette, a Frontend to Tabulated Data datasette · PyPI Datasette Reviews, Pricing & Alternatives (2026) | Toolradar Datasette - skills.network</a></li>
<li><a href="https://www.w3schools.com/tags/att_iframe_sandbox.asp">HTML iframe sandbox Attribute</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#plugin`, `#web app`, `#SQL`, `#data visualization`

---

<a id="item-13"></a>
## [Ubiquiti Launches Enterprise NAS with ZFS](https://blog.ui.com/article/introducing-enterprise-nas) ⭐️ 6.0/10

Ubiquiti announced the Enterprise NAS, a network-attached storage device built on the ZFS file system, featuring dual 25GbE SFP28 ports and redundant power supplies. This marks Ubiquiti's entry into the enterprise storage market, leveraging ZFS's advanced data integrity and snapshot features. However, community skepticism about Ubiquiti's software reliability and security history may dampen adoption. The NAS uses ZFS, which provides fault tolerance and efficient delta backups via its Merkle tree structure. It targets enterprises but faces questions about whether spinning disks can saturate the 25GbE links and concerns over past security incidents like leaked AWS keys and unauthorized camera feed access.

hackernews · ksec · Jun 18, 14:24 · [Discussion](https://news.ycombinator.com/item?id=48585866)

**Background**: ZFS is a combined file system and volume manager originally developed by Sun Microsystems, known for its data integrity, scalability, and advanced features like snapshots and replication. Ubiquiti is a networking hardware company that has faced criticism for software quality and security vulnerabilities in the past.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ZFS">ZFS - Wikipedia</a></li>
<li><a href="https://itsfoss.com/what-is-zfs/">What is ZFS ? Why are People Crazy About it?</a></li>

</ul>
</details>

**Discussion**: Comments show a mix of excitement about ZFS and skepticism toward Ubiquiti. Users highlight past security issues and software quality problems, with some calling the product 'test-it-in-prod.' Others appreciate no recurring fees but worry about long-term viability.

**Tags**: `#Ubiquiti`, `#NAS`, `#ZFS`, `#storage`, `#enterprise`

---

<a id="item-14"></a>
## [Datasette ACL Plugin Expands to General Resource Sharing](https://simonwillison.net/2026/Jun/18/datasette-acl/#atom-everything) ⭐️ 6.0/10

The datasette-acl plugin version 0.6a0 has been released, expanding from table-only permissions toward a general resource-sharing system for multi-user Datasette instances. This release paves the way for finer-grained access control within Datasette, enabling more flexible multi-user deployments and complex data sharing scenarios. The work was primarily done by Alex Garcia, and the plugin now supports managing permissions for resources beyond just tables, moving toward a comprehensive ACL system.

rss · Simon Willison · Jun 18, 19:03

**Background**: Datasette is an open-source tool for exploring and publishing data as interactive websites and APIs. The datasette-acl plugin adds advanced permission control, allowing administrators to grant or restrict access to specific data resources for different users.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/18/datasette-acl/">Release: datasette-acl 0.6a0 - simonwillison.net</a></li>
<li><a href="https://github.com/datasette/datasette-acl">GitHub - datasette/datasette-acl: Advanced permission ...</a></li>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#acl`, `#permissions`, `#plugin`

---