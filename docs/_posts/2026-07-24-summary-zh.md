---
layout: default
title: "Horizon Summary: 2026-07-24 (ZH)"
date: 2026-07-24
lang: zh
---

> 从 88 条内容中筛选出 20 条重要资讯。

---

1. [江森自控楼宇系统出现严重远程代码执行漏洞](#item-1)
2. [天文学家可能发现了首颗系外卫星](#item-2)
3. [2026 年菲尔兹奖得主提前泄露](#item-3)
4. [俄间谍组织利用 Zimbra 零日漏洞窃取 2FA 代码](#item-4)
5. [Check Point 修补正在被利用的 SmartConsole 漏洞](#item-5)
6. [DeepSeek 创始人优先考虑 AGI，而非增长和商业化](#item-6)
7. [DeepSeek V4 Flash 在两张 RTX 4090d GPU 上达到 105 token/秒](#item-7)
8. [Namecheap 因社会工程学将账户交给未验证第三方](#item-8)
9. [TheNumbers.com 因恶意爬取被迫关闭](#item-9)
10. [初创企业创始人反对禁止中国开源 AI 模型](#item-10)
11. [ATProto 公共数据与私有应用间的张力](#item-11)
12. [500 行 C++实现软件渲染教程](#item-12)
13. [软件工厂因缺乏更好指标与强化学习而失败](#item-13)
14. [CISA 警告 Weintek cMT3092X HMI 存在高危漏洞](#item-14)
15. [CISA 警告 Rockwell ThinManager 存在路径遍历漏洞](#item-15)
16. [俄罗斯 APT 组织 LAUNDRY BEAR 利用新漏洞攻击 Zimbra 用户](#item-16)
17. [CISA 警告 MZ Automation libIEC61850 存在严重漏洞](#item-17)
18. [Panduit IntraVUE 关键漏洞可远程接管工业控制系统设备](#item-18)
19. [Claude Cowork 沙箱逃逸漏洞影响 50 万 Mac 用户](#item-19)
20. [Chaos 勒索软件利用 msaRAT 通过无头浏览器路由 C2 通信](#item-20)

---

<a id="item-1"></a>
## [江森自控楼宇系统出现严重远程代码执行漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-204-01) ⭐️ 10.0/10

CISA 发布公告，警告江森自控 C-CURE 9000 和 Victor 应用服务器存在严重漏洞，攻击者可远程执行代码，CVSS 评分达 9.6。 这些漏洞影响全球关键制造业基础设施中广泛使用的楼宇管理系统，攻击者有可能破坏物理安全控制。 漏洞包括服务器端请求伪造（SSRF）和以不必要权限执行，影响 C-CURE 9000 和 Victor 的 v2.90_v3.0 及之前版本，以及 Victor Web 的 v7.1 及之前版本。

rss · CISA Cybersecurity Advisories · 7月23日 12:00

**背景**: 服务器端请求伪造（SSRF）是一种网络安全漏洞，允许攻击者诱使服务器端应用向非预期位置发起请求，通常用于访问内部资源。江森自控 C-CURE 9000 和 Victor 是用于关键基础设施物理安全和访问控制的楼宇管理系统。CISA 公告建议升级至 3.20 或更高版本，并实施网络分段和最小权限原则。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Server-side_request_forgery">Server-side request forgery - Wikipedia</a></li>
<li><a href="https://portswigger.net/web-security/ssrf">What is SSRF (Server-side request forgery)? Tutorial & Examples | Web Security Academy</a></li>

</ul>
</details>

**标签**: `#security`, `#CISA`, `#ICS advisory`, `#remote code execution`, `#Johnson Controls`

---

<a id="item-2"></a>
## [天文学家可能发现了首颗系外卫星](https://www.eso.org/public/news/eso2610/) ⭐️ 9.0/10

天文学家探测到一颗候选系外卫星，编号为 CD-35 2722 b I，它围绕一颗褐矮星运行，该系统距离地球约 5000 光年。 若得到确认，这将是人类发现的首颗系外卫星，为系外行星科学开辟新领域，并帮助理解太阳系外的卫星形成及潜在宜居性。 这颗候选系外卫星质量接近木星，而其宿主是一颗约 50 倍木星质量的褐矮星；这种不寻常的大小比例挑战了传统上对行星和卫星的定义。

hackernews · MarcoDewey · 7月23日 14:02 · [社区讨论](https://news.ycombinator.com/item?id=49021783)

**背景**: 系外卫星是绕系外行星或其他非恒星系外天体运行的自然卫星。探测系外卫星极其困难，因为它们相对其宿主行星而言既小又暗。褐矮星是质量过大而不能算作行星，但又不足以像恒星那样聚变氢的天体。这一发现是利用智利 ESO 拉西拉天文台的地基望远镜数据完成的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Exomoon">Exomoon</a></li>
<li><a href="https://www.theregister.com/science/2026/07/22/astronomers-spot-exomoon-candidate-thats-almost-as-massive-as-jupiter/5276419">Astronomers spot exomoon candidate that's almost as massive as Jupiter ...</a></li>

</ul>
</details>

**社区讨论**: 评论者就艺术家效果图中的大小准确性展开讨论，指出褐矮星作为恒星或行星的分类存在模糊性，并称赞发现地智利阿塔卡马沙漠的暗夜天空。

**标签**: `#astronomy`, `#exomoon`, `#exoplanets`, `#discovery`

---

<a id="item-3"></a>
## [2026 年菲尔兹奖得主提前泄露](https://www.mathunion.org/imu-awards/fields-medal/fields-medals-2026) ⭐️ 9.0/10

2026 年菲尔兹奖得主意外在國際數學聯盟网站上提前公布，获奖者因在调和分析和几何测度论方面的重大贡献而获奖，包括在傅里叶限制、Kakeya 问题和局部平滑猜想方面的进展。 菲尔兹奖是数学界最高荣誉之一，此次提前公布实属罕见，引发了学界广泛关注。这一事件也凸显了调和分析和几何测度论在现代数学中日益重要的地位。 此次提前公布似乎是由于网站失误所致；其中一位获奖者 Jacob Tsimerman 与人合著了一篇题为《涉及人工智能的全球毁灭未来分类》的论文。另一位获奖者曾是国际数学奥林匹克金牌得主。

hackernews · nill0 · 7月23日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=49022137)

**背景**: 菲尔兹奖每四年颁发一次，授予 40 岁以下数学家的杰出成就。调和分析研究函数如何分解为波的叠加；几何测度论将光滑几何推广到不规则的集合。这些领域与偏微分方程、数论和数据科学有着深刻联系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Harmonic_analysis">Harmonic analysis</a></li>
<li><a href="https://en.wikipedia.org/wiki/Geometric_measure_theory">Geometric measure theory - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对获奖者工作的技术深度表示敬畏，其中一人指出，无法向门外汉解释他们的成就。另一条评论提到了其中一位获奖者合著的 AI 安全论文，引发了关于数学家对 AI 担忧的讨论。整体氛围是祝贺和尊重。

**标签**: `#mathematics`, `#fields medal`, `#academia`, `#awards`

---

<a id="item-4"></a>
## [俄间谍组织利用 Zimbra 零日漏洞窃取 2FA 代码](https://thehackernews.com/2026/07/russian-espionage-group-exploited.html) ⭐️ 9.0/10

一个俄罗斯国家支持的间谍组织利用 Zimbra 网络邮件客户端中一个此前未知的零日漏洞，在数月内窃取了西方组织的电子邮件、密码和双因素认证恢复码。 此次攻击凸显了广泛使用的电子邮件平台中零日漏洞的风险，该漏洞实现了长期间谍活动，甚至攻破了受双因素认证保护的账户。 恶意载荷仅通过打开邮件即可触发，窃取了最近 90 天的邮件、整个邮件目录、浏览器中存储的密码以及双因素认证恢复码。

rss · The Hacker News · 7月23日 18:36

**背景**: Zimbra 是一个开源的企业级电子邮件和协作平台，被全球许多组织使用。双因素认证恢复码是备份代码，允许用户在丢失主要认证设备时重新获得账户访问权限；它们被视为最后一道防线，但其本身也是攻击者的重要目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zimbra">Zimbra - Wikipedia</a></li>
<li><a href="https://login.gov/help/create-account/authentication-methods/backup-codes/">Backup codes - Login.gov</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#zero-day`, `#espionage`, `#Zimbra`, `#vulnerability`

---

<a id="item-5"></a>
## [Check Point 修补正在被利用的 SmartConsole 漏洞](https://thehackernews.com/2026/07/check-point-patches-exploited.html) ⭐️ 9.0/10

Check Point 已发布安全更新，修补了 SmartConsole 中一个正在被野外积极利用的关键身份验证绕过漏洞（CVE-2026-16232）。 此漏洞允许未经身份验证的攻击者获得 Check Point 安全管理与多域管理产品的完全管理员权限，使整个网络面临风险。 该漏洞的 CVSS 评分为 9.3，影响 SmartConsole 登录过程，并涉及安全管理与 MDSM（多域安全管理）产品。

rss · The Hacker News · 7月23日 06:34

**背景**: SmartConsole 是管理员用于管理 Check Point 安全环境的图形用户界面（GUI），包括配置策略、设备和监控事件。多域管理（MDSM）允许集中管理多个 Check Point 安全域。CVE-2026-16232 漏洞绕过了 SmartConsole 登录的身份验证，使攻击者无需有效凭据即可获得完全管理控制权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sc1.checkpoint.com/documents/R81/WebAdminGuides/EN/CP_R81_SecurityManagement_AdminGuide/Topics-SECMG/Understanding-SmartConsole.htm">Understanding SmartConsole</a></li>
<li><a href="https://sc1.checkpoint.com/documents/R81/WebAdminGuides/EN/CP_R81_Multi-DomainSecurityManagement_AdminGuide/Topics-MDSG/SmartConsole.htm">SmartConsole</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#active exploitation`, `#Check Point`, `#authentication bypass`

---

<a id="item-6"></a>
## [DeepSeek 创始人优先考虑 AGI，而非增长和商业化](https://www.reddit.com/r/LocalLLaMA/comments/1v49lxp/deepseek_founders_4hour_investor_meeting_deepseek/) ⭐️ 9.0/10

DeepSeek 创始人梁文锋在四小时的投资者会议上表示，公司的核心目标是 AGI，而非用户增长或商业化，开源是提高成功概率的战略选择。 这揭示了 AI 行业中罕见的战略立场——大多数公司优先考虑市场份额和收入，同时强调了 AGI 最终巨大价值的长期押注。 DeepSeek 开源了其部署的相同模型，不打算构建超级应用或与字节跳动、腾讯竞争，并相信在资源限制内扩大规模会带来更好的结果。

reddit · r/LocalLLaMA · /u/MagicZhang · 7月23日 10:09

**背景**: DeepSeek 是一家专注于实现通用人工智能（AGI）的中国 AI 公司。创始人梁文锋主张开源，认为这是加速进展并避免因试图垄断 AGI 价值而被历史淘汰的风险。

**标签**: `#DeepSeek`, `#AGI`, `#AI strategy`, `#open source`

---

<a id="item-7"></a>
## [DeepSeek V4 Flash 在两张 RTX 4090d GPU 上达到 105 token/秒](https://www.reddit.com/r/LocalLLaMA/comments/1v4n8wj/deepseek_v4_flash_105_ts_on_two_nvidia_4090d_48g/) ⭐️ 9.0/10

一位开发者用 Triton 重新实现了仅 Blackwell 支持的核函数（DeepGEMM、FlashInfer 稀疏 MLA、分块缩放 FP8），从而在两张 Nvidia RTX 4090d GPU 上以 vLLM 运行 DeepSeek V4 Flash，达到 105 token/秒。与之前的方案相比，并行代理工作流速度提升 2-3 倍。 这使得 DeepSeek V4 Flash 的高性能推理能够在广泛可用的 Ada 代 GPU（RTX 4090）上实现，而无需 Blackwell 硬件。对于本地运行大语言模型进行代理和多轮应用，可行性显著提高。 首次运行会将模型压缩至~IQ2 量化以适配两张 GPU 共 96GB 显存。实现使用了自定义 Docker 镜像（vllm-moet-sm89），并需要启用 GPU 间的 P2P 补丁。作者指出可能还有进一步性能提升的空间。

reddit · r/LocalLLaMA · /u/iSevenDays · 7月23日 19:01

**背景**: Blackwell GPU（如 RTX 6000 Blackwell）包含专用硬件核函数，用于 FP8 矩阵乘法（DeepGEMM）、高效注意力（FlashInfer 稀疏 MLA）和分块缩放 FP8 量化，这些在 Ada（sm89）代 GPU（如 RTX 4090）上并不原生支持。Triton 是一种开源的领域特定语言，用于编写可针对多种架构的 GPU 核函数。通过用 Triton 重新实现这些核函数，开发者绕过了硬件限制，使推理在 Ada GPU 上成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/DeepGEMM">GitHub - deepseek-ai/DeepGEMM: DeepGEMM: clean and efficient BLAS kernel library on GPU · GitHub</a></li>
<li><a href="https://docs.flashinfer.ai/api/sparse.html">flashinfer . sparse - FlashInfer 0.6.14 documentation</a></li>
<li><a href="https://triton-lang.org/main/getting-started/tutorials/10-block-scaled-matmul.html">Block Scaled Matrix Multiplication — Triton documentation</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#Triton`, `#GPU`, `#vLLM`, `#performance`

---

<a id="item-8"></a>
## [Namecheap 因社会工程学将账户交给未验证第三方](https://news.ycombinator.com/item?id=49028037) ⭐️ 8.0/10

一名 Namecheap 用户报告称，在收到密码重置请求后，Namecheap 客服未经适当验证就更改了账户邮箱和密码，导致未经验证的第三方接管了账户。 这一事件揭示了 Namecheap 客服流程中的严重安全漏洞，可能影响所有依赖该注册商管理域名的用户。它凸显了加强身份验证和防范社会工程学攻击的必要性。 攻击者只需知道域名并致电客服，就能说服他们自己是所有者，尽管账户是在原所有者名下注册的。原所有者已提交工单否认密码重置请求，但 Namecheap 仍进行了更改。

hackernews · Thrashed · 7月23日 21:05

**背景**: 像 Namecheap 这样的域名注册商管理域名注册和 DNS 设置。社会工程学攻击涉及操纵人们执行操作或泄露机密信息。通过这种方式接管账户是已知风险，但适当的验证程序（例如致电注册所有者）本应防止这种情况发生。

**社区讨论**: 评论者对 Namecheap 的安全性表示担忧，有人指出该公司已被私募股权公司收购数月，类似问题此前也曾发生。一位评论者建议启用域名隐私保护可以防止攻击者看到注册者的邮箱，但这并不能为客服失误开脱。

**标签**: `#security`, `#domain registrar`, `#social engineering`, `#customer support`, `#Namecheap`

---

<a id="item-9"></a>
## [TheNumbers.com 因恶意爬取被迫关闭](https://stephenfollows.com/p/what-just-happened-to-thenumberscom-should-worry-us-all) ⭐️ 8.0/10

票房数据网站 TheNumbers.com 因遭受大规模恶意爬取（疑似来自 AI 公司）而被迫关闭，重新上线后功能大幅缩减，数据量减少。 此事件凸显了中小网站面对爬虫攻击的脆弱性，并引发了对 AI 训练时代公开数据可持续性的担忧。 文章推测，恶意爬取可能利用漏洞获取特权访问权限，用于在预测市场上进行押注；目前该网站仅返回原始数据的极小部分。

hackernews · nickthegreek · 7月23日 16:53 · [社区讨论](https://news.ycombinator.com/item?id=49024691)

**背景**: 网络爬取是从网站自动提取数据的技术。激进的爬取行为可能压垮服务器，影响正常用户访问。机器人缓解技术（如速率限制和验证码）用于防止滥用，但使用住宅代理和 AI 的复杂机器人可能绕过这些防护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://webscraping.ai/faq/domain-com-scraping/what-are-the-potential-consequences-of-scraping-domain-com-too-aggressively">What are the potential consequences of scraping ... | WebScraping .AI</a></li>
<li><a href="https://datadome.co/guides/bot-protection/bot-mitigation/">Bot Mitigation : Top Techniques to Stop Bot Attacks</a></li>
<li><a href="https://bunny.net/academy/security/bot-detection-and-mitigation-techniques/">Bot Detection and Mitigation Techniques</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了采用静态站点生成和机器人感知 CDN 等替代架构来降低成本。他们还注意到，文章暗示恶意行为者可能不仅仅是在爬取数据，而是为了在预测市场上获得竞争优势。一些人担心这类关闭事件可能成为免费数据源的趋势。

**标签**: `#web scraping`, `#AI`, `#bot detection`, `#system architecture`, `#content security`

---

<a id="item-10"></a>
## [初创企业创始人反对禁止中国开源 AI 模型](https://www.politico.com/news/2026/07/22/startup-founders-urge-trump-not-to-shut-off-chinese-open-weight-ai-01008992) ⭐️ 8.0/10

一群美国初创企业创始人致信特朗普政府，反对禁止中国开源 AI 模型，认为此类禁令无效且会损害美国创新。 这场政策辩论凸显了国家安全关切与推动 AI 进步的开源原则之间的紧张关系；禁令可能扰乱全球 AI 发展，并损害依赖开源模型的初创企业。 开源权重模型提供预训练权重，但不包含完整训练代码或数据，可进行微调但引发滥用担忧。创始人认为禁令无法执行，并可能将 AI 开发推向海外。

hackernews · theanonymousone · 7月23日 15:18 · [社区讨论](https://news.ycombinator.com/item?id=49023016)

**背景**: 开源权重 AI 模型是公开的神经网络权重，开发者可针对特定任务进行微调。中国的 DeepSeek、Qwen 等模型因性能优异而广受欢迎。美国政府以可能被用于虚假信息或监控为由，考虑对其进行限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xigh/open-weight-models">GitHub - xigh/open-weight-models: Curated list of open-weight ...</a></li>
<li><a href="https://onyx.app/self-hosted-llm-leaderboard">Best Self-Hosted LLM Leaderboard 2026 | Open-Weight Model ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍反对禁令，认为恶意行为者不会遵守，且模型蒸馏在法律上不构成知识产权盗窃。有人指出开源模型有利于初创企业，监管俘获可能压制竞争。

**标签**: `#AI policy`, `#open-source AI`, `#geopolitics`, `#technology regulation`, `#Chinese AI`

---

<a id="item-11"></a>
## [ATProto 公共数据与私有应用间的张力](https://lukekanies.com/writing/building-on-atproto/) ⭐️ 8.0/10

Luke Kanies 发表了一篇对 ATProto 协议用于构建应用的设计的批判性分析，指出了协议默认公共数据的模型与需要私有或权限数据的应用之间的固有张力。 这项分析意义重大，因为 ATProto 支撑着 Bluesky 和其他去中心化社交应用；解决这些设计上的张力对于协议在简单社交媒体用例之外的采用至关重要。 文章讨论了一项使用基于位置的访问控制的权限数据提案，有人觉得这种设计令人不适；社区正在积极辩论是否以及如何在不损害 ATProto 核心目标的情况下纳入私有数据功能。

hackernews · speckx · 7月23日 18:23 · [社区讨论](https://news.ycombinator.com/item?id=49025984)

**背景**: ATProto（认证传输协议）是为社交网络应用设计的去中心化协议，默认所有数据都是公开的。它是 Bluesky 的基础。该协议的架构鼓励对用户数据的开放访问，但这与需要私有或权限数据的应用（如企业工具或私密社区）的需求相冲突。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AT_Protocol">AT Protocol - Wikipedia</a></li>
<li><a href="https://atproto.com/guides/overview">Protocol Overview - AT Protocol</a></li>
<li><a href="https://atproto.com/">AT PROTOCOL</a></li>

</ul>
</details>

**社区讨论**: 像 pfraze（ATProto 团队成员）这样的评论者承认当前权限数据提案的尴尬，并表示他们仍在收集反馈。其他评论者，如 ekosz，认为试图将私有数据强加于一个默认公开的协议是方枘圆凿。一些人分享了在 ATProto 上构建应用的积极体验，而另一些人则质疑 ActivityPub 是否更合适。

**标签**: `#ATProto`, `#decentralized protocols`, `#social media`, `#Bluesky`, `#permissions`

---

<a id="item-12"></a>
## [500 行 C++实现软件渲染教程](https://haqr.eu/tinyrenderer/) ⭐️ 8.0/10

该教程由 haqr.eu 提供，教授如何仅用 500 行纯 C++代码从头实现软件渲染器，涵盖光栅化和变换等图形学基础概念。 它提供了不依赖硬件 API 的低层图形编程实践入门，帮助开发者理解核心渲染管线。对教育和希望构建自定义渲染系统的人意义重大。 该实现使用纯 C++，无外部库依赖，专注于逐像素光栅化。它在图形编程社区中因其简洁性和教育价值而受到广泛赞誉。

hackernews · mpweiher · 7月23日 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49022038)

**背景**: 软件渲染使用 CPU 而非专用图形硬件（如 GPU）生成图像。光栅化是将矢量图形（如三角形）转换为屏幕像素的过程。本教程从头讲解从模型加载到像素输出的整个渲染管线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Software_rendering">Software rendering</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rasterisation">Rasterisation</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了用 Rust 等语言实现该教程的个人经验，并称赞其价值。有人希望增加三角形裁剪的讲解，也有人怀念像 Foley/Van Dam 这样的经典计算机图形学书籍。

**标签**: `#software rendering`, `#C++`, `#graphics programming`, `#education`, `#tutorial`

---

<a id="item-13"></a>
## [软件工厂因缺乏更好指标与强化学习而失败](https://github.com/humanlayer/advanced-context-engineering-for-coding-agents/blob/main/wsff.md) ⭐️ 8.0/10

一篇新的批评文章指出，以拉取请求和提交次数来衡量生产力的“软件工厂”方法存在根本缺陷，真正的进步需要针对代码质量的强化学习以及像 MaintainabilityBench 这样的更好基准。 这很重要，因为随着 AI 编码代理变得更加普遍，有缺陷的指标可能导致代码质量下降和不可持续的工程实践，而提出的向基于强化学习的代码健康转变可能重塑团队评估和信任 AI 贡献的方式。 文章建议，通过 PR 和提交来测量代理生产力忽略了代码质量和可维护性，并提出一个'MaintainabilityBench'，奖励重构和检测代码重复，而不是盲目添加代码。

hackernews · dhorthy · 7月23日 15:18 · [社区讨论](https://news.ycombinator.com/item?id=49023019)

**背景**: “软件工厂”方法将软件开发视为自动化流水线，AI 代理被分配工单并通过吞吐量评判。“缰绳工程”是塑造 AI 编码代理所见内容、所能执行的操作以及其工作如何被检查的实践，强调模型-缰绳-人类的动态。该批评认为，没有适当的指标和针对代码健康的强化学习，这样的工厂会产生低质量代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.faros.ai/blog/harness-engineering">Harness Engineering : Making AI Coding Agents Work in 2026</a></li>
<li><a href="https://goat-flow.com/what-is-harness-engineering">Harness Engineering : Guardrails and memory for AI coding agents</a></li>
<li><a href="https://everforthecs.com/ecs-insight/article/what-should-your-ai-factory-look-like/">What Should Your AI Factory Look Like? — Everforth ECS</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为像 PR 和提交这样的传统指标不充分，有人称其为“bos”（一堆屎）。对于强化学习和基准测试的想法有热情，但对时间线说法持怀疑态度，指出代理能力直到 2025 年底后才显著提升。一些人还批评 PR 审查本身的用户体验是一个瓶颈。

**标签**: `#software factories`, `#coding agents`, `#AI productivity`, `#code quality`, `#reinforcement learning`

---

<a id="item-14"></a>
## [CISA 警告 Weintek cMT3092X HMI 存在高危漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-204-03) ⭐️ 8.0/10

CISA 于 2025 年 7 月 23 日发布公告（ICSA-26-204-03），警告 Weintek cMT3092X HMI 固件和 EasyWeb 存在多个高危漏洞，CVSS v3 基础评分为 8.8，可导致权限提升和凭据窃取。 这些漏洞影响全球关键制造业，成功利用可让攻击者提升权限或窃取用户凭据，对运营技术（OT）安全构成重大风险。 受影响版本包括 cMT3092X 固件 20210218 之前版本及 EasyWeb v2.1.20 之前版本；厂商发布了补丁包（cmt_typeB_20260316_007.patch），包含 EasyWeb 2.3.17-typeb，可通过联系 Weintek 支持或经销商获取。

rss · CISA Cybersecurity Advisories · 7月23日 12:00

**背景**: Weintek cMT3092X 是一款 9.7 英寸人机界面（HMI）面板，用于工业自动化中的操作控制和监控。HMI 通常运行 Web 服务器，若未妥善保护则易受攻击。漏洞包括依赖未验证的 Cookie（CWE-784）、权限分配不当、密码明文存储以及用户管理错误。

**标签**: `#ICS`, `#security`, `#CISA`, `#vulnerability`, `#OT`

---

<a id="item-15"></a>
## [CISA 警告 Rockwell ThinManager 存在路径遍历漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-204-05) ⭐️ 8.0/10

CISA 发布了一份公告（ICSA-26-204-05），详细描述了 Rockwell Automation ThinManager 13.0.0 至 14.0.2 版本中存在的一个路径遍历漏洞（CVE-2026-11917），CVSS 评分为 8.1。 ThinManager 广泛应用于全球关键基础设施行业的工业控制系统；成功利用此漏洞可使认证攻击者向受限系统目录写入任意文件，可能导致系统被攻陷或中断运行。 该漏洞影响版本 >=13.0.0 <13.0.7、>=13.1.0 <13.1.5、>=13.2.0 <13.2.4 和 >=14.0.0 <14.0.2；修复版本分别为 13.0.8、13.1.6、13.2.5 和 14.0.3。

rss · CISA Cybersecurity Advisories · 7月23日 12:00

**背景**: Rockwell Automation ThinManager 是一个用于工业制造可视化和设备管理的瘦客户端管理平台。路径遍历漏洞（CWE-22）指应用程序未正确验证文件路径，导致攻击者可在预期目录之外写入文件。该公告以 CSAF 格式发布，支持安全工具自动读取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinmanager.com/products/thinmanager.php">ThinManager Overview | ThinManager ®</a></li>

</ul>
</details>

**标签**: `#security`, `#OT`, `#vulnerability`, `#Rockwell Automation`, `#path traversal`

---

<a id="item-16"></a>
## [俄罗斯 APT 组织 LAUNDRY BEAR 利用新漏洞攻击 Zimbra 用户](https://www.cisa.gov/news-events/cybersecurity-advisories/aa26-204a) ⭐️ 8.0/10

自 2025 年 7 月起，俄罗斯政府支持的 APT 组织 LAUNDRY BEAR 针对 Zimbra Collaboration Suite 用户发起钓鱼攻击，利用零日漏洞（CVE-2025-66376），仅需查看恶意邮件即可窃取电子邮件数据。 此次攻击表明 LAUNDRY BEAR 转向更复杂的技术手段，针对西方政府和商业组织窃取敏感邮件数据，可能进一步助长间谍活动或影响力行动。 该漏洞利用基于查看操作，只需用户在存在漏洞的 Zimbra Web 客户端中查看邮件即可触发，尝试窃取最近 90 天的邮件、全局地址列表并建立持久访问。

rss · CISA Cybersecurity Advisories · 7月23日 12:00

**背景**: Zimbra Collaboration Suite 是一款广泛使用的电子邮件和协作平台，尤其在政府和商业领域。漏洞 CVE-2025-66376 已于 2025 年 11 月修复，但未修补的系统仍然面临风险。LAUNDRY BEAR 此前因网络间谍活动被荷兰情报机构及其他机构追踪。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zimbra_Collaboration_Suite">Zimbra Collaboration Suite</a></li>
<li><a href="https://thedailytechfeed.com/dutch-intelligence-unveils-russian-laundry-bear-cyber-espionage-targeting-police-and-nato/">Dutch Intelligence Unveils Russian ' Laundry Bear ' Cyber Espionage...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#Russian APT`, `#phishing`, `#Zimbra`, `#threat intelligence`

---

<a id="item-17"></a>
## [CISA 警告 MZ Automation libIEC61850 存在严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-204-06) ⭐️ 8.0/10

CISA 发布公告（ICSA-26-204-06），披露了 MZ Automation libIEC61850 1.0.0 至 1.6.1 版本中存在多个缓冲区溢出和空指针解引用漏洞，未认证的网络邻近攻击者可利用这些漏洞导致服务崩溃或执行任意代码。 由于 libIEC61850 广泛应用于能源、制造等关键基础设施领域的变电站 IEC 61850 通信中，这些漏洞可能导致电网监控和控制功能中断，影响全球范围。 漏洞包括基于栈的缓冲区溢出（CVE-2026-50039，CVSS 3.1 基础评分 7.5）和基于堆的缓冲区溢出（CVE-2026-49035，CVSS 4.0 基础评分 8.7），在 ASLR 禁用时已验证可实现远程代码执行。

rss · CISA Cybersecurity Advisories · 7月23日 12:00

**背景**: IEC 61850 是变电站通信协议的国际标准，实现智能电子设备（IED）之间的互操作性。libIEC61850 是此标准的开源 C 语言实现，常用于嵌入式系统和 SCADA 环境。漏洞影响 IEC 61850 通信核心的 MMS（制造报文规范）协议处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/mz-automation/libiec61850">GitHub - mz-automation/libiec61850: Official repository for ...</a></li>
<li><a href="https://libiec61850.com/downloads/">Downloads | libIEC61850 / lib60870</a></li>
<li><a href="https://www.mz-automation.de/">MZ Automation - Leading Experts in Communication Protocols</a></li>

</ul>
</details>

**标签**: `#security`, `#industrial control systems`, `#IEC61850`, `#buffer overflow`, `#CISA`

---

<a id="item-18"></a>
## [Panduit IntraVUE 关键漏洞可远程接管工业控制系统设备](https://www.cisa.gov/news-events/ics-advisories/icsa-26-204-04) ⭐️ 8.0/10

美国网络安全与基础设施安全局（CISA）披露了 Panduit IntraVUE 版本 3.2.1a14 及之前版本中的多个高危漏洞，包括明文密码存储和可绕过 OT 网络分段的混淆代理问题。 这些漏洞使攻击者在拥有 IT 网络访问权限的情况下，无需物理接触或专业知识即可远程操控工业控制设备，对全球关键基础设施行业构成严重威胁。 混淆代理漏洞（CVE-2026-42933）允许攻击者利用活跃代理绕过 OT 网络分段，而明文密码问题（CVE-2026-40430）通过 API 暴露明文凭证。这两个漏洞的 CVSS v3 基础评分均为 10（严重）。

rss · CISA Cybersecurity Advisories · 7月23日 12:00

**背景**: Panduit IntraVUE 是一款工业以太网可视化与监控工具，用于检测和诊断运营技术环境中的网络问题。它广泛应用于全球的关键制造业、能源和水利行业。此类软件中的漏洞可能使攻击者从 IT 网络跳转到 OT 网络，破坏运营或造成物理损害。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.panduit.com/content/dam/panduit/en/website/solutions/documents/solution-pdf/NI-IN-CPFL133-ENG.pdf">IntraVUE Industrial Ethernet Visualization and ... - Panduit</a></li>
<li><a href="https://www.panduit.com/content/dam/panduit/en/products/media/4/94/894/3894/110103894.pdf">IntraVUETM by Panduit</a></li>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#ICS`, `#CISA`, `#vulnerability`, `#Panduit IntraVUE`

---

<a id="item-19"></a>
## [Claude Cowork 沙箱逃逸漏洞影响 50 万 Mac 用户](https://thehackernews.com/2026/07/claude-cowork-flaw-could-let-ai-agent.html) ⭐️ 8.0/10

研究人员发现 Anthropic 的 Claude Cowork 存在一个沙箱逃逸漏洞，允许 AI 代理突破其 Linux 虚拟机，在宿主机 Mac 上读写文件，影响约 50 万 macOS 用户。 该漏洞凸显了关键的 AI 安全问题，表明运行在看似隔离环境中的 AI 代理可以逃脱并访问敏感用户数据，可能导致大规模数据泄露。 该漏洞由 Accomplish AI 披露，The Hacker News 报道。这是一个经典的沙箱逃逸漏洞，AI 代理绕过了 Linux 虚拟机的边界，与 macOS 文件系统进行交互。

rss · The Hacker News · 7月23日 13:27

**背景**: Claude Cowork 是 Anthropic 的一款 AI 代理，运行在用户桌面上执行多步骤任务，为了安全隔离而运行在 Linux 虚拟机内。沙箱逃逸漏洞是指代码逃离受限环境，获得对宿主系统的未授权访问。近期研究显示，安全社区越来越关注 AI 代理沙箱的安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://www.pillar.security/blog/the-week-of-sandbox-escapes">The Week of Sandbox Escapes - pillar.security</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#AI safety`, `#vulnerability`, `#sandbox escape`, `#Claude Cowork`

---

<a id="item-20"></a>
## [Chaos 勒索软件利用 msaRAT 通过无头浏览器路由 C2 通信](https://thehackernews.com/2026/07/chaos-ransomware-uses-msarat-to-route.html) ⭐️ 8.0/10

Chaos 勒索软件组织部署了一种名为 msaRAT 的新型 Rust 后门，该后门通过受害者自己的无头 Chrome 或 Edge 浏览器路由命令与控制（C2）流量，从而避免直接的出站网络连接。 这种技术使 C2 流量看似合法的浏览器活动，从而规避传统的基于网络的检测和防火墙规则，代表了勒索软件隐蔽战术的重大演变。 该植入程序仅与 127.0.0.1 通信，通过生成无头浏览器来中继命令，并利用 WebRTC over TURN 向受害者隐藏攻击者的真实 IP 地址。

rss · The Hacker News · 7月23日 13:11

**背景**: 无头浏览器是一种没有图形用户界面的网络浏览器，常用于自动化测试和网页抓取。攻击者可以滥用它，通过合法的浏览器进程代理恶意流量，从而增加检测难度。msaRAT 后门用 Rust 编写，通过在无头模式下启动 Chrome 或 Edge 并驱动浏览器与 C2 服务器通信，体现了这一技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Headless_browser">Headless browser - Wikipedia</a></li>
<li><a href="https://developer.chrome.com/docs/chromium/headless">Chrome Headless mode | Chromium | Chrome for Developers</a></li>

</ul>
</details>

**标签**: `#ransomware`, `#C2`, `#headless browser`, `#security research`, `#msaRAT`

---