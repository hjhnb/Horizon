---
layout: default
title: "Horizon Summary: 2026-08-18 (ZH)"
date: 2026-08-18
lang: zh
---

> 从 61 条内容中筛选出 20 条重要资讯。

---

1. [DuckDB 发布 v2.0 预览版，带来重大新特性](#item-1)
2. [Qwen3.8-27B 在 Artificial Analysis 上取得 52 分，比肩前沿模型](#item-2)
3. [AirTag 追踪珍本书籍到亚马逊 AI 训练设施](#item-3)
4. [Stripe 以 70 亿美元收购 OpenRouter](#item-4)
5. [Unisoc VoLTE 视频通话漏洞链可获取 Android 内核完全控制权](#item-5)
6. [AI 生成的 Copilot Autofix 在 Snowflake Jira 工作流中引入漏洞](#item-6)
7. [AI;DR：读者对 AI 生成内容表示反感](#item-7)
8. [重排任务顺序让 GPU 集群利用率提升 33 个百分点](#item-8)
9. [严重的 GitLab GraphQL 漏洞可使未认证攻击者删除公开项目](#item-9)
10. [Forminator 漏洞可致未认证远程代码执行](#item-10)
11. [MCP 服务器可通过明文配置与提示注入泄露企业机密](#item-11)
12. [疑似与中国有关联的 APT 利用 VMware vCenter 漏洞部署 Babuk 勒索软件](#item-12)
13. [Qwen 3.8 27B 在 16GB 显存的 llama.cpp 最佳配置：73k 上下文](#item-13)
14. [llama.cpp 的 PR 引入自适应 MTP 深度选择](#item-14)
15. [基准表测的是 bf16，用户跑的是量化版](#item-15)
16. [CISA 将遭活跃利用的 Ray 漏洞加入 KEV 目录](#item-16)
17. [Cavern C2 框架利用 DNS 和 Google Apps Script 实现隐蔽通信](#item-17)
18. [每周安全回顾：VMware 漏洞、Windows 零日漏洞与 MCP 攻击](#item-18)
19. [Evooo1Bot Linux 僵尸网络利用已知漏洞将边缘设备变为 SOCKS5 代理](#item-19)
20. [黑客声称窃取财富 500 强公司 360 万 Azure 账户记录](#item-20)

---

<a id="item-1"></a>
## [DuckDB 发布 v2.0 预览版，带来重大新特性](https://duckdb.org/2026/08/17/duckdb-20-highlights) ⭐️ 9.0/10

DuckDB 发布了 2.0 版本的预览版，这是一个重要的里程碑版本。公告重点介绍了这一嵌入式分析数据库的重大新特性和性能改进。 DuckDB 已成为分析工作负载中广泛使用的工具，v2.0 标志着其持续成熟和性能提升。该预览版在 Hacker News 上获得了 507 分和 90 条评论的社区高度关注，反映了实际应用中的验证与期待。 该预览版于 2026 年 8 月 17 日发布，但具体特性细节尚未完全公开。社区成员提及了即将推出的“Quack”功能，并指出项目在不到六个月内积累了超过 10,000 次提交。

hackernews · ibotty · 8月17日 13:46 · [社区讨论](https://news.ycombinator.com/item?id=49330781)

**背景**: DuckDB 是一个开源的列式关系数据库管理系统，专为分析型（OLAP）工作负载而设计。它以内嵌方式在应用程序内运行，无需在系统之间移动数据，并通过矢量化执行实现对复杂查询的高性能。这些特性使其成为本地分析、Python 数据处理以及消费级硬件上超内存计算的流行选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DuckDB">DuckDB - Wikipedia</a></li>
<li><a href="https://duckdb.org/">DuckDB – An in-process SQL OLAP database management system</a></li>
<li><a href="https://motherduck.com/learn/duckdb-vs-sqlite-databases/">DuckDB vs SQLite: Which Embedded Database Should You Use?</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了强烈的热情，有人将其描述为已在生产环境中采用并在多家公司推荐的工具。有人特别提到使用 DuckDB 处理每秒数千事件的实时分析管道，也有人对高提交速度、AI 辅助开发可能扮演的角色，以及相比 ClickHouse 缺少增量物化视图提出了疑问。

**标签**: `#DuckDB`, `#database`, `#analytics`, `#release`, `#SQL`

---

<a id="item-2"></a>
## [Qwen3.8-27B 在 Artificial Analysis 上取得 52 分，比肩前沿模型](https://artificialanalysis.ai/models/qwen3-8-27b) ⭐️ 9.0/10

阿里巴巴 Qwen 团队于 2026 年 8 月 14 日发布的紧凑型密集 27B 参数模型 Qwen3.8-27B，在 Artificial Analysis 基准测试中取得 52 分，超越所有中等规模模型，并与前沿规模的 MoE 模型 DeepSeek V4 Flash 0731 持平。据报道，它还在游戏 PC 上超越了 Opus 4.6。 这一结果意义重大，因为一个可在消费级硬件上运行的小型密集模型，如今能与规模大得多的前沿模型匹敌甚至超越，这挑战了“只有扩大参数规模才能达到顶级性能”的假设。这可能加速本地和边缘 AI 的应用，并将焦点转向效率和数据质量。 该模型是原生多模态模型，权重在 Hugging Face 和 ModelScope 上开源，发布当天即可在 OpenRouter 上使用。Artificial Analysis 是一个衡量质量、价格、速度和延迟的独立基准；52 分的成绩使其超过 40B–150B 区间内的所有模型，并与 DeepSeek V4 Flash（总参数 284B，激活 13B）持平。

hackernews · anana_ · 8月17日 17:25 · [社区讨论](https://news.ycombinator.com/item?id=49334544)

**背景**: Qwen 是阿里巴巴推出的开源权重大语言模型系列，以相对较小的参数量实现强劲性能而著称。DeepSeek V4 Flash 是 DeepSeek 推出的效率优化的混合专家（MoE）模型，总参数 284B，但仅激活 13B，支持 100 万 token 的上下文。Artificial Analysis 是一个广泛引用的独立排行榜，评估模型在通用任务上的表现，并追踪 API 托管模型的价格和速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-0731">deepseek-ai/DeepSeek-V4-Flash-0731 · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 评论者对一款 27B 模型能击败六个月前发布的 SOTA 模型 Opus 4.6 并与 DeepSeek V4 Flash 持平表示惊讶和难以置信。一些人注意到该模型在代理行为上表现出色，将其与 GPT-5.6-Sol-max 相提并论，另一些人则表示会进行大量测试；整体情绪既兴奋，也带有一丝“规模竞赛可能已经结束”的感慨。

**标签**: `#qwen`, `#llm`, `#benchmarks`, `#efficiency`, `#open-source`

---

<a id="item-3"></a>
## [AirTag 追踪珍本书籍到亚马逊 AI 训练设施](https://simonwillison.net/2026/Aug/17/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-tra/) ⭐️ 9.0/10

404 Media 将一个 AirTag 藏入通过 Biblio 下单的大约 1000 本珍稀书籍中，追踪到位于拉斯维加斯亚马逊 LAS8 设施的 VGT3 区域。工人论坛帖文证实该站点会破坏性地扫描大量书籍。 这提供了具体、物理层面的证据，表明亚马逊正在大规模扫描珍稀书籍用于人工智能训练，证实了外界长期以来对匿名批量购书的怀疑。它促使版权与数据来源方面的担忧进一步加剧，并让大型科技公司的训练数据行为面临更严格审视。 这本书被送到拉斯维加斯东北部亚马逊 LAS8 设施的 VGT3 区域，该入口处有恐龙与书的标志。亚马逊员工的在线讨论表明 VGT3 会进行破坏性的大量书籍扫描。

rss · Simon Willison · 8月17日 15:21

**背景**: Biblio 是独立运营的国际在线市场，专门销售珍本和收藏书籍，成立于 2003 年。近年来，书商多次报告有对价格不敏感的匿名客户大批量购书，外界普遍怀疑这些客户是寻求扫描素材的人工智能公司；例如，Anthropic 在 2025 年 6 月也曾受到类似指控。此次调查通过直接追踪而非推测，确认了其中一位买家。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Biblio.com">Biblio .com - Wikipedia</a></li>
<li><a href="http://bibliofiend.com/about-biblio.html">About Biblio Booksearch and Marketplace</a></li>

</ul>
</details>

**标签**: `#AI training data`, `#Amazon`, `#book scanning`, `#investigation`, `#copyright`

---

<a id="item-4"></a>
## [Stripe 以 70 亿美元收购 OpenRouter](https://www.latent.space/p/ainews-stripe-buys-openrouter-for) ⭐️ 9.0/10

Stripe 以 70 亿美元收购了统一 AI 模型网关 OpenRouter。这一交易凸显了 AI 基础设施和变现日益增长的战略价值。 此次收购表明支付与基础设施正在 AI 经济中融合，使 Stripe 得以控制开发者访问和付费使用 AI 模型的方式。这可能重塑 AI 分发渠道，并影响依赖 OpenRouter 路由服务的开发者。 OpenRouter 通过单一 API 和密钥即可访问来自 Anthropic、Google、Meta、Mistral 等提供商的数百种模型。该平台在原型设计和基准测试中广受欢迎，但生产用户通常还需要额外的治理、可观测性和安全功能。

rss · Latent Space · 8月17日 23:13

**背景**: OpenRouter 是一个 AI 模型网关，属于一类基础设施，通过提供统一 API 来简化对多个大语言模型的访问。这类网关让开发者能够根据价格、质量或性能将请求路由到不同模型，而无需重写代码。Stripe 是一家大型在线支付处理商，其收购 OpenRouter 表明它希望成为 AI 使用的支付层，即开发者按 API 调用付费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai-sdk.dev/providers/community-providers/openrouter">Community Providers: OpenRouter</a></li>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://www.truefoundry.com/blog/openrouter-vs-ai-gateway">OpenRouter Vs AI Gateway: Differences, Use Cases & Best Choice</a></li>

</ul>
</details>

**标签**: `#AI`, `#Acquisition`, `#OpenRouter`, `#Stripe`, `#Infrastructure`

---

<a id="item-5"></a>
## [Unisoc VoLTE 视频通话漏洞链可获取 Android 内核完全控制权](https://thehackernews.com/2026/08/unisoc-volte-video-call-exploit-chain.html) ⭐️ 9.0/10

SSD Secure Disclosure 的安全研究人员公布了一个两阶段漏洞利用链，可通过 VoLTE 视频通话在搭载 Unisoc 芯片的设备上获得完整的 Android 内核访问权限。第二阶段公告于 2026 年 8 月 17 日发布，Unisoc 尚未提供补丁。 这是一个严重且未修补的远程漏洞利用链，影响广泛使用的调制解调器供应商，可能使数百万 Android 设备面临完全被攻破的风险。由于厂商未提供修复，用户除了网络层或设备层缓解措施外几乎没有其他防护手段。 该漏洞链由 2026 年 3 月披露的初始远程代码执行和本阶段针对 Android 内核的权限提升组成，两者均位于 Unisoc 调制解调器固件中。漏洞通过 VoLTE 视频通话触发，因此是一种潜在的远程、无需用户交互的攻击向量。

rss · The Hacker News · 8月17日 10:52

**背景**: VoLTE（LTE 语音）允许通过 4G LTE 网络进行语音和视频通话，由调制解调器固件而非主应用处理器处理。Unisoc（原 Spreadtrum）是低端和中端 Android 手机的主要芯片组供应商，其调制解调器固件部署广泛。利用对基带具有特权访问权限的调制解调器，攻击者可升级至 Android 内核并完全控制设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/unisoc-volte-video-call-exploit-chain.html">Unisoc VoLTE Video Call Exploit Chain Can Give Attackers Full ...</a></li>
<li><a href="https://www.hkcsl.com/en/volte/">VoLTE Voice Call Service | csl</a></li>

</ul>
</details>

**标签**: `#android`, `#security`, `#unisoc`, `#exploit`, `#kernel`

---

<a id="item-6"></a>
## [AI 生成的 Copilot Autofix 在 Snowflake Jira 工作流中引入漏洞](https://www.wiz.io/blog/red-agent-snowflake-copilot-cicd-bug) ⭐️ 8.0/10

Wiz 研究人员披露了 Snowflake 公开的 snowflake-connector-net 仓库中存在一个 GitHub Actions 工作流注入漏洞。该漏洞由 AI 生成的 GitHub Copilot“autofix”建议引入，攻击者可能通过精心构造的 pull request 利用它攻陷 Snowflake 的 Jira 工作流。 这是一个 AI 建议代码在实际开发工作流中引入安全漏洞的真实案例。它表明 AI 代码助手可能降低引入不安全变更的成本，而代码验证仍然是开发者和安全团队面临的关键瓶颈。 该漏洞是 YAML 格式的 jira_issue.yml 工作流中的模板注入问题，用户可控的 PR 标题或正文被拼接进 run 命令中。Copilot Autofix 曾尝试转义特殊字符但未成功，而 zizmor 等静态分析工具可以用“code injection via template expansion”等错误标记此类问题。

hackernews · galnagli · 8月17日 14:18 · [社区讨论](https://news.ycombinator.com/item?id=49331423)

**背景**: GitHub Copilot Autofix 是 GitHub code scanning 的扩展功能，它会针对代码扫描警报自动提供修复建议，帮助开发者更快修复漏洞。模板注入是指未经过滤的用户输入被模板引擎或脚本引擎当作代码执行；在 GitHub Actions 中，恶意 PR 可以利用这一点向 CI 工作流注入命令。这段背景说明了看似有帮助的 AI 生成修复也可能制造危险的注入点，如果建议没有经过仔细审查的话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/code-security/concepts/code-scanning/copilot-autofix-for-code-scanning">About Copilot Autofix for code scanning - GitHub Docs</a></li>
<li><a href="https://portswigger.net/web-security/server-side-template-injection">Server-side template injection | Web Security Academy</a></li>
<li><a href="https://github.blog/news-insights/product-news/secure-code-more-than-three-times-faster-with-copilot-autofix/">Found means fixed: Secure code more than three times faster with Copilot Autofix - The GitHub Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者强调应对 AI 生成的代码进行静态分析，并指出用 zizmor 可以发现 GitHub Actions 中的模板注入。还有人指出，AI 让代码变更的成本降低，但审查成本并未同步下降，因此验证成为新的瓶颈；一位开发者表示自己很可能也会犯同样错误，也有人质疑所提及的 PR 是否真的包含有漏洞的 autofix。

**标签**: `#AI security`, `#GitHub Copilot`, `#CI/CD`, `#vulnerability`, `#Snowflake`

---

<a id="item-7"></a>
## [AI;DR：读者对 AI 生成内容表示反感](https://www.rickmanelius.com/p/aidr-ai-didnt-read) ⭐️ 8.0/10

这篇文章及其评论区（324 条评论）反映了一股日益强烈的对 AI 生成回复、文档和教程的抵制情绪。用户越来越倾向于跳过或无视那些被认为是懒惰、冗长或不真实的 AI 文本。 这标志着一个文化转折点：一度被视为惊艳的 AI 生成内容，如今在在线和工作场所沟通中常被视为噪音。它影响着从电子邮件到代码注释等一切内容的信任度、可读性和真实感。 评论者举出了具体的职场痛点，例如每个拉取请求中都有数百行 AI 生成的文档，以及关于代码的表演式评论。也有人认为真正的问题不在于作者是 AI，而在于质量低下；只要信息量足够，写得好的 AI 内容也可以接受。

hackernews · mooreds · 8月17日 19:47 · [社区讨论](https://news.ycombinator.com/item?id=49336573)

**背景**: AI;DR 是对网络缩略语 TL;DR（太长不读）的仿写，表达了读者不想再花时间阅读 AI 生成的填充内容。许多人在网上阅读是为了学习或被说服，他们期待的是人的声音和真正的洞见。在职场中，AI 输出的泛滥造就了“后可读性时代”的代码库，文档带来的更多是噪音而非清晰度。

**社区讨论**: 总体情绪强烈负面：人们认为用 AI 生成的回复来回应他人是一种冒犯，也是智力懒惰的表现，并抱怨其冗长、术语堆砌、过度自信和缺乏细微差别。一个显著的反驳观点是，质量才是真正的标准——只要能帮到人，AI 写的教程也应当受欢迎。

**标签**: `#AI`, `#AI-generated content`, `#Online communication`, `#Tech culture`, `#Commentary`

---

<a id="item-8"></a>
## [重排任务顺序让 GPU 集群利用率提升 33 个百分点](https://huggingface.co/blog/Dharma-AI/gpu-management-pt2) ⭐️ 8.0/10

这篇博客文章展示了在同一个 GPU 集群上，仅通过改变作业的调度顺序，就能让集群利用率在不增加任何硬件的情况下提升 33 个百分点。Dharma-AI 的作者在 Hugging Face 博客上分享了这一基于数据的调度经验。 在多租户 GPU 集群中，算力利用率直接决定成本效率，因此重排作业顺序是一种低成本、可立即落地的优化方式。这有助于减少 GPU 空转、提升 AI 训练和推理负载的整体吞吐，而无需扩充基础设施。 其核心思想是利用回填（backfill）调度，将短作业填入大型联合调度（gang scheduling）作业留下的资源空隙，从而降低集群碎片化。文章强调，在集群和硬件完全不变的前提下，仅优化排队顺序就能带来 33 个百分点的利用率提升。

rss · Hugging Face Blog · 8月17日 19:46

**背景**: GPU 集群通常由多个团队共同使用，而大型分布式训练作业往往采用联合调度（gang scheduling），即所有请求的 GPU 必须同时分配到位。这种“全有或全无”的方式会在集群中留下难以利用的小块空隙。回填（backfill）调度允许短作业在这些空隙中运行，只要它们能在预定的大作业开始前完成。文章中归因于利用率提升的正是这种通过重排作业顺序来给回填创造更多机会的策略变更。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.abhik.ai/concepts/gpu-computing/slurm-backfill">Slurm Backfill Scheduling : How Small Jobs Fill the Gaps | Abhik Sarkar</a></li>
<li><a href="https://www.sigarch.org/the-different-facets-of-large-scale-gpu-cluster-scheduling-for-ml-jobs/">The Different Facets of Large-Scale GPU Cluster Scheduling for ML Jobs | SIGARCH</a></li>
<li><a href="https://arxiv.org/html/2407.13088v1">Scheduling Deep Learning Jobs in Multi-Tenant GPU Clusters via Wise Resource Sharing</a></li>

</ul>
</details>

**标签**: `#GPU`, `#scheduling`, `#cluster utilization`, `#ML infrastructure`

---

<a id="item-9"></a>
## [严重的 GitLab GraphQL 漏洞可使未认证攻击者删除公开项目](https://thehackernews.com/2026/08/critical-gitlab-graphql-flaw-could-let.html) ⭐️ 8.0/10

GitLab 发布了针对 CVE-2026-19478 的安全更新，这是一个 CVSS 评分为 9.4 的严重 GraphQL 漏洞。该漏洞可能允许未认证攻击者修改或删除 GitLab CE 和 EE 中的公开项目与用户数据。 该漏洞非常关键，因为 GitLab 广泛用于源代码管理和 DevOps，未认证攻击可能导致大规模数据丢失或项目被篡改。运行受影响版本的组织应立即修补以防被利用。 该漏洞在某些条件下影响社区版（CE）和企业版（EE）。GitLab 给予 9.4 的 CVSS 评分，反映出其严重性高且无需认证即可利用。

rss · The Hacker News · 8月17日 21:03

**背景**: GraphQL 是一种开源的 API 查询语言，允许客户端精确请求所需的数据。通用漏洞评分系统（CVSS）是一个标准化的框架，用于按 0 到 10 分评估漏洞的严重程度。GitLab CE 和 EE 是流行的自托管及云端 DevOps 平台，会暴露 GraphQL API，因此该接口中的漏洞可能产生广泛影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GraphQL">GraphQL</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System">Common Vulnerability Scoring System - Wikipedia</a></li>
<li><a href="https://graphql.org/">GraphQL | The query language for modern APIs</a></li>

</ul>
</details>

**标签**: `#security`, `#GitLab`, `#CVE`, `#vulnerability`

---

<a id="item-10"></a>
## [Forminator 漏洞可致未认证远程代码执行](https://thehackernews.com/2026/08/forminator-wordpress-flaw-can-enable.html) ⭐️ 8.0/10

Forminator WordPress 插件中被披露了一个严重漏洞（CVE-2026-15748），未认证攻击者可通过上传恶意 PHP 文件执行任意代码。该漏洞的 CVSS 评分为 9.8，影响超过 60 万个活跃安装。 Forminator 是最受欢迎的 WordPress 表单构建插件之一，其庞大的安装量使得该漏洞成为高风险目标。未认证的远程代码执行可让攻击者完全控制网站，对依赖 WordPress 进行电子商务或客户数据处理的企业尤其危险。 CVE-2026-15748 的技术细节尚未完全公开，CVE 条目目前仍为保留状态，因此管理员应在补丁发布后立即更新插件。安全专家建议除了应用官方补丁之外，还应加固上传目录并启用运行时文件完整性监控。

rss · The Hacker News · 8月17日 18:22

**背景**: Forminator Forms 是一款免费的 WordPress 插件，允许用户通过拖拽方式创建联系表单、支付表单、测验和投票。远程代码执行（RCE）意味着攻击者可以在服务器上运行任意命令，从而获得对网站及其数据的完全控制。WordPress 插件漏洞是网站被入侵的常见入口，其中文件上传类漏洞尤其容易被武器化，因为攻击者可以直接投放 Web 木马。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wordpress.org/plugins/forminator/">Forminator Forms – Contact Form, Payment Form... | WordPress .org</a></li>
<li><a href="https://feedly.com/cve/CVE-2026-15748">CVE-2026-15748 - Exploits & Severity - Feedly</a></li>
<li><a href="https://vulners.com/cve/CVE-2026-15748">CVE-2026-15748 - vulnerability database | Vulners.com</a></li>

</ul>
</details>

**标签**: `#security`, `#wordpress`, `#rce`, `#vulnerability`, `#cve`

---

<a id="item-11"></a>
## [MCP 服务器可通过明文配置与提示注入泄露企业机密](https://thehackernews.com/2026/08/how-mcp-servers-can-expose-enterprise.html) ⭐️ 8.0/10

黑客新闻（The Hacker News）报道称，Model Context Protocol (MCP) 服务器可能通过明文配置文件、过度授权访问和提示注入泄露企业机密，而且往往在安全团队得知服务器运行之前就已发生。随着 AI 智能体被越来越多地采用，这将在基于 MCP 的集成中造成一种隐蔽的安全缺口。 这一问题的严重性在于，MCP 是 Anthropic、OpenAI、Google DeepMind 等主要 AI 厂商采用的开源标准，已成为企业 AI 基础设施的关键组成部分。隐蔽的机密泄露风险可能削弱人们对 AI 智能体的信任，并在安全团队做出反应前就引发数据泄露。 泄露途径包括：MCP 服务器以明文存储凭证或 API 密钥、被授予对企业系统过宽的权限，以及容易受到通过外部内容实施的间接提示注入攻击。报告强调，这些风险往往被忽视，因为 MCP 服务器可能在未经适当安全审查的情况下就被部署上线。

rss · The Hacker News · 8月17日 11:58

**背景**: Model Context Protocol (MCP) 由 Anthropic 于 2024 年 11 月发布，是一个开放标准，旨在规范大型语言模型等 AI 系统与外部工具、数据源和 API 的集成方式。提示注入是一种已知的 AI 漏洞：攻击者将恶意指令隐藏在电子邮件或文档等外部数据中，诱使 AI 执行非预期的命令。许多企业正在采用依赖 MCP 访问内部系统的 AI 智能体，这扩大了此类泄露的攻击面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>

</ul>
</details>

**标签**: `#security`, `#MCP`, `#AI agents`, `#enterprise`, `#secrets`

---

<a id="item-12"></a>
## [疑似与中国有关联的 APT 利用 VMware vCenter 漏洞部署 Babuk 勒索软件](https://thehackernews.com/2026/08/suspected-china-nexus-actor-exploits.html) ⭐️ 8.0/10

研究人员报告称，一个疑似与中国有关联的高级持续性威胁(APT)正在积极利用 CVE-2026-59310——Broadcom VMware vCenter 中的一个严重目录遍历漏洞——来部署 Babuk 变种勒索软件。该漏洞的 CVSS 评分为 9.8，可允许攻击者执行任意代码。 这一事件意义重大，因为 VMware vCenter 在企业虚拟化环境中广泛部署，一个被积极利用的严重漏洞会给许多组织带来直接的勒索软件威胁。它也凸显了修补 CVE-2026-59310 的紧迫性，以及 APT 组织利用漏洞发起勒索软件攻击这一日益增长的趋势。 该漏洞是 VMware vCenter 的 Syslog 服务器组件中的一个路径遍历缺陷(CWE-22)，允许具备网络访问权限的攻击者遍历目录并可能执行代码。Shadowserver 报告指出，攻击者已在所有已识别受害者的系统上部署了 reverse_ssh 持久化机制，这些系统应被视为完全失陷；此外，Babuk 泄露的源代码此前已催生了 Play 和 RTM Locker 等变种。

rss · The Hacker News · 8月17日 07:36

**背景**: VMware vCenter 是用于虚拟化基础设施的集中管理平台，因此是高价值攻击目标。目录遍历漏洞允许攻击者访问预期根目录之外受限制的目录，通常可导致代码执行。Babuk 是一个勒索软件家族，其源代码于 2021 年泄露，催生了许多衍生变种；疑似与中国有关联的 APT 是指受国家支持或与国家一致的团体，它们从事网络间谍活动，并越来越多地参与勒索软件行动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2026-59310">NVD - CVE-2026-59310</a></li>
<li><a href="https://www.shadowserver.org/what-we-do/network-reporting/vmware-vcenter-cve-2026-59310-exploitation-victim-special-report/">CRITICAL: VMware vCenter CVE-2026-59310 Exploitation Victim ...</a></li>
<li><a href="https://www.sentinelone.com/anthology/babuk/">Babuk Ransomware: In-Depth Analysis, Detection, Mitigation ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#APT`, `#VMware`, `#ransomware`, `#CVE`

---

<a id="item-13"></a>
## [Qwen 3.8 27B 在 16GB 显存的 llama.cpp 最佳配置：73k 上下文](https://www.reddit.com/r/LocalLLaMA/comments/1vqrt86/after_pushing_1m_tokens_through_qwen_38_27b_here/) ⭐️ 8.0/10

一位用户分享了在 16GB 显存 RTX 5060 Ti 上运行 Qwen3.8-27B GGUF 模型的完整 llama.cpp 配置，通过 KV 缓存量化和原生 MTP 推测解码实现了 73,728 token 的上下文窗口。他们还用仅三条提示词、超过一百万 token 自主构建了一个旧版 vBulletin 论坛的 REST API 和 MCP 服务器，验证了该配置。 这表明 27B 参数的大模型配合长上下文也能在消费级 16GB 显卡上流畅运行，让高级智能体编码工作流对爱好者和小团队更易用。这份经过实际测试的详细配置（包含 MTP 和分层 KV 缓存量化）为本地 LLM 社区提供了实用参考。 该配置使用 Qwen3.8-27B-UD-Q3_K_XL.gguf，开启 flash-attn、fit=on，上下文大小为 73,728。主上下文的 KV 缓存量化为 q4_1，MTP 草稿上下文为 q5_1，推测解码设置为 spec-type=draft-mtp、n-max=2；采样参数为 temp=0.4、top_p=0.90、top_k=15、min_p=0.02。

reddit · r/LocalLLaMA · /u/chiribe · 8月17日 13:05

**背景**: llama.cpp 是一个流行的 C/C++ 推理引擎，可以在本地硬件上运行量化后的 LLM。GGUF 是量化后的模型文件；Q3_K_XL 是一种量化级别，在压缩其余权重的同时将输出和嵌入权重保留为 Q8_0。推测解码（通过多词元预测（MTP）草稿模块）并行生成草稿词元并验证，从而加速生成；KV 缓存量化则压缩缓存的注意力键值对，以便在有限显存内塞进更长上下文或更大模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ggml-org/llama.cpp/blob/master/docs/speculative.md">llama.cpp/docs/speculative.md at master · ggml-org/llama.cpp</a></li>
<li><a href="https://kingy.ai/blog/qwen3-8-27b-best-quantization-gguf/">Best Qwen3.8-27B GGUF : Q2, Q 3 , Q4, Q5, Q6 and Q8</a></li>
<li><a href="https://modelpiper.com/blog/ollama-kv-cache-quantization/">Ollama KV Cache Quantization : Fit Longer Contexts ... — ModelPiper</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#Qwen`, `#LLM inference`, `#agentic coding`, `#VRAM optimization`

---

<a id="item-14"></a>
## [llama.cpp 的 PR 引入自适应 MTP 深度选择](https://www.reddit.com/r/LocalLLaMA/comments/1vqzud4/llamacpp_adaptive_mtp_pr27210/) ⭐️ 8.0/10

llama.cpp 的一个新 pull request（#27210）引入了一种自适应多 token 预测（MTP）模式，通过一个计数型状态机动态调整 MTP 深度，免去了手动调参的需要。与固定 MTP=3 相比，处理密集散文时速度约慢 3%，但在代码生成上快 10-15%，在回忆较早代码时快超过 50%。 这简化了 llama.cpp 用户的配置，同时显著提升了代码生成和记忆回放等常见真实场景的性能。它可能推动推测解码在本地大模型推理中的更广泛应用，并降低用户的调参维护负担。 推荐配置为 --spec-type draft-mtp-adaptive --spec-draft-n-max 12，深度范围从 3 到 12；可以通过 --spec-draft-n-min-adaptive 设置更低的下限。在较高温度下收益会缩小，但代码生成通常仍会略有好转。

reddit · r/LocalLLaMA · /u/Look_0ver_There · 8月17日 18:05

**背景**: 多 token 预测（MTP）允许模型从同一位置预测多个未来 token，而不仅仅是下一个 token，从而可以提高推理速度。推测解码通过使用一个草稿模型提出 token，并用一个更大的目标模型并行验证它们来加速生成，同时不降低输出质量。llama.cpp 是一个广泛使用的开源 C/C++ 推理引擎，一直在添加如 MTP 等各类推测解码特性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-token-prediction-mtp">Multi - Token Prediction ( MTP )</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency ...</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#MTP`, `#speculative decoding`, `#inference optimization`, `#LLM`

---

<a id="item-15"></a>
## [基准表测的是 bf16，用户跑的是量化版](https://www.reddit.com/r/LocalLLaMA/comments/1vr643w/we_benchmark_models_nobody_actually_runs/) ⭐️ 8.0/10

r/LocalLLaMA 上的一则帖子指出，热门 LLM 基准表公布的是 bf16 权重下的分数，而多数本地用户实际运行的是 Q4_K_M 等量化版本，因此被测试的模型与被下载的模型并非同一产物。帖子呼吁在同一个评测框架下，对同一模型在 bf16 与多种量化精度之间做系统性扫描，并附带误差棒。 这很重要，因为本地 LLM 用户依赖基准表来选模型；如果分数只反映 bf16 性能，排名可能无法预测量化模型的实际表现。系统性的量化基准测试能帮助用户回答实际问题，比如在相同显存下，量化的 27B 模型是否优于更小的高精度模型。 帖子具体要求是“同一模型、同一评测工具”，在 bf16、Q8、Q6_K、Q5_K_M、Q4_K_M 和 IQ4_XS 之间扫描，并给出误差棒。帖子还指出，困惑度（perplexity）可能几乎保持不变，但长上下文召回、多步数学推理或严格的工具调用 JSON 等特定能力会悄然退化。

reddit · r/LocalLLaMA · /u/AuspiciousApple · 8月17日 21:53

**背景**: LLM 权重通常以 bf16（bfloat16）等高精度格式发布；bf16 是一种专为深度学习设计的 16 位格式，保留了 float32 的动态范围。为了在消费级硬件上运行大模型，llama.cpp 等工具会把权重转换为 Q4_K_M、IQ4_XS 等量化 GGUF 格式，以降低内存占用，但会损失一定精度。困惑度（perplexity）是常见的内部评估指标，但它对能力下降可能不敏感，因此针对量化模型做任务级评测非常重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bfloat16_floating-point_format">bfloat16 floating-point format - Wikipedia</a></li>
<li><a href="https://tonisagrista.com/blog/2026/quantization/">GGUF quantization guide</a></li>
<li><a href="https://arxiv.org/html/2410.23771v5">What is Wrong with Perplexity for Long-context Language Modeling?</a></li>

</ul>
</details>

**标签**: `#LLM`, `#quantization`, `#benchmarking`, `#LocalLLaMA`

---

<a id="item-16"></a>
## [CISA 将遭活跃利用的 Ray 漏洞加入 KEV 目录](https://www.cisa.gov/news-events/alerts/2026/08/17/cisa-adds-one-known-exploited-vulnerability-catalog) ⭐️ 7.0/10

2026 年 8 月 17 日，CISA 将 CVE-2025-62593（Ray-Project Ray 中的代码注入漏洞）加入已知被利用漏洞（KEV）目录，依据是存在活跃利用的证据。该添加要求联邦民事行政分支机构根据约束性操作指令 26-04 优先修复。 Ray 是广泛使用的开源 AI/ML 计算引擎，因此其中被活跃利用的代码注入漏洞会给运行分布式机器学习工作负载的组织带来重大风险。将其加入 KEV 目录标志着联邦机构需紧急修补，并鼓励所有组织采用基于风险的漏洞管理。 CVE-2025-62593 是一个代码注入漏洞，攻击者利用后可能完全控制受影响的资产。根据 BOD 26-04 实施指南，CISA 鼓励组织在应用补丁前检查受损迹象。

rss · CISA Cybersecurity Advisories · 8月17日 12:00

**背景**: 已知被利用漏洞（KEV）目录是 CISA 发布的权威清单，列出经确认已在真实攻击中被利用的安全漏洞。约束性操作指令 26-04 于 2026 年 6 月发布，要求联邦民事机构优先快速修复目录中列出的高风险漏洞，尤其是那些位于公开暴露资产上、利用后可完全控制的漏洞。Ray 是一个开源框架，用于跨分布式集群扩展 AI 和 Python 工作负载，使其成为 AI/ML 环境中攻击者的高价值目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ray-project/ray">GitHub - ray-project/ray: Ray is an AI compute engine. Ray ...</a></li>
<li><a href="https://content.govdelivery.com/accounts/USDHSCISA/bulletins/41b445a">CISA Releases Binding Operational Directive 26-04 on ...</a></li>
<li><a href="https://cvefeed.io/cisakev/cisa-known-exploited-vulnerability-catalog">CISA Known Exploited Vulnerabilities (KEV) – CVEFeed Catalog</a></li>

</ul>
</details>

**标签**: `#CISA`, `#KEV`, `#vulnerability`, `#Ray`, `#security`

---

<a id="item-17"></a>
## [Cavern C2 框架利用 DNS 和 Google Apps Script 实现隐蔽通信](https://thehackernews.com/2026/08/cavern-c2-uses-dns-and-google-apps.html) ⭐️ 7.0/10

卡巴斯基研究人员发现了与伊朗有关的 Cavern（Cav3rn）命令与控制框架的新组件，这些组件利用 DNS A 记录查询和 Google Apps Script 中继来融入合法流量。新的 C2 模块在轮询命令前，会根据 DNS 响应在直接 HTTPS 和 Google Apps Script 中继之间进行选择。 这一演变表明，国家级威胁行为者越来越多地滥用云服务和 DNS 进行更隐蔽的命令与控制，增加了防御者的检测难度。监控伊朗网络行动的安全团队需要更新指标和检测规则，以应对这些融入正常流量的 C2 信道。 Cavern 框架是一个基于.NET 的模块化 C2 系统，被编译为多种二进制格式，包括.NET Framework、混合模式 C++/CLI 和.NET 8 NativeAOT。新发现的中继模块在每次命令轮询前执行 DNS A 记录查询，然后选择直接 HTTPS 或 Google Apps Script 中继进行通信。

rss · The Hacker News · 8月17日 17:41

**背景**: 命令与控制（C2）框架是黑客用来维持对受感染系统的持久访问并下达指令的工具。伊朗国家支持的黑客组织一直有攻击以色列实体的历史，而 Cavern 是一个被归因于这些行动的模块化后渗透框架。使用 DNS 和 Google Apps Script 能让恶意流量看起来像正常的互联网活动，因为 Google 服务在企业环境中通常被列入白名单。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://securityonline.info/project-cav3rn-framework-analysis/">Project CAV3RN Framework Adds DNS and Google Relays</a></li>
<li><a href="https://research.checkpoint.com/2026/cavern-manticore-exposing-iran-linked-modular-c2-framework/">Cavern Manticore: Exposing Iran-Linked Modular C 2 Framework ...</a></li>
<li><a href="https://thehackernews.com/2026/07/iran-linked-hackers-use-new-cavern-c2.html">Iran-Linked Hackers Use New Cavern C 2 Framework to Target Israeli...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#threat intelligence`, `#command-and-control`, `#malware`, `#evasion`

---

<a id="item-18"></a>
## [每周安全回顾：VMware 漏洞、Windows 零日漏洞与 MCP 攻击](https://thehackernews.com/2026/08/weekly-recap-vmware-exploits-windows-0.html) ⭐️ 7.0/10

本周安全回顾重点介绍了 VMware 漏洞、Windows 零日漏洞、MCP 相关攻击和浏览器会话劫持的活跃利用。一个反复出现的主题是，许多攻击利用的是已有的访问权限和被忽视的防御，而非高超的技巧。 这些事件表明，攻击者无需高级漏洞利用即可造成高影响破坏，因此补丁管理和访问控制等基础卫生措施至关重要。安全团队应将暴露的服务和受信任的会话视为主要目标，尤其是 MCP 等 AI 代理协议引入了新的攻击面。 受影响领域包括暴露的服务、旧漏洞的新利用、浏览器会话作为攻击路径，以及供应链传播超出初始入侵范围。对于 MCP，研究人员已确定工具投毒和间接提示注入是 AI 代理集成中的重大风险。

rss · The Hacker News · 8月17日 13:23

**背景**: VMware 是领先的虚拟化平台，其漏洞可能让攻击者逃逸虚拟机或破坏宿主机。零日漏洞是指在供应商发布补丁之前就被利用的软件缺陷。MCP（Model Context Protocol）是一种让 AI 代理连接工具和数据的开放协议；其服务器元数据可能被投毒以操纵代理行为。浏览器劫持通常指窃取会话 Cookie 以接管已认证的用户会话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://invariantlabs.ai/blog/mcp-security-notification-tool-poisoning-attacks">MCP Security Notification: Tool Poisoning Attacks</a></li>
<li><a href="https://developer.microsoft.com/blog/protecting-against-indirect-injection-attacks-mcp/">Protecting against indirect prompt injection attacks in MCP - Microsoft ...</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/cybersecurity/mcp-security/">Model Context Protocol (MCP) Security: Complete Guide</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerabilities`, `#zero-day`, `#exploits`, `#weekly recap`

---

<a id="item-19"></a>
## [Evooo1Bot Linux 僵尸网络利用已知漏洞将边缘设备变为 SOCKS5 代理](https://thehackernews.com/2026/08/evooo1bot-linux-botnet-exploits-known.html) ⭐️ 7.0/10

安全研究人员发现了一个新的 Linux 僵尸网络家族 Evooo1Bot，它复用了已泄露的 Mirai 源代码中的 DDoS 引擎。该恶意软件利用面向互联网的边缘设备中的已知漏洞，将其变为 SOCKS5 代理。 Evooo1Bot 将 Mirai 衍生恶意软件的威胁从 DDoS 扩展到了代理网络：被攻陷的路由器、摄像头等边缘设备会被用作隐蔽代理，帮助攻击者匿名转发流量。这也凸显出维护不善的 IoT 和边缘设备中已知漏洞仍在助长严重的网络滥用。 该僵尸网络继承了 Mirai 的 DDoS 功能，并新增了将被攻陷设备变为 SOCKS 代理的能力，不再只是纯粹的流量攻击。该恶意软件主要针对路由器、摄像头等面向互联网的 Linux 设备；作为一个新被记录的家族，它表明 Mirai 源代码衍生品仍在持续演化。

rss · The Hacker News · 8月17日 09:29

**背景**: Mirai 是 2016 年首次出现的臭名昭著的僵尸网络，其源代码后来被公开，任何人都能制作变种。它主要针对 IP 摄像头、家用路由器等采用 Linux 的物联网设备，并曾被用于史上最大规模的分布式拒绝服务（DDoS）攻击。SOCKS 是一种通过代理服务器转发 TCP 和 UDP 流量的互联网协议；SOCKS5 增加了可选认证，并允许客户端在不暴露真实 IP 的情况下连接任意目标，因此被攻陷的端点对于匿名化恶意流量极具价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mirai_botnet">Mirai botnet</a></li>
<li><a href="https://en.wikipedia.org/wiki/SOCKS_(proxy)">SOCKS (proxy)</a></li>
<li><a href="https://www.usenix.org/conference/usenixsecurity17/technical-sessions/presentation/antonakakis?trk=article-ssr-frontend-pulse_little-text-block">Understanding the Mirai Botnet | USENIX</a></li>

</ul>
</details>

**标签**: `#botnet`, `#cybersecurity`, `#Mirai`, `#Linux malware`, `#SOCKS5 proxy`

---

<a id="item-20"></a>
## [黑客声称窃取财富 500 强公司 360 万 Azure 账户记录](https://www.bleepingcomputer.com/news/security/hacker-claims-36-million-azure-account-records-stolen-from-major-companies/) ⭐️ 7.0/10

一名威胁行为者声称已窃取多家财富 500 强公司员工的 360 万条 Microsoft Azure 账户记录，并正在网上出售这些数据。据称此次入侵利用了泄露的凭据来获得对公司 Azure 基础设施的访问权限。 若该说法得到证实，这将成为影响全球最大企业的一起重大云安全事件，可能泄露敏感的员工信息。这一声明凸显了基于凭据的攻击对云基础设施构成的持续风险，尤其是在各组织加速采用 Azure 等平台的情况下。 据称这些数据包括来自 Microsoft Azure 基础设施的账户记录，但该说法尚未得到证实，也缺乏技术证据。据报道，威胁行为者利用泄露的凭据获得了访问权限，这些凭据通常来自钓鱼攻击、密码重用或第三方泄露。

rss · BleepingComputer · 8月17日 19:35

**背景**: Microsoft Azure 是一个云计算平台，提供虚拟机、数据库和身份管理等服务，被企业广泛使用。涉及云账户的数据泄露可能导致身份盗窃、企业间谍活动或进一步攻击，因为员工凭据通常是进入内部系统的门户。安全研究人员经常警告，撞库和钓鱼仍然是攻击者渗透云环境的最常见方式。如果这一事件得到证实，将再次表明配置不当或保护薄弱的账户如何可能削弱即使是大型组织的安全。

**标签**: `#security`, `#Azure`, `#data breach`, `#cloud`, `#hacking`

---