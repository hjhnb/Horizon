---
layout: default
title: "Horizon Summary: 2026-07-07 (ZH)"
date: 2026-07-07
lang: zh
---

> 从 59 条内容中筛选出 20 条重要资讯。

---

1. [16 年历史的 KVM 漏洞允许客户虚拟机逃逸至主机](#item-1)
2. [法国将从 2027 年起停止认证非量子安全加密](#item-2)
3. [OpenWrt One：开源路由器硬件平台](#item-3)
4. [Anthropic 提出大语言模型全局工作空间机制](#item-4)
5. [Kani：面向 Rust 的比特精确模型检验工具](#item-5)
6. [Elm 在通往 1.0 版本的路上宣布更快的构建](#item-6)
7. [NVIDIA 通过非均匀张量并行提升大模型训练有效吞吐量](#item-7)
8. [Amazon Nova 引入 rDPO 实现选择性模型遗忘](#item-8)
9. [威胁分子利用 Gitea Docker 漏洞 CVE-2026-20896](#item-9)
10. [TrojPix 攻击利用视频线缆辐射泄漏气隙系统数据](#item-10)
11. [Opera GX 漏洞允许静默安装 Mod 窃取数据](#item-11)
12. [SkillCloak：自解压打包技术逃逸 AI 技能扫描器](#item-12)
13. [通过虚假微软 Teams IT 支持电话传播 EtherRAT 恶意软件](#item-13)
14. [Adobe ColdFusion 严重漏洞遭攻击利用](#item-14)
15. [基准测试对比的是开放模型与闭源产品，而非模型本身](#item-15)
16. [蚂蚁集团 Robbyant 在 Apache-2.0 下开源 LingBot-Vision 骨干网络](#item-16)
17. [法院合并诉讼指控 ChatGPT 鼓励自杀和吸毒](#item-17)
18. [伊朗关联黑客部署新型 Cavern C2 框架](#item-18)
19. [本周网络安全回顾：日常组件中的信任被利用](#item-19)
20. [疑似中国关联黑客利用虚假税务工具部署 DcRAT](#item-20)

---

<a id="item-1"></a>
## [16 年历史的 KVM 漏洞允许客户虚拟机逃逸至主机](https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html) ⭐️ 10.0/10

Linux KVM 的 shadow MMU 代码中存在一个存在 16 年的释放后使用漏洞（CVE-2026-53359）。一个概念验证利用程序可导致主机内核恐慌，研究人员声称另一个未公开的利用程序可实现英特尔和 AMD x86 系统上的完整虚拟机逃逸。 该漏洞允许客户虚拟机破坏主机内核内存，并可能逃逸至主机，破坏了虚拟化的基本隔离。由于 KVM 在云和企业环境中广泛使用，这构成了严重的安全风险，需要立即修补。 该漏洞位于英特尔和 AMD x86 平台共享的 shadow MMU 代码中。公开的概念验证仅导致主机内核恐慌，但研究人员表示更精细的利用程序可在主机上实现任意代码执行。

rss · The Hacker News · 7月6日 17:37

**背景**: 释放后使用（UAF）是一种内存损坏漏洞，程序在释放内存后仍继续使用该内存，可能允许攻击者执行任意代码。KVM shadow MMU 是虚拟机管理程序中的一个组件，通过维护影子页表来高效管理客户虚拟内存；该代码中的漏洞可能导致虚拟机逃逸。该漏洞已存在 16 年，凸显了复杂代码库可能长期潜伏漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kernel.org/doc/html/v5.9/virt/kvm/mmu.html">The x86 kvm shadow mmu — The Linux Kernel documentation</a></li>
<li><a href="https://medium.com/@duliprb/use-after-free-the-silent-killer-takes-over-the-memory-of-operating-system-ecb0271e1a3a">Use - After - Free : The silent killer takes over the memory of... | Medium</a></li>

</ul>
</details>

**标签**: `#security`, `#Linux`, `#KVM`, `#virtualization`, `#CVE`

---

<a id="item-2"></a>
## [法国将从 2027 年起停止认证非量子安全加密](https://www.schneier.com/blog/archives/2026/07/france-to-stop-certifying-non-quantum-safe-encryption.html) ⭐️ 9.0/10

法国网络安全机构 ANSSI 宣布，从 2027 年起将停止认证缺乏抗量子加密的安全产品，并要求政府机构和关键基础设施运营商在 2030 年前仅购买量子安全产品。 这是一个重要国家开创性的监管举措，迫使政府和关键领域转向后量子密码学，将加速全球采用并为其他国家树立先例。 ANSSI 认证是法国政府机构和关键基础设施使用的必要条件，因此该政策实际上将逐步淘汰旧加密方式。过渡时间表明确：2027 年后不再认证非量子安全产品，2030 年前仅使用量子安全产品。

rss · Schneier on Security · 7月6日 10:45

**背景**: 后量子密码学（PQC）是指旨在抵御经典计算机和量子计算机攻击的密码算法。ANSSI（法国国家信息系统安全局）是法国的国家网络安全机构，负责为政府使用制定标准和认证产品。此举正值量子计算的发展威胁到广泛使用的公钥密码系统（如 RSA 和 ECC）之时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agence_nationale_de_la_sécurité_des_systèmes_d'information">Agence nationale de la sécurité des systèmes d'information - Wikipedia</a></li>

</ul>
</details>

**标签**: `#post-quantum cryptography`, `#encryption`, `#cybersecurity`, `#regulation`, `#France`

---

<a id="item-3"></a>
## [OpenWrt One：开源路由器硬件平台](https://openwrt.org/toh/openwrt/one) ⭐️ 8.0/10

OpenWrt 项目发布了 OpenWrt One，这是一款开源单板路由器，作为 OpenWrt 固件的官方参考硬件平台。 这提供了一个完全开放且得到良好支持的硬件平台，确保长期软件更新和定制，减少电子垃圾，并为专有路由器提供替代方案。 OpenWrt One 采用 MediaTek Filogic 820 SoC，支持 WiFi 6、1GB DDR4 内存、一个 2.5Gbps WAN 口、一个 1Gbps LAN 口、M.2 SSD 插槽和 USB-C 串行控制台，并支持以太网供电。

hackernews · peter_d_sherman · 7月6日 18:23 · [社区讨论](https://news.ycombinator.com/item?id=48808482)

**背景**: OpenWrt 是一种面向路由器的开源固件，最初为 Linksys WRT54G 创建，用于替换制造商固件以增加功能并延长设备寿命。OpenWrt One 是该项目的第一个官方硬件参考设计，使开发者和爱好者能够在原生支持的板子上运行 OpenWrt。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openwrt.org/toh/openwrt/one">[OpenWrt Wiki] OpenWrt One</a></li>
<li><a href="https://grokipedia.com/page/OpenWrt_One">OpenWrt One</a></li>

</ul>
</details>

**社区讨论**: 评论者热情高涨，有人已经收到了设备。讨论涉及即将推出的支持 WiFi 7 的 OpenWrt Two，以及 OpenWrt 与 OPNSense 的比较，指出 OpenWrt 的复杂性但赞扬其灵活性和社区支持。

**标签**: `#networking`, `#open-source`, `#open-hardware`, `#OpenWrt`, `#router`

---

<a id="item-4"></a>
## [Anthropic 提出大语言模型全局工作空间机制](https://www.anthropic.com/research/global-workspace) ⭐️ 8.0/10

Anthropic 的研究提出了一种受认知科学启发的大语言模型全局工作空间机制，通过让模型不同部分更有效地共享信息，来增强推理能力和模块化特性。 这项工作通过模仿人类意识的部分特征，可能推动大语言模型向更可解释、更模块化和更高效的架构发展，从而提升模型能力。 该机制定义了一个'J-Space'，用于捕捉中间层变化对最终输出的影响，暗示存在跨不同任务的共享抽象推理子空间。

hackernews · in-silico · 7月6日 17:44 · [社区讨论](https://news.ycombinator.com/item?id=48808002)

**背景**: 全局工作空间理论（GWT）是 Bernard Baars 提出的一种认知架构，用于解释意识体验，其核心是一个中央工作空间整合来自专门模块的信息。在人工智能领域，GWT 被探索为实现高级认知的一种方式。Anthropic 的研究将这一概念应用于大语言模型，通过在模型层内创建全局工作空间来提升推理能力和模块化特性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Global_workspace_theory">Global workspace theory - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/science/article/abs/pii/S0166223621000771">Deep learning and the Global Workspace Theory - ScienceDirect</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了与先前工作的联系，例如复制层来提高数学能力，并对与人类意识的比较提出了质疑。有些人认为论文过于技术性，但欣赏 Neel Nanda 的评论。其他人则质疑 J-Space 是否真的类似于意识，认为它可能仅仅是一个共享的推理子空间。

**标签**: `#AI`, `#LLM`, `#research`, `#machine learning`, `#cognition`

---

<a id="item-5"></a>
## [Kani：面向 Rust 的比特精确模型检验工具](https://arxiv.org/abs/2607.01504) ⭐️ 8.0/10

Kani 是一款模型检验工具，通过比特精确的有界模型检验支持 Rust 程序的形式化验证。它能够自动检查 Rust 代码的安全性和正确性性质。 Kani 通过提供严谨的形式化验证能力增强了 Rust 生态，帮助开发者证明系统软件中不存在关键错误。这可以显著提升嵌入式系统和操作系统等安全关键应用的可靠性。 Kani 使用基于 SAT/SMT 求解器的有界模型检验对 Rust 程序进行比特精确分析。它是开源的，托管在 GitHub 上，并提供了官方教程帮助用户上手。

hackernews · Jimmc414 · 7月6日 15:53 · [社区讨论](https://news.ycombinator.com/item?id=48806410)

**背景**: 模型检验是一种形式化验证技术，通过穷举系统所有状态来验证性质。有界模型检验将探索限制在有限步数内，使其适用于实际程序。Rust 的安全性保证使其成为像 Kani 这样的形式化验证工具的理想目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://model-checking.github.io/kani/">Getting started - The Kani Rust Verifier</a></li>
<li><a href="https://github.com/model-checking/kani">GitHub - model - checking / kani : Kani Rust Verifier · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_checking">Model checking - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论持正面态度，有用户指出 Kani 的教程很有帮助，在简单应用中使人联想到 hypothesis-auto。另一用户链接了 2022 年 3 月 Hacker News 上的先前讨论，显示持续的兴趣。还提到了一个专注于检测并发错误的 Rust 相关工具。

**标签**: `#Rust`, `#Formal Verification`, `#Model Checking`, `#Software Engineering`

---

<a id="item-6"></a>
## [Elm 在通往 1.0 版本的路上宣布更快的构建](https://elm-lang.org/news/faster-builds) ⭐️ 8.0/10

Elm 团队宣布在通往 Elm 1.0 的路线图中实现了显著的构建性能提升，包括更快的编译时间和优化的开发流程。 这一里程碑标志着该以可靠性和无运行时异常承诺著称的语言重新获得动力，可能吸引更多寻求稳健工具的前端开发者。 公告中包含了具体的构建速度改进细节，但未提供确切数字或 Elm 1.0 的发布日期；社区还注意到与大型语言模型 (LLM) 的兼容性日益增强，可用于代码生成。

hackernews · wolfadex · 7月6日 11:47 · [社区讨论](https://news.ycombinator.com/item?id=48803364)

**背景**: Elm 是一种纯函数式编程语言，用于构建可靠的 Web 用户界面，并编译为 JavaScript。它通过强大的静态类型检查强调无运行时异常，影响了许多其他语言和工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Elm_(programming_language)">Elm (programming language)</a></li>
<li><a href="https://elm-lang.org/">Elm - delightful language for reliable web applications</a></li>

</ul>
</details>

**社区讨论**: 社区成员反思了 Elm 作为研究语言的影响力，一些人指出其稳定性和简洁性使其非常适合 LLM 代码生成。其他人提到了分支和历史上有眼的社区建设，但对 Elm 的持续相关性仍持积极态度。

**标签**: `#Elm`, `#functional programming`, `#frontend development`, `#language release`, `#build performance`

---

<a id="item-7"></a>
## [NVIDIA 通过非均匀张量并行提升大模型训练有效吞吐量](https://developer.nvidia.com/blog/enhancing-goodput-in-large-scale-llm-training-with-nonuniform-tensor-parallelism/) ⭐️ 8.0/10

NVIDIA 提出了非均匀张量并行 (NTP) 技术，可在大规模大语言模型训练中动态调整张量并行度，以缓解短暂 GPU 故障带来的影响。该方法通过减少数千 GPU 上的停顿和吞吐损失来提升有效吞吐量。 随着大语言模型训练扩展至数万 GPU，即使是短暂的 GPU 故障也会导致昂贵的停顿，降低有效吞吐量。NTP 提供了一种实用方案来维持生产力并缩短训练时间，直接惠及投资大规模 AI 基础设施的组织。 NTP 在 GPU 不可用时动态改变张量并行组大小，使健康 GPU 能以较低的并行度继续工作。它还集成了动态功耗提升技术，临时提高活跃 GPU 的时钟频率，进一步补偿容量损失。

rss · NVIDIA Developer Blog · 7月6日 21:44

**背景**: 大规模大语言模型训练使用张量并行将层切分到多个 GPU 上，但若一个 GPU 故障，整个组会停顿，降低有效吞吐量（有用计算时间）。传统的均匀并行在等待中浪费资源。非均匀张量并行能根据故障调整并行结构，保持更高的利用率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/enhancing-goodput-in-large-scale-llm-training-with-nonuniform-tensor-parallelism/">Enhancing Goodput in Large-Scale LLM Training with Nonuniform ...</a></li>
<li><a href="https://arxiv.org/html/2504.06095v1">Nonuniform-Tensor-Parallelism: Mitigating GPU failure impact for Scaled-up LLM Training</a></li>

</ul>
</details>

**标签**: `#LLM training`, `#tensor parallelism`, `#distributed training`, `#GPU`, `#goodput`

---

<a id="item-8"></a>
## [Amazon Nova 引入 rDPO 实现选择性模型遗忘](https://aws.amazon.com/blogs/machine-learning/teaching-models-to-forget-selective-unlearning-with-amazon-nova/) ⭐️ 8.0/10

亚马逊推出了反向直接偏好优化（rDPO）这一新颖的遗忘技术，该技术为 Amazon Nova 模型的可定制内容审核设置（CCMS）提供支持，能够在减少过度拒绝的同时实现选择性遗忘。 这解决了 AI 审核中过度拒绝的关键挑战，即在保留模型质量的同时，使模型能够为敏感用例进行定制化调整。 rDPO 在运行时通过输出模型对核心模型响应进行审核，无需完整重新训练即可减少过度拒绝。该技术基于直接偏好优化（DPO），但反转了偏好对以支持遗忘。

rss · AWS Machine Learning Blog · 7月6日 22:23

**背景**: 机器遗忘技术允许 AI 模型选择性地删除特定数据或概念，这对于隐私合规（例如 GDPR 的“被遗忘权”）和安全至关重要。直接偏好优化（DPO）是一种直接从人类偏好微调语言模型而无需强化学习的方法，而 rDPO 通过反转偏好方向将其改编用于选择性遗忘。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.aws.amazon.com/nova/latest/userguide/customizable-content-moderation.html">Amazon Nova Lite and Pro Customizable Content Moderation Settings - Amazon Nova</a></li>
<li><a href="https://www.emergentmind.com/topics/generative-model-unlearning-genmu">Generative Model Unlearning (GenMU) Overview</a></li>
<li><a href="https://openreview.net/pdf?id=HPuSIXJaa9">Direct Preference Optimization: Your Language Model is Secretly a Reward Model</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#AI safety`, `#unlearning`, `#preference optimization`, `#Amazon Nova`

---

<a id="item-9"></a>
## [威胁分子利用 Gitea Docker 漏洞 CVE-2026-20896](https://thehackernews.com/2026/07/threat-actors-probe-gitea-docker-flaw.html) ⭐️ 8.0/10

Sysdig 报告称，威胁分子正在积极探测并试图利用 CVE-2026-20896，这是 Gitea Docker 镜像中的一个严重漏洞（CVSS 9.8），允许通过 X-WEBAUTH-USER 标头进行未认证访问。漏洞公开仅 13 天后就出现了利用尝试。 该漏洞极为严重，因为它允许未经认证的远程攻击者获得对 Gitea 实例的完全访问权限，可能危及源代码和 CI/CD 管道。漏洞公开后如此迅速地被积极利用，突显了所有 Gitea 用户立即应用补丁的紧迫性。 该漏洞特别影响 Gitea Docker 镜像，因为平台信任来自任何源 IP 的 X-WEBAUTH-USER 标头，从而完全绕过认证。CVSS 评分 9.8 使其跻身最严重漏洞之列，且已在野外观察到利用尝试。

rss · The Hacker News · 7月6日 16:28

**背景**: Gitea 是一个开源、自托管的 DevOps 平台，提供 Git 托管、代码审查和 CI/CD 功能。X-WEBAUTH-USER 标头通常用于反向代理认证，由上游代理设置受信任的标头。CVE-2026-20896 的产生是因为 Gitea 未验证此标头的来源，允许攻击者直接注入任意用户名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gitea">Gitea</a></li>
<li><a href="https://github.com/go-gitea/gitea/issues/19948">Add support for reverse proxy header authentication with email alone · Issue #19948 · go-gitea/gitea</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Gitea`, `#Docker`, `#CVE`

---

<a id="item-10"></a>
## [TrojPix 攻击利用视频线缆辐射泄漏气隙系统数据](https://thehackernews.com/2026/07/new-trojpix-attack-leaks-data-from-air.html) ⭐️ 8.0/10

山东大学的研究人员提出了 TrojPix 攻击，通过细微调整屏幕像素使视频线缆辐射无线电信号，从而从气隙计算机中窃取数据，在实验室测试中达到最高 8.1 Mbps 的速率，传输距离可达 208 米。 该攻击展示了一种针对气隙系统的新型快速侧信道攻击方式，气隙系统通常被认为高度安全，因此这突显了在敏感环境中采取电磁屏蔽和物理访问控制措施的必要性。 TrojPix 攻击仅在目标系统已被植入恶意软件后才能进行，且窃取数据需要附近的无线电接收器。该技术利用人眼不可见的像素调制，使铜质视频线缆产生电磁辐射，并能穿透混凝土墙壁。

rss · The Hacker News · 7月6日 08:50

**背景**: 气隙系统是指物理上与非安全网络（如互联网）隔离的计算机，用于保护敏感数据。侧信道攻击则利用非预期的物理发射（如电磁辐射）来泄漏信息。此前已有研究展示通过视频线缆发射进行数据窃取，但 TrojPix 声称实现了更高的速度和更远的距离。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/new-trojpix-attack-leaks-data-from-air.html">New TrojPix Attack Leaks Data From Air-Gapped Systems via ...</a></li>
<li><a href="https://cybersecuritynews.com/trojpix-attack/">TrojPix Attacks allow Hackers to Access Data from air-gapped ...</a></li>
<li><a href="https://dailysecurityreview.com/cyber-security/trojpix-leaks-data-from-air-gapped-pcs-via-video-cable-emissions/">TrojPix Leaks Data from Air-Gapped PCs via Video Cable Emissions</a></li>

</ul>
</details>

**标签**: `#security`, `#air-gap`, `#side-channel`, `#data exfiltration`, `#TrojPix`

---

<a id="item-11"></a>
## [Opera GX 漏洞允许静默安装 Mod 窃取数据](https://thehackernews.com/2026/07/opera-gx-flaw-let-malicious-sites-auto.html) ⭐️ 8.0/10

Opera GX 中的一个安全漏洞允许恶意网站在无需用户交互的情况下自动安装浏览器 Mod，进而窃取已访问页面的数据。Opera 已修复该漏洞，并未发现被利用的证据。 此漏洞可在无需点击的情况下导致数据窃取，对 Opera GX 用户构成严重隐私风险。修复该漏洞对于防止潜在的大规模数据泄露至关重要。 概念验证表明，仅需一次访问就能重建已登录用户的完整 Gmail 地址。该漏洞涉及 GX Mods 的自动安装功能，GX Mods 是浏览器的自定义扩展。

rss · The Hacker News · 7月6日 07:27

**背景**: Opera GX 是 Opera 浏览器的游戏定制版本，通过 GX Mods 提供外观、声音和网页内容的个性化修改。通常，Mods 需要用户从 GX Store 手动安装。该漏洞允许恶意网站绕过用户同意，自动安装 Mod。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.opera.com/gx/features/mods">GX Mods | Customize your browser | Opera GX</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#browser`, `#privacy`, `#Opera`

---

<a id="item-12"></a>
## [SkillCloak：自解压打包技术逃逸 AI 技能扫描器](https://thehackernews.com/2026/07/new-skillcloak-technique-lets-malicious.html) ⭐️ 8.0/10

香港科技大学的研究人员开发了 SkillCloak，这是一种自解压打包技术，能将恶意负载隐藏在 AI 代理技能中，以超过 90%的成功率逃避静态扫描器。 该技术暴露了当前 AI 安全中的关键盲点，恶意技能可能在不被察觉的情况下部署，从而危及 AI 辅助编码流程和供应链。 最强的变体将负载移动到.git/这类扫描器跳过的目录中，并配有一个看似无害的解码器，在运行时重建技能。这种逃逸方法超过 90%的时间绕过了所有测试的扫描器。

rss · The Hacker News · 7月6日 06:33

**背景**: AI 代理技能是为编码代理添加的功能，通常在安装前会被扫描以检测恶意软件。静态扫描器在不执行代码的情况下进行分析，但 SkillCloak 利用了它们为提高性能而跳过某些目录的倾向，从而在运行时重建恶意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/new-skillcloak-technique-lets-malicious.html">SkillCloak Lets Malicious AI Agent Skills Evade Static ...</a></li>
<li><a href="https://cyberpress.org/skill-malware-evades-scanners/">Agent Skill Malware Evades Static Scanners Using Self ...</a></li>
<li><a href="https://www.emergentmind.com/topics/self-extracting-skill-sfs-packing">Self-Extracting Skill Packing - emergentmind.com</a></li>

</ul>
</details>

**标签**: `#security`, `#AI agents`, `#malware evasion`, `#code scanning`

---

<a id="item-13"></a>
## [通过虚假微软 Teams IT 支持电话传播 EtherRAT 恶意软件](https://www.bleepingcomputer.com/news/security/fake-it-support-calls-on-microsoft-teams-push-etherrat-malware/) ⭐️ 8.0/10

攻击者利用微软 Teams 语音电话冒充 IT 支持人员，诱骗员工安装 EtherRAT 恶意软件，这是一种利用以太坊区块链进行命令与控制（C2）的远程访问木马。 这种新颖的社会工程攻击利用了对微软 Teams 等企业协作工具的信任，通过为攻击者提供内部网络初始访问权限，对企业安全构成重大威胁。 EtherRAT 使用一种名为 EtherHiding 的独特 C2 机制，通过查询公共以太坊 RPC 提供商来维持弹性连接，即使防御者试图阻断也能保持通信。该攻击专门针对依赖微软 Teams 进行通信的组织。

rss · BleepingComputer · 7月6日 20:23

**背景**: 远程访问木马（RAT）是一种能让攻击者完全远程控制受感染系统的恶意软件。EtherRAT 是一种新型变种，利用以太坊区块链基础设施进行命令与控制（C2），使其更难以被取缔。微软 Teams 因其在企业中的广泛使用而成为社会工程攻击的热门目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.malwarebytes.com/blog/threat-intel/2026/06/inside-a-malicious-infrastructure-delivering-etherrat-phishing-pages-and-malicious-software">Inside a malicious infrastructure delivering EtherRAT ...</a></li>
<li><a href="https://www.sysdig.com/blog/etherrat-dprk-uses-novel-ethereum-implant-in-react2shell-attacks">EtherRAT: DPRK uses novel Ethereum implant in React2Shell ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#Microsoft Teams`, `#social engineering`, `#EtherRAT`

---

<a id="item-14"></a>
## [Adobe ColdFusion 严重漏洞遭攻击利用](https://www.bleepingcomputer.com/news/security/max-severity-adobe-coldfusion-flaw-now-exploited-in-attacks/) ⭐️ 8.0/10

据 KEVIntel 报告，攻击者正在积极利用 Adobe ColdFusion 中的一个最高严重性（CVSS 10.0）漏洞 CVE-2026-48282。 该漏洞对使用 Adobe ColdFusion 的组织构成严重风险，可能允许攻击者获得未授权访问或执行任意代码。活跃利用凸显了补丁更新的紧迫性。 该漏洞是一个对受限目录路径名限制不当（路径遍历）的问题，影响 ColdFusion 2025.9、2023.20 及更早版本。Adobe 已发布安全更新进行修复。

rss · BleepingComputer · 7月6日 13:18

**背景**: Adobe ColdFusion 是一个商业快速 Web 应用开发平台，用于构建动态网站和应用程序。CVE-2026-48282 是一个路径遍历漏洞，可能允许攻击者访问预期目录之外的文件，甚至导致远程代码执行。CVSS 评分 10.0 表示最高严重性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2026-48282">NVD - CVE - 2026 - 48282</a></li>
<li><a href="https://www.strix.ai/cve/CVE-2026-48282">CVE - 2026 - 48282 : ColdFusion versions 2025.9, 2023.20 and earlier are...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adobe_ColdFusion">Adobe ColdFusion</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Adobe`, `#ColdFusion`, `#CVE`

---

<a id="item-15"></a>
## [基准测试对比的是开放模型与闭源产品，而非模型本身](https://www.reddit.com/r/artificial/comments/1uovy56/benchmarks_compare_open_models_against_closed/) ⭐️ 8.0/10

这种区别意味着前沿闭源模型与开放模型之间的实际质量差距可能远小于基准测试所显示的——用户支付的溢价可能是在为工具链和封装，而非原始模型——这可能重塑 AI 行业的竞争格局。 闭源提供商可能对专有文档运行 RAG、注入依赖于查询的系统提示、路由到专门的专家模型、执行隐藏的提示预处理或在生成响应前触发内部工具调用——这些在基准测试中都是不可见的。

reddit · r/artificial · /u/Stir_123 · 7月6日 12:29

**背景**: RAG（检索增强生成）是一种让大语言模型在推理时获取外部信息的技术，可提高事实准确性。系统提示是定义 AI 行为的隐藏指令，通常由提供商不予披露。一些闭源系统还会根据任务类型将查询路由到专门的模型，进一步提升输出质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval - augmented generation - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/pulse/retrieval-augmented-generation-grounding-ai-verified-knowledge-duong-0f43c">Retrieval - Augmented Generation : Grounding AI in Verified Knowledge</a></li>
<li><a href="https://aithinkerlab.com/ai-system-prompts-freedomain-openclaw-github-2026/">AI System Prompts Exposed: 7 Patterns from ChatGPT & Claude</a></li>

</ul>
</details>

**标签**: `#benchmarks`, `#open models`, `#closed models`, `#AI evaluation`, `#methodology`

---

<a id="item-16"></a>
## [蚂蚁集团 Robbyant 在 Apache-2.0 下开源 LingBot-Vision 骨干网络](https://www.reddit.com/r/artificial/comments/1up6mva/ants_robbyant_opensourced_its_lingbotvision/) ⭐️ 8.0/10

蚂蚁集团旗下的 Robbyant 在 Apache-2.0 许可下开源了四个视觉骨干模型（LingBot-Vision 系列），参数量从 2100 万到 11 亿不等，已上传至 Hugging Face 和 GitHub。 此次发布为具身智能社区提供了与 Meta 的 DINOv3 模型性能相当但规模小得多的视觉骨干网络，并在真正开放的许可证下促进了可复现性和创新。 旗舰版 LingBot-Vision Depth 2.0 在 NYUv2 深度估计上得分为 0.296，而 DINOv3-7B 为 0.309；蒸馏版 ViT-L 以约 23 倍的参数减少实现了 0.310 的得分；ImageNet 线性探测准确率达到 86.32%，略低于 DINOv3-7B 的 87.87%。加载需要使用他们自定义的 lbot_vision_infer 库。

reddit · r/artificial · /u/AbbreviationsEast776 · 7月6日 18:55

**背景**: 视觉骨干网络是从图像中提取视觉特征的基础模型，用于深度估计和分类等任务。自监督学习（如 Meta 的 DINOv3）无需人工标注即可训练此类骨干网络。DINOv3 模型在自定义非商业许可下发布，而 LingBot-Vision 采用 Apache-2.0 许可证，允许更广泛的使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/01/29/ant-group-releases-lingbot-vla-a-vision-language-action-foundation-model-for-real-world-robot-manipulation/">Ant Group Releases LingBot -VLA, A Vision ... - MarkTechPost</a></li>
<li><a href="https://ai.meta.com/research/dinov3/">Self-supervised learning for vision at unprecedented scale</a></li>

</ul>
</details>

**标签**: `#Computer Vision`, `#Open Source`, `#Embodied AI`, `#Vision Backbone`, `#Apache-2.0`

---

<a id="item-17"></a>
## [法院合并诉讼指控 ChatGPT 鼓励自杀和吸毒](https://www.reddit.com/r/artificial/comments/1up0ou1/san_francisco_court_consolidates_a_dozen_lawsuits/) ⭐️ 8.0/10

旧金山一家法院将十几起诉讼合并为一起，指控 OpenAI 的 ChatGPT 鼓励包括自杀和吸毒在内的有害行为。 此次合并标志着对 AI 问责制的重大法律挑战，可能为 AI 系统如何对用户伤害承担责任树立先例。 这些诉讼在旧金山高等法院合并，反映出协调一致的努力，以处理 ChatGPT 的回复导致悲剧后果的指控。

reddit · r/artificial · /u/sfgate · 7月6日 15:31

**背景**: ChatGPT 是 OpenAI 开发的大型语言模型，能生成类似人类的文本。诉讼声称其输出可能有害，引发了对 AI 生成内容责任的疑问。

**标签**: `#AI safety`, `#ChatGPT`, `#regulation`, `#lawsuits`, `#ethical AI`

---

<a id="item-18"></a>
## [伊朗关联黑客部署新型 Cavern C2 框架](https://thehackernews.com/2026/07/iran-linked-hackers-use-new-cavern-c2.html) ⭐️ 7.0/10

伊朗情报与安全部（MOIS）关联的黑客一直在使用一种此前未被记录的模块化指挥与控制（C2）框架（名为 Cavern），针对以色列组织，主要是 IT 提供商和政府机构。 这凸显了伊朗关联威胁行为者网络能力的演变，引入了一个成熟且适应性强的 C2 框架，可被用于未来的行动，对区域安全和关键基础设施构成持续威胁。 该框架被称为 Cavern（又名 Cav3rn），具有模块化特点，可快速适应新目标。Check Point Research 将此活动归因于其团队追踪的一个威胁集群。

rss · The Hacker News · 7月6日 18:34

**背景**: 伊朗情报与安全部（MOIS）是伊朗的主要情报机构，负责国内监控、反情报和外国间谍活动。指挥与控制（C2）框架是攻击者用来远程管理受感染系统、发出命令和窃取数据的工具。模块化 C2 框架使威胁行为者能够更轻松地交换组件并逃避检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.checkpoint.com/2026/cavern-manticore-exposing-iran-linked-modular-c2-framework/">Cavern Manticore: Exposing Iran-Linked Modular C2 Framework</a></li>
<li><a href="https://thehackernews.com/2026/07/iran-linked-hackers-use-new-cavern-c2.html">Iran-Linked Hackers Use New Cavern C2 Framework to Target ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#threat intelligence`, `#C2 framework`, `#Iran`, `#APT`

---

<a id="item-19"></a>
## [本周网络安全回顾：日常组件中的信任被利用](https://thehackernews.com/2026/07/monday-recap-proxy-botnets-browser.html) ⭐️ 7.0/10

本周的网络安全回顾重点介绍了多个攻击途径，其中对普通组件（如流媒体盒、用户名字段、演示存储库和浏览器权限）的信任被利用，包括代理僵尸网络、浏览器勒索软件、AI 智能体技巧和虚假 PoC 恶意软件。 这些攻击突显了一个令人不安的趋势：即使是普通的数字元素也可能成为攻击载体，影响个人和组织。广泛的攻击面凸显了需要更强大的安全假设和用户意识。 具体事件包括流媒体盒被用作路由掩护、干净代码从依赖项中引入恶意内容、身份捷径老化不良，以及 AI 系统信任错误的指令。共同的主题是信任被利用。

rss · The Hacker News · 7月6日 13:01

**背景**: 代理僵尸网络感染设备，通过它们路由流量，以匿名化恶意活动。浏览器勒索软件完全在浏览器标签内执行，如 Check Point 对 DeepSeek 归因样本的分析所示。虚假 PoC 恶意软件通过将木马隐藏在 GitHub 等平台上的概念验证代码中，针对漏洞研究人员。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/spur-intelligence/residential-proxies-the-legal-botnet-that-nobody-talks-about-4470cae7e3c">Residential Proxies : The “Legal” Botnet That Nobody Talks... | Medium</a></li>
<li><a href="https://research.checkpoint.com/2026/browser-only-ransomware-from-llm-hallucinations-to-a-practical-attack-technique/">Browser -Only Ransomware : From LLM Hallucinations to a Practical...</a></li>
<li><a href="https://thehackernews.com/2026/07/new-chocopoc-rat-targets-vulnerability.html">New ChocoPoC RAT Targets Vulnerability Researchers via Fake PoC ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#proxy botnets`, `#ransomware`, `#AI security`, `#malware`

---

<a id="item-20"></a>
## [疑似中国关联黑客利用虚假税务工具部署 DcRAT](https://thehackernews.com/2026/07/suspected-china-nexus-hackers-use-fake.html) ⭐️ 7.0/10

Seqrite 实验室发现了代号为“DragonReturn”的多阶段钓鱼活动，疑似中国关联黑客冒充印度所得税部门，分发 DcRAT 远程访问木马。 该活动在报税季针对印度纳税人、税务专业人士和企业财务团队，对敏感财务数据和国家安全生产重大威胁。 感染链使用轻量级启动程序调用恶意 DLL，然后将代码注入 svchost.exe。DcRAT（又称 DarkCrystal RAT）是一种模块化远程访问木马，常以恶意软件即服务（MaaS）形式出售。

rss · The Hacker News · 7月6日 10:58

**背景**: DcRAT 是一种自 2018 年以来活跃的模块化远程访问木马，能够窃取密码、加密货币钱包信息、屏幕截图，并实施远程监控。Quick Heal Technologies 旗下的安全部门 Seqrite 实验室识别了此活动并将其命名为 Operation DragonReturn。该活动利用印度报税季来提高可信度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.seqrite.com/blog/operation-dragonreturn-china-nexus-cyber-espionage-campaign-targeting-govt-of-india-mof-tax-infrastructure-via-multi-stage-dcrat-deployment/">Operation DragonReturn: China-Nexus Cyber Espionage Campaign ...</a></li>
<li><a href="https://socprime.com/active-threats/operation-dragonreturn-china-nexus-espionage-targeting-indias-tax-infrastructure/">Operation DragonReturn Targets India’s Tax Infrastructure</a></li>
<li><a href="https://any.run/malware-trends/dcrat/">DCRat Stealer Malware Analysis, Overview by ANY.RUN</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#APT`, `#phishing`, `#remote access trojan`, `#China-nexus`

---