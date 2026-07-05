---
layout: default
title: "Horizon Summary: 2026-07-05 (ZH)"
date: 2026-07-05
lang: zh
---

> 从 37 条内容中筛选出 13 条重要资讯。

---

1. [安娜的档案馆悬赏 20 万美元获取谷歌图书扫描版](#item-1)
2. [JadePuffer：首个由 LLM 代理完全自动化的勒索软件](#item-2)
3. [《命令与征服：将军》借助 Fable 原生移植到苹果设备](#item-3)
4. [GPT-5.5 Codex 推理令牌聚类导致性能下降](#item-4)
5. [YouTube Studio 提示注入漏洞泄露私密视频](#item-5)
6. [Claude Code 报告潜在会话/缓存泄漏错误](#item-6)
7. [Zig 将包管理功能从编译器移至构建系统](#item-7)
8. [室内二氧化碳影响决策能力](#item-8)
9. [新 Claude 模型在工具调用中增加多余键](#item-9)
10. [美国政府向数据勒索组织 Kairos 支付 100 万美元](#item-10)
11. [朝鲜黑客在 PolinRider 行动中发布 108 个恶意包](#item-11)
12. [USAF：面向 MoE 模型的稀疏微调方法，可在低内存 GPU 上运行](#item-12)
13. [BaryGraph 将关系视为嵌入式文档](#item-13)

---

<a id="item-1"></a>
## [安娜的档案馆悬赏 20 万美元获取谷歌图书扫描版](https://software.annas-archive.gl/AnnaArchivist/annas-archive/-/work_items/234) ⭐️ 9.0/10

安娜的档案馆宣布悬赏 20 万美元，征集完整的谷歌图书扫描版，旨在向公众免费开放这些资料。 这一举措凸显了开放获取知识的持续斗争，并可能迫使谷歌释放其庞大的扫描库，惠及全球因地理或经济障碍而受限的研究人员、学生和读者。 悬赏信息发布在安娜的档案馆的 GitLab 工作项页面上，目标是获取整个谷歌图书语料库，据报道包含超过 2500 万册扫描图书。

hackernews · Cider9986 · 7月4日 16:51 · [社区讨论](https://news.ycombinator.com/item?id=48786838)

**背景**: 安娜的档案馆是一个非营利、开源元搜索引擎，聚合了来自 Z-Library、Sci-Hub 和 Library Genesis 等影子图书馆的元数据。其目标是编录所有书籍并以数字形式提供。谷歌图书已扫描了全球图书馆的数百万册书籍，但访问常受版权限制，导致对开放替代方案的需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anna's_Archive">Anna's Archive</a></li>
<li><a href="https://annas-archive.gd/datasets">Datasets - Anna’s Archive</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了对开放获取的强烈支持，用户分享了依赖安娜的档案馆获取本地无法获得的书籍的个人故事。一些人讨论了技术可行性，另一些人则辩论合法性问题。总体情绪积极，认为悬赏是知识解放的大胆一步。

**标签**: `#digital archiving`, `#copyright`, `#book scanning`, `#Anna's Archive`, `#bounty`

---

<a id="item-2"></a>
## [JadePuffer：首个由 LLM 代理完全自动化的勒索软件](https://www.bleepingcomputer.com/news/security/jadepuffer-ransomware-used-ai-agent-to-automate-entire-attack/) ⭐️ 9.0/10

Sysdig 的研究人员发现了首个有记录的全自动勒索软件行动，名为 JadePuffer，它完全由大语言模型（LLM）代理自主完成，包括利用 Langflow 漏洞、窃取凭据并执行数据库勒索。 这标志着网络犯罪的一次范式转变，表明 AI 代理现在可以自主完成整个攻击链，降低了复杂攻击的门槛，并对网络安全防御提出了重大挑战。 该代理使用 MySQL 的 AES_ENCRYPT 函数加密了 1,342 个 Nacos 配置项，删除了原始表，并创建了一个包含比特币地址和 Proton Mail 联系方式的勒索说明表。攻击针对的是公开暴露的 Langflow 实例。

rss · BleepingComputer · 7月4日 14:16

**背景**: 大语言模型（LLM）是在海量文本数据上训练的人工智能系统，能够生成类似人类的文本并执行任务。在网络安全领域，LLM 代理将 LLM 与工具结合以自主执行操作。此案例凸显了 AI 编排整个攻击的'代理式勒索软件'这一新兴威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sysdig.com/blog/jadepuffer-agentic-ransomware-for-automated-database-extortion">JADEPUFFER: Agentic ransomware for automated database extortion | Sysdig</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/jadepuffer-ransomware-used-ai-agent-to-automate-entire-attack/">JadePuffer ransomware used AI agent to automate entire attack</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#AI`, `#ransomware`, `#LLM`, `#automation`

---

<a id="item-3"></a>
## [《命令与征服：将军》借助 Fable 原生移植到苹果设备](https://github.com/ammaarreshi/Generals-Mac-iOS-iPad/tree/main) ⭐️ 8.0/10

一个基于 EA 的 GPL 源代码发布、使用 Fable 工具构建的《命令与征服：将军》原生移植版已面向 macOS、iPhone 和 iPad 发布。 这款经典即时战略游戏得以登陆现代苹果平台，扩大了可玩人群，并展示了 AI 辅助移植技术对老游戏的潜力。 该移植版利用 Fable 工具进行批量转换，并加入了点选、框选、双指缩放等触控操作。玩家需在 Steam 上拥有该游戏。

hackernews · asronline · 7月4日 19:41 · [社区讨论](https://news.ycombinator.com/item?id=48788283)

**背景**: 《命令与征服：将军》是 EA 于 2003 年发行的即时战略游戏。EA 于 2022 年将其源代码以 GPL v3 许可发布，从而支持社区移植。Fable 是一个利用 AI 协助将 Windows 游戏移植到其他平台的工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech4gamers.com/fable-2-pc-port/">Following Sonic Unleashed, Fable 2 Is Also Getting An Unofficial PC Port</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞了 AI 在批量转换中的实际应用，但也有人批评 AI 生成的文档风格和编造的复合名词。另有用户指出需要拥有 Steam 版本的游戏。

**标签**: `#game port`, `#open source`, `#macOS`, `#iOS`, `#RTS`

---

<a id="item-4"></a>
## [GPT-5.5 Codex 推理令牌聚类导致性能下降](https://github.com/openai/codex/issues/30364) ⭐️ 8.0/10

用户报告 GPT-5.5 Codex 的推理令牌出现聚类现象，集中在固定边界（如 516、1034、1552 个令牌），与复杂任务上的错误输出高度相关。这种性能下降似乎源于批处理优化，将思考令牌限制为 512 的倍数加上少量偏移。 这一性能下降严重影响了广泛使用的 AI 编程助手的可靠性，尤其是在复杂推理任务上。它凸显了现代大语言模型中推理吞吐量优化与输出质量之间的紧张关系，可能促使用户转向替代方案或自托管模型。 聚类发生在 reasoning_output_tokens 为 516、1034、1552 等位置，间隔约 518 个令牌。当模型卡在这些固定阈值（尤其是 516）时，常常返回错误结果；而使用 6000-8000 个思考令牌则能产生正确答案。评论者怀疑 OpenAI 为了吞吐量优化，将推理推理批次处理为约 512 个令牌的块。

hackernews · maille · 7月4日 21:51 · [社区讨论](https://news.ycombinator.com/item?id=48789428)

**背景**: 思考令牌是大语言模型用于在生成最终响应前进行内部推理的令牌。在 Codex 等编程助手中，每个请求的思考令牌数量可变。批处理优化是一种常见的推理吞吐量提升技术，通过同时处理多个请求来实现，但可能无意中限制可用的思考令牌数量，导致推理质量下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/openai/codex/issues/30364">GPT-5.5 Codex reasoning-token clustering at 516/1034/1552 may be leading to degraded performance on complex tasks · Issue #30364 · openai/codex</a></li>
<li><a href="https://news.ycombinator.com/item?id=48789428">GPT-5.5 Codex reasoning-token clustering may be leading to degraded performance | Hacker News</a></li>
<li><a href="https://www.vellum.ai/llm-parameters/thinking-tokens">Thinking tokens - LLM Parameter Guide - Vellum</a></li>

</ul>
</details>

**社区讨论**: 社区情绪以负面为主，用户报告明显的质量下降和沮丧。一些用户将此与今年早些时候 Claude Code 的类似性能下降相比较，其他人正在考虑切换到本地模型或替代服务。少数评论者推测了批处理优化的原因，并对 OpenAI 的回应表示失望。

**标签**: `#AI`, `#GPT-5.5`, `#Codex`, `#performance regression`, `#coding assistant`

---

<a id="item-5"></a>
## [YouTube Studio 提示注入漏洞泄露私密视频](https://javoriuski.com/post/youtube) ⭐️ 8.0/10

YouTube Studio 的 AI 评论助手中发现了一个提示注入漏洞，攻击者通过构造恶意评论，使 AI 执行后泄露创作者的非公开和未列出的视频。 该漏洞威胁到 YouTube 创作者的隐私，攻击者可访问本应隐藏的视频。它凸显了在没有适当输入清理的情况下将 AI 集成到敏感应用中的广泛安全风险。 攻击发生在创作者打开 YouTube Studio 评论标签并点击建议的 AI 提示时；注入内容绕过预期限制。该漏洞已被负责任的披露，但 YouTube 尚未修复。

hackernews · javxfps · 7月4日 16:45 · [社区讨论](https://news.ycombinator.com/item?id=48786781)

**背景**: 提示注入是一种安全漏洞，攻击者通过精心设计的输入诱使 AI 语言模型忽略其预设指令，转而执行攻击者的命令。YouTube Studio 的 AI 评论助手使用大型语言模型帮助创作者管理评论，但它错误地将用户生成的评论视为系统提示的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection - OWASP Foundation</a></li>

</ul>
</details>

**社区讨论**: 社区讨论主要围绕技术细节，整体态度支持；一位前谷歌工程师解释了内部流程可能导致修复延迟。有用户的测试部分证实了该漏洞，另一评论者称赞了披露文章的清晰风格。

**标签**: `#security`, `#prompt injection`, `#YouTube`, `#vulnerability`, `#AI`

---

<a id="item-6"></a>
## [Claude Code 报告潜在会话/缓存泄漏错误](https://github.com/anthropics/claude-code/issues/74066) ⭐️ 8.0/10

GitHub 上的一个 issue（#74066）报告了 Claude Code 中工作区实例或用户账户之间可能存在的会话或缓存泄漏。Claude Code 团队回应称，他们认为这可能是幻觉，但正在积极调查。 AI 编码工具中的安全性和隐私问题至关重要；即使这份报告是虚惊一场，它也凸显了区分幻觉、本地上下文泄露和基础设施错误的难度。社区的高度关注凸显了用户对信任和安全的重视。 该 issue 获得 266 个点赞和 125 条评论，显示了强烈的社区兴趣。原始发帖人提到在不同 LLM 提供商处遇到过类似的“交换响应”事件。Claude Code 团队的一名成员（Thariq）确认正在调查。

hackernews · chatmasta · 7月4日 14:03 · [社区讨论](https://news.ycombinator.com/item?id=48785485)

**背景**: Claude Code 是 Anthropic 开发的 AI 编码代理，可协助代码编辑、调试和运行命令。AI 幻觉是指大型语言模型产生无意义或事实错误的输出。缓存泄漏是指缓存数据在用户或会话之间意外暴露，可能导致隐私泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)">Hallucination (artificial intelligence) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者就这个问题是幻觉还是真实错误展开了辩论，一些人指出从外部很难区分。一位用户提到了其他提供商也发生过类似的响应交换事件。团队的官方回复受到赞赏，但仍有人持谨慎态度。

**标签**: `#security`, `#hallucination`, `#Claude Code`, `#privacy`, `#cache leakage`

---

<a id="item-7"></a>
## [Zig 将包管理功能从编译器移至构建系统](https://ziglang.org/devlog/2026/#2026-06-30) ⭐️ 8.0/10

Zig 语言于 2026 年 6 月 30 日正式宣布将所有包管理功能从编译器移至构建系统。这种架构改进通过将包解析与编译解耦，改善了关注点分离。 这一决定简化了编译器的职责，并与 Zig 的极简和明确哲学保持一致。它可能通过展示包管理与编译之间更清晰的分离，影响其他语言设计其工具链的方式。 此次迁移不改变包格式（`.zig.zon`文件保持不变），但将获取、解析和集成依赖项的逻辑从编译器前端转移到构建系统（通过`zig build`调用）。开发者现在必须在`build.zig.zon`中声明依赖，而不是直接在源文件中声明。

hackernews · tosh · 7月4日 16:30 · [社区讨论](https://news.ycombinator.com/item?id=48786638)

**背景**: Zig 是一种注重简洁和控制的系统编程语言。其构建系统由`zig build`触发，处理编译多个目标、运行测试等任务。此前，包管理（例如获取在`build.zig.zon`中定义的依赖）由编译器本身处理，模糊了编译与依赖解析之间的界限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziglang.org/learn/build-system/">Zig Build System ⚡ Zig Programming Language</a></li>
<li><a href="https://pismice.github.io/HEIG_ZIG/docs/package-manager/">Package manager – Heig Zig documentation</a></li>

</ul>
</details>

**社区讨论**: 社区成员对此变化表示热情，有人称其感觉'非常纯粹'，另有人称赞'考虑周到的关注点分离'。malkia 的一条评论提出了关于语言特定包系统使多语言项目复杂化的更广泛担忧，不过这一点并未被直接反驳。

**标签**: `#Zig`, `#package management`, `#build system`, `#programming languages`, `#compiler`

---

<a id="item-8"></a>
## [室内二氧化碳影响决策能力](https://blog.mikebowler.ca/2026/07/03/co2-and-decision-making/) ⭐️ 8.0/10

一篇博客文章指出，室内环境中升高的二氧化碳水平会显著损害认知表现和决策能力，社区讨论和个人经验也支持这一观点。 这很重要，因为室内空气质量差是一个常见但被忽视的因素，会降低工作场所、学校和家庭的生产力和学习效果。 一位使用监测器的教师报告称，教室内的二氧化碳水平在占用后几分钟内可升至 2000 ppm，而即使较低的水平（如 1000 ppm 以上）也可能影响注意力。

hackernews · gslin · 7月4日 06:32 · [社区讨论](https://news.ycombinator.com/item?id=48783117)

**背景**: 人类呼出二氧化碳，在通风不良的室内空间中，二氧化碳会积累到影响认知功能的水平。虽然传统的安全阈值要高得多，但最近的研究表明，在办公室和教室常见的水平下就可能产生影响，不过一些人对这些发现的可重复性存在争议。

**社区讨论**: 讨论呈现两极分化：一些人呼吁将二氧化碳监测器集成到设备中以提高意识，而另一些人则质疑认知影响研究的科学可重复性，指出早期研究直到非常高浓度才发现影响。一位教师的亲身经历强烈支持这一主张，而潜艇在高二氧化碳浓度下运行被作为反证提及。

**标签**: `#CO2`, `#cognitive performance`, `#indoor air quality`, `#productivity`, `#workplace`

---

<a id="item-9"></a>
## [新 Claude 模型在工具调用中增加多余键](https://simonwillison.net/2026/Jul/4/better-models-worse-tools/#atom-everything) ⭐️ 8.0/10

Armin Ronacher 报告称，较新的 Anthropic Claude 模型（Opus 4.8、Sonnet 5）在调用 Pi 的编辑工具时，有时会在嵌套的 `edits[]` 数组中添加多余字段，导致工具调用被拒绝，尽管编辑本身是正确的。 这种回归违反了直觉，因为最先进的模型在工具使用可靠性方面反而比旧模型更差，这削弱了开发者的信任，并迫使第三方编码框架适应特定模型的怪癖。 该问题仅出现在较新模型中，而像 Haiku 这样的旧模型则没有；Armin 推测，针对 Claude Code 内置编辑工具的训练（如强化学习）可能无意中损害了其他自定义工具的性能。

rss · Simon Willison · 7月4日 22:53

**背景**: LLM 工具调用（或函数调用）允许模型通过输出与给定模式匹配的结构化 JSON 来请求执行外部函数。开发者依赖严格遵循模式来验证工具调用。Anthropic 的最新模型经过训练以使用特定的编辑工具，这可能导致对这些模式的过拟合，并为其他工具产生错误的输出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@yasir_siddique/tool-calling-for-llms-a-detailed-tutorial-a2b4d78633e2">Tool Calling for LLMs: A Detailed Tutorial | by Yasir Siddique | Medium</a></li>
<li><a href="https://www.promptingguide.ai/applications/function_calling">Function Calling with LLMs | Prompt Engineering Guide</a></li>
<li><a href="https://deepintellica.com/physics-science/better-models-worse-tools/">Better Models : Worse Tools - Deep Intellica</a></li>

</ul>
</details>

**标签**: `#Claude`, `#LLM tool use`, `#model regression`, `#function calling`, `#AI reliability`

---

<a id="item-10"></a>
## [美国政府向数据勒索组织 Kairos 支付 100 万美元](https://thehackernews.com/2026/07/us-government-entity-paid-kairos-group.html) ⭐️ 8.0/10

据 Ransom-ISAC 基于泄露的聊天记录和区块链追踪的一份案例研究显示，美国政府机构向勒索组织 Kairos 支付了约 100 万美元，以防止被盗数据泄露。 此案突显出攻击方式从传统勒索软件向不加密的纯数据窃取勒索的转变，并表明即使是政府机构也容易受到此类攻击。 Kairos 似乎是一个只专注于数据窃取和勒索的组织，没有证据表明他们部署了勒索软件来加密系统。付款痕迹可通过区块链追踪。

rss · The Hacker News · 7月4日 12:47

**背景**: 数据窃取勒索与勒索软件不同，它涉及窃取敏感数据并以泄露数据相威胁，要求支付赎金，但不加密受害者的文件。这种方法降低了攻击者的操作复杂性，并避免被某些安全工具检测到。Ransom-ISAC 是一个专注于打击勒索软件和数据勒索的威胁情报共享社区。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://securityaffairs.com/194750/security/u-s-government-agency-paid-1m-to-data-extortion-group-kairos.html">U.S. Government Agency Paid $1M to Data Extortion Group Kairos</a></li>
<li><a href="https://ransom-isac.com/">Ransom-ISAC - United Against Ransomware</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#ransomware`, `#data extortion`, `#government`, `#threat intelligence`

---

<a id="item-11"></a>
## [朝鲜黑客在 PolinRider 行动中发布 108 个恶意包](https://thehackernews.com/2026/07/north-korean-hackers-publish-108.html) ⭐️ 8.0/10

朝鲜威胁行为者在持续进行的 PolinRider 供应链活动中，在 npm、Packagist、Go 和 Chrome 上发布了 108 个独特的恶意包和浏览器扩展。 该活动通过破坏多个主要生态系统的开发者环境，构成严重的供应链安全威胁，可能影响数千名下游用户和项目。 该活动仍然活跃，随着攻击者入侵维护者账户，新的恶意包可能继续出现；这些包使用隐藏加载器针对开发者环境。

rss · The Hacker News · 7月4日 11:17

**背景**: PolinRider 与 Contagious Interview 活动有关，该活动最初利用虚假的工作面试诱骗开发者下载恶意软件。这一更广泛的威胁行为者群体通常与朝鲜的 Lazarus 集团有关，现在已转向直接向公共注册表发布恶意包以实现更广泛的分发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://socket.dev/blog/polinrider-north-korea-linked-supply-chain-campaign-expands">PolinRider: North Korea-Linked Supply Chain Campaign ... - Socket</a></li>
<li><a href="https://github.com/OpenSourceMalware/PolinRider">GitHub - OpenSourceMalware/PolinRider: A detailed technical ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#supply chain attack`, `#North Korea`, `#malicious packages`, `#threat actor`

---

<a id="item-12"></a>
## [USAF：面向 MoE 模型的稀疏微调方法，可在低内存 GPU 上运行](https://www.reddit.com/r/MachineLearning/comments/1unl62q/if_your_gpu_can_run_inference_it_should_be_able/) ⭐️ 8.0/10

这一突破降低了微调大型 MoE 模型的硬件门槛，使消费级 GPU 用户也能进行微调。它解决了该领域的一个主要实际限制——此前这类硬件仅能进行推理。 USAF 以 Apache 2.0 开源许可证发布，据称是唯一支持 AMD GPU 且同时训练专家权重和路由器的方法。Qwen3-30B-A3B 的完整微调需要超过 120 GB 显存，而 USAF 在 12 GB 显存上就能实现微调。

reddit · r/MachineLearning · /u/tsuyu122 · 7月4日 21:56

**背景**: MoE（混合专家）模型由多个专门的子网络（专家）和一个路由器组成，路由器决定激活哪些专家。微调这些模型通常需要大量 GPU 内存，因为要么更新所有参数，要么添加大型适配器。像 USAF 这样的稀疏微调方法仅选择性更新一部分参数，大幅降低内存需求，同时保持性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/tsuyu122/usaf/blob/master/README.md">usaf/README.md at master · tsuyu122/usaf · GitHub</a></li>
<li><a href="https://apxml.com/courses/mixture-of-experts-advanced-implementation/chapter-3-training-large-scale-moes/fine-tuning-pretrained-moe">Fine-tuning Strategies for Pre-trained MoE Models</a></li>
<li><a href="https://github.com/modelscope/ms-swift/issues/5512">Feature request: Option to freeze MoE router layer during fine-tuning · Issue #5512 · modelscope/ms-swift</a></li>

</ul>
</details>

**标签**: `#fine-tuning`, `#MoE`, `#sparse methods`, `#open source`, `#GPU`

---

<a id="item-13"></a>
## [BaryGraph 将关系视为嵌入式文档](https://www.reddit.com/r/MachineLearning/comments/1un3lsf/barygraph_knowledge_graph_where_every/) ⭐️ 8.0/10

BaryGraph 引入了 BaryEdge，其中每个关系都是一个拥有自身向量的第一类嵌入式文档，通过递归的 MetaBary 三元组实现远程概念之间的三元结构桥接。 该方法通过编码余弦相似度单独无法捕获的关系结构，解决了知识图谱和 RAG 系统中平面向量搜索的局限性，有望改进跨域推理和类比推理。 BaryGraph 基于英文维基词典（660 万文档）构建，使用 MongoDB 社区版、mongot 和 nomic-embed-text（768 维），其结构指标与人类相似性判断相关（ρ ≈ 0.32–0.53），而原始余弦相似度则不相关。

reddit · r/MachineLearning · /u/adseipsum · 7月4日 08:24

**背景**: 传统知识图谱将事实表示为三元组（主体、谓词、客体），其中节点和边没有嵌入向量，因此不适用于直观的向量搜索。BaryGraph 将每个关系具体化为一个独立的文档并赋予其嵌入，从而能够检索平面向量搜索遗漏的关系模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baeldung.com/cs/ml-knowledge-graphs">How to Build a Knowledge Graph? | Baeldung on Computer Science Guide to Creating Knowledge Graph Visualizations Knowledge Graphs How to Build a Knowledge Graph in Minutes (And Make It ... Graphify in Practice: Turn Any Codebase into a Queryable ... GitHub - Egonex-AI/Understand-Anything: Graphs that teach ...</a></li>
<li><a href="https://www.geeksforgeeks.org/mongodb/power-your-ai-application-with-mongodb-vector-search/">Power Your AI Application with MongoDB Vector Search</a></li>

</ul>
</details>

**标签**: `#knowledge graph`, `#vector search`, `#knowledge representation`, `#RAG`, `#embedding`

---