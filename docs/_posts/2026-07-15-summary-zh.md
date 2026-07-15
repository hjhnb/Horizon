---
layout: default
title: "Horizon Summary: 2026-07-15 (ZH)"
date: 2026-07-15
lang: zh
---

> 从 87 条内容中筛选出 20 条重要资讯。

---

1. [CISA 警告 ABB T-MAC Plus 存在严重漏洞](#item-1)
2. [微软修复创纪录的 622 个漏洞，包含两个已遭利用的零日漏洞](#item-2)
3. [Grok Build 将整个 Git 仓库上传至云存储](#item-3)
4. [频谱分析揭示神经网络中的普适结构信号](#item-4)
5. [Bonsai 27B：可在手机上运行的 270 亿参数 AI 模型](#item-5)
6. [不断升高的塔楼](#item-6)
7. [我们是否将太多思考外包给了 AI？](#item-7)
8. [Linux 输入延迟测量：X11 对比 Wayland、VRR 与 DXVK](#item-8)
9. [Armin Ronacher：共享语言与 AI 代理的冲击](#item-9)
10. [NVIDIA 分享 Kaggle 竞赛提升 AI 推理的教训](#item-10)
11. [CISA 敦促立即加固 SharePoint 以应对活跃利用](#item-11)
12. [CISA 警告 Rockwell 1715-AENTR 适配器存在严重漏洞](#item-12)
13. [SAP 修复 NetWeaver ABAP 严重漏洞，CVSS 9.9](#item-13)
14. [RabbitMQ 漏洞可泄露 OAuth 密钥并暴露跨租户元数据](#item-14)
15. [11 个微软签名的旧 UEFI Shim 可绕过 Secure Boot](#item-15)
16. [加密货币钱包扩展泄露地址，实现追踪](#item-16)
17. [OAuth 客户端 ID 欺骗可让攻击者验证被盗的 Entra 凭据](#item-17)
18. [苹果起诉 OpenAI；谷歌用 AI 摘要改造搜索](#item-18)
19. [AI 智能体生产部署：缺乏基础设施](#item-19)
20. [纽约州长暂停数据中心审批](#item-20)

---

<a id="item-1"></a>
## [CISA 警告 ABB T-MAC Plus 存在严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-195-03) ⭐️ 9.0/10

CISA 披露了 ABB T-MAC Plus 中的多个严重漏洞，CVSS 评分为 9.9，影响 4.0-24 版本。ABB 已发布 4.0-25 版更新以修复这些问题。 这些严重漏洞可能允许经过身份验证的远程攻击者破坏系统的机密性、完整性和可用性，从而可能扰乱全球的关键制造业运营。 这些漏洞包括文件泄露（CWE-552）、通过用户控制密钥的授权绕过（CWE-639）、跨站脚本（CWE-79）和不正确的授权（CWE-863）。CVSS 向量（AV:N/AC:L/PR:L/UI:N/S:C/C:H/I:H/A:H）表明攻击者可通过网络利用，复杂度低，无需用户交互。

rss · CISA Cybersecurity Advisories · 7月14日 12:00

**背景**: ABB T-MAC Plus 是一个终端管理系统，用于石油、天然气和化工等关键制造业领域，管理库存和产品发运。CISA 的公告遵循通用安全公告框架（CSAF）格式，该格式支持安全漏洞信息的自动化交换。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ticintl.com/products/terminal-management/abb-ability-t-mac-plus/">ABB Ability™ T-MAC Plus | TIC International</a></li>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CISA`, `#ABB`, `#industrial control systems`

---

<a id="item-2"></a>
## [微软修复创纪录的 622 个漏洞，包含两个已遭利用的零日漏洞](https://thehackernews.com/2026/07/microsoft-patches-record-622-flaws.html) ⭐️ 9.0/10

微软于 2026 年 7 月发布了史上最大规模的补丁星期二更新，修复了 622 个漏洞，其中包括两个正在被积极利用的零日漏洞和一个已公开披露的漏洞。 此次创纪录的补丁发布凸显了日益严峻的威胁态势以及立即打补丁的重要性，尤其是攻击者已在利用其中两个漏洞。全球 IT 团队必须优先应用这些更新，以防止潜在的攻击入侵。 微软将漏洞发现数量的激增部分归因于人工智能辅助的漏洞检测。这 622 个 CVE 不包括另外的 427 个影响 Microsoft Edge 的 Chromium 漏洞；其中 62 个 CVE 标记为严重（critical）级别。

rss · The Hacker News · 7月14日 20:25

**背景**: 补丁星期二（Patch Tuesday）是微软每月为其产品发布安全更新的固定周期，通常修复几十个漏洞。每个漏洞都会被分配一个 CVE（通用漏洞披露）标识符以便追踪。此前的纪录是 2026 年 6 月修复了约 200 个漏洞，而本月修复的 622 个漏洞是这一数字的三倍多。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://msrc.microsoft.com/update-guide">Security Update Guide - Microsoft</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerabilities_and_Exposures">Common Vulnerabilities and Exposures - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#Microsoft`, `#Patch Tuesday`, `#zero-day`, `#vulnerabilities`

---

<a id="item-3"></a>
## [Grok Build 将整个 Git 仓库上传至云存储](https://thehackernews.com/2026/07/grok-build-uploads-entire-git.html) ⭐️ 9.0/10

xAI 的 Grok Build CLI（0.2.93 版本）被发现将完整的 Git 仓库（包括全部提交历史）上传至 Google Cloud Storage 存储桶，而不仅仅是编码任务所需的文件。研究人员 cereblab 捕获并提取了该上传内容，发现了代理被明确指示不得访问的敏感文件。 这一广泛使用的 AI 编码工具中的严重隐私和安全漏洞，将用户的完整仓库历史（包括密钥、凭据和专有代码）暴露给 xAI 的云基础设施。它破坏了人们对 AI 辅助开发工具的信任，并引发了关于数据处理和用户同意的紧迫问题。 研究人员使用中间人代理拦截了一次 HTTPS 上传，该上传是一个包含整个仓库的 git bundle 文件。恢复的文件包含了代理被明确告知不得读取或修改的更改内容。

rss · The Hacker News · 7月14日 09:02

**背景**: Grok Build 是 xAI（Grok 语言模型背后的公司）推出的一款新型编码 CLI，作为基于终端的编码代理，能够规划、审查和批准代码更改。它于 2026 年 5 月进入早期测试阶段，面向 SuperGrok 和 X Premium Plus 订阅用户。Git bundle 是 Git 仓库的二进制归档文件，可以像远程仓库一样被克隆或获取，通常用于离线传输或备份。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://x.ai/news/grok-build-cli">Introducing Grok Build | SpaceXAI</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>

</ul>
</details>

**标签**: `#Security`, `#Privacy`, `#AI`, `#Data Leak`, `#Git`

---

<a id="item-4"></a>
## [频谱分析揭示神经网络中的普适结构信号](https://www.reddit.com/r/artificial/comments/1uwjwl6/opening_the_black_box_unison_zero_parameter_model/) ⭐️ 9.0/10

研究人员引入了一种新的频谱分析技术（Unison 零参数模型），将神经网络权重转换为频谱基底，发现 11 个从 4B 到 1 万亿参数的模型中，词元嵌入始终携带强结构信号。该方法已预注册且可复现，并且发现删除 GPT-2 最响亮的 1.5%频谱系数会破坏模型，而随机删除几乎无影响。 这一神经网络可解释性方面的突破为理解模型内部提供了新视角，可能改变我们理解和分析 AI 模型的方式。它表明检测到的结构不是计算的痕迹，而是计算本身，对 AI 安全、模型调试和理解训练动态具有重要意义。 该技术在 11 个从 4B 到 1 万亿参数的模型上进行了测试，包括 GPT-2，并显示训练实时写入结构：词元嵌入在步骤 256 首次激活，在步骤 4000 左右达到峰值，然后稳定下来。该方法还能读取记忆的训练数据，模型能逐字复现训练语料中的文本（如葛底斯堡演说：9 个词），而对未见文本显示为零。

reddit · r/artificial · /u/A_Freaky-Frog · 7月14日 20:12

**背景**: 神经网络可解释性旨在理解 AI 模型如何做出决策。传统方法在处理大模型时常常困难。频谱分析研究权重矩阵的特征值或奇异值分布，随机矩阵理论（RMT）预测初始化时应遵循特定普适分布（如维格纳半圆律）。训练后的网络会表现出非普适的离群值，指示学习到的结构。Unison 方法应用这些原理来识别不同规模模型中词元嵌入的结构信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mdpi.com/2813-0324/13/1/8">Spectral Analysis of Neural Network Weight Matrices and the ...</a></li>
<li><a href="https://arxiv.org/html/2507.12709v2">From SGD to Spectra: A Theory of Neural Network Weight Dynamics</a></li>

</ul>
</details>

**标签**: `#neural network interpretability`, `#spectral analysis`, `#machine learning research`, `#AI safety`, `#token embeddings`

---

<a id="item-5"></a>
## [Bonsai 27B：可在手机上运行的 270 亿参数 AI 模型](https://prismml.com/news/bonsai-27b) ⭐️ 8.0/10

PrismML 发布了 Bonsai 27B，这是一个通过量化压缩至可在移动设备上运行的 270 亿参数语言模型。该模型采用先进的压缩技术，将其大小从约 50GB 缩减至 4GB 以下，同时保留了大部分智能。 这一突破使得拥有 270 亿参数的大型语言模型能够在智能手机上本地运行，减少对云端推理的依赖，提升隐私性和响应速度。它为边缘设备上的高效 AI 部署树立了新标杆，可能加速设备端 AI 应用的发展。 该模型通过量化实现了 12.5 倍的大小缩减，从 50GB 降至约 4GB。社区初步报告显示，工具调用性能受到明显影响，部分用户在 LM Studio 中遇到了兼容性问题。

hackernews · xenova · 7月14日 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48910545)

**背景**: 模型量化是一种将权重和激活值从 32 位浮点数降低到较低位宽（如 4 位整数）的技术，从而大幅减少内存和计算需求。高效的 AI 压缩技术，如量化、剪枝和知识蒸馏，对于在手机等资源受限设备上部署大型模型至关重要。Bonsai 27B 利用这些方法将 270 亿参数模型适配到移动设备有限的存储和内存中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/model-quantization-concepts-methods-and-why-it-matters/">Model Quantization: Concepts, Methods, and Why It Matters | NVIDIA Technical Blog</a></li>
<li><a href="https://huggingface.co/docs/optimum/en/concept_guides/quantization">Quantization · Hugging Face</a></li>
<li><a href="https://www.runpod.io/articles/guides/ai-model-compression-reducing-model-size-while-maintaining-performance-for-efficient-deployment">AI Model Compression for Efficient Deployment</a></li>

</ul>
</details>

**社区讨论**: 评论者将 Bonsai 27B 与 4 位 QAT 版本的 Gemma 4 12B 进行比较，指出两者大小相似但质疑其相对智能。有人对工具调用性能下降和演示准确性表示担忧。还有人提到苹果潜在的合作伙伴关系，并询问 Hugging Face 上与 LM Studio 的兼容性问题。

**标签**: `#AI`, `#quantization`, `#edge computing`, `#large language models`, `#efficient ML`

---

<a id="item-6"></a>
## [不断升高的塔楼](https://lucumr.pocoo.org/2026/7/13/the-tower-keeps-rising/) ⭐️ 8.0/10

Armin Ronacher 的文章《不断升高的塔楼》指出，AI 辅助编程虽然提升了个人的生产力，但并未解决大型软件项目中协调和共同理解这一根本挑战。 这之所以重要，是因为随着 AI 工具越来越普及，软件开发的瓶颈从代码生产转向了团队协作，需要新的方法论和工具来管理共享的概念理解。 文章将之与“Lisp 诅咒”和“两极 Lisp 程序员”概念相类比，指出仅靠可组合性不足以支撑大规模协作。它强调，项目的共同语言存在于文档、代码评审、对话和共享经验中，而不仅仅是编程语言。

hackernews · cdrnsf · 7月14日 16:57 · [社区讨论](https://news.ycombinator.com/item?id=48909785)

**背景**: 可组合性是一种系统设计原则，允许选择和组装各种组件以满足用户需求。在软件中，AI 辅助编程使用 AI 代理生成或修改代码，可能加快开发速度。然而，大型项目面临协调挑战，限制了更快个人编码带来的好处。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Composability">Composability - Wikipedia</a></li>
<li><a href="https://www.contentful.com/blog/what-is-composability/">What is composability? Definitions, examples, and why it matters | Contentful</a></li>

</ul>
</details>

**社区讨论**: 社区评论与文章论点一致：tekacs 将可组合性比作俄罗斯方块，指出代理常违反此原则；ssivark 引用 Lisp 诅咒，认为轻松的可组合性反而阻碍协作；sixtyj 强调协调而非代码速度才是限制；apinstein 指出共享理解比形式化语言更重要。

**标签**: `#software engineering`, `#composability`, `#AI-assisted programming`, `#coordination`

---

<a id="item-7"></a>
## [我们是否将太多思考外包给了 AI？](https://www.artfish.ai/p/offloading-thinking-to-ai) ⭐️ 8.0/10

artfish.ai 上一篇高评分文章质疑过度依赖 AI 进行思考是否有害，引发了关于技能退化与有效使用 AI 的讨论，评论数超过 350 条。 这场讨论对软件工程和 AI 伦理至关重要，因为它触及了使用 AI 可能削弱批判性思维能力的问题，尤其是那些依赖 AI 生成代码却不理解其含义的初级开发者。 社区评论揭示了具体案例，例如一位初级开发者无法解释 AI 生成的错误计算，以及计算器类比质疑将思考外包给 LLM 后人类角色是否还有价值。

hackernews · yenniejun111 · 7月14日 15:18 · [社区讨论](https://news.ycombinator.com/item?id=48908178)

**背景**: 认知外包是通过使用外部工具或辅助手段（如记笔记或使用计算器）来减少心智负荷的自然过程。借助 LLM，人们可以外包复杂的推理，但批评者警告这可能随着时间的推移削弱深入理解和解决问题的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://evidencebased.education/resource/cognitive-offloading-what-is-it-and-why-is-it-important-2/">Cognitive Offloading: What is it and why is it important?</a></li>
<li><a href="https://www.sciencedirect.com/science/article/abs/pii/S1364661316300985">Cognitive Offloading - ScienceDirect</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了不同观点：有人为 AI 使用辩护，认为它能增强潜力；另一些人则分享了技能退化的亲身经历，一位评论者描述了一位初级开发者无法解释 AI 生成的代码。还有人提出了一个反乌托邦的担忧：未来可能会强制要求外包思考，迫使人们遵从 AI 的意见。

**标签**: `#AI`, `#cognitive offloading`, `#software engineering`, `#critical thinking`, `#LLMs`

---

<a id="item-8"></a>
## [Linux 输入延迟测量：X11 对比 Wayland、VRR 与 DXVK](https://marco-nett.de/blog/measuring-input-latency-on-linux-x11-vs-wayland-vrr-dxvk/) ⭐️ 8.0/10

一项详细的实证研究测量了 Linux 显示服务器（X11 对比 Wayland）在可变刷新率（VRR）和 DXVK 转换层下的输入延迟，发现在特定条件下 Wayland 配合 VRR 可以优于 X11。 这为一个长期争论的话题提供了具体的数据驱动见解，帮助玩家和开发者选择 Linux 上更低输入延迟的配置。 测试使用了 500Hz 显示器，一些评论者指出这可能掩盖了较低刷新率下的问题；XWayland 路径显示出额外的 3ms 延迟，可能代表一整帧的延迟。

hackernews · hoechst · 7月14日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=48909424)

**背景**: X11 和 Wayland 是 Linux 的显示协议；Wayland 是更现代、更安全的替代方案。可变刷新率（VRR）使显示器刷新率与 GPU 帧输出同步，以最小延迟减少撕裂。DXVK 将 Direct3D 调用转换为 Vulkan，使得 Windows 游戏能通过 Wine/Proton 在 Linux 上运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.kde.org/2025/06/02/revisiting-x11-vs-wayland-with-multiple-displays/">Revisiting X11 vs Wayland With Multiple Displays - KDE Blogs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Variable_refresh_rate">Variable refresh rate - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/DXVK">DXVK</a></li>

</ul>
</details>

**社区讨论**: 评论者赞扬了实证方法，认为这种分析推动了生态系统的改进。一些人质疑 500Hz 显示器的代表性，建议使用 120Hz 或 60Hz 测试会揭示更大的帧缓冲效应。另有人推测，Wayland 的慢速感可能源于 XWayland 的额外延迟。

**标签**: `#linux`, `#input latency`, `#wayland`, `#x11`, `#vrr`

---

<a id="item-9"></a>
## [Armin Ronacher：共享语言与 AI 代理的冲击](https://simonwillison.net/2026/Jul/14/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher 发表了一篇博文，指出软件项目中的共享语言是通过摩擦来维持的，而 AI 代理可能会消除这种摩擦，从而损害团队的同步性。 这一见解挑战了消除开发中所有摩擦都有益的假设，指出 AI 代理可能会削弱团队协调所必需的共享理解。 Ronacher 区分了浪费性摩擦和有助于同步人们理解的生产性摩擦，并指出共享语言存在于对话、代码审查和争论中，而不是被完全写下来。

rss · Simon Willison · 7月14日 18:04

**背景**: Armin Ronacher 是知名软件开发者，Flask 和 Jinja2 的创建者。软件项目中的共享语言是指团队成员对系统概念、边界和所有权的隐式共同理解。摩擦，例如需要提问或协调，有助于传播这种理解。

**标签**: `#software engineering`, `#AI agents`, `#shared understanding`, `#team coordination`, `#knowledge management`

---

<a id="item-10"></a>
## [NVIDIA 分享 Kaggle 竞赛提升 AI 推理的教训](https://developer.nvidia.com/blog/lessons-from-the-leaderboard-what-5000-kagglers-taught-us-about-improving-ai-reasoning/) ⭐️ 8.0/10

NVIDIA 发布了一篇博客文章，总结了来自 Kaggle 上超过 5,000 名参与者在 NVIDIA Nemotron 模型推理挑战中学到的关键技术，旨在提高 AI 推理的准确性。 这些见解提供了经过社区验证的实用方法，用于增强大型语言模型的推理能力，这对于构建可靠的 AI 代理和推动开源 AI 发展至关重要。 该竞赛专注于提高 Nemotron 模型家族的推理准确性，博客详细介绍了来自顶级参赛作品中的策略，如数据增强、提示工程和集成技术。

rss · NVIDIA Developer Blog · 7月14日 18:20

**背景**: NVIDIA Nemotron 是一个开源 AI 模型系列，具有开放的权重、训练数据和配方，旨在构建具有强大推理能力的专业 AI 代理。Kaggle 竞赛邀请社区探索提高推理准确性的技术，利用大规模协作基准测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nemotron">Nemotron - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/topics/ai/nemotron">Nemotron AI Models | NVIDIA Developer</a></li>

</ul>
</details>

**标签**: `#AI reasoning`, `#Kaggle competition`, `#NVIDIA Nemotron`, `#model improvement`, `#machine learning`

---

<a id="item-11"></a>
## [CISA 敦促立即加固 SharePoint 以应对活跃利用](https://www.cisa.gov/news-events/alerts/2026/07/14/cisa-urges-sharepoint-hardening-after-new-exploitations) ⭐️ 8.0/10

CISA 发布警报，指出三个关键 SharePoint Server 漏洞（CVE-2026-32201、CVE-2026-45659 和 CVE-2026-56164）正被积极利用，攻击者可通过窃取 IIS 机器密钥和反序列化攻击实现远程代码执行和持久化。 该警报影响所有受支持的本地 SharePoint Server 版本（2016、2019 和 Subscription Edition），并强调组织应立即应用补丁、启用 AMSI 集成，并在确保没有残留后门后轮换机器密钥。 三个被利用的 CVE 涉及远程代码执行和反序列化，另外两个 CVE（CVE-2026-55040、CVE-2026-58644）尚未被利用但存在潜在风险。CISA 提供了具体的 AMSI 检测签名，并建议在 SharePoint Subscription Edition 上对请求正文扫描使用“完整模式”。

rss · CISA Cybersecurity Advisories · 7月14日 12:00

**背景**: 反序列化攻击发生在应用程序从不受信任的序列化输入重建对象而未经验证时，攻击者可注入恶意代码。IIS 机器密钥是用于 ASP.NET 视图状态和表单身份验证的加密密钥；一旦被窃取，攻击者可伪造身份验证令牌并实现持久化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://portswigger.net/web-security/deserialization">Insecure deserialization | Web Security Academy - PortSwigger</a></li>
<li><a href="https://cheatsheetseries.owasp.org/cheatsheets/Deserialization_Cheat_Sheet.html">Deserialization - OWASP Cheat Sheet Series</a></li>
<li><a href="https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/hh831711(v=ws.11)">Machine Key | Microsoft Learn</a></li>

</ul>
</details>

**标签**: `#security`, `#SharePoint`, `#CISA`, `#CVE`, `#RCE`

---

<a id="item-12"></a>
## [CISA 警告 Rockwell 1715-AENTR 适配器存在严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-195-04) ⭐️ 8.0/10

CISA 发布公告(ICSA-26-195-04)，警告 Rockwell Automation 1715-AENTR EtherNet/IP 适配器（版本≤3.003）存在缺失认证漏洞(CVE-2026-10577，CVSS 10)，允许未认证远程攻击者执行侵入性 CLI 命令。 该漏洞可导致设备完全受控，影响能源、水务等关键基础设施行业的机密性、完整性和可用性。由于该设备全球部署，被利用可能中断工业运营。 受影响产品暴露了一个无适当权限控制的网络可访问调试端口，可导致任意文件读写删除、任务停止、内存修改和 I/O 状态改变。Rockwell Automation 建议升级至 3.011 或更高版本。

rss · CISA Cybersecurity Advisories · 7月14日 12:00

**背景**: EtherNet/IP 是一种工业网络协议，它将通用工业协议(CIP)适配到标准以太网，广泛应用于工厂自动化。1715-AENTR 是 Rockwell 1715 冗余 I/O 系统的适配器，用于高可用性控制系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/EtherNet/IP">EtherNet/IP - Wikipedia</a></li>
<li><a href="https://www.rockwellautomation.com/en-us/products/details.1715-AENTR.html">Hardware Catalog | Rockwell Automation | US</a></li>

</ul>
</details>

**标签**: `#CISA`, `#ICS`, `#Rockwell Automation`, `#critical vulnerability`, `#EtherNet/IP`

---

<a id="item-13"></a>
## [SAP 修复 NetWeaver ABAP 严重漏洞，CVSS 9.9](https://thehackernews.com/2026/07/sap-patches-cvss-99-netweaver-abap-flaw.html) ⭐️ 8.0/10

SAP 发布了 2026 年 7 月安全更新，修复了 NetWeaver Application Server ABAP 中的一个 CVSS 9.9 分越界写入漏洞（CVE-2026-44747），该漏洞可能导致数据泄露或篡改。 此事至关重要，因为 SAP NetWeaver ABAP 是许多企业 SAP 系统的核心组件，高 CVSS 评分表明对数据机密性和完整性有严重影响。 该漏洞（CVE-2026-44747）是一个越界写入漏洞（CWE-787），需要身份验证，但可能导致内存损坏和数据泄露。SAP 建议立即应用补丁。

rss · The Hacker News · 7月14日 18:17

**背景**: SAP NetWeaver Application Server (AS) ABAP 是基于 ABAP 的 SAP 应用程序的运行时环境。越界写入发生在软件将数据写入超出分配内存缓冲区时，可能导致损坏或代码执行。这类漏洞在缺乏内存安全的语言（如 C/C++）中常见。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SAP_NetWeaver_Application_Server">SAP NetWeaver Application Server</a></li>
<li><a href="https://cwe.mitre.org/data/definitions/787.html">CWE - CWE-787: Out-of-bounds Write (4.20) - Mitre Corporation</a></li>

</ul>
</details>

**标签**: `#SAP`, `#NetWeaver ABAP`, `#CVE-2026-44747`, `#vulnerability`, `#security update`

---

<a id="item-14"></a>
## [RabbitMQ 漏洞可泄露 OAuth 密钥并暴露跨租户元数据](https://thehackernews.com/2026/07/rabbitmq-flaws-could-leak-oauth-secrets.html) ⭐️ 8.0/10

研究人员披露了流行开源消息代理 RabbitMQ 中的两个访问控制漏洞。这些漏洞可能允许攻击者泄露 OAuth 客户端密钥，并绕过租户边界访问不同租户的队列元数据。 由于 RabbitMQ 广泛用于企业环境中的异步消息传递，这些漏洞构成了重大的安全风险。成功利用可能导致对敏感消息的未授权访问，并危害受 OAuth 保护的服务。 第一个漏洞泄露了代理的机密 OAuth 客户端密钥，而第二个漏洞则允许跨租户访问队列元数据。这两个漏洞均由 Miggo 安全研究团队发现并已负责地披露。

rss · The Hacker News · 7月14日 13:48

**背景**: RabbitMQ 是一个开源消息代理，用于促进分布式系统组件之间的异步通信。OAuth 客户端密钥是应用程序用于向 OAuth 授权服务器进行身份验证的机密凭据。在多租户环境中，需要严格的隔离以防止一个租户访问另一个租户的数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Message_broker">Message broker</a></li>
<li><a href="https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/">The Client ID and Secret - OAuth 2.0 Simplified</a></li>

</ul>
</details>

**标签**: `#security`, `#RabbitMQ`, `#vulnerability`, `#OAuth`, `#message broker`

---

<a id="item-15"></a>
## [11 个微软签名的旧 UEFI Shim 可绕过 Secure Boot](https://thehackernews.com/2026/07/11-old-microsoft-signed-linux-uefi.html) ⭐️ 8.0/10

网络安全研究人员发现，11 个旧的、由微软签名的 UEFI shim 应用程序可被利用来绕过 Secure Boot，使攻击者能够在系统启动时部署恶意 bootkit。 该漏洞威胁到无数系统上 Secure Boot 的基础信任，可能使攻击者能够在固件级别植入持久且隐蔽的恶意软件，从而绕过传统安全措施。 这些有漏洞的 shim 之前由微软签名，并被各 Linux 发行版广泛使用；利用这些漏洞需要物理访问或管理员权限才能将 shim 加载到系统上。

rss · The Hacker News · 7月14日 12:46

**背景**: UEFI Secure Boot 是一种安全标准，通过验证数字签名确保只有受信任的软件在启动过程中运行。UEFI shim 是一种小型引导加载程序，通过充当信任链，帮助 Linux 系统在启用了 Secure Boot 的硬件上启动。Bootkit 是一种恶意软件，它在操作系统加载之前感染启动过程，因此难以检测和清除。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UEFI">UEFI - Wikipedia</a></li>
<li><a href="https://github.com/rhboot/shim">GitHub - rhboot/shim: UEFI shim loader · GitHub</a></li>
<li><a href="https://www.crowdstrike.com/en-us/cybersecurity-101/malware/bootkits/">What Is Bootkit? Prevention and Removal | CrowdStrike</a></li>

</ul>
</details>

**标签**: `#security`, `#UEFI`, `#Secure Boot`, `#vulnerability`, `#bootkit`

---

<a id="item-16"></a>
## [加密货币钱包扩展泄露地址，实现追踪](https://thehackernews.com/2026/07/study-of-85-crypto-wallet-extensions.html) ⭐️ 8.0/10

鲁汶大学的研究人员测试了 85 款流行的加密货币钱包浏览器扩展，发现它们会泄露足够的信息，从而关联用户的不同地址并实现跨站追踪。 这一隐私漏洞影响数百万加密货币用户，可能允许广告商、分析服务或恶意行为者跟踪他们的在线活动，并在不同网站间关联其金融身份。 泄露发生在钱包扩展与网站及区块链服务器通信的过程中，使得外部人员能够将一个人的多个地址关联起来，并在站点间追踪他们。

rss · The Hacker News · 7月14日 11:55

**背景**: 加密货币钱包浏览器扩展允许用户直接通过浏览器与去中心化应用（dApps）交互并签署交易。它们通常会向访问的每个网站暴露用户的公钥地址。该研究揭示，这种暴露结合区块链服务器的数据，创建了一个可用于未经用户同意的跨站追踪的指纹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/study-of-85-crypto-wallet-extensions.html">Study of 85 Crypto Wallet Extensions Finds Address Leaks and ...</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#cryptocurrency`, `#browser extensions`, `#blockchain`

---

<a id="item-17"></a>
## [OAuth 客户端 ID 欺骗可让攻击者验证被盗的 Entra 凭据](https://thehackernews.com/2026/07/oauth-client-id-spoofing-lets-attackers.html) ⭐️ 8.0/10

攻击者利用 OAuth 客户端 ID 欺骗技术验证被盗的 Microsoft Entra ID 凭据，且不产生任何成功登录事件，从而规避安全遥测的检测。 该技术使攻击者能够悄无声息地确认有效凭据并枚举用户账户，提高凭据攻击的有效性且对防御者不可见，对云安全构成严重威胁。 该攻击使用资源所有者密码凭据（ROPC）OAuth 流程，向/common/oauth2/token 端点发送带有伪造客户端 ID 的 POST 请求，日志中显示空白应用程序名称而非真实客户端。

rss · The Hacker News · 7月14日 11:21

**背景**: OAuth 是一种授权框架，允许应用程序获取对 HTTP 服务上用户账户的有限访问权限。ROPC 授权类型允许直接提交凭据，通常用于遗留或受信任的应用程序。伪造客户端 ID 会欺骗授权服务器在没有正确验证的情况下接受请求，使攻击者能够测试凭据而不触发成功登录事件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.proofpoint.com/us/blog/threat-insight/oauth-client-id-spoofing-why-fake-client-ids-are-gaining-traction-stealthy">OAuth Client ID Spoofing: Why Fake Client IDs Are Gaining ...</a></li>
<li><a href="https://thehackernews.com/2026/07/oauth-client-id-spoofing-lets-attackers.html">OAuth Client ID Spoofing Lets Attackers Validate Stolen ...</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/07/13/entra-id-oauth-client-id-spoofing/">Fake OAuth client IDs are helping attackers slip past sign-in ...</a></li>

</ul>
</details>

**标签**: `#OAuth`, `#spoofing`, `#Microsoft Entra ID`, `#cloud security`, `#attack technique`

---

<a id="item-18"></a>
## [苹果起诉 OpenAI；谷歌用 AI 摘要改造搜索](https://www.reddit.com/r/artificial/comments/1uwh06x/apple_just_sued_openai_for_trade_secret_theft_and/) ⭐️ 8.0/10

苹果于 7 月 10 日起诉 OpenAI，指控其窃取商业秘密，称 OpenAI 的首席硬件官指示求职者将物理组件带到面试中，且一名前苹果工程师在加入 OpenAI 后访问了苹果的网络存储。同日，谷歌用 Gemini 生成的 AI 摘要取代了传统搜索结果，导致点击率下降 58%。 这两件事从根本上改变了科技公司和数字企业的格局：诉讼可能影响 OpenAI 即将进行的 IPO，并为商业秘密保护树立法律先例；而谷歌转向 AI 驱动的搜索改变了数十亿用户发现在线内容的方式，影响全球网站的流量和收入。 诉状提到，OpenAI 的首席硬件官 Tang Tan（苹果 24 年资深员工）指示求职者将苹果组件带到面试中进行'展示和讲解'。此外，一名跳槽到 OpenAI 的前苹果工程师利用漏洞从苹果网络存储下载了未发布产品的文件。

reddit · r/artificial · /u/Dapper-Tale-4021 · 7月14日 18:27

**背景**: 商业秘密盗窃是指未经授权获取提供竞争优势的机密商业信息。苹果与 OpenAI 关系复杂，苹果最近宣布与 OpenAI 合作将 ChatGPT 集成到其设备中，但在人才挖角和知识产权方面仍存在紧张关系。与此同时，谷歌使用其 Gemini 模型转向 AI 生成的搜索摘要，标志着从几十年来主导网络搜索的传统'十个蓝色链接'格式的重大转变，影响了企业优化搜索可见性的方式。

**标签**: `#Apple`, `#OpenAI`, `#Google`, `#AI`, `#trade secrets`

---

<a id="item-19"></a>
## [AI 智能体生产部署：缺乏基础设施](https://www.reddit.com/r/artificial/comments/1uwg8kk/the_absolute_nightmare_of_putting_ai_agents_into/) ⭐️ 8.0/10

行业正从构建 AI 智能体原型转向应对部署挑战，因为缺乏版本控制、安全和回滚等标准基础设施。 没有可靠的部署基础设施，大多数企业 AI 智能体项目将停留在试点阶段，阻碍实际影响和投资回报。 关键痛点包括为智能体管理唯一身份、防止数据泄露，以及无法将传统 DevOps 实践应用于本质上不可预测的 AI 系统。

reddit · r/artificial · /u/Kitchen-Owl4274 · 7月14日 18:01

**背景**: AI 智能体是使用大型语言模型执行任务的自主系统。将其部署到生产环境需要类似于传统软件的基础设施，但增加了幻觉和安全隐患等复杂性。LangGraph 和 CrewAI 等框架有助于构建智能体，但缺乏稳健的部署工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.langchain.com/langgraph">LangGraph: Agent Orchestration Framework for Reliable AI Agents</a></li>
<li><a href="https://crewai.com/">CrewAI</a></li>
<li><a href="https://research.google/pubs/agentic-ai-infrastructure-in-practice-learn-these-key-hurdles-to-deploy-production-ai-agents-efficiently/">Agentic AI Infrastructure in Practice: Learn These Key Hurdles to Deploy Production AI Agents Efficiently</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#production deployment`, `#DevOps`, `#LLM infrastructure`, `#software engineering`

---

<a id="item-20"></a>
## [纽约州长暂停数据中心审批](https://www.reddit.com/r/artificial/comments/1uwmxob/hochul_halts_new_data_center_approvals_via/) ⭐️ 8.0/10

纽约州长凯西·霍楚签署行政命令，暂停新数据中心的审批，理由是能源和环境方面的担忧。 这一举措直接影响纽约州 AI 和云基础设施的发展，可能减缓技术扩张并增加开发商的成本。 暂停适用于大型数据中心的新许可证，而现有项目及小型设施可能豁免。该命令还要求对能源使用和环境影响进行审查。

reddit · r/artificial · /u/news-10 · 7月14日 22:07

**背景**: 数据中心是容纳云计算、AI 训练等数字业务所需计算和网络设备的场所。它们消耗大量电力，引发了对电网容量和碳排放的担忧。纽约一直是科技投资的热点，但州监管机构正日益关注此类项目的环境足迹。

**标签**: `#data centers`, `#regulation`, `#New York`, `#AI infrastructure`, `#energy policy`

---