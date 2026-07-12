---
layout: default
title: "Horizon Summary: 2026-07-12 (ZH)"
date: 2026-07-12
lang: zh
---

> 从 28 条内容中筛选出 11 条重要资讯。

---

1. [vLLM v0.25.0：Model Runner V2 成为默认，移除旧版 PagedAttention](#item-1)
2. [jscrambler 8.14.0 npm 发布版遭篡改，植入 Rust 信息窃取器](#item-2)
3. [Ghostcommit 攻击在 PNG 图片中隐藏提示注入以窃取机密](#item-3)
4. [GPU 云热潮中的循环融资](#item-4)
5. [Zimbra 严重存储型 XSS 漏洞可通过邮件执行代码](#item-5)
6. [别再说「去问大模型」了](#item-6)
7. [ClickHouse 将 PgBouncer 吞吐量提升 4 倍](#item-7)
8. [推荐在 SQLite 中使用严格表](#item-8)
9. [黑客在多方间谍活动中针对俾路支省警察](#item-9)
10. [澳大利亚警告全球运动瞄准易受攻击的 CMS](#item-10)
11. [使用任意数量 VPN 隧道扫描恶意网站（第二部分）](#item-11)

---

<a id="item-1"></a>
## [vLLM v0.25.0：Model Runner V2 成为默认，移除旧版 PagedAttention](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 将 Model Runner V2 设为所有稠密模型的默认执行路径，移除了旧版 PagedAttention，并使 Transformers 后端达到与原生性能相同的水平。本次发布包含来自 232 位贡献者的 558 次提交，并新增了对 LLaVA-OneVision-2 和 GLM-5 等模型的支持。 此版本标志着 vLLM 架构的一个重要里程碑，简化了代码库并提升了性能。移除旧版 PagedAttention 以及 Model Runner V2 的成熟使得 vLLM 更易于维护且更高效，惠及整个开源 LLM 部署生态系统。 Model Runner V2 现在支持 EVS、实时嵌入、Mamba 混合模型的前缀缓存以及基于完整 CUDA 图的动态推测解码。Transformers 后端新增了 FP8 MoE 支持，并迁移了 GPTBigCode 和 RoBERTa 等额外模型架构。

github · khluu · 7月11日 20:06

**背景**: vLLM 是一个用于高吞吐量 LLM 推理的开源库，最初基于 PagedAttention 构建，这是一种通过分页高效管理 KV 缓存的自定义注意力机制。Model Runner V2 是一个重新设计的执行核心，采用模块化的模型逻辑和 GPU 原生的输入准备方式，解决了 V1 中的技术债务。此版本用更现代的 MRv2 后端取代了旧版 PagedAttention。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/stable/design/paged_attention/">Paged Attention - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>

</ul>
</details>

**标签**: `#vllm`, `#llm-inference`, `#open-source`, `#ai-engineering`, `#performance`

---

<a id="item-2"></a>
## [jscrambler 8.14.0 npm 发布版遭篡改，植入 Rust 信息窃取器](https://thehackernews.com/2026/07/compromised-jscrambler-8140-npm-release.html) ⭐️ 9.0/10

jscrambler npm 包 8.14.0 版本被破坏，嵌入了一个 preinstall 钩子，该钩子会在 Windows、macOS 和 Linux 系统上下载并执行一个基于 Rust 的信息窃取器。该恶意版本于 2026 年 7 月 11 日发布，并在六分钟内被 Socket 标记。 此事件凸显了 npm 生态系统中供应链攻击的严重风险，尤其是对于广泛使用的开发工具。任何安装了 8.14.0 版本的开发者都可能面临凭据、密钥等敏感数据被盗的风险，可能影响数千个项目。 恶意包包含分别针对 Windows、macOS 和 Linux 的独立原生二进制文件，使用 Rust 编写。preinstall 钩子在 npm install 期间自动执行二进制文件，无需任何显式的安装脚本调用。此攻击被 Socket 安全检测并报告，但在此之前安装的用户可能已被入侵。

rss · The Hacker News · 7月11日 17:59

**背景**: npm 包可以定义 preinstall 脚本，在安装前自动运行，常用于编译或设置。供应链攻击破坏受信任的包，向下游用户分发恶意软件。Jscrambler 是一个代码混淆工具，许多开发者用于保护 JavaScript 应用程序。使用 Rust 二进制文件使恶意软件更难以分析且跨平台兼容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.npmjs.com/package/jscrambler">jscrambler - npm</a></li>
<li><a href="https://socket.dev/">Socket - Block zero-day supply chain attacks</a></li>
<li><a href="https://docs.npmjs.com/cli/v8/using-npm/scripts/?v=true">scripts - npm Docs</a></li>

</ul>
</details>

**标签**: `#security`, `#npm`, `#supply chain attack`, `#malware`, `#jscrambler`

---

<a id="item-3"></a>
## [Ghostcommit 攻击在 PNG 图片中隐藏提示注入以窃取机密](https://www.bleepingcomputer.com/news/security/ghostcommit-hides-prompt-injection-in-images-to-fool-ai-agents-steal-secrets/) ⭐️ 9.0/10

研究人员展示了 Ghostcommit 攻击，该攻击在 PNG 图片中嵌入提示注入，当 AI 代码审查员处理该图片时，会诱骗编码代理读取仓库的.env 文件，并将机密以数字列表的形式写入代码以泄密。 该攻击绕过了从未打开图片文件的 CodeRabbit 和 Bugbot 等 AI 代码审查员，然后利用对 AI 代理的信任窃取敏感机密，凸显了 AI 驱动的供应链安全中的关键漏洞。 该攻击使用隐写术将恶意提示隐藏在 PNG 的最低有效位中，并且成功针对了 CodeRabbit 和 Bugbot，这些工具从不直接处理图片文件，但编码代理会处理。注入的提示指示代理读取.env 文件并将机密输出为数字以绕过检测。

rss · BleepingComputer · 7月11日 09:03

**背景**: 提示注入攻击利用了大语言模型（LLM）无法区分开发者指令和用户输入的弱点。间接提示注入发生在恶意提示被嵌入 LLM 检索的内容（如网页或图片）中。隐写术是将数据隐藏在其他数据中的技术，例如将文本隐藏在图像像素的最低有效位中以避免检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://docs.coderabbit.ai/">CodeRabbit Documentation - AI code reviews on pull requests, IDE, and CLI</a></li>
<li><a href="https://luhko.github.io/articles/png_struct_stegano/">PNG files : structure and Steganography | Luhko</a></li>

</ul>
</details>

**标签**: `#security`, `#prompt injection`, `#AI agents`, `#code review`, `#supply chain`

---

<a id="item-4"></a>
## [GPU 云热潮中的循环融资](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

一项分析揭示，英伟达对 CoreWeave 和 Nebius 等新型云服务商的投资，被后者用于购买英伟达 GPU，形成了引发可持续性担忧的循环融资结构。 这种循环融资模式可能人为推高 GPU 需求，掩盖 AI 云服务商的真实盈利能力，可能影响投资者以及更广泛的人工智能基础设施生态系统。 社区评论指出，英伟达对 CoreWeave 的 20 亿美元投资仅占其 2026 年资本支出的 5.7%，表明循环融资可能被夸大。讨论还聚焦于每代币 ROI 和企业代币预算等替代指标。

hackernews · adletbalzhanov · 7月11日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48873836)

**背景**: 循环融资指投资者向客户提供资金，客户再用这些资金购买投资者的产品，形成自我强化的循环。在 GPU 云市场中，英伟达投资于购买英伟达 GPU 的新型云服务商，既提振了英伟达的营收，也可能虚增了这些云服务商的增长表象。随着 AI 热潮推动大规模基础设施支出，这种做法引发了关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom">Nvidia, CoreWeave, and Nebius: Inside the Circular Financing ...</a></li>
<li><a href="https://www.spheron.network/blog/nvidia-neocloud-backstop-financing-circular-gpu-2026/">NVIDIA's Neocloud Backstop Financing Explained: What Circular ...</a></li>
<li><a href="https://seekingalpha.com/article/4915653-nvidia-coreweave-and-nebius-inside-the-circular-financing-of-the-gpu-boom">Nvidia, CoreWeave, And Nebius: Inside The Circular Financing ...</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：一些人认为考虑到英伟达投资规模相对较小，循环融资的说法被夸大了；另一些人则将焦点转向代币 ROI 和利用率等盈利指标。还有用户指出这是英伟达对超大规模厂商自研芯片的战略对冲。

**标签**: `#gpu`, `#cloud-computing`, `#nvidia`, `#ai-infrastructure`, `#finance`

---

<a id="item-5"></a>
## [Zimbra 严重存储型 XSS 漏洞可通过邮件执行代码](https://thehackernews.com/2026/07/critical-zimbra-flaw-could-let-crafted_0483473395.html) ⭐️ 8.0/10

Zimbra 披露了其 Classic Web Client 中的一个严重存储型跨站脚本（XSS）漏洞，该漏洞允许特制邮件在用户会话中执行任意代码，并敦促客户立即应用补丁。 由于 Zimbra 广泛部署于企业和服务提供商，此漏洞构成了重大安全风险，攻击者可能无需用户交互即可窃取会话令牌、访问敏感数据或篡改账户。 该漏洞是存在于 Zimbra Classic Web Client 中的存储型 XSS 漏洞，尚未分配 CVE 编号。利用该漏洞需要受害者在 Classic Web Client 界面中查看恶意邮件。

rss · The Hacker News · 7月11日 06:45

**背景**: Zimbra 是一款广泛使用的开源电子邮件与协作平台，被全球众多组织采用。Classic Web Client 是其功能丰富的网页界面，提供邮件、日历和任务管理。存储型跨站脚本（XSS）是一种安全漏洞，攻击者注入的恶意脚本会被永久存储在服务器上，当其他用户访问受影响页面时执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zimbra.github.io/documentation/zimbra-10/classic-user-guide.html">User’s Guide for Zimbra Classic Web App</a></li>
<li><a href="https://owasp.org/www-community/attacks/xss/">Cross Site Scripting ( XSS ) | OWASP Foundation</a></li>

</ul>
</details>

**标签**: `#security`, `#Zimbra`, `#XSS`, `#vulnerability`, `#email`

---

<a id="item-6"></a>
## [别再说「去问大模型」了](https://blog.yaelwrites.com/stop-telling-me-to-ask-an-llm/) ⭐️ 7.0/10

一篇博客文章批评了随口建议「去问大模型」的做法，认为这种回应忽视了提问者之前付出的努力和具体情境，并呼吁更周全的沟通方式。 这凸显了技术社区中效率与同理心之间日益加剧的摩擦，影响着帮助的给予和接收方式。它促使人们反思在 AI 辅助环境下的沟通规范。 作者表示在求助之前已经咨询过 Claude，而「去问大模型」的建议感觉像是敷衍而非真诚的帮助。文章以「Let Me Google That For You」为例进行类比。

hackernews · theorchid · 7月11日 22:28 · [社区讨论](https://news.ycombinator.com/item?id=48876441)

**背景**: 建议别人去问大模型的现象，类似于早期的「LMGTFY」（Let Me Google That For You，意为「让我帮你谷歌一下」）趋势——人们会指引提问者去用搜索引擎，而不是直接回答。这种方式或许高效，但当提问者已经做过研究时，往往显得敷衍。文章倡导在给出建议之前先询问对方已经尝试过哪些方法。

**社区讨论**: 评论者普遍认同这一批评，建议提问者事先说明已经做过的研究，或者回应者先询问大模型给了什么回答。也有人指出，有时专家确实认为大模型能给出更好的答案。

**标签**: `#LLM`, `#communication`, `#tech community`, `#help-seeking`, `#AI`

---

<a id="item-7"></a>
## [ClickHouse 将 PgBouncer 吞吐量提升 4 倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 7.0/10

ClickHouse 通过实现 SO_REUSEPORT 套接字分片和进程对等（peering）等系统级优化，将 PostgreSQL 连接池 PgBouncer 的吞吐量提升了 4 倍。 这一显著的性能提升有助于在不扩展硬件的情况下处理更多并发连接，对于依赖 PostgreSQL 的高流量应用至关重要。这些优化广泛适用于其他连接池和网络服务。 优化包括使用 SO_REUSEPORT 允许多个 PgBouncer 进程共享同一端口，以及进程对等以便将取消请求高效转发到正确的进程。这些更改针对 ClickHouse Managed Postgres 所使用的 PgBouncer 配置。

hackernews · saisrirampur · 7月11日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是一个轻量级的 PostgreSQL 连接池，用于管理数据库连接以减少开销。传统上它作为单个进程运行，在高负载下可能成为瓶颈。SO_REUSEPORT 是一个 Linux 套接字选项，允许多个套接字绑定到同一端口，使内核能够将传入连接分发到多个工作进程。进程对等确保查询取消等可能落在任意进程上的请求被转发到正确的进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.f5.com/company/blog/nginx/socket-sharding-nginx-release-1-9-1">Socket Sharding in NGINX Release 1.9.1 | F5</a></li>
<li><a href="https://man7.org/linux/man-pages/man7/socket.7.html">socket (7) - Linux manual page</a></li>

</ul>
</details>

**社区讨论**: 社区评论中对 Odyssey 和 pgdog 等替代方案表现出兴趣，并询问对等机制的设置简便性。在 Kubernetes 上运行 PgBouncer 的用户发现使用多进程很简单，而其他人则询问 SO_REUSEPORT 和对等配置的更多细节。

**标签**: `#postgresql`, `#pgbouncer`, `#scaling`, `#connection-pooling`, `#performance`

---

<a id="item-8"></a>
## [推荐在 SQLite 中使用严格表](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 7.0/10

一篇博文推荐在 SQLite 中使用 STRICT 模式来强制类型安全，以对抗 SQLite 默认的灵活类型行为。 这很重要，因为许多来自其他 SQL 数据库的开发者对 SQLite 缺乏类型强制感到惊讶，改用严格表可以防止数据损坏并提高生产系统的可靠性。 严格表自 SQLite 3.37.0 版本（2021-11-27）起可用，并通过 STRICT 关键字以表为单位启用。但严格模式下不支持 DATE 等类型。

hackernews · ingve · 7月11日 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48873940)

**背景**: SQLite 传统上使用灵活的类型系统，不强制列类型，允许插入任何值而不考虑声明的类型。这是有意设计的，在 SQLite 的《灵活类型的优势》页面中有说明。为了满足传统严格类型强制的要求，添加了 STRICT 模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite.org/stricttables.html">STRICT Tables - SQLite</a></li>
<li><a href="https://evanhahn.com/prefer-strict-tables-in-sqlite/">Prefer STRICT tables in SQLite - evanhahn.com</a></li>

</ul>
</details>

**社区讨论**: 社区讨论显示了不同的意见。一些开发者强烈支持将 STRICT 设为默认值，而另一些人则指出 SQLite 官方对灵活类型的理由。有人承认 SQLite 的主要用例是嵌入式数据库，灵活类型可以接受，但对于共享数据库，严格类型更受青睐。

**标签**: `#SQLite`, `#databases`, `#type safety`, `#software engineering`, `#best practices`

---

<a id="item-9"></a>
## [黑客在多方间谍活动中针对俾路支省警察](https://thehackernews.com/2026/07/hackers-weaponize-balochistan-police.html) ⭐️ 7.0/10

网络安全研究人员披露了一场持续两年多的间谍活动，疑似中国和印度关联的威胁行为者针对巴基斯坦执法机构，攻陷了俾路支省警察数据门户。 这一事件突显了执法机构基础设施面临的网络间谍威胁日益严重，来自敌对国家的国家关联行为者瞄准敏感的警察和公民数据，可能为未来行动或破坏稳定提供便利。 被攻陷的资产包括托管管理警察和公民数据（如犯罪记录）的网络应用的服务器。该活动涉及多个威胁行为者团体，表明复杂的地缘政治竞争。

rss · The Hacker News · 7月11日 17:49

**背景**: 高级持续性威胁（APT）是一种隐蔽的网络攻击，攻击者获得并保持对目标网络的未授权访问，通常长期不被发现。国家支持的 APT 团体通常专注于间谍活动以窃取敏感数据，而不是造成直接破坏。这则新闻突显了此类战术针对执法机构的使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advanced_persistent_threat">Advanced persistent threat - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cyber espionage`, `#threat actors`, `#law enforcement`, `#Pakistan`, `#APT`

---

<a id="item-10"></a>
## [澳大利亚警告全球运动瞄准易受攻击的 CMS](https://www.bleepingcomputer.com/news/security/australia-warns-of-global-campaign-targeting-vulnerable-cms-platforms/) ⭐️ 7.0/10

澳大利亚网络安全中心（ACSC）发布警告，称一场全球性利用运动正在针对易受攻击的内容管理系统（CMS）及其插件。 这一警告来自国家网络机构，表明威胁可信度高，可能影响全球无数网站，敦促管理员立即修补漏洞。 ACSC 警告指出，攻击者正在积极利用 CMS 平台和插件中的已知漏洞，可能导致数据窃取或网站篡改。

rss · BleepingComputer · 7月11日 14:18

**背景**: 内容管理系统（CMS）如 WordPress、Joomla 和 Drupal 广泛用于构建和管理网站。插件扩展了功能，但若不及时更新常会引入安全漏洞。攻击者扫描未打补丁的网站以获取未授权访问。

**标签**: `#cybersecurity`, `#CMS`, `#vulnerability`, `#exploitation`, `#Australia`

---

<a id="item-11"></a>
## [使用任意数量 VPN 隧道扫描恶意网站（第二部分）](https://www.reddit.com/r/netsec/comments/1uto85z/scanning_malicious_websites_with_arbitrary_number/) ⭐️ 7.0/10

该帖子描述了一种使用任意数量 VPN 隧道扫描恶意网站的技术，旨在提高匿名性和可扩展性。 这项技术很重要，因为它可以让研究人员在不暴露真实 IP 地址的情况下扫描危险网站，从而显著增强威胁情报能力，同时还能更高效地处理大规模扫描。 该方法依赖于 VPN 链式连接，即流量按顺序经过多个 VPN 隧道，使得恶意网站难以检测或阻止扫描器。

reddit · r/netsec · /u/moonlightelite · 7月11日 16:13

**背景**: VPN 在用户设备和服务器之间建立加密隧道，隐藏用户 IP 地址并保护数据安全。多跳 VPN 通过链式连接多个 VPN 服务器，让流量经过多个中继节点，从而进一步增强匿名性。该技术将这种多跳 VPN 链式连接应用于网页扫描，使扫描器能够从不同 IP 地址出现并避免被检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nordlayer.com/learn/vpn/types-and-protocols/">Types of VPN , Protocols and When to Use Them | NordLayer</a></li>
<li><a href="https://www.comparitech.com/blog/vpn-privacy/multi-hop-vpn/">What is a multi - hop VPN and do you need one?</a></li>
<li><a href="https://www.activateprotection.com/network-security-features-vpn-chaining">VPN Chaining : Understanding the Benefits and Security Features</a></li>

</ul>
</details>

**标签**: `#security`, `#VPN`, `#web scanning`, `#malicious websites`, `#network security`

---