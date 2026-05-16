---
layout: default
title: "Horizon Summary: 2026-05-16 (EN)"
date: 2026-05-16
lang: en
---

> From 47 items, 15 important content pieces were selected

---

1. [vLLM v0.21.0: Major Update with Breaking Changes and Performance Boost](#item-1) ⭐️ 9.0/10
2. [Google Project Zero Discloses 0-Click Exploit for Pixel 10](#item-2) ⭐️ 9.0/10
3. [Zulip transitions to nonprofit foundation](#item-3) ⭐️ 8.0/10
4. [Sigmoid curve challenges AI's Lindy effect assumption](#item-4) ⭐️ 8.0/10
5. [DOJ demands Apple and Google unmask 100k users of emissions-bypass app](#item-5) ⭐️ 8.0/10
6. [Waymo Recalls 3,800 Robotaxis Over Standing Water Glitch](#item-6) ⭐️ 8.0/10
7. [FiveThirtyEight Articles Removed by ABC News](#item-7) ⭐️ 8.0/10
8. [Coding agents reduce technology lock-in risks](#item-8) ⭐️ 8.0/10
9. [MitchellH warns companies suffer from AI psychosis](#item-9) ⭐️ 7.0/10
10. [California bill targets game shutdown refunds](#item-10) ⭐️ 7.0/10
11. [Explore Wikipedia via a Windows XP Desktop Interface](#item-11) ⭐️ 7.0/10
12. [Image-blaster: single image to 3D environments and meshes](#item-12) ⭐️ 7.0/10
13. [O(x)Caml in Space: Stack Allocation Boosts Satellite Software](#item-13) ⭐️ 7.0/10
14. [In-Browser Neural Net Learns to Play Snake via PPO](#item-14) ⭐️ 7.0/10
15. [Mitchell Hashimoto: Languages Are Becoming Fungible](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [vLLM v0.21.0: Major Update with Breaking Changes and Performance Boost](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 9.0/10

vLLM v0.21.0 deprecates transformers v4 support, requires C++20, integrates KV offloading with the Hybrid Memory Allocator, and introduces speculative decoding with thinking budget support for reasoning models. This release significantly improves inference efficiency for hybrid and reasoning models, and expands support for Blackwell GPUs, making it a critical update for production deployments. Key technical details include the new TOKENSPEED_MLA attention backend for Blackwell GPUs optimized for MLA models like DeepSeek-R1, and the integration of KV offloading with Hybrid Memory Allocator enabling sliding window group support and per-job store completion.

github · khluu · May 15, 08:44

**Background**: vLLM is an open-source library for high-throughput LLM inference. Speculative decoding accelerates generation by having a draft model propose multiple tokens that the target model verifies in parallel. The Hybrid Memory Allocator optimizes KV cache memory for models with different layer types, reducing waste. Blackwell is NVIDIA's next-generation GPU architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency in AI Inference | NVIDIA Technical Blog</a></li>
<li><a href="https://github.com/vllm-project/vllm/issues/11382">[RFC]: Hybrid Memory Allocator · Issue #11382 · vllm-project/vllm</a></li>
<li><a href="https://pytorch.org/blog/hybrid-models-as-first-class-citizens-in-vllm/">Hybrid Models as First-Class Citizens in vLLM – PyTorch</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#GPU optimization`, `#speculative decoding`, `#transformers`

---

<a id="item-2"></a>
## [Google Project Zero Discloses 0-Click Exploit for Pixel 10](https://projectzero.google/2026/05/pixel-10-exploit.html) ⭐️ 9.0/10

Google Project Zero has disclosed a 0-click exploit chain targeting the Pixel 10, highlighting new attack surfaces introduced by on-device AI features that automatically process media without user interaction. This disclosure underscores the growing security risks of AI-powered features in mobile devices, and it reignites discussions about Android patch response times and the overall security posture of the ecosystem. The exploit chain likely involves vulnerabilities in the VPU (Video Processing Unit) driver and other components, and it was patched within 90 days—notably fast for an Android driver bug. The disclosure also notes that AI features increase 0-click attack surface by decoding message media before the user opens them.

hackernews · happyhardcore · May 15, 13:39 · [Discussion](https://news.ycombinator.com/item?id=48148460)

**Background**: A 0-click exploit does not require any user interaction (such as clicking a link) to execute malicious code. Google Project Zero is a team of security researchers dedicated to finding and reporting zero-day vulnerabilities. On-device AI features that automatically process incoming messages, like on Pixel 10, decode media before the user even opens them, creating new opportunities for remote exploitation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://github.com/VivekMangale4/Zero-Click-Exploit">GitHub - VivekMangale4/Zero- Click - Exploit : A zero- click exploit is...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern over AI processing SMS without user permission, with one user asking 'haven't we learned our lesson?' Another noted that Google's 90-day patch was fast, but wondered about Apple's response times. There was also discussion about a perceived increase in exploit disclosures, possibly tied to AI hype.

**Tags**: `#security`, `#Android`, `#exploit`, `#vulnerability`, `#mobile`

---

<a id="item-3"></a>
## [Zulip transitions to nonprofit foundation](https://blog.zulip.com/2026/05/15/announcing-zulip-foundation/) ⭐️ 8.0/10

Zulip announced on May 15, 2026 that it is transitioning to the Zulip Foundation, an independent nonprofit organization, with founder Tim Abbott stepping back from full-time leadership to join Anthropic along with three senior team members. This governance change ensures Zulip's long-term independence and community trust, addressing common concerns about commercial pressures in open-source chat platforms. It sets a precedent for sustainable open-source governance. The Zulip Foundation will own the project's assets and oversee its development, serving the public good. Tim Abbott and three senior team members are donating the company to the foundation and will work on AI collaboration tools at Anthropic.

hackernews · boramalper · May 15, 18:37 · [Discussion](https://news.ycombinator.com/item?id=48152168)

**Background**: Zulip is an open-source team chat and collaboration software, known for its topic-based threading and often compared to Slack. Many open-source projects, like Apache, operate under nonprofit foundations to ensure community governance and long-term stability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zulip">Zulip</a></li>
<li><a href="https://zulip.com/">Zulip is an organized team chat app for distributed teams of all sizes.</a></li>
<li><a href="https://en.wikipedia.org/wiki/The_Apache_Software_Foundation">The Apache Software Foundation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise the move for ensuring trust and independence, while others express skepticism about the Friday afternoon announcement timing. Positive comments highlight Zulip's superior interface for serious discussions compared to Discord.

**Tags**: `#open-source`, `#nonprofit`, `#governance`, `#chat`, `#Zulip`

---

<a id="item-4"></a>
## [Sigmoid curve challenges AI's Lindy effect assumption](https://www.astralcodexten.com/p/the-sigmoids-wont-save-you) ⭐️ 8.0/10

An article on Astral Codex Ten argues that AI progress may follow sigmoid curves with diminishing returns, contradicting the Lindy effect which assumes future progress is proportional to past duration. This analysis challenges the common belief that AI scaling will continue indefinitely, suggesting instead that AI development may plateau without fundamental breakthroughs, affecting investment and timeline predictions. The article draws an analogy to aircraft speed improvements over the 20th century, where each technology (propeller, turbojet, ramjet) followed its own sigmoid curve. The author warns that AI scaling laws may hit similar fundamental limits.

hackernews · Tomte · May 15, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48147021)

**Background**: The Lindy effect proposes that the future life expectancy of non-perishable things (like technologies) is proportional to their current age. Sigmoid curves describe growth that accelerates, then decelerates and saturates. In AI, scaling laws suggest performance improves predictably with more data and compute, but these may eventually hit diminishing returns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sigmoid_curve">Sigmoid curve</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lindy_effect">Lindy effect</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_scaling_law">Neural scaling law - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments include debate on whether the author's prediction of AGI in 1-2 years biases his view (dreambuffer), and a counterargument that Lindy's Law still applies to trends (btilly). Another commenter argues AI progress measures are orthogonal to true intelligence (andy99).

**Tags**: `#AI`, `#scaling laws`, `#machine learning`, `#futurism`, `#software engineering`

---

<a id="item-5"></a>
## [DOJ demands Apple and Google unmask 100k users of emissions-bypass app](https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/) ⭐️ 8.0/10

The U.S. Department of Justice has issued subpoenas to Apple and Google demanding they reveal the identities of over 100,000 users of a car-tinkering app used to disable emissions control systems. This case sets a significant legal precedent regarding government surveillance and user privacy, potentially expanding law enforcement access to app user data beyond typical criminal investigations. The app allows users to modify vehicle engine control units (ECUs) to bypass emissions controls, a practice known as chip tuning or ECU remapping, which can be illegal when used to defeat emissions systems.

hackernews · tencentshill · May 15, 17:28 · [Discussion](https://news.ycombinator.com/item?id=48151383)

**Background**: ECU tuning is the modification of a vehicle's electronic control unit software to change performance, often to increase power or fuel efficiency. However, some modifications can disable emissions controls, in violation of the Clean Air Act. Defeat devices, like those used in the Volkswagen Dieselgate scandal, are illegal in the US.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ECU_tuning">ECU tuning</a></li>
<li><a href="https://en.wikipedia.org/wiki/Defeat_device">Defeat device</a></li>
<li><a href="https://www.vallejosun.com/epa-fines-benicia-based-company-for-selling-emissions-control-defeating-devices/">EPA fines Benicia-based company for selling emissions ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concerns about privacy and government overreach, with some arguing that the app is used for illegal emissions cheating and others warning that this could set a precedent for surveillance of lawful modifications. Several commenters highlighted the centralization of app distribution as a concern.

**Tags**: `#privacy`, `#government surveillance`, `#Apple`, `#Google`, `#emissions`

---

<a id="item-6"></a>
## [Waymo Recalls 3,800 Robotaxis Over Standing Water Glitch](https://www.cnbc.com/2026/05/12/waymo-recalls-3800-robotaxis-after-able-drive-into-standing-water.html) ⭐️ 8.0/10

Waymo issued a voluntary recall of approximately 3,800 robotaxis to fix a software glitch that could cause the vehicles to drive into standing water, potentially stranding them. This recall highlights a real-world challenge for autonomous driving—distinguishing safe puddles from hazardous deep water—and demonstrates the industry's ability to deploy fleet-wide over-the-air updates to improve safety. The recall affects fifth and sixth generation Waymo automated driving systems, and the fix is expected to be deployed remotely via a software update without requiring physical service visits.

hackernews · drob518 · May 15, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48151767)

**Background**: Autonomous vehicles rely on sensors like cameras, LiDAR, and radar to perceive their environment. Distinguishing between wet pavement and standing water is difficult because both appear similar in sensor data. This recall shows that even advanced systems can fail in edge cases, but over-the-air updates allow rapid corrections.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/05/12/waymo-recalls-3800-robotaxis-after-able-drive-into-standing-water.html">Waymo recalls 3,800 robotaxis after glitch allowed some vehicles to 'drive into standing water'</a></li>
<li><a href="https://www.livenowfox.com/news/waymo-recall-robotaxis-glitch-standing-water">Waymo recalls nearly 3,800 robotaxis for glitch that may allow vehicles to drive into standing water | LiveNOW from FOX</a></li>
<li><a href="https://www.msn.com/en-us/autos/general/waymo-recalls-nearly-4-000-robotaxis-due-to-dangerous-software-glitch/ar-AA236ZEX">Waymo recalls nearly 4,000 robotaxis due to dangerous software glitch</a></li>

</ul>
</details>

**Discussion**: Commenters debated the difficulty of detecting water depth, with some suggesting dedicated water sensors while others argued inference from vehicle behavior could suffice. The discussion also touched on the advantage of fleet-wide updates and compared Tesla's camera-only approach to Waymo's multi-sensor system.

**Tags**: `#autonomous vehicles`, `#Waymo`, `#robotaxi`, `#safety`, `#AI systems`

---

<a id="item-7"></a>
## [FiveThirtyEight Articles Removed by ABC News](https://twitter.com/baseballot/status/2055309076209492208) ⭐️ 8.0/10

ABC News has taken down all articles from FiveThirtyEight, effectively shutting down the data journalism site's content online. This move eliminates a major source of data-driven journalism on politics, sports, and culture, sparking criticism about content preservation and corporate handling of valuable journalism assets. The removal includes highly acclaimed interactive visualizations, such as gun deaths and microbiome explainers. Founder Nate Silver reportedly offered to buy back the IP but ABC refused.

hackernews · cmsparks · May 15, 19:07 · [Discussion](https://news.ycombinator.com/item?id=48152553)

**Background**: FiveThirtyEight, founded by Nate Silver, was known for its statistical analysis of elections and sports. It was acquired by ABC News in 2018 and gradually saw layoffs and reduced output before the content removal.

**Discussion**: Commenters expressed sadness over losing excellent visualizations and criticized ABC's decision. Some noted the brand was left to die despite its value, and speculated on Silver's prior attempts to buy it back.

**Tags**: `#media`, `#data journalism`, `#fivethirtyeight`, `#ABC News`, `#content removal`

---

<a id="item-8"></a>
## [Coding agents reduce technology lock-in risks](https://simonwillison.net/2026/May/14/not-so-locked-in/#atom-everything) ⭐️ 8.0/10

Simon Willison discusses how coding agents make technology choices less permanent, citing a company that used agents to port its iOS and Android apps to React Native with the option to port back to native if needed. This shift reduces the long-term risk of choosing a technology stack, enabling companies to experiment and switch more freely, potentially transforming software engineering decision-making. The anecdote parallels Mitchell Hashimoto's observation that programming languages are increasingly not lock-in, as demonstrated by Bun's migration from Zig to Rust.

rss · Simon Willison · May 14, 22:53

**Background**: Coding agents are AI-powered tools that assist or automate code generation, migration, and refactoring. They can significantly lower the cost of rewriting or porting code between languages or frameworks, reducing the historical barrier of technology lock-in where once a choice was made, it was costly to reverse.

<details><summary>References</summary>
<ul>
<li><a href="https://siliconangle.com/2025/06/23/ai-developer-coding-agents-software-engineering-roboticsaiinfrastructure/">Coding agents : Augment Code and AI-assisted... - SiliconANGLE</a></li>
<li><a href="https://medium.com/@dave-patten/the-state-of-ai-coding-agents-2026-from-pair-programming-to-autonomous-ai-teams-b11f2b39232a">The State of AI Coding Agents (2026): From Pair... | Medium</a></li>

</ul>
</details>

**Tags**: `#coding agents`, `#software engineering`, `#React Native`, `#programming languages`, `#AI-assisted development`

---

<a id="item-9"></a>
## [MitchellH warns companies suffer from AI psychosis](https://twitter.com/mitchellh/status/2055380239711457578) ⭐️ 7.0/10

MitchellH, creator of HashiCorp tools, tweeted that many companies are under 'AI psychosis' by outsourcing critical thinking to AI without proper oversight, leading to irrational decision-making. The post has gained high engagement on social media. This warning highlights a growing risk in the tech industry where companies may blindly trust AI outputs, potentially leading to flawed business decisions and diminished human expertise. It calls for a balanced approach to AI adoption that includes human oversight. MitchellH uses the term 'AI psychosis' metaphorically to describe organizational irrationality, not the clinical condition. The concept originally refers to individuals developing psychosis from chatbot interactions, as noted in Wikipedia and Psychology Today.

hackernews · reasonableklout · May 15, 20:26 · [Discussion](https://news.ycombinator.com/item?id=48153379)

**Background**: AI psychosis is a phenomenon first identified in 2023 where individuals experience worsening paranoia or delusions due to excessive interaction with AI chatbots. MitchellH extends this idea to companies that rely on AI for decision-making without critical evaluation, essentially outsourcing their thinking to the AI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chatbot_psychosis">Chatbot psychosis - Wikipedia</a></li>
<li><a href="https://modernorange.io/item/48153379">Mitchellh – I strongly believe there are entire companies now under AI ...</a></li>

</ul>
</details>

**Discussion**: Commenters generally agree with the warning, noting that AI-written code can become too complex for humans to understand, and that some financial professionals post ChatGPT outputs as their own reasoning. There is concern about unsustainable debugging cycles and loss of human judgment.

**Tags**: `#AI psychosis`, `#software engineering`, `#AI risk`, `#decision-making`, `#over-reliance`

---

<a id="item-10"></a>
## [California bill targets game shutdown refunds](https://arstechnica.com/gaming/2026/05/bill-to-keep-online-games-playable-clears-key-hurdle-in-california/) ⭐️ 7.0/10

A proposed California bill (AB 2426) would require game publishers to either release patches enabling offline play or provide refunds when they end support for an online game. This legislation could reshape the digital games market by forcing publishers to consider long-term playability and consumer rights, potentially setting a precedent for other states or countries. The bill exempts games offered solely on a subscription basis; publishers argue it could accelerate the shift to subscription models. It also requires 60 days' notice before shutting down.

hackernews · Lihh27 · May 15, 19:48 · [Discussion](https://news.ycombinator.com/item?id=48152994)

**Background**: Online games often rely on remote servers; when servers shut down, the game becomes unplayable. Software preservation efforts aim to keep such games accessible, but current laws grant only licenses, not ownership, to consumers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Software_preservation">Software preservation</a></li>
<li><a href="https://www.softwarepreservationnetwork.org/">Software Preservation Network</a></li>

</ul>
</details>

**Discussion**: Commenters were divided: some advocated open-sourcing server code to let communities run their own servers, while others worried about unintended consequences like accelerating subscription models or creating perverse incentives.

**Tags**: `#digital rights`, `#video games`, `#legislation`, `#software preservation`, `#consumer protection`

---

<a id="item-11"></a>
## [Explore Wikipedia via a Windows XP Desktop Interface](https://explorer.samismith.com/) ⭐️ 7.0/10

A web application called 'Explorer' at explorer.samismith.com lets users navigate Wikipedia articles through a simulated Windows XP desktop environment. The design mimics the classic folder and window system, turning Wikipedia categories into folders and articles into documents. This project offers a nostalgic and intuitive mental model for browsing knowledge, reminiscent of how users interacted with files before modern web interfaces. It may inspire renewed appreciation for desktop metaphors in UI design and prompt discussions about effective information organization. The interface replicates Windows XP's visual style, including large scrollbars, window borders, and the ability to resize windows. It transforms Wikipedia's category hierarchy into a folder tree, with uncategorized articles possibly placed on the desktop for a more authentic feel.

hackernews · smusamashah · May 15, 08:45 · [Discussion](https://news.ycombinator.com/item?id=48146129)

**Background**: Windows XP, released in 2001, featured a graphical user interface that used folders, files, and windows as core metaphors for organizing and accessing data. Over time, web applications largely abandoned these metaphors in favor of more minimal, content-focused designs. This project revives the XP aesthetic to explore how familiar UI paradigms can make large knowledge bases like Wikipedia feel more navigable.

**Discussion**: Commenters praised the design for matching the mental model of organizing knowledge, with some highlighting the relief of having large scrollbars and resizable windows. Other comments noted the visual style resembles Windows XP Media Center Edition more than standard XP, and suggested putting uncategorized articles directly on the desktop for authenticity.

**Tags**: `#Wikipedia`, `#UI design`, `#nostalgia`, `#web app`, `#interactive`

---

<a id="item-12"></a>
## [Image-blaster: single image to 3D environments and meshes](https://github.com/neilsonnn/image-blaster) ⭐️ 7.0/10

Image-blaster is an open-source tool that uses AI models to generate 3D environments, special effects, and meshes from a single input image, leveraging services like World Labs and Meshy.ai. This tool significantly lowers the barrier for creating 3D content, enabling artists and developers to quickly prototype scenes and assets from a single photo, which could accelerate workflows in game development, VR/AR, and visualization. The project integrates multiple AI models—including World Labs for environment generation and Meshy.ai for non-scene meshes—and supports texturing and auto-rigging, though community feedback notes that outputs can sometimes hallucinate unrealistic details.

hackernews · MattRogish · May 15, 15:42 · [Discussion](https://news.ycombinator.com/item?id=48150069)

**Background**: Single-image 3D reconstruction uses AI to infer depth, geometry, and texture from a flat picture, turning a 2D photo into a 3D model. Tools like this have existed for years, but recent advances in generative models have dramatically improved quality and speed, making them practical for prototyping.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/wolve/zero-to-printable-how-image-to-3d-ai-is-changing-rapid-prototyping-workflows-2gi9">Zero to Printable: How Image -to- 3 D AI Is Changing... - DEV Community</a></li>
<li><a href="https://www.meshy.ai/">Meshy AI - The #1 AI 3D Model Generator</a></li>
<li><a href="https://gen.hexa3d.io/free-online-ai-3d-image-to-model-generator">Image to 3D Model AI Generator | Free Online 3D Converter with Textured ...</a></li>

</ul>
</details>

**Discussion**: Commenters are impressed by the tool's capabilities, with one user recalling Microsoft's PhotoSynth from 17 years ago and noting that doing it with one image is 'an order of magnitude cooler.' However, some express concerns about usability, as results can be hallucinated and inconsistent, and others wonder about comparisons to alternative tools like TRELLIS or GPT Image 2.

**Tags**: `#3D reconstruction`, `#AI`, `#image-to-3D`, `#single-image 3D`, `#computer vision`

---

<a id="item-13"></a>
## [O(x)Caml in Space: Stack Allocation Boosts Satellite Software](https://gazagnaire.org/blog/2026-05-14-borealis.html) ⭐️ 7.0/10

The article describes using OCaml and its extension OxCaml in satellite software, achieving significant performance improvements through stack allocation annotations. This demonstrates that garbage-collected languages like OCaml can be effectively used in resource-constrained space systems, potentially expanding the role of high-level languages in aerospace software. With OxCaml's exclave_ stack annotations, p99.9 latency on the dispatch hot path dropped from 29 ns to 9 ns per packet, and minor GCs went from 394 to zero over 25 million packets.

hackernews · yminsky · May 15, 10:55 · [Discussion](https://news.ycombinator.com/item?id=48147058)

**Background**: OCaml is a statically-typed functional programming language with a garbage collector (GC). OxCaml is a set of extensions by Jane Street that give programmers more control over allocations, enabling stack allocation to reduce GC pressure. Stack allocation puts data on the stack instead of the heap, avoiding GC overhead and improving determinism.

<details><summary>References</summary>
<ul>
<li><a href="https://oxcaml.org/">OxCaml | About</a></li>
<li><a href="https://blog.janestreet.com/introducing-oxcaml/">Jane Street Blog - Introducing OxCaml</a></li>
<li><a href="https://news.ycombinator.com/item?id=44268782">OxCaml - a set of extensions to the OCaml programming language ...</a></li>

</ul>
</details>

**Discussion**: Commenters shared experiences with OCaml in space (e.g., GHGSat-D in 2016) and debated CCSDS complexity. Avsm highlighted latency improvements, while others discussed GC reduction techniques in high-frequency scenarios.

**Tags**: `#OCaml`, `#space software`, `#garbage collection`, `#performance optimization`, `#systems programming`

---

<a id="item-14"></a>
## [In-Browser Neural Net Learns to Play Snake via PPO](https://ppo.gradexp.xyz/) ⭐️ 7.0/10

A web-based demo allows users to watch a neural network trained with Proximal Policy Optimization (PPO) learn to play the game Snake in real-time, running entirely in the browser using tinygrad and WebGPU. This demo showcases the feasibility of running reinforcement learning training directly in the browser on consumer GPUs, lowering the barrier for education and experimentation in AI without requiring specialized hardware or cloud services. The demo relies on tinygrad's TinyJit to compile neural network operations into WebGPU kernels, enabling efficient GPU compute in web browsers. However, community reports indicate potential bugs leading to score corruption and training loops that get stuck.

hackernews · c1b · May 14, 15:35 · [Discussion](https://news.ycombinator.com/item?id=48136981)

**Background**: Proximal Policy Optimization (PPO) is a reinforcement learning algorithm that stabilizes training by limiting policy updates. Tinygrad is a minimal deep learning framework that can target multiple backends, including WebGPU via its compiler. WebGPU is a modern web standard for GPU acceleration, allowing complex computations like neural network training to run in the browser without plugins.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Proximal_Policy_Optimization">Proximal policy optimization - Wikipedia</a></li>
<li><a href="https://github.com/tinygrad/tinygrad">GitHub - tinygrad / tinygrad : You like pytorch? You like micrograd?</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the snake often gets penalized for not reaching the apple quickly, which may not align with the game's goal of maximizing length. Others observed that after reaching high scores, the training would suddenly drop to zero, suggesting a potential bug. Some pointed out that the snake can get stuck in infinite loops, indicating the reward function may need refinement.

**Tags**: `#neural networks`, `#reinforcement learning`, `#webgpu`, `#tinygrad`, `#demo`

---

<a id="item-15"></a>
## [Mitchell Hashimoto: Languages Are Becoming Fungible](https://simonwillison.net/2026/May/14/mitchell-hashimoto/#atom-everything) ⭐️ 6.0/10

Mitchell Hashimoto argues that programming languages are becoming fungible, citing Bun's rapid port from Zig to Rust as an example of how languages are no longer a lock-in. This challenges the traditional notion that programming languages create vendor lock-in, potentially changing how companies and developers evaluate technology stacks. If switching languages is cheap and fast, it could accelerate adoption of newer, more specialized languages. Bun is a JavaScript runtime originally built in Zig but was ported to Rust in roughly a week or two, demonstrating high language fungibility. Hashimoto notes that Rust, like Zig, is expendable if a better language emerges.

rss · Simon Willison · May 14, 22:31

**Background**: Bun is a fast all-in-one JavaScript runtime that bundles, transpiles, and runs JavaScript and TypeScript. It was originally written in Zig, a low-level systems programming language, but recently underwent a rewrite in Rust. Zig and Rust are both modern systems languages that aim to provide memory safety and performance, but they differ in philosophy and ecosystem. The concept of language fungibility means that the cost of switching between languages is low, reducing long-term commitment.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Tags**: `#programming languages`, `#rust`, `#zig`, `#bun`, `#software engineering`

---