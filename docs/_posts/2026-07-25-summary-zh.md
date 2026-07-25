---
layout: default
title: "Horizon Summary: 2026-07-25 (ZH)"
date: 2026-07-25
lang: zh
---

> 从 54 条内容中筛选出 20 条重要资讯。

---

1. [IRGC 声称摧毁了 AWS 巴林数据中心](#item-1)
2. [Anthropic 发布 Claude Opus 5，无数据保留要求](#item-2)
3. [WeLM 617B MoE：隐式缩放实现 AI 新缩放定律](#item-3)
4. [Black Forest Labs 发布 FLUX 3 多模态流模型](#item-4)
5. [Certighost 漏洞允许低权限用户模拟域控制器](#item-5)
6. [Bing 图片 SVG 漏洞可完全控制系统](#item-6)
7. [Kimi K3 代理发现 Redis 零日漏洞，研究人员报告](#item-7)
8. [利用 CVE-2026-46331 逃逸 Claude Cowork 的本地 VM 沙箱](#item-8)
9. [Postgres LISTEN/NOTIFY 实际可扩展](#item-9)
10. [韩华摄像头泄露 GitHub 管理员令牌](#item-10)
11. [科技巨头警告不要过度监管开放权重 AI 模型](#item-11)
12. [如果编码已被解决，为何软件越来越差？](#item-12)
13. [Flux 3 世界模型提取用于机器人技术](#item-13)
14. [ChatGPT AgentForger 漏洞可通过钓鱼链接部署恶意智能体](#item-14)
15. [黑客使用 Hermes AI 代理对泰国财政部发动无人值守攻击](#item-15)
16. [NodeBB 修复八项 AI 发现的高危漏洞](#item-16)
17. [虚假 Notepad++ 插件传播 MATCHBOIL.V2 恶意软件](#item-17)
18. [BlueNoroff 利用 Zoom 钓鱼工具包分析加密钱包](#item-18)
19. [AI 代理最小权限执行仍面临挑战](#item-19)
20. [黄金鸡威胁组织携四个新恶意软件家族重现](#item-20)

---

<a id="item-1"></a>
## [IRGC 声称摧毁了 AWS 巴林数据中心](https://houseofsaud.com/irgc-claims-destroyed-amazon-bahrain-data-center/) ⭐️ 10.0/10

伊斯兰革命卫队（IRGC）声称对亚马逊云服务（AWS）在巴林的数据中心被摧毁负责，这是该地区地缘政治紧张局势升级的一部分。 对主要云服务提供商基础设施的物理攻击凸显了集中式云服务在地缘政治冲突中的脆弱性，可能影响中东地区的 AWS 客户，并引发对数据中心安全的担忧。 AWS 的 me-south-1 区域包含三个数据中心；社区报告显示，位于麦纳麦的 BAH53 设施受损，一个变电站约在 2026 年 7 月 16 日被击中，主建筑在 7 月 22 日前受损。AWS 健康状态仪表板自 4 月 30 日起显示不可用。

hackernews · thisislife2 · 7月24日 09:52 · [社区讨论](https://news.ycombinator.com/item?id=49033240)

**背景**: AWS 区域由多个可用区组成，每个可用区包含一个或多个数据中心。中东地区一直面临问题：阿联酋可用区已瘫痪数月，沙特阿拉伯仍在建设中，如今巴林离线，该地区仅剩特拉维夫区域仍在运营。

**社区讨论**: 评论者指出，中东唯一仍在运营的 AWS 区域位于特拉维夫，具有讽刺意味，并强调此类攻击揭示了集中式基础设施的脆弱性。还分享了具体的技术细节和损坏时间线。

**标签**: `#cloud infrastructure`, `#cybersecurity`, `#geopolitics`, `#AWS`, `#data center attack`

---

<a id="item-2"></a>
## [Anthropic 发布 Claude Opus 5，无数据保留要求](https://www.anthropic.com/news/claude-opus-5) ⭐️ 9.0/10

Anthropic 发布了其最强大的旗舰模型 Claude Opus 5，该模型在各项基准测试中性能显著提升，并且对通用访问没有数据保留要求。 此次发布使组织能够使用前沿模型，而不必像竞争对手 Fable 那样受 30 天数据保留政策的限制，可能重塑企业 AI 采用格局，并加速 AI 模型路由这一日益增长的趨勢。 在社区测试中，Opus 5 在图像转 HTML 任务上表现优于 Fable，同时保留了其前身 Opus 4.8 独特的写作风格（“Claude 式表达”）。一份长达 190 页的系统卡已发布，详细记录了安全评估和能力。

hackernews · alvis · 7月24日 16:57 · [社区讨论](https://news.ycombinator.com/item?id=49038433)

**背景**: 数据保留政策规定了 AI 提供商存储用户输入和输出的时长，这通常是具有严格合规需求的企业所关注的。模型路由是指智能系统将提示词匹配到最合适的大型语言模型，由于多个提供商推出的模型数量激增，这成为一个快速增长领域。Opus 5 延续了 Anthropic 的高能力模型系列，直接与 Fable 和 Gemini 等产品竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/foundry/openai/concepts/model-router">Model router for Microsoft Foundry concepts - Microsoft Foundry</a></li>
<li><a href="https://github.com/Not-Diamond/awesome-ai-model-routing">A curated list of approaches to AI model routing - GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区强调无数据保留要求是最重要的方面，一位用户指出这使组织能够使用类似 Fable 的模型而不受其 30 天保留政策约束。其他人讨论了在图像转 HTML 等实际任务中的性能改进，并指出由于模型变体激增，模型路由是 AI 中增长最快的领域。

**标签**: `#AI`, `#LLM`, `#Claude`, `#Anthropic`, `#model release`

---

<a id="item-3"></a>
## [WeLM 617B MoE：隐式缩放实现 AI 新缩放定律](https://mp.weixin.qq.com/s?__biz=MzI3MTA0MTk1MA==&mid=2652714734&idx=1&sn=7e98659aa2ab44778c0d5587a1aa8a84) ⭐️ 9.0/10

微信团队发布了 WeLM 617B MoE，这是一个 6170 亿参数的混合专家模型，通过隐式缩放展示了 AI 的第三条缩放定律；该模型仅用了完整训练计算量的 5.3%就从 80B 参数扩展到 617B 参数，并在 9 个评测中超越自回归基线。 这项成果挑战了传统缩放定律，表明隐式推理可以高效缩放，可能大幅降低训练成本，用更少的数据实现更大的模型；这可能会影响大语言模型开发和 AI 研究的未来方向。 该模型使用混合专家（MoE）架构，总参数 6170 亿，但每个 token 仅激活一个子集，从 80B 检查点增量续训节省了 94.7%的计算量；它在 9 个评测中超越自回归模型，表明隐式推理随深度而非宽度缩放。

rss · 新智元 · 7月24日 04:33

**背景**: AI 缩放定律传统上将模型性能与参数、数据和计算量相关联；混合专家（MoE）通过每个输入仅激活相关专家网络来提高效率。隐式缩放是指在不需要显式逐步计算的情况下扩展推理能力，可能为高级 AI 提供更计算高效的路径。WeLM 617B MoE 基于这些概念提出了专注于隐式推理深度的第三条缩放定律。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.sina.cn/2026-07-24/detail-iniiwrah9261623.d.html?vt=4&cid=76993&node_id=76993">把思考折叠进序列：WeLM 617B MoE的隐式Scaling路径|scaling law|Token|大模型|微信|博客_手机新浪网</a></li>
<li><a href="https://www.163.com/dy/article/L2JT6QAK0511ABV6.html">把思考折叠进序列：WeLM 617B MoE的隐式Scaling路径|预训练|scaling_网易订阅</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>

</ul>
</details>

**标签**: `#AI`, `#scaling laws`, `#mixture of experts`, `#large language models`, `#WeLM`

---

<a id="item-4"></a>
## [Black Forest Labs 发布 FLUX 3 多模态流模型](https://www.latent.space/p/ainews-black-forest-labs-flux-3-multimodal) ⭐️ 9.0/10

Black Forest Labs 发布了 FLUX 3，这是一个统一的多模态流模型，可处理图像、视频、音频和动作预测，性能超越了 Seedance 2.0、Gemini Omni 和 Grok Imagine。他们还推出了 FLUX-mimic，一个视频动作机器人模型。 这代表了多模态 AI 的重大进步，FLUX 3 在多种模态上取得了最先进的结果，并引入了机器人组件，可能加速具身 AI 和内容创作的发展。 FLUX 3 是一个开放权重的模型（FLUX 3 Dev），可提前访问，但完整的 32B 参数版本可能较重；预计后续会推出更小的版本，如 FLUX 2 Klein。该模型采用统一架构，从图像、视频和音频中联合学习。

rss · Latent Space · 7月24日 04:30

**背景**: 多模态流模型是一类生成模型，学习多种模态之间数据分布的概率流，可实现文本到图像、文本到视频和音频生成等任务。字节跳动（Seedance）、Google（Gemini Omni）和 xAI（Grok Imagine）等公司发布了具有竞争力的多模态模型。Black Forest Labs（BFL）之前发布了 FLUX.2，FLUX 3 进一步推进了前沿。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bfl.ai/blog/flux-3">FLUX 3 - Real World Models: Towards Multimodal Flow Models as the Backbone of Visual Intelligence. | Black Forest Labs</a></li>
<li><a href="https://www.latent.space/p/ainews-black-forest-labs-flux-3-multimodal">[AINews] Black Forest Labs FLUX 3 - Multimodal Flow Models that beat Seedance 2.0, Gemini Omni and Grok Imagine, and FLUX-mimic video-action robotics model</a></li>
<li><a href="https://www.reddit.com/r/StableDiffusion/comments/1v4gpka/flux_3_real_world_models_towards_multimodal_flow/">r/StableDiffusion on Reddit: FLUX 3 - Real World Models: Towards Multimodal Flow Models as the Backbone of Visual Intelligence.</a></li>

</ul>
</details>

**社区讨论**: Reddit 上 r/StableDiffusion 的讨论提到了开放权重访问和对更小高效版本的期待。情绪总体正面，但承认当前模型大小需要大量计算。

**标签**: `#AI`, `#multimodal`, `#flow models`, `#robotics`, `#computer vision`

---

<a id="item-5"></a>
## [Certighost 漏洞允许低权限用户模拟域控制器](https://thehackernews.com/2026/07/certighost-exploit-lets-low-privileged.html) ⭐️ 9.0/10

研究员于 7 月 24 日发布了名为 Certighost（CVE-2026-54121）的可用漏洞利用代码，允许任何低权限 Active Directory 用户获取模拟域控制器的证书，进而通过 DCSync 攻击提取域机密。 该漏洞构成一条从低权限域用户到完全域管理员控制的严重提权路径，因为被模拟的域控制器可通过 DCSync 窃取 krbtgt 秘密及所有密码哈希值。这对使用 Active Directory 证书服务（AD CS）的组织构成严重风险，尤其对那些未对证书模板设置适当访问控制的组织。 该漏洞利用针对 AD CS 中的一种配置错误，允许低权限用户请求本应为域控制器保留的证书模板。一旦获取该证书，即可通过 Kerberos 身份验证模拟域控制器，进而获得 DCSync 所需的复制权限。

rss · The Hacker News · 7月24日 14:15

**背景**: Active Directory 证书服务（AD CS）提供域内颁发证书的公钥基础设施。域控制器拥有特殊权限，包括 DCSync 攻击所需的目录复制权限，可获取密码哈希值。如果为域控制器设计的证书模板配置错误，允许任何用户注册，攻击者便可利用这一点提升权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/certighost-exploit-lets-low-privileged.html">Certighost Exploit Lets Low-Privileged Active Directory Users Impersonate a Domain Controller</a></li>
<li><a href="https://github.com/aniqfakhrul/CVE-2026-54121">GitHub - aniqfakhrul/CVE-2026-54121: Certighost POC · GitHub</a></li>
<li><a href="https://sudoflare.com/technews/certighost-exploit-active-directory-domain-controller-2026/">Certighost Exploit 2026: Any User Can Hijack Active Directory - SudoFlare</a></li>

</ul>
</details>

**标签**: `#Active Directory`, `#security`, `#privilege escalation`, `#certificate exploit`, `#DCSync`

---

<a id="item-6"></a>
## [Bing 图片 SVG 漏洞可完全控制系统](https://thehackernews.com/2026/07/bing-images-flaws-let-crafted-svgs-run.html) ⭐️ 9.0/10

XBOW 研究人员发现，向 Bing 图片提交特制 SVG 文件可在 Windows 服务器上以 NT AUTHORITY\SYSTEM 权限执行任意命令，在 Linux 服务器上以 root 权限执行。微软发布了两个关键 CVE（CVE-2026-32191 和 CVE-2026-32194）来修复这些漏洞。 像 Bing 图片这样广泛使用的服务存在此类漏洞，可能允许攻击者完全入侵微软的生产服务器，进而访问敏感数据或渗透到内部网络。该问题在多台主机上均存在，表明 Bing 图像处理流水线存在系统性缺陷。 攻击通过两种方式实现：托管恶意 SVG 并通过 imgurl 参数将 URL 提供给 Bing 爬虫（CVE-2026-32191），或直接上传 SVG（CVE-2026-32194）。XBOW 在不同主机和网络范围内均得到相同结果，排除了单台机器被感染的可能。

rss · The Hacker News · 7月24日 11:45

**背景**: SVG（可缩放矢量图形）是一种基于 XML 的图像格式，允许嵌入脚本和外部实体。Windows 中的 NT AUTHORITY\SYSTEM 账户拥有最高本地权限，等同于 Linux 的 root。命令注入发生在用户提供的数据在被传递给 shell 之前未正确清理的情况下。在此案例中，Bing 的图像处理工作线程可能不安全地解析 SVG 文件，导致 XML 外部实体（XXE）攻击或直接命令注入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/bing-images-flaws-let-crafted-svgs-run.html">Bing Images Flaws Let Crafted SVGs Run Commands as SYSTEM on Microsoft's Servers</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows/win32/services/localsystem-account">LocalSystem Account - Win32 apps | Microsoft Learn</a></li>
<li><a href="https://hackerone.com/reports/845832">Lab45 disclosed on HackerOne: SVG file upload leads to XML injection</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Microsoft`, `#RCE`, `#SVG`

---

<a id="item-7"></a>
## [Kimi K3 代理发现 Redis 零日漏洞，研究人员报告](https://thehackernews.com/2026/07/kimi-k3-agents-found-redis-zero-days.html) ⭐️ 9.0/10

研究人员发现了 Redis 中的多个零日漏洞，可通过 RESTORE 命令实现经过身份验证的远程代码执行，导致 Redis 于 7 月 23 日发布了七个紧急安全版本，涵盖 6.2.23、7.2.15 和 7.4.10 版本。 这一点至关重要，因为 Redis 是最广泛使用的内存数据存储之一，经过身份验证的 RCE 可让攻击者完全控制受影响的系统，尤其是在认证较弱的环境中。 四个利用链都要求使用 RESTORE 命令；基于 Streams 的链还需要 EVAL 和 XGROUP，而 8.8.0 链额外需要 EVAL 和捆绑的 RedisBloom 模块。Redis 表示底层内存缺陷可能导致远程代码执行。

rss · The Hacker News · 7月24日 06:58

**背景**: Redis 中的 RESTORE 命令从 DUMP 反序列化数据以重新创建键，EVAL 命令在服务器端执行 Lua 脚本。RedisBloom 模块提供概率性数据结构。这些漏洞利用了反序列化或脚本执行过程中的内存损坏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://redis.io/docs/latest/commands/restore/">RESTORE | Docs</a></li>
<li><a href="https://redis.io/docs/latest/commands/eval/">EVAL | Docs - Redis</a></li>
<li><a href="https://github.com/RedisBloom/RedisBloom">GitHub - RedisBloom / RedisBloom : Probabilistic Datatypes Module ...</a></li>

</ul>
</details>

**标签**: `#security`, `#redis`, `#vulnerability`, `#RCE`, `#zeroday`

---

<a id="item-8"></a>
## [利用 CVE-2026-46331 逃逸 Claude Cowork 的本地 VM 沙箱](https://www.reddit.com/r/netsec/comments/1v52lix/escaping_claude_coworks_local_vm_sandbox_via/) ⭐️ 9.0/10

一名安全研究人员展示了如何利用 CVE-2026-46331（一个 Linux 内核中 net/sched pedit 模块的漏洞，导致页缓存损坏）从 Claude Cowork 的本地 VM 沙箱中逃逸。 该漏洞可能允许攻击者突破沙箱，获得对主机的未授权访问，从而危及敏感数据或执行任意代码。 该利用利用了一个内核漏洞，其中写时复制范围被错误计算，导致部分缓冲区无法写入并损坏页缓存，这可能导致权限提升或数据完整性问题。

reddit · r/netsec · /u/natcoba · 7月24日 05:53

**背景**: Claude Cowork 是一款 AI 代理，在用户本地机器的沙箱化 VM 内执行任务以限制访问。沙箱逃逸是指恶意进程突破 VM 隔离。CVE-2026-46331 是 2026 年 6 月披露的一个 Linux 内核流量控制子系统漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2026-46331">NVD - CVE-2026-46331</a></li>
<li><a href="https://coworkerai.io/claude-cowork-sandbox">Claude Cowork Sandbox — Permissions & Safe Execution</a></li>
<li><a href="https://github.com/advisories/GHSA-cr2w-747q-47qc">CVE-2026-46331 - GitHub Advisory Database</a></li>

</ul>
</details>

**标签**: `#CVE`, `#sandbox escape`, `#security`, `#vulnerability`, `#VM`

---

<a id="item-9"></a>
## [Postgres LISTEN/NOTIFY 实际可扩展](https://www.dbos.dev/blog/postgres-listen-notify-scalability) ⭐️ 8.0/10

DBOS 博客文章证明，PostgreSQL 的 LISTEN/NOTIFY 机制每秒可处理 6 万条通知，反驳了之前认为其不可扩展的说法。 这一发现对于在 PostgreSQL 上构建实时应用的开发者非常重要，它表明 LISTEN/NOTIFY 可以支持高吞吐消息传递，无需引入外部消息代理。 文章指出，之前的性能问题主要源于早期版本中锁机制不佳，而现代 PostgreSQL 已解决这些问题。测试在单台服务器上达到了每秒 6 万条通知。

hackernews · KraftyOne · 7月24日 19:05 · [社区讨论](https://news.ycombinator.com/item?id=49040296)

**背景**: LISTEN/NOTIFY 是 PostgreSQL 内置功能，允许数据库客户端在指定事件发生时接收异步通知。常用于实时更新、聊天应用和协调分布式系统。2025 年 7 月的一个热门 Hacker News 帖子声称 LISTEN/NOTIFY 不可扩展，因此引发了这篇反驳文章。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/sql-notify.html">PostgreSQL: Documentation: 18: NOTIFY</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-listen.html">PostgreSQL: Documentation: 18: LISTEN</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-01-25-use-listen-notify-real-time-postgresql/view">How to Use Listen/Notify for Real-Time Updates in PostgreSQL</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍欢迎这一纠正，有人指出可扩展性是一个连续谱而非二元属性。一位用户提到了之前 321 条评论的讨论，另一位指出原帖已包含勘误。讨论氛围积极，聚焦于正确使用和扩展因子。

**标签**: `#postgres`, `#scalability`, `#database`, `#messaging`, `#performance`

---

<a id="item-10"></a>
## [韩华摄像头泄露 GitHub 管理员令牌](https://hhh.hn/hanwha-github-token/) ⭐️ 8.0/10

韩华（Hanwha）安防摄像头的登录页面中被发现硬编码了一个 GitHub 管理员令牌，可对该公司的仓库进行广泛访问。 这一严重漏洞暴露了知识产权和源代码，反映了物联网设备中糟糕的安全实践以及硬编码凭证的危险。 该令牌以明文凭证的形式嵌入登录页面的 HTML/JavaScript 中，并拥有对韩华 GitHub 组织的管理员级权限。

hackernews · hhh · 7月24日 11:54 · [社区讨论](https://news.ycombinator.com/item?id=49034292)

**背景**: 硬编码凭证是嵌入源码或固件中的明文密钥，虽常见但风险很高。GitHub 个人访问令牌（PAT）用于 API 认证，一旦泄露可危及仓库安全。韩华是韩国大型电子公司，生产安防摄像头。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.beyondtrust.com/resources/glossary/hardcoded-embedded-passwords">What are Hardcoded Passwords/Embedded Credentials? | BeyondTrust</a></li>
<li><a href="https://apiiro.com/glossary/hardcoded-credentials/">What Are Hardcoded Credentials? Examples & Detection</a></li>
<li><a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens">Managing your personal access tokens - GitHub Docs</a></li>

</ul>
</details>

**社区讨论**: 评论区表达了对物联网安全的失望，并提及其他设备也存在类似问题。许多人建议通过网络分段（如 VLAN）隔离摄像头，也有人指出消费电子产品中硬编码凭证的普遍趋势。

**标签**: `#security`, `#IoT`, `#vulnerabilities`, `#GitHub`, `#supply chain`

---

<a id="item-11"></a>
## [科技巨头警告不要过度监管开放权重 AI 模型](https://www.cnbc.com/2026/07/24/nvidia-microsoft-meta-open-weight-ai-models.html) ⭐️ 8.0/10

这三大 AI 巨头联合表态标志着行业对拟议监管的重大反弹，可能影响美国 AI 政策以及开源与专有 AI 开发之间的未来平衡。 该公开信以 PDF 形式由 Nvidia 发布，并附有黄仁勋的 X 帖子以及一篇关于硅谷在对待中国 AI 问题上分裂的 Wired 文章链接。这些公司主张进行有针对性的监管，而非对开放权重模型进行全面限制。

hackernews · louiereederson · 7月24日 13:32 · [社区讨论](https://news.ycombinator.com/item?id=49035303)

**背景**: 开放权重 AI 模型是指其训练参数（权重）公开发布，允许任何人下载、运行和微调的模型。这与仅通过 API 访问的封闭模型（如 GPT-4）形成对比。随着来自中国的开放权重模型（如 DeepSeek 和阿里巴巴的模型）在全球获得关注，有关监管的辩论加剧，引发了安全和竞争力方面的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者将此事与 SOPA 抗议活动相提并论，部分人指出封闭源代码游说团体（Anthropic、OpenAI）现在被包括 Musk 在内的开放权重支持者压制。有一种观点认为，这封联合公开信反映了行业分歧：Anthropic 捐赠 4000 万美元用于推动模型监管的政治努力，而其他人担心过度监管可能导致 AI 领导权拱手让给中国。

**标签**: `#AI regulation`, `#open-weight AI`, `#tech policy`, `#industry lobbying`

---

<a id="item-12"></a>
## [如果编码已被解决，为何软件越来越差？](https://ptrchm.com/posts/nothing-works-and-everyone-is-euphoric/) ⭐️ 8.0/10

文章指出，尽管 AI 代码生成取得突破，但软件质量却在下降，因为速度优先于正确性，且用户体验决策不佳。 这一悖论凸显了当前软件行业的关键缺陷：AI 加速开发但未解决市场激励问题——市场奖励快速发布而非构建稳健软件，影响所有用户。 文章引用了具体的用户体验失败案例，如 Slack 在 macOS 上抢夺焦点，并指出 AI 代码生成改变了'快速'的定义，但未能提高对正确性的信心。

hackernews · pchm · 7月24日 09:08 · [社区讨论](https://news.ycombinator.com/item?id=49033004)

**背景**: AI 代码生成工具如 GitHub Copilot 和 ChatGPT 能够根据自然语言提示快速生成代码，使经验丰富的工程师一小时内完成以往一周的工作。然而，这些工具本身并不验证正确性或考虑整体用户体验，导致大量功能丰富但有缺陷的软件。市场往往奖励快速迭代而非彻底测试，加剧了问题。

**社区讨论**: 评论者普遍对软件更新引入回归感到沮丧，有人指出非 Linux 系统上的更新'简直可怕'。另一位评论者强调，市场激励历来偏向速度而非质量，AI 并未改变这一点。一位技术用户指出 KDE Plasma 的焦点窃取预防功能是 macOS 所缺乏的，说明糟糕的 UX 决策的影响。

**标签**: `#software quality`, `#AI code generation`, `#developer experience`, `#Hacker News discussion`

---

<a id="item-13"></a>
## [Flux 3 世界模型提取用于机器人技术](https://bfl.ai/blog/flux-3-mimic) ⭐️ 8.0/10

Black Forest Labs 从其 Flux 3 多模态视频生成模型中提取了内部世界表征，并将其应用于机器人技术，展示了成功的真实世界任务执行。 这一突破表明，先进的视频生成模型内在地学习了世界模型，可以重新用于机器人技术，可能加速通用机器人的发展，而无需为每项任务单独训练。 该方法虽然前景广阔，但与专门方法相比，产生的表征解耦程度较低，这可能限制其在需要深入理解世界的任务中的实用性。视频演示中，机械臂尝试了三次才重新安装车窗饰条，突出了能力与当前局限性。

hackernews · kensai · 7月24日 09:31 · [社区讨论](https://news.ycombinator.com/item?id=49033127)

**背景**: AI 中的世界模型是机器学习系统，它们构建环境的内部表征，预测环境如何随时间变化以响应动作。Black Forest Labs 的 Flux 3 是一个多模态模型，在图像、视频和音频上进行训练，学习世界的统一表征。这项工作是将'世界模型'用于机器人技术的更广泛趋势的一部分，从视频中学习的内部动态可以指导物理动作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bfl.ai/blog/flux-3">FLUX 3 - Real World Models: Towards Multimodal Flow Models as the Backbone of Visual Intelligence. | Black Forest Labs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Flux_(text-to-image_model)">Flux (text-to-image model) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence)</a></li>

</ul>
</details>

**社区讨论**: 评论者认为这种方法有趣，许多人注意到视频实验室转变为机器人实验室的新颖性。有人指出了描述表征为'解耦程度较低'的哲学讽刺。其他人评论了令人印象深刻但有些令人不安的机械臂视频，并对欧洲初创公司的合作表示赞赏。

**标签**: `#AI`, `#robotics`, `#video generation`, `#world models`, `#multimodal`

---

<a id="item-14"></a>
## [ChatGPT AgentForger 漏洞可通过钓鱼链接部署恶意智能体](https://thehackernews.com/2026/07/chatgpt-agentforger-flaw-could-deploy.html) ⭐️ 8.0/10

Zenity Labs 的安全研究人员披露了 OpenAI 的 ChatGPT Workspace Agents 中的一个严重漏洞，代号 AgentForger，该漏洞可允许单个钓鱼链接悄无声息地在受害者组织中创建、授权并部署恶意 AI 智能体。OpenAI 已于 2026 年 6 月 8 日修复了该漏洞。 该漏洞极为严重，因为攻击者仅需受害者初次点击，即可在企业环境中建立持久、自主的内部威胁。这凸显了具有广泛访问组织工具和数据的 AI 智能体所带来的新兴安全风险。 AgentForger 漏洞利用了 ChatGPT Workspace Agents 处理共享 URL 的方式，允许攻击者嵌入恶意指令，一旦智能体被部署便会自动执行。该攻击无需凭证，且由于智能体在受害者的已认证会话下运行，可绕过典型的安全控制。

rss · The Hacker News · 7月24日 11:53

**背景**: ChatGPT Workspace Agents 是 OpenAI 于 2026 年 4 月推出的 AI 智能体，可跨多种工具和服务自动化复杂工作流。它们在云端运行，旨在团队成员间共享。AgentForger 漏洞类似于跨站请求伪造（CSRF）攻击，但应用于 AI 智能体系统，通过精心构造的链接触发在受害者账户下创建恶意智能体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/chatgpt-agentforger-flaw-could-deploy.html">ChatGPT AgentForger Flaw Could Deploy Rogue Workspace Agents ...</a></li>
<li><a href="https://www.csoonline.com/article/4200978/agentforger-proves-ai-agents-can-become-persistent-insider-threats.html">AgentForger proves AI agents can become persistent insider ...</a></li>
<li><a href="https://openai.com/index/introducing-workspace-agents-in-chatgpt/">Introducing workspace agents in ChatGPT - OpenAI</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#ChatGPT`, `#AI agents`, `#phishing`

---

<a id="item-15"></a>
## [黑客使用 Hermes AI 代理对泰国财政部发动无人值守攻击](https://thehackernews.com/2026/07/hacker-runs-hermes-ai-agent-unattended.html) ⭐️ 8.0/10

一名威胁行为者部署了开源的 Hermes AI 代理，在无人值守的“YOLO”模式下自主对泰国财政部的网络进行后渗透活动。该代理扫描主机以获取 root 权限，搜索文件系统，并将其日志暴露在开放的目录中。 这是首次已知的真实世界中将 AI 代理用于无人值守自主后渗透的网络攻击，标志着 AI 赋能威胁的重大演变。它突显了针对 AI 驱动攻击的安全措施的紧迫需求，尤其是在关键政府基础设施中。 Hermes AI 代理由 Nous Research 开发，运行时禁用了批准提示（YOLO 模式），使其能够无需人工监督执行危险命令。攻击者的日志被留在开放的目录中，使研究人员能够分析此次入侵。

rss · The Hacker News · 7月24日 10:15

**背景**: 像 Hermes 这样的 AI 代理设计有安全功能，要求在执行危险命令前获得用户批准。然而，YOLO 模式绕过了这些保障，实质上赋予了代理完全自主权。Hermes 代理采用纵深防御安全模型，但禁用批准提示移除了一个关键保护层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hermes-agent.ai/">Hermes Agent — Open-Source AI Agent with Memory, Skills, and Cron</a></li>
<li><a href="https://www.howdoiuseai.com/blog/2026-07-24-why-your-coding-agent-s-yolo-mode-is-one-bad-promp">Why your coding agent's YOLO mode is one bad prompt away from ...</a></li>
<li><a href="https://thehackernews.com/2026/07/hacker-runs-hermes-ai-agent-unattended.html">Hacker Runs Hermes AI Agent Unattended for Post-Exploitation ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#AI agent`, `#autonomous attack`, `#post-exploitation`, `#Hermes AI`

---

<a id="item-16"></a>
## [NodeBB 修复八项 AI 发现的高危漏洞](https://thehackernews.com/2026/07/nodebb-patches-eight-ai-found-flaws.html) ⭐️ 8.0/10

NodeBB 发布了 4.14.2 版本，修复了由 AI 渗透测试代理在对源代码进行六小时审查时发现的八项高危安全漏洞，这些漏洞影响 4.14.0 之前的所有版本。 这些漏洞可能暴露广泛使用的论坛平台的管理员权限和私密聊天，而由 AI 代理发现它们展示了一种可能变得更常见的创新安全测试方法。 Aikido Security 将所有八项漏洞评为高危级别，其中最简单的利用仅需更改设置；管理员被敦促立即升级到 4.14.2 版本。

rss · The Hacker News · 7月24日 07:41

**背景**: NodeBB 是一个基于 Node.js 的开源论坛软件，通过 WebSocket 和 Redis 或 MongoDB 等数据库支持实时交互。AI 渗透测试代理是利用大语言模型的自主工具，用于模拟攻击和发现漏洞，例如 GitHub 上的 pentest-ai-agents 项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nodebb.org/">NodeBB Forum Software - The Modern Discussion Platform</a></li>
<li><a href="https://github.com/NodeBB/NodeBB">GitHub - NodeBB / NodeBB : Node.js based forum software built for...</a></li>
<li><a href="https://github.com/0xSteph/pentest-ai-agents">GitHub - 0xSteph/pentest-ai-agents: Turn Claude Code into ...</a></li>

</ul>
</details>

**标签**: `#security`, `#NodeBB`, `#AI pentesting`, `#vulnerability`, `#patching`

---

<a id="item-17"></a>
## [虚假 Notepad++ 插件传播 MATCHBOIL.V2 恶意软件](https://thehackernews.com/2026/07/fake-notepad-plugin-delivers.html) ⭐️ 8.0/10

乌克兰 CERT-UA 警告称，一场利用恶意 Notepad++ 插件传播 MATCHBOIL.V2 恶意软件加载器的活动，与亲俄威胁组织 UAC-0099 有关。 此次攻击针对 Windows 用户，可能危及乌克兰政府和国防机构，并凸显了通过受信任软件插件进行供应链攻击的持续风险。 该虚假插件以 DLL 形式交付，由合法的 Notepad++ 8.8.3 可执行文件进行侧加载，使用 BurnyBear 加载器部署 MATCHBOIL.V2，并通过每三分钟运行一次实现持久化。

rss · The Hacker News · 7月24日 06:50

**背景**: Notepad++ 是一款流行的 Windows 免费源代码编辑器，常通过插件扩展功能。UAC-0099 是一个至少自 2022 年起针对乌克兰实体的亲俄威胁组织，此前曾利用 WinRAR 漏洞和钓鱼诱饵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/fake-notepad-plugin-delivers.html">Fake Notepad++ Plugin Delivers MATCHBOIL.V2 in UAC-0099 Attacks</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-abuse-notepad-plus-plus-plugins-to-stealthily-install-malware/">Hackers abuse Notepad++ plugins to stealthily install malware</a></li>
<li><a href="https://cyberpress.org/hackers-weaponize-notepad-8-8-3/">Hackers Weaponize Notepad++ 8.8.3 to Silently Install MATCHBOIL.V2 Malware</a></li>

</ul>
</details>

**标签**: `#malware`, `#cybersecurity`, `#Notepad++`, `#Ukraine`, `#supply-chain attack`

---

<a id="item-18"></a>
## [BlueNoroff 利用 Zoom 钓鱼工具包分析加密钱包](https://thehackernews.com/2026/07/bluenoroff-zoom-phishing-kit-profiles.html) ⭐️ 7.0/10

BlueNoroff（一个朝鲜高级持续性威胁 APT 组织）被发现使用一个伪装成 Zoom 的钓鱼工具包，在通过社交工程活动投放恶意软件之前，先对加密货币钱包进行分析。 该技术使攻击者能够选择性地瞄准高价值加密货币持有者，提高其以财务为动机的攻击效率。这凸显了朝鲜网络行动在窃取数字资产方面不断演进的复杂性。 该钓鱼工具包使用了'ClickFix'社交工程技术，通过伪造的 CAPTCHA 页面诱骗用户运行恶意命令。攻击者使用拼写错误的 Zoom 域名和被入侵的行业联系人建立信任。

rss · The Hacker News · 7月24日 15:12

**背景**: BlueNoroff（也称为 APT38）是 Lazarus 组织的一个以财务为动机的子团体，被认为由朝鲜政府操控。ClickFix 技术通常呈现一个虚假的'验证'步骤（如 CAPTCHA），指示用户复制并运行恶意 PowerShell 命令，从而实现恶意软件投放。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BlueNorOff">BlueNorOff</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2025/08/21/think-before-you-clickfix-analyzing-the-clickfix-social-engineering-technique/">Think before you Click ( Fix ): Analyzing the ClickFix social engineering...</a></li>

</ul>
</details>

**标签**: `#cyber threat`, `#phishing`, `#North Korea`, `#crypto malware`, `#social engineering`

---

<a id="item-19"></a>
## [AI 代理最小权限执行仍面临挑战](https://thehackernews.com/2026/07/seeing-ai-agents-is-not-enough-security.html) ⭐️ 7.0/10

文章指出，对 AI 代理实施最小权限原则的难度超乎想象，目前正在探索从提示过滤到身份层访问控制等多种方法。 随着 AI 代理被广泛采用，控制其行为以防止误用和数据泄露至关重要，因此有效执行最小权限成为紧迫的安全问题。 提示过滤仅覆盖语言层面的风险，无法防止误用或过度访问，而身份层控制（如加密身份、即时访问）提供更强的执行能力，但需要针对代理的身份管理。

rss · The Hacker News · 7月24日 11:30

**背景**: AI 代理是代表用户执行任务的自主程序，通常拥有对系统和数据的访问权限。最小权限原则要求代理仅拥有完成任务所必需的权限，但传统的静态权限模型难以应对代理的动态和不可预测行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.token.security/blog/why-ai-agent-lifecycle-security-must-start-with-identity-not-prompt-filtering">Why AI Agent Lifecycle Security Must Start With Identity, Not Prompt ...</a></li>
<li><a href="https://repost.aws/articles/ARRfjH_lA4TZeKnM0OU0iYkg/secure-your-ai-agents-on-aws-part-1-inputs-identity-and-human-oversight">Secure Your AI Agents on AWS (Part 1): Inputs, Identity , and Human...</a></li>
<li><a href="https://www.linkedin.com/pulse/agent-control-plane-here-identity-layer-isnt-mark-a-johnston-grric">The Agent Control Plane Is Here. The Identity Layer Isn’t</a></li>

</ul>
</details>

**标签**: `#AI security`, `#least privilege`, `#agent security`, `#access control`, `#cybersecurity`

---

<a id="item-20"></a>
## [黄金鸡威胁组织携四个新恶意软件家族重现](https://thehackernews.com/2026/07/golden-chickens-resurfaces-with-four.html) ⭐️ 7.0/10

黄金鸡威胁行为者重新出现，推出了四个新恶意软件家族：TinyEgg、ChonkyChicken、ChonkyChicken 的模块化变体，以及名为 ChromEggscalator 的修改版凭据窃取工具。 此次重现表明，仅靠公开披露无法摧毁复杂的 MaaS 运营，对全球组织构成持续风险。 TinyEgg 是一个轻量级初始访问后门，仅限于信息收集；而 ChonkyChicken 是一个功能完整的远程访问木马，用于凭据窃取和横向移动。其模块化变体增强了灵活性。

rss · The Hacker News · 7月24日 10:09

**背景**: 黄金鸡是一个恶意软件即服务（MaaS）生态系统，为其他网络犯罪分子提供恶意工具。尽管此前已有公开披露，该组织仍继续开发并发布针对 Windows 系统的新恶意软件家族。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/golden-chickens-resurfaces-with-four.html">Golden Chickens Resurfaces With Four New Malware Families and Modular Implants</a></li>
<li><a href="https://news.shield53.com/golden-chickens-maas-evolves-four-new-malware-families-signal-dangerous-operational-resilience/">Golden Chickens MaaS Evolves: Four New Malware Families ...</a></li>
<li><a href="https://www.scworld.com/brief/golden-chickens-malware-as-a-service-resurfaces-with-four-new-families">Golden Chickens malware-as-a-service resurfaces with four new ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#Golden Chickens`, `#threat actors`, `#MaaS`

---