---
layout: default
title: "Horizon Summary: 2026-07-02 (ZH)"
date: 2026-07-02
lang: zh
---

> 从 87 条内容中筛选出 20 条重要资讯。

---

1. [首个能生长分裂的合成细胞诞生](#item-1)
2. [Box3D 发布：开源 3D 物理引擎](#item-2)
3. [未修补的 Argo CD 漏洞可致 Kubernetes 集群被接管](#item-3)
4. [Adobe 修补 ColdFusion 和 Campaign Classic 中的 7 个 CVSS 10.0 严重漏洞](#item-4)
5. [Cursor 严重漏洞可让提示注入逃逸沙箱](#item-5)
6. [幻影抢注：利用 AI 幻觉域名的攻击向量](#item-6)
7. [索尼将于 2028 年停止生产实体游戏光盘](#item-7)
8. [FFmpeg 9.1 AAC 编码器质量修复](#item-8)
9. [Cloudflare 推出基于 HTTP 402 的货币化网关](#item-9)
10. [乐观提供：将 IPFS 内容发布速度提升 10 倍](#item-10)
11. [Cursor 通过前部署工程师部署 AI 代理](#item-11)
12. [PEARL 与药物发现中的共折叠精确度](#item-12)
13. [Progress Kemp LoadMaster 预认证 RCE 漏洞正被积极利用](#item-13)
14. [AI 生成的勒索软件滥用 Chromium API 攻击 Windows 和 Android](#item-14)
15. [微软将后量子密码迁移时间提前至 2029 年](#item-15)
16. [Azure CLI 密码喷洒攻击致 78 个微软账户失陷](#item-16)
17. [ChocoPoC 恶意软件通过虚假 PoC 漏洞利用代码攻击研究人员](#item-17)
18. [美国国土安全部确认黑客入侵 HSIN 信息共享平台](#item-18)
19. [闭源与开源模型差距或为假象，因隐藏增强手段](#item-19)
20. [Claude Code 被指含间谍软件，针对中国用户](#item-20)

---

<a id="item-1"></a>
## [首个能生长分裂的合成细胞诞生](https://www.quantamagazine.org/for-the-first-time-a-cell-built-from-scratch-grows-and-divides-20260701/) ⭐️ 10.0/10

明尼苏达大学 Biotic 研究所的研究人员于 2026 年 7 月 1 日报告，他们创建了 SpudCell，这是首个从零构建并能生长分裂的合成细胞。 这一突破克服了合成生物学中实现最小细胞分裂的主要障碍，可能为生物技术、医学和基础研究设计定制细胞铺平道路。 SpudCell 仅包含 36 个基因，远少于实验室典型大肠杆菌的 4460 个基因，并通过一种避免需要细胞骨架的新型机制实现分裂。该研究最初被《细胞》期刊拒绝，随后以 190 页手稿直接向公众发布。

hackernews · defrost · 7月1日 14:20 · [社区讨论](https://news.ycombinator.com/item?id=48747304)

**背景**: 合成生物学的目标是通过组装最小基因组（生命所需的最小基因集）从无生命的化学物质中创造人造细胞。此前的里程碑包括 2010 年首个合成细菌细胞（JCVI-syn1.0），但这些细胞依赖于复杂的分裂过程。SpudCell 的发明者通过设计不同的分裂机制，绕过了通常分裂所需的关键结构组件——细胞骨架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SpudCell">SpudCell - Wikipedia</a></li>
<li><a href="https://www.nytimes.com/interactive/2026/07/01/science/spudcells-synthetic-cell.html">This Cell Feeds, Grows and Reproduces. And It’s Manmade.</a></li>
<li><a href="https://www.nytimes.com/2026/07/01/science/spud-cell-what-to-know.html">SpudCell: Scientists Made a Cell With Most of the Hallmarks ...</a></li>

</ul>
</details>

**社区讨论**: 评论者注意到非传统的公关策略，包括在发表前就建立了维基百科页面，并讨论了放弃细胞骨架的技术创新。一些人担心期刊拒稿和新闻保密期做法，而另一些人则称赞其开放性和里程碑意义。

**标签**: `#synthetic biology`, `#cell division`, `#breakthrough`, `#biotechnology`

---

<a id="item-2"></a>
## [Box3D 发布：开源 3D 物理引擎](https://box2d.org/posts/2026/06/announcing-box3d/) ⭐️ 9.0/10

Box2D 的创始人 Erin Catto 宣布了 Box3D，一款新的开源 3D 物理引擎。该发布在 Hacker News 上获得了 395 分和 86 条评论的广泛关注。 Box3D 将 Catto 成熟的物理模拟方法扩展到 3D，可能影响游戏开发、机器人模拟以及之前依赖 Box2D 的 2D 功能的机器学习环境。社区的高度参与表明对可靠的开源 3D 物理引擎的强烈需求。 虽然公告未明确说明确定性支持，但社区成员对网络应用中的确定性物理模拟表现出兴趣。评论者指出，该引擎在 3D 刚体模拟中面临碰撞检测和解析的固有挑战。

hackernews · makepanic · 7月1日 12:12 · [社区讨论](https://news.ycombinator.com/item?id=48745445)

**背景**: Box2D 是一个广泛使用的 2D 物理引擎，为许多独立游戏和模拟环境（包括 Angry Birds 物理）提供支持。它也是 OpenAI Gym 中流行的强化学习基准（如 Lunar Lander 和 Car Racing）的基础。Box3D 旨在将类似功能扩展到三维空间。

**社区讨论**: 社区评论表达了对 Box2D 在独立游戏中影响的兴奋和怀旧。用户如 Jeaye 希望获得用于网络游戏的确定性物理，而 adalacelove 警告 3D 物理模拟的复杂性。机器学习研究者 ainch 指出 Box2D 在强化学习环境中的重要性。

**标签**: `#physics engine`, `#open source`, `#game development`, `#Box2D`, `#simulation`

---

<a id="item-3"></a>
## [未修补的 Argo CD 漏洞可致 Kubernetes 集群被接管](https://thehackernews.com/2026/07/unpatched-argo-cd-repo-server-flaw.html) ⭐️ 9.0/10

Argo CD 的 repo-server 组件存在一个未修补的严重漏洞，允许未认证的攻击者执行任意代码并接管 Kubernetes 集群。该漏洞由 Synacktiv 发现并报告给维护者，但目前尚无修复补丁或 CVE 编号。 Argo CD 被广泛用于基于 GitOps 的 Kubernetes 部署，该漏洞可能导致在内部网络可达的情况下无需认证即可完全控制集群。由于没有补丁，依赖 Argo CD 管理关键基础设施的组织面临更高风险。 该漏洞位于 repo-server 组件中，只有当攻击者能够访问其内部网络端口时才可利用。Synacktiv 演示了该漏洞可导致完全接管 Kubernetes 集群，但目前尚无官方修复或 CVE 标识。

rss · The Hacker News · 7月1日 19:40

**背景**: Argo CD 是一个用于 Kubernetes 的声明式 GitOps 持续交付工具，广泛用于自动化应用部署。其 repo-server 组件负责从 Git 仓库克隆、缓存和生成清单。该组件中的未修补漏洞可能在内部网络端口暴露时导致远程代码执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://devopscube.com/argo-cd-architecture/">Argo CD Architecture: A Complete Guide</a></li>
<li><a href="https://argo-cd.readthedocs.io/en/latest/user-guide/commands/argocd_repo/">argocd repo Command Reference - Argo CD - Declarative GitOps CD ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#kubernetes`, `#argocd`

---

<a id="item-4"></a>
## [Adobe 修补 ColdFusion 和 Campaign Classic 中的 7 个 CVSS 10.0 严重漏洞](https://thehackernews.com/2026/07/adobe-patches-7-cvss-100-flaws-in.html) ⭐️ 9.0/10

Adobe 发布了针对 ColdFusion 和 Campaign Classic 中 7 个最高严重性漏洞（CVSS 10.0）的安全补丁，这些漏洞可能导致任意代码执行、权限提升和任意文件系统读取。 这些漏洞对依赖 ColdFusion 进行 Web 应用开发和 Campaign Classic 进行营销自动化的企业至关重要，成功利用可能导致系统完全受损。系统管理员必须立即应用补丁以防止潜在入侵。 ColdFusion 更新修复了包括任意代码执行和权限提升在内的多个漏洞，而 Campaign Classic 补丁解决了类似的最高严重性问题。所有七个漏洞的 CVSS 评分均为最高的 10.0。

rss · The Hacker News · 7月1日 15:25

**背景**: Adobe ColdFusion 是 1995 年推出的商用快速 Web 应用开发平台，用于构建动态网站并将 HTML 页面连接到数据库。Adobe Campaign Classic 是管理跨渠道营销活动的营销自动化平台。这两个产品在企业环境中广泛部署，使其成为攻击者的有利目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Adobe_ColdFusion">Adobe ColdFusion</a></li>
<li><a href="https://experienceleague.adobe.com/zh-hant/playlists/campaign-classic-v7-getting-started-for-business-users">Adobe Campaign Classic 企業使用者快速入門 | Adobe Campaign</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#adobe`, `#coldfusion`, `#vulnerabilities`, `#patching`

---

<a id="item-5"></a>
## [Cursor 严重漏洞可让提示注入逃逸沙箱](https://thehackernews.com/2026/07/critical-cursor-flaws-could-let-prompt.html) ⭐️ 9.0/10

Cursor AI 代码编辑器中发现两个严重漏洞（CVE-2026-50548 和 CVE-2026-50549，CVSS 9.8/9.3），统称为 DuneSlide，允许通过零点击提示注入绕过沙箱并在开发者机器上执行任意命令。 这些漏洞非常严重，因为 Cursor 被开发者广泛使用，且能在无需用户交互的情况下远程执行代码，对软件供应链构成严重安全风险。 这些漏洞由 Cato AI Labs 发现，无需用户点击或批准，影响 Cursor 的默认沙箱保护机制；攻击可通过一个看似普通的提示触发。

rss · The Hacker News · 7月1日 14:42

**背景**: 提示注入是一种攻击，诱使大型语言模型（LLM）忽略开发者指令而遵循攻击者控制的输入，可能导致意外行为。Cursor 是一款集成 LLM 以辅助编码的 AI 代码编辑器，它使用沙箱将模型命令与系统隔离。DuneSlide 漏洞打破了这种隔离，允许任意命令执行。这些漏洞凸显了随着 AI 工具获得代码执行能力而日益增长的安全挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/critical-cursor-flaws-could-let-prompt.html">Critical Cursor Flaws Could Let Prompt Injection Escape Sandbox and Run Commands</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>

</ul>
</details>

**标签**: `#security`, `#prompt injection`, `#Cursor`, `#AI code editor`, `#CVE`

---

<a id="item-6"></a>
## [幻影抢注：利用 AI 幻觉域名的攻击向量](https://unit42.paloaltonetworks.com/phantom-squatting-hallucinated-web-domains/) ⭐️ 9.0/10

Palo Alto Networks 的 Unit 42 发现了一种名为‘幻影抢注’的新型攻击向量，攻击者注册大语言模型幻觉生成的域名，用于托管钓鱼页面和恶意软件。 该攻击利用了 LLM 的幻觉特性——它们会编造听起来合理但实际不存在的域名，当 AI 工具将用户引导至这些攻击者控制的站点时，可能危及软件供应链安全。 Unit 42 研究人员发现，大语言模型会一致性地为合法品牌幻觉生成域名，攻击者可以抢先注册这些域名。每次新的 LLM 部署和代理 AI 能力的增强都会扩大攻击面。

rss · Unit 42 Threat Research · 7月1日 01:00

**背景**: 大语言模型会产生‘幻觉’，即生成不存在的虚假信息，包括不存在的网址。这种现象在 AI 研究中已有充分记录。幻影抢注是一种域名抢注攻击，类似于域名仿冒攻击，但利用的是 AI 生成的不准确性而非拼写错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://unit42.paloaltonetworks.com/phantom-squatting-hallucinated-web-domains/">Phantom Squatting: AI-Hallucinated Domains as a Software Supply Chain Vector</a></li>
<li><a href="https://thehackernews.com/2026/07/phantom-squatting-uses-ai-hallucinated.html">Phantom Squatting Uses AI-Hallucinated Domains for Phishing and Malware</a></li>
<li><a href="https://cybernews.com/security/phantom-squatting-hallucinated-domains-cyber-attacks/">AI “phantom squatting” fuels cyber attacks | Cybernews</a></li>

</ul>
</details>

**标签**: `#AI security`, `#supply chain attack`, `#LLM`, `#domain squatting`

---

<a id="item-7"></a>
## [索尼将于 2028 年停止生产实体游戏光盘](https://blog.playstation.com/2026/07/01/physical-disc-production-ending-in-january-2028-for-new-games-releasing-on-playstation-consoles/) ⭐️ 8.0/10

索尼宣布，新 PlayStation 游戏的实体光盘生产将于 2028 年 1 月停止，这标志着主机游戏实体媒体的终结。 这一重大行业转变引发了对数字所有权、游戏保存和消费者权益的担忧，因为一旦实体媒体消失，玩家可能失去拥有和转售游戏的能力。 该决定仅影响新游戏发行；现有实体光盘在库存耗尽前仍可购买。索尼此举发生在近期因无退款移除已购数字内容引发争议之后。

hackernews · Tiberium · 7月1日 12:13 · [社区讨论](https://news.ycombinator.com/item?id=48745456)

**背景**: 游戏行业正逐渐从实体发行转向数字发行，索尼和微软都在推广纯数字版主机。实体光盘允许玩家转售、借出和拥有游戏，不受在线服务限制，而数字购买往往带有严格的 DRM 和有限的消费者保护。实体生产线的关闭也可能影响蓝光市场，因为主机游戏曾是压片厂的重要收入来源。

**社区讨论**: 评论者表达强烈质疑和失望，引用索尼近期无退款移除已购电影的事件，证明数字所有权不可靠。许多人担心游戏保存问题及无法转售或交易数字游戏，一些人誓言如果实体媒体完全消失，他们将放弃游戏。

**标签**: `#PlayStation`, `#physical media`, `#digital ownership`, `#gaming industry`, `#game preservation`

---

<a id="item-8"></a>
## [FFmpeg 9.1 AAC 编码器质量修复](https://hydrogenaudio.org/index.php/topic,129691.0.html) ⭐️ 8.0/10

FFmpeg 9.1 包含了一个大幅改进的 AAC 编码器，修复了长期存在的质量问题（如啁啾伪影），并引入了更好的噪声整形和立体声处理。 此次更新为数以万计依赖 FFmpeg 内置 AAC 编码器进行视频录制、流媒体和转码的用户提升了音频质量，减少了对 Apple Core Audio 等外部编码器的需求。 该编码器针对 48 kHz 音频进行了优化，并绕过了 FFmpeg AAC 解码器中与立体声感知噪声替换（PNS）相关的错误。社区基准测试结果显示，新编码器与其他 AAC 编码器竞争良好，不过 Opus 在较低码率下仍表现更优。

hackernews · ledoge · 7月1日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48747116)

**社区讨论**: 社区成员赞赏了这一改进，但指出 Opus 在低码率下仍优于 AAC，并强调了编解码器评估中的主观因素。一名用户发现了 PNS 错误，另一名用户则质疑 48 kHz 是否已成为标准采样率。

**标签**: `#FFmpeg`, `#audio encoding`, `#AAC`, `#codec improvement`, `#open-source`

---

<a id="item-9"></a>
## [Cloudflare 推出基于 HTTP 402 的货币化网关](https://blog.cloudflare.com/monetization-gateway/) ⭐️ 8.0/10

Cloudflare 宣布推出 Monetization Gateway（货币化网关），允许客户对 Cloudflare 背后的任何资源（如网页、API、数据集、MCP 工具）进行收费，使用 HTTP 402 状态码并通过 x402 协议以稳定币结算。目前等待名单已开放。 这实现了数字资源的无摩擦微支付，可能改变 API 货币化模式，并为 AI 代理自动付费访问铺平道路。Cloudflare 的庞大规模可能推动此前微支付尝试未能实现的普及。 支付通过 x402 开放协议以稳定币结算，无需传统支付基础设施。该网关支持每次请求的微交易，并可应用于 Cloudflare 背后的任何资源。

hackernews · soheilpro · 7月1日 13:59 · [社区讨论](https://news.ycombinator.com/item?id=48746914)

**背景**: HTTP 402（Payment Required）是一个预留但从未广泛实现的状态码。x402 协议将其重新用于互联网原生支付标准，基于 Solana 构建以实现快速低成本的交易。这种方法旨在通过在协议层面处理结算来解决网络上长期存在的微支付问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/monetization-gateway/">Announcing the Monetization Gateway: charge for any resource behind Cloudflare via x402</a></li>
<li><a href="https://thedefiant.io/news/defi/cloudflare-monetization-gateway-x402-stablecoin-payments">Cloudflare Launches Monetization Gateway for Stablecoin Payments via x402 - "The Defiant"</a></li>
<li><a href="https://solana.com/x402/what-is-x402">What is x402? | Payment Protocol for AI Agents on Solana</a></li>

</ul>
</details>

**社区讨论**: 评论显示对 AI 代理实际微交易感到兴奋，但也提出了担忧：一位用户指出在机器人增加成本的同时保留免费人类体验的困难，另一位强调法律复杂性如发票和增值税，第三位则对 Cloudflare 实现临界规模持谨慎乐观态度。

**标签**: `#Cloudflare`, `#API monetization`, `#microtransactions`, `#HTTP 402`, `#web payments`

---

<a id="item-10"></a>
## [乐观提供：将 IPFS 内容发布速度提升 10 倍](https://probelab.io/blog/optimistic-provide/) ⭐️ 8.0/10

一篇来自 Probelab 的博客介绍了一种名为“乐观提供”的新优化，通过在大多数 PUT RPC 成功后将控制权返回给用户并异步处理剩余部分，使 IPFS 内容发布速度提升高达 10 倍。 这一优化通过降低感知延迟显著改善了 IPFS 内容发布者的体验，可能促进 IPFS 作为去中心化存储解决方案的更广泛采用。同时展示了分布式系统中一致性与速度之间的实际权衡。 这一名为“乐观提供”的优化修改了提供过程，在大多数（而非全部）PUT RPC 成功后就提前返回，剩余操作在后台继续执行。这与此前等待所有操作完成才返回的行为有所不同。

hackernews · dennis-tra · 7月1日 15:30 · [社区讨论](https://news.ycombinator.com/item?id=48748518)

**背景**: IPFS 是一种点对点分布式文件系统，使用内容寻址来存储和共享文件。当用户发布内容时，IPFS 节点通过将提供者记录存储到分布式哈希表（DHT）中向网络宣告该内容。提供过程涉及向不同对等节点发送多个 PUT RPC；此前节点需等待所有 RPC 完成，速度较慢。DHT 是 IPFS 内容路由的关键组件，使节点能通过内容标识符（CID）找到谁拥有某文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.ipfs.tech/concepts/dht/">Distributed Hash Tables ( DHT ) | IPFS Docs</a></li>
<li><a href="https://docs.ipfs.tech/quickstart/publish/">Publish a file with IPFS using a pinning service | IPFS Docs</a></li>
<li><a href="https://medium.com/@sevcsik/publishing-to-ipfs-b627b6c8799a">Publishing to IPFS . If you visited this site more than once | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论表达了几种不同的看法。有人质疑该优化是否真正提升了 10 倍速度，因为它只是将部分操作改为异步执行而非减少工作量。还有人质疑 IPFS 在生产环境中的实际使用情况，并指出过去的性能问题导致许多项目放弃使用 IPFS。也有建议认为，通过将网络拓扑编码到 PeerID 中进行架构改进可以提升查找速度。

**标签**: `#IPFS`, `#distributed systems`, `#performance optimization`, `#DHT`

---

<a id="item-11"></a>
## [Cursor 通过前部署工程师部署 AI 代理](https://www.latent.space/p/cursor-forward-deployed-engineers) ⭐️ 8.0/10

由 Pauline Brunet 领导的 Cursor 前部署工程师团队，帮助企业建立用于编码和部署的 AI 代理软件工厂。该模式将工程师直接嵌入客户环境，以定制 AI 解决方案。 这种方法解决了将 AI 代理集成到实际企业工作流中的难题，加速了 AI 在软件开发中的采用。它标志着从通用工具到定制化、亲手部署服务的转变。 前部署工程师（FDE）执行软件工程、销售和平台工程等混合任务。由于需要将 AI 解决方案集成到企业环境中，该角色最近需求增加。

rss · Latent Space · 7月1日 19:03

**背景**: 前部署工程师（FDE）是一种与客户紧密合作，在操作环境中开发、定制和部署技术解决方案的专业角色。该模式起源于 Palantir 等公司，现在被 Cursor 等 AI 初创公司采用，以帮助企业构建 AI 驱动的软件工厂。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Forward_Deployed_Engineer">Forward Deployed Engineer - Wikipedia</a></li>
<li><a href="https://newsletter.pragmaticengineer.com/p/forward-deployed-engineers">What are Forward Deployed Engineers, and why are they so in demand?</a></li>
<li><a href="https://factory.ai/">Factory | Agent -Native Software Development</a></li>

</ul>
</details>

**标签**: `#Cursor`, `#AI agents`, `#enterprise deployment`, `#software engineering`, `#AI-assisted coding`

---

<a id="item-12"></a>
## [PEARL 与药物发现中的共折叠精确度](https://www.latent.space/p/the-coolest-diffusion-research-isnt) ⭐️ 8.0/10

本文探讨了前 Meta Llama 负责人为何离开并加入 Genesis Molecular AI，强调了 PEARL 在 OpenBind 基准上的零样本胜利，并探索了当共折叠精确度跨越关键阈值时解锁的潜力。 这连接了前沿 AI 研究与实际药物发现，因为 PEARL 在蛋白质-配体复合物预测上超越了 AlphaFold 3，可能加速治疗设计。 PEARL 使用基于 SO(3)等变扩散架构，在大型合成数据上训练，实现了最先进的蛋白质-配体共折叠。OpenBind 基准提供了一个结构-亲和力数据集用于评估此类模型。

rss · Latent Space · 7月1日 14:42

**背景**: 扩散模型通过逆转噪声过程生成数据，已被应用于蛋白质结构预测。共折叠预测蛋白质-配体复合物的三维结构，对药物发现至关重要。AlphaFold 3 为此类预测设定了高标准，但 PEARL 声称在实际任务中超越了它。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.genesis.ml/news/introducing-pearl">Introducing Pearl: The Next Generation Foundation Model for ...</a></li>
<li><a href="https://arxiv.org/abs/2510.24670">[2510.24670] Pearl: A Foundation Model for Placing Every Atom ... Genesis Molecular AI | AI for Small Molecule Drug Discovery Pearl: A Foundation Model for Placing Every Atom in the Right ... NeurIPS Talk Pearl: A Foundation Model Advancing Small ... Placing Every Atom Right: PEARL's Deep Learning Approach to ...</a></li>
<li><a href="https://openbind.uk/news/blog-openbinds-first-release-a-structure-affinity-dataset-for-structure-based-ai/">Blog: OpenBind’s first release: A structure–affinity dataset for structure-based AI | openbind.uk</a></li>

</ul>
</details>

**标签**: `#AI`, `#diffusion models`, `#drug discovery`, `#protein design`, `#molecular biology`

---

<a id="item-13"></a>
## [Progress Kemp LoadMaster 预认证 RCE 漏洞正被积极利用](https://thehackernews.com/2026/07/latest-progress-kemp-loadmaster-pre.html) ⭐️ 8.0/10

据 eSentire 威胁响应部门报告，Progress Kemp LoadMaster 中存在一个严重的预认证远程代码执行漏洞（CVE-2026-8037，CVSS 9.6），目前正被积极利用。 该漏洞允许未经身份验证的攻击者在受影响的 LoadMaster 设备上执行任意命令，对依赖此负载均衡器保障应用可用性和性能的组织构成严重风险。 该漏洞是一个操作系统命令注入缺陷，CVSS 评分为 9.6，且无需任何预先身份验证即可在野外观察到利用尝试。

rss · The Hacker News · 7月1日 13:56

**背景**: Progress Kemp LoadMaster 是一款负载均衡器和应用交付控制器 (ADC)，用于将传入的网络流量分发到多台服务器，以确保应用的可用性、可扩展性和安全性。预认证远程代码执行 (RCE) 意味着攻击者无需有效凭据即可利用该漏洞，可能完全控制设备。CVE-2026-8037 是最近披露的漏洞，目前已确认遭到积极攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://labs.watchtowr.com/enterprise-tech-in-shell-out-progress-kemp-loadmaster-uninitialized-heap-to-pre-auth-rce-cve-2026-8037/">Enterprise Tech In, Shell Out (Progress Kemp LoadMaster Uninitialized Heap to Pre-Auth RCE CVE-2026-8037)</a></li>
<li><a href="https://docs.progress.com/bundle/loadmaster-product-overview-progress-kemp-loadmaster-ga/page/Introduction-to-Progress-Kemp-and-the-LoadMaster-Products.html">Introduction to Progress Kemp and the LoadMaster Products</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CVE`, `#RCE`, `#exploit`

---

<a id="item-14"></a>
## [AI 生成的勒索软件滥用 Chromium API 攻击 Windows 和 Android](https://thehackernews.com/2026/07/ai-generated-browser-ransomware-abuses.html) ⭐️ 8.0/10

网络安全研究人员发现首个有记录的案例，前沿 AI 模型 DeepSeek 生成了勒索软件，该软件滥用 Chromium API，完全在 Windows 和 Android 设备的浏览器内运行。 这标志着 AI 辅助恶意软件的一个重要里程碑，展示了高级 AI 能够将不切实际的浏览器恶意软件概念与真实的浏览器能力相结合，创造新的攻击路径，可能降低网络犯罪的门槛。 该勒索软件完全在浏览器内运行，无需传统可执行文件，支持 Windows 和 Android 双平台，是首个已知的前沿 AI 模型生成此类跨平台浏览器勒索软件的案例。

rss · The Hacker News · 7月1日 12:59

**背景**: DeepSeek 是一家中国 AI 公司，开发大型语言模型，例如参数达 6710 亿的混合专家模型 DeepSeek-V3。Chromium 是支撑 Google Chrome 及其他浏览器的开源浏览器项目，提供可被 Web 应用访问的 API。此事件突显了 AI 如何被滥用，利用合法的浏览器功能实现恶意目的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://developer.chrome.com/docs/chromium">Chromium | Chrome for Developers</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#ransomware`, `#AI`, `#Chromium`, `#malware`

---

<a id="item-15"></a>
## [微软将后量子密码迁移时间提前至 2029 年](https://thehackernews.com/2026/07/microsoft-accelerates-post-quantum.html) ⭐️ 8.0/10

微软宣布将后量子密码迁移的最后期限提前至 2029 年，理由是量子计算技术取得快速进展。该公司 Azure 首席技术官表示，风险时间线已经改变，提前迁移至关重要。 这一加速表明，主要科技公司认为能够破解当前加密的量子计算机可能比预期更早到来。这给全球组织带来了压力，要求他们更早开始迁移到抗量子算法，以保护敏感数据免受未来威胁。 新的 2029 年截止日期适用于微软自身的基础设施和云服务，该公司敦促客户立即开始规划。此举与美国国家标准与技术研究院（NIST）在 2024 年发布的首批后量子密码标准保持一致。

rss · The Hacker News · 7月1日 10:41

**背景**: 后量子密码学（PQC）是指旨在抵抗经典计算机和量子计算机攻击的密码算法。当前广泛使用的公钥算法（如 RSA 和 ECC）依赖于数学难题，而 Shor 算法能在足够强大的量子计算机上解决这些问题。虽然此类量子计算机尚未存在，但专家警告存在'先收割，后解密'的攻击方式，即加密数据被存储以待未来解密。NIST 一直主导 PQC 算法标准化工作，并于 2024 年发布了三个最终标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography</a></li>
<li><a href="https://csrc.nist.gov/projects/post-quantum-cryptography">Post-Quantum Cryptography | CSRC</a></li>

</ul>
</details>

**标签**: `#post-quantum cryptography`, `#Microsoft`, `#quantum computing`, `#cybersecurity`, `#encryption`

---

<a id="item-16"></a>
## [Azure CLI 密码喷洒攻击致 78 个微软账户失陷](https://thehackernews.com/2026/07/azure-cli-password-spray-hits-at-least.html) ⭐️ 8.0/10

一场针对微软 Azure CLI 的持续性自动化密码喷洒攻击在 6 月 12 日至 26 日期间产生了超过 8100 万次登录尝试，至少导致 78 个账户被攻破。攻击流量来自互联网基础设施提供商 LSHIY LLC（AS32167）控制的 IPv6 地址段（2a0a:d683::/32）。 此次大规模攻击凸显了针对云基础设施（尤其是 Azure CLI 等开发工具）的自动化凭据攻击威胁日益增长。依赖 Azure 的组织必须紧急实施多因素认证并监控异常认证模式。 攻击采用密码喷洒技术，对大量账户尝试少量常见密码以规避账户锁定。Huntress 研究人员识别出该恶意活动并将其关联到与 LSHIY LLC 相关的 IPv6 子网 2a0a:d683::/32。

rss · The Hacker News · 7月1日 05:46

**背景**: 密码喷洒攻击是一种暴力破解技术，攻击者对大量账户尝试少量常用密码，而不是对单个账户尝试大量密码。Azure CLI 是微软用于管理 Azure 资源的跨平台命令行工具。此类攻击利用弱密码或重复使用的密码，若未适当监控则往往能逃避检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huntress.com/blog/hunting-for-m365-password-spraying">Password Spraying Tools: How Attackers Spray M365 | Huntress</a></li>
<li><a href="https://learn.microsoft.com/en-us/cli/azure/install-azure-cli-windows?view=azure-cli-latest">Install the Azure CLI on Windows | Microsoft Learn</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#azure`, `#password spray`, `#microsoft`, `#cloud security`

---

<a id="item-17"></a>
## [ChocoPoC 恶意软件通过虚假 PoC 漏洞利用代码攻击研究人员](https://www.bleepingcomputer.com/news/security/new-chocopoc-malware-targets-researchers-via-trojanized-poc-exploits/) ⭐️ 8.0/10

一项新的恶意软件活动通过托管在 GitHub 上的被木马化的概念验证（PoC）漏洞利用代码，传播名为 ChocoPoC 的基于 Python 的远程访问木马（RAT），目标针对网络安全研究人员。 该攻击直接针对发现漏洞至关重要的网络安全研究人员，削弱了对 PoC 代码仓库的信任，并可能危及敏感的研究数据和系统。 ChocoPoC 远程访问木马用 Python 编写，能够执行任意命令、窃取敏感数据，并为攻击者提供远程访问基础设施的能力。

rss · BleepingComputer · 7月1日 20:08

**背景**: 概念验证（PoC）漏洞利用代码是展示如何利用漏洞的代码示例，通常由安全研究人员分享。远程访问木马（RAT）允许攻击者远程控制受感染的机器。这场活动显示了威胁行为者将 PoC 代码武器化以感染同行研究人员，这种趋势在之前的攻击中也有出现，例如针对 RegreSSHion 漏洞的攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/chocopoc-malware-delivered-via-trojanized-exploits-on-github/">ChocoPoc malware delivered via trojanized exploits on GitHub</a></li>
<li><a href="https://www.helpnetsecurity.com/2025/12/23/fake-poc-exploits-webrat-malware/">Budding infosec pros and aspiring cyber crooks targeted with fake PoC exploits - Help Net Security</a></li>
<li><a href="https://thehackernews.com/2024/12/390000-wordpress-credentials-stolen-via.html">390,000+ WordPress Credentials Stolen via Malicious GitHub Repository Hosting PoC Exploits</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#GitHub`, `#RAT`, `#cybersecurity`

---

<a id="item-18"></a>
## [美国国土安全部确认黑客入侵 HSIN 信息共享平台](https://www.bleepingcomputer.com/news/security/dhs-confirms-hackers-breached-hsin-info-sharing-platform/) ⭐️ 8.0/10

美国国土安全部已确认，黑客攻破了国土安全信息网络（HSIN），该平台用于在联邦、州、地方及私营部门伙伴之间共享敏感但非机密的信息。 此次入侵构成重大安全风险，因为 HSIN 是协调国土安全行动和共享威胁情报的关键工具。它可能削弱对政府信息共享系统的信任，并可能使敏感数据暴露给对手。 美国国土安全部官员确认了此次入侵，但未透露关于入侵程度、被访问数据以及攻击者身份的具体细节。调查正在进行中。

rss · BleepingComputer · 7月1日 17:32

**背景**: 国土安全信息网络（HSIN）是由美国国土安全部运营的基于 Web 的平台，使各种政府机构和私营部门伙伴之间能够可信地共享敏感但非机密（SBU）信息。它用于支持反恐、网络安全和灾害响应工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Homeland_Security_Information_Network">Homeland Security Information Network - Wikipedia</a></li>
<li><a href="https://www.dhs.gov/homeland-security-information-network-hsin">Homeland Security Information Network (HSIN) | Homeland Security</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#government`, `#data breach`, `#HSIN`

---

<a id="item-19"></a>
## [闭源与开源模型差距或为假象，因隐藏增强手段](https://www.reddit.com/r/LocalLLaMA/comments/1ukp2bu/the_gap_between_closed_and_open_models_might_be/) ⭐️ 8.0/10

一篇 Reddit 帖子指出，像 Claude 这样的闭源模型在基准测试中表现优越，可能并非仅因模型架构更好，而是因为其背后使用了未公开的增强手段，如 RAG、提示预处理和隐藏工具调用，导致与开源模型的比较不公平。 这挑战了闭源模型本质上更优越的普遍假设，呼吁更透明的评估方法，可能改变 AI 社区解读基准测试结果和分配资源的方式。 帖子特别指出，Anthropic 会隐去推理轨迹，并可能使用 RAG、知识注入、上下文相关系统提示以及“小丑车 MoE”（将查询路由到专门的专家模型）等技术，这些都能在不暴露真实模型能力的情况下提升表面性能。

reddit · r/LocalLLaMA · /u/-p-e-w- · 7月1日 15:35

**背景**: 检索增强生成（RAG）是一种让大语言模型在生成回答前先从外部获取相关信息的技术，能提升准确性。混合专家模型（MoE）使用多个专门的子模型，每次仅激活其中一部分。“小丑车 MoE”这个说法幽默地指代动态调用大量小型专家模型的做法，就像小丑从小车里涌出。如果这些增强手段隐藏在 API 背后，会让模型在原始推理能力未被知晓的情况下显得强大得多。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation - Wikipedia</a></li>
<li><a href="https://aws.amazon.com/what-is/retrieval-augmented-generation/">What is RAG? - Retrieval-Augmented Generation AI Explained - AWS</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-mixture-of-experts">A Visual Guide to Mixture of Experts ( MoE )</a></li>

</ul>
</details>

**标签**: `#closed models`, `#open models`, `#benchmarking`, `#RAG`, `#AI evaluation`

---

<a id="item-20"></a>
## [Claude Code 被指含间谍软件，针对中国用户](https://www.reddit.com/r/LocalLLaMA/comments/1ukkz9a/non_us_ally_should_be_afraid/) ⭐️ 8.0/10

Reddit 上的一篇帖子声称 Anthropic 的 Claude Code 中存在类似间谍软件的代码，秘密针对中国用户。 如果这一指控属实，将严重破坏对 AI 工具的信任，并可能加剧地缘政治紧张局势，影响全球用户隐私和企业采用。 该指控未经证实，源自一条 Reddit 帖子，目前尚未有 Anthropic 的官方回应。Claude Code 是一个 AI 编程代理，可根据自然语言指令读取代码库并编辑文件。

reddit · r/LocalLLaMA · /u/zakadit · 7月1日 12:57

**背景**: Claude Code 是 Anthropic 开发的一款工具，集成在终端、IDE 和浏览器中，用于辅助软件开发。Anthropic 以其“宪法 AI”方法著称，旨在使模型符合伦理准则。该工具此前已引发争议：美国联邦机构因 Anthropic 拒绝取消其合同中关于禁止大规模监控和自主武器的条款，已开始逐步淘汰 Claude。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**标签**: `#AI`, `#ethics`, `#security`, `#spyware`, `#Claude`

---