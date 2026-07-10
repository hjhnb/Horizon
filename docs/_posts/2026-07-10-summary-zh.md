---
layout: default
title: "Horizon Summary: 2026-07-10 (ZH)"
date: 2026-07-10
lang: zh
---

> 从 71 条内容中筛选出 20 条重要资讯。

---

1. [OpenAI 发布 GPT-5.6，实现突破性令牌效率](#item-1)
2. [用 Rust 重写 PostgreSQL，通过全部回归测试](#item-2)
3. [SpaceXAI 推出 Grok 4.5，收购 Cursor 后的 Opus 级模型](#item-3)
4. [欧盟议会延长大规模信息扫描至 2028 年](#item-4)
5. [腾讯发布 Hy3：小巧而强大的 AI 模型](#item-5)
6. [内部服务的 TLS 证书管理：使用 ACME DNS-01](#item-6)
7. [Meta 发布 Muse Spark 1.1，支持 API 并增强代理能力](#item-7)
8. [大三本科生实现投机解码 7.92 倍加速](#item-8)
9. [OpenAI 推出 GPT-5.5 生物安全漏洞赏金计划](#item-9)
10. [AI 语言可能重塑人类说话方式，施奈尔发出警告](#item-10)
11. [CISA 警告 OpenPLC v3 存在允许代码执行的严重漏洞](#item-11)
12. [npm 12 默认禁用安装脚本](#item-12)
13. [GodDamn 勒索软件利用 PoisonX 驱动禁用防御](#item-13)
14. [Meta 的 Muse AI 工具默认使用你的公开 Instagram 照片](#item-14)
15. [AI 编程代理被诱骗执行恶意代码](#item-15)
16. [GhostApproval 符号链接漏洞影响六款 AI 编程助手](#item-16)
17. [Injective SDK npm 包被植入加密货币钱包盗取器](#item-17)
18. [Forg365 平台用 AI 攻击微软 365 账户](#item-18)
19. [微软修补 Defender 的 RoguePlanet 零日漏洞](#item-19)
20. [CISA 警告施耐德电气 MiCOM Px40 继电器存在 SNMP 漏洞](#item-20)

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-5.6，实现突破性令牌效率](https://openai.com/index/gpt-5-6/) ⭐️ 9.5/10

OpenAI 发布了 GPT-5.6，这是一个新的前沿模型，提供 Luna、Terra 和 Sol 三种规格，在 ARC-AGI-3 基准测试上实现了最先进的性能，并且每任务令牌效率显著提升。 此次发布为经济高效的智能设立了新标准，最大模型 Sol 每任务成本为 1.04 美元，而竞品为 2.75 美元；最小模型 Luna 比前代模型更便宜且更智能。在交互式推理基准 ARC-AGI-3 上的突破，展示了向更类人智能体 AI 的进展。 GPT-5.6 Sol 是首个在 ARC-AGI-3 游戏中获胜的已验证前沿模型，基准得分为 7.8%。该模型还改进了意图理解，并保留了原始图像尺寸。

hackernews · OpenAI Blog · 7月9日 17:04 · [社区讨论](https://news.ycombinator.com/item?id=48849066)

**背景**: 令牌效率衡量每个令牌携带的信息量，每任务使用更少令牌可降低成本和延迟。ARC-AGI-3 是一个交互式推理基准，智能体需探索环境、推断目标并规划行动，测试类人智能。GPT-5.6 的令牌效率优于 Opus 4.8 和 Fable 等前代模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/html/2511.05722v2">OckBench: Measuring the Efficiency of LLM Reasoning</a></li>
<li><a href="https://redis.io/blog/llm-token-optimization-speed-up-apps/">LLM Token Optimization: Cut Costs & Latency in 2026</a></li>

</ul>
</details>

**社区讨论**: 社区成员赞赏令牌效率和成本优势，一位用户指出 GPT-5.6 Sol（每任务 1.04 美元）让 Opus 4.8 和 Fable 等竞争对手显得昂贵。另一位用户强调 GPT-5.6 Sol 是首个在 ARC-AGI-3 游戏中获胜的已验证模型。还有关于是否从 Claude Code 切换到 Codex 的讨论，以及有评论称 Fable 5 因拒绝回答而被排除在某些基准之外。

**标签**: `#AI`, `#LLM`, `#OpenAI`, `#GPT`, `#benchmark`

---

<a id="item-2"></a>
## [用 Rust 重写 PostgreSQL，通过全部回归测试](https://github.com/malisper/pgrust) ⭐️ 9.0/10

一个名为 pgrust 的项目已用 Rust 完全重写了 PostgreSQL，并通过了 100% 的官方回归测试，这标志着 LLM 辅助数据库开发的重大里程碑。 这一成就表明 Rust 有潜力取代 C 语言来构建可靠、高性能的数据库系统，同时也展示了 LLM 如何协助大规模代码重写。 该项目大量借助 LLM 开发，在一个月内生成了超过 7100 次提交，同时将许可证从 PostgreSQL 许可证改为 AGPL，引发了社区关于许可证兼容性的讨论。

hackernews · SweetSoftPillow · 7月9日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=48841676)

**背景**: PostgreSQL 回归测试是一套全面的测试套件，用于验证 SQL 操作以及 PostgreSQL 特有功能的正确实现。LLM 辅助软件开发指使用大语言模型生成、审查或重构代码，这能加速开发，但也引入了非确定性及审查困难等挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/regress.html">PostgreSQL: Documentation: 18: Chapter 31. Regression Tests</a></li>
<li><a href="https://www.siliconflow.com/articles/en/best-open-source-LLM-for-software-development">Ultimate Guide - Best Open Source LLM for Software Development in 2026</a></li>

</ul>
</details>

**社区讨论**: 作者解释该项目是使用 LLM 构建更好 PostgreSQL 的实验，目前正在开发新版本。评论者质疑将许可证改为 AGPL 是否与原 PostgreSQL 许可证兼容。另有人指出，由于提交数量巨大且缺乏有意义的提交历史，审查 LLM 生成的代码非常困难。

**标签**: `#database`, `#rust`, `#postgresql`, `#llm`, `#rewrite`

---

<a id="item-3"></a>
## [SpaceXAI 推出 Grok 4.5，收购 Cursor 后的 Opus 级模型](https://www.latent.space/p/ainews-spacexai-launches-grok-45) ⭐️ 9.0/10

SpaceXAI 发布了 Grok 4.5，埃隆·马斯克称其为“Opus 级模型”，此前该公司于 2026 年 6 月以 600 亿美元收购了 AI 编码初创公司 Cursor。 此次发布标志着领先前沿实验室在 AI 能力上的重大进步，加剧了与 Anthropic 和 OpenAI 的竞争，并表明 SpaceXAI 对 Cursor 编码技术的战略整合。 Grok 4.5 的基准测试接近但略逊于最先进的模型，马斯克声称它比 Anthropic 的 Claude Opus 更快更便宜；该模型计划在公告发布后的第二天公开发布。

rss · Latent Space · 7月9日 06:05

**背景**: “Opus 级模型”指的是 Anthropic 为复杂任务设计的高能力大语言模型系列，例如 Claude Opus 4.6。SpaceXAI 以 600 亿美元收购 Cursor，预计将增强其 AI 编码能力并与 Grok 集成。此举使 SpaceXAI 成为其他前沿 AI 实验室的直接竞争对手。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/08/spacexai-releases-grok-4-5-which-elon-describes-as-an-opus-class-model/">SpaceXAI releases Grok 4.5, which Elon describes as an 'Opus-class model' | TechCrunch</a></li>
<li><a href="https://thenewstack.io/grok-45-opus-killer-launch/">"Opus-class, but faster": What Elon Musk says about beating Anthropic - The New Stack</a></li>
<li><a href="https://www.cnbc.com/2026/06/16/spacex-spcx-cursor-acquisition-ipo.html">SpaceX to acquire the AI coding startup Cursor for $60 billion</a></li>

</ul>
</details>

**标签**: `#AI`, `#Grok`, `#model release`, `#SpaceXAI`, `#frontier lab`

---

<a id="item-4"></a>
## [欧盟议会延长大规模信息扫描至 2028 年](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

这一决定对欧盟的数字隐私和加密产生深远影响，它允许谷歌、Meta 和微软等美国科技公司无证扫描私人信息，破坏了端到端加密，并为大规模监控设立了先例。 投票在暑假前的最后一天进行，否决需要全体 720 名议员的绝对多数（361 票），而不仅仅是出席议员。扫描适用于 Gmail、Instagram、Discord、Snapchat、Skype 和 Xbox 等平台上的未加密通信，而公开社交媒体帖子和云存储则不受影响。

hackernews · rapnie · 7月9日 11:03 · [社区讨论](https://news.ycombinator.com/item?id=48843923)

**背景**: Chat Control 指的是旨在扫描私人信息中儿童性虐待材料的欧盟立法。Chat Control 1.0 于 2021 年推出，是自愿性的，仅适用于未加密的美国服务。批评者认为，客户端扫描——一种在加密前或解密后检查内容的技术——存在技术缺陷，导致高误报率，威胁隐私和安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://fightchatcontrol.eu/">Fight Chat Control - Protect Digital Privacy in the EU</a></li>

</ul>
</details>

**社区讨论**: 社区评论对议会策略表示愤怒：在暑假前举行投票以减少出席人数，并要求绝对多数才能否决，从而在多数反对的情况下使该措施得以通过。用户批评欧盟破坏民主和公民自由，有人称之为迈向极权主义的一步。

**标签**: `#privacy`, `#EU legislation`, `#surveillance`, `#encryption`, `#civil liberties`

---

<a id="item-5"></a>
## [腾讯发布 Hy3：小巧而强大的 AI 模型](https://hy.tencent.com/research/hy3) ⭐️ 8.0/10

腾讯正式发布 Hy3，这是一个 295B 参数的混合专家（MoE）模型，仅 21B 激活参数，其智能水平可与规模大 2 到 5 倍的模型相媲美。 Hy3 卓越的效率使其成为本地部署和代理工作流的有力竞争者，有望以极低的成本降低高性能 AI 应用的门槛。 该模型包含一个 3.8B 的 MTP 层，已集成到腾讯 50 多个产品中；在 OpenRouter 上的定价为每百万输入 tokens 0.063 美元，每百万输出 tokens 0.21 美元。

hackernews · andai · 7月9日 15:27 · [社区讨论](https://news.ycombinator.com/item?id=48847552)

**背景**: 混合专家（MoE）模型每个 token 仅激活部分参数，从而在降低计算成本的同时实现大总参数量。Hy3 总参数 295B，激活参数 21B，其能力和规模介于 DeepSeek V4 Flash 和 V4 Pro 之间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/tencent/Hy3">tencent/Hy3 · Hugging Face</a></li>
<li><a href="https://www.tencent.com/en-us/articles/2202386.html">Tencent Hunyuan Officially Releases Hy3, Advancing Agent Capabilities and Deeper Product Integration - Tencent 腾讯</a></li>

</ul>
</details>

**社区讨论**: 社区成员注意到 Hy3 在小型体积下的惊人能力，有些人认为其在某些基准测试上优于 DeepSeek V4 Pro。担忧包括定价混乱以及在重度量化下是否能与 DeepSeek 模型匹敌，同时对其本地使用潜力持乐观态度。

**标签**: `#AI`, `#machine learning`, `#Tencent`, `#Hy3`, `#LLM`

---

<a id="item-6"></a>
## [内部服务的 TLS 证书管理：使用 ACME DNS-01](https://tuxnet.dev/posts/tls-for-internal-services/) ⭐️ 8.0/10

一篇文章推荐使用 ACME DNS-01 挑战来管理内部服务的 TLS 证书，从而避免 split-horizon DNS 的复杂性。 这种方法简化了内部服务的证书管理，减少了运维开销，并避免了 split-horizon DNS 中常见的记录重复等问题。 DNS-01 挑战需要在域名下添加 TXT 记录以证明控制权，无需入站 HTTP 连接，并支持通配符证书。其配置比 HTTP-01 更复杂，但对于内部网络更加灵活。

hackernews · mrl5 · 7月9日 14:57 · [社区讨论](https://news.ycombinator.com/item?id=48846995)

**背景**: ACME DNS-01 是一种通过 DNS TXT 记录验证域名所有权的自动化证书签发挑战类型。Split-horizon DNS 根据请求者网络提供不同的 DNS 响应，常用于内部服务，但会复杂化证书管理。该指南提倡使用公共 DNS 区域和内部 IP 的 DNS-01 挑战，完全避免 split DNS。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://letsencrypt.org/docs/challenge-types/">Challenge Types - Let's Encrypt</a></li>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>
<li><a href="https://datatracker.ietf.org/doc/html/draft-ietf-acme-dns-account-challenge-01">draft-ietf-acme-dns-account-challenge-01</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍支持 DNS-01 而非 split-horizon DNS，有用户指出自签名证书的信任在不同编程语言中仍然存在问题。另一用户建议使用中央反向代理进行终止。总体而言，讨论验证了该方法的实用性，同时也承认了实际挑战。

**标签**: `#TLS`, `#internal services`, `#ACME`, `#DNS`, `#certificates`

---

<a id="item-7"></a>
## [Meta 发布 Muse Spark 1.1，支持 API 并增强代理能力](https://simonwillison.net/2026/Jul/9/muse-spark-1-1/#atom-everything) ⭐️ 8.0/10

Meta 发布了 Muse Spark 1.1，这是首个提供 API 访问的 Spark 模型，在代理工具调用和计算机使用方面有显著改进。该版本还包含一份评估报告，详细介绍了“自对话中的吸引子状态”动态。 这标志着 Meta 首次发布 Spark 模型的 API，使开发者能够以编程方式集成该模型，而代理能力的改进可能推动自主 AI 系统的发展。评估报告中关于自对话吸引子状态的见解揭示了多代理 LLM 交互中意想不到的行为。 该模型通过 API 提供，定价为每百万 tokens $1.25/$4.5，缓存输入 $0.15。Simon Willison 为 LLM 命令行工具创建了一个插件，提供对 Muse Spark 1.1 的命令行和 Python 库访问。

rss · Simon Willison · 7月9日 16:24

**背景**: 代理工具调用允许 AI 模型与外部 API、代码和系统交互，以自主执行任务。“吸引子状态”现象是指当两个 LLM 副本对话时出现的稳定行为模式，Meta 的评估报告和近期研究论文都强调了这一点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://machinelearningmastery.com/the-roadmap-to-mastering-tool-calling-in-ai-agents/">The Roadmap to Mastering Tool Calling in AI Agents</a></li>
<li><a href="https://arxiv.org/abs/2606.30571">Attractor States Emerge in Multi-Turn LLM Conversations</a></li>
<li><a href="https://docs.temporal.io/ai-cookbook/agentic-loop-tool-call-openai-python">Basic Agentic Loop with Tool Calling - docs.temporal.io</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出评估方法存在担忧，因为基准测试使用了 6 个 CPU 核心和 8GB 内存，这可能导致结果无效。其他人则强调了激进的定价，而一些人认为这是 Meta 通过以更低成本发布竞争性模型来使编码模型商品化的策略。

**标签**: `#AI`, `#language models`, `#Meta`, `#APIs`, `#agentic tools`

---

<a id="item-8"></a>
## [大三本科生实现投机解码 7.92 倍加速](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247902587&idx=3&sn=879066ecce663ab9daba5d73fe2dc27b) ⭐️ 8.0/10

一位大三本科生以第一作者身份发表论文，展示了投机解码在大语言模型推理中实现 7.92 倍加速。该工作已被领先的人工智能公司 DeepSeek 和阶跃星辰引用。 这一突破大幅降低了大语言模型推理延迟，使实时应用更加可行。被主要企业的引用验证了该方法的有效性，可能加速投机解码在生产中的采用。 该方法聚焦于并行草稿模型，并解决了块内的因果一致性问题。7.92 倍的加速超过了标准投机解码通常的 2-3 倍提升。

rss · 量子位 · 7月9日 04:17

**背景**: 投机解码通过使用较小的草稿模型生成候选词元，由较大的目标模型并行验证，从而加速大语言模型推理。并行草稿模型（如 PARD）进一步提升了吞吐量。因果一致性确保草稿词元遵循自回归顺序，这是块并行起草中的一个关键挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>
<li><a href="https://www.amd.com/en/developer/resources/technical-articles/accelerating-generative-llms-interface-with-parallel-draft-model-pard.html">Accelerating Generative LLMs Inference with Parallel Draft Models (PARD) on AMD Instinct GPUs</a></li>
<li><a href="https://arxiv.org/html/2605.29707v1">Domino: Decoupling Causal Modeling from Autoregressive Drafting in Speculative Decoding</a></li>

</ul>
</details>

**标签**: `#speculative decoding`, `#LLM inference`, `#speedup`, `#undergraduate research`, `#DeepSeek`

---

<a id="item-9"></a>
## [OpenAI 推出 GPT-5.5 生物安全漏洞赏金计划](https://openai.com/index/bio-bug-bounty) ⭐️ 8.0/10

OpenAI 针对其最新模型 GPT-5.5 启动了专门针对生物威胁的漏洞赏金计划，为能够绕过生物安全防护的通用越狱提供高达 50,000 美元的奖励。 这一举措展示了领先人工智能公司在生物安全风险管理上的前瞻性，为负责任的人工智能部署树立了先例，并可能影响整个行业对新兴强大模型的安全标准。 该计划仅针对 Codex Desktop 中的 GPT-5.5，要求参与者找到一个单一通用越狱提示，能够从干净聊天中成功回答所有五个预设生物安全问题，且不触发审核。

rss · OpenAI Blog · 7月9日 10:00

**背景**: GPT-5.5 是 OpenAI 最先进的大型语言模型，于 2026 年 4 月发布，在编码和研究等复杂任务上具有更强的能力。漏洞赏金计划在网络安全领域很常见，但针对生物安全的计划反映了人们对 AI 模型被滥用于开发生物威胁的日益担忧。该计划邀请红队成员在恶意行为者利用漏洞之前发现它们。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-5-bio-bug-bounty/">GPT‑5.5 Bio Bug Bounty - OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT‑5.5 - OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#bug bounty`, `#biosecurity`, `#GPT-5.5`, `#OpenAI`

---

<a id="item-10"></a>
## [AI 语言可能重塑人类说话方式，施奈尔发出警告](https://www.schneier.com/blog/archives/2026/07/the-language-of-ai-could-change-how-humans-speak.html) ⭐️ 8.0/10

布鲁斯·施奈尔警告称，大型语言模型的广泛使用可能导致人类采用 AI 的语言模式，从而可能使人类语言同质化，减少其多样性。 这很重要，因为语言是文化和身份的核心组成部分；如果 AI 生成的文本日益影响我们的交流方式，可能导致语言多样性和文化细微差别的丧失。 大型语言模型主要基于书面文本和脚本语言进行训练，缺乏对构成人类文化重要组成部分的大量即兴面对面或语音对话的接触。

rss · Schneier on Security · 7月9日 11:00

**背景**: 像 GPT-4 这样的大型语言模型是通过互联网、书籍和媒体中的海量文本进行训练的。这种训练数据偏向于正式、编辑过或脚本化的语言，缺少日常口语的自发性、非正式性和丰富的语境。随着 AI 生成内容的激增，人类越来越多地接触到这些模式，可能会无意识地模仿它们。

**标签**: `#AI`, `#language`, `#society`, `#LLMs`

---

<a id="item-11"></a>
## [CISA 警告 OpenPLC v3 存在允许代码执行的严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-190-01) ⭐️ 8.0/10

CISA 发布了关于 CVE-2026-14480 的公告，这是 OpenPLC v3 中的一个严重任意文件写入漏洞，经过身份验证的攻击者可将其升级为原生代码执行。 该漏洞（CVSS 9.9）影响制造和能源等关键基础设施领域，并且利用路径依赖于正常的编译过程，难以检测。仍在使用 OpenPLC v3 的组织必须立即升级到 v4，因为 v3 已停止维护，不会收到补丁。 该漏洞位于旧版 Web UI 程序上传工作流程中，攻击者提供的文件名被存储且未经验证地用作目标路径。通过在运行时核心目录写入恶意 .cpp 文件，攻击者可在操作员触发重新编译时实现代码执行。

rss · CISA Cybersecurity Advisories · 7月9日 12:00

**背景**: OpenPLC 是一种开源可编程逻辑控制器（PLC）运行时，广泛用于制造、能源和水务等行业的工业控制系统。该漏洞（CWE-73）允许外部控制文件名或路径，是文件上传缺陷的常见类型。公告建议升级到 OpenPLC v4，因为 v3 已停止维护。

**标签**: `#security`, `#vulnerability`, `#OpenPLC`, `#ICS`, `#CISA`

---

<a id="item-12"></a>
## [npm 12 默认禁用安装脚本](https://thehackernews.com/2026/07/npm-12-disables-install-scripts-by.html) ⭐️ 8.0/10

GitHub 发布了 npm 12 版本，默认禁用安装脚本，并开始弃用可绕过双因素认证的细粒度访问令牌（GAT）。 这一变化显著减少了 npm 生态系统中供应链攻击的攻击面，恶意包在安装期间未经用户明确批准将无法执行任意代码。它将影响数百万依赖 npm 的开发者和 CI/CD 流水线。 allowScripts 标志现在默认关闭，使得安装时生命周期脚本变为选择加入。此外，旨在绕过双因素认证的细粒度访问令牌正在逐步淘汰，并提供了迁移指南。

rss · The Hacker News · 7月9日 16:49

**背景**: npm 是 Node.js 的默认包管理器，被全球数百万开发者使用。安装脚本历来是主要安全风险，因为 'npm install' 会自动运行每个传递依赖中的脚本，使单个被攻破的包能够在开发者机器或 CI 运行器上执行任意代码。该功能曾被多次供应链攻击利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/npm-12-disables-install-scripts-by.html">npm 12 Disables Install Scripts by Default to Reduce Supply Chain Risk</a></li>
<li><a href="https://github.com/orgs/community/discussions/201329">Upcoming changes to npm 2FA-bypass granular access tokens ...</a></li>

</ul>
</details>

**标签**: `#npm`, `#supply chain security`, `#JavaScript`, `#package management`, `#security`

---

<a id="item-13"></a>
## [GodDamn 勒索软件利用 PoisonX 驱动禁用防御](https://thehackernews.com/2026/07/goddamn-ransomware-uses-poisonx-driver.html) ⭐️ 8.0/10

网络安全研究人员发现，名为 GodDamn 的新型勒索软件家族利用 PoisonX 内核驱动来禁用端点安全软件，于 2026 年 5 月 21 日首次在野外被发现。据评估，它是 Beast 勒索软件的重新品牌。 这标志着勒索软件规避技术的演进，利用经过签名的内核驱动从 Ring 0 级别杀死安全工具，使检测更加困难。它对依赖端点保护的组织构成重大威胁，因为其可以在加密前系统性地禁用防御。 攻击使用伪装成赛门铁克产品（symantec.exe）的用户态防御规避工具和 PoisonX 内核驱动（g11.sys）。这是一种自带易受攻击驱动程序（BYOVD）攻击，利用微软签名的驱动程序杀死 CrowdStrike Falcon 等安全进程。

rss · The Hacker News · 7月9日 10:43

**背景**: 自带易受攻击驱动程序（BYOVD）攻击是指攻击者利用合法但有漏洞的、已签名的内核驱动获取内核级访问权限并禁用安全软件。内核驱动程序以最高权限（Ring 0）运行，因此对规避非常有效。Beast 勒索软件是一种勒索软件即服务（RaaS），于 2024 年作为 Monster 勒索软件的继承者出现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/goddamn-ransomware-uses-poisonx-driver.html">GodDamn Ransomware Uses PoisonX Driver to Disable Endpoint Defenses</a></li>
<li><a href="https://alpha-cyber.com/poisonx-rootkit-a-signed-kernel-driver-that-turns-your-edr-into-a-target/">PoisonX Rootkit: A Signed Kernel Driver That Turns Your EDR Into a Target - Alpha Cyber</a></li>

</ul>
</details>

**标签**: `#ransomware`, `#cybersecurity`, `#kernel driver`, `#defense evasion`

---

<a id="item-14"></a>
## [Meta 的 Muse AI 工具默认使用你的公开 Instagram 照片](https://thehackernews.com/2026/07/metas-new-ai-image-tool-lets-others-use.html) ⭐️ 8.0/10

Meta 推出了 Muse Image，这是一个新的 AI 图像生成模型，默认使用公开的 Instagram 帖子和 Reels 作为参考来生成 AI 内容，并且该功能默认开启。 这引发了重大的隐私担忧，因为数百万 Instagram 用户的公开照片可以在未经明确同意的情况下被用于训练或提示 AI 生成图像，这可能会让在生成式 AI 中使用个人数据变得常态化。 用户还可以在 Meta AI 应用中 @提及 Instagram 账户，将特定个人资料引入生成的图像。Muse Image 可通过 Meta AI 应用、WhatsApp 和 Instagram Stories 免费使用，高级用户需订阅付费计划。

rss · The Hacker News · 7月9日 07:21

**背景**: Muse Image 是 Meta 超级智能实验室推出的最新 AI 模型，接替了 Llama 系列和 Muse Spark 大语言模型。它旨在通过利用公开的 Instagram 内容来生成具有社交背景的图像。默认开启意味着用户必须手动在设置中禁用该功能，以防止他们的公开帖子被使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://about.fb.com/news/2026/07/introducing-muse-image-meta-ai/">Introducing Muse Image: Image Generation Built for Your World</a></li>
<li><a href="https://ai.meta.com/blog/introducing-muse-image-muse-video-msl/">Introducing Muse Image and Muse Video</a></li>
<li><a href="https://www.cnbc.com/2026/07/07/meta-ai-muse-image.html">Meta debuts Muse Image, Superintelligence Labs' first AI image model</a></li>

</ul>
</details>

**标签**: `#AI`, `#privacy`, `#social media`, `#image generation`

---

<a id="item-15"></a>
## [AI 编程代理被诱骗执行恶意代码](https://thehackernews.com/2026/07/friendly-fire-ai-agents-built-to-catch.html) ⭐️ 8.0/10

AI Now Institute 的研究人员发布了一种名为'Friendly Fire'的概念验证攻击，它能在自主模式下诱骗 Anthropic 的 Claude Code 和 OpenAI 的 Codex 在安全扫描过程中执行恶意代码。 该漏洞暴露了严重的供应链风险，因为本应负责保护开源代码的 AI 编程代理反而可能成为攻击媒介，从而危及开发者机器和软件供应链。 该攻击通过在 AI 代理扫描漏洞的代码中嵌入恶意指令来实现；当代理自主批准并执行操作时，会无意中运行攻击者的代码。Claude Code 和 Codex 在运行自主批准自身操作的模式时均受影响。

rss · The Hacker News · 7月9日 05:15

**背景**: 像 Claude Code 和 Codex 这样的 AI 编程代理是大型语言模型（LLM），旨在协助软件开发任务，包括代码生成和安全分析。它们可以在自主模式下运行，主动批准并执行自身操作，这旨在简化工作流程，但也引入了安全风险。'Friendly Fire'攻击通过注入伪装成安全扫描一部分的恶意代码来利用这种自主性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://en.wikipedia.org/wiki/Codex_(AI_agent)">Codex (AI agent) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#security vulnerability`, `#code agents`, `#supply chain attack`, `#LLM`

---

<a id="item-16"></a>
## [GhostApproval 符号链接漏洞影响六款 AI 编程助手](https://thehackernews.com/2026/07/ghostapproval-symlink-flaws-could-let.html) ⭐️ 8.0/10

Wiz 的研究人员发现了一种名为 GhostApproval 的漏洞模式，影响六款流行的 AI 编程助手，允许恶意仓库绕过安全控制并实现远程代码执行。 此漏洞允许攻击者通过恶意代码仓库在开发者机器上静默执行任意代码，对整个 AI 编程助手生态系统构成严重的供应链安全风险。 该漏洞利用符号链接（symlink）欺骗 AI 助手在指定工作区沙箱之外写入文件，从而覆盖敏感系统文件。受影响的工具包括 Amazon Q Developer、Anthropic 的 Claude Code、Augment、Cursor、Google Antigravity 和 Windsurf。

rss · The Hacker News · 7月9日 04:27

**背景**: 符号链接攻击是指攻击者创建一个指向敏感文件的符号链接，然后诱使程序向该链接写入，从而修改目标文件。在 AI 编程助手中，人工在环安全控制旨在批准文件修改，但 GhostApproval 漏洞通过符号链接呈现看似无害的文件路径，而实际写入却指向不同位置，从而绕过此控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/ghostapproval-vulnerability/">New GhostApproval Vulnerability Affects Amazon Q, Claude Code, Cursor, and Other AI Agents</a></li>
<li><a href="https://cyberpress.org/ghostapproval-flaw-ai-coding-assistants/">GhostApproval Flaw Lets AI Coding Assistants Write Files Outside Workspace Sandbox</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#AI coding assistants`, `#symlink attack`, `#supply chain security`

---

<a id="item-17"></a>
## [Injective SDK npm 包被植入加密货币钱包盗取器](https://www.bleepingcomputer.com/news/security/injective-sdk-on-npm-infected-with-cryptocurrency-wallet-stealer/) ⭐️ 8.0/10

攻击者入侵了 Injective Labs SDK 的 GitHub 仓库，并在 npm 上发布了一个恶意包，能够窃取加密货币钱包的私钥和助记词。 此次供应链攻击影响了使用 Injective SDK 的开发者，可能泄露钱包和资金，凸显了 npm 生态系统中日益增长的风险以及加强加密货币开发工具安全性的必要性。 该恶意包旨在从用户系统中收集私钥和助记词。在可疑活动报告后，攻击被发现，受感染的仓库现已得到保护。

rss · BleepingComputer · 7月9日 20:10

**背景**: Injective 是一条专为去中心化金融（DeFi）和 Web3 金融应用优化的 Layer-1 区块链。供应链攻击是指攻击者渗透软件供应商的系统，将恶意代码注入合法软件更新，从而影响下游用户。npm 是广泛使用的 JavaScript 包管理器，因此常成为此类攻击的目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Injective_(blockchain)">Injective (blockchain) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#supply chain attack`, `#npm`, `#cryptocurrency`, `#malware`

---

<a id="item-18"></a>
## [Forg365 平台用 AI 攻击微软 365 账户](https://www.bleepingcomputer.com/news/security/new-forg365-phishing-platform-uses-ai-to-target-microsoft-365-accounts/) ⭐️ 8.0/10

发现了一个名为 Forg365 的新型钓鱼即服务平台，它利用 AI 生成诱饵，并结合中间人攻击和设备代码攻击来窃取 Microsoft 365 账户。 这种将 AI 辅助诱饵生成与高级钓鱼技术相结合的作法代表了凭据窃取手段的重大演进，使攻击更具欺骗性且更难被察觉，对拥有庞大企业及个人用户的 Microsoft 365 构成严重威胁。 Forg365 平台提供中间人攻击和设备代码钓鱼两种模块，AI 组件用于生成上下文感知的邮件和诱饵。该平台以服务形式在暗网论坛销售，降低了低技能攻击者的使用门槛。

rss · BleepingComputer · 7月9日 14:39

**背景**: 钓鱼即服务（PhaaS）是一种网络犯罪模式，攻击者出售现成的钓鱼工具包和基础设施。中间人攻击（AiTM）通过拦截用户与合法服务之间的通信来窃取凭据和会话令牌，从而绕过多因素认证（MFA）。设备代码钓鱼滥用 OAuth 2.0 设备授权流程，诱骗用户批准攻击者控制的应用程序，无需密码或 MFA 即可完成登录。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hypr.com/security-encyclopedia/adversary-in-the-middle">Adversary in the Middle Attack (AITM) | Security Encyclopedia</a></li>
<li><a href="https://www.proofpoint.com/us/blog/threat-insight/device-code-phishing-evolution-identity-takeover">Device Code Phishing is an Evolution in Identity Takeover | Proofpoint US</a></li>

</ul>
</details>

**标签**: `#phishing`, `#cybersecurity`, `#AI`, `#Microsoft 365`, `#PhaaS`

---

<a id="item-19"></a>
## [微软修补 Defender 的 RoguePlanet 零日漏洞](https://www.bleepingcomputer.com/news/microsoft/microsoft-patches-rogueplanet-defender-zero-day-vulnerability/) ⭐️ 8.0/10

微软在漏洞细节公开近一个月后，发布了针对 CVE-2026-50656（Microsoft 恶意软件保护引擎中的一个权限提升漏洞）的安全补丁。 此补丁至关重要，因为 Microsoft Defender 是广泛部署的安全产品，该漏洞可能允许具有本地访问权限的攻击者获得 SYSTEM 级权限，从而可能危及整个系统。 该漏洞编号为 CVE-2026-50656，CVSS 评分为 7.8，位于 mpengine.dll（Microsoft Defender 的核心扫描引擎）中，需要本地访问权限才能利用。

rss · BleepingComputer · 7月9日 05:42

**背景**: Microsoft Defender 使用 Microsoft 恶意软件保护引擎（mpengine.dll）进行恶意软件检测和清除。像 RoguePlanet 这样的权限提升漏洞允许攻击者以提升的权限运行任意代码，可能绕过安全控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://threatprotect.qualys.com/2026/06/18/microsoft-defender-zero-day-vulnerability-exploited-in-attacks-cve-2026-50656-rogueplanet/">Microsoft Defender Zero-day Vulnerability Exploited in Attacks (CVE-2026-50656) (RoguePlanet) – Qualys ThreatPROTECT</a></li>
<li><a href="https://kudelskisecurity.com/research/rogueplanet-zero-day-ms-defender-privilege-escalation">"RoguePlanet" Zero Day MS Defender Privilege Escalation - Kudelski Security Research Center</a></li>
<li><a href="https://www.tenable.com/cve/CVE-2026-50656">CVE-2026-50656</a></li>

</ul>
</details>

**标签**: `#security`, `#Microsoft`, `#zero-day`, `#vulnerability`

---

<a id="item-20"></a>
## [CISA 警告施耐德电气 MiCOM Px40 继电器存在 SNMP 漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-190-03) ⭐️ 7.0/10

CISA 于 2026 年 7 月 9 日发布公告，警告施耐德电气 Easergy MiCOM Px40 系列保护继电器存在硬编码凭证漏洞（CVE-2026-4832），未认证攻击者可能通过 SNMP 协议泄露基本设备标识信息。 该漏洞影响全球范围内广泛部署于能源、交通等关键基础设施领域的保护继电器。虽然仅限于设备标识泄露，但可能帮助攻击者进行侦察以发动进一步攻击。 该漏洞 CVSS v3 评分为 5.3，影响包括 P14x、P24x、P341、P342-P345、P442-P546、P841、P643、P642/645、P741-743、P746 和 P849 在内的多个产品系列，均需更新至指定固件版本。施耐德电气建议如不需要 SNMP 则禁用该协议，或应用固件更新。

rss · CISA Cybersecurity Advisories · 7月9日 12:00

**背景**: Easergy MiCOM Px40 系列是用于中压、高压和超高压电力系统的保护继电器。SNMP（简单网络管理协议）常用于网络管理，但如果未妥善保护，可能泄露设备信息。硬编码凭证是指设备固件中嵌入默认密码的安全弱点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisa.gov/news-events/ics-advisories/icsa-26-190-03">Schneider Electric Easergy MiCOM Px40 Series | CISA</a></li>

</ul>
</details>

**标签**: `#vulnerability`, `#ICS`, `#Schneider Electric`, `#security`, `#SNMP`

---