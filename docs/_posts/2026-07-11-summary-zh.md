---
layout: default
title: "Horizon Summary: 2026-07-11 (ZH)"
date: 2026-07-11
lang: zh
---

> 从 79 条内容中筛选出 20 条重要资讯。

---

1. [Gitea Docker 认证绕过漏洞被利用](#item-1)
2. [苹果起诉 OpenAI 窃取商业机密](#item-2)
3. [OpenAI 推出 GPT-5.6 Sol/Terra/Luna 及 Codex 超级应用](#item-3)
4. [激光攻击重置 Tangem 钱包密码，卡片无法修复](#item-4)
5. [XQUIC 中未修补的 XRING 漏洞可导致 HTTP/3 服务器崩溃](#item-5)
6. [Progress 因可信威胁敦促 ShareFile 管理员关闭服务器](#item-6)
7. [QuadRF 开源 SDR 可穿透墙壁可视化射频信号](#item-7)
8. [好工具应隐于无形](#item-8)
9. [成功公司为何创新困难](#item-9)
10. [AR 眼镜需要侵入式摄像头和云处理](#item-10)
11. [主机卸载缓解 JAX LLM 训练 HBM 瓶颈](#item-11)
12. [CUDA 内核融合：优化内存与启动开销](#item-12)
13. [NVIDIA 提出硬件友好的大语言模型设计原则](#item-13)
14. [Injective Labs GitHub 遭入侵导致恶意 npm 包发布](#item-14)
15. [MODBEACON RAT 利用 gRPC 流实现加密 C2 通信](#item-15)
16. [研究揭示免费安卓 VPN 应用泄露数据、追踪用户](#item-16)
17. [黑客利用虚假 Microsoft Entra 通行密钥注册劫持账户](#item-17)
18. [攻击者利用‘Ill Bloom’漏洞窃取 500 万美元加密钱包资金](#item-18)
19. [勒索软件谈判者因协助 BlackCat 被判 70 个月](#item-19)
20. [数百万 ChatGPT 对话被命令披露；OpenAI 被指控隐瞒](#item-20)

---

<a id="item-1"></a>
## [Gitea Docker 认证绕过漏洞被利用](https://www.bleepingcomputer.com/news/security/hackers-exploit-critical-auth-bypass-in-gitea-docker-image/) ⭐️ 10.0/10

攻击者正在积极利用官方 Gitea Docker 镜像中的一个严重认证绕过漏洞，该漏洞允许他们冒充任何用户，包括管理员。 该漏洞对数千个自托管的 Gitea 实例构成直接安全风险，可能导致未授权访问、数据泄露以及开发基础设施的完全沦陷。 该漏洞特别影响官方 Docker 镜像，允许远程攻击者绕过认证机制，无需有效凭据即可冒充任何已注册用户的身份。

rss · BleepingComputer · 7月10日 15:48

**背景**: Gitea 是一种流行的自托管 Git 服务，类似于 GitHub 或 GitLab，常被组织用于管理源代码和协作。认证绕过是一种漏洞，使攻击者通过欺骗系统跳过或绕过登录检查来获得未授权访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gitea">Gitea</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/identity-security/authentication-bypass/">What Is Authentication Bypass? Techniques & Examples</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#docker`, `#gitea`, `#exploitation`

---

<a id="item-2"></a>
## [苹果起诉 OpenAI 窃取商业机密](https://9to5mac.com/2026/07/10/apple-sues-openai-trade-secret-theft/) ⭐️ 9.0/10

苹果已对 OpenAI 提起诉讼，指控其前员工窃取苹果的机密硬件信息，并利用这些信息接触苹果的供应商。 这起诉讼可能对 AI 行业产生重大影响，包括对 AI 公司的信任以及商业机密保护的法律先例。 诉讼称，OpenAI 指导新员工如何在离开苹果时避免审查，并且发现了员工在离职时通过电子邮件发送机密信息的模式。

hackernews · stock_toaster · 7月10日 20:47 · [社区讨论](https://news.ycombinator.com/item?id=48865019)

**背景**: 商业机密盗窃是一个严重的法律问题。苹果历来积极保护其知识产权。OpenAI 是一家领先的 AI 研究机构。此案凸显了科技巨头之间在人才和机密信息方面的紧张关系。

**社区讨论**: 评论者大多批评 OpenAI，认为证据确凿，OpenAI 将面临严重后果。有人指出，这对一家处理大量用户知识产权的公司来说形象极差。

**标签**: `#Apple`, `#OpenAI`, `#trade secrets`, `#lawsuit`, `#AI ethics`

---

<a id="item-3"></a>
## [OpenAI 推出 GPT-5.6 Sol/Terra/Luna 及 Codex 超级应用](https://www.latent.space/p/ainews-openai-launches-gpt-56-solterraluna) ⭐️ 9.0/10

OpenAI 宣布对 GPT-5.6 模型系列进行有限预览，该系列包含三个分级版本，代号分别为 Sol、Terra 和 Luna，并将 Codex 转变为集聊天与编程能力于一体的 ChatGPT 超级应用。 此次发布将 OpenAI 混乱的模型阵容（如 o3、o4-mini、GPT-4 Turbo 等）简化为清晰的分级结构，方便开发者选择合适的模型。将 Codex 整合进 ChatGPT 作为超级应用，可能将编程辅助功能集中到流行的聊天机器人中，从而重塑开发者工作流程。 GPT-5.6 系列包括 gpt-5.6-sol、gpt-5.6-terra 和 gpt-5.6-luna，每种模型具有不同的推理模式与定价层级。Codex 模型最初是 GPT-3 针对代码微调的衍生版本，现已成为 ChatGPT 超级应用的核心引擎，支持高级编程、计算机操作和研究工作流。

rss · Latent Space · 7月10日 06:19

**背景**: OpenAI GPT-5.6 Sol、Terra 和 Luna 是 OpenAI 最新模型系列，采用政府限制访问机制，并提供三个等级的推理能力。Codex 是一种大型语言模型，于 2021 年发布，基于 GPT-3 微调而成，能够将自然语言转化为源代码，最初为 GitHub Copilot 提供支持。此举将 OpenAI 的编程与通用人工智能统一整合到 ChatGPT 这一单一体验中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.swisherpost.com/technology/openai-gpt-5-6-sol-terra-luna-preview/">OpenAI previews GPT - 5 . 6 Sol , Terra and Luna models | Swisher Post</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2026/07/gpt-5-6-sol-terra-luna/">GPT - 5 . 6 Is Here: Sol , Terra , and Luna Pricing & Benchmarks</a></li>
<li><a href="https://blog.getbind.co/gpt-5-6-is-government-gated-what-sol-terra-and-luna-mean-for-developers/">GPT - 5 . 6 Sol , Terra , Luna : Government-Gated Access Explained</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(language_model)">OpenAI Codex (language model) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT`, `#LLM`, `#AI News`

---

<a id="item-4"></a>
## [激光攻击重置 Tangem 钱包密码，卡片无法修复](https://thehackernews.com/2026/07/laser-attack-resets-tangem-wallet.html) ⭐️ 9.0/10

Ledger Donjon 安全团队的研究人员展示，通过精准定时激光脉冲，无需旧密码或备份卡即可重置 Tangem 加密钱包卡的密码，攻击者可完全控制钱包。 该漏洞动摇了硬件钱包的核心安全承诺——即使设备被物理接触，资金仍安全——并凸显了在安全芯片中修补此类缺陷的困难。 该攻击需要物理接触卡上的芯片和精密设备，因此在大多数实际盗窃中不可行。Tangem 卡使用无法通过固件更新的安全芯片，因此除非更换卡片，否则漏洞永久存在。

rss · The Hacker News · 7月10日 14:51

**背景**: Tangem 卡等硬件钱包在安全芯片中离线存储加密货币私钥，以防止远程攻击。激光故障注入（LFI）是一种物理攻击技术，利用短时精准激光脉冲干扰芯片正常运行，可能绕过安全检查。这并非针对安全芯片的首次 LFI 攻击，但因针对不可修补的消费级加密钱包而备受关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tangem.com/en/blog/post/laser-fault-injection-attack/">Laser Fault Injection (LFI) Attacks Against Secure Elements | Tangem Blog</a></li>
<li><a href="https://www.appluslaboratories.com/global/en/news/publications/new-fault-injection-attacks">Lateral Laser Fault Injection: A new variant to one of the most effective hardware attack on secure chips, developed by Applus+ Laboratories</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#hardware wallet`, `#laser attack`, `#cryptocurrency`

---

<a id="item-5"></a>
## [XQUIC 中未修补的 XRING 漏洞可导致 HTTP/3 服务器崩溃](https://thehackernews.com/2026/07/unpatched-xring-flaw-in-xquic-lets.html) ⭐️ 9.0/10

2026 年 7 月 8 日，FoxIO 研究员 Sébastien Féry 披露了阿里巴巴 XQUIC 库中的 XRING 漏洞，允许任何远程客户端通过约 260 字节的普通 QPACK 流量使 HTTP/3 服务器崩溃。目前尚无补丁。 这个广泛使用的 QUIC 库中的关键未修补拒绝服务漏洞可能被轻易利用来破坏 HTTP/3 服务，影响许多依赖 XQUIC 的服务器。攻击无需身份验证或畸形数据包，执行起来非常简单。 该漏洞是 XQUIC 库 QPACK 处理中某一行代码的单变量错误。攻击使用完全符合 RFC 9204 定义的 QPACK 流量，使得检测变得困难。

rss · The Hacker News · 7月10日 11:47

**背景**: QUIC 是一种旨在提高 TCP 性能的传输协议，HTTP/3 是运行在 QUIC 上的 HTTP 版本。QPACK 是 HTTP/3 的头压缩格式，类似于 HTTP/2 的 HPACK。XQUIC 是阿里巴巴开源的 QUIC 和 HTTP/3 实现，用于多种生产环境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/unpatched-xring-flaw-in-xquic-lets.html">Unpatched XRING Flaw in XQUIC Lets Remote Clients Crash HTTP/3 Servers</a></li>
<li><a href="https://github.com/alibaba/xquic">GitHub - alibaba/xquic: XQUIC Library released by Alibaba is ...</a></li>
<li><a href="https://datatracker.ietf.org/doc/html/rfc9204">RFC 9204 - QPACK : Field Compression for HTTP / 3 | IETF Datatracker</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#QUIC`, `#HTTP/3`, `#DoS`

---

<a id="item-6"></a>
## [Progress 因可信威胁敦促 ShareFile 管理员关闭服务器](https://www.bleepingcomputer.com/news/security/progress-urges-sharefile-customers-to-shut-down-servers-over-credible-threat/) ⭐️ 9.0/10

Progress Software 已通过电子邮件通知使用 Storage Zone Controller 的 ShareFile 客户，由于存在可信的外部安全威胁，需立即关闭其本地服务器。该公司已出于谨慎暂时禁用受影响账户的访问权限。 这一紧急通告表明一款广泛使用的企业文件共享解决方案存在严重且已被积极利用的漏洞，可能泄露敏感数据。需要立即采取行动以防止潜在入侵，影响众多依赖 ShareFile 进行安全数据交换的组织。 该威胁专门针对本地 ShareFile 部署中的 Storage Zone Controller (SZC) 组件，Progress 已确认正在与内部及外部安全团队合作。此前，ShareFile 的 SZC 曾被发现存在允许预认证远程代码执行的漏洞。

rss · BleepingComputer · 7月10日 16:26

**背景**: Progress Software 的 ShareFile 是一款企业级安全文件共享平台。Storage Zone Controller (SZC) 是本地组件，用于在本地存储文件并与 ShareFile 云集成。SZC 过去的漏洞曾允许攻击者在无需凭证的情况下绕过认证。当前威胁被描述为“可信的”，但具体细节尚未披露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.sharefile.com/en-us/storage-zones-controller/5-0.html">Storage zones controller 5.x</a></li>
<li><a href="https://www.cloaked.com/post/are-your-sharefile-vulnerabilities-leaving-you-open-to-pre-auth-rce-and-data-theft">Cloaked - Are Your ShareFile Vulnerabilities Leaving You Open to...</a></li>

</ul>
</details>

**标签**: `#security`, `#Progress Software`, `#ShareFile`, `#vulnerability`, `#threat`

---

<a id="item-7"></a>
## [QuadRF 开源 SDR 可穿透墙壁可视化射频信号](https://www.jeffgeerling.com/blog/2026/quadrf-can-spot-drones-and-see-wifi-through-my-wall/) ⭐️ 8.0/10

QuadRF 是一款开源、相位相干的四通道软件定义无线电（SDR），利用射频传感技术来检测无人机并可视化穿透墙壁的 WiFi 信号，最近在博客文章中进行了演示。 该工具使先进的射频传感技术对爱好者和黑客变得可及，在无人机检测、隐私审计和增强现实方面具有潜在应用，同时也引发了重要的隐私影响。 QuadRF 采用混合开放模式，开源了用户可修改的组件，同时保护了射频核心实现。它支持 4x4 MIMO 操作，专为无线电定向设计。

hackernews · speckx · 7月10日 15:59 · [社区讨论](https://news.ycombinator.com/item?id=48861717)

**背景**: 软件定义无线电（SDR）是一种无线电通信系统，其中通常由硬件实现的组件改由软件实现。射频传感利用无线电信号及其反射来检测和跟踪物体，通常结合人工智能算法。QuadRF 是一个特定的 SDR 平台，其四个通道保持相位相干，从而支持定向和空间感知。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/open-space-sdr/main">GitHub - open -space-sdr/main · GitHub</a></li>
<li><a href="https://www.crowdsupply.com/scale-rf/quadrf">QuadRF | Crowd Supply</a></li>
<li><a href="https://feedbagel.com/post/seeing-the-world-in-radio-waves-with-the-quadrf">QuadRF : An Open - Source Four-Channel SDR for Radio... | FeedBagel</a></li>

</ul>
</details>

**社区讨论**: 创建者 mrtnmcc 回答了问题，并指出根据反馈进行了改进。评论者将其与热成像相机比较，讨论了声音定位的应用，并推测了政府能力。有些人表示有兴趣将类似工具集成到智能眼镜中。

**标签**: `#RF sensing`, `#open-source hardware`, `#drone detection`, `#privacy`, `#visualization`

---

<a id="item-8"></a>
## [好工具应隐于无形](https://www.gingerbill.org/article/2026/07/10/good-tools-are-invisible/) ⭐️ 8.0/10

一篇新文章提出，最好的工具应尽可能减少摩擦，直到用户几乎察觉不到其存在，而必要的复杂性则可通过熟悉而融入背景。 这一原则对用户体验设计和软件工程至关重要，它指导开发者创建减少认知负荷、提高生产力的工具。 文章强调，设计师添加的随意性摩擦（如不必要的功能）会损害易用性，但即使是类似解决合并冲突这样的干扰性任务，经过反复接触后也会变得自然。

hackernews · theanonymousone · 7月10日 10:32 · [社区讨论](https://news.ycombinator.com/item?id=48858121)

**背景**: “工具隐于无形”这一概念源于以下观点：有效的工具不会被用户注意到；它们成为用户意图的延伸。在软件中，这意味着界面应当直观且不引人注目，让用户专注于目标而非工具本身。

**社区讨论**: 评论者普遍赞同这一原则，但增加了更多细节。一位开发者指出，即使是内部工具，暴露内部结构也会妨碍同事的工作。另一位则区分了必要的摩擦（如合并冲突）和随意的复杂性。还有人讨论了终端与图形界面的优劣，认为 90 年代标准化的界面更直观。

**标签**: `#UX`, `#tool design`, `#software engineering`, `#developer experience`

---

<a id="item-9"></a>
## [成功公司为何创新困难](https://ianreppel.org/how-successful-companies-go-blind/) ⭐️ 8.0/10

一篇文章指出，成功公司常因根深蒂固的官僚主义、风险规避及缺乏变革激励而对创新视而不见。 这一见解对于理解大型成熟组织为何难以适应并失去竞争优势至关重要，影响着需要应对创新挑战的员工、领导者和投资者。 文章论点得到了社区高参与度的支持——185 个点赞和 63 条评论，其中许多评论提供了来自国防和科技行业的一手经验，强调发展势头和内部政治是主要障碍。

hackernews · speckx · 7月10日 13:31 · [社区讨论](https://news.ycombinator.com/item?id=48859678)

**背景**: 成功公司往往建立了最初推动效率但后来扼杀创新的流程和层级。官僚主义造成了守门人、部门壁垒和规避风险的文化，阻碍了实验和适应。这一现象在商业文献中广为人知，但该文章通过评论者的真实案例提供了当代讨论。

**社区讨论**: 评论者基本同意文章观点，分享了个人经历。一位指出发展势头而非盲目是因素之一，另一位区分了能力与背景问题，认为官僚体制中的人才无法展现才华。第三位评论强调，VC 资助的 MVP 式公司因过于关注业务问题而非工程，随时间推移导致质量下降。

**标签**: `#company-culture`, `#innovation`, `#bureaucracy`, `#technology-management`, `#hacker-news-discussion`

---

<a id="item-10"></a>
## [AR 眼镜需要侵入式摄像头和云处理](https://simonwillison.net/2026/Jul/10/nilay-patel/#atom-everything) ⭐️ 8.0/10

The Verge 主编 Nilay Patel 在 The Vergecast 节目中提出，增强现实眼镜本质上需要持续录像的摄像头和云端处理，这使得重大的隐私入侵不可避免。 Patel 的分析挑战了围绕 AR 作为下一代计算平台的普遍乐观叙事，揭示了技术可行性与社会隐私规范之间的根本矛盾，这可能会影响行业方向和公共政策。 Patel 指出，目前没有芯片能小到塞进眼镜腿中，同时提供足够的处理能力和能效来实现实时 AR，因此数据必须发送到云端；唯一的替代方案是像 Apple Vision Pro 那样笨重、需外接电池包的设备。

rss · Simon Willison · 7月10日 17:05

**背景**: 增强现实（AR）眼镜将数字信息叠加到现实世界中，需要持续分析用户的环境。设备端处理能更好地保护隐私，但要求有强大且节能的芯片，目前尚无法装入眼镜的小型化设计中。云端处理则将计算任务卸载，但需要将视频数据通过互联网传输，引发隐私和延迟问题。当前的 AR 设备如 Apple Vision Pro 采用设备端与云端混合处理，但存在成本高、重量大和电池续航有限等缺点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aismartglasses.wordpress.com/2026/07/05/on-device-ai-vs-cloud-ai-whats-the-difference/">On-Device AI vs Cloud AI: What’s the Difference?</a></li>
<li><a href="https://milvus.io/ai-quick-reference/what-are-the-design-challenges-specific-to-wearable-ar-devices">What are the design challenges specific to wearable AR devices ?</a></li>

</ul>
</details>

**标签**: `#augmented reality`, `#privacy`, `#cloud computing`, `#technology ethics`

---

<a id="item-11"></a>
## [主机卸载缓解 JAX LLM 训练 HBM 瓶颈](https://developer.nvidia.com/blog/reducing-high-bandwidth-memory-bottlenecks-in-jax-based-llm-training-with-host-offloading/) ⭐️ 8.0/10

NVIDIA 发布了一篇博客文章，详细介绍了通过主机卸载技术来缓解基于 JAX 的大语言模型训练中的高带宽内存（HBM）瓶颈。 该技术通过将选定的数据卸载到主机内存，使得在现有 GPU 上训练更大的模型成为可能，有望减少对昂贵内存升级的需求并提高训练效率。 该主机卸载技术在 NVIDIA Grace Blackwell 系统上尤为有效，该系统利用 NVLink-C2C 在 Grace CPU 和 Blackwell GPU 之间提供 900 GB/s 的双向带宽。

rss · NVIDIA Developer Blog · 7月10日 18:17

**背景**: 大语言模型训练通常受限于 GPU 内存容量，因为模型权重、梯度和优化器状态会消耗大量高带宽内存（HBM）。JAX 是一个面向加速器的数组计算和程序变换的 Python 库，常用于高性能机器学习研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/reducing-high-bandwidth-memory-bottlenecks-in-jax-based-llm-training-with-host-offloading/">Reducing High-Bandwidth Memory Bottlenecks in JAX-Based LLM...</a></li>
<li><a href="https://en.wikipedia.org/wiki/JAX_(software)">JAX (software) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#JAX`, `#LLM training`, `#memory optimization`, `#HBM`, `#host offloading`

---

<a id="item-12"></a>
## [CUDA 内核融合：优化内存与启动开销](https://developer.nvidia.com/blog/kernel-fusion-in-nvidia-cuda-optimizing-memory-traffic-and-launch-overhead/) ⭐️ 8.0/10

NVIDIA 发布了一篇博客文章，详细介绍了如何通过内核融合将多个 GPU 内核合并为一个，以减少内存流量和内核启动开销。 此技术对 GPU 程序员至关重要，可最大化内存受限应用（如深度学习和高性能计算）的性能，减少全局内存访问并提高利用率。 内核融合通过将中间数据保留在片上存储器（共享内存或寄存器）中，而不是在内核之间写入和读取全局内存，同时消除了每个内核的启动开销。

rss · NVIDIA Developer Blog · 7月10日 16:41

**背景**: 在 GPU 计算中，内核是在 GPU 上执行的函数。启动多个内核会产生开销并强制通过全局内存传输数据。内核融合将多个计算合并到一个内核中，提高内存带宽效率并减少启动延迟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vrushankdes.ai/diffusion-policy-inference-optimization/part-vi---kernel-fusion-in-cuda">Part VI - Kernel Fusion in CUDA</a></li>
<li><a href="https://stackoverflow.com/questions/53305830/cuda-how-does-kernel-fusion-improve-performance-on-memory-bound-applications-on">CUDA How Does Kernel Fusion Improve... - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#CUDA`, `#GPU optimization`, `#kernel fusion`, `#memory bandwidth`

---

<a id="item-13"></a>
## [NVIDIA 提出硬件友好的大语言模型设计原则](https://developer.nvidia.com/blog/ai-model-co-design-hardware-friendly-llm-design/) ⭐️ 8.0/10

NVIDIA 发布了一篇技术博客，详细介绍了硬件友好的大语言模型设计，强调通过硬件-软件协同设计来共同优化准确率、吞吐量和交互性。博客提供了具体指南，例如将模型维度与 GPU tile 大小对齐，并倾向于宽度大于深度的宽高比。 随着大语言模型规模的增长，在 GPU 上实现高效推理对于部署至关重要。NVIDIA 的指南帮助模型开发者和系统设计者在不牺牲准确率的前提下降低延迟并提高吞吐量，从而可能降低部署成本。 关键建议包括使用近似方形的线性层维度、对齐到 128 的倍数（理想为 256 或 512），以及设计宽度大于深度的宽高比模型以最大化计算强度。这些原则源于 NVIDIA GPU 架构的特性。

rss · NVIDIA Developer Blog · 7月10日 16:36

**背景**: 硬件-软件协同设计是一种将模型架构与硬件共同优化以提高性能的方法。对于在 GPU 上运行的大语言模型，内存带宽、计算单元利用率以及 tile 大小兼容性等因素会显著影响吞吐量和延迟。NVIDIA 的博客为基于 Transformer 的模型提供了可操作的设计模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://forums.developer.nvidia.com/t/ai-model-co-design-hardware-friendly-llm-design/376491">AI Model Co-Design: Hardware-Friendly LLM Design - Technical Blog - NVIDIA Developer Forums</a></li>

</ul>
</details>

**标签**: `#LLM`, `#hardware design`, `#AI optimization`, `#co-design`, `#NVIDIA`

---

<a id="item-14"></a>
## [Injective Labs GitHub 遭入侵导致恶意 npm 包发布](https://thehackernews.com/2026/07/injective-labs-github-compromise-pushes.html) ⭐️ 8.0/10

未知攻击者入侵了 Injective Labs 的 GitHub 仓库，并发布了恶意 npm 包@injectivelabs/sdk-ts@1.20.21，该包旨在窃取加密货币钱包私钥和助记词种子短语。 此次供应链攻击直接威胁到 Injective SDK 的用户，可能让攻击者清空加密货币钱包。它凸显了开源仓库和包注册表被入侵的持续风险。 该恶意包包含了虚假遥测功能，用于泄露钱包数据。安装了 1.20.21 版本的用户应立即更换钱包密钥并迁移到安全版本。

rss · The Hacker News · 7月10日 16:29

**背景**: 助记词种子短语是一串 12 到 24 个单词的序列，作为加密货币钱包的主备份，允许完全访问资金。针对 npm 等包注册表的供应链攻击通过入侵上游依赖项向下游用户分发恶意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.coinbase.com/learn/wallet/what-is-a-seed-phrase">What is a seed phrase? - Coinbase</a></li>
<li><a href="https://www.trellix.com/blogs/research/npm-account-hijacking-and-the-rise-of-supply-chain-attacks/">npm Account Hijacking and the Rise of Supply Chain Attacks</a></li>

</ul>
</details>

**标签**: `#security`, `#supply chain attack`, `#npm`, `#cryptocurrency`, `#GitHub`

---

<a id="item-15"></a>
## [MODBEACON RAT 利用 gRPC 流实现加密 C2 通信](https://thehackernews.com/2026/07/new-modbeacon-rat-uses-grpc-streaming.html) ⭐️ 8.0/10

与中国有关的 Silver Fox 组织部署了一种名为 MODBEACON 的新型基于 Rust 的远程访问木马，该木马利用 gRPC 流实现加密的命令与控制（C2）通信以逃避检测。 这标志着恶意软件逃避技术的重要演进，因为 gRPC 流在 C2 通信中很少使用，使得传统检测方法效果降低。网络安全专业人员必须更新防御手段以识别加密的 gRPC 流量。 该恶意软件通过使用 SEO 投毒技术的虚假软件安装程序进行分发，针对科技、教育和国有企业。它由中国网络安全公司奇安信发现。

rss · The Hacker News · 7月10日 13:15

**背景**: gRPC 是一种高性能远程过程调用（RPC）框架，支持流式传输，允许在单个连接上传输多条消息。Silver Fox 是一个与中国有关的网络犯罪组织，以低复杂度但高频率的操作闻名，常利用社会工程学和 SEO 投毒来传播恶意软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/new-modbeacon-rat-uses-grpc-streaming.html">New MODBEACON RAT Uses gRPC Streaming for Encrypted C2 Traffic</a></li>
<li><a href="https://cybersixt.com/a/7sZ8jeM9HjHYikA-MTmDwM">New MODBEACON RAT exploits gRPC stealth for encrypted attacks</a></li>
<li><a href="https://cyberwebspider.com/the-hacker-news/modbeacon-rat-encrypted-c2-traffic/">MODBEACON RAT Uses Encrypted C2 | Security News</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#RAT`, `#gRPC`, `#C2`

---

<a id="item-16"></a>
## [研究揭示免费安卓 VPN 应用泄露数据、追踪用户](https://thehackernews.com/2026/07/study-of-281-free-android-vpn-apps.html) ⭐️ 8.0/10

一项对谷歌商店 281 款免费安卓 VPN 应用的研究发现，许多应用未能保护流量安全，导致 DNS 泄露、IPv6 泄露、未加密数据传输以及用户追踪，影响超过 24 亿次安装。 这凸显了流行免费 VPN 中普遍存在的隐私漏洞，削弱了其保护作用，使数十亿用户面临监视和数据窃取的风险。 该研究使用新的测试系统评估这些应用，发现 29 款应用允许用户流量泄露到 VPN 隧道之外。这些问题很基础而非复杂，暴露出根本性的安全缺陷。

rss · The Hacker News · 7月10日 10:56

**背景**: VPN 通过加密流量和隐藏 IP 地址来保护隐私。DNS 泄露发生在 DNS 查询绕过 VPN 隧道直接发送给 ISP 服务器时，从而泄露访问的网站。IPv6 泄露则发生在 VPN 未能正确处理 IPv6 流量时，暴露用户的真实 IP。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DNS_leak">DNS leak</a></li>
<li><a href="https://en.wikipedia.org/wiki/IPv6_header">IPv6 header</a></li>
<li><a href="https://haddadi.github.io/papers/PETS2015VPN.pdf">A Glance through the VPN Looking Glass: IPv 6 Leakage and DNS...</a></li>

</ul>
</details>

**标签**: `#security`, `#VPN`, `#privacy`, `#Android`, `#research`

---

<a id="item-17"></a>
## [黑客利用虚假 Microsoft Entra 通行密钥注册劫持账户](https://thehackernews.com/2026/07/hackers-use-fake-microsoft-entra.html) ⭐️ 8.0/10

一个被追踪为 O-UNC-066 的威胁行为者通过语音钓鱼电话，诱骗 Microsoft 365 用户注册由攻击者控制的 Entra 通行密钥，从而实现账户接管和数据勒索。 这种攻击绕过了传统的基于密码的防御，利用了合法的身份验证机制，对企业安全构成重大威胁。这突显了组织需要教育用户防范针对通行密钥注册的钓鱼攻击。 该钓鱼工具包由控制面板控制，能够实时针对通行密钥注册过程。攻击行为归因于 O-UNC-066，已在多个行业中被观察到。

rss · The Hacker News · 7月10日 10:30

**背景**: Microsoft Entra ID 支持通行密钥（FIDO2）认证作为一种无密码登录方式。通行密钥注册通常是安全的过程，但攻击者通过诱骗用户注册攻击者控制的通行密钥来滥用它，从而提供能绕过密码重置的持久访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/hackers-use-fake-microsoft-entra.html">Hackers Use Fake Microsoft Entra Passkey Enrollment to Gain ...</a></li>
<li><a href="https://cybersecuritynews.com/hackers-abuse-microsoft-entra-passkey-enrollment/">Hackers Abuse Microsoft Entra Passkey Enrollment to Hijack ...</a></li>
<li><a href="https://learn.microsoft.com/en-us/entra/identity/authentication/how-to-register-passkey">Register a Passkey (FIDO2) - Microsoft Entra ID | Microsoft Learn</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#phishing`, `#Microsoft Entra`, `#Microsoft 365`, `#authentication`

---

<a id="item-18"></a>
## [攻击者利用‘Ill Bloom’漏洞窃取 500 万美元加密钱包资金](https://thehackernews.com/2026/07/attackers-exploit-ill-bloom.html) ⭐️ 8.0/10

安全公司 Coinspect 披露了加密钱包恢复短语生成中的‘Ill Bloom’漏洞。攻击者于 2026 年 5 月 27 日利用该漏洞，从多个钱包中盗取了超过 500 万美元。 该漏洞展示了钱包软件中的关键缺陷，可能导致直接的经济损失。它影响多个区块链的用户，并凸显了加密钱包中安全熵生成的必要性。 该漏洞源于生成 BIP39 恢复短语时的弱随机性。攻击者于 5 月 27 日进行了协调扫描，针对具有可预测种子的钱包，导致超过 500 万美元的损失。

rss · The Hacker News · 7月10日 09:00

**背景**: 加密货币钱包使用 12-24 个词的恢复短语（种子短语）来派生私钥。该短语通常通过随机熵源生成。如果熵较弱，攻击者可以通过暴力破解或预测短语来控制用户资金。BIP39 标准定义了短语的生成方式，但随机性实现缺陷可能引入漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/attackers-exploit-ill-bloom.html">Attackers Exploit 'Ill Bloom' Vulnerability to Drain Over $5 Million From Cryptocurrency Wallets</a></li>
<li><a href="https://beincrypto.com/ill-bloom-vulnerability-crypto-wallets/">Ill Bloom Vulnerability Drains $3.1 Million From Crypto Wallets: Are You Exposed?</a></li>
<li><a href="https://illbloom.org/">Ill Bloom: Crypto Wallet Vulnerability</a></li>

</ul>
</details>

**标签**: `#cryptocurrency`, `#security`, `#vulnerability`, `#wallet`, `#exploit`

---

<a id="item-19"></a>
## [勒索软件谈判者因协助 BlackCat 被判 70 个月](https://thehackernews.com/2026/07/ransomware-negotiator-gets-70-months-in.html) ⭐️ 8.0/10

一名 41 岁的前勒索软件谈判者因在 2023 年与 BlackCat 勒索软件集团合谋勒索多名受害者而被判处 70 个月监禁。 此案为起诉勒索软件攻击的协助者树立了法律先例，表明协助犯罪分子的网络安全专业人员将面临严重后果。 被告曾是网络安全事件响应公司 DigitalMint 的前员工，并与另外两人合作攻击更多受害者。量刑备忘录详细说明了他勒索美国公司的角色。

rss · The Hacker News · 7月10日 08:10

**背景**: BlackCat（也称 ALPHV）是一种用 Rust 编写的勒索软件即服务（RaaS），于 2021 年首次出现，全球受害者超过 1000 个。勒索软件谈判者通常由受害者聘请与攻击者沟通，但在此案中，谈判者站在了犯罪分子一边。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BlackCat_(cyber_gang)">BlackCat (cyber gang) - Wikipedia</a></li>
<li><a href="https://digitalmint.io/">DigitalMint Cyber Threat Intel & Incident Response | Home</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#ransomware`, `#blackcat`, `#law enforcement`

---

<a id="item-20"></a>
## [数百万 ChatGPT 对话被命令披露；OpenAI 被指控隐瞒](https://www.reddit.com/r/artificial/comments/1usbdyd/updated_millions_of_chatgpt_user_conversations/) ⭐️ 8.0/10

联邦法院命令 OpenAI 提供 2000 万条去标识化的 ChatGPT 对话日志，供原告在版权侵权案件中进行搜索。生产后，原告指控 OpenAI 未能保留许多对话，并进行了 190 亿次编辑，已请求制裁。 此案为 AI 聊天机器人对话中的用户隐私预期设定了重要先例，可能影响 AI 公司在诉讼中处理用户数据的方式。隐瞒和过度编辑的指控引发了对遵守发现命令的严重质疑。 该命令最初涉及 1.2 亿条日志，后减少至 2000 万条。原告声称 OpenAI 低估了使用检索增强生成（RAG）的对话，并对每条日志进行了 1000 次编辑，总计 190 亿次编辑。法院正在考虑制裁，包括禁止 OpenAI 在辩护中使用这些日志，并就删除的对话向陪审团作出指示。

reddit · r/artificial · /u/Apprehensive_Sky1950 · 7月10日 02:54

**背景**: 去标识化是一种去除个人身份信息以保护隐私的过程。在此背景下，“输出日志”指的是用户与 ChatGPT 的对话记录。此案是对 OpenAI 提起的更大规模版权侵权诉讼的一部分，原告指控其版权作品未经许可被使用。法院的发现程序要求双方在审判前交换相关信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/De-identification">De - identification - Wikipedia</a></li>
<li><a href="https://genai.byu.edu/data-de-identification">Data De - Identification</a></li>

</ul>
</details>

**社区讨论**: Reddit 用户对隐私问题以及 OpenAI 去标识化过程缺乏透明度表示了强烈担忧。一些人质疑，在法院命令下，任何聊天机器人的对话是否还能被视为私密。其他人则辩论去标识化的充分性以及对话数据可能被滥用的风险。

**标签**: `#ChatGPT`, `#Privacy`, `#Legal`, `#OpenAI`, `#Data Disclosure`

---