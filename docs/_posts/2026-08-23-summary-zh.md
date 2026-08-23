---
layout: default
title: "Horizon Summary: 2026-08-23 (ZH)"
date: 2026-08-23
lang: zh
---

> 从 37 条内容中筛选出 12 条重要资讯。

---

1. [Llama.cpp 发布 0.2.0 版本并提供预编译二进制文件](#item-1)
2. [SGLang v0.5.18 发布，新增模型支持与性能提升](#item-2)
3. [Munder Difflin：本地多智能体框架，用智能体克隆运行一个办公室](#item-3)
4. [MCP 路线图：远程服务器转为 HTTP 负载，强化 Agent 授权](#item-4)
5. [Claude 如何为 AI 生成文本添加水印：视频深度解析](#item-5)
6. [单张 RTX 5090 实测 Qwen3.8-27B NVFP4 真 262K 上下文](#item-6)
7. [为何本地 LLM 显得更笨：配置与量化是关键](#item-7)
8. [macOS 27 弃用 hdiutil，改用 diskutil image](#item-8)
9. [编程代理：验证胜过逐行审查](#item-9)
10. [为何仿真正在接管：性能略逊 10%，成本百倍低，速度快万倍](#item-10)
11. [TikTok 同意支付 4 亿美元和解美国儿童隐私诉讼](#item-11)
12. [黑客利用安卓车机更新应用植入代理僵尸网络](#item-12)

---

<a id="item-1"></a>
## [Llama.cpp 发布 0.2.0 版本并提供预编译二进制文件](https://www.reddit.com/r/LocalLLaMA/comments/1vv4mei/llamacpp_version_020_is_out/) ⭐️ 9.0/10

llama.cpp 项目发布了 0.2.0 版本，这是这一广受欢迎的本地推理库的一个重要里程碑。该版本包含变更日志和源代码，并附带 b10566 标签下的预编译二进制文件。 作为在本地运行大型语言模型的事实标准，llama.cpp 支撑着 Ollama 和 LM Studio 等工具，因此这一重要版本发布影响了庞大的开发者和用户生态。它标志着本地 LLM 推理在持续成熟与稳定。 源代码和变更日志可在 GitHub 官方 v0.2.0 版本发布页面获取，而相关的预编译二进制文件则通过单独的发布标签 b10566 分发。用户应查阅变更日志以了解具体更新和潜在的破坏性变更。

reddit · r/LocalLLaMA · /u/PhilippeEiffel · 8月22日 06:23

**背景**: llama.cpp 是一个开源软件库，用 C/C++ 编写，对 Llama 等大型语言模型执行推理，并与 GGML 张量库协同开发。它已成为本地推理的事实标准，几乎构成 Ollama、LM Studio 等所有本地推理工具的核心。本地 LLM 推理是指在自己硬件上运行训练好的模型，而不是依赖远程云服务器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/releases">Releases · ggml-org/llama.cpp - GitHub</a></li>
<li><a href="https://prajnaaiwisdom.medium.com/what-is-local-llm-inference-a-beginners-guide-b31043768d4f">What Is Local LLM Inference? A Beginner’s Guide | by PrajnaAI | Medium</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#LLM`, `#release`, `#local inference`, `#software engineering`

---

<a id="item-2"></a>
## [SGLang v0.5.18 发布，新增模型支持与性能提升](https://github.com/sgl-project/sglang/releases/tag/v0.5.18) ⭐️ 8.0/10

SGLang v0.5.18 已发布，包含来自 212 位贡献者的 710 个拉取请求。它新增了对 Muse Glimmer、Intern-S2-Mobius、SANA-Video 和 LTX-2.5 等模型的支持，并提供了重叠检查点暂存和 FlashInfer MNNVL 纯 allreduce 等性能优化。 此版本将 SGLang 的支持扩展到基于扩散的视频模型和智能体模型，使其成为 AI 生态中更通用的服务框架。启动和解码延迟的改进直接惠及 DeepSeek-V4 和 Qwen3 等大型模型的生产部署。 关键性能特性包括启动时的重叠检查点暂存（Qwen3-32B 在 H100 上最高加速 2.38 倍）、TP LMHead 的 All-to-All 将 DeepSeek-V4-Pro B200 上的 LMHead 时间从 320us 降至 169us，以及 FlashInfer MNNVL 纯 allreduce 在 Blackwell 上最高带来 +6.9% 的解码收益。依赖项升级到 torch 2.13.0、flashinfer 0.6.17 和 sgl-kernel 0.4.6.post1，编译内核缓存统一到 SGLANG_CACHE_DIR 下。

github · Fridge003 · 8月22日 00:09

**背景**: SGLang 是一个开源的高性能服务框架，用于大型语言模型和多模态模型，由 UC Berkeley 开发并由 LMSYS 托管。它利用 RadixAttention 自动复用 KV 缓存以实现高吞吐。此版本反映了该领域超越文本 LLM 的扩展：Muse Glimmer 是 Meta 推出的 30B 参数智能体模型，而 SANA-Video 是一种用于生成一分钟时长视频的高效扩散模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/sgl-project/sglang">GitHub - sgl-project/sglang: SGLang is a high-performance serving framework for large language models and multimodal models. · GitHub</a></li>
<li><a href="https://inference.net/content/sglang-complete-guide/">SGLang: The Complete Guide to High-Performance LLM Inference | Inference.net</a></li>
<li><a href="https://ollama.com/library/muse-glimmer">muse - glimmer</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#SGLang`, `#open source`, `#release`, `#AI/ML`

---

<a id="item-3"></a>
## [Munder Difflin：本地多智能体框架，用智能体克隆运行一个办公室](https://munderdiffl.in/) ⭐️ 8.0/10

Munder Difflin 是一个免费、开源、本地优先的多智能体 harness（框架），可包装 Claude Code 和 Codex 等现有编码智能体。它能运行不消耗 token 的确定性智能体团队仿真，上线一周内已吸引超过 2 万名用户。 通过在不增加 token 消耗的情况下模拟确定性智能体团队，Munder Difflin 使多智能体开发变得更经济、更可预测。它的快速采用表明，开发者对能够为日益流行但混乱的 LLM 智能体集群带来秩序的工具存在强烈需求。 该框架支持几乎所有主流的编码智能体 harness，用户反馈称它降低了整体 token 消耗。其仿真过程是确定性的，项目由独立开发者 Chaitanya Giri 维护。

hackernews · simonpure · 8月22日 09:49 · [社区讨论](https://news.ycombinator.com/item?id=49398152)

**背景**: 多智能体 harness 的作用是将多个 AI 编码智能体协调成一个团队，这与单个智能体或框架不同，Munder Difflin 的博客正是这样定义的。LLM 智能体本质上是概率性的，因此确定性编排通常需要运行时门控或精细控制。Munder Difflin 包装 Claude Code、Codex 等现有编码智能体，使开发者无需支付额外 token 就能构建确定性团队工作流；它的“克隆办公室”主题也讽刺了智能体集群常因目标冲突而最终崩溃的现象。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://munderdiffl.in/blog/what-is-a-multi-agent-harness/">What Is a Multi - Agent Harness ? — Munder Difflin Blog</a></li>
<li><a href="https://github.com/chaitanyagiri/munder-difflin">GitHub - chaitanyagiri/ munder - difflin : local multi - agent harness</a></li>
<li><a href="https://www.elementum.ai/blog/are-ai-agents-deterministic">Are AI Agents Deterministic ? | Elementum AI</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认为《办公室》的模仿是对智能体集群失调的准确比喻，同时也提出了建设性反馈。作者 Chaitanya 亲自在讨论中回答问题，并提到 2 万多名用户表示该工具降低了 token 消耗。一位用户给出了详细评测，称赞其概念但希望用基于角色的流水线代替固定智能体；还有人喜欢“迈克尔 vs 德怀特”式的管理幽默。

**标签**: `#multi-agent systems`, `#LLM tools`, `#coding agents`, `#developer tools`, `#AI`

---

<a id="item-4"></a>
## [MCP 路线图：远程服务器转为 HTTP 负载，强化 Agent 授权](https://blog.modelcontextprotocol.io/posts/mcp-roadmap/) ⭐️ 8.0/10

新的 MCP 路线图在博客文章中发布，宣布计划将远程 MCP 服务器视为普通 HTTP 负载，标准化自主代理的授权，并回应关于 MCP 过于复杂的批评。这标志着协议演进的重要转变。 该路线图意义重大，因为 MCP 正成为 AI 代理连接的关键标准，而将其简化为 HTTP 可以加速开发者和企业的采用。为代表用户行事的代理改进授权，对于自主 AI 系统的发展至关重要。 路线图特别提出，到 2026 年 7 月 28 日发布时，远程 MCP 服务器将与其他 HTTP 负载无异，以回应常见批评。它还概述了一种标准化方式，让服务器识别和信任代理身份，包括代表用户运行的子代理和云工作负载。

hackernews · pentagrama · 8月22日 13:31 · [社区讨论](https://news.ycombinator.com/item?id=49399591)

**背景**: MCP（模型上下文协议）是一种开源标准，用于将 AI 应用程序连接到外部数据源和工具。它由 Anthropic 推出，旨在用单一协议取代碎片化的集成，使 AI 模型更容易访问数据库、文件和 API。路线图对 HTTP 的关注反映了行业向更简单、更原生网络协议发展的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>
<li><a href="https://github.com/modelcontextprotocol">Model Context Protocol · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一，但多数人欢迎转向 HTTP，有评论者称赞放弃“定制协议”。然而，也有人质疑有多少服务器会完整实现该路线图，部分人对 MCP 是否比 REST 端点加 skills.md 文件更具优势仍持怀疑态度，并对过去的转向和复杂性表示不满。

**标签**: `#MCP`, `#AI`, `#protocols`, `#LLM`, `#HTTP`

---

<a id="item-5"></a>
## [Claude 如何为 AI 生成文本添加水印：视频深度解析](https://magazine.sebastianraschka.com/p/claude-watermarking) ⭐️ 8.0/10

Sebastian Raschka 发布了一段 48 分钟的视频深度解析，讲解 Claude 如何为 AI 生成的文本添加水印，涵盖 token 采样、水印检测和去除方法。 AI 文本水印是一个及时的主题，因为它有助于检测假新闻、学术作弊和其他 AI 生成内容的滥用。本教程由知名机器学习作者提供，为从业者带来了技术性的实践讲解。 据报道，该视频讲解了 token 采样、水印检测和去除，但所提供的文章文本仅包含标题、摘要和链接，没有展示代码或实现细节。本教程面向已经熟悉 LLM 推理和采样的读者。

rss · Sebastian Raschka · 8月22日 11:11

**背景**: 文本水印是一种在文本中嵌入隐藏信息以验证其真实性、来源或所有权的技术。随着大语言模型的兴起，为 AI 生成的文本加水印已成为检测假新闻和学术作弊的重要手段。LLM 通过概率分布和采样机制（如 temperature、top-k、top-p）逐 token 生成文本，水印可以通过微妙地偏置这些采样决策来嵌入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Text_watermarking">Text watermarking - Wikipedia</a></li>
<li><a href="https://gate.ai/blog/how-llms-generate-text-tokens-probabilities-and-sampling-mechanisms">How LLMs Generate Text: Tokens, Probabilities, and Sampling ...</a></li>
<li><a href="https://arxiv.org/html/2504.03765v1">Watermarking for AI Content Detection: A Review on Text ...</a></li>

</ul>
</details>

**标签**: `#AI watermarking`, `#LLM`, `#Machine Learning`, `#AI safety`, `#Tutorial`

---

<a id="item-6"></a>
## [单张 RTX 5090 实测 Qwen3.8-27B NVFP4 真 262K 上下文](https://www.reddit.com/r/LocalLLaMA/comments/1vvl7pc/single_rtx_5090_qwen3827b_nvfp4_at_a_real_262k/) ⭐️ 8.0/10

一位 Reddit 用户发布了完全可复现的 vLLM 0.27.1 配置，在单张 RTX 5090 上以 NVFP4 量化运行 Qwen3.8-27B，完整容纳 262,144 token 上下文，同时还保留了视觉、FP8 KV cache 和前缀缓存。系统在 1K 上下文下解码速度达到 77.2 tok/s，在 128K resident 上下文下为 64.7 tok/s。 这表明真正的 262K token 上下文窗口不再局限于数据中心硬件，消费级显卡也能实现，从而降低了本地长上下文智能体和研究的使用门槛。文章还提供了具体可测的性能数据，有助于其他用户和开发者优化自己的部署。 该模型是 JonathanColetti/Qwen3.8-27B-Uncensored 的 NVFP4 ModelOpt 导出，固定 revision 为 e5ff4986938dcd0dd05ab4cce89da1b052be6ce3，检查点 19.18 GiB，并保留视觉塔和 MTP 头。混合架构包含 48 层 Gated DeltaNet 和 16 层全注意力；262,000 token 的 prefill 耗时 166 秒，前缀缓存的冷启动到缓存 TTFT 加速比为 22.3 倍。

reddit · r/LocalLLaMA · /u/Fz1zz · 8月22日 19:16

**背景**: NVFP4 是 NVIDIA ModelOpt 用于量化 LLM 权重的 4 位浮点格式，相比 FP8 可进一步减半显存占用，同时保持较好质量。Gated DeltaNet 是一种线性注意力变体，通过带门控的 delta 规则更新状态，让大部分层能以高效方式扩展上下文，同时保留少量全注意力层以保证精度。RTX 5090 拥有 32 GB 显存，此前很难在完整上下文下容纳 27B 模型，而 NVFP4 加混合注意力正是本套配置能够成功的关键。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/NVIDIA/Model-Optimizer">GitHub - NVIDIA / Model -Optimizer: A unified library of SOTA model ...</a></li>
<li><a href="https://sebastianraschka.com/llms-from-scratch/ch04/08_deltanet/">Gated DeltaNet | Sebastian Raschka, PhD</a></li>
<li><a href="https://tensara.org/problems/nvfp4-quantize">NVFP 4 Quantization | Tensara</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#RTX 5090`, `#Qwen3.8-27B`, `#Long Context`, `#NVFP4`

---

<a id="item-7"></a>
## [为何本地 LLM 显得更笨：配置与量化是关键](https://forum.level1techs.com/t/why-your-local-llm-feels-dumber-than-it-is/253917) ⭐️ 7.0/10

Level1Techs 论坛上的讨论剖析了本地运行的 LLM 为何表现不如预期，指出差距主要来自量化、推理参数和服务软件的选择，而非模型本身的质量。社区成员报告称，经过正确配置的模型（如 MacBook Pro 上的 Qwen 3.8 27B MLX）表现十分出色。 理解这些因素可以帮助实践者在无需更换模型的情况下显著提升本地 LLM 的表现。同时也会影响到 Ollama、vLLM、sglang 等工具的选择，因为它们在吞吐量和输出质量上都会对实际应用产生影响。 社区成员提到了具体的量化格式（如 Q4_K_P、NVFP4）和服务引擎，其中一位用户通过 sglang 在 5090 上实现了 150+ tokens/s。关于 Ollama 的推理质量是否与 vLLM 或 sglang 有差异存在争论，Ollama 因易用性受到青睐，但其质量也受到质疑。

hackernews · felineflock · 8月22日 18:14 · [社区讨论](https://news.ycombinator.com/item?id=49402232)

**背景**: 本地 LLM 通常通过量化压缩以在消费级硬件上运行，但过于激进的量化会降低输出质量。推理参数（如 temperature、top_p、上下文长度）以及服务框架也会影响用户对模型智能程度的感知。Ollama 因安装设置简单而成为本地部署的热门工具，而 vLLM 和 sglang 则侧重于高吞吐量服务与更先进的分批处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/what-llm-quantization-simply-explained-simon-frey-ybdzf">What is LLM quantization ? Simply explained .</a></li>
<li><a href="http://saumitra.me/2024/2024-03-03-llm-inference-parameters/">LLM Inference Parameters - Saumitra's Blog</a></li>
<li><a href="https://dev.to/primghostdev/run-your-own-ai-model-locally-a-practical-ollama-setup-guide-2026-2kk9">Run Your Own AI Model Locally: A Practical Ollama Setup Guide ...</a></li>

</ul>
</details>

**社区讨论**: 讨论整体氛围积极，用户分享了令人印象深刻的实际体验，例如在 4090 上运行 Qwen3.8 无审查版应对 CTF 挑战。一位用户为 Ollama 的便利性辩护，同时质疑其可能存在的质量差异；另一位用户则强调 sglang 的速度优势。还有用户开玩笑地询问讨论中提到的“不愉快的数学”版本。

**标签**: `#LLM`, `#local-inference`, `#quantization`, `#Ollama`, `#benchmarking`

---

<a id="item-8"></a>
## [macOS 27 弃用 hdiutil，改用 diskutil image](https://lapcatsoftware.com/articles/2026/8/7.html) ⭐️ 7.0/10

苹果在 macOS 27（Golden Gate）中弃用了命令行工具 hdiutil。hdiutil 的手册页现在指出，所有磁盘映像操作都应改用 diskutil image。 这对依赖 hdiutil 编写磁盘映像脚本的开发者和管理员意义重大。这标志着苹果在持续整合命令行工具，并可能最终移除 hdiutil，尽管 Xcode 等旧分发格式仍在使用已弃用的 xip。 弃用意味着 hdiutil 可能不再获得更新，diskutil image 提供 attach、create、resize、info 和 chpass 等子命令。社区评论者指出，hdiutil 曾是创建 RAM 磁盘的唯一方式，因此相关工作流可能受影响。

hackernews · zdw · 8月22日 19:04 · [社区讨论](https://news.ycombinator.com/item?id=49402741)

**背景**: hdiutil 是 macOS 中长期使用的命令行工具，用于管理 .dmg、.iso、.cdr 等磁盘映像文件，可以创建、挂载、转换、压缩和验证磁盘映像。苹果通常只弃用工具但不会立即移除——例如 xip 已弃用很久，但 Xcode 仍以该格式分发。这一模式表明 hdiutil 可能会在 macOS 中继续存在很多年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://keith.github.io/xcode-man-pages/hdiutil.1.html">HDIUTIL (1)</a></li>
<li><a href="https://iboysoft.com/wiki/hdiutil.html">What is hdiutil & How to Use It to Convert DMG to ISO</a></li>

</ul>
</details>

**社区讨论**: 评论者对 hdiutil 会真正消失持怀疑态度，并引用苹果对 xip 的历史做法。一些人对苹果的维护优先级表示不满，调侃一家万亿美元公司却不愿花几个工程小时来维护这个工具；另一些人则将此次弃用视为苹果在处理 bug 报告时态度敷衍的一部分。

**标签**: `#macOS`, `#hdiutil`, `#deprecation`, `#Apple`, `#developer tools`

---

<a id="item-9"></a>
## [编程代理：验证胜过逐行审查](https://simonwillison.net/2026/Aug/22/more-than-just-code-review/) ⭐️ 7.0/10

西蒙·威利森指出，高效使用编程代理的关键在于自信地给出修改指令，并验证据此做出的更改是否已正确落实，而无需逐行审查代码。文章强调，除了逐行检查之外，还有其他的验证方法。 这一点很重要，因为随着 AI 编程代理逐渐普及，开发者需要有效验证 AI 生成代码的实用策略。从全面审查转向结果验证，可以在保证质量的同时节省时间。 威利森提到，逐行审查有时是必要的，但他认为其他验证方式同样可以达到目的。他指出，逐行检查从来都不是验证软件更改的最有效方式。

rss · Simon Willison · 8月22日 15:56

**背景**: 编程代理是基于自然语言指令编写、修改和测试代码的 AI 工具，例如 OpenAI 的 Codex 和 Cursor。代理工程是指运用工程专业知识来监督 AI 代理完成软件开发过程的实践，由人类定义目标和约束，代理负责具体实现。随着这些工具的发展，开发者的角色从编写代码转向指定更改并验证结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-engineering">What is agentic engineering? - IBM</a></li>
<li><a href="https://www.glideapps.com/blog/what-is-agentic-engineering">What is agentic engineering? How AI engineering has evolved ...</a></li>

</ul>
</details>

**标签**: `#code-review`, `#coding-agents`, `#generative-ai`, `#agentic-engineering`, `#ai`

---

<a id="item-10"></a>
## [为何仿真正在接管：性能略逊 10%，成本百倍低，速度快万倍](https://www.latent.space/p/ainews-10-worse-100x-cheaper-10000x) ⭐️ 7.0/10

文章认为，仿真正在成为 AI 领域的主导范式，尽管性能略有下降，但其成本更低、速度更快。文章将这一论点从模型训练延伸到递归自我改进（RSI），认为仿真将推动 AI 进步。 这种转变可能使 AI 研究更加普及，并加速迭代周期，影响 AI/ML 从业者、机器人技术及系统研究人员。成本与性能的权衡可能成为扩展 AI 能力的主流方法。 “性能差 10%，成本低 100 倍，速度快 10000 倍”这一表述强调了基于仿真的方法的务实权衡。sim-to-real 迁移和域随机化等技术有助于弥合仿真与现实之间的差距，使这种方法日益可行。

rss · Latent Space · 8月22日 07:36

**背景**: 递归自我改进（RSI）是一种假设过程，即 AI 系统改进自身能力，可能最终导致超级智能。基于仿真的训练（AI 智能体在虚拟环境中学习）早已用于机器人和强化学习领域。仿真与现实的差距（即 sim-to-real gap）一直是一个主要挑战，但域随机化等技术已改善了迁移效果。文章认为，由于成本和速度优势超过了适度的性能损失，仿真如今有望占据主导地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/transferring-industrial-robot-assembly-tasks-from-simulation-to-reality/">Transferring Industrial Robot Assembly Tasks from Simulation to ...</a></li>
<li><a href="https://www.alphaxiv.org/abs/2409.06613">DemoStart: Demonstration-led auto-curriculum applied to sim - to - real ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#simulation`, `#cost-efficiency`, `#machine-learning`, `#analysis`

---

<a id="item-11"></a>
## [TikTok 同意支付 4 亿美元和解美国儿童隐私诉讼](https://thehackernews.com/2026/08/tiktok-agrees-to-400-million-settlement.html) ⭐️ 7.0/10

美国司法部宣布，字节跳动旗下的 TikTok 将支付 4 亿美元，以和解一起指控其违反美国儿童隐私法的 2024 年诉讼。和解金包括立即支付的 3 亿美元，以及在撤销先前同意法令后再支付的 1 亿美元。 这是涉及大型社交媒体平台的数额最大的儿童隐私和解案之一，标志着美国对儿童数据保护的执法力度加强。这可能为平台如何处理未成年人数据及承担监管后果树立先例。 和解金结构为：3 亿美元立即支付，另有 1 亿美元以撤销先前针对该公司下达的同意法令为条件。该诉讼于 2024 年提起，司法部于一个周五宣布了这项协议。

rss · The Hacker News · 8月22日 14:32

**背景**: 美国儿童隐私法，特别是《儿童在线隐私保护法》（COPPA），要求在线服务在收集 13 岁以下儿童数据前必须获得父母同意。TikTok 此前曾面临监管行动，包括 2019 年因违反 COPPA 与 FTC 达成的和解，该和解很可能涉及本次协议中所提到的同意法令。字节跳动是一家中国科技公司，全球拥有 TikTok。

**标签**: `#privacy`, `#regulation`, `#TikTok`, `#child safety`, `#legal settlement`

---

<a id="item-12"></a>
## [黑客利用安卓车机更新应用植入代理僵尸网络](https://www.bleepingcomputer.com/news/security/hackers-infect-android-car-head-units-with-proxy-botnet-malware/) ⭐️ 7.0/10

一场供应链攻击正在滥用安卓车载中控（Android 车机）上的合法更新应用来植入恶意软件。该恶意软件会将设备纳入代理僵尸网络，或利用它们进行广告欺诈。 这是针对嵌入式/IoT 设备的新型供应链攻击载体，而这类设备通常没有安全团队监控。它表明攻击者可以将车主的设备悄悄变成收费代理网络的一部分，并带来广告欺诈和隐私风险。 恶意软件通过合法的设备更新应用下发，说明攻击者篡改了更新通道，而不是依赖第三方应用商店。被控制的车机会被当作住宅代理来转发匿名流量，或被用于广告欺诈活动。

rss · BleepingComputer · 8月22日 14:14

**背景**: 安卓车机是由中国厂商大量生产的后装车载信息娱乐系统，例如 FF_866X 这类型号常配备联发科处理器，并通过 AliExpress 等平台广泛销售。代理僵尸网络是指被攻陷的住宅设备组成的网络，其 IP 地址被出租用作看似合法的代理，Spur Intelligence 的文章对此有详细说明。这类嵌入式设备始终在线且更新机制往往不严格，因此正成为攻击者青睐的目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/FF_866X_Android_car_head_unit">FF_866X Android car head unit</a></li>
<li><a href="https://medium.com/spur-intelligence/residential-proxies-the-legal-botnet-that-nobody-talks-about-4470cae7e3c">Residential Proxies : The “Legal” Botnet That Nobody Talks... | Medium</a></li>
<li><a href="https://www.aliexpress.com/w/wholesale-android-car-headunit.html">android car headunit - Buy android car headunit with free shipping...</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#malware`, `#Android`, `#IoT`

---