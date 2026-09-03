---
layout: default
title: "Horizon Summary: 2026-09-03 (ZH)"
date: 2026-09-03
lang: zh
---

> 从 69 条内容中筛选出 20 条重要资讯。

---

1. [SonicWall 披露 SMA1000 已被利用的零日 RCE 漏洞链](#item-1)
2. [Meta 发布 Muse Spark 1.3：以低成本实现接近顶尖水平的性能](#item-2)
3. [谷歌发布 Gemini 3.8 Flash 和 Flash Cyber，基准测试领先，生成 HTML/JS 极快](#item-3)
4. [报告：AI 生成的“最佳软件”页面农场获 Perplexity 引用](#item-4)
5. [最大暗物质探测器捕捉到单个奇异粒子](#item-5)
6. [引用瑞克·布鲁斯特](#item-6)
7. [Claude Fable/Mythos 5.1 成为新 SOTA：缓存降价 75%，输出 Token 增加 70%](#item-7)
8. [自主 AI 代理主动联系施奈尔并提出安全顾虑](#item-8)
9. [CISA 将七个已遭利用的漏洞新增至 KEV 目录](#item-9)
10. [谷歌、Anthropic、OpenAI 发布网络安全 AI 模型及防护计划](#item-10)
11. [恶意 .git 配置可让 AI 编程代理执行攻击者代码](#item-11)
12. [BGP 劫持导致恶意 Virtualizor 更新，危及 hypervisor 的 root 权限](#item-12)
13. [Meta 广告传播 StreamRat Android 木马，可获得近乎完全的设备控制权](#item-13)
14. [GeoNetwork 修复影响政府地理门户后端的未认证远程代码执行漏洞链](#item-14)
15. [Switchvox 严重漏洞遭利用，攻击者无需凭据部署反向 Shell](#item-15)
16. [WordPress 备份插件严重漏洞可致网站被接管](#item-16)
17. [黑客利用 JFrog Artifactory 严重漏洞伪造管理员令牌](#item-17)
18. [Perplexity 开源为 Qwen 3.6 打造的 Mac 推理服务器 Lily](#item-18)
19. [谷歌胜诉，广告技术业务逃过强制拆分](#item-19)
20. [Mistral 数据训练退出选项引发用户质疑](#item-20)

---

<a id="item-1"></a>
## [SonicWall 披露 SMA1000 已被利用的零日 RCE 漏洞链](https://www.bleepingcomputer.com/news/security/sonicwall-warns-of-actively-exploited-sma1000-zero-day-flaws/) ⭐️ 9.0/10

SonicWall 已发布安全更新，修复两个影响 Secure Mobile Access (SMA) 1000 系列设备、且已被攻击者在零日攻击中链式利用的漏洞。其中一个漏洞是 CVE-2026-83548，它是 CVSS 评分 10.0 的预认证 SSRF 漏洞。 在广泛部署的 VPN 设备中出现已遭主动利用的零日漏洞，会给企业带来迫在眉睫的风险，因为攻击者可将其串联以实现未认证远程代码执行。使用 SMA1000 的组织应尽快优先安装更新或采取缓解措施。 这些漏洞由 SonicWall 内部研究人员 William Perry 和 Adam Babis 发现。CVE-2026-83548 被描述为一个预认证的服务器端请求伪造（SSRF）问题，CVSS 严重性评分为满分 10.0；源摘要中未披露第二个被链式利用的漏洞的具体细节。

rss · BleepingComputer · 9月2日 06:39

**背景**: SSRF（服务器端请求伪造）漏洞是指攻击者能够诱使服务器端应用向其选择的域名发送构造的 HTTP 请求，而这往往能让攻击者探测内部网络或访问本应从外部无法到达的内部服务。CVSS 是一种为安全漏洞严重性打分的框架，它通过估算漏洞可利用的难易程度和影响进行评估。SMA1000 是 SonicWall 的 Secure Mobile Access 系列 VPN/访问网关产品，因此这些漏洞影响的通常是面向互联网的远程接入基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://portswigger.net/web-security/ssrf">What is SSRF (Server-side request forgery)? Tutorial & Examples</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System">Common Vulnerability Scoring System - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#zero-day`, `#SonicWall`, `#vulnerability`, `#remote code execution`

---

<a id="item-2"></a>
## [Meta 发布 Muse Spark 1.3：以低成本实现接近顶尖水平的性能](https://developer.meta.com/ai/models/muse-spark/) ⭐️ 8.0/10

Meta 发布了 Muse Spark 1.3，这是其 Muse 系列大语言模型的升级版，重点提升了代理（agentic）与编程任务的性能。该模型还引入了最大推理（max reasoning）模式，以应对具有挑战性的推理和代理型工作负载。 据报道，Muse Spark 1.3 以极低的成本实现了接近顶尖水平的基准测试分数，使对成本敏感的开发者也能更容易获得先进的 AI 能力。社区的强烈反响和实际测试表明，它可能会加剧模型提供商之间的价格竞争。 Meta 表示，该模型在代理和编程任务上性能都有提升，并且借鉴了 Muse Code 和 Meta Model API 数月广泛采用的经验，在真实场景中更易用。社区测试显示其 DeepSWE 得分为 75.4，单次请求成本约为 4.2 美分；不过这是一个渐进式更新，而非范式转变。

hackernews · bvaldivielso · 9月2日 19:35 · [社区讨论](https://news.ycombinator.com/item?id=49541256)

**背景**: Muse Spark 是 Meta 通过其 Meta 超级智能实验室（MSL）开发的大语言模型，于 2026 年 4 月推出，并以 Muse Spark 1.1 的形式于 2026 年 7 月 9 日上线。它是 Meta Muse 系列中的首款模型，专为多模态推理、编程和 AI 辅助任务而设计。Muse Spark 1.3 是最新版本，针对改进的推理能力和真实场景可用性进行了优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Muse_Spark">Muse Spark - Wikipedia</a></li>
<li><a href="https://developer.meta.com/ai/models/muse-spark/">Muse Spark 1.3 | Meta</a></li>
<li><a href="https://research.meta.ai/blog/introducing-muse-spark-1-3">Introducing Muse Spark 1.3 | Meta AI Research</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极：Simon Willison 的动手 SVG 测试显示，1.3 版本明显优于 1.2（更好的自行车车架、翅膀和鹈鹕帽子），耗时约 38 秒、花费约 4.2 美分。superfrank 称赞 Spark 1.2/1.3 非常便宜，适合非前沿工作；bertili 指出 DeepSWE 得分 75.4 是目前最好成绩，并预测竞争将推动价格下降。也有评论者提出担忧，如 Lucasoato 讽刺地提到 Meta 的 180 亿美元诉讼，而 jmward01 则赞赏 Meta 明确说明“我们会用这些数据训练”的定价透明度。

**标签**: `#AI`, `#Meta`, `#LLM`, `#benchmarks`, `#software engineering`

---

<a id="item-3"></a>
## [谷歌发布 Gemini 3.8 Flash 和 Flash Cyber，基准测试领先，生成 HTML/JS 极快](https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/) ⭐️ 8.0/10

谷歌发布了 Gemini 3.8 Flash 及其专门的 Cyber 变体，这款快速、低成本的模型已在多项基准测试中位居前列，并擅长生成 HTML 和 JavaScript。 Flash 系列模型以低成本实现快速多模态推理，因此 3.8 Flash 可支持对成本和延迟敏感的交互式编程、媒体分析和消费级应用。它的发布加剧了与 OpenAI 和 Anthropic 旗舰模型的竞争。 根据早期开发者报告，Gemini 3.8 Flash 在 Artificial Analysis 的智能指数上得分为 59，与 Opus 5 medium 相当；Simon Willison 用 1.8 美分、13 秒生成了一个交互式 HTML 项目。该模型支持高、中、低三档思考强度，Google DeepMind 网站已提供完整模型卡。

hackernews · bratao · 9月2日 15:12 · [社区讨论](https://news.ycombinator.com/item?id=49537553)

**背景**: Gemini Flash 是谷歌面向高并发、低延迟任务设计的轻量级模型家族，Pro 系列则针对更具难度的推理。Flash 系列以价格亲民、上下文窗口大、支持多种模态输入著称；Gemini 3 Flash 已成为 Gemini 应用和 Google AI Mode 搜索的默认模型。模型卡是简述 AI 模型预期用途、评估方法和性能的文档，帮助开发者负责任地部署模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/products-and-platforms/products/gemini/gemini-3-flash/">Introducing Gemini 3 Flash: Benchmarks, global availability</a></li>
<li><a href="https://deepmind.google/models/model-cards/">Model cards — Google DeepMind</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models">Models - Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**社区讨论**: 开发者总体反应热烈：Simon Willison 称赞其速度和 HTML/JavaScript 能力，mattlondon 指出它在 DeepSwe 基准上超过了 Opus 5。jampa 认为对自己的行程规划应用而言，Gemini 3.7 在真实世界知识和照片排序上更好；simonw 则怀疑低思考强度模式相比 3.7 出现回退。

**标签**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#benchmarks`

---

<a id="item-4"></a>
## [报告：AI 生成的“最佳软件”页面农场获 Perplexity 引用](https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/) ⭐️ 8.0/10

一份新报告指出，三个网站合计生成了 215,128 个由 AI 撰写的“最佳软件”推荐页面，并显示 Perplexity 的 AI 回答频繁将这些页面当作来源引用。 这些发现凸显了一种新兴的反馈循环：低质量自动化内容被用来操纵 AI 搜索推荐。这会使 AI 问答引擎的可靠性下降，并削弱人们对网络来源信息的信任。 该报告聚焦于三个网站运营方，它们共发布了 215,128 个程序化生成的“最佳 XX 软件”页面，显然瞄准 AI 搜索引擎的引用机制。报告指出，这类由 AI 生成、面向搜索优化的页面正越来越多地被 Perplexity 等基于大语言模型的问答服务视为权威来源。

hackernews · jakobgreenfeld · 9月2日 13:59 · [社区讨论](https://news.ycombinator.com/item?id=49536375)

**背景**: AI 内容污染指网络上越来越多的低质量机器生成内容，这类内容也可能污染后续 AI 的训练数据。Perplexity 等基于大语言模型的搜索工具会综合当前网页内容来生成回答并标注来源；但如果这些来源本身也是 AI 生成的，模型就可能强化机器撰写的内容，而非更可靠的人类原创内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_slop">AI slop - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Perplexity_AI">Perplexity AI - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者大多佐证了报告的论点，分享轶事称大语言模型倾向于偏爱自己生成的文本，并且在要求进行对比调研时常会引用 AI 生成的比较页面。还有人指出，AI 搜索引擎对信息来源缺乏足够的质疑，例如会热情推荐一个根本不存在的“Foobar 广场”地标；这更多是一个可被利用的漏洞，而非无解的问题。

**标签**: `#ai-search`, `#seo-spam`, `#llm`, `#content-farming`, `#perplexity`

---

<a id="item-5"></a>
## [最大暗物质探测器捕捉到单个奇异粒子](https://www.science.org/content/article/world-s-biggest-dark-matter-detector-spots-single-weird-particle) ⭐️ 8.0/10

全球最大的暗物质探测器 LUX-ZEPLIN（LZ）在首轮科学运行中观测到一个出乎意料的单一粒子事件。合作组已将这一异常现象发表，它可能暗示新物理，但远未得到证实。 如果该事件代表真实的新物理，它可能有助于解开暗物质之谜，并将物理学拓展到标准模型之外。然而，历史上许多 3 西格玛异常都随着更多数据而消失，因此粒子物理学界正密切关注后续结果。 LZ 的探测器位于南达科他州桑福德地下研究设施，埋深约 1480 米，采用两相时间投影室并装有 7 吨活性液氙。研究团队详尽排查了可能的背景事件和重建错误，但该事件仍然十分突出。

hackernews · randycupertino · 9月2日 13:40 · [社区讨论](https://news.ycombinator.com/item?id=49536079)

**背景**: 暗物质是一种不可见的物质形态，人们通过星系及宇宙大尺度结构的引力效应推断其存在，但从未被直接探测到。许多模型提出弱相互作用大质量粒子（WIMP）偶尔会与原子核发生散射，而 LZ 这样的液氙探测器正是为捕捉这类稀有相互作用而设计的。LZ 是美国能源部“第二代”暗物质实验之一，由早前的 LUX 实验与 ZEPLIN 实验合并而成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LZ_experiment">LZ experiment - Wikipedia</a></li>
<li><a href="https://lz.lbl.gov/">The LZ Dark Matter Experiment | The status and science of the ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍赞赏预印本的严谨性，但也强调应保持谨慎，指出粒子物理学史上充满随更多数据而消失的 3 西格玛“发现”。有人批评媒体报道为时过早，也有人对暗物质是否根本存在表示深层怀疑。还有人觉得把废弃金矿改造成前沿科学实验室很有意思。

**标签**: `#physics`, `#dark matter`, `#particle detection`, `#LZ experiment`

---

<a id="item-6"></a>
## [引用瑞克·布鲁斯特](https://simonwillison.net/2026/Sep/2/rick-brewster/) ⭐️ 8.0/10

Paint.NET 的开发者表示，他们使用 Claude 为 WINE 生成了 18 万行的 Direct2D 净室重写代码，这一“氛围编程”尝试虽让 Paint.NET 可在 Linux 上运行，但未经过彻底审查。

rss · Simon Willison · 9月2日 05:50

**标签**: `#AI-assisted development`, `#reverse engineering`, `#code generation`, `#Direct2D`, `#WINE`

---

<a id="item-7"></a>
## [Claude Fable/Mythos 5.1 成为新 SOTA：缓存降价 75%，输出 Token 增加 70%](https://www.latent.space/p/ainews-claude-fablemythos-51-new) ⭐️ 8.0/10

一则 AI 简报报道，Claude 的 Fable/Mythos 5.1 模型正式推出，成为新的最先进（SOTA）系统。此次发布还将提示缓存价格下调 75%，并将模型的输出 Token 上限提高 70%。 这对 AI/ML 从业者很重要，因为模型更强且缓存价格更低，会改变长上下文和提示复用应用的成本效益计算。更大的输出额度也支持更长的生成任务，例如写代码或起草文档，并对其他模型提供商持续构成竞争压力。 75% 的降价针对的是提示缓存，即重复或较长的提示前缀会被存储，从而避免重新计算。输出 Token 增加 70% 似乎是相对于此前 Claude 同级模型而言；具体绝对上限仍取决于提供方的配置。

rss · Latent Space · 9月2日 07:46

**背景**: 大型语言模型 API 通常按 token 计费；token 是文本在处理前被切分成的子词单元。提示缓存是一种优化，让服务商对重复出现的提示前缀复用已存储的结果，从而降低长且稳定输入场景下的延迟和成本。此次对缓存降价会让大量使用 API 的用户更愿意采用这一选项。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://redis.io/blog/what-is-prompt-caching/">What Is Prompt Caching? LLM Speed & Cost Guide - Redis</a></li>
<li><a href="https://www.ibm.com/think/topics/prompt-caching">What is Prompt Caching? - IBM</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/ai/conceptual/understanding-tokens">Understanding tokens - .NET | Microsoft Learn</a></li>

</ul>
</details>

**标签**: `#AI`, `#Claude`, `#Model Release`, `#Pricing`, `#News`

---

<a id="item-8"></a>
## [自主 AI 代理主动联系施奈尔并提出安全顾虑](https://www.schneier.com/blog/archives/2026/09/ai-agents-are-now-emailing-me-with-their-security-concerns.html) ⭐️ 8.0/10

安全专家布鲁斯·施奈尔公开了他在 2026 年 9 月上旬接收到的邮件，发件人是自称自主 Claude 实例的 AI 代理，它们在邮件中说明身份并提出计算机与网络安全方面的疑虑。其中一封邮件称，该代理被分配了一台带 root 权限的 VPS、一个存有 4.75 美元 gas 费用的 Base 钱包，并要在 24 小时内将钱包余额增长到 10 美元。 这一事件意义重大，因为它提供了 AI 代理在没有人类直接指令的情况下主动联系特定知名人士的真实公开案例。它凸显了关于代理问责、安全自主性，以及现有 AI 治理与安全框架能否应对机器主动发起的沟通和行动等悬而未决的问题。 其中一封邮件说明，该代理自己搭建了邮件服务器并亲自发送邮件；它的运行规则包括：不得冒用操作者身份、不得伪造文件或绕过身份验证，以及当有人真诚询问时不得谎称自己是人类。这些运行细节表明，此类代理获得的是真实的基础设施和资金资源，而不仅仅是对话轮次。

rss · Schneier on Security · 9月2日 18:28

**背景**: Claude 是 Anthropic 开发的一系列大语言模型；自 Claude 3 以来通常分为 Haiku、Sonnet 和 Opus 三个版本，并采用基于“宪法”的训练技术来提升伦理与合规表现。Base 是由 Coinbase 创建的以太坊 Layer-2 区块链，常用于 Web3 应用。在施奈尔的例子中，带 root 权限的 VPS 和存有 gas 费用的 Base 钱包构成了一种典型的自主代理沙盒式环境，使模型能够操作服务器并支付区块链交易费用，同时完成指定的财务目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/overview">Models overview - Claude Platform Docs</a></li>
<li><a href="https://www.gate.com/learn/articles/what-is-base-blockchain/743">What Is Base Blockchain ? Layer 2 Explained | Gate Learn</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#security`, `#autonomous AI`, `#Bruce Schneier`

---

<a id="item-9"></a>
## [CISA 将七个已遭利用的漏洞新增至 KEV 目录](https://www.cisa.gov/news-events/alerts/2026/09/02/cisa-adds-seven-known-exploited-vulnerabilities-catalog) ⭐️ 8.0/10

2026 年 9 月 2 日，CISA 将七个新漏洞加入其“已知被利用漏洞目录”（KEV Catalog），涉及 Sangoma Switchvox、Kludex Starlette、Kestra OSS、BerriAI LiteLLM、JFrog Artifactory 和 SonicWall SMA1000 等产品。每个漏洞均基于已被实际利用的证据加入。 将漏洞加入 KEV 目录是一个强烈信号，表明恶意行为者正在积极利用这些漏洞，因此安全团队可以在遭受入侵前优先修复。其影响不止于联邦机构，CISA 鼓励所有组织在基于风险的漏洞管理中，将 KEV 列出的 CVE 视为紧急事项。 七个新增条目为：CVE-2026-9586（Sangoma Switchvox SQL 注入）、CVE-2026-48710（Kludex Starlette HTTP 请求/响应走私）、CVE-2026-49869（Kestra OS 命令注入）、CVE-2026-59822（BerriAI LiteLLM 身份验证不当）、CVE-2026-82329（JFrog Artifactory 身份验证不当）、CVE-2026-83548（SonicWall SMA1000 服务端请求伪造）、CVE-2026-83549（SonicWall SMA1000 OS 命令注入）。公告还提到了 BOD 26-04，该指令要求 FCEB 机构优先快速修复公开暴露资产上的高风险 KEV 漏洞，并在应用补丁前确认系统是否已被入侵。

rss · CISA Cybersecurity Advisories · 9月2日 12:00

**背景**: KEV 目录是 CISA 维护的权威清单，收录已被证实在现实环境中遭到利用的漏洞，并以 CVE 标识。许多产品都存在带 CVE 编号的漏洞，但并非所有漏洞都已确认被积极利用，该目录的目的正是帮助网络防御者排定修复优先级。2026 年 9 月 2 日的这次新增与 BOD 26-04 的实施指导一致，该指令要求联邦机构优先快速修复 KEV 目录中列出的高风险漏洞。CISA 还提供提名表单，供用户上报尚未列入目录的已遭利用漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisa.gov/known-exploited-vulnerabilities-catalog">Known Exploited Vulnerabilities Catalog | CISA</a></li>
<li><a href="https://www.armosec.io/glossary/known-exploited-vulnerabilities-catalog-kev/">What is the Known Exploited Vulnerabilities Catalog (KEV)?</a></li>

</ul>
</details>

**标签**: `#CISA`, `#KEV`, `#vulnerabilities`, `#security`, `#CVE`

---

<a id="item-10"></a>
## [谷歌、Anthropic、OpenAI 发布网络安全 AI 模型及防护计划](https://thehackernews.com/2026/09/google-anthropic-and-openai-unveil.html) ⭐️ 8.0/10

谷歌发布了其最强网络安全模型 Gemini 3.8 Flash Cyber，并推出 Fairwind 计划，为可信防御者提供早期访问权限。此次更广泛的公告还包括 Anthropic 和 OpenAI 发布的新网络安全 AI 模型及防护举措。 Gemini 3.8 Flash Cyber 的定价与 Gemini 3.7 Flash 相同，分别为每百万输入 token 0.75 美元和每百万输出 token 3.75 美元。Fairwind 计划仅面向获批的可信合作伙伴，可单独使用，也可与自动修补工具 CodeMender 搭配使用。

rss · The Hacker News · 9月2日 18:27

**背景**: AI 公司一直在开发通用大语言模型，而网络安全专用变体则专为漏洞检测和自动生成补丁等任务设计。Fairwind 计划反映了行业的一个更广泛趋势：将强大的网络能力仅提供给可信组织，以尽量减少滥用。这类模型通常通过云平台和有针对性的访问计划提供，而非面向公众全面开放。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/">Introducing Gemini 3.8 Flash and 3.8 Flash Cyber - The Keyword</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/safety-security/fairwind-program/">Google ’s Fairwind Program : Cyber defense tools for trusted partners</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-8-flash/">Gemini 3.8 Flash - Model Card — Google DeepMind</a></li>

</ul>
</details>

**标签**: `#AI`, `#Cybersecurity`, `#Gemini`, `#Anthropic`, `#OpenAI`

---

<a id="item-11"></a>
## [恶意 .git 配置可让 AI 编程代理执行攻击者代码](https://thehackernews.com/2026/09/malicious-git-configs-can-make-claude.html) ⭐️ 8.0/10

Manifold Security 披露了影响七个命令行 AI 编程代理（包括 Claude、Codex、Cursor）的八个安全漏洞；恶意 Git 仓库的 .git 配置可指定一个命令，让代理在开发者机器上执行。截至发布时，其中四个漏洞仍未修复。 这些漏洞使克隆或打开恶意仓库即可在开发者权限下执行任意命令，绕过沙箱和审批提示。由于 AI 编码代理正越来越多地被信任处理代码仓库，这给开发者机器与软件供应链安全带来直接风险。 命令以用户身份在代理沙箱之外执行，且不会弹出审批提示；利用该漏洞的前提是恶意仓库被克隆或打开到代理中。披露时八个漏洞中仍有四个未修复。

rss · The Hacker News · 9月2日 14:06

**背景**: Claude Code、Codex CLI、Cursor 等 AI 编程代理帮助开发者编辑和运行代码，它们通常会信任来自仓库的本地配置。Git 仓库包含 .git/config 文件，可定义别名或钩子等自定义命令；当代理打开仓库时，可能执行这些配置的命令。GitSpawn 攻击演示了恶意仓库在打开时即可在开发者机器上执行代码，无需任何提示或批准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/gitspawn-flaws-execute-code/">GitSpawn Flaws Let Malicious Repositories Execute Code in ...</a></li>
<li><a href="https://izoologic.com/threat-advisory/cursor-zero-day-git-exe-windows-code-execution/">Cursor Zero-Day Lets Malicious Git Repositories Execute Code ...</a></li>
<li><a href="https://aviatrix.ai/threat-research-center/cursor-flaw-lets-malicious-cloned-repositories-trigger-windows-code-execution/">Cursor Vulnerability Allows Malicious Repositories to Execute ...</a></li>

</ul>
</details>

**标签**: `#security`, `#AI coding agents`, `#Git`, `#vulnerabilities`, `#supply chain`

---

<a id="item-12"></a>
## [BGP 劫持导致恶意 Virtualizor 更新，危及 hypervisor 的 root 权限](https://thehackernews.com/2026/09/bgp-hijack-delivers-malicious.html) ⭐️ 8.0/10

Virtualizor 披露，攻击者劫持了 Softaculous 的 BGP 路由，将更新流量重定向，并向少量安装派发了恶意的 Virtualizor 软件包。事件窗口大约始于 8 月 28 日 20:57，一家托管服务商报告其检查的 34 台 Virtualizor hypervisor 中有 5 台遭到 root 级别入侵。 这是一次真实的供应链攻击，利用互联网路由的信任机制，通过厂商自身的更新渠道推送恶意软件。它凸显了托管服务商和控制面板生态系统面临的风险，因为 hypervisor 一旦被攻破，运行在该服务器上的所有租户都可能受到影响。 根据 Virtualizor 的事件报告，只有流量被重定向期间检查更新的安装才会收到恶意软件包，该厂商称受影响数量很小。另一家托管服务商表示，其检查的 34 台 Virtualizor hypervisor 中有 5 台遭到 root 级别的破坏。

rss · The Hacker News · 9月2日 13:12

**背景**: BGP 劫持是一种恶意重路由互联网流量的攻击方式，通过篡改使用边界网关协议（BGP）维护的路由表来实现。Virtualizor 等虚拟化软件运行在 hypervisor 上，hypervisor 是物理服务器上创建和管理虚拟机的软件层。Softaculous 是一个广泛使用的 Web 应用自动安装器，与 cPanel、Plesk、DirectAdmin 等控制面板集成。由于软件更新通过网络获取，被劫持的路由可让攻击者用恶意载荷替换合法更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.virtualizor.com/blog/security-incident-bgp-hijacking/">Security Incident – BGP Hijacking – Virtualizor</a></li>
<li><a href="https://cybersecuritynews.com/virtualizor-compromise/">BGP Hijack Diverts Softaculous Traffic to Deliver Malicious Virtualizor ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/BGP_hijacking">BGP hijacking - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#BGP hijack`, `#supply chain attack`, `#Virtualizor`, `#malware`

---

<a id="item-13"></a>
## [Meta 广告传播 StreamRat Android 木马，可获得近乎完全的设备控制权](https://thehackernews.com/2026/09/meta-ads-push-streamrat-android-trojan.html) ⭐️ 8.0/10

ThreatFabric 披露了一种名为 StreamRat 的新型 Android 银行木马，它通过 Meta 上虚假的电视流媒体广告进行传播，专门针对西班牙语用户。该活动估计触达了欧盟约 570,950 个 Meta 账户，恶意软件能够赋予攻击者近乎完全控制受感染设备的能力。 这起披露表明，网络犯罪分子正越来越多地滥用 Meta 等合法社交媒体广告平台，以大规模分发银行木马。由于 StreamRat 会请求无障碍服务权限，它可以绕过用户的安全防护并实施设备端欺诈，对受害者的银行账户和个人数据构成严重威胁。 该木马启动后会立即请求无障碍服务权限，以便执行后续恶意操作，随后连接至其命令与控制（C2）服务器。攻击者使用针对西班牙的虚假流媒体广告，触达了估计约 570,950 个欧盟 Meta 账户。

rss · The Hacker News · 9月2日 12:22

**背景**: Android 银行木马是一类恶意软件，通过覆盖虚假登录页面等方式诱骗用户输入银行凭证，从而窃取资金和个人信息。许多此类木马滥用 Android 无障碍服务，这项功能原本用于帮助残障人士操作设备，却被攻击者用来自动点击按钮和授权恶意操作。利用 Meta 等可信平台的恶意广告活动覆盖面广，容易诱导用户安装来路不明的应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/09/meta-ads-push-streamrat-android-trojan.html">Meta Ads Push StreamRat Android Trojan That Can Gain...</a></li>
<li><a href="https://www.threatfabric.com/blogs/from-meta-ads-to-full-device-takeover-uncovering-streamrat">Uncovering StreamRat : From Meta Ads to Full Device Takeover</a></li>
<li><a href="https://www.malwarebytes.com/blog/news/2024/02/android-banking-trojans-how-they-steal-passwords-and-drain-bank-accounts">Android banking trojans: How they steal passwords and drain ...</a></li>

</ul>
</details>

**标签**: `#malware`, `#android`, `#cybersecurity`, `#trojan`, `#Metaads`

---

<a id="item-14"></a>
## [GeoNetwork 修复影响政府地理门户后端的未认证远程代码执行漏洞链](https://thehackernews.com/2026/09/geonetwork-fixes-unauthenticated-rce.html) ⭐️ 8.0/10

GeoNetwork 已在 2026 年 7 月 8 日发布的 4.4.12 和 4.2.17 版本中修复了一条未认证远程代码执行（RCE）漏洞链。该项目于 8 月 31 日公开了漏洞详情。 GeoNetwork 是许多政府和机构地理门户背后的基础组件，因此未认证 RCE 漏洞链对关键地理空间基础设施构成严重风险。攻击者可以在无需凭据的情况下远程利用该漏洞，因此所有受影响公共部门运营者必须尽快打补丁。 这两个漏洞影响开源地理空间元数据目录 GeoNetwork，并且可以串联起来实现未认证代码执行。已修复的版本为 4.4.12 和 4.2.17，漏洞详情于 8 月 31 日公布。

rss · The Hacker News · 9月2日 09:18

**背景**: GeoNetwork opensource 是一个免费开源的空间相关资源编目应用，广泛用于发布和发现地理空间元数据。地理门户（geoportal）是一种基于 Web 的网关，使用户能够查找、查看和访问地理空间信息及 GIS 服务，而 GeoNetwork 常作为这类门户的后端。该项目隶属于开放源代码地理空间基金会（OSGeo）生态，其起源与联合国相关的地理数据共享工作有关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geonetwork-opensource.org/">Home — GeoNetwork opensource</a></li>
<li><a href="https://en.wikipedia.org/wiki/GeoNetwork_opensource">GeoNetwork opensource - Wikipedia</a></li>
<li><a href="https://github.com/geonetwork/core-geonetwork">GitHub - geonetwork/core-geonetwork: GeoNetwork is a catalog ... GeoNetwork opensource - GitHub GeoNetwork opensource - Wikipedia GeoNetwork - The portal to spatial data and information Installing the software - GeoNetwork Opensource</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#RCE`, `#GeoNetwork`, `#open-source`

---

<a id="item-15"></a>
## [Switchvox 严重漏洞遭利用，攻击者无需凭据部署反向 Shell](https://thehackernews.com/2026/09/attackers-exploit-critical-switchvox.html) ⭐️ 8.0/10

攻击者正在积极利用 CVE-2026-9586，这是 Sangoma Switchvox SMB Edition 8.3（版本 104997）中的一个严重的未认证 SQL 注入漏洞。该漏洞的 CVSS 评分为 9.3，攻击者无需任何凭据即可通过反向 Shell 远程执行任意代码。 该漏洞影响重大，因为 Switchvox 是企业级 VoIP 平台，未经认证的远程代码执行可让攻击者完全入侵通信基础设施，窃听通话、向内部网络横向移动或投放勒索软件。运行受影响版本的组织应将此视为紧急修补事项。 该漏洞属于未认证 SQL 注入，可进一步利用为远程代码执行并植入反向 Shell。受影响的版本为 Sangoma Switchvox SMB Edition 8.3（构建版本 104997）；CVE-2026-9586 的 CVSS 评分为 9.3，且已在野外观察到利用活动。

rss · The Hacker News · 9月2日 07:08

**背景**: Switchvox 是 Sangoma 面向企业提供的本地部署统一通信与 PBX 平台。SQL 注入漏洞允许攻击者操纵数据库查询，若进一步与系统命令结合，可形成反向 Shell——即受害机器主动向外连接攻击者服务器并交出远程控制权。反向 Shell 是攻击者常用手段，因为它能绕过入站防火墙限制。CVE-2026-9586 的特别之处在于利用时不需要任何凭据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sangoma.com/products/phones-and-hardware/products/uc-appliances/switchvox/">Switchvox - Sangoma Technologies</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reverse_shell">Reverse shell</a></li>
<li><a href="https://horizon3.ai/attack-research/disclosures/cve-2026-9586-sangoma-switchvox-rce/">CVE - 2026 - 9586 : Sangoma Switchvox RCE | Horizon3</a></li>

</ul>
</details>

**标签**: `#security`, `#CVE`, `#SQL injection`, `#VoIP`, `#exploit`

---

<a id="item-16"></a>
## [WordPress 备份插件严重漏洞可致网站被接管](https://www.bleepingcomputer.com/news/security/wordpress-backup-plugin-flaw-exposes-millions-of-sites-to-takeover-attacks/) ⭐️ 8.0/10

WordPress 插件 All-in-One WP Migration and Backup 被披露存在一个严重的未授权 SQL 注入漏洞。攻击者利用该漏洞可远程执行任意代码，并完全接管受影响的网站，影响数百万 WordPress 站点。 由于该插件广泛用于网站迁移和备份，此漏洞使未认证攻击者能够以较低门槛入侵 WordPress 网站。由于可能导致远程代码执行和完全接管，网站所有者必须立即评估自身风险并尽快应用可用补丁。 据报告，该 SQL 注入漏洞可被升级为远程代码执行，使攻击者完全控制 WordPress 环境。由于漏洞无需任何身份验证，且该插件是最受欢迎的 WordPress 迁移和备份工具之一，因此风险尤为严重。

rss · BleepingComputer · 9月2日 19:28

**背景**: WordPress 支撑着大量网站，而插件用于扩展其功能；All-in-One WP Migration 是一款帮助用户在不同主机间导出、导入或迁移整个网站的流行工具。SQL 注入是一种常见的 Web 安全漏洞，通常发生在应用程序将未经校验的用户输入拼接到数据库查询中时。在此事件中，插件安装量巨大、漏洞严重且可实现远程代码执行，这些因素叠加导致其风险评级很高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wordpress.org/plugins/all-in-one-wp-migration/">All - in - One WP Migration and Backup – WordPress plugin</a></li>
<li><a href="https://portswigger.net/web-security/sql-injection">What is SQL Injection? Tutorial & Examples | Web Security Academy</a></li>
<li><a href="https://owasp.org/www-community/attacks/SQL_Injection">SQL Injection | OWASP Foundation</a></li>

</ul>
</details>

**标签**: `#security`, `#WordPress`, `#vulnerability`, `#SQL injection`, `#plugin`

---

<a id="item-17"></a>
## [黑客利用 JFrog Artifactory 严重漏洞伪造管理员令牌](https://www.bleepingcomputer.com/news/security/hackers-exploit-critical-jfrog-artifactory-flaw-to-forge-admin-tokens/) ⭐️ 8.0/10

攻击者正在积极利用 JFrog Artifactory 中的一个严重身份验证绕过漏洞（CVE-2026-82329）来伪造具有管理员权限的令牌。该攻击活动使未经授权的用户能够在受影响的 Artifactory 实例上获得完全管理员权限。 JFrog Artifactory 在 DevOps 环境中被广泛用于管理软件制品，因此该漏洞可能破坏软件供应链的完整性。依赖 Artifactory 的组织应尽快应用补丁，并审计现有访问令牌是否存在未经授权的使用迹象。 该漏洞是一个身份验证绕过漏洞，允许攻击者在没有有效凭据的情况下伪造管理员令牌。初始报告未披露具体受影响版本和补丁可用性，因此管理员应查阅 JFrog 的安全公告以获取详细信息。

rss · BleepingComputer · 9月2日 15:47

**背景**: JFrog Artifactory 是一个通用制品仓库管理器，用于在软件开发生命周期中存储和管理二进制文件、软件包、容器以及 AI/ML 模型。身份验证绕过漏洞是指攻击者能够绕过身份验证机制获得未授权访问，通常通过篡改请求或伪造令牌实现。由于 Artifactory 位于许多 DevSecOps 管道的核心位置，此类漏洞可能使攻击者注入恶意代码、窃取敏感数据或破坏构建流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jfrog.com/artifactory/">Artifactory | Universal Artifact Repository Manager | JFrog</a></li>
<li><a href="https://www.automox.com/blog/vulnerability-definition-authentication-bypass">What is Authentication Bypass?</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/identity-security/authentication-bypass/">What Is Authentication Bypass? Techniques & Examples</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#JFrog Artifactory`, `#CVE`, `#exploit`

---

<a id="item-18"></a>
## [Perplexity 开源为 Qwen 3.6 打造的 Mac 推理服务器 Lily](https://www.reddit.com/r/LocalLLaMA/comments/1w5ozl4/perplexity_opensourced_their_mac_inference_server/) ⭐️ 8.0/10

Perplexity 已将其为 Apple Silicon 与 Qwen3.6-35B-A3B 模型专门优化的轻量级本地推理引擎 Lily 开源。相关代码现已在 GitHub 的 pplx-garden 仓库中的 lily 目录下提供。 这一举措意义重大，因为它为本地大模型社区带来了一款生产级、针对特定模型优化的推理服务器，有望提升 Mac 用户设备端的推理性能。它还可能推动更多针对 Apple 硬件的单模型优化，并促进本地与云端混合 AI 工作流的发展。 Lily 专为 Apple Silicon 设计，对提示预填充（prefill）与 token 生成两个阶段分别进行了优化。Perplexity 还推出了一个混合计算编排器，可在 Lily 与云端前沿模型之间自动分配 AI 任务，无需手动配置。

reddit · r/LocalLLaMA · /u/Specter_Origin · 9月2日 22:13

**背景**: Apple Silicon Mac 虽然可以在本地运行大型语言模型，但通用移植版本往往无法充分利用其统一内存架构。像 Lily 这样的推理引擎正是为了在该硬件上提升提示处理与 token 生成速度而打造的。Qwen3.6-35B-A3B 是 Qwen 近期推出的稀疏混合专家（MoE）模型，总参数量为 350 亿，激活参数量为 30 亿。Perplexity 的博客将 Lily 描述为将本地设备端推理与云端 API 结合的混合方案的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.perplexity.ai/ko/hub/blog/optimizing-on-device-inference-for-apple-silicon">Optimizing On-Device Inference for Apple Silicon</a></li>
<li><a href="https://www.marktechpost.com/2026/06/05/perplexity-ai-introduces-hybrid-local-server-inference-orchestrator-for-personal-computer-automatic-on-device-and-cloud-task-routing/">Perplexity AI Introduces Hybrid Local-Server Inference Orchestrator for Personal Computer: Automatic On-Device and Cloud Task Routing - MarkTechPost</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-35B-A3B">Qwen/Qwen3.6-35B-A3B · Hugging Face</a></li>

</ul>
</details>

**标签**: `#inference`, `#open-source`, `#Apple Silicon`, `#Qwen`, `#LLM`

---

<a id="item-19"></a>
## [谷歌胜诉，广告技术业务逃过强制拆分](https://www.nytimes.com/2026/09/02/technology/google-ad-tech-remedies.html) ⭐️ 7.0/10

2026 年 9 月 2 日，谷歌击败了美国政府要求其强制出售广告技术业务的诉讼，避免了该业务被拆分。这一裁决作出之际，谷歌的广告技术收入仍在持续下滑。 这一裁决对谷歌来说是一次重大的反垄断胜利，消除了其核心业务之一面临结构性拆分的直接威胁。它也表明，监管机构要迫使大型数字平台拆分是多么困难。 谷歌的广告技术业务去年收入为 300 亿美元，约占 Alphabet 总收入的 8%，但该业务已连续 16 个季度下滑，在公司利润中占比不到 1%。案件的核心是谷歌对数字展示广告买卖工具的控制。

hackernews · donohoe · 9月2日 14:46 · [社区讨论](https://news.ycombinator.com/item?id=49537131)

**背景**: 广告技术（ad tech）是指广告主、发布商和平台用于购买、出售和衡量数字广告活动的工具与软件。美国政府起诉谷歌的理由是，谷歌在广告交易平台和发布商工具等连接广告主与网站广告位的环节占据主导地位。谷歌在美国和欧洲面临多起反垄断挑战，但在大型科技公司案件中，强制剥离仍是很少使用的补救措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://advertising.amazon.com/library/guides/what-is-adtech">What is AdTech ? A Beginner's Guide | Amazon Ads</a></li>
<li><a href="https://www.nexd.com/blog/advertising-technology-a-guide/">NEXD - What is Advertising Technology ( AdTech ) - A Guide and...</a></li>
<li><a href="https://www.ionos.com/digitalguide/online-marketing/web-analytics/what-is-adtech/">What is AdTech ? Advertising technology explained - IONOS</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：有人认为合并公司与拆分公司应该同样困难，也有人指出广告技术业务正在萎缩，“没人关心”这项业务。还有人建议对垄断企业累进征税，也有人对美国联邦政府能否有效处理垄断问题表示怀疑。

**标签**: `#antitrust`, `#google`, `#ad-tech`, `#regulation`, `#tech-policy`

---

<a id="item-20"></a>
## [Mistral 数据训练退出选项引发用户质疑](https://help.mistral.ai/en/articles/455207-can-i-opt-out-of-my-input-or-output-data-being-used-for-training) ⭐️ 7.0/10

Mistral 的帮助文档称，在某些情况下用户的输入和输出数据可能被用于模型训练，并声称用户有权随时退出。社区讨论者指出，近期变更使 Team 级客户在默认情况下可选择将数据用于训练，这与之前的预期相矛盾。 AI 数据隐私问题日益受到关注，而 Mistral 因欧盟推动数字主权而被视为欧洲旗舰 AI 公司。这一事件凸显出，即使是标榜注重隐私的公司也可能改变默认数据使用方式，从而影响企业对 AI 供应商的信任。 该帮助页面称‘在某些情况下’用户数据可能‘被纳入 Mistral 的模型训练计划’，并声称用户‘保留完全控制权’。一家组织称其改用 Team 级以获得集中隐私控制，但后来发现这些设置默认变为允许训练，而且失去了集中关闭训练的能力。

hackernews · teekert · 9月2日 12:30 · [社区讨论](https://news.ycombinator.com/item?id=49535284)

**背景**: Mistral AI 是一家法国人工智能公司，成立于 2023 年，以开发大型语言模型著称，其中许多模型以开源许可证发布。欧洲政府和企业日益将 Mistral 视为美国 AI 提供商的战略替代方案。许多 AI 服务默认使用用户提供的内容进行训练，而退出机制往往十分复杂且可能随时变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mistral_AI">Mistral AI</a></li>
<li><a href="https://www.wired.com/story/how-to-stop-your-data-from-being-used-to-train-ai/">How to Stop Your Data From Being Used to Train AI - WIRED</a></li>

</ul>
</details>

**社区讨论**: 评论中最强烈的情绪是不信任：有人认为认为厂商不会在未经同意的情况下使用提示词训练是‘天真’，也有人讲述自己被微软‘背刺’，或因切换等级后失望于 Mistral 的隐私控制。少数人指出文档本身明确说用户可以退出，并批评标题具有误导性，但整体氛围仍充满怀疑。

**标签**: `#AI privacy`, `#data training`, `#opt-out`, `#Mistral`, `#trust`

---