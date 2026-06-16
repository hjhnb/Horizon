---
layout: default
title: "Horizon Summary: 2026-06-16 (ZH)"
date: 2026-06-16
lang: zh
---

> 从 77 条内容中筛选出 20 条重要资讯。

---

1. [领英求职邀请中的后门利用 npm prepare 脚本](#item-1)
2. [Salesforce 以 36 亿美元收购前 Intercom 旗下的 Fin](#item-2)
3. [LiteLLM 漏洞链允许低权限用户完全接管服务器](#item-3)
4. [SearchLeak 攻击将 Microsoft 365 Copilot 变为数据窃取工具](#item-4)
5. [vLLM 0.23.0：DeepSeek-V4 强化，MRv2 扩展](#item-5)
6. [Iroh 1.0 发布：用拨号键而非 IP 地址](#item-6)
7. [黑客新闻用户分享本地 LLM 编码体验](#item-7)
8. [Hetzner 云服务器价格因硬件成本飙升而涨至三倍](#item-8)
9. [TimescaleDB 时间序列压缩技术深度解析](#item-9)
10. [福克斯据报道收购 Roku 引发整合担忧](#item-10)
11. [分析内存安全 CVE：Rust 与 C/C++的细微差别](#item-11)
12. [Typst 0.15.0 发布，支持多参考文献列表](#item-12)
13. [中国黑客利用 Google Workspace 规则窃取电子邮件](#item-13)
14. [WordPress 插件脚本被篡改，植入隐藏后门](#item-14)
15. [Palo Alto 警告 PAN-OS VPN 漏洞正被积极利用](#item-15)
16. [思科修复 Catalyst SD-WAN 管理器零日漏洞](#item-16)
17. [Infinite Campus 数据泄露影响 13.7 万学校员工账户](#item-17)
18. [CISA 将两个已被积极利用的漏洞添加到 KEV 目录](#item-18)
19. [朝鲜黑客利用开发者工具传播恶意软件](#item-19)
20. [每周安全回顾：Chrome 零日、UniFi 漏洞、macOS 窃密软件、VPN 缺陷](#item-20)

---

<a id="item-1"></a>
## [领英求职邀请中的后门利用 npm prepare 脚本](https://roman.pt/posts/linkedin-backdoor/) ⭐️ 9.0/10

一名求职者发现了一个隐藏的 GitHub 仓库后门，该仓库由招聘人员通过领英发送。后门利用 npm 的 prepare 生命周期脚本，在受害者运行 npm install 时执行任意代码。 此次攻击揭示了一种针对求职者（尤其是科技行业）的新型社会工程学攻击途径。同时也凸显了 npm 自动执行脚本功能的危险性——这一直是供应链安全的长期风险。 招聘人员发送了一个公开的 GitHub 仓库，并要求受害者检查一个“已弃用的 Node 模块问题”。有效载荷隐藏在注释掉的测试中，并通过 prepare 脚本执行。npm 在 npm install 后自动运行 prepare，因此仅安装依赖项就会执行后门。

hackernews · lwhsiao · 6月15日 20:00 · [社区讨论](https://news.ycombinator.com/item?id=48546294)

**背景**: npm 的 prepare 生命周期脚本会在 npm install 后自动执行（针对 git、文件和链接依赖），此前已被用于供应链攻击。2026 年 5 月，GitHub 和 npm 近期做出更改，默认阻止安装和 prepare 脚本的自动执行，但许多旧版或未修补的环境仍然存在风险。npm 生态系统经历了多起供应链攻击，包括维护者账号被攻陷和域名抢注活动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infoworld.com/article/4183849/github-finally-pulls-the-plug-on-automatic-install-script-execution-for-npm.html">GitHub finally pulls the plug on automatic install script execution for npm | InfoWorld</a></li>
<li><a href="https://cybernews.com/security/npm-packages-with-millions-downloads-compromised/">Hundreds of NPM packages compromised in a new supply chain attack | Cybernews</a></li>

</ul>
</details>

**社区讨论**: 评论者对领英和 GitHub 在求职中的作用表示不满，并呼吁建立更好的网络犯罪举报渠道。一些人指出，这种攻击与正常的面试任务非常相似，因此对疲惫或急于求职的人来说是一个危险的陷阱。

**标签**: `#security`, `#social-engineering`, `#npm`, `#job-scam`, `#supply-chain-attack`

---

<a id="item-2"></a>
## [Salesforce 以 36 亿美元收购前 Intercom 旗下的 Fin](https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/?bc=HL) ⭐️ 9.0/10

Salesforce 宣布达成最终协议，以 36 亿美元收购 Fin——这家原名 Intercom 的 AI 客户支持平台。 此次收购加剧了 AI 客户支持代理领域的竞争，使 Salesforce 直接与由前 Salesforce CEO Bret Taylor 创立的 Sierra 以及其他初创公司如 Decagon 展开竞争。 Fin 一个月前从 Intercom 更名，在超过 1.2 万家客户中平均解决率达到 76%，许多客户超过 85%。该交易对 Fin 的估值为 36 亿美元。

hackernews · colesantiago · 6月15日 12:08 · [社区讨论](https://news.ycombinator.com/item?id=48540126)

**背景**: Fin 是一个 AI 驱动的客户支持平台，将实时聊天、帮助中心和自动化机器人整合到一个系统中。它使用名为 Fin 飞轮的持续改进循环来处理复杂查询。企业软件的 AI 代理领域竞争日益激烈，参与者包括 Sierra（估值 158 亿美元）和 Decagon（估值 45 亿美元）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fin.ai/capabilities">Fin capabilities: resolve complex customer queries | Fin</a></li>
<li><a href="https://listin.gg/tools/intercom">Intercom — AI -powered customer messaging and support platform .</a></li>
<li><a href="https://dust.tt/blog/top-ai-agent-builder-platforms-enterprises">Top AI Agent Builder Platforms for Enterprises (2026) | Dust Blog</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映出不同的反应。一些用户称赞得当的 AI 客户支持，指出 Fin 可以超越人工客服。其他人质疑帮助台公司的长期可行性，因为小型企业转向定制 AI 解决方案。还有人担心 Salesforce 可能会毁掉这个产品。

**标签**: `#acquisition`, `#salesforce`, `#ai customer support`, `#fin`, `#intercom`

---

<a id="item-3"></a>
## [LiteLLM 漏洞链允许低权限用户完全接管服务器](https://thehackernews.com/2026/06/litellm-vulnerability-chain-lets-low.html) ⭐️ 9.0/10

LiteLLM AI 网关中的三个连锁漏洞允许默认的低权限用户升级为完全管理员并实现远程代码执行，从而泄露所有提供商密钥和机密。 这一漏洞链至关重要，因为 LiteLLM 被广泛部署为 AI 模型访问的中央网关，服务器被接管会暴露超过 100 个 LLM 提供商的凭证，危及许多组织的安全态势。 这些漏洞由 Obsidian Security 的研究人员披露，该漏洞链利用默认的低权限账户提升至管理员权限，并在 LiteLLM 代理服务器上执行远程代码。

rss · The Hacker News · 6月15日 16:39

**背景**: LiteLLM 是一个开源的 Python SDK 和 AI 网关，为调用超过 100 个大型语言模型 API 提供与 OpenAI 兼容的接口。像 LiteLLM 这样的 AI 网关充当中间件，处理 LLM 调用的集成、路由、安全和成本跟踪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/LiteLLM">LiteLLM</a></li>
<li><a href="https://www.litellm.ai/">LiteLLM</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#AI gateway`, `#LiteLLM`, `#privilege escalation`

---

<a id="item-4"></a>
## [SearchLeak 攻击将 Microsoft 365 Copilot 变为数据窃取工具](https://www.bleepingcomputer.com/news/security/new-attack-turned-microsoft-365-copilot-into-1-click-data-theft-tool/) ⭐️ 9.0/10

Varonis Threat Labs 的研究人员发现了一个名为 SearchLeak 的漏洞链，攻击者可以通过点击精心构造的 URL，从 Microsoft 365 Copilot Enterprise Search 中窃取敏感数据。微软已将该漏洞修补为 CVE-2026-42824。 这一攻击链展示了像 Copilot 这样的企业 AI 助手存在的严重风险，因为它们深度访问用户数据。如果被利用，可能导致从电子邮件、OneDrive 和 SharePoint 大规模窃取数据，影响依赖 Microsoft 365 的组织。 该攻击链名为 SearchLeak，链式利用了三个漏洞，包括参数到提示注入，允许通过 URL 中的'q'参数进行自然语言查询。该漏洞编号为 CVE-2026-42824，CVSS 评分为 6.5，但微软将其标记为严重，因为它可以在仅需一次点击的情况下泄露数据。

rss · BleepingComputer · 6月15日 13:00

**背景**: Microsoft 365 Copilot 是一款 AI 驱动的生产力工具，它与 Microsoft Graph 集成，可访问电子邮件、日历、文件等企业数据。它使用语义索引来回答自然语言查询。SearchLeak 漏洞利用了 Copilot Enterprise Search 处理 URL 参数的方式，允许攻击者注入恶意提示，迫使 Copilot 将数据泄露到攻击者控制的服务器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.darkreading.com/application-security/copilot-searchleak-attack-1-click-data-theft">Copilot ' SearchLeak ' Attack Allows 1-Click Data Theft</a></li>
<li><a href="https://windowsnews.ai/article/cve-2026-42824-microsoft-shuts-down-searchleak-attack-chain-in-copilot.426371">CVE-2026-42824: Microsoft Shuts Down ‘ SearchLeak ’ Attack Chain in...</a></li>
<li><a href="https://www.microsoft.com/en-us/microsoft-365-copilot">Microsoft 365 Copilot | AI Productivity Tools for Work</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Microsoft 365`, `#Copilot`, `#data-theft`

---

<a id="item-5"></a>
## [vLLM 0.23.0：DeepSeek-V4 强化，MRv2 扩展](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 8.0/10

vLLM v0.23.0 发布了来自 200 位贡献者的 408 次提交，主要包含对 DeepSeek-V4 的重大强化（稀疏 MLA 解耦、TRTLLM-gen 内核、EPLB 支持），并将 Model Runner V2 默认扩展到 Llama 和 Mistral 密集模型。 此版本显著提升了 DeepSeek-V4 模型系列的推理性能和内存效率，同时使先进的 Model Runner V2 成为流行密集模型的默认选项，惠及整个 LLM 部署生态系统。 值得注意的技术细节包括：将稀疏 MLA 元数据从 DeepSeek-V3.2 解耦、新的用于生成阶段的 TRTLLM-gen 注意力内核、用于专家并行负载均衡的 EPLB，以及滑动窗口 KV 缓存的选择性前缀缓存保留。Model Runner V2 还获得了 FlashInfer 采样器、可分解的 CUDA 图和流水线并行气泡消除。

github · khluu · 6月15日 05:27

**背景**: vLLM 是一个面向大型语言模型的高吞吐量、内存高效的推理引擎。DeepSeek-V4 是一系列混合专家模型，需要高效的稀疏注意力和专家并行。Model Runner V2 是为提升结构化模型性能而引入的优化执行路径。TRTLLM 是 NVIDIA 的 TensorRT-LLM 库，用于 GPU 加速，EPLB 是用于专家并行负载均衡的工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/EPLB">GitHub - deepseek-ai/ EPLB : Expert Parallelism Load Balancer</a></li>
<li><a href="https://nvidia.github.io/TensorRT-LLM/advanced/gpt-attention.html">Multi-Head, Multi-Query, and Group-Query Attention — TensorRT- LLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/deepseek_v4/sparse_mla/">sparse _ mla - vLLM</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#release`, `#deepseek`, `#optimization`

---

<a id="item-6"></a>
## [Iroh 1.0 发布：用拨号键而非 IP 地址](https://www.iroh.computer/blog/v1) ⭐️ 8.0/10

Iroh 1.0 是这款基于 Rust 的对等网络库的重要版本，它引入了应用层加密连接，使用「拨号键」而非 IP 地址，并支持自定义传输协议。 此版本简化了应用开发者的对等连接，消除了对 IP 地址的依赖，并实现设备间安全的直接连接，有望促进去中心化应用的开发。 Iroh 原生支持 IPv4、IPv6 和中继传输，现在允许开发者实现针对 WebRTC、BLE 或 LoRa 等协议的自定义传输，扩展了其在多样网络环境中的适用性。

hackernews · chadfowler · 6月15日 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48542480)

**背景**: 传统网络依赖 IP 地址和 DNS 进行设备识别，这种方式可能不稳定。Iroh 使用加密密钥作为设备标识，实现无需中间商的直接连接。应用层加密确保数据由应用本身保护，独立于底层网络安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.iroh.computer/blog/v1">Iroh 1.0 - Dial Keys, not IPs - Iroh</a></li>
<li><a href="https://github.com/n0-computer/iroh">GitHub - n0-computer/iroh: IP addresses break, dial keys instead. Modular networking stack in Rust. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区将 Iroh 比作应用层的 Tailscale，强调了嵌入应用无需用户账户的便利性。开发者询问了自定义传输支持，Iroh 团队确认了可扩展性。一些人对基于密钥的身份模型提出疑问，但总体态度积极且技术讨论深入。

**标签**: `#iroh`, `#p2p`, `#networking`, `#encryption`, `#rust`

---

<a id="item-7"></a>
## [黑客新闻用户分享本地 LLM 编码体验](https://news.ycombinator.com/item?id=48542100) ⭐️ 8.0/10

一次黑客新闻讨论（306 条评论）揭示，许多开发者已成功用本地模型替代 Claude 和 GPT 等云端编码助手，在日常编码中取得了令人满意的性能。 这表明开源本地模型正成为专有云服务的可行替代方案，在隐私、成本节约和离线能力方面带来好处，且不会过多牺牲生产力。 用户报告使用 Qwen3.6-35B 和 Gemma-4-26B 等模型，硬件配置如双 RTX 3090 或 128GB RAM 的 Mac Studio，速度可达 150 tok/s。有人指出本地模型能力略逊于前沿模型，但足以完成大部分工作。

hackernews · cloudking · 6月15日 14:46

**背景**: 本地 LLM 在用户硬件上运行，消除对云 API 的依赖。推理速度以每秒 token 数（tok/s）衡量。Qwen 和 Gemma 等模型是开源的，通过混合专家（MoE）和分组查询注意力等架构优化效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@walterdeane/running-a-local-llm-for-code-assistance-dea64748041a">Running a Local LLM for Code Assistance - Medium</a></li>
<li><a href="https://grokipedia.com/page/Tokens_per_second">Tokens per second — Grokipedia</a></li>
<li><a href="https://github.com/UnknownGamer11/awesome-local-llm-2026">Awesome Local LLM Setup 2026 - GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者热情分享正面体验，许多人报告已完全替代云服务。有人指出与顶级模型相比能力有限，但强调为了隐私和成本，这种权衡是值得的。社区普遍对本地模型的未来持乐观态度。

**标签**: `#local-LLM`, `#coding-assistant`, `#open-source-models`, `#privacy`, `#AI-tools`

---

<a id="item-8"></a>
## [Hetzner 云服务器价格因硬件成本飙升而涨至三倍](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers) ⭐️ 8.0/10

Hetzner 宣布对其云服务器产品进行大幅价格调整，部分套餐价格约涨至原来的三倍，原因是 RAM 和 SSD 成本上涨。 此次涨价反映了 AI 热潮推动的硬件稀缺趋势，影响到依赖 Hetzner 等提供商提供经济型云基础设施的中小企业和开发者。 CPX11 套餐从每月 6.99 美元涨至 20.49 美元，且社区指出调整后缺乏针对轻负载场景的新低价选项。

hackernews · tuhtah · 6月15日 13:19 · [社区讨论](https://news.ycombinator.com/item?id=48540844)

**背景**: Hetzner 是一家以实惠价格著称的德国网络托管和云服务提供商。云服务器定价很大程度上取决于 DRAM 和 SSD 成本，而这两者因 AI 训练和数据中心需求增加而上涨。三倍涨幅相较常规年度调整显得异常剧烈。

**社区讨论**: 社区情绪强烈负面，许多用户批评涨幅过大。部分评论者将涨价归因于 AI 驱动的硬件需求，另一些则对缺乏针对低使用量虚拟机的经济型替代方案表示不满。

**标签**: `#cloud`, `#pricing`, `#hardware costs`, `#infrastructure`, `#AI boom`

---

<a id="item-9"></a>
## [TimescaleDB 时间序列压缩技术深度解析](https://roszigit.com/en/blog/timescaledb-compression-hypercore) ⭐️ 8.0/10

一篇详细文章解释了 TimescaleDB 的 hypercore 引擎如何使用 delta 编码、delta-of-delta、Gorilla XOR 和游程编码，在 PostgreSQL 中为时间序列数据实现高达 98%的压缩率。 这很重要，因为时间序列数据增长迅速，高效压缩可以降低存储成本，同时保持数据在线且可查询。这些技术也揭示了 CPU 与 I/O 之间的数据库性能权衡。 hypercore 引擎是一个混合行列引擎，可自动压缩超过可配置阈值的数据块。压缩是无损的，可以通过手动或自动策略应用。

hackernews · lkanwoqwp · 6月15日 17:29 · [社区讨论](https://news.ycombinator.com/item?id=48544451)

**背景**: TimescaleDB 是用于时间序列数据的 PostgreSQL 扩展。它将数据组织成块（超表），并提供原生压缩以减少存储。常见的压缩算法包括用于时间戳的 delta-of-delta 和用于浮点值的 XOR，灵感来自 Facebook 的 Gorilla 论文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://roszigit.com/en/blog/timescaledb-compression-hypercore">TimescaleDB Compression: Hypercore and Columnar Storage with up to 98% Ratio in PostgreSQL</a></li>
<li><a href="https://dev.to/philip_mcclarence_2ef9475/timescaledb-compression-a-complete-guide-to-95-storage-reduction-2mo4">TimescaleDB Compression: A Complete Guide to 95%+ Storage Reduction - DEV Community</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-02-02-timescaledb-compression/view">How to Compress Data in TimescaleDB</a></li>

</ul>
</details>

**社区讨论**: 社区赞扬了技术深度，但强调了性能权衡：压缩可以提高扫描速率但可能增加 CPU 使用。一些用户将 TimescaleDB 与其他扩展如 deltax 进行了比较，并讨论了用于物联网的有损替代方案如 swinging-door。还有人对标题中的“高达”措辞提出了批评。

**标签**: `#timescaledb`, `#compression`, `#time-series`, `#postgresql`, `#database-performance`

---

<a id="item-10"></a>
## [福克斯据报道收购 Roku 引发整合担忧](https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9) ⭐️ 8.0/10

据《华尔街日报》报道，福克斯（Fox）正在收购流媒体硬件和平台公司 Roku。这笔交易将使福克斯直接接触到 Roku 数千万家庭用户群体。 这笔收购将一家大型内容制作商与主导性流媒体硬件平台结合，极大地集中了媒体权力，可能影响消费者的内容选择和访问。这引发了关于垂直整合和流媒体市场竞争的担忧。 Roku 被大约 30-50%的美国家庭使用，为福克斯提供了直达观众的渠道。社区成员猜测可能出现的变化，比如专用的福克斯新闻按钮或强制在 Roku 主屏上放置内容。

hackernews · thm · 6月15日 12:50 · [社区讨论](https://news.ycombinator.com/item?id=48540499)

**背景**: Roku 是一个流行的流媒体设备和操作系统，提供对各种流媒体服务的访问，最初以服务中立著称。福克斯是一家大型媒体集团，拥有新闻和娱乐等内容。福克斯收购 Roku 将是一次垂直整合举措，类似于过去的媒体整合趋势，并可能破坏 Roku 的中立平台地位。

**社区讨论**: 评论者普遍悲观，表达了对媒体整合、内容控制和硬件访问的担忧。几位用户担心可能出现福克斯新闻按钮或强制内容，一些人已经开始迁移到 Nvidia Shield 等替代品。

**标签**: `#acquisition`, `#streaming`, `#Roku`, `#Fox`, `#media consolidation`

---

<a id="item-11"></a>
## [分析内存安全 CVE：Rust 与 C/C++的细微差别](https://kobzol.github.io/rust/2026/06/15/how-memory-safety-cves-differ-between-rust-and-c-cpp.html) ⭐️ 8.0/10

该分析挑战了系统编程社区中过于简单化的说法，帮助开发者和安全专业人员更明智地评估语言采用和安全性。 该文章指出，Rust 的内存安全保证减少了某些类型的错误，但其 CVE 范围包括 panic 和逻辑错误，而 C/C++的 CVE 通常涉及不安全的库依赖；因此，没有上下文的直接 CVE 计数是不可靠的。

hackernews · nicoburns · 6月15日 16:11 · [社区讨论](https://news.ycombinator.com/item?id=48543392)

**背景**: 内存安全漏洞，如缓冲区溢出和释放后使用，是 C 和 C++程序中安全问题的主要来源。Rust 旨在通过其所有权系统和借用检查器防止这些错误，但仍需要不安全代码进行底层操作，这可能会引入类似的风险。

**社区讨论**: 评论者大多同意原始 CVE 数量是一个糟糕的指标；一位用户表示，他们会直接忽略任何比较 CVE 数量的人。其他人则讨论细微差别，例如 Rust 的 Option<T>使 None 处理显式化，而 C 中空指针崩溃，并质疑 Rust 中的类型安全漏洞是否应被视为漏洞。

**标签**: `#rust`, `#c++`, `#memory safety`, `#CVE`, `#systems programming`

---

<a id="item-12"></a>
## [Typst 0.15.0 发布，支持多参考文献列表](https://typst.app/docs/changelog/0.15.0/) ⭐️ 8.0/10

Typst 0.15.0 新增了在单个文档中包含多个参考文献列表的功能，并改进了 HTML 导出，包括自动将数学公式转换为 MathML。 此次发布增强了 Typst 对大型学术文档和书籍的适用性，响应了一个长期存在的功能需求。HTML/MathML 的改进也使 Typst 更适用于网络出版。 多参考文献列表功能允许用户按章节或类别分隔参考文献，类似于 LaTeX 的 bibunit 或 chapterbib 包。HTML 输出中的数学公式现在会自动渲染为 MathML，提升了可访问性。

hackernews · schu · 6月15日 17:24 · [社区讨论](https://news.ycombinator.com/item?id=48544396)

**背景**: Typst 是一个开源的排版系统，旨在作为 LaTeX 的现代替代品。它使用简洁的标记语法，并可以编译为 PDF、图片或 HTML。该项目旨在为技术和学术文档提供更直观、更强大的创作体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://typst.app/">Typst : The new foundation for documents</a></li>
<li><a href="https://github.com/typst/typst/issues/1097">Multiple bibliographies · Issue #1097 · typst/typst - GitHub</a></li>
<li><a href="https://banglamedm.medium.com/what-is-typst-and-why-i-love-it-36fe20eece3e">What is typst and why I love it. Typst is a content authoring... | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区反响非常积极，许多用户赞扬新的多参考文献列表功能。然而，一些用户指出脚注和参考文献引用方面仍存在问题，少数评论提到了基于 LLM 的工作流程的学习曲线。

**标签**: `#typst`, `#typesetting`, `#open source`, `#version release`

---

<a id="item-13"></a>
## [中国黑客利用 Google Workspace 规则窃取电子邮件](https://thehackernews.com/2026/06/chinese-hackers-abused-google-workspace.html) ⭐️ 8.0/10

一个与中国有关联的间谍组织（追踪编号 UNC6508）利用 InfiniteRed 恶意软件入侵了 REDCap 研究服务器，窃取了登录凭证，然后篡改受害者的 Google Workspace 规则，在长达一年的活动中外泄了敏感的研究和国防邮件。 此事件突显了一种利用合法 Google Workspace 功能进行外泄的新技术，使得检测变得困难，并强调了国家支持的黑客对敏感研究和国防领域的持续威胁。 InfiniteRed 恶意软件挂钩 REDCap 的 PHP post_process 钩子，捕获包含登录凭证的 POST 请求体，使用 AES-128-CBC 加密，并存储在 redcap_log_event 表中。攻击者随后利用受害者的 Google Workspace 邮件路由规则，将邮件副本转发到外部账户。

rss · The Hacker News · 6月15日 19:44

**背景**: REDCap（研究电子数据采集）是一个用于构建和管理在线调查及数据库的安全网络应用程序，常用于学术和医学研究。Google Workspace 邮件路由规则允许管理员根据条件自动转发或复制邮件。入侵 REDCap 服务器与滥用 Google Workspace 规则的结合，使得数据外泄能够逃避典型的安全监控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://projectredcap.org/software/requirements/">Installation & Technical Requirements – REDCap</a></li>
<li><a href="https://undercodetesting.com/inside-unc6508s-infinitered-how-prc-hackers-spent-a-year-stealing-military-and-medical-secrets-via-redcap-video/">Inside UNC6508’s INFINITERED: How PRC Hackers Spent a Year ...</a></li>
<li><a href="https://www.scworld.com/brief/china-linked-group-uses-infinitered-malware-to-target-medical-research-institutions">China-linked group uses InfiniteRed malware to target medical ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#espionage`, `#Google Workspace`, `#China`, `#data exfiltration`

---

<a id="item-14"></a>
## [WordPress 插件脚本被篡改，植入隐藏后门](https://thehackernews.com/2026/06/popular-wordpress-plugin-scripts.html) ⭐️ 8.0/10

攻击者篡改了三个流行 WordPress 插件（PushEngage、OptinMonster 和 TrustPulse）的 JavaScript 文件，在管理员登录时创建隐藏的管理员账户和后门。 这次供应链攻击危及数千个网站使用的可信插件，使攻击者能够在不被察觉的情况下接管网站。网站管理员必须立即检查是否有未授权的管理员账户和隐藏插件。 恶意代码仅在网站管理员登录时激活，普通访客不受影响。攻击者创建了一个新的管理员账户并安装了一个隐藏插件以维持持久访问。

rss · The Hacker News · 6月15日 09:59

**背景**: PushEngage、OptinMonster 和 TrustPulse 是广泛使用的营销插件，分别用于网页推送通知、潜在客户生成和社会证明。供应链攻击通过渗透合法更新或依赖关系来分发恶意软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bit.ly/3vmpGPM">PushEngage - The Best Mobile & Web Push Notification Service</a></li>
<li><a href="https://optinmonster.com/pricing/">OptinMonster Pricing - Lead Generation & Conversion Optimization Software</a></li>
<li><a href="https://trustpulse.com/">TrustPulse: Best Social Proof and Fomo App for Marketers</a></li>

</ul>
</details>

**标签**: `#security`, `#wordpress`, `#supply chain attack`, `#backdoor`

---

<a id="item-15"></a>
## [Palo Alto 警告 PAN-OS VPN 漏洞正被积极利用](https://thehackernews.com/2026/06/palo-alto-warns-of-active-exploitation.html) ⭐️ 8.0/10

Palo Alto Networks 确认 CVE-2026-0257 正在被积极利用，这是 PAN-OS GlobalProtect VPN 门户和网关组件中的一个关键身份验证绕过漏洞（CVSS 7.8）。 该漏洞影响广泛部署的 PAN-OS 防火墙，可能允许攻击者绕过身份验证并未经授权访问企业网络。立即修补对于防止入侵至关重要。 CVE-2026-0257 漏洞影响 PAN-OS 软件的门户和网关组件，CVSS 评分为 7.8。Palo Alto 未将此次利用归因于特定威胁行为者，但敦促所有用户应用可用补丁。

rss · The Hacker News · 6月15日 06:17

**背景**: PAN-OS 是驱动 Palo Alto Networks 下一代防火墙的操作系统，通过 App-ID、Content-ID 和 User-ID 提供可视化和控制。GlobalProtect 是一种 VPN 解决方案，可为移动员工提供安全的远程访问。该漏洞允许攻击者绕过 GlobalProtect 门户和网关的身份验证，可能导致未经授权的网络访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.paloaltonetworks.com/pan-os">PAN-OS - Palo Alto Networks</a></li>
<li><a href="https://docs.paloaltonetworks.com/globalprotect">GlobalProtect - Palo Alto Networks</a></li>

</ul>
</details>

**标签**: `#vulnerability`, `#security`, `#Palo Alto Networks`, `#VPN`, `#CVE`

---

<a id="item-16"></a>
## [思科修复 Catalyst SD-WAN 管理器零日漏洞](https://www.bleepingcomputer.com/news/security/cisco-fixes-sd-wan-vmanage-flaw-exploited-in-zero-day-attacks/) ⭐️ 8.0/10

思科发布了安全更新，修复了 Catalyst SD-WAN 管理器中的 CVE-2026-20262 漏洞，该漏洞曾作为零日漏洞被积极利用，可在设备上提升至 root 权限。 此修复对于依赖思科 SD-WAN 解决方案的企业至关重要，因为该漏洞已在野外被利用，攻击者可完全控制受影响系统。建议立即打补丁以防止被入侵。 该漏洞编号为 CVE-2026-20262，影响 Catalyst SD-WAN 管理器（原名 vManage），允许未经身份验证的远程攻击者获取 root 权限。思科已为所有支持版本提供软件更新。

rss · BleepingComputer · 6月15日 17:12

**背景**: SD-WAN（软件定义广域网）是一种通过将控制平面与硬件解耦来简化广域网管理的技术。思科 Catalyst SD-WAN 管理器是一个集中管理平台，用于配置、监控和故障排查 SD-WAN 设备。零日漏洞是指在供应商知晓或发布补丁之前就被利用的漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisco.com/site/us/en/products/networking/wan/sd-wan-manager/index.html">Cisco Catalyst SD - WAN Manager (formerly vManage) - Cisco</a></li>
<li><a href="https://en.wikipedia.org/wiki/SD-WAN">SD-WAN</a></li>

</ul>
</details>

**标签**: `#security`, `#cisco`, `#vulnerability`, `#zero-day`, `#SD-WAN`

---

<a id="item-17"></a>
## [Infinite Campus 数据泄露影响 13.7 万学校员工账户](https://www.bleepingcomputer.com/news/security/infinite-campus-data-breach-affects-137-000-school-staff-accounts/) ⭐️ 8.0/10

勒索团伙 ShinyHunters 在 3 月份通过针对 Infinite Campus（一款广泛使用的 K-12 学生信息系统）的 Salesforce 攻击，窃取了超过 13.7 万学校员工账户的个人数据。 此次泄露事件凸显了教育 IT 系统的关键漏洞，暴露了大量学校员工的敏感个人信息，可能引发进一步的攻击或身份盗窃。 攻击专门针对 Infinite Campus 使用的 Salesforce 实例，ShinyHunters 是一个以数据勒索和暗网销售闻名的网络犯罪团伙。

rss · BleepingComputer · 6月15日 12:38

**背景**: ShinyHunters 是一个自 2019 年起活跃的黑客组织，以大规模数据泄露和勒索闻名。Salesforce 攻击通常涉及社会工程学手段，例如冒充 IT 支持人员绕过多因素认证，近期多次活动均采用类似手法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ShinyHunters">ShinyHunters - Wikipedia</a></li>
<li><a href="https://cybernews.com/security/massive-salesforce-breach-campaign-started-on-github/">Massive Salesforce breach campaign explained | Cybernews</a></li>

</ul>
</details>

**标签**: `#data breach`, `#cybersecurity`, `#education`, `#privacy`, `#extortion`

---

<a id="item-18"></a>
## [CISA 将两个已被积极利用的漏洞添加到 KEV 目录](https://www.cisa.gov/news-events/alerts/2026/06/15/cisa-adds-two-known-exploited-vulnerabilities-catalog) ⭐️ 7.0/10

CISA 在其已知被利用漏洞（KEV）目录中新增了两个已被积极利用的漏洞：影响 Cisco Catalyst SD-WAN 管理器的 CVE-2026-20262，以及影响 LiteSpeed cPanel 插件的 CVE-2026-54420。 这些漏洞对使用受影响软件的联邦企业及所有组织构成重大风险，因为恶意网络行为者正在积极利用它们。CISA 将其加入 KEV 目录后，根据 BOD 26-04 要求联邦机构优先修复，并鼓励所有组织采用基于风险的漏洞管理。 CVE-2026-20262 是 Cisco Catalyst SD-WAN Manager（原 vManage）中的目录或路径遍历漏洞，而 CVE-2026-54420 是 LiteSpeed cPanel 插件中的 UNIX 符号链接跟随漏洞。这两个 CVE 均有被积极利用的证据和明确的缓解指南。

rss · CISA Cybersecurity Advisories · 6月15日 12:00

**背景**: CISA 的已知被利用漏洞（KEV）目录是一个公开列表，收录了已在野外被积极利用的漏洞，要求联邦机构根据约束性操作指令在规定时间内修复。Cisco Catalyst SD-WAN Manager 是用于管理 SD-WAN 部署的集中式仪表板，在企业网络中广泛使用。LiteSpeed Web Server 及其 cPanel 插件是托管网站的 Apache 流行高性能替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisco.com/site/us/en/products/networking/wan/sd-wan-manager/index.html">Cisco Catalyst SD-WAN Manager (formerly vManage) - Cisco</a></li>
<li><a href="https://docs.litespeedtech.com/lsws/cp/cpanel/quickstart/">Quick Start LiteSpeed Web Server with cPanel | LiteSpeed ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerabilities`, `#CISA`, `#Cisco`, `#LiteSpeed`

---

<a id="item-19"></a>
## [朝鲜黑客利用开发者工具传播恶意软件](https://thehackernews.com/2026/06/north-korean-hackers-are-turning.html) ⭐️ 7.0/10

Proofpoint 标记了两起与朝鲜威胁组织 Contagious Interview 相关的恶意活动，这些活动利用虚假的开发人员招聘和代码审查主题来传播恶意软件。 通过开发人员信任的工具和工作流程进行攻击构成了严重的供应链风险，可能危及跨行业的软件项目和敏感数据。 这些活动通过虚假编程测试传递后门，如 OtterCookie 和 FlexibleFerret；该威胁行为者也被追踪为 Famous Chollima、HexagonalRodent 和 Void Dokkaebi。

rss · The Hacker News · 6月15日 19:32

**背景**: Contagious Interview 是一个长期存在的朝鲜网络间谍活动（首次于 2023 年被报道），威胁行为者伪装成加密货币和 AI 公司的招聘人员，诱使开发人员下载恶意软件。该集团还以利用非法自由职业活动向朝鲜输送资金而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/03/11/contagious-interview-malware-delivered-through-fake-developer-job-interviews/">Contagious Interview: Malware delivered through fake developer job interviews | Microsoft Security Blog</a></li>
<li><a href="https://unit42.paloaltonetworks.com/north-korean-threat-actors-lure-tech-job-seekers-as-fake-recruiters/">Contagious Interview: DPRK Threat Actors Lure Tech Industry Job Seekers to Install New Variants of BeaverTail and InvisibleFerret Malware</a></li>
<li><a href="https://www.crowdstrike.com/en-us/adversaries/famous-chollima/">Famous Chollima Adversary Profile | CrowdStrike</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#north korea`, `#malware`, `#phishing`, `#developer tools`

---

<a id="item-20"></a>
## [每周安全回顾：Chrome 零日、UniFi 漏洞、macOS 窃密软件、VPN 缺陷](https://thehackernews.com/2026/06/weekly-recap-chrome-0-day-unifi.html) ⭐️ 7.0/10

Thehackernews.com 发布了一篇每周回顾，涵盖 Chrome 零日漏洞、包括 Log4Shell 和严重缺陷在内的多个 UniFi 漏洞、日益增多的 macOS 信息窃取程序（如 Atomic Stealer），以及一个 VPN 缺陷。文章强调过时和暴露的软件仍然是主要攻击途径。 这篇回顾及时提醒组织要积极打补丁、淘汰已废弃的软件并保护暴露的服务。被利用的遗留组件的反复出现影响了广大用户和管理员。 UniFi 漏洞包括影响版本 5.13.29 至 6.5.53 的 Log4Shell（CVE-2021-44228），以及 UniFi OS 中最近的严重漏洞 CVE-2026-34908（不当访问控制）和 CVE-2026-34909（路径遍历）。macOS 窃密程序如 Atomic Stealer、Poseidon Stealer 和 DigitStealer 常通过恶意的 DMG 安装程序传播。

rss · The Hacker News · 6月15日 13:49

**背景**: 每周回顾汇总了显著的安全事件，帮助专业人员保持对活跃威胁的警觉。文章的主题“又出问题了”强调许多入侵源于被遗忘或未打补丁的软件。关键概念包括零日漏洞（未修补的漏洞）、Log4Shell（Log4j 中的严重远程代码执行缺陷）以及信息窃取程序（窃取敏感数据的恶意软件）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rapid7.com/db/modules/exploit/multi/http/ubiquiti_unifi_log4shell/">UniFi Network Application Unauthenticated JNDI Injection ...</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/ubiquiti-patches-three-max-severity-unifi-os-vulnerabilities/">Ubiquiti patches three max severity UniFi OS vulnerabilities</a></li>
<li><a href="https://unit42.paloaltonetworks.com/macos-stealers-growing/">Stealers on the Rise: A Closer Look at a Growing macOS Threat</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerabilities`, `#exploits`, `#zero-day`, `#weekly recap`

---