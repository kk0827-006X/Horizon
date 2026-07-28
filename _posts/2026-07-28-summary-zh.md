---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> From 47 items, 8 important content pieces were selected

---

1. [vLLM v0.26.0 发布：支持 Inkling 模型与 DeepSeek-V4 优化](#item-1) ⭐️ 9.0/10
2. [MoonShot AI 发布 Kimi-K3 2.8 万亿参数权重](#item-2) ⭐️ 9.0/10
3. [Anthropic 主张对开放权重模型进行强制性安全测试](#item-3) ⭐️ 8.0/10
4. [Python-build-standalone 提供被 uv 等工具使用的便携式 Python 发行版](#item-4) ⭐️ 8.0/10
5. [法官驳回谷歌利用 DMCA 阻止爬取的企图](#item-5) ⭐️ 8.0/10
6. [论坛软件将 React 替换为 HTMX](#item-6) ⭐️ 8.0/10
7. [LLM 令牌中继市场利用免费试用和窃取凭证](#item-7) ⭐️ 8.0/10
8. [Ethan Mollick 指南从聊天转向智能体 AI](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 发布：支持 Inkling 模型与 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 提供了对 Thinking Machines Lab 的 Inkling 1T 参数多模态模型家族的首日支持，包括相对注意力、短卷积和共享专家汇等新型架构组件。同时，该版本带来了跨厂商的 DeepSeek-V4 性能大幅提升、fp32 lm_head 支持、灵活的注意力后端以及成熟的 KV 卸载功能。 此版本是开源 LLM 推理的一个重要里程碑，vLLM 在首日即支持最新的 1T 参数多模态模型，使得最新架构能够高效部署。灵活的注意力后端和增强的 KV 卸载功能改善了对混合模型和长上下文应用的支持，惠及更广泛的 AI 服务生态系统。 Inkling 支持包括基础建模、分段 CUDA 图、Hopper FA4 相对注意力、MTP=1 推测解码、LoRA 和 ModelOpt NVFP4 量化。DeepSeek-V4 获得了专用路由内核（端到端 TPOT 提升 2.94%）、fused_topk_bias（内核速度提升 1.5–2 倍）以及冗余重复/复制消除（端到端 TPOT 提升 1.8%）。

github · khluu · Jul 27, 01:06

**背景**: vLLM 是一个用于大语言模型（LLM）的高性能推理引擎，广泛用于生产环境中的模型服务。Thinking Machines Lab 的 Inkling 模型家族是一个 1T 参数的多模态模型，支持文本、图像和音频输入，最长上下文可达 1M。FlashAttention-4 (FA4) 是面向 Hopper GPU 的优化注意力内核，NVFP4 是 NVIDIA 通过 ModelOpt 支持的 4 位浮点量化格式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm.ai/blog/2026-07-15-inkling">TML Inkling on vLLM: Day-0 Support with Optimized Performance</a></li>
<li><a href="https://arxiv.org/html/2603.05451v1">FlashAttention-4: Algorithm and Kernel Pipelining Co-Design ...</a></li>
<li><a href="https://github.com/vllm-project/vllm/blob/main/vllm/models/inkling/nvidia/ops/fa4_rel_attention.py">vllm/vllm/models/inkling/nvidia/ops/fa4_rel_attention.py at ...</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#model optimization`, `#open-source release`, `#GPU performance`

---

<a id="item-2"></a>
## [MoonShot AI 发布 Kimi-K3 2.8 万亿参数权重](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 9.0/10

MoonShot AI 在 Hugging Face 上发布了其 2.8 万亿参数的 Kimi-K3 模型权重，大小达 1.56TB，并采用了取代之前修改版 MIT 许可的新许可协议。新协议要求年收入超过 2000 万美元的大型模型即服务（MaaS）企业单独签订协议。 此次发布为开放权重社区提供了目前最大的公开可用模型之一，极大推动了开放 AI 研究与竞争。许可协议的变化凸显了 AI 行业中开放性与商业控制之间的持续张力。 Kimi-K3 模型拥有 2.8 万亿参数，以 FP16 格式提供，运行需要大量硬件资源。该许可明确要求大型 MaaS 提供商与 MoonShot 单独签订协议，区别于此前 K2 模型使用的“修改版 MIT”标签。

rss · Simon Willison · Jul 27, 23:39

**背景**: MoonShot AI 是一家中国公司，以开发 Kimi 系列大型语言模型而闻名。2025 年 7 月，他们以修改版 MIT 许可发布了 Kimi-K2，要求大型商业实体进行署名。新的 K3 许可不再自称修改版 MIT，而是施加了更严格的商业条款。开放权重模型发布已训练的参数，但可能不完全符合开源促进会（OSI）的定义，本例许可即是如此。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(chatbot)">Kimi (chatbot) - Wikipedia</a></li>
<li><a href="https://localaimaster.com/models/kimi-k2">Kimi K 2 : 1T MoE Model (32B Active) — Local Setup... | Local AI Master</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open Source`, `#Large Language Models`, `#Machine Learning`

---

<a id="item-3"></a>
## [Anthropic 主张对开放权重模型进行强制性安全测试](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 发布了一份立场声明，反对彻底禁止开放权重 AI 模型，而是呼吁对所有足够强大的模型（包括开放和封闭模型）进行强制性安全测试。批评者认为，这一立场实际上通过设置昂贵或难以获得的测试要求来限制开放开发。 作为一家领先的 AI 公司，Anthropic 的政策立场可能影响全球 AI 监管和开源 AI 的未来。如果被采纳，强制性安全测试可能为小型开发者和研究人员设置障碍，潜在地将 AI 开发集中在资金充足的组织手中。 Anthropic 的 CEO Dario Amodei 此前表示他认为禁令没有用处，但该立场支持禁止向中国出售芯片等措施，被指责为虚伪。声明未明确由谁执行安全测试或制定标准，实施细节不清晰。

hackernews · surprisetalk · Jul 27, 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重 AI 模型是指其训练参数（权重）公开发布的模型，任何人都可以下载、修改并在自己的硬件上运行。这种开放性促进了创新和可访问性，但也引发了滥用担忧，因为这些模型可以在没有监督的情况下使用。关于如何监管这类模型的辩论是 AI 安全政策的核心，需要在开放性与防止危害之间取得平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership - microsoft.com</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**社区讨论**: 社区评论高度批评，用户 cogman10 等人认为，由于成本和行政障碍，强制性测试实际上就是禁令。其他人指出 Anthropic 立场中的矛盾，例如支持芯片禁令却声称反对禁令，并质疑该公司的动机，认为其是在保护自己的封闭、昂贵的模型。

**标签**: `#AI safety`, `#open-weights`, `#AI policy`, `#artificial intelligence`, `#regulation`

---

<a id="item-4"></a>
## [Python-build-standalone 提供被 uv 等工具使用的便携式 Python 发行版](https://gregoryszorc.com/docs/python-build-standalone/main/) ⭐️ 8.0/10

python-build-standalone 项目生成自包含、高度可移植的 Python 发行版，现已成为 uv、pipx、Hatch、Poetry 和 Bazel 等许多工具的主要 Python 安装来源。 这些发行版简化了将 Python 捆绑到应用程序中的过程，无需系统 Python 安装，对现代 Python 工具和应用程序分发至关重要。 这些发行版包含大部分标准库扩展模块，并且跨平台高度可移植。Astral（uv 背后的公司）已接管该项目的维护，确保持续开发。

hackernews · jcbhmr · Jul 27, 18:43 · [社区讨论](https://news.ycombinator.com/item?id=49073942)

**背景**: 传统上，Python 应用程序需要用户单独安装 Python，这可能导致版本冲突和复杂的设置。python-build-standalone 提供完全自包含的 Python 构建，可直接嵌入应用程序或按需下载，消除对系统 Python 的依赖。这种方法类似于 Rust 的 rustup 管理工具链的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/astral-sh/python-build-standalone">GitHub - astral-sh/ python - build - standalone : Produce redistributable...</a></li>
<li><a href="https://astral.sh/blog/python-build-standalone">A new home for python - build - standalone</a></li>
<li><a href="https://gregoryszorc.com/docs/python-build-standalone/main/">Python Standalone Builds — python - build - standalone documentation</a></li>

</ul>
</details>

**社区讨论**: 社区成员，包括 charliermarsh（uv 的创建者）和 simonw，称赞这些发行版简化了 Python 捆绑，并指出 Astral 现已维护该项目。其他人提到了相关项目，如用于单文件可执行文件的 PyOxy 和用于跨平台二进制的 Cosmopolitan，突显了便携式 Python 解决方案的更广泛生态系统。

**标签**: `#Python`, `#standalone`, `#portable`, `#distribution`, `#tooling`

---

<a id="item-5"></a>
## [法官驳回谷歌利用 DMCA 阻止爬取的企图](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

一名联邦法官驳回了谷歌试图利用《数字千年著作权法》（DMCA）阻止 SerpAPI 爬取其搜索引擎结果页面的请求。 这一裁决重申了公开可访问的网络数据通常可以自由爬取，这对于维护开放的互联网以及依赖替代搜索数据访问的开发者至关重要，尤其是在谷歌弃用其搜索 API 之后。 谷歌辩称其搜索结果属于可受版权保护的汇编，爬取它们违反了 DMCA 的反规避条款，但法官认为这些搜索结果缺乏版权保护所需的最低限度的创造性。

hackernews · cdrnsf · Jul 27, 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: DMCA 是一部美国版权法，包含禁止规避用于保护受版权作品的技术措施的规定。网络爬取是从网站自动提取数据的做法，这一行为时常面临法律挑战。谷歌自身就是建立在爬取和索引开放网络的基础上的，这一点在这一案件中让许多人感到讽刺。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eff.org/issues/dmca">DMCA | Electronic Frontier Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_scraping">Web scraping - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍指出，谷歌自身起源于网络爬虫，却利用 DMCA 阻止爬取，这具有讽刺意味。一些人批评谷歌在删除其廉价的搜索 API 的同时仍反对第三方爬取，称这是典型的大公司行为，恰恰催生了它所起诉的活动。

**标签**: `#legal`, `#web scraping`, `#Google`, `#DMCA`, `#copyright`

---

<a id="item-6"></a>
## [论坛软件将 React 替换为 HTMX](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 8.0/10

Misago 论坛项目在 2023 年移除了 React.js，转而采用 HTMX 实现 UI 交互，并在社区讨论中详细阐述了这一过程。 这一转变反映了从繁重的客户端框架向更简单的服务端驱动交互的发展趋势，降低了复杂性并提升了内容型网站的性能。 HTMX 通过自定义属性扩展 HTML，支持 AJAX、WebSockets 和服务器推送事件，无需编写 JavaScript 即可实现动态部分更新。讨论指出，对于论坛软件，HTMX 提供了轻量级替代 SPA 的方案。

hackernews · Ralfp · Jul 27, 09:58 · [社区讨论](https://news.ycombinator.com/item?id=49067301)

**背景**: HTMX 是一个开源 JavaScript 库，通过 HTML 属性实现动态网页，遵循超媒体驱动的方法。它根据用户操作发送 HTTP 请求，并用服务器响应更新页面区域，与使用虚拟 DOM 的 React 等客户端框架形成对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>

</ul>
</details>

**社区讨论**: 许多评论者支持这一转变，一些用户分享了实践经验：James2doyle 指出当响应体较大时性能变慢，而 prologic 在所有 Web 应用（包括 PWA）中使用 HTMX。其他人则推荐了像 PyView 这样的服务端渲染交互替代方案。

**标签**: `#HTMX`, `#React`, `#web development`, `#JavaScript frameworks`, `#server-side rendering`

---

<a id="item-7"></a>
## [LLM 令牌中继市场利用免费试用和窃取凭证](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

Matt Lenhard 的调查揭示了一个蓬勃发展的中继市场，该市场通过汇集来自免费试用、被盗凭证和退款攻击的 API 密钥，以折扣价转售 LLM 令牌，主要在中国运营。 这个市场对 LLM 供应商和开发者构成重大风险，因为它助长了欺诈、API 密钥滥用和潜在的模型蒸馏，凸显了加强 API 安全性和成本控制的紧迫需求。 这些代理基于开源项目 one-api 及其分支 new-api 构建，这些是合法的工具，可在聚合的 API 凭证上实现负载均衡。转售商通过利用未受保护的支持机器人、被盗信用卡或退款欺诈来提供折扣。

rss · Simon Willison · Jul 26, 19:30

**背景**: LLM API 提供商（如 OpenAI）按令牌使用量收费，开发者通常为密钥设置限制。中继市场通过汇集大量密钥来提供更便宜的访问，有时使用欺诈手段。开源 API 网关（如 one-api 和 new-api）本意是用于合法的多模型管理，但可能被滥用于此目的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/QuantumNous/new-api">GitHub - QuantumNous/new-api: A unified AI model hub for aggregation & distribution. It supports cross-converting various LLMs into OpenAI-compatible, Claude-compatible, or Gemini-compatible formats. A centralized gateway for personal and enterprise model management. 🍥</a></li>

</ul>
</details>

**标签**: `#LLM`, `#API security`, `#fraud`, `#proxy`, `#token reselling`

---

<a id="item-8"></a>
## [Ethan Mollick 指南从聊天转向智能体 AI](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 7.0/10

Ethan Mollick 更新了他的 AI 使用指南，现在重点介绍能够自主执行数小时人类工作的智能体系统，如 ChatGPT Work 和 Claude Cowork。 这一转变凸显了从聊天式 AI 到自主智能体的行业趋势，帮助从业者为复杂的多步骤任务选择合适的模型。 指南指出 Gemini 不再被列入，因为 Google 缺乏类似的 Codex/ChatGPT Work/Cowork 类别。ChatGPT 和 Claude 提供了名称令人困惑的模式，如 Work、Cowork、Codex 和 Code，每种模式具有不同能力。

rss · Simon Willison · Jul 27, 21:55

**背景**: 智能体 AI 指的是能够在有限人类监督下追求目标、使用工具并采取行动的系统。早期的 AI 指南侧重于聊天界面，但较新的模型如 GPT-4、Claude 4 Opus 和 Gemini 2.5 Pro 现在支持超越简单对话的智能体能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://chatgpt.com/ru-RU/work/">ChatGPT Work</a></li>

</ul>
</details>

**标签**: `#AI`, `#agents`, `#opinion guide`, `#Ethan Mollick`

---