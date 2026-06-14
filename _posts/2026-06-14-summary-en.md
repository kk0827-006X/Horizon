---
layout: default
title: "Horizon Summary: 2026-06-14 (EN)"
date: 2026-06-14
lang: en
---

> From 49 items, 13 important content pieces were selected

---

1. [vLLM v0.23.0 Boosts DeepSeek-V4 and Expands Model Runner V2](#item-1) ⭐️ 9.0/10
2. [Census Bureau Bans Noise Infusion in Statistical Products](#item-2) ⭐️ 9.0/10
3. [Police officer investigated for using AI to 'create evidence'](#item-3) ⭐️ 9.0/10
4. [US Government Orders Suspension of Anthropic's Fable 5 and Mythos 5](#item-4) ⭐️ 9.0/10
5. [GLM-5.2: Fully Open Frontier Model Released by Z.ai](#item-5) ⭐️ 8.0/10
6. [Pancreatic tumor treatment may reveal cancer's master switch](#item-6) ⭐️ 8.0/10
7. [Google proposes using retired phones as low-carbon computing platform](#item-7) ⭐️ 8.0/10
8. [Arabic Text Rendering: Technical Debt and User Struggles](#item-8) ⭐️ 8.0/10
9. [Pyodide 314.0 Enables Publishing WASM Wheels to PyPI](#item-9) ⭐️ 8.0/10
10. [Blog Post Demands Perfect UI Animation in Every Frame](#item-10) ⭐️ 7.0/10
11. [RTX 5080 + RTX 3090 Combo Hits 80 Tok/s on Qwen 3.6 27B Q8](#item-11) ⭐️ 7.0/10
12. [OpenAI WebRTC Audio Session Gets Document Context and GPT-Realtime-2](#item-12) ⭐️ 6.0/10
13. [AI Could Disrupt Half of Entry-Level White-Collar Jobs](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [vLLM v0.23.0 Boosts DeepSeek-V4 and Expands Model Runner V2](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 9.0/10

vLLM v0.23.0 was released with 408 commits from 200 contributors, significantly maturing DeepSeek-V4 support across backends and making Model Runner V2 the default for Llama and Mistral dense models. This release brings critical optimizations for the widely-used DeepSeek-V4 MoE model and extends performance enhancements to popular dense models like Llama and Mistral, directly benefiting thousands of vLLM users in production inference. Key technical highlights include decoupled sparse MLA metadata for DeepSeek-V4, a TRTLLM-gen attention kernel, EPLB support for Mega-MoE, selective prefix-cache retention, and Model Runner V2 gaining FlashInfer sampler and breakable CUDA graphs.

github · khluu · Jun 12, 23:29

**Background**: vLLM is a high-throughput, memory-efficient inference engine for large language models. DeepSeek-V4 is a Mixture-of-Experts (MoE) architecture that uses Multi-Latent Attention (MLA) to reduce KV cache memory consumption. Model Runner V2 is a new execution path that eliminates pipeline-parallel bubbles and supports advanced features like breakable CUDA graphs for better GPU utilization.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/deepseek_v4/sparse_mla/">sparse_mla - vLLM</a></li>
<li><a href="https://deepwiki.com/NVIDIA/TensorRT-LLM/9.2-trtllm-attention-backend">TRTLLM Attention Backend | NVIDIA/TensorRT-LLM | DeepWiki</a></li>
<li><a href="https://github.com/vllm-project/vllm/issues/20468">[Feature]: Support EPLB for More MoE Models, e.g. Qwen 3, Llama 4 · Issue #20468 · vllm-project/vllm</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#llm-inference`, `#deepseek`, `#optimization`, `#release`

---

<a id="item-2"></a>
## [Census Bureau Bans Noise Infusion in Statistical Products](https://desfontain.es/blog/banning-noise.html) ⭐️ 9.0/10

The U.S. Department of Commerce issued an order banning noise infusion (a differential privacy technique) from all statistical products published by the Census Bureau and the Bureau of Economic Analysis. This policy removes a key privacy protection mechanism for individual data in official statistics, increasing re-identification risks and affecting trust in government data. Noise infusion adds calibrated random noise to statistical outputs to achieve differential privacy; the order specifically prohibits this method, which had been used in recent Census Bureau products.

hackernews · nl · Jun 13, 13:54 · [Discussion](https://news.ycombinator.com/item?id=48517377)

**Background**: Differential privacy is a mathematical framework that ensures individual privacy by limiting what can be inferred from released statistics. The Census Bureau had adopted noise infusion for products like the 2020 Census, but critics argued it reduced data utility. The ban represents a shift toward prioritizing accuracy over formal privacy guarantees.

<details><summary>References</summary>
<ul>
<li><a href="https://desfontain.es/blog/banning-noise.html">Banning noise will be a disaster for statistical data ...</a></li>
<li><a href="https://www.bea.gov/help/faq/1490">Why didn’t BEA use noise infusion as its statistical ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Differential_privacy">Differential privacy</a></li>

</ul>
</details>

**Discussion**: Comments reflect deep divisions: enumerators express concern about loss of trust and increased risk of data misuse, while others argue differential privacy is necessary to protect individuals. Some note grassroots political pressure against DP, citing examples of state-level opposition.

**Tags**: `#differential privacy`, `#census`, `#data privacy`, `#government statistics`, `#policy`

---

<a id="item-3"></a>
## [Police officer investigated for using AI to 'create evidence'](https://news.sky.com/story/derbyshire-police-officer-investigated-for-using-ai-to-create-evidence-in-multiple-cases-13553661) ⭐️ 9.0/10

A Derbyshire police officer is under investigation for allegedly using artificial intelligence to create or falsify evidential material in multiple cases. This case highlights the emerging risk of AI misuse in law enforcement, potentially undermining the integrity of evidence and public trust in the justice system. The specific nature of the AI-generated evidence has not been disclosed, but it could involve image enhancement, deepfake creation, or falsified witness statements.

hackernews · austinallegro · Jun 13, 19:54 · [Discussion](https://news.ycombinator.com/item?id=48520807)

**Background**: Deepfakes are synthetic media generated by AI that can depict realistic but fabricated events. Courts are still developing standards for authenticating AI-generated evidence, raising concerns about reliability and due process.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thomsonreuters.com/en-us/posts/ai-in-courts/deepfakes-evidence-authentication/">Deepfakes on trial: How judges are navigating AI evidence authentication - Thomson Reuters Institute</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deepfake">Deepfake - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments express outrage over evidence tampering and question how many people may have been unjustly convicted due to fabricated or enhanced evidence. Some speculate that the officer may have used AI to 'enhance' blurry images, which is still unacceptable.

**Tags**: `#AI ethics`, `#legal evidence`, `#police misconduct`, `#technology misuse`

---

<a id="item-4"></a>
## [US Government Orders Suspension of Anthropic's Fable 5 and Mythos 5](https://simonwillison.net/2026/Jun/13/us-government-directive-to-suspend-access/#atom-everything) ⭐️ 9.0/10

On June 12, 2026, the US government issued an export control directive requiring Anthropic to immediately suspend access to its Fable 5 and Mythos 5 AI models for all customers, including foreign national employees, citing national security concerns over a reported jailbreak vulnerability. Anthropic complied, and the models were disabled within hours. This event marks a significant escalation in government intervention over AI safety, setting a precedent for national security-based shutdowns of advanced AI models. It raises critical questions about regulatory overreach, the balance between security and openness, and the future of AI model deployment. The government's directive did not provide specific details of the national security concern; Anthropic stated that the alleged jailbreak technique is simple and replicable on other models like GPT-5.5. Access to Fable 5 was cut off at 6:59 PM Pacific on June 12.

rss · Simon Willison · Jun 13, 01:01

**Background**: Jailbreaking AI models involves crafting adversarial inputs to bypass built-in safety constraints, causing the model to generate content it was trained to refuse. Fable 5 was a recently released frontier model by Anthropic, known for its autonomous capabilities in software engineering and knowledge work. The US government has export control authorities over AI models deemed national security risks, which previously were mainly used to restrict chip exports rather than model access.

<details><summary>References</summary>
<ul>
<li><a href="https://aisecurityandsafety.org/en/guides/jailbreaking-attacks/">Jailbreaking AI Models: Attack Patterns, Examples & Defenses ...</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Commenters expressed confusion about why this specific jailbreak prompted government action, with some speculating about Amazon's involvement as a government contractor. Others noted that Fable 5 was designed to resist exploitation, while some argued that all LLMs are jailbreakable and questioned the lack of transparency in the directive.

**Tags**: `#AI regulation`, `#national security`, `#jailbreaking`, `#Anthropic`, `#export control`

---

<a id="item-5"></a>
## [GLM-5.2: Fully Open Frontier Model Released by Z.ai](https://twitter.com/jietang/status/2065784751345287314) ⭐️ 8.0/10

Zhipu AI (Z.ai) released GLM-5.2, a fully open-weight frontier AI model, in late July 2025. The release emphasizes unrestricted access to advanced AI capabilities. GLM-5.2's open release contrasts with recent US restrictions on models like Fable, highlighting a geopolitical divide in AI accessibility. It provides a permissively licensed alternative that can be used by researchers and developers globally without barriers. The model was released without an official benchmark blog post yet, but community discussions note the timing coincides with a US government letter to Anthropic restricting Fable. GLM-5.2 is an open-weight model, meaning its parameters are publicly available for fine-tuning and deployment.

hackernews · aloknnikhil · Jun 13, 16:18 · [Discussion](https://news.ycombinator.com/item?id=48518684)

**Background**: GLM is a series of large language models developed by Zhipu AI (Z.ai), a leading Chinese AI lab. Previous versions like GLM-4.5 used Mixture-of-Experts architecture. The release of GLM-5.2 continues Z.ai's tradition of open-sourcing their models, which is seen as a counterpoint to increasingly restrictive US AI policies.

<details><summary>References</summary>
<ul>
<li><a href="https://glm5.net/">GLM-5 | Zhipu AI's Next-Generation Large Language Model</a></li>
<li><a href="https://z.ai/blog/glm-4.5">GLM-4.5: Reasoning, Coding, and Agentic Abililties - z.ai</a></li>

</ul>
</details>

**Discussion**: Community members praised the open release, with some noting it reads like fiction that Chinese labs are releasing open models while the US censors them. Others highlighted the precise timing with the US government's action against Fable, and expressed gratitude for permissive licensing.

**Tags**: `#GLM`, `#AI`, `#Open Source`, `#Geopolitics`, `#Machine Learning`

---

<a id="item-6"></a>
## [Pancreatic tumor treatment may reveal cancer's master switch](https://economist.com/science-and-technology/2026/06/12/treating-pancreatic-tumours-may-have-revealed-cancers-master-switch) ⭐️ 8.0/10

A new treatment approach targeting pancreatic tumors has potentially uncovered a key vulnerability in cancers driven by KRAS mutations, a target previously considered undruggable. This discovery matters because KRAS mutations are present in about 25% of all tumors, including hard-to-treat cancers like pancreatic, lung, and colorectal cancer, and successfully targeting them could lead to effective treatments for millions of patients. The breakthrough applies to approximately 20% of cancers, not all, as noted in community discussion; recent advancements in biologics design have made it possible to tackle previously undruggable targets like KRAS.

hackernews · andsoitis · Jun 13, 13:34 · [Discussion](https://news.ycombinator.com/item?id=48517199)

**Background**: KRAS is a gene that produces a protein involved in cell signaling and growth. Mutations in KRAS can cause uncontrolled cell growth, leading to cancer. For decades, KRAS was considered undruggable because its smooth surface and high affinity for GTP made it difficult to inhibit with conventional drugs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KRAS">KRAS - Wikipedia</a></li>
<li><a href="https://www.mdanderson.org/cancerwise/targeting-the-kras-mutation-for-more-effective-cancer-treatment.h00-159458478.html">Targeting the KRAS mutation for more effective cancer treatment | UT MD Anderson</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11899378/">KRAS Mutations in Cancer: Understanding Signaling Pathways to Immune Regulation and the Potential of Immunotherapy - PMC</a></li>

</ul>
</details>

**Discussion**: Commenters noted the hyperbolic title, clarifying that the discovery applies to about 20% of tumors, but still represents a significant step forward. One user highlighted that targeting KRAS was previously considered impossible, and this breakthrough broadens the horizon for future treatments.

**Tags**: `#cancer`, `#pancreatic cancer`, `#KRAS`, `#drug discovery`, `#medical research`

---

<a id="item-7"></a>
## [Google proposes using retired phones as low-carbon computing platform](https://research.google/blog/a-low-carbon-computing-platform-from-your-retired-phones/) ⭐️ 8.0/10

Google Research has proposed using retired smartphones as a low-carbon computing platform for edge computing tasks, repurposing e-waste into a distributed server network. If successful, this approach could significantly reduce e-waste and carbon footprint by extending the life of mobile hardware, while also providing affordable computing resources for edge applications. The proposal treats each phone as a weak server akin to a Raspberry Pi, but faces challenges from locked bootloaders, proprietary firmware, and limited security update lifespans from OEMs.

hackernews · vikas-sharma · Jun 13, 09:38 · [Discussion](https://news.ycombinator.com/item?id=48515336)

**Background**: Edge computing processes data near its source rather than in central data centers, reducing latency and bandwidth use. E-waste from retired phones is a growing environmental problem, as phones contain valuable materials but are often discarded due to lack of software support.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Edge_computing">Edge computing</a></li>

</ul>
</details>

**Discussion**: Commenters expressed enthusiasm for repurposing hardware but emphasized security risks from outdated software and locked-down devices. Some called for regulations to require unlockable bootloaders, while others noted that current Android phones are far easier to repurpose than iPhones.

**Tags**: `#sustainability`, `#edge computing`, `#e-waste`, `#Android`, `#cloud computing`

---

<a id="item-8"></a>
## [Arabic Text Rendering: Technical Debt and User Struggles](https://lr0.org/blog/p/arabic/) ⭐️ 8.0/10

A detailed blog post explores the systemic technical debt in rendering Arabic script in text editors, exposing flaws in bidirectional text algorithms and font shaping that cause daily user frustration. This matters because Arabic script is used by hundreds of millions of people, yet poor rendering support creates significant productivity loss and cognitive burden, highlighting a blind spot in internationalization efforts. The post describes how the Unicode Bidirectional Algorithm and OpenType shaping features like 'init', 'medi', 'fina', and 'isol' are inadequately implemented, leading to cursor misbehavior and text corruption in mixed English-Arabic emails.

hackernews · bookofjoe · Jun 13, 12:40 · [Discussion](https://news.ycombinator.com/item?id=48516710)

**Background**: Arabic script requires contextual shaping: letters change form based on position (isolated, initial, medial, final). Additionally, Arabic is written right-to-left but often mixed with left-to-right text, requiring the Unicode Bidirectional Algorithm. The OpenType font format provides shaping features for Arabic, but many text editors and systems have incomplete support, leading to technical debt accumulated over years of expedient implementations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bidirectional_text">Bidirectional text - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/typography/script-development/arabic">Developing OpenType Fonts for Arabic Script - Typography Arabic Script Shaping | harfbuzz/harfrust | DeepWiki Arabic Script Resources - World Wide Web Consortium (W3C) Deficiencies of Handling Arabic Script in OpenType (and Some ... Application Support - Arabic Fonts</a></li>
<li><a href="https://en.wikipedia.org/wiki/Technical_debt">Technical debt - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed empathy for Arabic users, with one sharing a vivid anecdote about engineers abandoning mixed-language emails. Another noted the beauty of Arabic script and compared the complexity to English layout. There were also links to academic treatments and alternative disconnected fonts.

**Tags**: `#typography`, `#internationalization`, `#Arabic script`, `#text rendering`, `#technical debt`

---

<a id="item-9"></a>
## [Pyodide 314.0 Enables Publishing WASM Wheels to PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 8.0/10

Pyodide 314.0, released in June 2026, now allows Python packages compiled as WebAssembly wheels to be published directly to PyPI and installed at runtime using micropip, removing the previous need for central hosting by the Pyodide maintainers. This change dramatically reduces the maintenance burden on Pyodide maintainers and removes a major bottleneck for the community, enabling any package author to distribute WASM-compiled Python packages via the standard PyPI infrastructure. The new platform tag 'pyemscripten' defined in PEP 783 is used for these wheels, and cibuildwheel supports building them. A canonical example is the luau-wasm package, which embeds the Luau compiler as a CPython extension compiled to WebAssembly.

rss · Simon Willison · Jun 13, 23:55

**Background**: Pyodide is a Python distribution for browsers and Node.js based on WebAssembly. Previously, over 300 packages had to be built and hosted manually by the Pyodide core team. PEP 783 standardized the Emscripten platform tag, enabling this new workflow. WebAssembly allows compiled code to run in browsers at near-native speed.

<details><summary>References</summary>
<ul>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging | peps.python.org</a></li>

</ul>
</details>

**Tags**: `#Pyodide`, `#WebAssembly`, `#Python`, `#PyPI`, `#WASM`

---

<a id="item-10"></a>
## [Blog Post Demands Perfect UI Animation in Every Frame](https://tonsky.me/blog/every-frame-perfect/) ⭐️ 7.0/10

A blog post titled 'Every Frame Perfect' by developer Nikita Prokopov argues that UI animations should be flawless in every single frame, criticizing examples from macOS where animations show glitchy or imperfect frames. The article challenges the common practice in computer graphics of exploiting human visual perception limits to save resources, sparking debate among developers and designers about the right balance between animation quality and performance. The author provides specific macOS examples, including the save dialog shaking, Notes app buttons jumping, and Safari address bar animation glitches, claiming that even a single 'wrong' frame degrades user experience.

hackernews · ravenical · Jun 13, 11:40 · [Discussion](https://news.ycombinator.com/item?id=48516251)

**Background**: The human visual system can perceive motion with as little as 3–6 milliseconds of visual stimulation. In animation, each frame can be a perfect instant (no motion blur) or include simulated motion blur to make motion appear smoother. The debate centers on whether UI animations should prioritize frame perfection or lean on perceptual tricks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Motion_blur_(media)">Motion blur (media) - Wikipedia</a></li>
<li><a href="https://www.mdpi.com/2411-5150/3/1/5">Temporal Limits of Visual Motion Processing: Psychophysics ...</a></li>

</ul>
</details>

**Discussion**: Commenters have mixed reactions: some agree that the examples shown are bad but disagree with the strict premise of requiring every frame to be perfect, arguing that graphics often exploit perceptual limits. Others call the argument weak and note that the author doesn't provide superior alternatives.

**Tags**: `#UI/UX`, `#animation`, `#macOS`, `#software design`, `#human perception`

---

<a id="item-11"></a>
## [RTX 5080 + RTX 3090 Combo Hits 80 Tok/s on Qwen 3.6 27B Q8](https://imil.net/blog/posts/2026/rtx-5080-+-rtx-3090-setup-80+-tok-s-on-qwen-3.6-27b-q8/) ⭐️ 7.0/10

A user demonstrated a local inference setup combining an RTX 5080 and an RTX 3090 to run Qwen 3.6 27B in Q8 quantization at 80 tokens per second. This benchmark shows that high-throughput local LLM inference is achievable on relatively affordable consumer GPUs, potentially reducing reliance on cloud services for AI tasks. The setup uses a two-GPU configuration with llama.cpp or similar software, and the 80 tokens/s performance is for the Q8 quantized version of the 27B parameter model, which balances quality and speed.

hackernews · iMil · Jun 13, 09:55 · [Discussion](https://news.ycombinator.com/item?id=48515454)

**Background**: Large language models (LLMs) like Qwen 3.6 27B typically require significant VRAM; quantization reduces model precision (e.g., Q8 uses 8-bit weights) to fit on consumer GPUs. The RTX 5080 (16GB VRAM) and RTX 3090 (24GB VRAM) together provide 40GB, sufficient for the 27B Q8 model with overhead.

<details><summary>References</summary>
<ul>
<li><a href="https://qwen.ai/blog?id=qwen3.6-27b">Qwen3.6-27B: Flagship-Level Coding in a 27B Dense Model</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-27B">Qwen/Qwen3.6-27B · Hugging Face</a></li>
<li><a href="https://mljourney.com/quantized-llms-explained-q4-vs-q8-vs-fp16/">Quantized LLMs Explained: Q4 vs Q8 vs FP16 - ML Journey</a></li>

</ul>
</details>

**Discussion**: Users shared optimization hints (e.g., temperature, top-p, MTP settings) and compared performance; one user with a 4090 and Tenstorrent cards only got 30 tps, noting electricity costs in California make cloud cheaper. Another suggested a $25 Oculink card for multi-GPU setups.

**Tags**: `#LLM inference`, `#GPU optimization`, `#local AI`, `#Qwen`, `#token throughput`

---

<a id="item-12"></a>
## [OpenAI WebRTC Audio Session Gets Document Context and GPT-Realtime-2](https://simonwillison.net/2026/Jun/12/openai-webrtc/#atom-everything) ⭐️ 6.0/10

Simon Willison updated his OpenAI WebRTC Audio Session tool to support document context pasting and the new GPT-Realtime-2 model, enabling users to have audio conversations about pasted documents. This update bridges a gap by allowing developers to explore documents through voice conversations with a state-of-the-art reasoning model, potentially improving productivity and accessibility for users who prefer audio interaction. The tool now includes a collapsible 'Document context' section where users can paste text before starting a session; the model selected is GPT-Realtime-2, which OpenAI describes as its first voice model with GPT-5-class reasoning and a knowledge cutoff of September 30, 2024.

rss · Simon Willison · Jun 12, 23:53

**Background**: OpenAI's Realtime API allows low-latency, interactive voice applications using WebRTC, a standard for real-time communication. GPT-Realtime-2 is a speech-to-speech model introduced in May 2026 that enhances reasoning and instruction following. Simon Willison's tool is a browser-based playground that demonstrates this API, now upgraded to include document context for more practical use cases.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.openai.com/docs/guides/realtime-webrtc">Realtime API with WebRTC | OpenAI API</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-realtime-2">GPT-Realtime-2 Model | OpenAI API</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#WebRTC`, `#audio`, `#AI`, `#tool`

---

<a id="item-13"></a>
## [AI Could Disrupt Half of Entry-Level White-Collar Jobs](https://www.investing.com/news/economy-news/what-if-ai-really-does-disrupt-50-of-all-entrylevel-whitecollar-jobs-4741043) ⭐️ 6.0/10

A news article speculates that artificial intelligence could disrupt up to 50% of entry-level white-collar jobs, citing potential automation of routine tasks such as data processing and report generation. This prediction highlights a significant shift in the labor market, potentially reducing entry-level opportunities for recent graduates and increasing demand for advanced skills. The article is speculative and does not provide concrete data or expert interviews; it focuses on the vulnerability of repetitive administrative and analytical tasks to AI automation.

rss · Investing.com All News · Jun 13, 19:45

**Background**: Entry-level white-collar jobs often involve routine tasks like data entry, scheduling, and basic analysis. AI systems, particularly large language models and robotic process automation, have shown capability in performing these tasks with increasing accuracy, leading to concerns about job displacement in sectors like finance, customer service, and legal support.

**Tags**: `#AI`, `#job displacement`, `#economics`, `#white-collar jobs`

---