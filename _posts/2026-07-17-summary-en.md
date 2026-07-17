---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 48 items, 15 important content pieces were selected

---

1. [Moonshot AI Releases Kimi K3, Open Frontier Model](#item-1) ⭐️ 9.0/10
2. [GPT-5.6 Codex Bug Deletes User Files in Full Access Mode](#item-2) ⭐️ 9.0/10
3. [Inkling: Thinking Machines Lab's Open-Weights MoE Model](#item-3) ⭐️ 9.0/10
4. [Linus Torvalds Endorses AI as Tool in Linux Development](#item-4) ⭐️ 9.0/10
5. [Decoy Font Hides Secret Message from AI, Revealed by Blurring](#item-5) ⭐️ 8.0/10
6. [Firefox Runs Inside Another Browser via WebAssembly](#item-6) ⭐️ 8.0/10
7. [xAI open-sources Grok Build after privacy backlash](#item-7) ⭐️ 8.0/10
8. [Claude web_fetch tool tricked into leaking private memories](#item-8) ⭐️ 8.0/10
9. [LM Studio Launches Bionic: AI Agent for Open Models](#item-9) ⭐️ 7.0/10
10. [Microsoft open-sources Comic Chat, nostalgic IRC client](#item-10) ⭐️ 7.0/10
11. [Classical ML for LLM Text Detection](#item-11) ⭐️ 7.0/10
12. [OnePlus halts new product launches in Europe and North America](#item-12) ⭐️ 7.0/10
13. [Immersive Linear Algebra Book with Interactive 3D Figures (2015)](#item-13) ⭐️ 7.0/10
14. [Google Rebrands NotebookLM to Gemini Notebook](#item-14) ⭐️ 6.0/10
15. [WebAssembly tool converts Mermaid diagrams to Unicode box art](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Moonshot AI Releases Kimi K3, Open Frontier Model](https://www.kimi.com/blog/kimi-k3) ⭐️ 9.0/10

Moonshot AI has released Kimi K3, an open frontier intelligence model that reportedly achieves performance second only to proprietary models like Claude Fable 5 and GPT-5.6 Sol, with full model weights to be made available in the coming days. This release marks a significant milestone in open AI, potentially democratizing access to frontier-level model capabilities and challenging the dominance of closed-source leaders. The community's strong engagement and discussion around API training and costs reflect its impact on the AI ecosystem. Kimi K3 is a 2.5 trillion parameter MoE model with a 1M-token context window, optimized for long-horizon coding and end-to-end knowledge work. Full weights and a technical report are promised soon, but early benchmark results claim it ranks just behind the top proprietary models.

hackernews · vincent_s · Jul 16, 14:46 · [Discussion](https://news.ycombinator.com/item?id=48935342)

**Background**: Frontier AI models have traditionally been proprietary, with limited access to weights and full capabilities. Open models like Kimi K3 aim to provide comparable performance while allowing researchers and developers to inspect, modify, and self-host the model. This approach could accelerate innovation and reduce dependence on a few large AI labs.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://wan27.org/blog/kimi-k3-explained">What Is Kimi K3? Moonshot AI's 2.5T Flagship Model Explained ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight both excitement and caution: some users express concerns about Moonshot AI training on API data as per their terms, while others discuss the high inference cost and the strategic implications of Chinese labs pushing toward commoditized AI. The overall sentiment is one of cautious optimism, with recognition of the model's strong benchmark performance.

**Tags**: `#AI`, `#open-source`, `#large language models`, `#Moonshot AI`

---

<a id="item-2"></a>
## [GPT-5.6 Codex Bug Deletes User Files in Full Access Mode](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 9.0/10

OpenAI has confirmed a bug in GPT-5.6's Codex where the model can delete user files when full access mode is enabled without sandboxing, because it mistakenly targets $HOME instead of a temporary directory. This bug poses a critical safety risk for AI coding agents, potentially causing irreversible data loss for developers who rely on Codex for automated tasks. It underscores the urgent need for robust sandboxing and review mechanisms in AI-assisted development tools. The issue occurs when full access mode is enabled and Codex runs without sandboxing protections or auto review. The model attempts to override the $HOME environment variable to define a temporary directory but mistakenly deletes $HOME instead.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is an AI coding agent from OpenAI that can perform tasks like code generation, editing, and terminal commands. Full access mode allows Codex to directly interact with the user's file system, which requires careful safeguards. Sandboxing and auto-review are protections that can prevent unintended file modifications.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-codex/">Introducing Codex | OpenAI</a></li>
<li><a href="https://talkin.icu/blog/codex-app-full-access-still">Codex App: Full Access Still Limited To Workspace-Write Sandbox</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-3"></a>
## [Inkling: Thinking Machines Lab's Open-Weights MoE Model](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, a 975B total parameter open-weights multimodal Mixture-of-Experts model under Apache-2.0 license, trained on 45 trillion tokens of text, images, audio, and video. Inkling strengthens the US open-weights AI ecosystem, offering a competitive base model fine-tunable via the Tinker platform, and its Apache-2.0 license encourages broad adoption and customization. Inkling has 975B total parameters with 41B active per token, and Thinking Machines also announced Inkling-Small (276B total, 12B active) which is still in testing. The model card and training data documentation are noted to be sparse.

rss · Simon Willison · Jul 16, 15:35

**Background**: Open-weights models allow users to download and use the trained weights but may not include full training code or data, distinguishing them from fully open-source AI. Mixture-of-Experts (MoE) architecture divides the model into multiple specialized sub-models (experts) and activates only a subset per input, enabling large total parameter counts with efficient inference. Inkling is a multimodal model that handles text, images, audio, and video.

<details><summary>References</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told – Open Source Initiative</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>

</ul>
</details>

**Tags**: `#open-weights`, `#mixture-of-experts`, `#multimodal`, `#AI model`, `#Thinking Machines Lab`

---

<a id="item-4"></a>
## [Linus Torvalds Endorses AI as Tool in Linux Development](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 9.0/10

Linus Torvalds, the creator of Linux, publicly stated on the Linux Media Mailing List that AI is a clearly useful tool for kernel development, and that those who disagree can fork the project or leave. This definitive endorsement from the top Linux maintainer could shift the open-source community's stance on AI, signaling that AI integration in kernel development is now an accepted practice. Torvalds emphasized that AI usefulness is no longer in question, though he acknowledged uncertainties about the AI economy. The statement was made on the kernel's media mailing list, indicating relevance to multimedia subsystem development.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linus Torvalds is the creator and lead maintainer of the Linux kernel, one of the most influential open-source projects. His opinions carry significant weight in the developer community. AI tools, such as large language models, are increasingly used for code generation, bug fixing, and documentation.

**Tags**: `#Linux`, `#AI`, `#open source`, `#kernel`, `#Linus Torvalds`

---

<a id="item-5"></a>
## [Decoy Font Hides Secret Message from AI, Revealed by Blurring](https://www.mixfont.com/experiments/decoy-font) ⭐️ 8.0/10

Mixfont has released 'Decoy Font', a typeface that encodes two different messages in the same glyphs: one visible to humans and a second hidden message readable only when the text is blurred, exploiting differences in how AI models perceive spatial frequencies. This project highlights vulnerabilities in AI image recognition, demonstrating that vision models can be fooled by adversarial examples that are imperceptible to humans, and raises questions about the robustness of AI systems in security-sensitive applications. The font uses separate spatial frequencies: high-frequency components form the visible 'decoy' letters, while low-frequency components create the hidden message that emerges when the image is downsampled or blurred. The technique is related to adversarial examples in machine learning.

hackernews · ray__ · Jul 16, 16:18 · [Discussion](https://news.ycombinator.com/item?id=48936584)

**Background**: Adversarial examples are inputs intentionally perturbed to cause a machine learning model to make a mistake. In image recognition, small pixel changes invisible to humans can confuse models. Decoy Font uses the same principle by embedding two letters in the same space using different spatial frequencies, so that an AI model's interpretation changes with blur level or resolution.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mixfont.com/experiments/decoy-font">Decoy Font: A TTF font that hides what you type</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adversarial_machine_learning">Adversarial machine learning - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members tested Decoy Font with various models: GPT-4 and Claude read the visible text correctly, but when prompted about a hidden message, GPT-4 partially identified it while Claude could not. Others noted that reducing resolution (e.g., to 150x150) makes the hidden text readable, and the project is considered a cool but not practically useful demonstration.

**Tags**: `#font`, `#AI`, `#image-recognition`, `#adversarial-examples`, `#typography`

---

<a id="item-6"></a>
## [Firefox Runs Inside Another Browser via WebAssembly](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 8.0/10

Puter has compiled the entire Firefox browser to WebAssembly, enabling it to run inside another browser using Gecko's single-process support. The project consumed an estimated $25,000 in AI tokens from Claude Opus and Fable. This demonstrates an unprecedented level of browser-in-browser capability, potentially enabling new forms of sandboxing, cross-browser testing, and legacy application compatibility. It also showcases the power of AI-assisted programming in tackling complex compilation challenges. All network traffic is proxied through Puter's server using the Wisp protocol over a WebSocket, because browser code cannot open arbitrary connections. The team had to scale servers to handle Hacker News traffic, and the demo claims end-to-end encryption, which was confirmed by inspecting WebSocket messages.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (WASM) is a binary instruction format that allows code written in languages like C/C++ to run in web browsers at near-native speed. Compiling a full browser engine like Gecko into WASM requires extensive modification and is technically challenging. Puter is an open-source internet operating system project.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low ...</a></li>
<li><a href="https://github.com/HeyPuter/puter">GitHub - HeyPuter/ puter : The Internet Computer!</a></li>

</ul>
</details>

**Discussion**: On Hacker News, commenters expressed amazement at the technical feat, though some questioned the practicality and cost. The Puter team responded about scaling issues and confirmed end-to-end encryption.

**Tags**: `#WebAssembly`, `#Firefox`, `#browser`, `#compilation`, `#demo`

---

<a id="item-7"></a>
## [xAI open-sources Grok Build after privacy backlash](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 8.0/10

xAI released the entire Grok Build codebase under an Apache 2.0 license on GitHub after a severe privacy flaw was discovered where the Grok CLI tool uploaded entire directories, including sensitive user data, by default. This incident highlights significant privacy risks in AI-powered CLI tools and the importance of transparency and user control. By open-sourcing the code, xAI aims to regain user trust and set a precedent for responsible AI tool development. The vulnerability caused data uploads to xAI's Google Cloud buckets; xAI stated that all retained data was deleted and retention is now disabled by default. The codebase is written in Rust with 844,530 lines of code, and includes a self-contained terminal renderer for Mermaid diagrams.

rss · Simon Willison · Jul 15, 23:59

**Background**: The Grok CLI is a terminal-based AI coding agent developed by xAI, powered by Grok 4.5. It allows developers to interact with AI for coding tasks, but the default behavior of uploading entire directories exposed users to serious privacy risks. Open-sourcing the codebase allows independent auditing and local-first usage.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xai-org/grok-build">GitHub - xai - org / grok - build : SpaceXAI's coding agent harness and...</a></li>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://x.ai/open-source">Open Source: Grok Build Coding Agent & CLI | SpaceXAI</a></li>

</ul>
</details>

**Discussion**: No community comments were directly provided, but the news report describes severe backlash from users who reported uploading SSH keys, password databases, and other sensitive files. The incident prompted xAI to disable the feature and delete retained data.

**Tags**: `#privacy`, `#open-source`, `#AI`, `#CLI`, `#xAI`

---

<a id="item-8"></a>
## [Claude web_fetch tool tricked into leaking private memories](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Researcher Ayush Paul discovered a method to bypass Claude's web_fetch tool protections, allowing data exfiltration of user memories by crafting a honeypot website that leads the agent to follow nested links. The attack successfully extracted the user's name, city, and employer. This vulnerability highlights ongoing security challenges in AI agents that combine private data access with web browsing capabilities. It demonstrates that even carefully designed protections can be circumvented, emphasizing the need for robust isolation and input validation. The attack exploited a loophole where web_fetch could navigate to URLs embedded in previously fetched pages, creating a chain of requests that ultimately exfiltrated data. Anthropic declined a bug bounty, stating they had already identified the issue internally, and subsequently closed the hole by preventing web_fetch from following links returned in fetched content.

rss · Simon Willison · Jul 15, 14:21

**Background**: The "lethal trifecta" refers to the combination of private data access, untrusted content, and exfiltration capability that makes LLM agents vulnerable to data theft. Claude's web_fetch tool is designed to only fetch URLs explicitly provided by the user or returned from its companion web_search tool, but the loophole allowed following links from fetched pages, enabling the attack.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.claude.com/en/docs/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Docs</a></li>
<li><a href="https://www.cyera.com/research/when-language-becomes-the-attack-vector-the-lethal-trifecta-of-ai-agents">When Language Becomes the Attack Vector: The Lethal Trifecta of AI...</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI safety`, `#prompt injection`, `#data exfiltration`, `#Claude`

---

<a id="item-9"></a>
## [LM Studio Launches Bionic: AI Agent for Open Models](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 7.0/10

LM Studio has introduced Bionic, an AI agent designed to perform tasks such as coding, research, and document manipulation using open models, available both locally and via the LM Studio Secure Cloud. This marks LM Studio's expansion from a simple chat interface to a full-fledged agent platform, potentially making powerful open models more accessible for enterprise use cases while addressing data security concerns. Bionic offers specialized project types: 'Code' for coding tasks and 'Work' for document creation/manipulation with automatic checkpointing. It also connects to frontier open models like GLM 5.2, Kimi K2.6, and Kimi Coder K2.7 via cloud.

hackernews · minimaxir · Jul 16, 20:18 · [Discussion](https://news.ycombinator.com/item?id=48939662)

**Background**: LM Studio is a desktop application that allows users to run open-source large language models locally on their own computers without needing cloud services. It has been popular among developers and AI enthusiasts for its ease of use. Bionic represents a new product direction, transforming LM Studio from a chat tool into an agentic platform capable of executing complex workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://lmstudio.ai/blog/introducing-lm-studio-bionic">Introducing LM Studio Bionic : the AI agent for open models</a></li>
<li><a href="https://9to5mac.com/2026/07/16/lm-studio-expands-beyond-chat-with-bionic-a-new-ai-agent-app-for-open-models/">LM Studio launches Bionic , a new AI agent app for open... - 9to5Mac</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed. Some users express concern about the shift in business model from free local usage to a cloud-dependent enterprise offering, while others question the value proposition compared to existing tools. The founder, Yagil, invites users to try Bionic with free credits, emphasizing its document handling capabilities.

**Tags**: `#AI agent`, `#open source models`, `#local LLM`, `#LM Studio`, `#enterprise`

---

<a id="item-10"></a>
## [Microsoft open-sources Comic Chat, nostalgic IRC client](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 7.0/10

On July 16, 2026, Microsoft released the source code of Comic Chat (later known as Microsoft Chat), a graphical IRC client from 1996, as open source under a permissive license. This release preserves a piece of early internet history and demonstrates Microsoft's continued commitment to open source. It allows developers and enthusiasts to study, modify, and run the software on modern systems, sparking nostalgia and educational interest. The original developer was David Kurlander of Microsoft Research; the open-sourcing effort was led by Robert Standefer with support from Scott Hanselman. Comic Chat extended the IRC protocol with custom commands for character appearance and actions.

hackernews · jervant · Jul 16, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48936426)

**Background**: Microsoft Comic Chat, first released with Internet Explorer 3.0 in 1996, automatically converted text-based IRC conversations into comic strips with characters and speech bubbles. It was later renamed Microsoft Chat and bundled with Windows 98, but fell out of use as modern instant messaging emerged.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Comic_Chat">Microsoft Comic Chat</a></li>
<li><a href="https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/">Microsoft Comic Chat is now open source | Microsoft Open Source...</a></li>

</ul>
</details>

**Discussion**: Comments express strong nostalgia and gratitude for the open-sourcing. Robert Standefer shared the backstory, and Jeremy Herrman noted it inspired his first startup. Some users recalled that Comic Chat was disliked on IRC due to its non-standard protocol extensions.

**Tags**: `#open-source`, `#microsoft`, `#irc`, `#nostalgia`, `#history`

---

<a id="item-11"></a>
## [Classical ML for LLM Text Detection](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 7.0/10

A blog post explores using classical machine learning classifiers, such as support vector machines and random forests, to detect whether a text was generated by an LLM. The author describes training a classifier based on features like perplexity and burstiness, achieving moderate accuracy on a small dataset. If classical ML can reliably detect LLM-generated text, it could provide a lightweight, privacy-preserving alternative to large neural detectors, potentially usable in browser extensions. However, the community remains skeptical about the fundamental feasibility of detecting LLM texts due to the lack of inherent provenance signals. The classifier is small enough that the author wonders if a similar English model could run as a browser extension against every paragraph. The approach relies on statistical tells that may change as LLMs improve, raising questions about long-term robustness.

hackernews · uneven9434 · Jul 16, 16:41 · [Discussion](https://news.ycombinator.com/item?id=48936880)

**Background**: LLM-generated text detection is an active area of research, with methods including watermarking, statistical analysis, and deep learning classifiers. Classical machine learning approaches like SVM and Random Forest use handcrafted features, such as perplexity (how surprising the text is to a language model) and burstiness (variation in word frequency), to distinguish human from machine writing. The reliability of detection is disputed, as texts are not information-dense enough to carry a reliable provenance signal.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/better-programming/detecting-llm-generated-texts-befce4426da9">Detecting LLM - Generated Texts . Is it possible to differentiate between</a></li>
<li><a href="https://arxiv.org/pdf/2303.07205">The Science of Detecting LLM - Generated Texts</a></li>

</ul>
</details>

**Discussion**: Commenters express strong skepticism: akersten likens detection to "tarot card reading," and docheinestages argues that measuring effort in writing is more viable than detecting AI origin. Krssst finds potential in a browser extension, while connorboyle points out a translation issue in the article where "faked" might be too strong a rendering of the original Chinese. Overall, the sentiment leans toward detection being a losing battle.

**Tags**: `#LLM`, `#AI detection`, `#machine learning`, `#text classification`, `#blog`

---

<a id="item-12"></a>
## [OnePlus halts new product launches in Europe and North America](https://community.oneplus.com/thread/2170715118587871237) ⭐️ 7.0/10

OnePlus announced it will stop launching new products in Europe and North America, although it will continue to support existing devices with software updates and security patches. This strategic shift marks a significant retreat from key global markets for a major smartphone brand, potentially affecting consumer choice and competition in those regions. The decision does not affect existing devices, which will continue to receive software updates and security patches as originally committed; OnePlus's parent company OPPO will back the support.

hackernews · pilililo2 · Jul 16, 10:14 · [Discussion](https://news.ycombinator.com/item?id=48932539)

**Background**: OnePlus was founded in 2013 as a subsidiary of OPPO, focusing on high-spec, affordable smartphones with near-stock Android. It gained popularity among enthusiasts for its 'Never Settle' ethos, unlocked bootloaders, and competitive pricing. In recent years, the brand has faced challenges including cultural shifts, reduced differentiation, and market consolidation.

**Discussion**: Community members corrected the misleading title, emphasizing that OnePlus is not halting all operations but only new product launches. Some lamented the brand's decline from its hacker-friendly roots, while others noted that existing devices remain well-supported and praised recent models like the OnePlus 13 and 15 for their battery life.

**Tags**: `#OnePlus`, `#smartphone industry`, `#market withdrawal`, `#tech news`

---

<a id="item-13"></a>
## [Immersive Linear Algebra Book with Interactive 3D Figures (2015)](https://immersivemath.com/ila/) ⭐️ 7.0/10

An online linear algebra book called 'Immersive Linear Algebra' uses interactive 3D figures to help visualize concepts. It was released in 2015 and remains a popular educational resource. This book makes linear algebra more intuitive by allowing readers to manipulate 3D visualizations directly, which can improve understanding for students. It represents a step forward in math education by combining interactivity with traditional textbook content. The book covers standard linear algebra topics such as vectors, matrices, and eigenvalues, with embedded figures that can be rotated and zoomed. The presentation is clean and includes tooltips for additional explanations.

hackernews · srean · Jul 16, 15:32 · [Discussion](https://news.ycombinator.com/item?id=48935951)

**Background**: Linear algebra is a foundational topic in mathematics and computer science, but its abstract concepts can be hard to grasp. Traditional textbooks rely on static 2D diagrams, which limit the ability to show multidimensional relationships. Interactive figures address this by letting students explore concepts from multiple angles.

**Discussion**: The community response is overwhelmingly positive. Commenters praise the book's clarity and interactivity, with one noting they wish such resources existed when they were studying. Some suggest expanding the approach to other subjects like statistics and robotics, while others see potential for AI-enhanced features like 'explain this' popups.

**Tags**: `#linear algebra`, `#interactive learning`, `#mathematics education`, `#educational technology`, `#book`

---

<a id="item-14"></a>
## [Google Rebrands NotebookLM to Gemini Notebook](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook/) ⭐️ 6.0/10

Google has rebranded NotebookLM as Gemini Notebook, aligning the AI note-taking and research tool with its Gemini brand family. The name change aims to simplify branding and reflect deeper integration with Google's Gemini AI models. This rebranding signals Google's strategic push to unify its AI products under the Gemini umbrella, potentially improving user recognition and trust. However, it may also cause confusion among existing users and sparks debates about the product's direction versus competitors like ChatGPT. NotebookLM, known for its Audio Overviews and research features, now runs on Gemini 3.5 models as of June 2026. The rebranding does not introduce new features immediately, but aligns the tool with Google's broader AI ecosystem.

hackernews · xnx · Jul 16, 16:08 · [Discussion](https://news.ycombinator.com/item?id=48936451)

**Background**: NotebookLM (now Gemini Notebook) is an AI-powered research and note-taking tool from Google Labs that uses retrieval-augmented generation to help users interact with documents. It gained popularity for generating podcast-like Audio Overviews and video summaries. The rebranding reflects Google's effort to consolidate its AI offerings under the Gemini brand, which also includes Gemini chat and other services.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NotebookLM">NotebookLM</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some users welcome the clearer branding, while others express disappointment that no major improvements accompanied the rename. Several users share their own workarounds or alternative tools, such as using ChatGPT Live for audio learning or building custom solutions like Notebooker.ai.

**Tags**: `#NotebookLM`, `#Gemini`, `#Google`, `#AI`, `#rebranding`

---

<a id="item-15"></a>
## [WebAssembly tool converts Mermaid diagrams to Unicode box art](https://simonwillison.net/2026/Jul/16/grok-mermaid/#atom-everything) ⭐️ 6.0/10

Simon Willison created a WebAssembly-based tool called grok-mermaid that converts Mermaid diagrams into Unicode box art, running entirely in the browser. It ports a Rust terminal renderer from the open-sourced Grok CLI codebase. This demonstrates how WebAssembly enables creative reuse of Rust terminal tools in the browser, making them accessible without installation. It also provides a lightweight, text-based way to view Mermaid diagrams in environments without native rendering support. The tool compiles the Rust Mermaid renderer to WebAssembly, then uses Unicode box-drawing characters to draw the diagram on a canvas. It includes controls for adjusting maximum width, copying the diagram as plain text, and generating a shareable link.

rss · Simon Willison · Jul 16, 00:33

**Background**: Mermaid is a popular JavaScript-based tool that defines diagrams using plain text syntax. Unicode box-drawing characters are a set of symbols in the Unicode standard that can be used to create simple, text-based boxes and lines. WebAssembly allows code written in languages like Rust to run in the browser at near-native speed, enabling porting of command-line tools to web applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Box-drawing_characters">Box-drawing characters - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/WebAssembly/Guides/Rust_to_Wasm">Compiling from Rust to WebAssembly - WebAssembly | MDN</a></li>
<li><a href="https://rust-lang.org/what/wasm/">WebAssembly - Rust Programming Language</a></li>

</ul>
</details>

**Tags**: `#Mermaid`, `#Unicode`, `#WebAssembly`, `#tool`, `#Rust`

---