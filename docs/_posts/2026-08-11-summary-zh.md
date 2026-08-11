---
layout: default
title: "Horizon Summary: 2026-08-11 (ZH)"
date: 2026-08-11
lang: zh
---

> 从 64 条内容中筛选出 20 条重要资讯。

---

1. [OpenAI 推出 GPT-5.6-Cyber，通过 Daybreak Red 扩展授权安全测试](#item-1)
2. [OpenAI 因网络安全能力跃升暂停 Astra 内部工作](#item-2)
3. [CISA 警告 LoadMaster 命令注入漏洞正遭积极利用](#item-3)
4. [vLLM v0.27.0 发布，支持 Kimi K3 并升级至 PyTorch 2.13](#item-4)
5. [Meta 发布 Muse Glimmer：30B 开源智能体模型，专为本地设备优化](#item-5)
6. [扎克伯格批评封闭 AI 对手，重申 Meta 开源模型路线](#item-6)
7. [利用超长中断指令攻破系统管理模式（SMM）](#item-7)
8. [Mistral 获美国专利：代码实现的工具调用](#item-8)
9. [伊利诺伊州新法要求操作系统承担年龄验证义务，Linux 受波及](#item-9)
10. [Python 的 pyca/cryptography 库新增 ML-KEM 与 ML-DSA 支持](#item-10)
11. [NVIDIA Magpie TTS：低延迟多语言语音智能体的开放权重方案](#item-11)
12. [让知识蒸馏在规模化部署中更具成本效益](#item-12)
13. [CISA 发布关于 Gunra 勒索软件双重勒索 RaaS 的公告](#item-13)
14. [新型攻击击破通行密钥保护，恢复同步私钥](#item-14)
15. [恶意的 Solidity Pro VS Code 扩展窃取加密钱包和凭据](#item-15)
16. [黑客经由私有 APN 入侵波兰热电厂](#item-16)
17. [BdThemes 插件供应链攻击创建恶意管理员账户](#item-17)
18. [CISA：勒索软件团伙正在利用 SonicWall SMA1000 漏洞](#item-18)
19. [Aeternum 僵尸网络利用 Polygon 区块链实现去中心化指挥与控制](#item-19)
20. [中国关联黑客 Storm-1175 利用 N-Central 漏洞部署新型 StormEncryptor 勒索软件](#item-20)

---

<a id="item-1"></a>
## [OpenAI 推出 GPT-5.6-Cyber，通过 Daybreak Red 扩展授权安全测试](https://openai.com/index/expanding-daybreak-as-the-cyber-defense-window-narrows) ⭐️ 9.0/10

OpenAI 推出了 GPT-5.6-Cyber，这是一款专用于网络安全的模型，通过 Daybreak Red 提供授权漏洞研究、漏洞利用验证和安全测试。此次扩展将 Daybreak 分为 Blue 和 Red 两个层级，其中 Red 提供这一新的前沿网络模型。 这标志着 AI 驱动的安全测试取得重大进展，在 AI 主导攻击不断升级的背景下，让经过审查的安全团队能够使用前沿模型。它可能通过严格治理下更快、更有效的漏洞发现和利用验证，改变网络防御范式。 GPT-5.6-Cyber 基于 GPT-5.6 Sol 构建，并经过训练以减少对授权漏洞研究和利用链任务的拒绝。根据 OpenAI 的 Preparedness Framework，目前仅限经国家网络总监办公室批准的特定企业合作伙伴使用。

rss · OpenAI Blog · 8月10日 10:00

**背景**: Daybreak 是 OpenAI 将前沿 AI 模型交予经审查的网络安全专业人士使用的项目。该项目提供对专用模型的访问，用于授权的防御性和攻击性安全工作。GPT-5.6-Cyber 是 Daybreak Red 中的专用模型，旨在以更少的拒绝执行授权漏洞研究、漏洞利用验证和安全测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/expanding-daybreak-as-the-cyber-defense-window-narrows/">Expanding Daybreak as the Cyber Defense Window Narrows | OpenAI</a></li>
<li><a href="https://techcrunch.com/2026/08/10/as-ai-led-attacks-multiply-openai-launches-a-new-cyber-model/">As AI-led attacks multiply, OpenAI launches a new cyber... | TechCrunch</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Cybersecurity`, `#AI Model`, `#GPT-5.6-Cyber`, `#Daybreak Red`

---

<a id="item-2"></a>
## [OpenAI 因网络安全能力跃升暂停 Astra 内部工作](https://thehackernews.com/2026/08/openais-next-ai-model-astra-shows-cyber.html) ⭐️ 9.0/10

OpenAI 宣布，在内部评估发现即将推出的 Astra 模型在智能体编码和网络安全方面取得显著进展后，将暂停部分涉及该模型的内部活动。该公司还正在为高能力模型实施新的安全控制措施。 这一事件凸显了前沿 AI 模型带来的日益增长的网络安全风险，因为连 OpenAI 自己都认为有必要暂停。这表明，随着模型逐渐接近自主网络能力，开发者和监管机构都需要更强大的保障措施。 内部评估特别指出了智能体编码和网络安全方面的进展，促使 OpenAI 采取安全控制措施，例如对涉及高能力模型的活动进行隔离。Astra 是 OpenAI 尚未发布的模型系列，被描述为该公司的“下一代主要模型”，首次在 2026 年 8 月 1 日的研究帖子中亮相。

rss · The Hacker News · 8月10日 05:50

**背景**: 智能体编码是一种软件开发方法，由自主 AI 智能体在极少人工干预的情况下规划、编写、测试和修改代码。Astra 是 OpenAI 尚未发布的模型系列，据称是其“下一代主要模型”；早期报告显示它已产生了新的数学成果。这些能力与高级编码自主性相结合，引发了对可能被滥用于网络攻击的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-coding">What is Agentic Coding? | IBM</a></li>
<li><a href="https://aiwiki.ai/wiki/openai_astra">Astra (OpenAI) - AI Wiki</a></li>
<li><a href="https://explainx.ai/blog/openai-astra-next-major-model-announcement-2026">OpenAI Astra: Next Major Model Explained | explainx.ai Blog</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI Safety`, `#Cybersecurity`, `#Astra`, `#Agentic Coding`

---

<a id="item-3"></a>
## [CISA 警告 LoadMaster 命令注入漏洞正遭积极利用](https://www.bleepingcomputer.com/news/security/cisa-warns-of-critical-progress-loadmaster-flaw-exploited-in-attacks/) ⭐️ 9.0/10

CISA 发布警告称，攻击者正在积极利用 Progress Kemp LoadMaster 中的一个严重级命令注入漏洞。该通告敦促各组织立即应用厂商补丁。 由于该漏洞正被野外利用，受影响的 LoadMaster 设备面临立即被完全入侵的风险。对于依赖 LoadMaster 进行应用交付和负载均衡的企业而言，这一警告尤其重要。 该漏洞是一个命令注入漏洞，允许攻击者在底层操作系统上执行任意系统命令。CISA 的警告表明存在真实世界的利用，因此各组织应优先进行修补并检查是否存在入侵指标。

rss · BleepingComputer · 8月10日 09:49

**背景**: 命令注入是一种攻击方式，应用程序将不安全的用户输入传递给系统 shell，使攻击者能够执行任意操作系统命令。Progress Kemp LoadMaster 是一种负载均衡器和应用交付控制器，用于在服务器之间分配网络流量；这类设备中的严重漏洞可能使核心基础设施暴露于远程攻击之下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://owasp.org/www-community/attacks/Command_Injection">Command Injection - OWASP Foundation</a></li>
<li><a href="https://www.ecnetworker.com/kemp-loadmaster/">KEMP LoadMaster ® ADC與負載平衡器 – 易璽科技 ECNETWORKER</a></li>

</ul>
</details>

**标签**: `#security`, `#CVE`, `#LoadMaster`, `#CISA`, `#command injection`

---

<a id="item-4"></a>
## [vLLM v0.27.0 发布，支持 Kimi K3 并升级至 PyTorch 2.13](https://github.com/vllm-project/vllm/releases/tag/v0.27.0) ⭐️ 8.0/10

vLLM v0.27.0 已发布，包含 561 个提交和 242 位贡献者。该版本为 Kimi K3 提供全栈支持，升级至 PyTorch 2.13.0/TorchVision 0.28.0/Triton 3.7.1，并深化了 SM100 上的 FlashAttention 4 集成。 此版本通过支持 Kimi K3、Qwen3.5 等前沿模型大幅扩展了 vLLM 的模型覆盖范围，同时对核心框架依赖进行了现代化升级。性能优化和容错特性进一步巩固了 vLLM 作为生产级 LLM 推理引擎的地位。 Kimi K3 集成包括 AttnRes 内核、DeepGEMM 支持、DSpark AR 融合和可选的共享专家分片。其他亮点包括 Qwen3.5 纯文本模型、K-EXAONE-2.0-750B-A37B、VaultGemma，以及 Model Runner V2 扩展到嵌入/分类任务。

github · khluu · 8月10日 21:18

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理与服务引擎，使用 PagedAttention 管理 KV 缓存内存。Kimi K3 是月之暗面（Moonshot AI）推出的 2.8T 参数开源模型，拥有 1M token 上下文窗口，基于 Kimi Delta Attention 和 Attention Residuals 构建。FlashAttention 4 为 NVIDIA SM100 GPU 提供优化的注意力内核，并新增 JIT 预热以避免首次请求的编译延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm.ai/blog/2026-07-22-kimi-k3-preview">A Preview of Production-Scale Kimi K3 Support on vLLM</a></li>
<li><a href="https://www.kimi.com/ai-models/kimi-k3">Kimi K3: 2.8T Open Model for Coding & Knowledge Work</a></li>
<li><a href="https://github.com/deepseek-ai/DeepGEMM">GitHub - deepseek-ai/DeepGEMM: DeepGEMM: clean and efficient ...</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#release`, `#PyTorch`, `#FlashAttention`

---

<a id="item-5"></a>
## [Meta 发布 Muse Glimmer：30B 开源智能体模型，专为本地设备优化](https://research.meta.ai/blog/introducing-muse-glimmer-open-agentic-model) ⭐️ 8.0/10

Meta 超级智能实验室发布了 Muse Glimmer，这是一个 300 亿参数、采用 Apache 2.0 许可的开源权重稠密模型，专为“常驻本地”的智能体工作流优化。Meta 还表示不久将发布更大规模基础模型 Muse Spark 1.2 的权重。 这意味着开发者有了一个可在本地自托管、用于自主编码和工具调用智能体的实用选择，无需依赖云服务，有望降低成本并提升隐私。它还加剧了与 Qwen 等模型在开源权重领域的竞争，同时帮助 Meta 巩固其作为领先的美国开源权重提供商的地位。 Muse Glimmer 是一个稠密(dense)30B 视觉-语言模型而非 MoE，官方称其具有较强的函数调用能力；Unsloth 等社区工具已提供动态量化版本用于本地部署。它还是 Meta 超级智能实验室发布的首个开源模型，据《纽约时报》报道，它与更大的 Muse Spark 几乎相同，具备代码、文本和图像生成能力。

hackernews · riordan · 8月10日 10:10 · [社区讨论](https://news.ycombinator.com/item?id=49241679)

**背景**: Meta 此前发布过 Llama 等开源权重模型，其新的 Muse 系列大致分为大型基础模型和用于边缘部署的较小蒸馏变体。智能体工作流要求模型具备多步规划、工具/函数调用和对话记忆能力；在本地运行这些模型可使其“常驻在线”——始终可用、保护隐私，且无需按 token 付费。稠密模型每个 token 都会激活全部参数，这与混合专家(MoE)设计不同，在普通硬件上表现更可预测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.meta.ai/blog/introducing-muse-glimmer-open-agentic-model">Introducing Muse Glimmer: An Open Agentic Model That Runs on ...</a></li>
<li><a href="https://unsloth.ai/docs/models/muse-glimmer">Muse Glimmer - How to Run Locally | Unsloth Documentation</a></li>
<li><a href="https://www.nytimes.com/2026/08/10/technology/meta-ai-open-source.html">Meta Unveils an Open Version of Its Most Powerful A.I. Model</a></li>

</ul>
</details>

**社区讨论**: 评论区反响热烈：有人把它与即将发布的 Qwen3.8 27B 对比，也有人认为承诺开源 Muse Spark 1.2 权重才是对自托管者而言“更大的新闻”。一些用户已在 32GB Mac Mini 上用 Ollama 实测，认为可用但推理较慢；还有人用“大型机时代转向小型便携大脑”来类比 AI 从数据中心走向本地设备，并质疑 Meta 此举意在对抗中国开源权重模型竞争的战略动机。

**标签**: `#AI`, `#LLM`, `#Meta`, `#open-weights`, `#local-inference`

---

<a id="item-6"></a>
## [扎克伯格批评封闭 AI 对手，重申 Meta 开源模型路线](https://www.ft.com/content/4e3957f8-ea7c-4c46-a3de-cdce8e526878) ⭐️ 8.0/10

马克·扎克伯格发表声明，公开批评“封闭”的 AI 竞争对手，重申 Meta 对开放（开放权重）AI 模型的承诺，并链接到 Meta 的宣言页面“未来属于每个人”。他还反驳了关于 AI 的悲观论调，认为权力集中并非安全之路。 作为 Llama 开放权重模型系列的创造者，Meta CEO 的公开立场可能进一步推动行业向开放模型倾斜，并对 OpenAI 和谷歌等封闭实验室形成压力。这对依赖可下载、可定制 AI 模型而非仅限 API 访问的开发者和企业具有重要意义。 扎克伯格的言论发表之际，Meta 正“回归开放模型”，表明在先前争论之后的战略调整。值得注意的是，像 Llama 这样的开放权重模型并非完全开源——训练数据和代码往往仍是专有的——这一区别是开放与封闭之争的核心。

hackernews · root-parent · 8月10日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=49243880)

**背景**: AI 模型权重是在大量数据训练过程中学到的参数，编码了模型的知识和行为。开放权重模型（如 Meta 的 Llama、Mistral 和 Gemma）公开这些权重，任何人都可以下载、运行和微调；而像 GPT-4 和 Claude 这样的封闭模型只能通过 API 访问。开放与封闭之间的分歧已成为 AI 未来的核心商业和哲学之争，开源倡导者主张透明和竞争，封闭模型支持者则强调安全和控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://enigmatica.ai/glossary/model-weights">What Is Model Weights ? Definition & Guide</a></li>
<li><a href="https://www.gptcrunch.com/blog/open-source-vs-closed-source-ai-models">Open Source vs Closed Source AI Models: A Comprehensive ...</a></li>
<li><a href="https://www.cbc.ca/lite/story/9.7287025">What is open - weight AI , the tech behind Kimi K3 that's turning heads...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论总体上支持开放权重，有用户称赞 Meta 在 2023 年用 Llama 开启了开源竞赛，并认为更多开放模型是净积极的事。然而，也有人对扎克伯格的动机表示怀疑，认为他的立场听起来像“我输了，所以想改规则”；还有人指出，如果 LLM 已经商品化，封闭模型可能面临生存挑战。

**标签**: `#AI`, `#Open Source`, `#Meta`, `#Zuckerberg`, `#LLMs`

---

<a id="item-7"></a>
## [利用超长中断指令攻破系统管理模式（SMM）](https://github.com/xoreaxeaxeax/smiiiiiiiiiiiiiiii) ⭐️ 8.0/10

安全研究员 xoreaxeaxeax 发布了一个概念验证，通过执行一条超长的中断指令来攻破系统管理模式（SMM）。该技术在 smiiiiiiiiiiiiiiii 仓库中展示，打破了 SMM 的运行假设，从而暴露了这个不可见的高权限执行环境。 SMM 的权限等级高于虚拟机监控器和操作系统，因此这一层的漏洞可能导致固件被篡改，进而造成难以清除的持久性劫持。该研究表明，即使是简单构造的错误指令也能威胁到一种设计上对用户不可见且不可控制的 CPU 模式。 该概念验证需要 root 权限，因此仅凭此技术无法远程利用。仓库内容强调，中断指令必须“非常、非常、非常长”，并指出固件设计者早已预料到这种攻击，却将超时决策交给了平台厂商。

hackernews · WhiteDawn · 8月10日 16:03 · [社区讨论](https://news.ycombinator.com/item?id=49245491)

**背景**: SMM（系统管理模式）是 x86 CPU 的一种特殊运行模式，有时被称为 ring -2。它会暂停包括操作系统在内的所有正常执行，转而运行高权限固件代码，用于电源管理、硬件控制等任务。由于 SMM 运行在操作系统无法检查的受保护内存区域中，因此一旦 SMM 被攻破，后果极其严重。虽然微软的 System Guard Secure Launch 和 SMM 隔离等现代防御机制有助于保护平台，但这项研究揭示了 SMM 在应对超长运行指令时更基本的缺陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/System_Management_Mode">System Management Mode - Wikipedia</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2020/11/12/system-management-mode-deep-dive-how-smm-isolation-hardens-the-platform/">System Management Mode deep dive: How SMM isolation hardens ...</a></li>
<li><a href="https://gist.github.com/yawaworks/ab53fa6760596592b48de9cf398dc297">Exploiting System Management Mode with a very long interrupt</a></li>

</ul>
</details>

**社区讨论**: 评论者们讨论了该技术是否算真正的漏洞，因为它需要 root 权限；有人主张这更像是“夺回对自己硬件的控制权”，并认为 SMM 对用户不可见是邪恶的设计。还有人提到了相关的 asm-hall-of-shame 仓库，引用了固件代码表明超时问题被推给厂商，并质疑超长指令如何转化为实际可利用的攻击。

**标签**: `#security`, `#SMM`, `#x86`, `#firmware`, `#exploit`

---

<a id="item-8"></a>
## [Mistral 获美国专利：代码实现的工具调用](https://patentsgazette.uspto.gov/week26/OG/html/1547-5/US12670045-20260630.html) ⭐️ 8.0/10

美国专利商标局(USPTO)于 2026 年 6 月 30 日授予 Mistral 专利 US12670045，涉及“代码实现的工具调用”——LLM 的一项核心能力。该专利的授予引发了关于软件专利有效性和现有技术的争议。 工具调用支撑着 AI 行业中广泛使用的 LLM 智能体和外部集成，该专利可能会影响开发者和公司实现这一常见技术的方式。批评者担心，这一领域宽泛的软件专利可能阻碍创新，而非保护有实际价值的投入。 该专利公布于美国专利商标局《官方公报》第 US12670045 号(2026 年第 26 周)。评论者指出，该技术本质上类似于远程过程调用(RPC)，并对其新颖性提出质疑；还有人指出，这类软件功能在欧盟基本无法获得专利。

hackernews · theanonymousone · 8月10日 13:29 · [社区讨论](https://news.ycombinator.com/item?id=49243397)

**背景**: 函数调用或工具调用是大语言模型的能力，它把自然语言转换为 API 调用，让模型能够在外部系统中检索数据或执行操作。这是一种被广泛记录的技术，例如 OpenAI 的函数调用文档和提示工程指南中都有介绍。在美国专利法中，现有技术指在申请日之前已经公开或可获得的、能证明发明已被知晓的任何证据；若发明不具备新颖性或属于显而易见，现有技术可导致专利无效。软件专利一直存在争议，因为批评者认为其中许多专利保护的是显而易见的想法，而非昂贵的研究投入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prior_art">Prior art - Wikipedia</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/function-calling">Function calling | OpenAI API</a></li>
<li><a href="https://www.promptingguide.ai/applications/function_calling">Function Calling with LLMs | Prompt Engineering Guide</a></li>

</ul>
</details>

**社区讨论**: 评论者几乎一致批评这项专利：有人称软件专利是“祸害”，认为没有一个值得授予；有人则要求提供现有技术，因为“RPC 调用绝不可能是新颖的”。另有人认为这是防御性专利申请，因为该功能在欧盟基本无法获得专利。一位构建自定义 harness 的开发者表示，他们原本就计划解析并在本地执行工具调用，以获得最大控制权。

**标签**: `#patents`, `#Mistral`, `#AI`, `#software law`, `#tool calls`

---

<a id="item-9"></a>
## [伊利诺伊州新法要求操作系统承担年龄验证义务，Linux 受波及](https://linuxstans.com/illinois-hb5511-operating-system-age-verification/) ⭐️ 8.0/10

伊利诺伊州通过了 HB5511 法案，要求操作系统提供商实现年龄验证机制，Linux 发行版也被纳入适用范围。该法律义务施加在操作系统层面，而非单个网站或应用。 这标志着首批将年龄验证法律责任直接施加给操作系统的法律之一，而这一要求与去中心化、由社区开发的 Linux 发行版难以契合。若该法案成为模板，可能迫使开源项目要么加入验证功能、要么限制访问，对隐私和采用率影响深远。 关于该法律的讨论指出，它似乎只要求用户自行声明年龄，而非基于证件的验证，但实际执行中的问题仍然很大。Linux 生态的多样性——从志愿者维护者到内核不含网络驱动的离线优先发行版——使得任何统一合规机制都极难实现。

hackernews · speckx · 8月10日 20:20 · [社区讨论](https://news.ycombinator.com/item?id=49249150)

**背景**: 年龄验证立法以往主要针对色情网站，但新一波提案将义务转向操作系统提供商。加利福尼亚州曾审议 AB-1043，英国已出现苹果在操作系统层面要求部分 iPhone 功能进行年龄验证的做法，而埃莉斯·斯特凡尼克支持的美国联邦法案也将在全国范围推行操作系统级年龄验证。这些动态解释了为什么伊利诺伊州针对操作系统的法律会受到开源社区密切关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://discussion.fedoraproject.org/t/a-practical-architectural-solution-to-os-level-age-verification-laws/183387">A Practical Architectural Solution to OS-Level Age Verification Laws - Fedora Discussion</a></li>
<li><a href="https://proton.me/blog/age-verification-operating-system">When age verification moves into your operating system | Proton</a></li>
<li><a href="https://itsfoss.com/news/os-level-age-verification-across-us/">Oh No! Now A Federal Bill Wants OS-Level Age Verification for Everyone in the USA</a></li>

</ul>
</details>

**社区讨论**: 评论几乎一边倒地持反对态度：一位 Linux 发行版创始人表示绝不会实施这一要求，也有人认为法律设计思路颠倒，并指出该法只要求用户自行声明年龄。还有评论者质疑操作系统级年龄验证背后的政治力量，并分享了 agelesslinux.org 等资源。

**标签**: `#Linux`, `#age verification`, `#legislation`, `#privacy`, `#open source`

---

<a id="item-10"></a>
## [Python 的 pyca/cryptography 库新增 ML-KEM 与 ML-DSA 支持](https://www.schneier.com/blog/archives/2026/08/python-now-has-a-post-quantum-encryption-library.html) ⭐️ 8.0/10

后量子加密现在只需一条 pip 命令即可用于整个 Python 生态：pyca/cryptography 库已加入对 NIST 标准密钥封装原语 ML-KEM 和数字签名原语 ML-DSA 的支持。这项工作由 Sovereign Tech Agency 资助，并于 2026 年 6 月 30 日宣布。 这使 NIST 标准的后量子加密可通过一个广泛使用的库提供给海量开发者，降低了实现早期加密敏捷性的门槛。各机构可以在量子计算机构成实际威胁之前开始迁移，以防范“先收割、后解密”的攻击。 ML-KEM（FIPS 203）是原称 Kyber 的密钥封装机制；ML-DSA（FIPS 204）是基于模块格的数字签名算法。该实现位于 pyca/cryptography 中，开发者只需常规执行 pip install cryptography 即可使用。

rss · Schneier on Security · 8月10日 11:02

**背景**: 后量子密码学（PQC）指被认为能抵御未来量子计算机攻击的算法，不同于 RSA、Diffie-Hellman 或椭圆曲线方案——后者可能被 Shor 算法破解。2024 年，NIST 发布了首批 PQC 标准，其中包括基于格问题的 ML-KEM 和 ML-DSA，它们对经典和量子攻击都有抵抗力。紧迫性并非来自迫在眉睫的量子威胁，而是来自“先收割、后解密”的数据收集，以及加密系统迁移所需的漫长准备时间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ML-KEM">ML-KEM</a></li>
<li><a href="https://en.wikipedia.org/wiki/ML-DSA">ML-DSA</a></li>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#post-quantum`, `#python`, `#security`, `#ML-KEM`

---

<a id="item-11"></a>
## [NVIDIA Magpie TTS：低延迟多语言语音智能体的开放权重方案](https://huggingface.co/blog/nvidia/magpie-tts-multilingual-voice-agents) ⭐️ 8.0/10

NVIDIA 发布了 Magpie TTS，一个开放权重的多语言文本转语音模型（nvidia/magpie_tts_multilingual_357m），支持 30 多种语言，延迟低于 200 毫秒。该模型已在 Hugging Face 和 NVIDIA NIM 上提供，为开发者提供语音智能体的完整部署控制。 开放权重允许开发者微调模型并自行托管，低延迟则支持实时对话式语音智能体。这减少了对专有 TTS API 的依赖，并为多语言语音应用提供了隐私敏感或离线部署的可能性。 该模型为 357M 参数版本，并集成到 NVIDIA Riva 语音 AI 平台。通过 NVIDIA API 使用该模型时需遵守 NVIDIA API 试用服务条款，而模型权重本身可公开下载。

rss · Hugging Face Blog · 8月10日 16:25

**背景**: 文本转语音（TTS）技术将书面文本转换为语音，多语言 TTS 则将其扩展到多种语言。低延迟对于语音智能体的自然感和响应速度至关重要。开放权重模型允许公众下载和修改模型参数，从而支持自定义微调和本地部署。NVIDIA Riva 是一个基于 GPU 加速的语音 AI 工具包，包含 TTS、语音识别和翻译等功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/nvidia/magpie_tts_multilingual_357m">nvidia / magpie _ tts _multilingual_357m · Hugging Face</a></li>
<li><a href="https://build.nvidia.com/nvidia/magpie-tts-multilingual">magpie - tts -multilingual Model by NVIDIA | NVIDIA NIM</a></li>
<li><a href="https://www.linkedin.com/posts/noellebecker_enhancing-multilingual-human-like-speech-activity-7350647190073094145-wPwJ">NVIDIA releases Riva with Magpie TTS for multilingual voice... | LinkedIn</a></li>

</ul>
</details>

**标签**: `#TTS`, `#multilingual`, `#low-latency`, `#NVIDIA`, `#open-weights`

---

<a id="item-12"></a>
## [让知识蒸馏在规模化部署中更具成本效益](https://huggingface.co/blog/MultiverseComputingCAI/efficient-knowledge-distillation) ⭐️ 8.0/10

这篇 Hugging Face 博客文章介绍了一种降低知识蒸馏计算成本的方法，使其在大规模 AI 部署中变得可行。该方法旨在降低从大型教师模型训练紧凑学生模型的额外开销。 知识蒸馏是模型压缩的关键技术，使较小的模型能够部署在资源受限的硬件上。降低成本使得更多组织能够高效地采用大型模型的能力，减少基础设施成本并支持更广泛的边缘部署。 典型的知识蒸馏需要大型教师模型进行多次前向传播以生成软标签，这计算成本很高。所提出的方法专门针对降低这种开销，同时保持知识迁移的质量。

rss · Hugging Face Blog · 8月10日 10:05

**背景**: 知识蒸馏是一种模型压缩技术，较小的学生模型学习模仿较大的预训练教师模型的行为。教师模型的软输出概率（而非硬标签）被用作训练目标以迁移泛化知识。这使得较小的模型在接近教师模型性能的同时运行成本更低，适用于移动和边缘设备。然而，教师模型本身的评估成本很高，因此高效的蒸馏方法对可扩展性至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation</a></li>

</ul>
</details>

**标签**: `#knowledge distillation`, `#model compression`, `#efficiency`, `#AI/ML`

---

<a id="item-13"></a>
## [CISA 发布关于 Gunra 勒索软件双重勒索 RaaS 的公告](https://www.cisa.gov/news-events/cybersecurity-advisories/aa26-222a) ⭐️ 8.0/10

2026 年 8 月 10 日，CISA 发布公告 AA26-222A，警告名为 Gunra 的勒索软件即服务（RaaS）变种；该变种于 2025 年首次出现，并在 2026 年扩展为 RaaS 运营。公告提供了针对此次双重勒索攻击的技术细节、失陷指标（IOC）以及检测与缓解指导，攻击目标涉及政府和关键基础设施。 这很重要，因为 Gunra 的加盟者正积极攻击政府和关键基础设施领域，一旦得手可能扰乱基本服务并损害公众信任。CISA 的官方指导为防御者提供了可操作的指标和优先事项，有助于抵御不断演变的 RaaS 威胁。 公告强调的关键措施包括：修补面向互联网的 VPN 和 RDP 基础设施中已知被利用的漏洞、实施离线不可变备份，以及进行网络分段以限制横向移动。公告还提供了包含失陷指标的可下载 STIX XML 和 JSON 文件。

rss · CISA Cybersecurity Advisories · 8月10日 12:00

**背景**: 勒索软件即服务（RaaS）是一种网络犯罪商业模式，开发者向加盟者出售或出租勒索软件，由其发起攻击。双重勒索将加密与数据窃取相结合，攻击者威胁在专用泄露网站（DLS）上公布被盗数据，从而获得额外的施压手段。该公告是 CISA“#StopRansomware”系列的一部分，旨在提醒组织防范活跃的勒索软件威胁并提供实用防御措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ransomware_as_a_service">Ransomware as a service - Wikipedia</a></li>
<li><a href="https://www.techtarget.com/searchSecurity/definition/double-extortion-ransomware">What is Double Extortion Ransomware? How to Defend Your ... What Is Double Extortion Ransomware? - Zscaler What is Double Extortion Ransomware? And How to Avoid It Double extortion ransomware: from encryption to blackmail Double Extortion Ransomware: What It Is and How to Respond Double Extortion Ransomware: What It Is, How It Works And How ...</a></li>
<li><a href="https://www.group-ib.com/resources/knowledge-hub/dedicated-leak-sites/">What is a Dedicated Leak Site? | Group-IB Knowledge Hub</a></li>

</ul>
</details>

**标签**: `#ransomware`, `#CISA`, `#cybersecurity`, `#threat intelligence`, `#RaaS`

---

<a id="item-14"></a>
## [新型攻击击破通行密钥保护，恢复同步私钥](https://thehackernews.com/2026/08/new-passkey-attacks-can-recover-synced.html) ⭐️ 8.0/10

研究人员展示了三种独立的攻击方式，在不破解底层密码学的情况下击破了通行密钥（passkey）的保护。所演示的方法包括复用 Windows 暴露的签名认证材料，以及通过受害者机器上已有的恶意软件滥用云端同步的通行密钥系统。 这些发现挑战了通行密钥天然具有防钓鱼性且安全可靠的普遍假设。它们揭示了安全专业人员在部署基于通行密钥的身份验证和防钓鱼 MFA 时必须考虑的实际攻击路径。 这些攻击并未破解密码学原语，而是利用了实现层面的弱点，例如暴露签名认证材料，以及依赖恶意软件可访问的云同步机制。该研究以三项独立工作形式发布，但所提供的摘要中未包含第三种攻击的细节。

rss · The Hacker News · 8月10日 12:25

**背景**: 通行密钥基于 WebAuthn 标准（W3C 发布），利用数字签名而非密码进行用户身份验证。由于认证器只向同一网站注册的凭据提供验证，因此旨在抵御钓鱼攻击。许多实现通过 Apple Keychain 或 Google 等云服务同步通行密钥，提升了便利性，但也引入了新的攻击面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Passkey">Passkey</a></li>
<li><a href="https://practicaldev-herokuapp-com.global.ssl.fastly.net/corbado/what-are-synced-passkeys-ppn">What are Synced Passkeys ? - DEV Community</a></li>
<li><a href="https://www.cisa.gov/sites/default/files/publications/fact-sheet-implementing-phishing-resistant-mfa-508c.pdf">Implementing Phishing-Resistant MFA</a></li>

</ul>
</details>

**标签**: `#passkeys`, `#security`, `#authentication`, `#MFA`, `#vulnerabilities`

---

<a id="item-15"></a>
## [恶意的 Solidity Pro VS Code 扩展窃取加密钱包和凭据](https://thehackernews.com/2026/08/solidity-pro-vs-code-extensions-steal.html) ⭐️ 8.0/10

研究人员标记了两个恶意的 Visual Studio Code 扩展 helper-beeps.solidity-pro 和 web3devtoolsx.solidity-pro，它们会投放浏览器钱包和凭据窃取程序。这些扩展已从 Open VSX 注册表中移除，但之前曾可供用户使用。 这凸显了开发者工具生态系统中的供应链风险，受信任的工具可能被武器化，用来窃取加密货币和敏感凭据。使用 VS Code 兼容编辑器进行 Solidity 开发的开发者应立即审计自己安装的扩展。 恶意扩展的名称为 helper-beeps.solidity-pro 和 web3devtoolsx.solidity-pro。据研究人员称，这些扩展会投放针对浏览器加密钱包的恶意软件并窃取凭据；虽然它们已不在 Open VSX 上，但用户可能仍已安装，或可能从其他来源获取。

rss · The Hacker News · 8月10日 07:38

**背景**: Solidity 是一种静态类型编程语言，专为开发运行在以太坊上的智能合约而设计。Open VSX 是一个开源、厂商中立的 VS Code 兼容扩展注册表，供不依赖微软专有 Visual Studio Marketplace 的编辑器使用。浏览器钱包窃取程序是一类恶意软件，它从加密钱包浏览器扩展和 2FA 扩展中收集内存数据，使攻击者能够绕过安全防护并盗取钱包。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.soliditylang.org/">Home | Solidity Programming Language</a></li>
<li><a href="https://open-vsx.org/">Open VSX Registry</a></li>
<li><a href="https://www.kaspersky.com/resource-center/threats/mars-stealer-malware">What is Mars Stealer Malware</a></li>

</ul>
</details>

**标签**: `#security`, `#VS Code`, `#malware`, `#crypto wallet`, `#supply chain`

---

<a id="item-16"></a>
## [黑客经由私有 APN 入侵波兰热电厂](https://www.bleepingcomputer.com/news/security/hackers-breached-a-small-polish-energy-plant-via-private-apn-last-year/) ⭐️ 8.0/10

去年，黑客利用私有接入点名称（APN）接入运营技术（OT）网络，入侵了波兰一座热电联产厂。该设施为大约 5 万名居民供热。 该事件表明，常用于工业网络远程维护的私有 APN 连接可能成为攻击关键基础设施的有效途径。这提醒人们需要在 OT 环境周围实施更严格的安全控制措施。 私有 APN 是一种专用蜂窝网关，可将 IoT 或工业设备直接连接到私有网络，绕过公共互联网。尽管它可以提供加密和访问控制，但错误配置或隔离不足仍可能使 OT 系统暴露给攻击者。

rss · BleepingComputer · 8月10日 23:07

**背景**: 运营技术（OT）包括监控和控制物理设备及工业流程（如发电厂设施）的硬件和软件。私有 APN 通常用于为移动或远程设备提供对私有网络的安全、专用访问，而无需经过公共互联网。OT 安全侧重于在确保安全可靠运行的同时保护这些系统。在此事件中，私有 APN 成为了进入该厂 OT 网络的入口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stacuity.com/what-is-an-apn/">What is an APN? Guide to Access Point Names & Private APNs</a></li>
<li><a href="https://flolive.net/blog/glossary/private-apn-how-it-works-types-pros-cons-and-best-practices/">Private APN: How It Works, Types, Pros/Cons & Best Practices</a></li>
<li><a href="https://www.fortinet.com/solutions/industries/scada-industrial-control-systems/what-is-ot-security">fortinet.com/solutions/industries/scada-industrial-control-systems/what...</a></li>

</ul>
</details>

**标签**: `#security`, `#OT`, `#APN`, `#critical infrastructure`, `#cyberattack`

---

<a id="item-17"></a>
## [BdThemes 插件供应链攻击创建恶意管理员账户](https://www.bleepingcomputer.com/news/security/bdthemes-plugins-supply-chain-hack-creates-rogue-wordpress-admins/) ⭐️ 8.0/10

BdThemes（一家高级 WordPress 网页设计工具开发商）遭遇供应链攻击，攻击者入侵其上游基础设施，并修改了发送到管理员浏览器的远程 JSON feed，以创建恶意管理员账户。 这一事件凸显了 WordPress 生态系统中供应链攻击日益增长的风险——单个被篡改的更新或 feed 就可能危及数千个网站。网站管理员必须迅速审计管理员账户并加固其安装，插件开发者则必须强化构建和分发流程。 该攻击并非直接修改插件代码，而是篡改了插件远程获取的 JSON feed，导致恶意 JavaScript 在已登录管理员的浏览器上下文中执行。这使得攻击者无需修改服务器上的插件文件即可添加恶意管理员账户，从而增加了通过文件完整性监控进行检测的难度。

rss · BleepingComputer · 8月10日 21:12

**背景**: 供应链攻击针对受信任的第三方供应商或依赖项，以危害下游用户。在本例中，JSON feed 是插件所依赖的外部配置或数据源，由于它的安全防护不如插件代码本身严格，攻击者得以注入恶意内容。WordPress 网站通常使用插件扩展功能，而管理员账户是 WordPress 安装中权限最高的账户，因此创建恶意管理员账户尤其危险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>
<li><a href="https://www.crowdstrike.com/en-us/cybersecurity-101/cyberattacks/supply-chain-attack/">What Is a Supply Chain Attack? - CrowdStrike</a></li>
<li><a href="https://en.wikipedia.org/wiki/JSON_Feed">JSON Feed - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#WordPress`, `#malware`

---

<a id="item-18"></a>
## [CISA：勒索软件团伙正在利用 SonicWall SMA1000 漏洞](https://www.bleepingcomputer.com/news/security/cisa-sonicwall-sma1000-flaws-now-exploited-by-ransomware-gangs/) ⭐️ 8.0/10

CISA 已确认，勒索软件团伙正在积极利用两个近期修补的 SonicWall SMA1000 漏洞，其中包括一个最大严重级别的服务器端请求伪造（SSRF）漏洞。这一确认提高了管理员立即应用安全更新的紧迫性。 这些漏洞影响 SonicWall SMA1000 远程访问设备，此类设备广泛用于为企业网络提供安全的远程访问。勒索软件团伙的积极利用使其成为紧迫威胁，可能导致网络沦陷和勒索软件部署。 这两个漏洞中最严重的是一个最大严重级别的 SSRF 漏洞，可能允许攻击者从易受攻击的服务器向内部系统发出请求。这些漏洞已于近期修补，因此建议立即打补丁以减轻积极利用的风险。

rss · BleepingComputer · 8月10日 14:34

**背景**: SonicWall SMA 1000 系列是 Secure Mobile Access 设备家族，为远程用户提供对企业应用程序和内部资源的安全访问。服务器端请求伪造（SSRF）是一种 Web 安全漏洞，攻击者可利用它让服务器端应用向非预期位置发起请求，通常可以访问仅内部可见的服务。攻击者经常以这类远程访问设备为目标，因为它们位于网络边界，是进入内部网络的网关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Server-side_request_forgery">Server-side request forgery - Wikipedia</a></li>
<li><a href="https://portswigger.net/web-security/ssrf">What is SSRF (Server-side request forgery)? Tutorial ...</a></li>
<li><a href="https://www.linkedin.com/pulse/two-sonicwall-sma-1000-zero-days-exploited-one-could-enable-rajora-c78wc">Two SonicWall SMA 1000 Zero-Days Exploited, One Could Enable...</a></li>

</ul>
</details>

**标签**: `#security`, `#CISA`, `#SonicWall`, `#ransomware`, `#vulnerabilities`

---

<a id="item-19"></a>
## [Aeternum 僵尸网络利用 Polygon 区块链实现去中心化指挥与控制](https://unit42.paloaltonetworks.com/aeternum-blockchain-c2-analysis/) ⭐️ 8.0/10

Unit 42 发布了对 Aeternum 的分析报告，这是一个利用 Polygon 区块链智能合约来运行去中心化指挥与控制（C2）基础设施并执行载荷的僵尸网络加载器。 这标志着恶意软件抗打击能力的演进：通过将 C2 通信锚定在公共区块链上，该僵尸网络更难通过传统的域名或 IP 查封来破坏。防御者现在需要将区块链活动监控纳入其威胁情报工具包。 该报告详细说明了 Aeternum 如何从 Polygon 智能合约读取指令并获取载荷，使其网络流量与合法的区块链活动混杂在一起。报告还为安全团队提供了检测方法和失陷指标。

rss · Unit 42 Threat Research · 8月10日 22:00

**背景**: 僵尸网络加载器是恶意软件组件，用于在被入侵设备上安装其他载荷，通常与可被查封或封锁的集中式 C2 服务器通信。Polygon 是一个兼容以太坊的 Layer 2 区块链，交易成本低，因此成为隐蔽 C2 通信的理想渠道。通过将指令存储在智能合约中，操作者避免了对易受打击的基础设施的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Polygon_(blockchain)">Polygon (blockchain)</a></li>
<li><a href="https://polygon.technology/">Polygon | The Go-To Blockchain for Global Payments</a></li>
<li><a href="https://cybersecuritynews.com/new-botnet-loader-as-a-service-exploiting-routers/">New Botnet Loader-as-a-Service Exploiting Routers and IoT ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#botnet`, `#blockchain`, `#C2`, `#threat intelligence`

---

<a id="item-20"></a>
## [中国关联黑客 Storm-1175 利用 N-Central 漏洞部署新型 StormEncryptor 勒索软件](https://thehackernews.com/2026/08/china-linked-hackers-deploy-new.html) ⭐️ 7.0/10

微软威胁情报披露，与中国有关的、受经济利益驱动的威胁行为者 Storm-1175 自 2026 年 8 月 2 日起开始部署一种此前未被记录的新型勒索软件变种 StormEncryptor。该恶意软件用 C++编写，标志着该行为者从以前使用的 Medusa 勒索软件转向，并可能通过 N-able N-central 漏洞 CVE-2026-18577 传播。 这一披露凸显了臭名昭著的操作者如何不断转向新工具，也强调 N-able N-central 等 RMM 平台一旦被攻破所具有的风险。如果该漏洞未及时修补，托管服务提供商及其客户可能面临严重的供应链勒索软件攻击。 StormEncryptor 是一种 C++勒索软件，加密文件后附加.encrypted 扩展名。攻击约始于 2026 年 8 月 2 日，N-able 此后发布了针对关键身份验证绕过漏洞 CVE-2026-18577 的补丁（例如版本 2026.3.1.7）。

rss · The Hacker News · 8月10日 16:38

**背景**: Storm-1175（也被追踪为 Spearwing）是一个自 2023 年起活跃的、与中国有关的、受经济利益驱动的网络犯罪组织，此前以利用面向 Web 系统中的 N-day 漏洞实施高速 Medusa 勒索攻击而闻名。N-able N-central 是被托管服务提供商广泛使用的远程监控与管理（RMM）解决方案；CVE-2026-18577 是一个身份验证绕过漏洞，攻击者可利用它无需认证即可获得 RMM 控制台的'上帝模式'访问权限，从而访问受管端点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/new-stormencryptor-ransomware-used-by-former-medusa-affiliate/">New StormEncryptor ransomware used by former Medusa affiliate</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/04/06/storm-1175-focuses-gaze-on-vulnerable-web-facing-assets-in-high-tempo-medusa-ransomware-operations/">Storm-1175 focuses gaze on vulnerable web-facing assets in ...</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/08/03/cve-2026-18577-n-able-n-central-vulnerability/">Attackers exploit N-able N-central flaw to reach managed endpoints (CVE-2026-18577) - Help Net Security</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#ransomware`, `#threat intelligence`, `#Microsoft`, `#malware`

---