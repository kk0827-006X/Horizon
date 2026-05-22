---
layout: default
title: "Horizon Summary: 2026-05-22 (EN)"
date: 2026-05-22
lang: en
---

> From 59 items, 16 important content pieces were selected

---

1. [SpaceX S-1 Reveals Anthropic's $1.25B/Month Compute Deal](#item-1) ⭐️ 9.0/10
2. [Google Tests Gemini-Powered Ads in Search](#item-2) ⭐️ 8.0/10
3. [New Freenet Redesign Uses WebAssembly Contracts for Decentralized Apps](#item-3) ⭐️ 8.0/10
4. [Locally Index Year of Video on MacBook with Gemma4-31B](#item-4) ⭐️ 8.0/10
5. [Python 3.15's Underappreciated Features](#item-5) ⭐️ 8.0/10
6. [Project Hail Mary Star Chart Uses GAIA DR3 for 1.8 Billion Stars](#item-6) ⭐️ 7.0/10
7. [Blog migrated from Ubuntu 16.04 to FreeBSD after 10 years](#item-7) ⭐️ 7.0/10
8. [Seattle Police Intelligence Network with Private Partners](#item-8) ⭐️ 7.0/10
9. [Waymo Pauses Atlanta Service After Robotaxis Drive Into Floods](#item-9) ⭐️ 7.0/10
10. [Restored Trinity Test Photos Reveal New Atomic Details](#item-10) ⭐️ 7.0/10
11. [BBEdit 16 Released with One-Time Purchase Pricing](#item-11) ⭐️ 7.0/10
12. [Datasette Agent: AI assistant for conversational data querying](#item-12) ⭐️ 7.0/10
13. [Flipper One Announced: Community Help Sought](#item-13) ⭐️ 6.0/10
14. [How fast is 10 tokens per second really?](#item-14) ⭐️ 6.0/10
15. [Simon Willison's Cautious Take on Google I/O 2026](#item-15) ⭐️ 6.0/10
16. [Rocket Lab wins $90M Space Force satellite contract](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [SpaceX S-1 Reveals Anthropic's $1.25B/Month Compute Deal](https://simonwillison.net/2026/May/20/spacex-s1/#atom-everything) ⭐️ 9.0/10

SpaceX's S-1 filing with the SEC reveals that Anthropic has agreed to pay $1.25 billion per month through May 2029 for compute capacity on SpaceX's COLOSSUS and COLOSSUS II supercomputers. This is a groundbreaking financial commitment between two major AI players, signaling an unprecedented scale in AI infrastructure investment and highlighting the growing demand for massive compute resources for AI training and inference. The agreement includes a ramp-up period in May and June 2026 at a reduced fee, and either party may terminate with 90 days' notice. The COLOSSUS supercomputer, originally built by xAI in 2024, is the world's largest AI supercomputer and is used to train xAI's Grok models.

rss · Simon Willison · May 20, 22:26

**Background**: COLOSSUS is a supercomputer built in 2024 in Memphis, Tennessee, originally by xAI (Elon Musk's AI venture) for training the Grok chatbot. SpaceX acquired xAI earlier in 2026, gaining ownership of COLOSSUS and its successor COLOSSUS II. Anthropic is a leading AI research company known for developing the Claude series of models. This deal provides Anthropic with massive compute resources for AI training and inference, potentially including access to advanced hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Colossus_(supercomputer)">Colossus (supercomputer) - Wikipedia</a></li>
<li><a href="https://siliconangle.com/2026/05/06/anthropic-use-spacexs-colossus-1-supercomputer-inference/">Anthropic to use SpaceX’s Colossus 1 supercomputer for inference - SiliconANGLE</a></li>
<li><a href="https://www.forbes.com/sites/antoniopequenoiv/2026/05/06/musks-spacex-will-give-anthropic-access-to-its-colossus-super-computer-for-ai-training/">Musk’s SpaceX Will Give Anthropic Access To Its ‘Colossus’ Super Computer For AI Training</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cloud computing`, `#SpaceX`, `#Anthropic`, `#compute infrastructure`

---

<a id="item-2"></a>
## [Google Tests Gemini-Powered Ads in Search](https://blog.google/products/ads-commerce/google-marketing-live-search-ads/) ⭐️ 8.0/10

Google is testing new AI-powered ad formats in Search that use its Gemini model to generate personalized product explanations for advertisers, and expanding its Direct Offers pilot to surface targeted discounts in AI-driven shopping experiences. This marks a significant step in integrating generative AI into advertising, raising concerns about user manipulation and the erosion of organic search results. It could fundamentally change how businesses reach consumers and how users perceive search ads. The new ad format uses Gemini to pull up relevant products and write custom explainers for advertisers, while Direct Offers activates promotional deals from existing Shopping or Performance Max campaigns inside AI Mode. Both features are currently in testing or pilot phases.

hackernews · sofumel · May 21, 09:49 · [Discussion](https://news.ycombinator.com/item?id=48220105)

**Background**: Gemini is a family of multimodal large language models developed by Google DeepMind, succeeding LaMDA and PaLM 2. It powers various Google AI experiences. Direct Offers is a new pilot program that allows Google to surface promotional deals from advertisers directly within AI-powered shopping experiences, such as AI Mode in Search.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(AI_model)">Gemini (AI model)</a></li>
<li><a href="https://marketing4ecommerce.net/en/direct-offers-google/">What are Google Direct Offers - Marketing 4 Ecommerce</a></li>
<li><a href="https://adtechradar.com/2026/01/12/google-direct-offers-ai-shopping/">Google Brings Deal-Based Ads to AI Search With Direct Offers</a></li>

</ul>
</details>

**Discussion**: Community comments express strong concerns about the ethical implications of AI-generated ads, with some users calling the approach 'evil' and worrying about manipulation. Others indicate they will block Google bots or hope for a public alternative, reflecting deep distrust of AI in advertising.

**Tags**: `#AI`, `#advertising`, `#Google`, `#search`, `#ethics`

---

<a id="item-3"></a>
## [New Freenet Redesign Uses WebAssembly Contracts for Decentralized Apps](https://freenet.org/) ⭐️ 8.0/10

After 5 years of development, a ground-up redesign of Freenet has launched as a decentralized key-value store where keys are WebAssembly contracts that define state validity, mutation rules, and synchronization via commutative merge operations. Early applications include River (group chat) and Delta (CMS), with users already building games and a search engine called Atlas. This redesign revives a pioneering P2P project with a novel technical approach—using commutative merges for eventual consistency without consensus—and provides a platform for truly decentralized applications that can be downloaded and run in the browser. The merge operation in every contract must be commutative, allowing state updates to propagate like a virus and typically achieve global consistency in seconds. Users run a local peer and connect to it via WebSocket from browser-based single-page apps, avoiding centralized API servers.

hackernews · sanity · May 21, 14:34 · [Discussion](https://news.ycombinator.com/item?id=48223362)

**Background**: The original Freenet (now Hyphanet) was an early 2000s peer-to-peer anonymity network. The new Freenet reimagines it as a general-purpose decentralized key-value store inspired by CRDTs (Conflict-free Replicated Data Types), using WebAssembly contracts to enforce application logic and commutative merge operations for synchronization.

<details><summary>References</summary>
<ul>
<li><a href="https://freenet.org/build/manual/components/contracts/">Contracts | Freenet</a></li>
<li><a href="https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type">Conflict-free replicated data type - Wikipedia</a></li>
<li><a href="https://www.reddit.com/r/privacy/comments/1h84mtc/freenets_deltasync_efficient_scalable_data/">r/privacy on Reddit: Freenet's Delta-Sync: Efficient scalable data synchronization in a decentralized system</a></li>

</ul>
</details>

**Discussion**: Some commenters raised governance concerns about the project fork, alleging the board made a top-down decision to replace the original team. Others discussed technical aspects: one suggested syncing update logs for values without natural merge functions, another proposed burning crypto for ghost keys instead of donating to the foundation, and a developer expressed excitement about using WASM to define arbitrary consistency algorithms.

**Tags**: `#p2p`, `#decentralized`, `#webassembly`, `#key-value store`, `#freenet`

---

<a id="item-4"></a>
## [Locally Index Year of Video on MacBook with Gemma4-31B](https://blog.simbastack.com/indexed-a-year-of-video-locally/) ⭐️ 8.0/10

A developer successfully indexed a full year of personal video footage locally on a 2021 MacBook by running Google's Gemma4-31B model with 50 GB of swap memory, and released the code as open source under MIT license. This project shows that large language models can be used for practical personal archiving and video indexing on consumer hardware, not just in the cloud. It lowers the barrier for individuals to apply AI to their own media collections without relying on third-party services. The model ran at 4-bit quantization, theoretically requiring ~19 GB, but actual memory usage reached 28.4 GB, leading to heavy swap utilization that can accelerate SSD wear. The project also plans to integrate with DaVinci Resolve for faster video editing using the generated index.

hackernews · asenna · May 21, 14:01 · [Discussion](https://news.ycombinator.com/item?id=48222733)

**Background**: Gemma 4 is Google's family of open-weight LLMs. The 31B dense variant delivers frontier-level performance for coding and reasoning. Running such large models on devices with limited RAM (e.g., 16 GB) requires memory swapping to disk, which can be slow and cause wear, but tools like llama.cpp and quantization techniques make it feasible.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-31B">google/ gemma - 4 - 31 B · Hugging Face</a></li>
<li><a href="https://arxiv.org/html/2411.09317v1">Pie: Pooling CPU Memory for LLM Inference</a></li>
<li><a href="https://ryanagibson.com/posts/run-llms-larger-than-ram/">How to Run LLMs Larger than RAM · Ryan A. Gibson</a></li>

</ul>
</details>

**Discussion**: Commenters expressed interest in the code and raised concerns about SSD wear from heavy swapping. Some suggested that 4-bit quantization of Gemma4-31B should only require ~19 GB, questioning the necessity of 50 GB swap. Others shared similar experiences running Gemma on older hardware with upgraded memory.

**Tags**: `#local LLM`, `#video indexing`, `#AI on consumer hardware`, `#open source`, `#personal archive`

---

<a id="item-5"></a>
## [Python 3.15's Underappreciated Features](https://blog.changs.co.uk/python-315-features-that-didnt-make-the-headlines.html) ⭐️ 8.0/10

Python 3.15 introduces lazy imports via PEP 690, iterator synchronization primitives in the threading module, and improved set operations for collections.Counter (including symmetric difference). These features improve Python's performance (lazy imports reduce startup time), concurrency safety (iterator synchronization), and API completeness (Counter symmetric difference). They address long-standing pain points for developers. Lazy imports can be enabled globally with the -L flag or via importlib.set_lazy_imports(). Iterator synchronization provides a context manager to safely iterate over shared data. Counter now supports the XOR operator (^) for symmetric difference, complementing &, |, -.

hackernews · rbanffy · May 21, 11:10 · [Discussion](https://news.ycombinator.com/item?id=48220696)

**Background**: In Python, importing modules normally loads and executes them immediately, which can slow startup. Lazy imports defer this work until the module is actually used. Iterator synchronization is needed because Python iterators are not thread-safe by default; the new primitives help prevent race conditions. Counter is a dict subclass for counting hashable objects, and set operations like union, intersection, and difference were added in Python 3.10, while symmetric difference is new in 3.15.

<details><summary>References</summary>
<ul>
<li><a href="https://peps.python.org/pep-0690/">PEP 690 – Lazy Imports | peps. python .org</a></li>
<li><a href="https://docs.python.org/3.15/library/threading.html">threading — Thread-based parallelism — Python ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about lazy imports and iterator synchronization, with one noting it complements their threaded-generator package. A correction was made about Counter subtraction: c - d returns Counter({'a': 2}), not the example's result. Some debated the usefulness of Counter's symmetric difference, but others defended it via set theory.

**Tags**: `#python`, `#python 3.15`, `#programming`, `#features`

---

<a id="item-6"></a>
## [Project Hail Mary Star Chart Uses GAIA DR3 for 1.8 Billion Stars](https://valhovey.github.io/gaia-mary/) ⭐️ 7.0/10

A developer created a stellar navigation chart demo that visualizes over 1.8 billion stars from the ESA's GAIA DR3 dataset into a custom skybox, accessible via web browser. This project demonstrates the practical application of large astronomical datasets in interactive visualizations, making real star data accessible to the public and inspiring interest in space exploration. The star positions and colors are based on GAIA data, except for a few bright stars. The project uses a Python script to render all stars into custom images for the skybox, and the scale of planets and stars is not accurate.

hackernews · speleo · May 21, 16:23 · [Discussion](https://news.ycombinator.com/item?id=48225297)

**Background**: GAIA is a European Space Agency mission that measures the positions, distances, and motions of stars. Its third data release (DR3) contains over 1.8 billion stars. A skybox is a 3D graphics technique that creates a background environment by mapping images to the inside of a cube, commonly used in games.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cosmos.esa.int/web/gaia/dr3">Gaia Data Release 3 (Gaia DR3) - ESA Cosmos</a></li>

</ul>
</details>

**Discussion**: The creator (speleo) explained the technical process and praised the GAIA dataset. A commenter (ggreer) pointed out that the sizes and orbits are not to scale, highlighting the vast emptiness of space. Another user (ceheaaf) recommended the game Elite Dangerous for a similar exploration experience.

**Tags**: `#astronomy`, `#data visualization`, `#GAIA`, `#star chart`, `#Python`

---

<a id="item-7"></a>
## [Blog migrated from Ubuntu 16.04 to FreeBSD after 10 years](https://crocidb.com/post/this-blog-ran-on-ubuntu-16-04-for-10-years-i-migrated-it-to-freebsd/) ⭐️ 7.0/10

The author migrated a personal blog that had been running on Ubuntu 16.04 for ten years to FreeBSD, documenting the process and lessons learned. This story highlights the practical challenges of long-term system maintenance and migration, offering valuable insights for system administrators facing similar legacy upgrades. Ubuntu 16.04 reached end-of-life in April 2021, leaving the blog without security updates. The migration involved learning FreeBSD's different package management, rc.d init system, and configuration conventions.

hackernews · speckx · May 21, 18:54 · [Discussion](https://news.ycombinator.com/item?id=48227397)

**Background**: Ubuntu 16.04 LTS (Xenial Xerus) is a long-term support release that was popular for stable server deployments, but it became obsolete. FreeBSD is a free and open-source Unix-like operating system known for its robustness, advanced networking, and ZFS filesystem, making it an attractive alternative for personal servers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/FreeBSD">FreeBSD</a></li>
<li><a href="https://klarasystems.com/articles/easily-migrate-from-linux-to-freebsd/">Easily Migrate from Linux to FreeBSD - Klara Systems</a></li>

</ul>
</details>

**Discussion**: Commenters shared similar experiences: arjie regretted high uptime on a VPS that became too hard to migrate, while others expressed fear of updating old servers. Some praised FreeBSD's clean design but noted pain points like buggy PM2 support and complex firewall configuration.

**Tags**: `#sysadmin`, `#migration`, `#freebsd`, `#ubuntu`, `#long-term maintenance`

---

<a id="item-8"></a>
## [Seattle Police Intelligence Network with Private Partners](https://prismreports.org/2026/05/20/seattle-shield-private-companies-surveillance/) ⭐️ 7.0/10

A Prism Reports investigation reveals that the Seattle Police Department operates Seattle Shield, an intelligence-sharing network involving private companies and federal agencies, prompting renewed debate over surveillance and privacy. This network blurs the line between public safety and corporate surveillance, potentially expanding the reach of law enforcement monitoring without public oversight. Seattle Shield is an unfunded program managed by SPD Officer Erin Nicholson, and its members include entities like the Church of Scientology, U.S. Navy, and Washington State Military Department, though some have since withdrawn.

hackernews · root-parent · May 21, 17:55 · [Discussion](https://news.ycombinator.com/item?id=48226588)

**Background**: Intelligence-sharing networks like Seattle Shield are designed to facilitate information exchange between law enforcement and private sector partners to counter terrorism. However, critics argue they can lead to disproportionate surveillance and erosion of civil liberties. The network operates largely without public transparency, raising concerns about accountability.

<details><summary>References</summary>
<ul>
<li><a href="https://seattleshield.org/PageMenuSwitch2.aspx?AspxAutoDetectCookieSupport=1">Seattle Shield</a></li>
<li><a href="https://truthout.org/articles/corporations-federal-agencies-are-using-seattle-polices-surveillance-network/">Corporations, Federal Agencies Are Using Seattle Police’s ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed views: some saw it as a benign neighborhood watch for businesses, while others warned of a 'Panopticon' and urged employees at partner companies to reconsider working there. A few noted that the title sensationalized the roles of Amazon and Facebook, which were only briefly mentioned.

**Tags**: `#surveillance`, `#privacy`, `#police`, `#Seattle`, `#intelligence-sharing`

---

<a id="item-9"></a>
## [Waymo Pauses Atlanta Service After Robotaxis Drive Into Floods](https://techcrunch.com/2026/05/21/waymo-pauses-atlanta-service-as-its-robotaxis-keep-driving-into-floods/) ⭐️ 7.0/10

Waymo has paused its autonomous ride-hailing service in Atlanta after repeated incidents of its robotaxis driving into flooded streets, exposing challenges in handling unusual environmental conditions. This incident highlights real-world limitations of autonomous driving systems when encountering edge cases like flooded roads, raising safety concerns and potentially affecting public trust and regulatory oversight. Waymo recalled 3,791 vehicles earlier in May 2026 for software issues related to flooded roads. The problem stems from LiDAR sensor difficulties in detecting water surfaces due to reflections and signal attenuation.

hackernews · mattas · May 21, 16:30 · [Discussion](https://news.ycombinator.com/item?id=48225426)

**Background**: Autonomous vehicles rely on sensors like LiDAR and cameras to perceive surroundings. However, water surfaces can cause LiDAR beams to reflect or be absorbed, leading to misinterpretation of flooded areas as safe to drive. Rain and poor visibility further complicate detection. Waymo's incidents in Atlanta and San Antonio prompted the recall.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techbuzz.ai/articles/waymo-recalls-robotaxis-for-driving-on-flooded-roads">Waymo recalls robotaxis for driving on flooded roads | The Tech Buzz</a></li>
<li><a href="https://distratech.com/waymo-robotaxi-flooded-roads-recall/">Waymo Recalls 3,791 Robotaxis for Driving on Flooded Roads ...</a></li>

</ul>
</details>

**Discussion**: Comments show mixed views: some see it as a normal part of service rollout and a learning opportunity, while others express concerns about AI's inability to handle edge cases despite years of development. One former Waymo insider notes that the problem is well-known and simulated, but the system is not perfect; however, Waymo remains very safe in validated domains.

**Tags**: `#autonomous vehicles`, `#Waymo`, `#AI safety`, `#edge cases`, `#flood detection`

---

<a id="item-10"></a>
## [Restored Trinity Test Photos Reveal New Atomic Details](https://spectrum.ieee.org/trinity-nuclear-test) ⭐️ 7.0/10

High-speed photographs from the 1945 Trinity nuclear test, captured by Rapatronic cameras, have been digitally restored, unveiling previously unseen details of the first atomic explosion. This restoration provides historians and scientists with a clearer view of the early moments of the nuclear age, demonstrating the value of preserving historical film through digital technology. The Rapatronic cameras used exposure times as short as 10 nanoseconds, and arrays of up to 12 cameras were deployed to capture sequential images milliseconds after detonation.

hackernews · pseudolus · May 21, 11:02 · [Discussion](https://news.ycombinator.com/item?id=48220639)

**Background**: The Rapatronic camera, developed by Harold Edgerton in the 1940s, uses two polarizing filters and a Faraday cell to achieve shutter speeds fast enough to photograph nuclear explosions. The camera's magneto-optical shutter rotates the polarization plane of light when a high-voltage pulse is applied, allowing exposures as brief as 10 nanoseconds. Such cameras were essential for documenting the earliest stages of atomic detonations.

<details><summary>References</summary>
<ul>
<li><a href="https://spectrum.ieee.org/trinity-nuclear-test">Lost Images From the 1945 Trinity Nuclear Test Restored - IEEE Spectrum</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rapatronic_camera">Rapatronic camera</a></li>
<li><a href="https://www.cbsnews.com/news/nuclear-test-videos-from-cold-war-era-restored-declassified/">Restored and declassified videos reveal power of Cold War nuclear tests - CBS News</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal connections: one used Trinity as a course starting point, another explored time zone intricacies, and a third highlighted the overlooked health impacts on downwinders near the test site, noting their exclusion from compensation acts.

**Tags**: `#history`, `#photography`, `#nuclear`, `#restoration`, `#science`

---

<a id="item-11"></a>
## [BBEdit 16 Released with One-Time Purchase Pricing](https://www.barebones.com/products/bbedit/bbedit16.html) ⭐️ 7.0/10

Bare Bones Software has released BBEdit 16, an incremental update to its long-standing macOS text editor, continuing to offer a one-time purchase license instead of a subscription model. BBEdit remains a highly respected tool for developers and writers, and its refusal to adopt subscription pricing sets it apart in an industry increasingly moving to recurring revenue models. An individual license is priced at $60 USD, a substantial real-terms decrease from the $120 ($245 inflation-adjusted) it cost in 1998. The editor supports extensibility via shell scripts, Python, Rust, or any external tool.

hackernews · qaz_plm · May 21, 18:21 · [Discussion](https://news.ycombinator.com/item?id=48226944)

**Background**: BBEdit is a proprietary text editor for macOS developed by Bare Bones Software, first released as shareware in the early 1990s. It is renowned for its powerful text manipulation tools, HTML editing features, and scriptability. The editor has maintained a loyal user base for decades, partly due to its consistent one-time purchase pricing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BBEdit">BBEdit</a></li>
<li><a href="https://grokipedia.com/page/BBEdit">BBEdit</a></li>
<li><a href="https://www.barebones.com/products/bbedit/">BBEdit | Bare Bones Software</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, with users praising BBEdit's longevity, reasonable pricing, and extensibility. Some note that alternatives like CotEditor or Zed have emerged, but many remain loyal to BBEdit for its unique workflow integration.

**Tags**: `#macOS`, `#text-editor`, `#software-release`, `#developer-tools`

---

<a id="item-12"></a>
## [Datasette Agent: AI assistant for conversational data querying](https://simonwillison.net/2026/May/21/datasette-agent/#atom-everything) ⭐️ 7.0/10

Simon Willison announced the first release of Datasette Agent, an extensible AI assistant that integrates LLM and Datasette to provide conversational querying and chart generation for data stored in Datasette. This marks the convergence of two major projects—LLM and Datasette—enabling users to interact with databases using natural language without writing SQL, which significantly lowers the barrier for data exploration and could transform data workflows for analysts and developers. Datasette Agent runs on the cheap and fast Gemini 3.1 Flash-Lite model, and can be extended via plugins such as datasette-agent-charts for chart generation using Observable Plot and datasette-agent-openai-imagegen for image generation. The live demo is available at agent.datasette.io.

rss · Simon Willison · May 21, 19:52

**Background**: Datasette is an open-source tool for exploring and publishing data, often used with SQLite databases. LLM is a CLI tool and Python library by Simon Willison for interacting with various large language models. Datasette Agent brings these together, allowing users to pose questions in plain English and get answers generated by LLMs, with optional charts and images.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/llm">GitHub - simonw/llm: Access large language models from the command-line · GitHub</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#AI assistant`, `#data exploration`, `#LLM`, `#plugin`

---

<a id="item-13"></a>
## [Flipper One Announced: Community Help Sought](https://blog.flipper.net/flipper-one-we-need-your-help/) ⭐️ 6.0/10

Flipper Devices announced the Flipper One, a pocket-sized Linux computer for hacking, and called for community support without specifying what help is needed. The Flipper One represents a significant upgrade from the popular Flipper Zero, offering more power and versatility, potentially expanding the hacking tool market to advanced users. The device is based on a Rockchip RK3576 processor with an AI hardware accelerator, features a modular design, and omits NFC, RFID, and sub-GHz radios to focus on networking and Linux capabilities.

hackernews · sandebert · May 21, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48220647)

**Background**: The Flipper Zero was a versatile wireless multi-tool for penetration testing and hobbyist hacking. The Flipper One aims to be a more powerful and open Linux platform for advanced users, with built-in Wi-Fi and Ethernet support.

<details><summary>References</summary>
<ul>
<li><a href="https://www.zdnet.com/article/flipper-one-hacking-tool-tiny-linux-pc/">The Flipper One may be the ultimate Linux PC for hackers in ...</a></li>
<li><a href="https://liliputing.com/flipper-one-is-a-pocket-sized-linux-computer-and-network-hacking-tool/">Flipper One is a pocket-sized Linux computer and networking tool</a></li>

</ul>
</details>

**Discussion**: Community members expressed confusion over the vague 'need help' message, with some unable to find the specific ask after scrolling several pages. Others raised concerns about feature creep and the second-system effect, while a few were excited about the RK3576 chip and potential for open-source projects.

**Tags**: `#Flipper`, `#hardware`, `#hacking tool`, `#open source`, `#IoT`

---

<a id="item-14"></a>
## [How fast is 10 tokens per second really?](https://simonwillison.net/2026/May/20/tokens-per-second/#atom-everything) ⭐️ 6.0/10

Mike Veerman created a simple HTML app that simulates LLM token output speeds ranging from 5 to 800 tokens per second, allowing users to visualize and compare different advertised rates. This tool makes abstract speed specifications tangible, helping developers and users better understand and compare LLM performance when choosing models. The app is a single HTML file hosted on GitHub Pages, with source code available on GitHub. It simulates speeds from 5 to 800 tokens per second, covering both slow and very fast models.

rss · Simon Willison · May 20, 17:57

**Background**: In large language models, a 'token' is a unit of text, roughly equivalent to a word or subword. Output speed, measured in tokens per second, is a key metric for user experience — slower speeds feel laggy, while faster speeds enable real-time interactions. Many model providers advertise their speeds, but it can be hard to gauge what a number like '30 tokens/second' feels like in practice.

**Tags**: `#llms`, `#ai`, `#tools`, `#visualization`, `#performance`

---

<a id="item-15"></a>
## [Simon Willison's Cautious Take on Google I/O 2026](https://simonwillison.net/2026/May/20/google-io/#atom-everything) ⭐️ 6.0/10

Simon Willison shared his cautious analysis of Google I/O announcements, highlighting Gemini 3.5 Flash and the upcoming Gemini Spark personal AI agent, which reportedly runs on a combination of Gemini 3.5 Flash and a new system called Antigravity. This matters because Gemini Spark represents Google's ambitious entry into the personal AI agent space, competing with tools like OpenClaw, and its security approach will be critical as users trust it with sensitive data. The shift from open-source Gemini CLI to closed-source Antigravity CLI also signals a change in Google's developer strategy. According to Simon Willison, the Gemini Spark FAQ states it runs on 'Gemini 3.5 Flash and Antigravity,' but the connection between the hosted agent and the Antigravity Go binary is unclear. Additionally, Google announced that the open-source Gemini CLI (TypeScript, Apache 2.0) will cease to work on June 18, 2026, replaced by the closed-source Antigravity CLI.

rss · Simon Willison · May 20, 15:32

**Background**: Google I/O is Google's annual developer conference where it announces new products and technologies. Gemini is Google's family of large language models. Gemini Spark is described as a 24/7 personal AI agent that can connect with Google apps like Gmail and Calendar to proactively manage tasks. Antigravity appears to be a new platform that includes a desktop app, CLI, SDK, and IDE, and seems to be the underlying runtime for Gemini Spark. OpenClaw is an open-source autonomous AI agent that executes tasks via LLMs and serves as a competitor to Gemini Spark.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/products/gemini-app/next-evolution-gemini-app/">The Gemini app becomes more agentic, delivering proactive, 24/7 help</a></li>
<li><a href="https://www.everydev.ai/tools/gemini-spark">Gemini Spark - Google Personal AI Agent | EveryDev. ai</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Google I/O`, `#Gemini`, `#AI agent`, `#personal AI`

---

<a id="item-16"></a>
## [Rocket Lab wins $90M Space Force satellite contract](https://www.investing.com/news/company-news/rocket-lab-wins-90m-space-force-contract-for-two-satellites-93CH-4705643) ⭐️ 6.0/10

Rocket Lab has been awarded a $90 million contract by the U.S. Space Force to build and deliver two satellites, marking a significant step into defense satellite manufacturing. This contract signals growing government confidence in commercial aerospace companies for national security missions and validates Rocket Lab's vertical integration strategy spanning launch and satellite production. The award covers the design, manufacture, and delivery of two satellites, though specific mission details and timelines have not been publicly disclosed. It is one of the largest satellite manufacturing contracts for Rocket Lab to date.

rss · Investing.com All News · May 22, 00:05

**Background**: Rocket Lab is a private aerospace company best known for its Electron small-lift launch vehicle. The company has been expanding into satellite manufacturing through its subsidiary, aiming to become a one-stop shop for space services. The U.S. Space Force has been awarding contracts to multiple commercial providers to diversify access to space and leverage innovative technologies.

**Tags**: `#space`, `#government contract`, `#satellite`, `#aerospace`

---