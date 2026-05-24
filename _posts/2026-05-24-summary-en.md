---
layout: default
title: "Horizon Summary: 2026-05-24 (EN)"
date: 2026-05-24
lang: en
---

> From 29 items, 10 important content pieces were selected

---

1. [SpaceX Launches Starship v3 Rocket](#item-1) ⭐️ 9.0/10
2. [80386 Microcode Disassembled by Reverse Engineer](#item-2) ⭐️ 9.0/10
3. [US to Require Green Card Applicants to Leave Country](#item-3) ⭐️ 8.0/10
4. [C# introduces union types in .NET 11 preview](#item-4) ⭐️ 8.0/10
5. [Making deep learning go brrrr from first principles](#item-5) ⭐️ 8.0/10
6. [AI-Driven HBM Demand Causes Consumer Electronics Repricing](#item-6) ⭐️ 8.0/10
7. [Deep Dive into HTML <dl> Semantics and History](#item-7) ⭐️ 7.0/10
8. [Hengefinder: Web tool predicts sun-street alignments](#item-8) ⭐️ 7.0/10
9. [FTC Fines Cox Media Group $1M for Fake AI 'Active Listening'](#item-9) ⭐️ 7.0/10
10. [Building a Minimal Linux Writerdeck for Focused Writing](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [SpaceX Launches Starship v3 Rocket](https://www.space.com/space-exploration/launches-spacecraft/spacex-starship-v3-megarocket-first-test-flight) ⭐️ 9.0/10

SpaceX's Starship v3 rocket conducted its first test flight on May 2026, successfully launching but experiencing engine issues during booster return and ship landing. This test marks a major milestone in aerospace, demonstrating SpaceX's rapid iteration approach to developing a fully reusable super-heavy lift rocket, which is critical for future Moon and Mars missions. During the flight, one engine on the Super Heavy booster failed during ascent, and the boost-back burn failed, though a landing burn was attempted. The Starship upper stage lost one engine but still landed precisely on target.

hackernews · busymom0 · May 22, 23:41 · [Discussion](https://news.ycombinator.com/item?id=48242959)

**Background**: Starship v3 is the latest iteration of SpaceX's fully reusable rocket system, designed to carry over 100 metric tons to low Earth orbit. It stands 124 meters tall, making it the tallest rocket ever built. This test continues SpaceX's 'build, test, learn' philosophy, where failures are treated as data for rapid improvement.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starship">SpaceX Starship - Wikipedia</a></li>
<li><a href="https://arstechnica.com/space/2026/05/spacex-completes-fueling-test-setting-stage-for-first-launch-of-starship-v3/">Once again, SpaceX has set a new record for the tallest rocket ever built - Ars Technica</a></li>

</ul>
</details>

**Discussion**: The community praised the successful landing and improved heat shield performance, with one commenter noting no visible hot spots during reentry. However, disappointment was expressed over the booster's failure to return, reminiscent of a similar issue in a previous flight. Overall, sentiment supports the rapid iteration approach.

**Tags**: `#SpaceX`, `#Starship`, `#Rocket Launch`, `#Space Exploration`, `#Aerospace Engineering`

---

<a id="item-2"></a>
## [80386 Microcode Disassembled by Reverse Engineer](https://www.reenigne.org/blog/80386-microcode-disassembled/) ⭐️ 9.0/10

A detailed disassembly of the Intel 80386 CPU's microcode has been published, revealing the low-level control logic that interprets complex x86 instructions. This reverse engineering effort provides unprecedented insight into the inner workings of a classic 32-bit processor, aiding retrocomputing enthusiasts and open-source hardware projects seeking to replicate or understand the 80386. The disassembly was performed by reenigne, who also contributed to the ongoing z386 project that aims to build an open-source 80386 using the original microcode. The microcode is stored on-chip in a specialized ROM and implements complex instructions like string operations and protected mode transitions.

hackernews · nand2mario · May 23, 12:11 · [Discussion](https://news.ycombinator.com/item?id=48247004)

**Background**: Microcode is a low-level layer of control data that translates machine instructions into sequences of hardware operations. The 80386, released in 1985, was Intel's first 32-bit x86 processor and used microcode to handle complex instructions while keeping the hardware design simpler. Disassembling microcode requires careful analysis of the processor's die or, as in this case, studying the documented behavior to reconstruct the microcode program.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microcode">Microcode</a></li>

</ul>
</details>

**Discussion**: The Hacker News community reacted with fascination and respect, with comments praising the reverse engineering effort and linking to related projects like the open-source z386. Some users discussed the technical process of extracting microcode from die images, while others recommended further reading on microprogramming.

**Tags**: `#reverse engineering`, `#microcode`, `#80386`, `#CPU architecture`, `#retrocomputing`

---

<a id="item-3"></a>
## [US to Require Green Card Applicants to Leave Country](https://www.nytimes.com/2026/05/22/us/politics/green-card-changes-trump.html) ⭐️ 8.0/10

The Trump administration announced on May 22, 2026, that most green card applicants must leave the United States to apply, reversing the long-standing adjustment of status process. This policy change could severely disrupt the lives and careers of hundreds of thousands of legal immigrants, particularly H-1B visa holders in the tech industry, who previously could adjust status without leaving the US. The policy takes immediate effect and only allows adjustment of status in extraordinary circumstances. Applicants must now go through consular processing abroad, which can involve long wait times and risks for families with US-born children.

hackernews · tlhunter · May 22, 21:27 · [Discussion](https://news.ycombinator.com/item?id=48241890)

**Background**: Adjustment of status is a process that allows immigrants already in the US on temporary visas to apply for permanent residence without returning to their home country. For decades, this has been the primary path for skilled workers on H-1B visas to get green cards. The new rule eliminates this option for most applicants.

<details><summary>References</summary>
<ul>
<li><a href="https://www.uscis.gov/green-card/green-card-processes-and-procedures/adjustment-of-status">Adjustment of Status - USCIS</a></li>
<li><a href="https://www.usa.gov/adjustment-of-status">Adjustment of status: Get a Green Card if you are in the ... - USAGov</a></li>

</ul>
</details>

**Discussion**: Commenters express widespread shock and outrage, describing the policy as reckless and devastating for families and tech workers. Many share personal experiences and highlight the impracticality of leaving the US, especially for families with American children and lengthy consular backlogs.

**Tags**: `#immigration`, `#policy`, `#tech workforce`, `#H1B`, `#green card`

---

<a id="item-4"></a>
## [C# introduces union types in .NET 11 preview](https://andrewlock.net/exploring-the-dotnet-11-preview-2-dotnet-gets-union-types/) ⭐️ 8.0/10

The .NET 11 preview introduces union types to C#, a long-awaited feature that allows values from a closed set of types with exhaustive pattern matching support. Union types enhance type safety and expressiveness in C#, enabling developers to model state more precisely and reduce runtime errors. This feature brings C# closer to languages like F# that have long had unions, and it will benefit millions of .NET developers. The implementation separates union types from union declarations, allowing succinct syntax with opinionated semantics while enabling existing types to opt into union behavior. The feature is still in preview and syntax may change based on feedback.

hackernews · ingve · May 22, 12:28 · [Discussion](https://news.ycombinator.com/item?id=48234954)

**Background**: Union types, also known as discriminated unions, allow a variable to hold one of several specified types. In C#, they have been a highly requested feature for years, with F# having them for decades. The new proposal builds on pattern matching and provides exhaustive checking, meaning the compiler ensures all cases are handled.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/union">Union types - C# reference | Microsoft Learn</a></li>
<li><a href="https://github.com/dotnet/csharplang/blob/main/proposals/unions.md">csharplang/proposals/unions.md at main · dotnet/csharplang</a></li>

</ul>
</details>

**Discussion**: The community reaction is positive, with developers expressing long-time anticipation. Some note that F# has had unions for decades, and C# is gradually incorporating these features. Others appreciate the effort and see it as enabling better interop with other languages, not just for use within C#.

**Tags**: `#C#`, `#.NET`, `#union types`, `#programming languages`, `#type systems`

---

<a id="item-5"></a>
## [Making deep learning go brrrr from first principles](https://horace.io/brrr_intro.html) ⭐️ 8.0/10

A comprehensive guide published in 2022 explains how to optimize deep learning performance from first principles, covering modern hardware like NVIDIA GPUs. This guide helps deep learning practitioners write efficient code by understanding fundamental performance bottlenecks, and it highlights NVIDIA's continued dominance in GPU computing. The article covers FLOPs, memory bandwidth, and kernel launch overhead, demonstrating that an A100 can process 9.75 million FLOPS in the time Python performs a single FLOP.

hackernews · tosh · May 23, 11:50 · [Discussion](https://news.ycombinator.com/item?id=48246889)

**Background**: Deep learning models require massive computation, making GPU acceleration critical. Modern GPUs like NVIDIA's A100 have hierarchical memory and parallel execution units, and optimizing performance requires understanding these hardware details and the CUDA programming model.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CUDA">CUDA - Wikipedia</a></li>
<li><a href="https://www.digitalocean.com/community/tutorials/the-hidden-bottleneck-how-gpu-memory-hierarchy-affects-your-computing-experience">The Hidden Bottleneck: How GPU Memory Hierarchy ... | DigitalOcean</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article as a classic, noting that NVIDIA's lead in TFLOPs and bandwidth shows remarkable competitive momentum. Some raised concerns about portability across runtimes and the need for graceful degradation in production systems, while others highlighted the stark performance gap between Python and GPU compute.

**Tags**: `#deep learning`, `#performance optimization`, `#NVIDIA`, `#ML systems`, `#GPU computing`

---

<a id="item-6"></a>
## [AI-Driven HBM Demand Causes Consumer Electronics Repricing](https://simonwillison.net/2026/May/22/memory-shortage/#atom-everything) ⭐️ 8.0/10

Memory manufacturers are reallocating wafer capacity from consumer memory (DDR, LPDDR) to high-bandwidth memory (HBM) for AI data centers, with HBM's share expected to rise from 2% to 20% by end of 2026, causing price increases for consumer electronics like smartphones. This structural shift will make budget smartphones and other consumer devices significantly more expensive, particularly affecting emerging markets in Africa and South Asia where sub-$100 phones are critical, and signals a lasting change in semiconductor economics driven by AI. HBM consumes over three times the wafer capacity per gigabyte compared to DDR or LPDDR, and memory manufacturers intentionally under-provision fab capacity to maintain profit margins, exacerbating the shortage for consumer memory types.

rss · Simon Willison · May 22, 22:01

**Background**: Memory manufacturers (only three major players remain) have fixed wafer capacity that must be split among DDR (used in desktops and servers), LPDDR (mobile and low-power devices), and HBM (used with GPUs). HBM is a 3D-stacked memory architecture that provides extremely high bandwidth for AI workloads but uses significantly more wafer area per gigabyte. The AI boom has dramatically increased HBM demand, forcing manufacturers to prioritize it over consumer memory, leading to price hikes for electronics.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HBM_memory_shortage">HBM memory shortage</a></li>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.rambus.com/blogs/hbm3-everything-you-need-to-know/">High Bandwidth Memory (HBM): Everything You Need to Know - Rambus</a></li>

</ul>
</details>

**Tags**: `#memory shortage`, `#AI hardware`, `#consumer electronics`, `#HBM`, `#semiconductor industry`

---

<a id="item-7"></a>
## [Deep Dive into HTML <dl> Semantics and History](https://benmyers.dev/blog/on-the-dl/) ⭐️ 7.0/10

Ben Myers published a technical blog post titled 'On The <dl>' that thoroughly examines the semantics, history, and proper usage of the HTML <dl> element, challenging common misconceptions. The post includes detailed examples and corrections, such as detailing the evolution from a simple definition list to a general association list in HTML5. This analysis is significant for web developers and accessibility advocates because correct usage of <dl> improves semantic structure and accessibility. The post clarifies confusion around <dl>'s role and ARIA compatibility, helping developers make informed markup decisions. The article notes that prior to HTML5, <dl> was called a definition list, but HTML5 expanded its purpose to represent any list of key-value pairs. It also discusses ARIA role restrictions, noting that <dl> lacks an implicit role and can only take specific explicit roles like 'group' or 'list'.

hackernews · ravenical · May 23, 13:03 · [Discussion](https://news.ycombinator.com/item?id=48247325)

**Background**: The <dl> element originated from early markup languages like IBM's GML, where it was used for definition lists. In HTML, it was initially intended solely for glossaries of terms and definitions. HTML5 redefined it to accommodate any group of term-description pairs, but many developers still misuse it for layout or styling purposes, leading to accessibility issues.

**Discussion**: A commenter named chrismorgan pointed out an accessibility error in the blog post regarding the use of aria-label on <dl>, citing W3C rules. Another user, kqp, expressed frustration with semantic HTML, stating that <dl> often lacks flexibility for complex designs, leading to regrets in usage. The discussion overall was lively, with corrections and debates on proper semantics.

**Tags**: `#HTML`, `#semantics`, `#web development`, `#accessibility`, `#history`

---

<a id="item-8"></a>
## [Hengefinder: Web tool predicts sun-street alignments](https://victoriaritvo.com/blog/hengefinder/) ⭐️ 7.0/10

Hengefinder is a new web tool that calculates exactly when the sun will align with any street worldwide, similar to Manhattanhenge events. This tool makes it easy for photographers and urban planners to plan around solar alignments, democratizing a previously niche calculation. The tool uses precise astronomical calculations combined with real road data to predict alignments down to the minute, and works internationally.

hackernews · evakhoury · May 22, 20:39 · [Discussion](https://news.ycombinator.com/item?id=48241335)

**Background**: A 'henge' refers to an event like Manhattanhenge, where the sun sets perfectly aligned with the street grid. Such events occur twice a year in New York City and are popular for photography. Hengefinder generalizes this concept to any street worldwide using map data and solar position algorithms.

<details><summary>References</summary>
<ul>
<li><a href="https://hengefinder.rcdis.co/">Hengefinder</a></li>
<li><a href="https://play.google.com/store/apps/details?id=com.hengefinderllc.hengefinder&hl=en-US">Hengefinder - Apps on Google Play</a></li>

</ul>
</details>

**Discussion**: Comments expressed interest in an inverse tool for shading, requested mobile access, compared to existing apps like The Photographer's Ephemeris, and suggested features like .ics calendar downloads.

**Tags**: `#solar alignment`, `#web tool`, `#urban planning`, `#photography`, `#Hacker News discussion`

---

<a id="item-9"></a>
## [FTC Fines Cox Media Group $1M for Fake AI 'Active Listening'](https://simonwillison.net/2026/May/22/ftc-active-listening/#atom-everything) ⭐️ 7.0/10

The FTC ordered Cox Media Group, MindSift, and 1010 Digital Works to pay nearly $1 million to settle charges that they falsely marketed an AI-powered 'Active Listening' service that claimed to eavesdrop on consumers' conversations through smart devices to target ads. This case marks a significant regulatory action against deceptive AI marketing claims, reinforcing that companies cannot exaggerate the capabilities of AI-powered surveillance technologies without facing consequences. The 'Active Listening' service did not actually listen to conversations or use voice data; instead, it simply resold email lists from other data brokers at a markup. The FTC also stated that burying an opt-in within terms of service does not constitute adequate consent for such invasive data collection.

rss · Simon Willison · May 22, 04:48

**Background**: The 'Active Listening' service was marketed as an AI-powered tool that could capture real-time intent data by listening to conversations via smart devices, fueling long-standing conspiracy theories that phones are constantly eavesdropping for ad targeting. The FTC's investigation found these claims were baseless, as no such listening or voice data collection occurred.

<details><summary>References</summary>
<ul>
<li><a href="https://thecyberexpress.com/ftc-ai-powered-active-listening-case/">AI-Powered Marketing Service “Active Listening” Deceived Customers: FTC - The Cyber Express</a></li>

</ul>
</details>

**Discussion**: Simon Willison, who previously covered this story, expressed relief that the FTC's findings confirm his theory that the 'active listening' claim was a marketing exaggeration rather than a real eavesdropping capability. He sees this as useful ammunition against the persistent conspiracy theory that phones spy on users via microphones.

**Tags**: `#AI ethics`, `#privacy`, `#regulation`, `#FTC`, `#marketing`

---

<a id="item-10"></a>
## [Building a Minimal Linux Writerdeck for Focused Writing](https://veronicaexplains.net/my-first-writerdeck/) ⭐️ 6.0/10

The author details how she built a custom Linux-based writerdeck — a minimal, distraction-free writing machine — using an old laptop, a lightweight Linux distribution, and a plain-text editor. This project highlights the growing desire among knowledge workers to reclaim focus from constant digital distractions, though the effort required to build such a device may paradoxically become another form of distraction. The writerdeck uses a tiling window manager, no network connectivity, and a minimal text editor like Vim or Emacs, stripping away all non-essential features to create a pure writing environment.

hackernews · hggh · May 23, 18:45 · [Discussion](https://news.ycombinator.com/item?id=48250144)

**Background**: A writerdeck is a dedicated device for writing—like a modern digital typewriter—intended to eliminate the distractions of web browsers, notifications, and multitasking. This concept is inspired by commercial products like the Astrohaus Freewrite and the Alphasmart Neo, as well as DIY projects.

<details><summary>References</summary>
<ul>
<li><a href="https://www.writerdeck.org/">writerDeck.org</a></li>
<li><a href="https://www.reddit.com/r/writerDeck/wiki/index/">writerDeck - Reddit</a></li>
<li><a href="https://www.makeuseof.com/tag/get-distraction-free-computer-10-easy-steps/">How to Get a Distraction-Free Computer in 10 Easy Steps</a></li>

</ul>
</details>

**Discussion**: Commenters noted the irony of spending hours tinkering to build a focus machine, with some comparing the behavior to ADHD hyperfocus on the wrong task. Others suggested simpler alternatives like using Linux virtual consoles (Ctrl+Alt+F3) to achieve a similar distraction-free environment, and one commenter questioned whether such individual solutions address broader societal issues.

**Tags**: `#distraction-free computing`, `#Linux`, `#minimalism`, `#productivity`, `#writerdeck`

---