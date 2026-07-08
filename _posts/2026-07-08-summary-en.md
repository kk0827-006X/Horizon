---
layout: default
title: "Horizon Summary: 2026-07-08 (EN)"
date: 2026-07-08
lang: en
---

> From 38 items, 14 important content pieces were selected

---

1. [Kokoro: Local, CPU-Friendly, High-Quality TTS Model](#item-1) ⭐️ 8.0/10
2. [EU Chat Control Proposals Threaten Encryption and Privacy](#item-2) ⭐️ 8.0/10
3. [EU mandates driver monitoring cameras in all new cars](#item-3) ⭐️ 8.0/10
4. [sqlite-utils 4.0 released with schema migrations](#item-4) ⭐️ 8.0/10
5. [Tencent Releases Hy3: 295B MoE Model Under Apache 2.0](#item-5) ⭐️ 8.0/10
6. [Datasette 1.0a36 adds bulk insert UI and JSON API fixes](#item-6) ⭐️ 7.0/10
7. [StreetComplete: Gamifying OpenStreetMap Data Improvement](#item-7) ⭐️ 7.0/10
8. [Davit: Native macOS UI for Apple Containers](#item-8) ⭐️ 7.0/10
9. [30papers.com: Ilya's 30 ML Papers for Beginners](#item-9) ⭐️ 7.0/10
10. [Why we built yet another Postgres connection pooler: pgdog](#item-10) ⭐️ 7.0/10
11. [TrueType Font Generates QR Codes via Glyph Substitution](#item-11) ⭐️ 6.0/10
12. [GitHub Code Web Component Built with GPT-5.5](#item-12) ⭐️ 6.0/10
13. [sqlite-utils 4.0rc4 Released with AI Review Feedback](#item-13) ⭐️ 6.0/10
14. [sqlite-utils 4.0rc3 Adds Compound Foreign Keys](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Kokoro: Local, CPU-Friendly, High-Quality TTS Model](https://ariya.io/2026/03/local-cpu-friendly-high-quality-tts-text-to-speech-with-kokoro/) ⭐️ 8.0/10

Kokoro is an open-weight TTS model with 82 million parameters that delivers high-quality speech synthesis on CPU, making it accessible without requiring a powerful GPU. This expands accessibility for voice applications to users without dedicated GPUs, bridging the gap for hobbyists, accessibility products, and low-resource environments. Despite its lightweight architecture (82M parameters), Kokoro achieves quality comparable to larger models, is Apache-licensed, and can be deployed via CLI or WebUI.

hackernews · speckx · Jul 7, 18:24 · [Discussion](https://news.ycombinator.com/item?id=48821576)

**Background**: Traditional high-quality TTS models often require powerful GPUs due to their size. Kokoro's design focuses on efficiency, allowing real-time speech synthesis on CPU, which is particularly beneficial for users without GPU resources.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/hexgrad/Kokoro-82M">hexgrad/Kokoro-82M · Hugging Face</a></li>
<li><a href="https://github.com/hexgrad/kokoro">GitHub - hexgrad/kokoro: https://hf.co/hexgrad/Kokoro-82M</a></li>

</ul>
</details>

**Discussion**: Community comments highlight real-world use in accessibility products and positive experiences with CPU-only setups. Some users note limitations with short phrases and homograph pronunciation, but overall sentiment is very positive, with users sharing integrations like voice input systems and podcast generation.

**Tags**: `#TTS`, `#text-to-speech`, `#machine learning`, `#accessibility`, `#open source`

---

<a id="item-2"></a>
## [EU Chat Control Proposals Threaten Encryption and Privacy](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 8.0/10

The European Union's Chat Control proposals (CSAR) would require providers to scan private messages for illegal content, including client-side scanning that breaks end-to-end encryption. If passed, these laws would undermine end-to-end encryption and mass surveillance of all EU citizens, setting a dangerous precedent for global privacy. Chat Control 1.0 expired, but companies continue scanning voluntarily; Chat Control 2.0 would mandate client-side scanning, affecting encrypted messaging apps like WhatsApp and Signal.

hackernews · gasull · Jul 7, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48818311)

**Background**: Chat Control refers to a set of EU regulations proposed to combat child sexual abuse material (CSAM). The approach involves scanning private communications, which critics argue breaks encryption and enables mass surveillance. Client-side scanning occurs on the user's device before encryption or after decryption, undermining the security of end-to-end encrypted systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://edri.org/our-work/chat-control-what-is-actually-going-on/">Chat Control: What is actually going on? - European Digital Rights (EDRi)</a></li>
<li><a href="https://fightchatcontrol.eu/">Fight Chat Control - Protect Digital Privacy in the EU</a></li>

</ul>
</details>

**Discussion**: Comments express strong opposition, noting the broad scope and privacy invasion. Users highlight that while stopping CSAM is important, this law grants excessive power and undermines encryption. Some question how scanning can work with E2EE, pointing to client-side scanning risks.

**Tags**: `#privacy`, `#encryption`, `#surveillance`, `#EU law`, `#public policy`

---

<a id="item-3"></a>
## [EU mandates driver monitoring cameras in all new cars](https://allaboutcookies.org/eu-mandatory-distracted-driver-system) ⭐️ 8.0/10

The European Union has mandated that all new cars sold from July 2024 must include a driver monitoring camera system to detect distraction and drowsiness. This regulation is part of the General Safety Regulations aiming to reduce road fatalities. This mandate could significantly reduce traffic accidents and save lives by alerting distracted drivers. However, it also sparks debate over privacy, data security, and the usability of modern car interfaces. The system uses an infrared camera and AI to track eye movement, head position, and signs of drowsiness. It can issue warnings and, in some cases, intervene with braking or steering if the driver does not respond.

hackernews · nickslaughter02 · Jul 7, 20:50 · [Discussion](https://news.ycombinator.com/item?id=48823557)

**Background**: Driver monitoring systems (DMS) have been in development for years, using computer vision to assess driver alertness. The EU's General Safety Regulations, adopted in 2019, set a roadmap to halve road fatalities by 2030. These regulations also mandate other advanced driver-assistance systems (ADAS) like lane-keeping assist and automated emergency braking. The DMS requirement applies to all new type approvals from July 2024 and all new cars from July 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Driver_Monitoring_System">Driver monitoring system - Wikipedia</a></li>
<li><a href="https://reclaimthenet.org/eu-mandates-driver-facing-cameras-in-new-cars-from-today">EU Mandates Driver-Facing Cameras in New Cars From Today</a></li>
<li><a href="https://smarteye.se/blog/the-general-safety-regulations-gsr-and-driver-monitoring-systems-dms/">How Driver Monitoring Systems (DMS) Are Being Made Mandatory ...</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed feelings: some users worry about annoying alerts and poor UX in modern cars, citing examples like false positives from speed limit sign recognition. Others note that existing DMS in Fords and other brands are accurate and could save lives, though privacy and government overreach remain concerns.

**Tags**: `#regulation`, `#automotive`, `#privacy`, `#safety`, `#technology`

---

<a id="item-4"></a>
## [sqlite-utils 4.0 released with schema migrations](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0 has been released, introducing database schema migrations defined in Python files, nested transactions via a new db.atomic() method, and support for compound foreign keys. This major version update significantly enhances sqlite-utils' ability to manage SQLite database schemas programmatically, addressing a long-standing need for version-controlled schema changes in the SQLite ecosystem. It is particularly valuable for Python developers and users of the Datasette project. Migrations are implemented using the table.transform() method, which follows the SQLite-recommended pattern of creating a temporary table with the new schema, copying data, and renaming tables. Compound foreign keys allow referencing composite primary keys across tables.

rss · Simon Willison · Jul 7, 19:32

**Background**: sqlite-utils is a Python library and command-line tool for manipulating SQLite databases, widely used in the Datasette ecosystem for data publishing and exploration. Previously, schema changes required manual SQL statements or external migration tools, making it difficult to track changes over time.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite-utils.datasette.io/en/latest/migrations.html">Database migrations - sqlite-utils</a></li>
<li><a href="https://simonwillison.net/2026/Jul/7/sqlite-utils-4/">sqlite-utils 4.0, now with database schema migrations</a></li>
<li><a href="https://github.com/simonw/sqlite-utils/issues/117">Support for compound (composite) foreign keys · Issue #117 · simonw/sqlite-utils</a></li>

</ul>
</details>

**Tags**: `#sqlite-utils`, `#database migrations`, `#SQLite`, `#Python`, `#tools`

---

<a id="item-5"></a>
## [Tencent Releases Hy3: 295B MoE Model Under Apache 2.0](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

Tencent released Hy3, a 295B-parameter Mixture-of-Experts model with 21B active parameters, under the permissive Apache 2.0 license, and it is available for free on OpenRouter until July 21st. Hy3 outperforms similarly-sized models and rivals flagship open-source models with 2-5x parameters, marking a significant advancement in open-source AI from a major Chinese company. The full model is 598GB on Hugging Face, with an FP8 quantized version at 300GB, and supports a context length of 256K tokens.

rss · Simon Willison · Jul 6, 23:57

**Background**: Hy3 uses a Mixture-of-Experts (MoE) architecture, which has a large total parameter count but only activates a subset per input, keeping inference efficient. The model also incorporates Multi-Token Prediction (MTP) layers, a technique that enhances training by predicting multiple future tokens simultaneously, as first seen in DeepSeek-V3. This approach allows Hy3 to achieve high performance while maintaining lower computational cost compared to dense models of similar total size.

<details><summary>References</summary>
<ul>
<li><a href="https://www.baeldung.com/cs/mixture-of-experts">The Mixture-of-Experts ML Approach - Baeldung</a></li>
<li><a href="https://docs.nvidia.com/nemo/megatron-bridge/nightly/training/multi-token-prediction.html">Multi-Token Prediction (MTP) — Megatron Bridge</a></li>

</ul>
</details>

**Tags**: `#AI/ML`, `#open-source`, `#MoE`, `#Tencent`, `#LLM`

---

<a id="item-6"></a>
## [Datasette 1.0a36 adds bulk insert UI and JSON API fixes](https://github.com/simonw/datasette/releases/tag/1.0a36) ⭐️ 7.0/10

Datasette 1.0a36 introduces new UIs for bulk inserting rows (from TSV, CSV, or JSON) and creating a table from data, along with numerous JSON API consistency fixes in preparation for a 1.0 stable release. These features significantly improve the usability of Datasette for data ingestion and manipulation, making it easier for users to work with tabular data directly in the web interface. The JSON API fixes ensure consistent behavior, which is crucial for developers relying on Datasette's API for integration. The bulk insert UI supports skipping rows with existing primary keys or upserting when the actor has appropriate permissions. A new max_post_body_bytes setting (default 2MB) protects against memory exhaustion, while BLOB handling now includes previews and dedicated controls for binary values.

github · simonw · Jul 7, 21:43

**Background**: Datasette is an open-source tool for exploring and publishing data as interactive websites and APIs. It supports SQLite databases and offers a web interface for querying, browsing, and editing data. This alpha release continues the path toward a 1.0 stable version, adding user-requested features for bulk operations and API consistency.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>
<li><a href="https://docs.datasette.io/en/latest/json_api.html">JSON API - Datasette documentation</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#data`, `#database`, `#UI`, `#JSON API`

---

<a id="item-7"></a>
## [StreetComplete: Gamifying OpenStreetMap Data Improvement](https://streetcomplete.app/) ⭐️ 7.0/10

StreetComplete is an Android app that presents users with simple, location-based quests to fill in missing OpenStreetMap data, such as street names, building heights, or sidewalk details. This app significantly lowers the barrier to entry for contributing to OpenStreetMap, enabling non-expert users to improve map data in their vicinity, which enhances the overall quality and coverage of OSM. The app uses the OpenStreetMap API directly (since v26.0) and migrated from Tangram-ES to MapLibre for map rendering in v59.0. It is available on Google Play and F-Droid, and translations are managed via POEditor.

hackernews · kls0e · Jul 7, 12:38 · [Discussion](https://news.ycombinator.com/item?id=48816883)

**Background**: OpenStreetMap (OSM) is a collaborative, free geographic database built by volunteers. Traditional editing requires knowledge of tagging schemes and editing tools, which can be intimidating. StreetComplete applies gamification by turning data collection into a series of simple, rewarding quests, making it accessible to casual users.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/StreetComplete">StreetComplete</a></li>
<li><a href="https://streetcomplete.app/">StreetComplete</a></li>
<li><a href="https://wiki.openstreetmap.org/wiki/StreetComplete">StreetComplete - OpenStreetMap Wiki StreetComplete - Apps on Google Play GitHub - streetcomplete/StreetComplete: Easy to use ... StreetComplete - Wikipedia Releases · streetcomplete/StreetComplete - GitHub StreetComplete | F-Droid - Free and Open Source Android App ...</a></li>

</ul>
</details>

**Discussion**: Commenters praise the app for its beginner-friendly interface and fun quests, but some note limitations like inability to add roads or footpaths directly. Others appreciate complementary apps like Every Door. A concern is raised about Google potentially benefiting from OSM data without reciprocating.

**Tags**: `#OpenStreetMap`, `#mobile app`, `#crowdsourcing`, `#mapping`, `#open data`

---

<a id="item-8"></a>
## [Davit: Native macOS UI for Apple Containers](https://davit.app/) ⭐️ 7.0/10

Davit is a new open-source macOS app that provides a native user interface for managing Apple's container runtime, built with the ContainerAPIClient library directly. This app fills a gap in Apple's container ecosystem by offering a graphical interface, making container management more accessible to macOS users who prefer native apps over command-line tools. The app is 17 MB compressed (56 MB binary), was developed with 28 commits over 3 days all co-authored by Claude Fable 5, and is signed and notarized.

hackernews · xinit · Jul 7, 18:44 · [Discussion](https://news.ycombinator.com/item?id=48821848)

**Background**: Apple Container is an open-source command-line utility and runtime developed by Apple for running Linux containers on macOS using lightweight VMs via Virtualization.framework, introduced in 2025 at WWDC. Before Davit, users managed containers via terminal or third-party tools like Orbstack.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_container">Apple container - Wikipedia</a></li>
<li><a href="https://github.com/apple/container">GitHub - apple/container: A tool for creating and running Linux containers using lightweight virtual machines on a Mac. It is written in Swift, and optimized for Apple silicon. · GitHub</a></li>
<li><a href="https://medium.com/@rpavank2000/apples-container-native-lightweight-container-runtime-for-macos-44a69d57ef41">Apple’s Container: Native, Lightweight Container Runtime for macOS | by Pavan Kumar | Medium</a></li>

</ul>
</details>

**Discussion**: The Hacker News community reacted positively, praising the app's native feel and small size, with suggestions for a getting started tutorial. Some users compared it to Orbstack, while others noted technical details like binary compression ratio and macOS UI quirks.

**Tags**: `#apple containers`, `#macos`, `#docker`, `#ui`, `#open source`

---

<a id="item-9"></a>
## [30papers.com: Ilya's 30 ML Papers for Beginners](https://30papers.com/) ⭐️ 7.0/10

A student at Trinity College Dublin created 30papers.com, a website that presents a curated list of 30 essential machine learning papers attributed to Ilya Sutskever in a beginner-friendly format, with explanations and toggles for animations. This resource lowers the barrier for newcomers to study foundational ML papers, potentially accelerating learning in the field. However, the authenticity of the paper list is questioned as the source is unverified. The website includes toggles to disable movement and background animations after user complaints. It is a work-in-progress side project with a GitHub repository for contributions.

hackernews · notmcrowley · Jul 7, 15:58 · [Discussion](https://news.ycombinator.com/item?id=48819608)

**Background**: Ilya Sutskever is a co-founder and chief scientist of OpenAI, known for his influential work in deep learning and neural networks. Machine learning papers are primary sources of research findings, but beginners often find them inaccessible due to dense mathematics and jargon. This website aims to bridge that gap by summarizing key papers in a simplified format.

**Discussion**: Commenters praised the idea but criticized the heavy animations and lack of reading order. The author responded by adding accessibility toggles and explaining the project's origin as a personal learning tool. Some users suggested alternative resources like the Welch Labs Illustrated Guide to AI.

**Tags**: `#machine learning`, `#research papers`, `#beginners`, `#curated list`, `#Ilya Sutskever`

---

<a id="item-10"></a>
## [Why we built yet another Postgres connection pooler: pgdog](https://pgdog.dev/blog/why-yet-another-connection-pooler) ⭐️ 7.0/10

pgdog is a new open-source connection pooler, load balancer, and sharding proxy for PostgreSQL, as introduced in a blog post explaining its design motivations and addressing limitations in existing poolers. pgdog tackles common issues like connection state leakage and single-threaded bottlenecks, and its choice of AGPL license over BSL sparks discussion in the open-source community, potentially influencing Postgres infrastructure decisions. pgdog is multi-threaded and resets connection state between uses to prevent leakage, and it improves NOTIFY performance, though one commenter questions whether this breaks transactional semantics.

hackernews · levkk · Jul 7, 15:36 · [Discussion](https://news.ycombinator.com/item?id=48819308)

**Background**: Connection poolers manage a pool of persistent database connections, multiplexing many client connections over fewer backend connections to reduce overhead. Existing poolers like PgBouncer and Odyssey are widely used, but pgdog aims to address specific limitations such as state leakage and single-threaded performance bottlenecks.

<details><summary>References</summary>
<ul>
<li><a href="https://pgdog.dev/blog/why-yet-another-connection-pooler">Why we built yet another Postgres connection pooler - PgDog</a></li>
<li><a href="https://github.com/pgdogdev/pgdog">GitHub - pgdogdev/pgdog: PostgreSQL connection pooler, load balancer and database sharder. · GitHub</a></li>
<li><a href="https://docs.pgdog.dev/">PgDog</a></li>

</ul>
</details>

**Discussion**: Commenters praised the use of AGPL license over BSL. One raised concerns about state leakage in typical setups. Others asked about query caching, schema switching, and NOTIFY transactional semantics.

**Tags**: `#Postgres`, `#connection pooling`, `#pgdog`, `#database performance`, `#open source`

---

<a id="item-11"></a>
## [TrueType Font Generates QR Codes via Glyph Substitution](https://github.com/jimparis/qr-font) ⭐️ 6.0/10

Jim Paris has released a TrueType font that renders typed text as a scannable QR code by abusing glyph substitution tables. The font is available on GitHub and works as a proof of concept for embedding QR codes in any text field. This hack demonstrates a novel way to generate QR codes without special software, leveraging the font rendering pipeline. While not practical for general use, it showcases the power of OpenType font features and sparks creativity in font engineering. The font only supports Basic Latin characters and has issues with spaces—a QR code including a space may not scan correctly. However, it allows users to select the QR code as text and copy the original message, offering a unique text extraction feature.

hackernews · arantius · Jul 7, 16:30 · [Discussion](https://news.ycombinator.com/item?id=48820119)

**Background**: TrueType and OpenType fonts can include a GSUB (Glyph Substitution) table that replaces one glyph with another based on context, commonly used for ligatures or language-specific forms. This font exploits GSUB to replace each character with a QR code segment, assembling the full code from the input text. QR codes are two-dimensional barcodes that encode data, scannable by most smartphone cameras.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/typography/opentype/spec/gsub">GSUB — Glyph Substitution Table (OpenType 1.9.1) - Typography</a></li>
<li><a href="https://learn.microsoft.com/en-us/typography/develop/processing-part2">OpenType glyph processing (part 2) - Typography | Microsoft Learn</a></li>

</ul>
</details>

**Discussion**: Commenters were amazed by the clever hack, calling it 'fun' and 'amazing' despite its limitations. They noted spacing issues (QR code fails with spaces on Safari iOS) and the restriction to English only. A positive aspect is that selecting the QR code copies the original text, which some found useful.

**Tags**: `#font`, `#qr-code`, `#true-type`, `#hack`

---

<a id="item-12"></a>
## [GitHub Code Web Component Built with GPT-5.5](https://simonwillison.net/2026/Jul/7/github-code-component/#atom-everything) ⭐️ 6.0/10

Simon Willison created an experimental Web Component named github-code that embeds specified lines of code from GitHub repositories, generated entirely using GPT-5.5 via a single prompt. This demonstrates the growing capability of large language models like GPT-5.5 to produce functional, reusable web components from natural language descriptions, lowering the barrier for developers to create custom elements without deep framework knowledge. The component takes a GitHub URL with a line range, converts it to a raw.githubusercontent.com URL, fetches the file, and displays the specified lines with line numbers but no syntax highlighting.

rss · Simon Willison · Jul 7, 16:18

**Background**: Web Components are a set of web platform APIs that allow developers to create custom, reusable HTML elements with encapsulated styling and behavior. GPT-5.5 is OpenAI's latest large language model released in April 2026, known for strong coding and reasoning capabilities. The raw.githubusercontent.com domain serves raw file content directly from GitHub repositories.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Web_Components">Web Components</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>
<li><a href="https://github.com/orgs/community/discussions/42655">Not able to open https://raw.githubusercontent.com · community · Discussion #42655</a></li>

</ul>
</details>

**Tags**: `#web-components`, `#github`, `#LLM`, `#experimental-tool`, `#simon-willison`

---

<a id="item-13"></a>
## [sqlite-utils 4.0rc4 Released with AI Review Feedback](https://simonwillison.net/2026/Jul/7/sqlite-utils-2/#atom-everything) ⭐️ 6.0/10

Simon Willison released sqlite-utils 4.0rc4, the last release candidate before the stable 4.0 version, which mainly implements feedback from a detailed code review by the AI model Claude Fable 5. This demonstrates a practical integration of AI-assisted code review into an active open-source project, potentially improving code quality and reducing bugs before final release. It also highlights the growing role of large language models in software development workflows. The RC includes changes based on issue #769 comments from Claude Fable 5's review. This is the fourth release candidate, indicating the stable release is imminent.

rss · Simon Willison · Jul 7, 05:36

**Background**: sqlite-utils is a Python command-line tool and library for manipulating SQLite databases, created by Simon Willison. It simplifies tasks like importing data, running queries, and creating tables. Claude Fable 5 is a large language model developed by Anthropic, released as a safer version of the more powerful Claude Mythos model, capable of detailed code analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#sqlite-utils`, `#release-candidate`, `#SQLite`, `#AI-review`

---

<a id="item-14"></a>
## [sqlite-utils 4.0rc3 Adds Compound Foreign Keys](https://simonwillison.net/2026/Jul/6/sqlite-utils/#atom-everything) ⭐️ 6.0/10

sqlite-utils 4.0rc3 introduces support for introspecting and creating compound foreign keys, and now follows SQLite's convention for case-insensitive column matching. This release enhances the tool's ability to handle complex database schemas more accurately, benefiting developers who work with multi-column foreign key relationships and case-insensitive queries in SQLite. The compound foreign key feature involves a subtle breaking change to the table.foreign_keys property, which necessitated inclusion in the 4.0 stable release. Case-insensitive column matching touched multiple parts of the codebase.

rss · Simon Willison · Jul 6, 05:40

**Background**: SQLite supports foreign key constraints, including composite foreign keys that reference multiple parent columns. Compound foreign keys allow a foreign key to span multiple columns, enabling complex relational integrity. SQLite also provides the NOCASE collation for case-insensitive comparisons, but column name matching was previously case-sensitive. This update aligns sqlite-utils with SQLite's default behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/foreignkeys.html">SQLite Foreign Key Support</a></li>
<li><a href="https://stackoverflow.com/questions/8002756/sqlite-composite-key-2-foreign-keys-link-table">database design - SQLite composite key (2 foreign keys) Link ... Code sample</a></li>
<li><a href="https://shallowdepth.online/posts/2022/01/5-ways-to-implement-case-insensitive-search-in-sqlite-with-full-unicode-support/">5 ways to implement case-insensitive search in SQLite with full Unicode support | ShallowDepth</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#python`, `#database`, `#release`

---