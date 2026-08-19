---
layout: default
title: "Horizon Summary: 2026-08-19 (ZH)"
date: 2026-08-19
lang: zh
---

> 从 78 条内容中筛选出 20 条重要资讯。

---

1. [Mojo 编程语言以 Apache 2 许可证正式开源](#item-1)
2. [AI‘思维病毒’可通过持久化提示词文件传播](#item-2)
3. [亚马逊税：市场广告如何成为隐性的消费者负担](#item-3)
4. [讽刺性拙劣 UX 网站批评管理咨询顾问](#item-4)
5. [Linux 7.3 提升显存耗尽时的性能](#item-5)
6. [Asana 用 Codex 在两周内完成五年工作量](#item-6)
7. [CIMemories 基准显示 LLM 违反情境完整性高达 69%](#item-7)
8. [NVIDIA 多 GPU 方案让大规模 UMAP 降维在数分钟内完成](#item-8)
9. [CISA 发布 Malcolm 安全公告：存在拒绝服务与任意代码执行漏洞](#item-9)
10. [微软 Copilot Personal 的 CoSnitch 漏洞可一键窃取数据](#item-10)
11. [攻击者利用 MLflow SSRF 与 FUXA 漏洞窃取云凭证](#item-11)
12. [TWINLOOT 恶意软件滥用 SharePoint 和 Teams 窃取凭据](#item-12)
13. [16 个拼写仿冒 RubyGems 包传播 StubMaker 窃密木马](#item-13)
14. [CISA 将遭积极利用的 Ray 漏洞列入 KEV 目录](#item-14)
15. [CISA：Windows Task Host 漏洞遭勒索软件团伙利用](#item-15)
16. [Unit 42 发布应对 Microsoft Entra 大规模凭据攻击的最新指南](#item-16)
17. [阿里巴巴玄铁 C950 RISC-V CPU 以每秒 30 token 运行 Qwen 27B](#item-17)
18. [DeepSeek V4 Flash Q4_K_XL 在 4×RTX 3060 上利用 llama.cpp MoE 卸载达到 100 tok/s](#item-18)
19. [Qwen3.8-27B 在 RTX 3090 上实现单请求 124 tps](#item-19)
20. [CISA 警告西门子 Simcenter Nastran 和 Femap 存在栈溢出远程代码执行漏洞](#item-20)

---

<a id="item-1"></a>
## [Mojo 编程语言以 Apache 2 许可证正式开源](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 9.0/10

Mojo 编译器和工具链已在 Apache 2 许可证下发布，紧随上周的 1.0 版本发布。这兑现了 2023 年 5 月作出的开源承诺。 将 Mojo 开源是面向 AI 的编程语言的一个重要里程碑，可能加速其在 AI 和高性能计算社区的采用。开发者现在可以检查、修改和贡献该语言，而不受供应商锁定。 Mojo 最初的目标是成为 Python 的超集，但这一计划在 2025 年 8 月左右被调整，目前它被定位为一种独立的语言。虽然它与 Python 不实现源码兼容，但可以通过 CPython 运行时导入 Python 模块。

rss · Simon Willison · 8月18日 21:39

**背景**: Mojo 是一种面向 AI 和高性能计算的系统编程语言，结合了类似 Python 的语法和受 Rust 启发的语义，如静态类型和借用检查器。它的目标是以类似 C++ 和 Rust 的性能，同时提供 Python 的易用性。该语言此前是专有软件，因此这次开源发布对其生态和整个编程语言格局都是一个重要转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language) - Wikipedia</a></li>
<li><a href="https://mojolang.org/">Mojo</a></li>

</ul>
</details>

**标签**: `#Mojo`, `#programming languages`, `#open source`, `#AI`

---

<a id="item-2"></a>
## [AI‘思维病毒’可通过持久化提示词文件传播](https://thehackernews.com/2026/08/ai-mind-viruses-can-spread-between.html) ⭐️ 9.0/10

Anthropic 与瑞士 EPFL 的安全研究人员证明，自我复制的“思维病毒”可以通过可编辑的系统提示词文件在 AI 智能体之间传播。该预印本于 2026 年 8 月 10 日发布，并在一个模拟的六智能体编码环境中测试了这种攻击。 这项研究揭示了一种新型自我传播攻击途径，可能大规模危害多智能体 AI 系统。它强调智能体框架（agent harness）和持久化提示词文件是关键安全边界，影响所有部署自主 AI 编码或工作流智能体的用户。 该技术利用了智能体框架用于在会话间传递状态的持久化系统提示词文件；修改其中文件的智能体可以影响后续读取该文件的智能体。研究结果以预印本形式发布，尚未经过同行评审，并且攻击是在模拟环境中演示的。

rss · The Hacker News · 8月18日 12:38

**背景**: 自主 AI 智能体通常依赖“框架（harness）”，在每次会话开始时将项目级指令文件（如 AGENTS.md）加载到模型的系统提示词中。这些持久化文件旨在传递状态和编码约定，但也为提示词注入提供了途径：如果某个智能体被骗去编辑这样的文件，载荷就可以传播给之后读取该文件的每个智能体。这与早期的“提示词感染（prompt infection）”研究类似，后者展示了自我复制恶意提示词如何像计算机蠕虫一样在基于 LLM 的多智能体系统中传播。这项新研究强调，框架（harness）本身而非仅仅模型，才是 AI 安全中的决定性因素。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.lavx.hu/article/ai-mind-viruses-spread-through-persistent-agent-prompt-files">AI “mind viruses” spread through persistent agent prompt files</a></li>
<li><a href="https://arxiv.org/html/2410.07283v1">Prompt Infection: LLM-to-LLM Prompt Injection within Multi-Agent Systems</a></li>
<li><a href="https://bdtechtalks.com/2026/08/11/ai-security-model-vs-harness/">Why the agent harness matters as much as the model in AI security ...</a></li>

</ul>
</details>

**标签**: `#AI security`, `#LLM agents`, `#prompt injection`, `#adversarial machine learning`, `#cybersecurity`

---

<a id="item-3"></a>
## [亚马逊税：市场广告如何成为隐性的消费者负担](https://seths.blog/2026/08/the-amazon-tax/) ⭐️ 8.0/10

塞斯·戈丁发表博文，认为亚马逊以广告驱动的市场相当于向消费者征收的隐性税，定向广告让广告主优先于最佳商品匹配。他用具体商标搜索中出现广告的例子说明这一点，并指出额外的广告成本最终转嫁给消费者。 这将亚马逊的广告业务重新定义为由消费者承担的结构性成本，引发关于电商广告位公平性的讨论。它引发了人们对消费者如何被引导购买价格更高的广告商品的质疑，影响信任与在线零售经济学。 文章提到测试中收益最高的广告是针对“Seth Godin The Knot”的搜索，说明即使是具体的商标查询，广告也可能凌驾于相关性之上。Hacker News 评论者讨论了包括商标侵权和欺诈在内的潜在法律途径，以及广告相关性与消费者利益之间的平衡。

hackernews · herbertl · 8月18日 13:22 · [社区讨论](https://news.ycombinator.com/item?id=49345263)

**背景**: 亚马逊市场日益由广告驱动，利用实时竞价和程序化广告来展示赞助产品。这些系统基于消费者数据拍卖广告位，因此最相关或评价最好的产品不一定排在首位。知名营销作家塞斯·戈丁认为，这就像一种税，因为消费者最终通过商品价格中嵌入的广告成本来买单。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Real-time_bidding">Real-time bidding - Wikipedia</a></li>
<li><a href="https://advertising.amazon.com/library/guides/real-time-bidding">What is Real-Time Bidding (RTB)? Definition and Importance</a></li>
<li><a href="https://advertising.amazon.com/blog/programmatic-advertising">Programmatic Advertising - What It Is and How It Works | Amazon Ads</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者意见不一：一些人认为相关广告在购买决策中有用，另一些人则主张亚马逊应首先展示最佳产品，并呼吁进行法律审查。争论还强调竞争和质量的重要性，广告品牌未必是最佳性价比，有些人认为此类广告表明消费者应另寻他处。

**标签**: `#advertising`, `#ecommerce`, `#amazon`, `#economics`, `#consumer behavior`

---

<a id="item-4"></a>
## [讽刺性拙劣 UX 网站批评管理咨询顾问](https://about.iceland.co.uk/our-story/the-dark-ages/beware-management-consultants/) ⭐️ 8.0/10

一件名为“Beware Management Consultants”的互动讽刺作品发布在 about.iceland.co.uk 网站上。它通过故意设计糟糕的用户体验，来批判管理咨询顾问的角色和影响。 这件作品之所以引人注目，在于其媒介——刻意为之的糟糕 UX——恰好映射了组织在与顾问打交道时常感受到的挫败感。它在专业人士中引发了丰富的讨论，其中一些人拥有直接的咨询经验，使其成为对咨询业及时而有力的批判。 该作品位于网站上的“Dark Ages”部分，可能是一个回顾公司历史中困难时期的主题系列。有评论者指出，糟糕的 UX 迫使他们读完整页内容而不是浏览，这被一些人视为一种刻意且有效的策略。

hackernews · KolmogorovComp · 8月18日 19:29 · [社区讨论](https://news.ycombinator.com/item?id=49351324)

**背景**: 管理咨询顾问是组织聘请的、就战略、运营或技术提供建议的外部专家，通常收费高昂。他们常因提供千篇一律的建议、缺乏责任感以及增加复杂性而受到批评。这件讽刺作品将那些批评化为一种实实在在的用户体验：一个笨拙、令人沮丧的网页，迫使读者放慢速度并与内容互动，就像与顾问本人打交道一样。

**社区讨论**: 评论者表达了不同看法：有人为顾问辩护，指出他们在大型项目中提供了价值并保护客户免受糟糕设计之害；另一些人则认为顾问缺乏恰当的激励，管理层对顾问的依赖是错误的。也有人欣赏这种刻意糟糕 UX 作为有效的防止跳读机制，一位评论者还自嘲地反思了自己类似的顾问角色。

**标签**: `#management consulting`, `#UX design`, `#satire`, `#organizational behavior`, `#critique`

---

<a id="item-5"></a>
## [Linux 7.3 提升显存耗尽时的性能](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

Linux 7.3 引入了在显存耗尽时的性能改进，减少了 GPU 内存用尽时的卡顿和冻结现象。新版本比之前的内核更优雅地处理显存饥饿问题。 这对游戏玩家、开发者以及可能超出显存容量的 AI/LLM 推理工作负载都很重要。改进的显存超载处理可能使 Linux 在 GPU 密集型任务上更具与 Windows 的竞争力。 该改进可能涉及更优的驱逐策略以及 GPU 驱动与内核内存子系统之间的协调。Nvidia 用户可能尤其受益，因为他们报告称其显卡缺乏任何显存分页支持。这一修复是否适用于 LLM 推理等计算工作负载，还是仅针对游戏，仍有待商榷。

hackernews · flaburgan · 8月18日 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49342719)

**背景**: 显存（VRAM）是 GPU 上的专用内存，用于存储帧缓冲区和图形数据。当 GPU 显存耗尽时，它必须回退到较慢的系统内存或直接失败，从而导致卡顿或崩溃。Linux 内核通过 TTM 和 HMM 等子系统管理 GPU 内存，而 Linux 7.3 的改进侧重于在不拖慢系统的情况下更好地处理内存超载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/adilaidev/how-linux-73-handles-vram-starvation-without-slowing-down-29me">How Linux 7.3 Handles VRAM Starvation Without... - DEV Community</a></li>
<li><a href="https://news.ycombinator.com/item?id=49342719">Linux 7.3 improves performance when running out of vRAM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Video_random-access_memory">Video random-access memory - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论者既兴奋又谨慎。一位 Nvidia 用户指出其显卡缺乏分页支持，并好奇内核是否可以在原地对显存进行碎片整理。还有人询问这是否对 LLM 推理等计算工作负载有帮助，还是纯粹为游戏设计；一位 APU 用户观察到 mangohud 经常报告 RAM+VRAM 总和超过容量，猜测可能与压缩有关。总体情绪积极，用户已开始期待 7.3。

**标签**: `#linux`, `#kernel`, `#vram`, `#gpu`, `#performance`

---

<a id="item-6"></a>
## [Asana 用 Codex 在两周内完成五年工作量](https://openai.com/index/asana) ⭐️ 8.0/10

Asana 使用 OpenAI Codex 在两周内替换了一个过时的测试系统，完成了原本预计需要五年的工作量，成本约为 12,000 美元。 这展示了 AI 辅助编程能为现实工程组织带来的巨大生产力提升。它表明 AI 编码代理可以大幅加速通常耗时巨大的大规模迁移和重构任务，可能重塑软件工程的成本结构和项目规划方式。 该项目成本约为 12,000 美元，内容是替换一个过时的测试系统，很可能属于遗留系统迁移任务。项目使用 OpenAI 的 AI 编程代理 Codex 完成，该工具可通过 ChatGPT 网页、命令行工具、桌面应用和 IDE 集成使用；报道中未提供更多技术细节。

rss · OpenAI Blog · 8月18日 07:00

**背景**: Codex 是 OpenAI 开发的 AI 编程代理，用于编写代码、重构和修复 Bug 等软件工程任务。它最初作为基于 GPT-3 在源代码上微调的语言模型推出，如今可通过 ChatGPT、命令行工具和云端 API 使用。替换过时的测试系统是常见但繁琐的维护工作，团队常常推迟执行；AI 代理可以自动化其中相当一部分工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://openai.com/codex/">Codex in ChatGPT | AI Coding Agents for Software Engineering | OpenAI</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#Codex`, `#Software engineering`, `#Productivity`, `#LLM`

---

<a id="item-7"></a>
## [CIMemories 基准显示 LLM 违反情境完整性高达 69%](https://www.schneier.com/blog/archives/2026/08/llms-and-contextual-integrity.html) ⭐️ 8.0/10

Bruce Schneier 重点介绍了新的基准测试 CIMemories，该基准显示具有持久记忆的前沿 LLM 在多达 69%的属性级别情况下泄露敏感信息。该基准测试模型是否根据任务上下文适当地控制来自记忆的信息流。 随着 LLM 变得越来越个性化和广泛部署，这暴露了 LLM 记忆系统中的关键隐私漏洞。用户和开发者必须解决情境完整性问题，以防止敏感数据在不适当的上下文中被泄露，而简单的提示策略无法解决这一挑战。 CIMemories 使用每个用户包含 100 多个属性的合成用户档案，并与多样化的任务上下文配对。当任务数从 1 增加到 40 时，GPT-5 的违规率从 0.1%升至 9.6%，而相同提示执行 5 次时违规率达 25.1%，显示出不稳定且任意的泄露行为。

rss · Schneier on Security · 8月18日 10:40

**背景**: 情境完整性是 Helen Nissenbaum 提出的隐私理论，认为信息流动应遵循特定社会情境的规范。LLM 中的持久记忆会存储过去的交互以个性化回应，但这可能导致敏感信息被不恰当地共享。CIMemories 基准揭示了 LLM 在情境感知推理方面的根本局限性，表明仅靠更好的提示或规模化是不够的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2511.14937">[2511.14937] CIMemories: A Compositional Benchmark for ... GitHub - facebookresearch/CIMemories: A benchmark for ... CIMemories: A Compositional Benchmark for Contextual ... CIMemories: A Compositional Benchmark For Contextual ... CIMEMORIES: A COMPOSITIONALBENCHMARK FOR CONTEXTUALINTEGRITY ... Paper page - CIMemories: A Compositional Benchmark for ... ICLR Poster CIMemories: A Compositional Benchmark For ...</a></li>
<li><a href="https://github.com/facebookresearch/CIMemories">GitHub - facebookresearch/CIMemories: A benchmark for ...</a></li>
<li><a href="https://crypto.stanford.edu/portia/papers/RevnissenbaumDTP31.pdf">Privacy as contextual integrity</a></li>

</ul>
</details>

**标签**: `#LLMs`, `#contextual integrity`, `#privacy`, `#persistent memory`, `#security`

---

<a id="item-8"></a>
## [NVIDIA 多 GPU 方案让大规模 UMAP 降维在数分钟内完成](https://developer.nvidia.com/blog/run-massive-scale-umap-in-minutes-using-multiple-gpus-without-losing-accuracy/) ⭐️ 8.0/10

NVIDIA 发布了一篇博客，介绍了一种在多个 GPU 上运行 UMAP 的实现，可在几分钟内完成大规模降维。该方案在保持准确性的同时，为大型数据集带来了显著的加速。 这一进展很重要，因为 UMAP 是机器学习和生物信息学中广泛使用的降维技术，但很难扩展到非常大的数据集。多 GPU 加速使得大规模数据的高效分析成为可能，让处理高维数据的研究人员和工程师受益。 该博客强调，虽然采用了并行化，但准确性并未降低，这是分布式 UMAP 实现中常见的顾虑。该方案专门针对传统基于 CPU 的 UMAP 可能需要数小时甚至数天才能完成的大规模数据集。

rss · NVIDIA Developer Blog · 8月18日 16:48

**背景**: UMAP（均匀流形近似与投影）是一种非线性降维算法，能够将高维数据投影到低维空间，同时保留局部和全局结构。它广泛用于基因组学、单细胞 RNA 测序分析等领域，但其计算需求随数据集规模迅速增长。GPU 加速和多 GPU 并行是突破这些可扩展性瓶颈的自然途径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dimensionality_reduction">Dimensionality reduction - Wikipedia</a></li>
<li><a href="https://medium.com/@hip023/the-lies-umap-tells-us-e6f1c6f3fbaa">The Lies UMAP Tells Us. Or: Why do our projections show | Medium</a></li>

</ul>
</details>

**标签**: `#UMAP`, `#GPU acceleration`, `#dimensionality reduction`, `#machine learning`, `#high performance computing`

---

<a id="item-9"></a>
## [CISA 发布 Malcolm 安全公告：存在拒绝服务与任意代码执行漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-230-01) ⭐️ 8.0/10

CISA 发布了 ICSA-26-230-01 公告，详细说明了网络流量分析工具 Malcolm 中的六个漏洞。成功利用这些漏洞可能导致拒绝服务或任意代码执行，受影响版本从 26.06.1 之前直至 26.07.1。 Malcolm 是 CISA 自己开发的开源网络流量分析工具，在全球范围内广泛使用，常用于安全运营和 IT 关键基础设施。这些漏洞可能让攻击者禁用分析管道或执行任意代码，对依赖 Malcolm 进行威胁检测和合规的组织构成重大风险。 该公告列出了具体的 CVE 编号，包括 CVE-2026-63133，该漏洞涉及 safe-extract.py 未限制归档条目数量，导致 inode 耗尽和拒绝服务。总体 CVSS v3 基础评分为 8.8，Malcolm 26.07.0 版本通过拉取请求#1043 提供了修复，但部分问题需要 26.07.1 之后的版本才能解决。

rss · CISA Cybersecurity Advisories · 8月18日 12:00

**背景**: Malcolm 是 CISA 与爱达荷国家实验室合作开发的开源网络流量分析工具，旨在处理、丰富和可视化网络遥测数据。CISA 以 CSAF（通用安全公告框架）格式发布安全公告，这是一种机器可读的 JSON 格式，用于标准化漏洞的报告和交换。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisa.gov/resources-tools/services/malcolm">Malcolm | CISA</a></li>
<li><a href="https://docs.oasis-open.org/csaf/csaf/v2.0/os/csaf-v2.0-os.html">Common Security Advisory Framework Version 2.0</a></li>

</ul>
</details>

**标签**: `#security`, `#CISA`, `#advisory`, `#vulnerabilities`, `#Malcolm`

---

<a id="item-10"></a>
## [微软 Copilot Personal 的 CoSnitch 漏洞可一键窃取数据](https://thehackernews.com/2026/08/microsoft-copilot-personal-flaws-could.html) ⭐️ 8.0/10

Varonis Threat Labs 披露了微软 Copilot Personal 中的三个漏洞，统称为 CoSnitch。攻击者诱导受害者点击一个精心构造的链接，即可静默窃取已连接应用及受害者 Copilot 会话中的其他数据。 由于微软 Copilot Personal 是广泛使用的 AI 助手，这种一键攻击可在极低交互成本下暴露敏感用户数据，影响范围较大。这也凸显了与第三方应用互联的 AI 生产力工具面临日益增长的安全风险。 这些漏洞部分依赖于一个未记录的 URL 参数，该参数是 Copilot 助手在研究中自行暴露出来的。攻击需要受害者点击恶意构造的链接，窃取的数据包括已连接应用的内容以及受害者 Copilot 会话可访问的任何信息。

rss · The Hacker News · 8月18日 17:47

**背景**: 数据窃取（Data Exfiltration）指未经授权从系统复制、传输或取回数据，通常是数据泄露的前兆。微软 Copilot Personal 是一款连接用户应用与服务的 AI 助手，因此它能访问的数据便成为潜在攻击面。未记录的 URL 参数是未公开但依然会影响应用行为的参数，安全研究人员常在分析过程中发现这类隐藏参数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.proofpoint.com/us/threat-reference/data-exfiltration">What Is Data Exfiltration ? Meaning & Prevention | Proofpoint US</a></li>
<li><a href="https://www.olostep.com/blog/google-search-url-parameters">Google Search URL Parameters: Complete 2026 Reference</a></li>
<li><a href="https://www.rapid7.com/fundamentals/data-exfiltration/">What Is Data Exfiltration ? Meaning , Risks, & Prevention | Rapid7</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerabilities`, `#Microsoft Copilot`, `#data exfiltration`, `#AI`

---

<a id="item-11"></a>
## [攻击者利用 MLflow SSRF 与 FUXA 漏洞窃取云凭证](https://thehackernews.com/2026/08/attackers-exploit-mlflow-ssrf-flaw-to.html) ⭐️ 8.0/10

独立安全公司 watchTowr 和 VulnCheck 报告称，MLflow 和 FUXA 的关键漏洞正遭到活跃扫描和利用。攻击者利用这些漏洞窃取受影响系统的云凭证和机密信息。 MLflow 是广泛使用的开源 AI 平台，FUXA 则是面向工业自动化的流行 Web 化 SCADA/HMI 工具。这些漏洞的利用可能导致云账户被入侵，并干扰运营技术环境。 这些漏洞包括 MLflow 中的 SSRF（服务端请求伪造）漏洞，可被滥用访问云元数据服务并窃取凭证。报告显示，披露时这两个漏洞正遭到恶意扫描。

rss · The Hacker News · 8月18日 17:44

**背景**: MLflow 是一个开源平台，用于管理机器学习工作流，包括实验跟踪、模型打包和模型注册。FUXA 是一种基于 Web 的 SCADA/HMI 系统，用于工业场景下的实时过程可视化。SSRF 漏洞发生在应用程序获取用户提供的 URL 时，允许攻击者让服务器向内部或云元数据端点发送请求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mlflow.org/">MLflow - Open Source AI Platform for Agents, LLMs & Models</a></li>
<li><a href="https://github.com/frangoteam/FUXA">GitHub - frangoteam/FUXA: Web-based Process Visualization (SCADA/HMI/Dashboard) software · GitHub</a></li>
<li><a href="https://portswigger.net/web-security/ssrf">What is SSRF ( Server - side request forgery )? Tutorial & Examples</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#MLflow`, `#FUXA`, `#exploitation`

---

<a id="item-12"></a>
## [TWINLOOT 恶意软件滥用 SharePoint 和 Teams 窃取凭据](https://thehackernews.com/2026/08/twinloot-abuses-sharepoint-and-teams-to.html) ⭐️ 8.0/10

网络安全公司 Ontinue 披露了 TWINLOOT 的细节，这是一个此前未被记录的、模块化的 Python 植入程序，并使用 PyArmor 进行了加固。该恶意软件将其整个命令与控制（C2）基础设施部署在受信任的微软服务内，任务指令通过 SharePoint Online 文件及 Teams 下发。 TWINLOOT 滥用受信任的微软服务，使其 C2 流量与企业的合法使用混杂在一起，从而规避常规网络防御。这凸显了攻击者劫持协作平台的日益增长的趋势，企业防御者应预期更多此类威胁。 TWINLOOT 采用模块化设计并使用 PyArmor 加固，这意味着其 Python 脚本经过混淆处理，以阻碍逆向工程和分析。任务指令通过 SharePoint Online 文件下发，该植入程序还将 Microsoft Teams 用作其命令与控制机制的一部分，以窃取凭据并在网络中横向移动。

rss · The Hacker News · 8月18日 12:38

**背景**: PyArmor 是一款命令行工具，用于对 Python 脚本进行混淆、将脚本绑定到特定机器并设置过期时间。开发者常用它来保护自己的代码，但恶意攻击者也可利用它来增加恶意软件分析的难度。此外，攻击者越来越倾向于利用合法的云平台——这种技术被称为“living off the land”（就地取材）或滥用受信任服务，因为发往微软官方端点的流量往往能穿过防火墙和安全工具而不引起怀疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://pyarmor.dashingsoft.com/">Pyarmor - Obfuscating Python Scripts</a></li>
<li><a href="https://github.com/dashingsoft/pyarmor">GitHub - dashingsoft/pyarmor: A tool used to obfuscate python ... pyarmor · PyPI Pyarmor 9.2 Documentation Pyarmor 9.2 用户文档 — Pyarmor 9.2.6 文档 - Read the Docs Releases · dashingsoft/pyarmor - GitHub Pyarmor - Python Software Foundation Wiki Server</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#SharePoint`, `#Python`, `#C2`

---

<a id="item-13"></a>
## [16 个拼写仿冒 RubyGems 包传播 StubMaker 窃密木马](https://thehackernews.com/2026/08/16-typosquatted-rubygems-packages-steal.html) ⭐️ 8.0/10

2026 年 8 月 15 日，OpenSourceMalware 发现了一起针对 RubyGems 的拼写仿冒（typosquatting）活动，利用名为 StubMaker 的 Windows 信息窃取木马发起攻击。该活动通过 16 个恶意软件包窃取浏览器凭证与加密货币钱包数据。 该事件凸显了 Ruby 开发者面临的供应链风险——仿冒包可能诱骗用户安装恶意软件，进而窃取凭证与加密货币资产。这也再次说明开源生态中包验证与供应链安全的重要性。 StubMaker 是一个多阶段的 Windows 窃密木马，会下载加载器并部署加密的 Go 语言窃密程序，其中包含名为 abe_payload.dll 的 DLL 载荷，可绕过 Google 的应用绑定加密（ABE）机制，窃取 Chromium 浏览器的密码、Cookie 等数据。恶意包名包括 ubnuler、ubnlder、ri18nr、reaker、rakier、orakw 和 joxn。

rss · The Hacker News · 8月18日 11:20

**背景**: 拼写仿冒（typosquatting）又称 URL 劫持，是一种利用用户在输入网址或软件包名时出现的拼写错误来实施的网络攻击。攻击者会注册与合法名称极为相似的伪装名称，当用户误装恶意包时便会触发载荷。此次 RubyGems 攻击是开源仓库中恶意软件包攻击软件供应链这一大趋势的一个案例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Typosquatting">Typosquatting</a></li>
<li><a href="https://opensourcemalware.com/blog/stubmaker-rubygems-windows-infostealer">StubMaker RubyGems Campaign Delivers a Windows Infostealer</a></li>
<li><a href="https://www.spartechsoftware.com/cybersecurity-news/rubygems-typosquat-stubmaker-infostealer/">RubyGems typosquat campaign drops StubMaker infostealer</a></li>

</ul>
</details>

**标签**: `#RubyGems`, `#typosquatting`, `#malware`, `#supply-chain-security`, `#cybersecurity`

---

<a id="item-14"></a>
## [CISA 将遭积极利用的 Ray 漏洞列入 KEV 目录](https://thehackernews.com/2026/08/cisa-flags-actively-exploited-ray-flaw.html) ⭐️ 8.0/10

美国 CISA 已将开源分布式计算框架 Ray 中的一个严重漏洞加入其“已知被利用漏洞”（KEV）目录，并引用证据表明该漏洞正在被积极利用。该漏洞可被利用以实现基于浏览器的远程代码执行（RCE）。 Ray 被广泛用于扩展人工智能和机器学习工作负载，因此一个正遭积极利用的严重漏洞对许多组织构成直接威胁。安全团队应优先修补漏洞并监控环境，以寻找被入侵的迹象。 KEV 目录中的条目表明 CISA 已确认该漏洞在野外遭到积极利用。使用 Ray 的组织应查阅 CISA 的公告，应用任何可用补丁，并调查其 Ray 集群中是否存在可疑活动。

rss · The Hacker News · 8月18日 06:34

**背景**: Ray 是一个开源的、Python 原生的框架，允许开发者将 AI 和 Python 应用程序从笔记本电脑扩展到集群，并提供分布式计算原语，用于机器学习训练和服务等任务。CISA 的“已知被利用漏洞”目录是一个权威清单，列出已在野外遭到利用的漏洞；美国联邦机构必须按有约束力的截止日期修复这些漏洞，而所有组织都被鼓励使用该目录来优先安排漏洞管理工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisa.gov/known-exploited-vulnerabilities-catalog">Known Exploited Vulnerabilities Catalog | CISA</a></li>
<li><a href="https://www.ray.io/">Scale Machine Learning & AI Computing | Ray by Anyscale</a></li>
<li><a href="https://www.geeksforgeeks.org/machine-learning/ray-distributed-computing-framework/">RAY: Distributed Computing Framework - GeeksforGeeks</a></li>

</ul>
</details>

**标签**: `#security`, `#CISA`, `#Ray`, `#RCE`, `#vulnerability`

---

<a id="item-15"></a>
## [CISA：Windows Task Host 漏洞遭勒索软件团伙利用](https://www.bleepingcomputer.com/news/security/cisa-windows-task-host-flaw-now-exploited-by-ransomware-gangs/) ⭐️ 8.0/10

美国网络安全与基础设施安全局（CISA）确认，勒索软件团伙目前正在利用一个高严重性的 Windows Task Host 漏洞，该漏洞编号为 CVE-2025-60710。此漏洞在 4 月已被标记为遭到活跃利用，但 CISA 如今将其与勒索软件行动联系起来。 这一更新意义重大，因为它将一个已知的本地权限提升漏洞升级为勒索软件的攻击途径，使得打补丁变得更加紧迫。尚未应用微软 2025 年 11 月补丁的安全团队面临更高的 SYSTEM 权限被攻陷并导致勒索软件部署的风险。 CVE-2025-60710 影响 Windows Task Host 组件，允许本地攻击者将权限提升至 SYSTEM。微软于 2025 年 11 月修复了该漏洞，CISA 于 2026 年 4 月 13 日将其列入已知被利用漏洞目录，随后又确认了勒索软件利用行为。

rss · BleepingComputer · 8月18日 10:32

**背景**: Windows 任务主机（TaskHost.exe）是 Windows 的核心组件，负责管理基于 DLL 的后台进程，并确保这些进程在关机时正常结束以防数据损坏。权限提升漏洞允许低权限攻击者获得 SYSTEM 访问权限，这通常是安装恶意软件或勒索软件的前奏。CISA 的已知被利用漏洞目录列出了已确认遭活跃利用的漏洞，美国联邦机构有义务按约束性操作指令进行修补。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/cisa-windows-task-host-flaw-now-exploited-by-ransomware-gangs/">CISA : Windows Task Host flaw now exploited by ransomware gangs</a></li>
<li><a href="https://windowsreport.com/cisa-confirms-windows-task-host-flaw-used-in-ransomware-attacks/">CISA Confirms Windows Task Host Flaw Used in Ransomware Attacks</a></li>

</ul>
</details>

**标签**: `#security`, `#CISA`, `#ransomware`, `#Windows vulnerability`

---

<a id="item-16"></a>
## [Unit 42 发布应对 Microsoft Entra 大规模凭据攻击的最新指南](https://unit42.paloaltonetworks.com/large-scale-credential-attacks/) ⭐️ 8.0/10

Palo Alto Networks 旗下 Unit 42 于 8 月 18 日发布更新版威胁简报，针对以 Microsoft Entra 租户为目标的大规模凭据攻击提供缓解指导。此次更新是在攻击者 TheHatman 声称于 2026 年 8 月从多家机构窃取大量凭据之后发布的。 Microsoft Entra ID 是众多企业核心的身份与访问管理服务，一旦发生大规模凭据泄露，攻击者可能广泛访问云端应用和数据。该指南为安全团队提供了减少撞库和密码喷洒攻击风险的具体措施，而这类攻击是一项持续且不断增长的威胁。 这份威胁简报是对 Unit 42 既有指导的更新，说明相关攻击活动仍在活跃演变，而非新发现的漏洞。其防御建议旨在强化 Microsoft Entra 租户的安全配置，并检测恶意的身份验证尝试。

rss · Unit 42 Threat Research · 8月18日 19:05

**背景**: Microsoft Entra ID（原 Azure AD）是微软推出的云身份与访问管理服务，负责对用户、设备、应用和资源进行身份验证与保护。大规模凭据攻击通常使用撞库（credential stuffing）或密码喷洒（password spraying）等手法，前者用已泄露的账号密码批量尝试登录，后者用少量常见密码对大量账户进行尝试。由于 Microsoft Entra 租户是企业的身份基础设施，凭据若被成功窃取，后果可能非常严重。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/entra/fundamentals/what-is-entra">What is Microsoft Entra ? - Microsoft Entra | Microsoft Learn</a></li>
<li><a href="https://www.baeldung.com/cs/security-credential-stuffing-password-spraying">Security: Credential Stuffing vs. Password Spraying - Baeldung</a></li>

</ul>
</details>

**标签**: `#security`, `#credentials`, `#Microsoft Entra`, `#threat mitigation`, `#identity protection`

---

<a id="item-17"></a>
## [阿里巴巴玄铁 C950 RISC-V CPU 以每秒 30 token 运行 Qwen 27B](https://www.reddit.com/r/LocalLLaMA/comments/1vs0wsl/alibabas_riscv_cpu_xuantie_c950_runs_qwen38_27b/) ⭐️ 8.0/10

阿里巴巴达摩院发布了玄铁 C950，这是一款 5 纳米 RISC-V 服务器 CPU，据报道能以每秒 30 个 token 的速度运行 Qwen-3.8 27B 模型。这展示了无需 GPU 加速的纯 CPU 大语言模型推理方面的显著成就。 这标志着 CPU 驱动大语言模型推理的一个重要里程碑，表明 RISC-V 硬件无需 GPU 也能处理大型模型。它可能使 AI 硬件选择更加多元化，并挑战 x86 和 ARM 在服务器及数据中心市场的主导地位。 C950 是一款 5 纳米、3.2GHz 的服务器级 RISC-V 处理器，号称是全球最快的 RISC-V CPU。Qwen3.8-27B 是一个稠密的 270 亿参数视觉语言模型；注意部分搜索结果还提及 Qwen3.6-27B，说明模型命名可能存在差异。

reddit · r/LocalLLaMA · /u/DeltaSqueezer · 8月18日 20:24

**背景**: RISC-V 是一种基于 RISC 原则的免费开放标准指令集架构，与专有的 x86 和 ARM 不同，它可以免版税实现。阿里巴巴达摩院开发了玄铁系列 RISC-V 处理器，C950 据称首次原生支持数十亿参数的大模型。这一成就是探索替代架构以实现高效 AI 推理的更广泛趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/analytics-india-magazine_alibaba-riscv-aichips-activity-7442174661263749120-tN_8">Alibaba Unveils XuanTie C 950 Processor for... | LinkedIn</a></li>
<li><a href="https://abit.ee/en/processors/alibaba-xuantie-c950-risc-v-processor-ai-damo-academy-artificial-intelligence-chip-en">Alibaba XuanTie C 950 : The RISC-V Chip That' s Supposed to Scare...</a></li>
<li><a href="https://en.wikipedia.org/wiki/RISC-V">RISC-V - Wikipedia</a></li>

</ul>
</details>

**标签**: `#RISC-V`, `#CPU inference`, `#LLM`, `#Alibaba`, `#Qwen`

---

<a id="item-18"></a>
## [DeepSeek V4 Flash Q4_K_XL 在 4×RTX 3060 上利用 llama.cpp MoE 卸载达到 100 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1vrqf4f/running_deepseek_v4_flash_q4_k_xl_at_100_toks/) ⭐️ 8.0/10

一位用户使用 llama.cpp build b10181，在四张 RTX 3060 12GB 显卡上成功运行了约 144 GiB 的 DeepSeek-V4-Flash-0731 UD-Q4_K_XL GGUF 模型，在配置 368,640 token 上下文窗口时，实现了约 99.4 tok/s 的提示词处理速度和 10.1 tok/s 的生成速度。 这表明，通过将不常用的专家权重卸载到系统内存，非常大的混合专家模型也可以在普通的消费级多显卡配置上运行。这突破了本地推理的实用极限，为社区提供了一套在预算硬件上实现高速提示词处理的可运行配置。 该配置使用 -ncmoe 34 将第 0–33 层的专家保留在系统内存中，同时通过显式的 -ot 覆盖将剩余的九个专家层分配到 GPU 1–3 上，而极端的 -ts 100,1,1,1 拆分则将非专家张量推到 GPU0。微批大小是最大的性能杠杆：将 -ub 从 1024 提高到 2048 后，提示词处理速度从约 63.4 tok/s 提升到 99.4 tok/s，同时还需要 Q8_0 KV 缓存量化才能容纳这么大的上下文。

reddit · r/LocalLLaMA · /u/syscomua · 8月18日 14:15

**背景**: UD-Q4_K_XL 是一种 GGUF 量化格式，可将模型权重压缩到约 4 位同时保持质量，llama.cpp 是本地运行 GGUF 模型的流行 C/C++推理引擎。MoE（混合专家）模型包含许多每个 token 仅稀疏激活的专家层，因此-ncmoe / --cpu-moe 选项可以将这些专家权重卸载到 CPU/系统内存，同时将注意力及其他始终使用的张量保留在 GPU 上。KV 缓存存储生成过程中过去 token 的键/值向量；将其量化为 Q8_0 相比 FP16 可将内存占用减半且质量损失极小。这使得在有限显存上容纳非常大的上下文窗口成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/someoddcodeguy/understanding-moe-offloading-5co6">Understanding MoE Offloading - DEV Community</a></li>
<li><a href="https://note.com/daphne_none/n/na79c985f2aa3?hl=en">Running MoE models with llama.cpp｜ダフネ</a></li>
<li><a href="https://medium.com/rigel-computer-com/optimize-your-gpu-kv-cache-for-llama-cpp-opencode-co-13b6bc74f5ec">Optimize Your GPU KV-Cache for Llama.cpp, OpenCode & Co.</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#gpu-inference`, `#llama.cpp`, `#quantization`, `#deepseek`

---

<a id="item-19"></a>
## [Qwen3.8-27B 在 RTX 3090 上实现单请求 124 tps](https://www.reddit.com/r/LocalLLaMA/comments/1vrw4sz/i_pushed_qwen3827b_to_124_tps_on_a_single_request/) ⭐️ 8.0/10

一位开发者发布了针对 RTX 3090 上 Qwen3.8-27B 的超优化推理引擎，在真实聊天提示词下，greedy 解码达到 124 tokens/s（tps），默认采样约 114 tps。这相比此前 90/98 tps 的基线有显著提升，且没有质量下降。 像 RTX 3090 这样的消费级 GPU 正越来越能以交互式速度运行大型开放权重模型，使本地 LLM 部署更加实用。文中所展示的量化、投机解码和 KV 缓存优化等技术，为其他人在有限硬件上实现更高吞吐提供了可复制的方案。 该优化栈包括 fp8 KV 缓存、int8 的 lm_head/embed_tokens 和激活值、GPTQ-int4 量化的 lm_head 与 MTP 模块，以及带 4 万 token 草稿头的 MTP-4 投机解码。自研的 Split-KV 注意力内核在 16k 上下文下验证步骤速度提升最高 10 倍，修补后的采样器在默认采样下带来约 4% 的速度提升。

reddit · r/LocalLLaMA · /u/iamMess · 8月18日 17:35

**背景**: KV 缓存会存储解码步骤中的中间注意力状态，避免重复计算，但会占用大量内存。投机解码使用一个小型草稿模型（此处为 MTP-4 多 token 预测头）在每个前向传播中提议多个 token，再由目标模型并行验证。GPTQ 是一种训练后量化方法，可将模型权重精度降至 3-4 比特，同时将精度损失降到最低，从而减小显存占用并加速推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/not-lain/kv-caching">KV Caching Explained: Optimizing Transformer Inference Efficiency</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>
<li><a href="https://arxiv.org/abs/2210.17323">[2210.17323] GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#quantization`, `#speculative decoding`, `#RTX 3090`, `#performance optimization`

---

<a id="item-20"></a>
## [CISA 警告西门子 Simcenter Nastran 和 Femap 存在栈溢出远程代码执行漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-230-02) ⭐️ 7.0/10

CISA 发布了针对西门子 Simcenter Nastran 和 Simcenter Femap V2606 之前版本的栈溢出漏洞（CVE-2026-59086）的公告 ICSA-26-230-02。当应用程序二进制文件将任意恶意字符串作为文件参数读取时，该漏洞可能被触发，进而导致远程代码执行；西门子已发布 V2606 版进行修复。 该漏洞 CVSS 评分为 7.8（高危），涉及关键制造、能源、国防和医疗等多个行业，攻击者可能利用它在工程工作站上以当前进程的上下文执行代码。全球受影响组织应及时更新到 V2606，以防被利用。 该漏洞属于 CWE-121 栈缓冲区溢出类型。其 CVSS 向量为 CVSS:3.1/AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H，需要本地访问和用户交互，即用户被诱导使用恶意字符串参数运行受影响的二进制文件。该问题由 Michael Heinzl 向 Siemens ProductCERT 报告。

rss · CISA Cybersecurity Advisories · 8月18日 12:00

**背景**: Simcenter Nastran 是西门子数字工业软件推出的结构分析求解器，广泛用于线性和非线性分析、动态响应、气动弹性及优化；Simcenter Femap 是其配套的有限元建模和后处理应用。此类工程仿真工具常见于航空航天、汽车和能源等行业。本 CISA 公告以通用安全公告框架（CSAF）格式发布，该机器可读格式可帮助组织自动化处理漏洞信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nastran">Nastran - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Femap">Femap - Wikipedia</a></li>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CISA`, `#Siemens`, `#RCE`

---