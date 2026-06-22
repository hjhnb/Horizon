---
layout: default
title: "Horizon Summary: 2026-06-22 (ZH)"
date: 2026-06-22
lang: zh
---

> 从 39 条内容中筛选出 11 条重要资讯。

---

1. [宁可重复代码也不要做错误的抽象](#item-1)
2. [开发者普遍误解 CORS](#item-2)
3. [sqlite-utils 4.0rc1：新增迁移和嵌套事务](#item-3)
4. [矩阵循环单元更新：稳定性改进与并行扫描](#item-4)
5. [在 GPT-2 中等规模上的无 Softmax 注意力模型](#item-5)
6. [Apertus：面向主权 AI 的开放基础模型](#item-6)
7. [Anthropic 要求 Claude 用户通过 Persona 进行身份验证](#item-7)
8. [软件销售的最小可行单元](#item-8)
9. [Peter Norvig 的经典 Python 实现 Lisp 解释器教程](#item-9)
10. [几何代数批判引发争议](#item-10)
11. [AryStinger 僵尸网络感染数千台 D-Link 路由器](#item-11)

---

<a id="item-1"></a>
## [宁可重复代码也不要做错误的抽象](https://sandimetz.com/blog/2016/1/20/the-wrong-abstraction) ⭐️ 8.0/10

Sandi Metz 在 2016 年的文章中提出，过早或错误的抽象比代码重复更糟糕，并敦促开发者推迟抽象直到明确的模式出现。 这一见解挑战了“不要重复自己”（DRY）的传统观念，并提供了一个关于何时重构的实用规则，帮助开发者避免过度设计并保持灵活性。 文章强调，重复通常比错误的抽象成本更低，因为消除重复比修复错误的抽象更容易。它建议在至少有三个重复实例之前不要进行抽象。

hackernews · rafaepta · 6月21日 16:08 · [社区讨论](https://news.ycombinator.com/item?id=48620090)

**背景**: 在软件工程中，抽象用于通过隐藏实现细节来简化代码。然而，过早的抽象可能导致僵化、难以更改的代码。Sandi Metz 的方法优先考虑清晰性和简单性，而非过早优化，提倡渐进式重构。

**社区讨论**: 评论者大多同意文章观点，但有些人警告说，违反单一事实来源的重复仍应重构。其他人指出函数式编程和 TypeScript 减少了抽象问题，还有一位用户分享了个人经历，称赞作者的工作坊。

**标签**: `#software engineering`, `#code duplication`, `#abstraction`, `#clean code`, `#refactoring`

---

<a id="item-2"></a>
## [开发者普遍误解 CORS](https://fosterelli.co/developers-dont-understand-cors) ⭐️ 8.0/10

一篇文章解释，CORS 并不限制跨域请求的发送，而是阻止浏览器读取响应，除非服务器明确允许，这是开发者常见的误解。 正确理解 CORS 对 Web 安全至关重要，配置错误可能导致安全漏洞。澄清这一概念有助于开发者避免常见陷阱，构建更安全的系统。 CORS 头部由浏览器强制执行，而非服务器，因此任何服务器都可以接收任意来源的请求。该机制仅控制浏览器能否访问和使用响应内容。

hackernews · toilet · 6月21日 01:35 · [社区讨论](https://news.ycombinator.com/item?id=48614844)

**背景**: 同源策略（SOP）是浏览器的一项安全措施，阻止来自一个源的脚本访问另一个源的数据。CORS 是一种标准，允许服务器有选择地放宽 SOP，以支持合法的跨域请求，例如来自不同域的 API 调用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CORS">CORS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Same-origin_policy">Same-origin policy</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/Security/Defenses/Same-origin_policy">Same-origin policy - Security | MDN - MDN Web Docs</a></li>

</ul>
</details>

**社区讨论**: 评论者争论细节：有人认为文章本身误读了 CORS，暗示它可以限制哪些来源可以与服务器通信；其他人则同意核心观点，即 CORS 被广泛误解。讨论突显了即使是有经验的开发者之间对 CORS 也存在深刻分歧和困惑。

**标签**: `#CORS`, `#web security`, `#HTTP`, `#a cross-origin requests`

---

<a id="item-3"></a>
## [sqlite-utils 4.0rc1：新增迁移和嵌套事务](https://simonwillison.net/2026/Jun/21/sqlite-utils/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0rc1 引入了数据库迁移支持（从 sqlite-migrate 包移植）和通过保存点实现的嵌套事务，这是一个重大版本候选发布，包含少量不向后兼容的更改。 此次发布为一个广泛使用的 SQLite 工具添加了关键的生产级功能，使 Python 开发者和数据从业者能够更安全地进行模式演进和更健壮的事务处理。 迁移系统使用基于装饰器的 API 来定义顺序迁移（例如，创建表、添加列），并可通过 Python 或 sqlite-utils migrate CLI 命令应用；它有意不提供反向迁移。嵌套事务通过 SQLite 保存点实现。

rss · Simon Willison · 6月21日 23:30

**背景**: sqlite-utils 是一个 Python 库和 CLI 工具，在 Python 内置的 sqlite3 模块之上提供高级操作，例如从 JSON 自动创建表和复杂的表转换。SQLite 本身不原生支持嵌套事务，但可以使用保存点来模拟。此候选版本集成了之前作为独立包维护的迁移系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library for manipulating SQLite databases · GitHub</a></li>
<li><a href="https://sqlite-utils.datasette.io/">sqlite - utils</a></li>
<li><a href="https://github.com/simonw/sqlite-migrate">GitHub - simonw/ sqlite - migrate : A simple database migration system...</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#python`, `#database`, `#release`, `#sqlite-utils`

---

<a id="item-4"></a>
## [矩阵循环单元更新：稳定性改进与并行扫描](https://www.reddit.com/r/MachineLearning/comments/1ubz5o8/an_update_on_matrix_recurrent_units_an_attention/) ⭐️ 8.0/10

作者重新审视了矩阵循环单元（MRU），一种线性时间注意力替代方案，并引入了多种方法来约束矩阵状态，如使用 Cayley 映射的斜对称矩阵和 LDU 分解，改进了训练稳定性。他们还实现了一种并行扫描以在 GPU 上高效执行。 MRU 为序列建模提供了线性时间复杂度，解决了标准注意力的二次瓶颈。稳定性改进和高效的并行扫描使其成为长上下文任务中更可行的选择，为寻找高效架构做出了贡献。 在 shakespeare-char 数据集上，一个小型 MRU 语言模型与类似规模的 Transformer 表现相当，但在 TinyStories 数据集上表现更差。作者发现正交矩阵阻碍了学习，表明剪切变换对模型的表达能力很重要。

reddit · r/MachineLearning · /u/mikayahlevi · 6月21日 19:39

**背景**: Transformer 使用自注意力机制，其复杂度随序列长度呈二次增长，因此处理超长序列时效率低下。矩阵循环单元（MRU）是一种循环架构，通过累积矩阵乘法以线性时间混合序列信息。并行扫描算法使得原本顺序的循环计算能够在 GPU 上高效执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/mikayahlevi/mru-lm">GitHub - mikayahlevi/mru-lm: An LM forked from my transformer ...</a></li>
<li><a href="https://medium.com/@wanimohit1/mamba-the-linear-time-alternative-to-transformers-thats-changing-llm-architecture-6470d0ad6ead">"Mamba: The Linear-Time Alternative to Transformers That's ... - Medium</a></li>

</ul>
</details>

**标签**: `#sequence modeling`, `#attention alternative`, `#linear-time architecture`, `#recurrent units`, `#efficiency`

---

<a id="item-5"></a>
## [在 GPT-2 中等规模上的无 Softmax 注意力模型](https://www.reddit.com/r/MachineLearning/comments/1ubmybr/i_released_a_softmaxfree_attention_model_at_gpt2/) ⭐️ 8.0/10

一个在 GPT-2 中等规模（约 3.54 亿参数，在 115 亿 tokens 上训练）的无 Softmax 注意力模型已发布，附带开放权重和自定义 Triton 内核，该内核实现了结构稀疏性和 tile-skipping 以节省长上下文场景下的显存。 这项工作表明，无 Softmax 注意力可以扩展到相当大的模型规模，并为长上下文 Transformer 提供实用的显存节省，有望在资源受限的环境中实现更高效的推理和训练。 该模型利用结构稀疏性减少注意力计算，并使用 tile-skipping 内核动态跳过无关的 tile，全部用 Triton 实现以保证灵活性；权重和内核已在 GitHub 上开源。

reddit · r/MachineLearning · /u/NonGameCatharsis · 6月21日 10:46

**背景**: 标准 Transformer 注意力使用 Softmax 操作来归一化注意力分数，这可能计算开销较大。无 Softmax 注意力用更简单的归一化（如ℓ1 范数）替代 Softmax，以降低开销。结构稀疏性（例如 N:M 模式）和 tile-skipping 是进一步加速计算和减少内存使用的优化技术。Triton 是一种基于 Python 的语言和编译器，用于编写高效的 GPU 自定义内核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openaccess.thecvf.com/content/WACV2024/papers/Koohpayegani_SimA_Simple_Softmax-Free_Attention_for_Vision_Transformers_WACV_2024_paper.pdf">SimA: Simple Softmax-free Attention for Vision Transformers</a></li>
<li><a href="https://github.com/triton-lang/triton">GitHub - triton-lang/triton: Development repository for the Triton ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S092523122400239X">Sparsity in transformers: A systematic literature review</a></li>

</ul>
</details>

**标签**: `#softmax-free attention`, `#efficient transformers`, `#Triton kernels`, `#long-context`, `#open source`

---

<a id="item-6"></a>
## [Apertus：面向主权 AI 的开放基础模型](https://apertvs.ai/) ⭐️ 7.0/10

Apertus 发布了一个完全开放的 700 亿参数基础模型，由学术和公共机构在阿尔卑斯超级计算机上训练，提供了一个完全符合欧盟 AI 法案的主权 AI 替代方案。 该项目解决了日益增长的主权 AI 担忧，特别是对于寻求减少对美国前沿实验室依赖的欧洲及其他地区，并为完全透明和可审计的 AI 开发树立了先例。 该模型完全开放，包括训练流程和数据集，并设计为尊重退出选项、移除个人身份信息（PII）并防止记忆。它在阿尔卑斯超级计算机上运行，旨在大规模满足欧盟 AI 法案要求。

hackernews · T-A · 6月21日 21:29 · [社区讨论](https://news.ycombinator.com/item?id=48622778)

**背景**: 主权 AI 是指国家或组织控制其整个 AI 技术栈的能力，包括基础设施、数据和模型。来自美国公司如 OpenAI 和 Anthropic 的主要前沿模型并非完全开放，引发了数据主权和依赖性的担忧。Apertus 是一项欧洲倡议，旨在创建一个完全开放的基础模型，作为专有系统的制衡力量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apertvs.ai/?trk=article-ssr-frontend-pulse_little-text-block">Fully Open Foundation Model for Sovereign AI</a></li>
<li><a href="https://modernorange.io/item/48622778">Apertus – Open Foundation Model for Sovereign AI | Modern Orange</a></li>
<li><a href="https://articles.phantom-byte.com/how-academia-trained-70b-model-apertus.html">How Academia Trained a 70B Model Without Big Tech's Budget</a></li>

</ul>
</details>

**社区讨论**: 社区成员将 Apertus 与其他完全开放的模型如 OLMo 和 K2 Think V2 进行比较，有人对其竞争力表示怀疑，认为其以委员会的速度推进。然而，其他人强调了团队专业知识的价值，指出如果团队有更多经验，他们可以以更低的成本取得更好的结果。

**标签**: `#open-source`, `#LLM`, `#AI sovereignty`, `#foundation model`, `#European AI`

---

<a id="item-7"></a>
## [Anthropic 要求 Claude 用户通过 Persona 进行身份验证](https://support.claude.com/en/articles/14328960-identity-verification-on-claude) ⭐️ 7.0/10

Anthropic 宣布，Claude 用户必须通过第三方服务 Persona 完成身份验证，这一政策变化至少自 2025 年 4 月起已生效。 此举引发了对隐私和可访问性的重大担忧，用户需向第三方提供政府颁发的身份证件，可能根据地区或验证状态限制对 AI 模型的访问。 Persona 可能将提交的数据用于欺诈预防模型的训练，且验证失败可能导致永久无法访问顶级模型，这与 OpenAI 的类似政策一致。

hackernews · bathory · 6月21日 12:44 · [社区讨论](https://news.ycombinator.com/item?id=48618455)

**背景**: 像 Persona 这样的身份验证服务用于遵守 KYC 和反洗钱法规，但在 AI 服务中使用它们引入了安全与用户隐私之间的张力。许多 AI 公司越来越要求身份检查以防止滥用，但批评者认为这限制了开放访问并造成了区域不平等。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Persona_(identity_verification_service)">Persona (identity verification service)</a></li>
<li><a href="https://withpersona.com/">Secure Identity Verification Solutions | Persona</a></li>
<li><a href="https://www.gartner.com/reviews/product/persona">Persona Reviews & Ratings 2026 | Gartner Peer Insights</a></li>

</ul>
</details>

**社区讨论**: 评论中反应不一：一些用户对区域限制和永久封禁表示不满，而另一些人则指出该政策并非新规。关于 Persona 数据使用的隐私担忧被强调，并与网络中立性进行了比较。

**标签**: `#Claude`, `#identity verification`, `#Anthropic`, `#privacy`, `#AI regulation`

---

<a id="item-8"></a>
## [软件销售的最小可行单元](https://brandur.org/minimum-viable-unit) ⭐️ 7.0/10

这一分析挑战了传统的自建与购买决策，表明更低的构建成本支持更多定制方案，但并未消除权衡的必要性，影响开发者、初创企业和大型企业。 作者指出，尽管构建软件比以往更便宜，但打磨副项目的动力和努力常常超过其效用；同时强调社区效应和共享软件的外部性在孤立构建中缺失。

hackernews · brandur · 6月21日 16:41 · [社区讨论](https://news.ycombinator.com/item?id=48620342)

**背景**: 自建与购买是软件工程中的经典决策，即在开发定制软件与购买现有方案之间选择。最小可行单元概念源自精益创业方法论，指能提供价值并可销售的最小软件片段。近期 AI 编程助手的进步显著降低了构建成本和时间，使定制开发更加易得。

**社区讨论**: 评论者普遍认为构建成本仍不为零，且内部构建可能吸引竞争者，缩小可行范围。他们还指出，共享软件中的社区驱动功能提供了定制构建所缺乏的好处。

**标签**: `#software engineering`, `#product development`, `#build vs buy`, `#economics of software`, `#side projects`

---

<a id="item-9"></a>
## [Peter Norvig 的经典 Python 实现 Lisp 解释器教程](https://norvig.com/lispy.html) ⭐️ 7.0/10

Peter Norvig 于 2010 年发布的教程，教授如何用 Python 编写一个 Lisp 解释器，至今仍是学习语言实现的经典入门材料，涵盖了 eval/apply 循环和 S-表达式解析等核心概念。 该教程从头构建完整的解释器，消除了编程语言实现的神秘感，让不具备编译器背景的程序员也能轻松理解，并激励了许多人探索语言实现领域。 解释器核心用不到 100 行 Python 代码实现了一个极简的 Scheme 风格 Lisp 方言。教程分为两部分：第一部分构建基础解释器，第二部分增加宏、延续（continuations）等高级特性。

hackernews · tosh · 6月21日 15:36 · [社区讨论](https://news.ycombinator.com/item?id=48619831)

**背景**: S-表达式（symbolic expression）是一种嵌套列表数据表示法，Lisp 语言用它来表示源代码和数据。eval/apply 循环是 Lisp 解释器的核心：eval 在给定环境中计算表达式的值，apply 处理函数应用。理解这个循环是掌握语言实现的关键。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/S-expression">S-expression - Wikipedia</a></li>
<li><a href="https://github.com/tangledgroup/tangled-skills/blob/main/.agents/skills/scheme-in-python-2026-05-03/reference/02-eval-apply-loop.md">02-eval-apply-loop.md - GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区评论非常积极，用户分享了相关项目：wmedrano 制作了 Rust 版本，chombier 推荐了教程第二部分和《Crafting Interpreters》，leonardool 提到了极简 R4RS REPL 项目 Ribbit，zahlman 则用 S-表达式形式开了个玩笑。

**标签**: `#Lisp`, `#Python`, `#interpreter`, `#programming languages`, `#tutorial`

---

<a id="item-10"></a>
## [几何代数批判引发争议](https://alexkritchevsky.com/2024/02/28/geometric-algebra.html) ⭐️ 7.0/10

该批判挑战了几何代数支持者的主张，可能影响其在物理和工程领域的采纳，其中几何代数被推崇为统一框架。 文章甚至批评了几何代数的关键人物 David Hestenes，并指出其缺乏单位制和量纲分析等问题。该博文在 Hacker News 上获得 116 个点赞和 115 条评论。

hackernews · Hbruz0 · 6月21日 11:06 · [社区讨论](https://news.ycombinator.com/item?id=48617782)

**背景**: 几何代数，又称克利福德代数，通过定义几何积将向量扩展为多重向量，从而推广了向量代数。它被用于物理中描述旋转和电磁场，但其支持者有时会夸大其相对于传统方法的优越性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geometric_algebra">Geometric algebra - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Comparison_of_vector_algebra_and_geometric_algebra">Comparison of vector algebra and geometric algebra - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者意见分歧：有人赞同批评，认为缺乏严谨性；另一些人则从实用角度为 GA 辩护，认为其更直观。也有评论批评文章中存在人身攻击。

**标签**: `#mathematics`, `#geometric algebra`, `#controversy`, `#community discussion`

---

<a id="item-11"></a>
## [AryStinger 僵尸网络感染数千台 D-Link 路由器](https://www.bleepingcomputer.com/news/security/arystinger-botnet-infected-thousands-of-d-link-routers-worldwide/) ⭐️ 7.0/10

安全研究人员发现了一个名为 AryStinger 的此前未知的僵尸网络，它已感染全球超过 4000 台过时的 D-Link 路由器，并将其转化为恶意流量的代理。 该僵尸网络突显了未打补丁的过时路由器带来的持续风险，它们很容易被劫持用于发起网络攻击。数千台设备被入侵强调用户需要更换或保护过时硬件，以防止其网络被武器化。 AryStinger 利用已停产的 D-Link 路由器型号中的已知漏洞，部署轻量级恶意软件载荷，将每台设备纳入代理僵尸网络。该恶意软件利用路由器资源路由恶意流量，使得追踪原始攻击者变得困难。

rss · BleepingComputer · 6月21日 14:14

**背景**: 僵尸网络是由攻击者远程控制的受感染设备组成的网络，常用于发起分布式拒绝服务（DDoS）攻击、发送垃圾邮件或代理恶意流量。路由器是诱人的目标，因为它们常常未打补丁且安全性弱于计算机。AryStinger 专门针对不再受制造商支持的旧款 D-Link 路由器，这意味着它们不会收到安全更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://threat-modeling.com/arystinger-botnet-dlink-routers-june-2026/">AryStinger Botnet Infects Thousands of D-Link Routers Worldwide</a></li>
<li><a href="https://hoploninfosec.com/arystinger-botnet-router-hijacking-attack">AryStinger Botnet Hijacks 4,000+ Routers Worldwide</a></li>

</ul>
</details>

**标签**: `#security`, `#botnet`, `#D-Link`, `#malware`, `#networking`

---