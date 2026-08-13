---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> 从 70 条内容中筛选出 20 条重要资讯。

---

1. [DeepSeek 发布新一代旗舰模型 V4 Pro 0813](#item-1)
2. [Qwen 发布大型 MoE 模型，宣称性能接近顶尖](#item-2)
3. [Lazarus 利用 Windows 零日漏洞获取 SYSTEM 权限并部署后门](#item-3)
4. [攻击者利用 VMware vCenter 漏洞实现持久远程访问](#item-4)
5. [ShieldBreak 零日 PoC 绕过微软 Defender 补丁获取 SYSTEM 权限](#item-5)
6. [Tailscale 将数据库损坏追溯至一个存在 16 年的 SQLite WAL 重置 Bug](#item-6)
7. [WebSocket 传输 HTML：几乎不用 JavaScript 的实时 SPA](#item-7)
8. [xAI 发布 Grok 4.6，前沿模型定价激进](#item-8)
9. [Chrome 的部分 JPEG 解码导致小尺寸图片渲染不同](#item-9)
10. [车牌读取器搜索应需搜查令](#item-10)
11. [高尔斯：LLM 擅长数学靠采样而非刻意推理](#item-11)
12. [Woxi：开源 Rust 实现的 Wolfram 语言解释器](#item-12)
13. [NVIDIA 详解在 GB300 NVL72 上部署 Qwen3.8-2.4T-A95B](#item-13)
14. [737 个恶意 Chrome VPN 扩展被曝劫持浏览器流量](#item-14)
15. [API 漏洞使较弱 AI 模型可解码顶级 LLM 的加密推理](#item-15)
16. [Adobe 修复 ColdFusion 与 Campaign Classic 中三个 CVSS 10.0 漏洞](#item-16)
17. [与 Trivy 黑客事件相关的恶意 LiteLLM 发布可能影响 2100 多家组织](#item-17)
18. [SAP 修复 Commerce Cloud 高危漏洞，可导致远程代码执行](#item-18)
19. [Cisco ASA 与 FTD 漏洞 CVE-2026-20349 遭野外利用可致远程拒绝服务](#item-19)
20. [黑客利用 Adobe Commerce 关键漏洞劫持用户账户](#item-20)

---

<a id="item-1"></a>
## [DeepSeek 发布新一代旗舰模型 V4 Pro 0813](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 9.0/10

DeepSeek 发布了 DeepSeek V4 Pro 0813，这是一款新的高性能 AI 模型，已在 OpenRouter 上线。早期社区反馈显示，该模型在交通模拟器和分布式物理引擎等开发工作负载上带来了显著提升。 作为 DeepSeek 这一领先开源权重 AI 实验室的发布产品，V4 Pro 0813 有望进一步推动开源大语言模型的能力上限，并降低推理成本。它很可能会影响 AI/ML 开发工作流，并加剧各模型厂商之间的竞争。 该新闻条目链接到 OpenRouter，不过社区成员指出该页面缺乏有用信息，并建议改用官方 API 文档或官方评测帖。还有评论者批评基准测试图表缺少标签和刻度；早期用户在约 50% 缓存命中率下、每 2B tokens 约 12.50 美元的成本中报告了不错的表现。

hackernews · explosion-s · 8月12日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=49274600)

**背景**: DeepSeek 是一家以发布开源权重模型著称的中国 AI 公司，其 DeepSeek-R1 于 2025 年 1 月登上 iOS App Store 下载榜首，引发全球关注。据公开资料，DeepSeek V4 Pro 采用混合专家（MoE）架构，总参数达 1.6 万亿，但每次推理仅激活约 49B 参数，从而实现高效、低成本的推理。该模型现已通过 OpenRouter、Hugging Face 等平台提供。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek -ai/ DeepSeek - V 4 - Pro · Hugging Face</a></li>
<li><a href="https://framia.converge.ai/page/zh-CN/news/deepseek-v4-canshu-xiangjie">DeepSeek V 4 参数解析：1.6 万亿总参数与 49B 激活参数详解</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(product)">DeepSeek (product)</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极——有用户表示一整天都在交通模拟器和分布式物理引擎上使用 V4 Pro 0813，发现“显著提升”且没有引入新问题；也有用户说此前的 DeepSeek Flash 更新已经令人惊艳，非常期待这次新版本。但也有批评集中在展示方式上：有评论者称 OpenRouter 页面信息量不足、基准测试图表没有标签和刻度，还有人指出所附 SVG 演示存在渲染错误。

**标签**: `#AI`, `#DeepSeek`, `#LLM`, `#Model Release`

---

<a id="item-2"></a>
## [Qwen 发布大型 MoE 模型，宣称性能接近顶尖](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen 发布了 Qwen3.8-2.4T-A95B，一个拥有 2.4 万亿总参数、950 亿激活参数的开源 MoE 模型。该发布包含 BF16 和 FP8 检查点，并宣称性能可与 Claude Opus 和 Kimi k3 等顶级模型媲美。 此次发布推进了开源模型的边界，可能让研究人员和开发者在无需专有 API 的情况下获得接近顶级的性能。同时也加剧了开源实验室之间的竞争，并可能加速低比特量化技术的应用。 该模型架构包含 512 个路由专家，每个 token 激活 10 个专家外加 1 个共享专家，基于 92 层混合注意力主干。完整 BF16 检查点约 4.9TB，而 Unsloth 的 1 比特量化版本约为 397GB；许可证允许内部使用或年营收低于 5000 万美元时免费使用。

hackernews · Philpax · 8月12日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=49273478)

**背景**: Mixture-of-Experts（MoE）是一种架构，对于每个输入 token 只条件性地激活一部分参数，从而在可接受的推理成本下构建更大的模型。FP8 量化将模型权重压缩为 8 位浮点数，大幅降低内存和计算需求，使大规模模型更易于部署在消费级硬件上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://deepwiki.com/zenrran4nlp/Awesome-LLM-Inference-Serving/4.3-mixture-of-experts-(moe)">Mixture of Experts ( MoE ) | DeepWiki</a></li>
<li><a href="https://arxiv.org/abs/2208.09225">[2208.09225] FP8 Quantization: The Power of the Exponent</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论总体正面，赞赏 1 比特量化版本约 397GB、可在单台高端机器上运行，同时也指出完整 BF16 模型难以服务。部分用户指出与 Qwen3.8-Max 相比，开源版本缺少视觉输入和 1M 上下文长度，另外还讨论了与 Kimi k3 以及 DeepSeek 即将推出的 V4-Pro 基准对比。

**标签**: `#AI`, `#LLM`, `#Qwen`, `#MoE`, `#Machine Learning`

---

<a id="item-3"></a>
## [Lazarus 利用 Windows 零日漏洞获取 SYSTEM 权限并部署后门](https://thehackernews.com/2026/08/lazarus-exploits-windows-zero-day-to.html) ⭐️ 9.0/10

Lazarus 集团（朝鲜国家支持的黑客组织）利用了微软 2026 年 8 月补丁日刚修复的 Windows 零日漏洞 CVE-2026-68820，部署了一款此前从未见过的后门。此攻击针对法国、德国、巴西和印度的国防与航空航天企业，是 Operation Dream Job 行动的一部分。 此次事件表明，国家级威胁行为者会积极利用新发现的零日漏洞攻击关键工业领域，可能导致数据窃取、知识产权流失以及更深入的网络入侵。由于该漏洞可用于本地权限提升，防御者必须优先应用 2026 年 8 月的安全更新，以防止攻击者获得 SYSTEM 权限并部署后续后门。 CVE-2026-68820 是 Windows WinSock 辅助功能驱动程序（Ancillary Function Driver）中的一个释放后使用（use-after-free）漏洞，允许已认证攻击者在本地将权限提升至 SYSTEM。微软 2026 年 8 月补丁日共修复了 400 多个漏洞，但在补丁发布前，该零日漏洞已被野外利用。

rss · The Hacker News · 8月12日 17:39

**背景**: Lazarus Group 是一个疑似由朝鲜政府支持的高级持续性威胁组织，曾发动索尼影业攻击、WannaCry 勒索病毒等破坏性攻击，并参与多起加密货币盗窃事件。Operation Dream Job 是一项长期间谍行动，通过虚假招聘信息引诱受害者下载恶意软件，主要针对国防、航空航天等高价值领域。此次新攻击将该行动的触角扩展至更多国家，并使用新型后门，凸显了国家级对手带来的持续威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2026-68820">NVD - CVE-2026-68820</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/08/12/august-2026-patch-tuesday-cve-2026-68820/">Microsoft patches 400+ vulnerabilities, one zero-day under ...</a></li>
<li><a href="https://attack.mitre.org/campaigns/C0022/">Operation Dream Job, Operation North Star, Operation Interception, Campaign C0022 | MITRE ATT&CK®</a></li>

</ul>
</details>

**标签**: `#security`, `#zero-day`, `#malware`, `#threat intelligence`, `#Windows`

---

<a id="item-4"></a>
## [攻击者利用 VMware vCenter 漏洞实现持久远程访问](https://thehackernews.com/2026/08/attackers-exploit-vmware-vcenter.html) ⭐️ 9.0/10

QUIRSO 发现 CVE-2026-59310 正在被积极利用，这是 Broadcom VMware vCenter Server 中的一个严重目录遍历漏洞（CVSS 9.8），攻击者可通过网络访问执行任意代码。虽然补丁已发布，但威胁行为者已利用该漏洞获取持久远程访问权限。 由于 vCenter Server 是 vSphere 环境的核心管理平台，成功利用该漏洞可能危及企业大量虚拟基础设施。CVSS 评分极高且已被野外利用，安全团队应视为紧急修补事项。 CVE-2026-59310 是一个 CVSS 评分为 9.8 的目录遍历漏洞，具有网络访问权限的攻击者可利用它执行任意代码。Broadcom 已发布补丁，但报告未包含 Broadcom 官方声明；组织应核对其 vCenter Server 版本与厂商公告是否匹配。

rss · The Hacker News · 8月12日 09:01

**背景**: 目录遍历（路径遍历）攻击利用诸如 ../ 之类的特殊序列，使攻击者能够逃出 Web 根目录，访问预期目录之外的敏感文件。VMware vCenter Server 是用于 vSphere 虚拟基础设施的集中管理工具，通常部署在本地和混合云环境中。CVSS 评分范围从 0 到 10，9.8 分被视为严重级别，但优先级排序可能还会考虑可利用性和资产是否暴露于互联网等因素。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Directory_traversal_attack">Directory traversal attack - Wikipedia</a></li>
<li><a href="https://www.vmware.com/docs/vmw-datasheetvcenter">vCenter Server Datasheet - VMware</a></li>
<li><a href="https://nvd.nist.gov/vuln-metrics/cvss">NVD - Vulnerability Metrics CVSS Scoring Explained: How Vulnerability Scores Work CVSS Score Explained: How CVSS Scoring Really Works NVD - CVSS v3 Calculator What is CVSS? | Tutorial and examples | Snyk Learn CVSS 9.8 Is Not Priority: Triage with EPSS + KEV — AppScale Blog</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#VMware`, `#CVE`, `#exploit`

---

<a id="item-5"></a>
## [ShieldBreak 零日 PoC 绕过微软 Defender 补丁获取 SYSTEM 权限](https://thehackernews.com/2026/08/shieldbreak-zero-day-poc-claims.html) ⭐️ 9.0/10

安全研究员 Chaotic Eclipse（又名 Nightmare Eclipse）发布了名为 ShieldBreak 的零日漏洞概念验证（PoC），该漏洞可绕过微软于 2026 年 8 月补丁星期二发布的、针对 Microsoft Defender 中 CVE-2026-50656（RoguePlanet）的修复补丁，从而在 Windows 上获得 SYSTEM 级访问权限。目前该说法尚未得到独立证实。 如果得到证实，ShieldBreak 将构成一个关键的权限提升攻击途径，因为它能绕过微软最近为广泛部署的组件（Microsoft Defender/恶意软件防护引擎）发布的安全补丁。这将促使企业防御者紧急评估自身风险暴露面，并促使微软准备应对措施，同时也会引发关于补丁可靠性和零日漏洞披露的更广泛讨论。 ShieldBreak 针对的是 CVE-2026-50656（又名 RoguePlanet）的补丁绕过，该漏洞是 Microsoft Defender 所使用的微软恶意软件防护引擎中的权限提升漏洞（CVSS 评分为 7.8）。该 PoC 在 2026 年 8 月补丁星期二更新发布后不久即被公开，研究人员声称可利用其提升至 SYSTEM 权限，但完整技术细节尚未得到验证。

rss · The Hacker News · 8月12日 06:41

**背景**: Microsoft Defender 是 Windows 内置的杀毒和端点保护平台，其恶意软件防护引擎负责在内核态和用户态执行文件扫描。CVE-2026-50656（公开代号 RoguePlanet）是该引擎中的一个权限提升漏洞，微软此前已对其进行修复。所谓“补丁绕过”意味着研究人员找到了绕过该修复的方法，可能使已应用补丁的系统重新暴露在风险之中。零日漏洞和补丁绕过声明尤其严重，因为补丁是许多组织最重要的缓解措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vulmon.com/vulnerabilitydetails?qid=CVE-2026-50656">Vulnerability details of CVE - 2026 - 50656</a></li>
<li><a href="https://www.linkedin.com/posts/cyber-tzar-intelligence_microsoft-releases-fix-for-rogueplanet-defender-activity-7480973024570253312-uwQF">Microsoft Fixes Windows Defender Vulnerability CVE - 2026 - 50656</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lldzQyX0VSRUx1blRSRFVxT2JpZ0FQAQ?hl=en-US&gl=US&ceid=US:en">Google News - Microsoft fixes RoguePlanet zero-day vulnerability in...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#zero-day`, `#Microsoft Defender`, `#privilege escalation`, `#CVE-2026-50656`

---

<a id="item-6"></a>
## [Tailscale 将数据库损坏追溯至一个存在 16 年的 SQLite WAL 重置 Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale 发布了一篇博客文章，详细说明了一个存在 16 年的 SQLite 预写日志（WAL）重置逻辑 Bug 如何导致数据库损坏，并宣布他们资助了一个开源 VFS shim，用于隔离这一竞争条件并帮助未来发现类似问题。 这件事意义重大，因为 SQLite 是使用最广泛的数据库引擎之一，而一个隐藏了 16 年的 Bug 揭示了即使再充分的测试也有其局限。其资助的 VFS shim 为更广泛的开源生态提供了可复用的调试工具，并有助于防止类似的损坏问题。 该 Bug 位于 SQLite 的 WAL 重置逻辑中，只有在多个数据库连接以特定方式交互时才会触发。Tailscale 采用的是单写入者设计，但竞争条件仍然发生；他们资助的 VFS shim 可以隔离该竞争条件，并可复用于检测类似问题。

hackernews · ropbear · 8月12日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49272832)

**背景**: SQLite 使用预写日志（WAL）模式来提高性能和并发性，将更改先写入单独的 -wal 文件，然后再检查点到主数据库。VFS（虚拟文件系统）shim 是围绕默认 VFS 的包装器，可以拦截和检测文件操作；例如，SQLite 提供了一个校验和 VFS shim 来验证页面完整性。竞争条件是指多个进程或线程同时访问共享数据，而最终结果取决于它们执行的时序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite.org/vfs.html">The SQLite OS Interface or "VFS"</a></li>
<li><a href="https://notes.nikolamilekic.com/Readwise/Articles/SQLite+Write-Ahead+Logging">SQLite Write - Ahead Logging - Nikola's Digital Garden</a></li>
<li><a href="https://www.geeksforgeeks.org/operating-systems/race-condition-in-operating-systems/">Race condition - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: 评论者对这篇文章表示赞赏，并指出即使 SQLite 拥有非凡的测试覆盖率（单元测试的行覆盖率达到 59,000%），也未能发现这个存在 16 年的缺陷，凸显了测试的局限性。其他人认可 Tailscale 资助特定开源调试工具的做法，并围绕“尽管采用单写入者设计，但多个连接仍会导致竞争条件”展开了讨论。

**标签**: `#sqlite`, `#tailscale`, `#database`, `#bug`, `#open-source`

---

<a id="item-7"></a>
## [WebSocket 传输 HTML：几乎不用 JavaScript 的实时 SPA](https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/) ⭐️ 8.0/10

Andros Fenollosa 的这篇文章探讨了 HTML-over-WebSockets 模式，即服务器通过 WebSocket 连接推送渲染好的 HTML 片段来更新页面，从而以极少的客户端 JavaScript 实现实时 SPA。文章将这种方法定位为更广泛的 HTML-over-the-wire 家族中的双向变体，并以 Phoenix LiveView 作为先驱示例。 这之所以重要，是因为它挑战了“实时 SPA 必须依赖大型客户端 JavaScript 框架”的假设，提供了一种更简单、以服务器为中心的单一语言模型。它还引发了社区关于 WebSocket、Server-Sent Events（SSE）和 htmx 等方法之间取舍的热烈讨论。 文章提出的经验法则是：对于聊天、协作或游戏等需要双向低延迟通信的场景使用 WebSocket；对于大多数服务器推送场景，则优先使用 Server-Sent Events（SSE）加 Fetch，因为浏览器已经会对 HTTP 请求进行多路复用。文章以 Phoenix LiveView 作为推广服务器端渲染实时 HTML 的框架示例，该技术也出现在 server-side Blazor 中。

hackernews · redbell · 8月12日 16:51 · [社区讨论](https://news.ycombinator.com/item?id=49275335)

**背景**: HTML-over-WebSockets 是 HTML-over-the-wire 技术的一种变体：服务器生成 HTML 片段，并通过一条长期存活的 WebSocket 连接发送给客户端，客户端只需将这些片段替换到 DOM 中。Phoenix LiveView 是 Elixir 的 Phoenix 框架的实时扩展，它以一个普通 HTTP 请求开始，随后升级为基于 WebSocket 的有状态视图，并在服务器端状态变化时自动重新渲染。这种方法属于一个更广泛的趋势：偏爱服务器端渲染和极简 JavaScript，而不是 JSON API 加客户端渲染。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hexdocs.pm/phoenix_live_view/Phoenix.LiveView.html">Phoenix.LiveView — Phoenix LiveView v1.2.9</a></li>
<li><a href="https://alistapart.com/article/the-future-of-web-software-is-html-over-websockets/">The Future of Web Software Is HTML-over-WebSockets – A List Apart</a></li>
<li><a href="https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/">HTML over WebSockets: real-time SPAs with barely any JavaScript | Andros Fenollosa</a></li>

</ul>
</details>

**社区讨论**: 评论者们正在积极地讨论其中的取舍：有人认为对于大多数应用来说 SSE 更简单、成本更低，WebSocket 应留给真正需要双向低延迟的场景；也有人为 WebSocket 方法辩护，指出该技术早于 LiveView（源于 Chris McCord 的 Rails 项目 Sync）。还有几位评论者推荐用 htmx 配合 SSE 和 DOM 变形来获得类似好处，而无需“重新发明轮子”；其中一位还附上了对这篇文章的回应链接（yagni.club）。

**标签**: `#websockets`, `#real-time`, `#spa`, `#html`, `#phoenix-liveview`

---

<a id="item-8"></a>
## [xAI 发布 Grok 4.6，前沿模型定价激进](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI（现以 SpaceXAI 名义运营）于当天发布了 Grok 4.6，这是一个基于 V9 基础架构、拥有 1.5 万亿参数的前沿模型。据报道，它的 ELO 达 1753，在 Artificial Analysis 上与 GPT-5.6 Sol 持平，定价约为竞争对手前沿模型的一半。 Grok 4.6 以显著更低的价格提供接近顶尖的性能，加剧了前沿 AI 市场的竞争，可能促使其他实验室降价。它对长时间运行的智能体、编程和知识工作的关注，也使其成为企业和开发者工作负载的实用工具。 据报道，该模型与 Grok 4.5 同基于 V9 基础架构，拥有 1.5 万亿参数，但增加了补充训练并改进监督微调。在 Artificial Analysis 上，它超越了 Kimi K3，与 GPT-5.6 Sol 并列全球第三，同时提供更便宜的 API 定价和 Cursor 订阅上的慷慨用量。

hackernews · iLuddite · 8月12日 15:32 · [社区讨论](https://news.ycombinator.com/item?id=49274027)

**背景**: 前沿 AI 模型是最高级的通用人工智能系统，通常需要极大的算力预算（约 10^26 FLOPS），并在多个领域超越当前最先进水平，这是前沿模型论坛的定义。xAI 由埃隆·马斯克创立，一直在快速迭代 Grok 系列；Grok 4.5 大约一个月前发布，定价为每百万输入 tokens 2 美元、每百万输出 tokens 6 美元，token 效率约为对手的两倍。Grok 4.6 在此基础上构建，公司也更名为 SpaceXAI，反映其与 SpaceX 推理投资的紧密联系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.basenor.com/blogs/news/xai-launches-grok-4-6-1753-elo-half-the-price-of-rival-frontier-models">xAI Launches Grok 4.6: 1753 ELO, Half the Price of Rival Frontier Models</a></li>
<li><a href="https://venturebeat.com/technology/spacexai-debuts-grok-4-6-overtaking-kimi-k3s-performance-and-matching-gpt-5-6-sol-for-worlds-third-best-on-artificial-analysis">SpaceXAI debuts Grok 4.6, overtaking Kimi K3's performance and matching GPT-5.6 Sol for world's third best on Artificial Analysis | VentureBeat</a></li>
<li><a href="https://x.ai/news/grok-4-5">Introducing Grok 4.5 | SpaceXAI</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一。一些用户抱怨 API 现在会注入默认系统提示词，覆盖用户指令；另一些人则质疑所有主要实验室如何在两个月内突然达到‘Fable 级别’的性能，怀疑是基准测试作弊。还有部分人认为 Grok 4.6 是一个健康、更便宜的竞争者，并指出 Grok 的回答风格比竞争对手更简洁。

**标签**: `#AI`, `#Grok`, `#xAI`, `#LLM`, `#Model Release`

---

<a id="item-9"></a>
## [Chrome 的部分 JPEG 解码导致小尺寸图片渲染不同](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

一篇技术博客文章指出，Chrome 在缩小小型图片时采用部分 JPEG 解码，其显示效果与 Firefox 先完整解码再缩放的方式显著不同。文章还提供了变通方法，并建议避免使用 JPEG 作为图标格式。 这种细微的跨浏览器渲染差异会导致网页和 Electron 应用界面显示不一致，甚至使图标在 Chrome 优化后异常。了解其根本原因有助于开发者选择合适的图片格式和分辨率，以确保渲染可靠。 该文章给出了变通方法，并提醒 JPEG 适用于照片而非边缘锐利的图标等图形。Firefox 正在 Bugzilla bug 2033250 中跟踪按比例解码的支持；评论者还指出 Chrome 和 Firefox 使用不同的缩放算法，Chrome 更模糊，Firefox 更锐利但容易出现振铃伪影。

hackernews · gutechh · 8月12日 14:00 · [社区讨论](https://news.ycombinator.com/item?id=49272549)

**背景**: JPEG 是一种有损图像格式，采用基于分块的 DCT 压缩和色度抽样，因此不适用于边缘锐利的图标。当浏览器需要显示小尺寸图片时，一些浏览器会为了提高效率只解码部分压缩数据，即“部分解码”；另一些浏览器则先完整解码再缩放。loopbio 的博客文章指出，部分解码 JPEG（例如只解码裁剪区域而不处理整张图片）是性能敏感型库中的一种已知优化。cgjennings.ca 上关于 JPEG 压缩的文章展示了不同缩放方法如何产生不同伪影。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://blog.loopbio.com/video-io-2-jpeg-decoding.html">Video I/O Part 2: Fast JPEG Decoding – loopbio blog</a></li>
<li><a href="https://www.cgjennings.ca/articles/jpeg-compression/">How JPEG works (Christopher G. Jennings)</a></li>

</ul>
</details>

**社区讨论**: 评论者称相同问题也出现在 PNG 上，并在一次 Electron 升级中导致图标异常。有评论者认为真正的教训是使用合适分辨率的图片而非 JPEG 做图标，另有评论者指出 Chrome 和 Firefox 使用了不同的缩放算法。一位 Firefox 开发者还贴出了用于低比例解码工作的 Bugzilla 链接。

**标签**: `#jpeg`, `#chrome`, `#firefox`, `#image-processing`, `#web-performance`

---

<a id="item-10"></a>
## [车牌读取器搜索应需搜查令](https://andrewpwheeler.com/2026/08/12/license-plate-reader-searches-should-require-a-warrant/) ⭐️ 8.0/10

Andrew Wheeler 的新文章主张，执法部门搜索自动车牌识别（ALPR）数据应需要搜查令，理由是隐私关切和警察问责。这篇文章引发了广泛的社区讨论，共有 323 条评论。 由于 ALPR 摄像头会拍摄每辆过往车辆的车牌并记录其位置和时间，无搜查令访问会让普通人的行踪遭到大规模追踪。要求搜查令将为此类目前仅受各州零散薄弱法律约束的监控技术加上司法监督。 文章认为，所有公共空间安装摄像头是不可避免的，因此关注的是法律保障而非禁止该技术。评论者指出，ALPR 是可联网、可重新编程的摄像头，而且 2025–2026 年的审计发现，联邦和外州机构绕过了各州的留存和数据共享规定。

hackernews · apwheele · 8月12日 14:43 · [社区讨论](https://news.ycombinator.com/item?id=49273165)

**背景**: 自动车牌识别（ALPR）利用摄像头和图像处理软件自动读取车牌，通常安装在警车或固定路侧摄像头上。相关数据会被存储，并可通过检索来还原车辆的行踪。目前美国没有全面的联邦法律来监管 ALPR，而是由各州零散的法律来规定数据留存与共享；隐私倡导者警告，此类数据库容易遭到泄露和滥用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sls.eff.org/technologies/automated-license-plate-readers-alprs">Automated License Plate Readers</a></li>
<li><a href="https://www.recordinglaw.com/us-laws/automated-license-plate-readers/">Automated License Plate Reader (ALPR) Laws Explained (2026)</a></li>
<li><a href="https://www.homelandsecuritynewswire.com/dr20251015-despite-widespread-interest-only-3-states-passed-license-plate-reader-laws-this-year">Privacy, license-plate readers, law enforcement | Homeland ...</a></li>

</ul>
</details>

**社区讨论**: 评论者大体上认为有搜查令总比没有好，但有人提出，大规模监控本就不应默认存在。还有人强调，ALPR 是通用型、可重新编程的摄像头，担心警察滥用数据——比如警员跟踪前伴侣；也有评论者提出一种涉及车牌号码轮换的加密设想。

**标签**: `#privacy`, `#surveillance`, `#law enforcement`, `#public policy`, `#technology`

---

<a id="item-11"></a>
## [高尔斯：LLM 擅长数学靠采样而非刻意推理](https://gowers.wordpress.com/2026/08/12/what-sort-of-maths-are-llms-good-at/) ⭐️ 8.0/10

蒂莫西·高尔斯（Timothy Gowers）的新博文分析了大型语言模型擅长处理哪些类型的数学问题，认为其成功主要来自采样（sampling）和测试时扩展（test-time scaling），而非刻意的推理。这篇文章以一个数学家的视角解释了为什么这些方法如此强大。 作为菲尔兹奖得主的权威分析，这篇文章为 LLM 数学能力的真实机制提供了可信的专家视角，有助于引导研究方向并管理公众预期。它也呼应了行业中以测试时扩展来提升模型性能的趋势。 这篇文章从未明确使用“测试时扩展”一词，但评论者将其观点与这一研究领域联系起来。文章还强调了朴素采样——生成大量候选输出并筛选——是一种出人意料有效的方法，正如 2022 年谷歌 AlphaCode 所展示的那样。

hackernews · ColinWright · 8月12日 10:04 · [社区讨论](https://news.ycombinator.com/item?id=49270022)

**背景**: 大型语言模型（LLM）通过预测下一个词元（token）来生成文本，而温度、top-k、top-p 等采样技术控制着这种预测的随机性。测试时扩展是指在推理阶段给模型更多计算量——例如让它生成更多样本或更长时间地推理——以提高输出质量。蒂莫西·高尔斯是一位著名数学家，以组合数学和泛函分析方面的工作闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2408.03314">[2408.03314] Scaling LLM Test-Time Compute Optimally can be More Effective than Scaling Model Parameters</a></li>
<li><a href="https://testtimescaling.github.io/">What, How, Where, and How Well? A Survey on Test-Time Scaling in Large Language Models</a></li>
<li><a href="https://machinelearningmastery.com/how-llms-choose-their-words-a-practical-walk-through-of-logits-softmax-and-sampling/">How LLMs Choose Their Words: A Practical Walk-Through of Logits, Softmax and Sampling - MachineLearningMastery.com</a></li>

</ul>
</details>

**社区讨论**: 评论者对这篇文章反应热烈，有几人指出它本质上是在讨论测试时扩展，并以 AlphaCode 作为早期纯采样成功的例子。也有人赞同高尔斯关于如何识别人类水平数学贡献的标准，并分享了 AI 数学成就的列表；还有评论者好奇编码代理（coding agent）在时序逻辑上的表现。总体情绪积极且充满求知欲。

**标签**: `#LLM`, `#mathematics`, `#test-time scaling`, `#sampling`, `#AI research`

---

<a id="item-12"></a>
## [Woxi：开源 Rust 实现的 Wolfram 语言解释器](https://woxi.ad-si.com/) ⭐️ 8.0/10

Woxi 是一个用 Rust 编写的 Wolfram 语言开源解释器，随附基于 iced 框架构建的类 Mathematica 图形界面 Woxi Studio。它还提供 CLI、Jupyter 内核、Python/npm 包和 WASM 模块，并通过约 26,000 个单元测试和约 900 个.wls 脚本快照测试来保证符合性。 Woxi 为专有的 Mathematica/Wolfram 语言提供了免费、开源的替代方案，毫秒级启动时间使其适用于脚本和短生命周期进程。这可能会降低依赖 Wolfram 语言但偏好开源工具的学生、研究人员和开发者的使用门槛。 主要限制包括不支持乱序执行和%变量，这些在 Mathematica 笔记本中很常见。该项目目前专注于修复边界情况、提升性能和发展社区，项目文档站点上提供了与 Mathematica 的详细对比。

hackernews · adius · 8月12日 10:06 · [社区讨论](https://news.ycombinator.com/item?id=49270040)

**背景**: Wolfram 语言是 Wolfram Research 开发的专有高级多范式编程语言，以符号计算著称，并作为 Mathematica 的编程语言使用。WolframScript 是运行 Wolfram 语言代码的官方命令行工具，但通常需要数秒才能启动。Woxi 使用 Rust 编写，基于 iced 跨平台 GUI 库，目标是快速启动，并可通过 WebAssembly 或作为嵌入式脚本语言嵌入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wolfram_Language">Wolfram Language</a></li>
<li><a href="https://www.wolfram.com/wolframscript/">WolframScript for the Command Line: Execute Wolfram Language ...</a></li>
<li><a href="https://iced.rs/">iced - A cross-platform GUI library for Rust</a></li>

</ul>
</details>

**社区讨论**: 评论者总体持积极但谨慎态度，称赞项目潜力的同时指出缺少%和乱序执行等功能，还有人请求添加控制系统模块。一位评论者希望它成为 SageMath 的集成良好、快速替代品，另一位在 Woxi Studio 中测试了微积分可视化，认为大部分能显示，还有用户指出该项目六个月前曾发布过。

**标签**: `#Rust`, `#Wolfram Language`, `#open-source`, `#interpreter`, `#scientific computing`

---

<a id="item-13"></a>
## [NVIDIA 详解在 GB300 NVL72 上部署 Qwen3.8-2.4T-A95B](https://developer.nvidia.com/blog/serve-qwen3-8-2-4t-a95b-a-2-4t-parameter-model-with-configurable-reasoning-on-nvidia-gb300-nvl72/) ⭐️ 8.0/10

阿里巴巴发布了 Qwen3.8-2.4T-A95B（Qwen3.8-Max）的开源权重，这是一个拥有 2.4T 参数、95B 活跃参数的稀疏混合专家模型。NVIDIA 发布了一篇博客文章，演示如何在 GB300 NVL72 平台上以可配置推理方式部署该模型。 这标志着迄今为止最大规模的开源权重模型发布，将接近前沿的能力带给了开源社区。NVIDIA 在 GB300 NVL72 上的部署指南帮助企业规模化运行诸如代码生成和文档分析等智能体 AI 工作负载。 该模型采用稀疏混合专家架构，总参数 2.4T，但只有 95B 活跃参数，因而在如此规模下仍能高效推理。GB300 NVL72 是 NVIDIA 的 Blackwell Ultra 机架级平台，配备液冷，专为大规模大语言模型部署设计。

rss · NVIDIA Developer Blog · 8月12日 18:23

**背景**: Qwen 是阿里巴巴的开源大语言模型系列，Qwen3.8-2.4T-A95B 是 Qwen3.8 Max 的开源权重版本。混合专家模型每个 token 只激活一部分参数，从而在模型容量与算力成本之间取得平衡。NVIDIA GB300 NVL72 是一款配备 72 个 GPU 和液冷的机架级服务器，适合部署前沿规模的模型。可配置推理允许用户根据任务复杂度开启或关闭推理模式，在延迟与准确性之间进行取舍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/serve-qwen3-8-2-4t-a95b-a-2-4t-parameter-model-with-configurable-reasoning-on-nvidia-gb300-nvl72/">Serve Qwen3.8-2.4T-A95B, a 2.4T-Parameter Model, with ...</a></li>
<li><a href="https://benchable.ai/models/qwen/qwen3.8-2.4t-a95b-20260812">Qwen: Qwen3.8 2.4T A95B - AI Model Details & Benchmarks</a></li>
<li><a href="https://www.modelscope.cn/models/Qwen/Qwen3.8-2.4T-A95B">Model Details · ModelScope</a></li>

</ul>
</details>

**标签**: `#Qwen`, `#NVIDIA`, `#LLM serving`, `#open-source model`, `#AI infrastructure`

---

<a id="item-14"></a>
## [737 个恶意 Chrome VPN 扩展被曝劫持浏览器流量](https://thehackernews.com/2026/08/737-chrome-vpn-extensions-caught.html) ⭐️ 8.0/10

研究人员发现，Chrome 网上应用店中有 737 个恶意扩展，冒充知名 VPN 和代理服务。这些扩展将用户浏览器流量通过由单一运营商控制的 SOCKS5 代理转发，累计安装量达 75,486 次，分布于至少 40 个开发者账户。 这一活动暴露了 Chrome 网上应用店中的供应链风险：免费的 VPN 和代理扩展可以静默拦截并重定向敏感浏览器流量。受影响用户主要是试图绕过封锁的俄语用户，其浏览数据可能被暴露，这对整个扩展生态来说是一个严重的隐私与安全问题。 这 737 个扩展通过至少 40 个 Chrome 网上应用店开发者账户发布，其中 274 个冒充 66 个知名 VPN 和代理品牌。它们并非提供真正的私密隧道，而是将流量转发到由单一运营商控制的 SOCKS5 代理基础设施，这意味着浏览活动可能被记录或监控。

rss · The Hacker News · 8月12日 14:09

**背景**: SOCKS5 是一种互联网协议，它通过代理服务器在客户端和服务器之间转发网络数据包，通常用于保护隐私和绕过地域限制。恶意扩展滥用该协议，将用户的浏览器流量静默发送到第三方代理，从而让运营者能够拦截、记录或修改数据。免费 VPN 扩展通常要求用户授予广泛权限，因此成为这类攻击的常见载体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SOCKS_(proxy)">SOCKS (proxy)</a></li>

</ul>
</details>

**标签**: `#security`, `#chrome extensions`, `#malware`, `#VPN`, `#privacy`

---

<a id="item-15"></a>
## [API 漏洞使较弱 AI 模型可解码顶级 LLM 的加密推理](https://thehackernews.com/2026/08/openai-anthropic-google-api-flaw-let.html) ⭐️ 8.0/10

研究人员披露了一个影响 OpenAI、Anthropic 和 Google 推理 API 的架构性漏洞，较弱的同类模型可借此从加密推理块中恢复隐藏的思维链推理过程。该攻击还能从会话日志中提取 API 密钥和密码等机密信息。 这一漏洞意义重大，因为它破坏了主要 AI 提供商用来保护专有推理过程隐私的机制，可能导致敏感数据跨会话和跨用户泄露。使用这些推理 API 的企业和开发者面临即时的数据泄露风险，该缺陷也引发了对加密思维链设计安全性的更广泛质疑。 论文《Stealing Reasoning Traces from Proprietary LLM APIs》演示了四种攻击向量，包括绕过防蒸馏机制，并表明加密推理块可在会话、用户和模型之间重放。研究人员报告称，在测试中公共日志暴露了 182 个凭据。

rss · The Hacker News · 8月12日 11:47

**背景**: 前沿 LLM API 通常通过向客户端返回加密的推理块来隐藏模型的“思维链”（即内部逐步推理过程），目的是保护知识产权并减少信息泄露。这种设计假设密文无法被解读或重放，但新研究显示，这些推理块可以被输入到防护较弱的同类模型中，从而还原出明文推理内容以及会话日志中嵌入的敏感数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.09867">Stealing Reasoning Traces from Proprietary LLM APIs</a></li>
<li><a href="https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/">Stealing Reasoning Traces from Proprietary LLM APIs</a></li>
<li><a href="https://cybersecuritynews.com/top-ai-models-apis-flaw-exposes-hidden-reasoning/">OpenAI, Anthropic, and Google LLM APIs vulnerability Exposes ...</a></li>

</ul>
</details>

**标签**: `#security`, `#AI`, `#API`, `#vulnerability`, `#LLM`

---

<a id="item-16"></a>
## [Adobe 修复 ColdFusion 与 Campaign Classic 中三个 CVSS 10.0 漏洞](https://thehackernews.com/2026/08/adobe-patches-three-cvss-100-coldfusion.html) ⭐️ 8.0/10

Adobe 已为 ColdFusion、Commerce 和 Campaign Classic 发布安全更新，修复了多个严重漏洞，其中包括三个最高严重级别的 CVSS 10.0 漏洞。目前已披露的最严重漏洞是 CVE-2026-48362，这是 ColdFusion 中的一个操作系统命令注入漏洞，可能允许任意代码执行。 这些是广泛使用的企业软件中存在的最高严重级别漏洞，因此管理员和安全团队应立即应用补丁。成功利用这些漏洞可能导致任意代码执行和权限提升，使受影响的系统面临高风险。 公告列出了 CVE-2026-48362，其 CVSS 评分为 10.0，这是 ColdFusion 中的一个操作系统命令注入漏洞。Adobe 的更新还涵盖 Adobe Commerce 和 Campaign Classic 中的关键问题，不过摘要中未包含其他两个 CVSS 10.0 漏洞的完整细节。

rss · The Hacker News · 8月12日 11:13

**背景**: Adobe ColdFusion 是一个商业化的快速 Web 应用开发平台，使用 CFML 脚本语言，广泛用于构建和部署 Web 应用。Adobe Campaign Classic 是一款营销工具，允许组织通过电子邮件、短信、移动应用和其他数字渠道编排营销活动。CVSS 10.0 是通用漏洞评分系统（CVSS）下的最高严重级别评分，表示此类漏洞既容易被利用又具有很高的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Adobe_ColdFusion">Adobe ColdFusion - Wikipedia</a></li>
<li><a href="https://www.adobe.com/sg/products/coldfusion-family.html">Adobe ColdFusion Family</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System">Common Vulnerability Scoring System - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#adobe`, `#vulnerability`, `#patch`, `#coldfusion`

---

<a id="item-17"></a>
## [与 Trivy 黑客事件相关的恶意 LiteLLM 发布可能影响 2100 多家组织](https://thehackernews.com/2026/08/malicious-litellm-releases-tied-to.html) ⭐️ 8.0/10

今年 3 月，PyPI 上的两个恶意 LiteLLM 版本包含窃取凭据的代码，并公开了约 40 分钟。CloudSEK 表示，从攻击者截获的大约 43.4 万个文件中获得的数据显示，可能影响到 2100 多家组织。 这是一次针对广泛使用的开源 LLM 代理的供应链攻击，可能导致云密钥、SSH 密钥等敏感信息泄露。影响面广，可能引发后续入侵，因此及时修复和轮换凭据至关重要。 恶意版本仅公开约 40 分钟，数据集包含攻击者截获的 43.4 万个文件。此事件与之前 Trivy（一款流行的开源安全扫描器）遭黑客攻击有关。受影响组织应审计泄露凭据并监控可疑活动。

rss · The Hacker News · 8月12日 08:04

**背景**: LiteLLM 是 BerriAI 开发的开源 Python SDK 和 AI 网关，允许开发者以 OpenAI 兼容格式调用 100 多种 LLM API。Trivy 是一种广泛使用的开源安全扫描器，用于检测漏洞、错误配置和密钥。CloudSEK 是一家威胁情报公司，提供攻击路径情报和外部威胁监控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.litellm.ai/">LiteLLM — Open-Source AI Gateway & LLM Proxy</a></li>
<li><a href="https://trivy.dev/">Trivy</a></li>
<li><a href="https://www.cloudsek.com/">CloudSEK: Predictive Attack Path Intelligence</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#PyPI`, `#LiteLLM`, `#credentials`

---

<a id="item-18"></a>
## [SAP 修复 Commerce Cloud 高危漏洞，可导致远程代码执行](https://thehackernews.com/2026/08/sap-commerce-cloud-flaw-could-let.html) ⭐️ 8.0/10

SAP 已发布针对 CVE-2026-58231 的补丁，这是 Commerce Cloud（Data Hub Adapter）中的一个最高严重级别漏洞，CVSS 评分为 10.0。由于授权检查和输入验证不足，该漏洞允许未认证的攻击者执行任意代码。 这很关键，因为 SAP Commerce Cloud 是广泛使用的企业级电商平台，未认证的远程代码执行可能导致系统完全受损、数据泄露和供应链攻击。使用受影响组件的组织应立即应用补丁。 该漏洞 CVE-2026-58231 是由 Data Hub Adapter（用于将 SAP Commerce Cloud 与后端系统集成）中的授权检查和输入验证不足引起的。CVSS 评分 10.0 表示最高严重级别，意味着利用该漏洞不需要任何权限或用户交互。

rss · The Hacker News · 8月12日 07:31

**背景**: SAP Commerce Cloud 是一个企业级电子商务平台，使用 Data Hub 与 ERP 及其他后端系统进行异步集成。Data Hub Adapter 负责在商务平台和 Data Hub 服务器之间发送和接收数据。CVSS（通用漏洞评分系统）是评估安全漏洞严重性的框架，评分从 0 到 10，其中 10 表示最严重。SAP 通常会在其补丁日发布安全说明来解决此类问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System">Common Vulnerability Scoring System - Wikipedia</a></li>
<li><a href="https://help.sap.com/docs/SAP_COMMERCE_CLOUD_PUBLIC_CLOUD/b2f400d4c0414461a4bb7e115dccd779/50bc36e2540144fe86caac6b8d904f6d.html">Data Hub with ERP Commerce Cloud Manifest Example | SAP Help Portal</a></li>
<li><a href="https://hybrismart.com/2019/08/12/commerce-data-hub-a-deep-look-better-late-than-never/">A Deeper Look at SAP Commerce Data Hub - hybrismart</a></li>

</ul>
</details>

**标签**: `#security`, `#SAP`, `#CVE-2026-58231`, `#vulnerability`, `#arbitrary code execution`

---

<a id="item-19"></a>
## [Cisco ASA 与 FTD 漏洞 CVE-2026-20349 遭野外利用可致远程拒绝服务](https://thehackernews.com/2026/08/cisco-asa-and-ftd-flaw-exploited-in.html) ⭐️ 8.0/10

思科警告称，CVE-2026-20349（CVSS 评分 8.6）是 Secure Firewall ASA 和 FTD 软件中的一个高危漏洞，正被积极利用于野外攻击，允许未认证的远程攻击者触发拒绝服务。该漏洞源于处理 HTTP 请求时错误检查不足。 由于 ASA 和 FTD 是企业广泛部署的防火墙和 VPN 产品，远程可利用的拒绝服务漏洞可能破坏网络安全边界，影响众多组织。野外利用使其紧急修补更为关键，也凸显了针对网络边缘设备的持续风险。 CVE-2026-20349 的 CVSS 评分为 8.6，无需认证，可通过特制的 HTTP 请求触发。思科建议尽快应用可用的软件更新；由于问题出在错误处理上，可能没有有效的临时缓解措施。

rss · The Hacker News · 8月12日 06:15

**背景**: Cisco 自适应安全设备（ASA）是思科于 2005 年 5 月推出的网络安全设备系列，提供防火墙、VPN 和入侵防御功能。Cisco Secure Firewall Threat Defense（FTD）是结合 ASA 和 FirePOWER 服务的统一软件镜像，用于下一代防火墙部署。CVE-2026-20349 使用通用漏洞评分系统（CVSS）进行评级，该系统用于近似评估漏洞的利用难度和影响。由于这些产品守护网络边界，拒绝服务漏洞可能导致受影响组织的安全检测中断。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cisco_ASA">Cisco ASA - Wikipedia ASA Images download Link - NetworkLessons.com Community Forum Cisco ASA Software Release 9.0 Data Sheet Cisco Adaptive Security Appliance (ASA) Software Review Top Stories</a></li>
<li><a href="https://www.cisco.com/c/en_in/products/security/adaptive-security-appliance-asa-software/index.html">Cisco Adaptive Security Appliance (ASA) Software</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System">Common Vulnerability Scoring System - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Cisco`, `#CVE-2026-20349`, `#security`, `#DoS`, `#vulnerability`

---

<a id="item-20"></a>
## [黑客利用 Adobe Commerce 关键漏洞劫持用户账户](https://www.bleepingcomputer.com/news/security/hackers-exploit-critical-adobe-commerce-flaw-to-hijack-customer-accounts/) ⭐️ 8.0/10

安全研究人员已检测到针对 Adobe Commerce 和 Magento 平台中的关键漏洞 CVE-2026-71362 的主动利用，攻击者正利用该漏洞劫持用户账户。 Adobe Commerce 和 Magento 支撑着大量在线商店，账户劫持的成功可能导致数据盗窃、撞库攻击和金融欺诈。此次主动利用使得商家急需应用补丁并保护其网站安全。 CVE-2026-71362 是一个不正确的授权漏洞，允许未认证的攻击者绕过身份验证控制。该漏洞评级为严重，且已在野外被利用，可能导致用户账户被接管。

rss · BleepingComputer · 8月12日 20:54

**背景**: Adobe Commerce 和 Magento 是广泛用于构建和管理在线商店的电子商务平台。CVE-2026-71362 是这些平台中的一个关键漏洞，利用该漏洞可导致账户被接管。使用这些平台的组织应紧急应用供应商提供的最新安全更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cvefeed.io/vuln/detail/CVE-2026-71362">CVE-2026-71362 - Adobe Commerce | Incorrect Authorization ...</a></li>
<li><a href="https://feedly.com/cve/CVE-2026-71362">CVE-2026-71362 - Exploits & Severity - Feedly</a></li>
<li><a href="https://basefortify.eu/cve_reports/2026/08/cve-2026-71362.html">CVE-2026-71362 | Incorrect Authorization in Adobe Commerce ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Adobe Commerce`, `#Magento`, `#CVE`

---