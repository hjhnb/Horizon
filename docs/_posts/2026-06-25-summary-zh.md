---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> 从 70 条内容中筛选出 20 条重要资讯。

---

1. [OpenAI 发布首款自研 AI 推理芯片 'Jalapeño'](#item-1)
2. [思考奖励模型量化大模型推理质量](#item-2)
3. [恶意软件使用违禁文本逃避 AI 检测](#item-3)
4. [Amadey 与 StealC 恶意软件网络被摧毁，2700 万凭据被追回](#item-4)
5. [Cordyceps CI/CD 漏洞威胁 300 多个 GitHub 仓库](#item-5)
6. [CISA 警告 Ubiquiti 和 Lantronix 设备漏洞正被利用](#item-6)
7. [Gefen 优化器声称比 AdamW 节省 8 倍内存](#item-7)
8. [高通以 40 亿美元收购 AI 初创公司 Modular](#item-8)
9. [GitHub 上的 PR 垃圾信息如同 2000 年代初的邮件垃圾信息](#item-9)
10. [NVIDIA 的 45°C 冷却方案将数据中心用水降至接近零](#item-10)
11. [卡马克后悔对 id Software 施压过大](#item-11)
12. [Nub：通过预加载钩子为 Node.js 带来类似 Bun 的工具集](#item-12)
13. [Rust 的 crates.io 发布仍依赖 GitHub](#item-13)
14. [CISA 警告 Lantronix EDS5000 关键漏洞正被利用](#item-14)
15. [顶级智能代理对手出现](#item-15)
16. [思科统一 CM 漏洞 PoC 发布后遭利用](#item-16)
17. [Mandiant 披露思科 SD-WAN 零日漏洞获取 root 权限细节](#item-17)
18. [Edge 扩展滥用原生消息传递实现恶意软件投递](#item-18)
19. [隐蔽后门 Mistic 与勒索软件访问代理 KongTuke 关联](#item-19)
20. [Linux 进程名称伪装技术](#item-20)

---

<a id="item-1"></a>
## [OpenAI 发布首款自研 AI 推理芯片 'Jalapeño'](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI 发布了首款自研 AI 推理芯片 'Jalapeño'，该芯片与 Broadcom 合作开发，并由 TSMC 制造。该芯片旨在优化大型语言模型的运行性能和成本效率。 这标志着 OpenAI 从完全依赖第三方硬件转向控制自己的芯片供应，可能降低成本和减少对 NVIDIA GPU 的依赖。这也表明 AI 公司向定制芯片发展的趋势，以在推理效率上获得竞争优势。 Jalapeño 专为推理工作负载设计，采用针对 Transformer 模型优化的定制架构。该芯片从设计到生产耗时九个月，OpenAI 利用自身模型加速了部分设计流程。

hackernews · jamdesk · 6月24日 17:47 · [社区讨论](https://news.ycombinator.com/item?id=48663324)

**背景**: AI 推理是运行已训练的 AI 模型以生成输出的过程，与训练相对。传统上，OpenAI 等公司使用 NVIDIA 的通用 GPU 进行训练和推理，但随着推理需求增长，定制芯片可提供更好的性价比。OpenAI 此举效仿了 Google（TPU）、Amazon（Trainium）等其他公司的垂直整合硬件策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>
<li><a href="https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/">OpenAI unveils its first custom chip, built by Broadcom</a></li>
<li><a href="https://uvation.com/articles/ai-inference-chips-latest-rankings-who-leads-the-race">AI Inference Chips 2025: Rankings & Leaders - uvation.com</a></li>

</ul>
</details>

**社区讨论**: 评论者对 OpenAI 声称其模型帮助设计了芯片表示怀疑，有人认为这可能是营销噱头。讨论中还涉及了权重在硅中的架构，以及与 Google TPU 和 Taalas 的全硅模型等其他定制芯片的比较。

**标签**: `#OpenAI`, `#AI hardware`, `#custom chip`, `#Broadcom`, `#inference`

---

<a id="item-2"></a>
## [思考奖励模型量化大模型推理质量](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247899199&idx=3&sn=b0d6764e50d881295fd85b75f8f9434a) ⭐️ 9.0/10

来自上海人工智能实验室、上海交通大学和香港中文大学的研究人员提出了思考奖励模型（TRM），这是一个量化大型语言模型推理质量的框架，已被接收为 ICML '26 Oral 论文，并在 GitHub 上开源，收获超过 4.2k 星标。 这解决了评估大模型是否真正理解推理过程，还是仅仅为了得到正确答案的问题，从而能够更好地对齐和训练模型。它提供了一种奖励高质量推理链的方法，可以改进模型训练和测试时的缩放。 TRM 引入了 ME²原则（最大化熵与效率），并使用有向无环图（DAG）来抽象复杂推理结构。该模型可用于测试时的缩放和强化学习，以提升推理质量。

rss · 量子位 · 6月24日 04:00

**背景**: 像 GPT-4 这样的大型语言模型（LLM）可以生成逐步推理（思维链），但除了最终答案的正确性外，评估推理过程的质量具有挑战性。传统的奖励模型关注结果正确性，而非推理过程。TRM 借鉴了思维链生成式奖励模型、token 级别的自我奖励估计以及学会思考的框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/thinking-supervised-reward-model-trm">Thinking -supervised Reward Model ( TRM )</a></li>
<li><a href="https://eu.36kr.com/en/p/3866659734279170">TRM Thinking Reward Model Launched: Large Models ' Reasoning...</a></li>
<li><a href="https://www.aitntnews.com/newDetail.html?newId=26520">TRM 思考奖励模型上线，大模型推理质量终于能量化了 | ICML‘26 Oral</a></li>

</ul>
</details>

**标签**: `#large language models`, `#reward model`, `#reasoning quality`, `#ICML`, `#open source`

---

<a id="item-3"></a>
## [恶意软件使用违禁文本逃避 AI 检测](https://www.schneier.com/blog/archives/2026/06/embedding-forbidden-text-in-spyware-to-discourage-ai-analysis-2.html) ⭐️ 9.0/10

恶意软件开发者开始在间谍软件代码中嵌入包含核武器和生物武器文本的 JavaScript 注释，旨在触发 AI 分析工具的安全过滤器，导致它们拒绝分析或误将恶意软件归类为良性。 这种新型规避技术利用了用于代码分析的大语言模型的安全机制，可能破坏自动化恶意软件检测管线，迫使安全团队做出调整。这标志着对抗性 AI 军备竞赛的重大升级。 违禁文本放在 JavaScript 块注释内，不影响执行但可被 AI 扫描器看到。实际恶意代码使用 try{eval(...)}包裹字符代码数组和 ROT 式替换密码进行混淆。

rss · Schneier on Security · 6月24日 11:03

**背景**: 基于 AI 的恶意软件分析工具日益依赖大语言模型来解读代码片段并标记可疑内容。这些模型通常具有安全过滤器，拒绝处理与大规模杀伤性武器等有害主题相关的内容。通过在注释中嵌入此类触发短语，攻击者可使 AI 跳过或错误分类文件。这是一种对抗性规避攻击形式，类似于提示注入，但目标是分析管道而非最终用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.checkpoint.com/artificial-intelligence/ai-evasion-the-next-frontier-of-malware-techniques/">AI Evasion: The Next Frontier of Malware Techniques</a></li>
<li><a href="https://arxiv.org/abs/2604.21310">[2604.21310] Adversarial Evasion in Non-Stationary Malware ... ADVERSARIAL MACHINE LEARNING IN EVASION ATTACKS ... Adversarial Binaries: AI-guided Instrumentation Methods for ... Adversarial Machine Learning in Cybersecurity: Defending ... NIST Identifies Types of Cyberattacks That Manipulate ... AI Evasion: The Next Frontier of Malware Techniques New Malware Embeds Prompt Injection to Evade AI Detection ...</a></li>
<li><a href="https://www.dcode.fr/rot-cipher">ROT Cipher - Rotation - Online Rot Decoder, Solver, Translator</a></li>

</ul>
</details>

**标签**: `#malware`, `#AI security`, `#adversarial evasion`, `#spyware`, `#JavaScript`

---

<a id="item-4"></a>
## [Amadey 与 StealC 恶意软件网络被摧毁，2700 万凭据被追回](https://thehackernews.com/2026/06/amadey-and-stealc-malware-network.html) ⭐️ 9.0/10

此次行动摧毁了网络犯罪分子用于发动勒索软件、金融欺诈和关键基础设施攻击的“装配线”，对网络犯罪生态系统产生了重大影响，并保护潜在受害者免遭凭据盗窃。 Amadey 恶意软件作为一种恶意软件即服务运作，而 StealC 则是一款针对浏览器数据和加密货币钱包的窃密木马。此次行动由欧洲刑警组织宣布，并涉及私营部门的威胁情报共享。

rss · The Hacker News · 6月24日 15:59

**背景**: Amadey 是一款多功能的模块化信息窃取程序，针对 Windows 系统，常被用作加载器来传播其他恶意软件。StealC 是一款用 C 语言编写的信息窃取恶意软件，从浏览器和应用程序中收集凭据、Cookie 和加密货币钱包数据。这两种恶意软件均被广泛用于网络犯罪活动，其基础设施被摧毁是对凭据盗窃行动的沉重打击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/amadey-and-stealc-malware-network.html">Amadey and StealC Malware Network Disrupted, 27M Stolen ...</a></li>
<li><a href="https://malpedia.caad.fkie.fraunhofer.de/details/win.stealc">Stealc (Malware Family)</a></li>
<li><a href="https://any.run/malware-trends/amadey/">Amadey Infostealer Malware Analysis, Overview by ANY.RUN</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#law enforcement`, `#credential theft`, `#infrastructure takedown`

---

<a id="item-5"></a>
## [Cordyceps CI/CD 漏洞威胁 300 多个 GitHub 仓库](https://thehackernews.com/2026/06/cordyceps-cicd-flaws-expose-300-github.html) ⭐️ 9.0/10

Novee Security 的研究人员发现了一个名为 Cordyceps 的关键 CI/CD 工作流弱点，攻击者可利用它劫持工作流，危及包括微软、谷歌和阿帕奇在内的 300 多个 GitHub 仓库。 该漏洞代表了一类新的供应链攻击，攻击者可完全控制代码仓库，可能导致开源生态系统中广泛的恶意软件分发和凭据窃取。 Cordyceps 漏洞影响超过 300 个仓库，可实现代码执行和凭据窃取。研究人员尚未确认任何真实世界利用，但该模式具有关键性和广泛性。

rss · The Hacker News · 6月24日 12:48

**背景**: CI/CD（持续集成/持续部署）工作流自动执行软件的构建、测试和部署。GitHub Actions 是一个流行的 CI/CD 平台，开发者可以在 YAML 文件中定义工作流。Cordyceps 漏洞利用了工作流与外部服务之间的信任关系，允许攻击者注入恶意步骤。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/cordyceps-cicd-flaws-expose-300-github.html">Cordyceps CI/CD Flaws Expose 300+ GitHub Repositories to ...</a></li>
<li><a href="https://cybersecuritynews.com/cordyceps-supply-chain-flaw-impacting-code-repositories/">Cordyceps Supply Chain Flaw Impacting Code Repositories at ...</a></li>

</ul>
</details>

**标签**: `#security`, `#CI/CD`, `#supply-chain attack`, `#GitHub`, `#open-source`

---

<a id="item-6"></a>
## [CISA 警告 Ubiquiti 和 Lantronix 设备漏洞正被利用](https://www.bleepingcomputer.com/news/security/cisa-warns-of-max-severity-ubiquiti-flaws-exploited-in-attacks/) ⭐️ 9.0/10

美国网络安全和基础设施安全局（CISA）发出警告，攻击者正在积极利用 Ubiquiti UniFi OS 和 Lantronix 串口转以太网服务器中的最高严重性漏洞，敦促立即修补。 这些漏洞影响广泛使用的网络和工业设备，可能让远程攻击者控制受影响设备，导致数据泄露或网络被攻陷。 这些漏洞被评定为最高严重性（CVSS 10.0），并且已在野外被积极利用。使用 Ubiquiti UniFi OS 控制器和 Lantronix 设备服务器的用户应立即应用可用更新。

rss · BleepingComputer · 6月24日 14:35

**背景**: Ubiquiti UniFi OS 是 Ubiquiti 网络硬件（包括路由器和接入点）的操作系统。Lantronix 串口转以太网服务器允许传统串行设备连接到 IP 网络。这些系统在企业和工业环境中很常见，使其成为攻击者的诱人目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ui.com/">UniFi - Rethinking IT - Ubiquiti</a></li>
<li><a href="https://www.lantronix.com/lantronix-products/network-infrastructure/serial-to-ethernet-device-servers/">Lantronix Serial-to-Ethernet Device Servers | Industrial ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CISA`, `#Ubiquiti`, `#exploit`

---

<a id="item-7"></a>
## [Gefen 优化器声称比 AdamW 节省 8 倍内存](https://www.reddit.com/r/LocalLLaMA/comments/1uep96s/gefen_is_a_dropin_replacement_for_the_adamw/) ⭐️ 9.0/10

Gefen 是 AdamW 优化器的即插即用替代方案，声称能将训练内存使用量降低 8 倍。相关论文和 GitHub 仓库已发布。 这种内存节省可使现有硬件支持更大模型或更大批次训练，显著提升训练效率和可及性。 Gefen 通过跨参数块共享二阶矩估计，并使用学习到的码本量化一阶矩来实现内存节省。它被设计为直接替代方案，无需修改模型架构。

reddit · r/LocalLLaMA · /u/indicava · 6月24日 20:39

**背景**: AdamW 是深度学习中广泛使用的优化器，但它维护的一阶和二阶动量缓冲区各占用与模型参数同等大小的内存，实际使内存使用翻倍。Gefen 的方法压缩这些动量缓冲区，大幅减少训练时的内存占用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pypi.org/project/gefen/">Gefen optimizer for memory-efficient PyTorch training</a></li>
<li><a href="https://arxiv.org/abs/2606.13894">[2606.13894] Gefen : Optimized Stochastic Optimizer</a></li>
<li><a href="https://nefut.com/article/996-csai-gefen-optimized-stochastic-optimizer-with-8x-memory-reduction">[CS.AI] Gefen : Optimized Stochastic Optimizer with 8x Mem... - Nefut</a></li>

</ul>
</details>

**标签**: `#optimizer`, `#memory reduction`, `#deep learning`, `#AdamW`, `#training efficiency`

---

<a id="item-8"></a>
## [高通以 40 亿美元收购 AI 初创公司 Modular](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 8.0/10

2026 年 6 月 24 日，高通宣布以 40 亿美元收购 AI 基础设施初创公司 Modular，旨在提升其在硬件和软件方面的 AI 能力。 此次收购标志着 AI 行业的一次重大整合，高通试图通过将 Modular 的统一计算层和 Mojo 编程语言整合到其产品组合中，挑战英伟达在 AI 推理和训练领域的主导地位。 Modular 的核心技术包括一个能让 AI 模型无需修改代码即可在不同芯片上运行的平台，以及 Mojo 语言——它结合了 Python 的易用性和系统级性能。这笔 40 亿美元的交易预计将于今年晚些时候完成。

hackernews · timmyd · 6月24日 13:49 · [社区讨论](https://news.ycombinator.com/item?id=48659798)

**背景**: Modular 由前苹果和谷歌工程师于 2022 年创立，开发了旨在统一跨硬件 AI 开发的编程语言 Mojo。高通以移动芯片（骁龙）闻名，近年来正积极拓展 AI 和数据中心市场。此次收购符合高通构建从边缘到云端完整 AI 生态系统的战略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://startups.in/united-states/modular">Modular - Valuation, Funding, Competitors & News | startups .in</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo ( programming language ) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人质疑高通在高端 AI 推理/训练领域缺乏存在感，而另一些人则认为这是高通包括 RISC-V 和其他 AI 投资在内的大胆组合战略的一部分。还有人指出其中的讽刺意味，因为 Modular 的创始人此前曾批评硬件公司的 AI 软件栈。

**标签**: `#acquisition`, `#AI`, `#Qualcomm`, `#Modular`, `#Mojo`

---

<a id="item-9"></a>
## [GitHub 上的 PR 垃圾信息如同 2000 年代初的邮件垃圾信息](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 8.0/10

Greptile 博客上的一篇文章将 GitHub 上最近激增的垃圾拉取请求与 2000 年代初的邮件垃圾信息泛滥相提并论，揭示了开源维护者日益严重的困扰。 这种比较突出了一个可能阻碍开源协作的系统性问题，因为维护者浪费时间去审查低质量的 PR。社区讨论中提出的潜在解决方案可能会影响 GitHub 和项目未来如何对抗垃圾信息。 GitHub 最近推出了可配置的 PR 限制，以在一定程度上帮助维护者解决问题；一些项目现在要求新贡献者在合并第一个 PR 之前以非文本形式与维护者会面。作者指出，PR 垃圾信息与早期的邮件垃圾信息一样，利用低成本、低努力的外联来获取关注或奖励。

hackernews · dakshgupta · 6月24日 14:32 · [社区讨论](https://news.ycombinator.com/item?id=48660579)

**背景**: 拉取请求（PR）垃圾信息是指在 GitHub 上创建的自动化或低质量 PR，通常作为教程或营销活动的一部分，向仓库涌入无意义的贡献。这已成为开源维护者的重大负担，他们必须手动审查并拒绝这些 PR。2000 年代初的邮件垃圾信息时代出现了类似模式，导致了复杂过滤系统的发展。理解这段历史可能为 GitHub 提供更好的反垃圾信息措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/animesh-chouhan/github-spamstop">animesh-chouhan/ github -spamstop: Prevent PR and Issue spam on ...</a></li>
<li><a href="https://www.kushcreates.com/blogs/inside-the-open-source-prs-massacre-of-github">Inside The Open Source Softwares (OSS) PRs Massacre of GitHub</a></li>
<li><a href="https://mansoorbarri.medium.com/how-can-github-fix-spamming-14e9bab59294">How Can GitHub Fix Spamming ?. Background | by Mansoor... | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者强调 GitHub 的新 PR 限制是有帮助的一步，但指出邮件垃圾信息的缓解依赖于服务器级别的发送者声誉，这不直接适用于 GitHub 个人用户。其他人分享了实用解决方案，例如要求新贡献者进行非文本会面，或者允许维护者接收代币积分以分配资源对抗垃圾信息。

**标签**: `#PR spam`, `#open source`, `#spam prevention`, `#GitHub`, `#maintainer tools`

---

<a id="item-10"></a>
## [NVIDIA 的 45°C 冷却方案将数据中心用水降至接近零](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA 宣布了一种用于 AI 数据中心的新型液冷架构，其冷却液温度高达 45°C（113°F），大幅降低了用水量，并为与区域供暖系统集成提供了可能。 这项创新解决了 AI 数据中心日益严重的水和能源可持续性问题（这些中心冷却需要消耗大量水）。通过将用水量降至接近零并促进废热再利用，它为行业树立了新的效率标杆。 冷却液由 75%的水和 25%的丙二醇混合而成，温度高于典型热水浴缸（100–104°F）。该系统采用芯片直接液冷和室外干冷器，在一年中大部分时间无需蒸发水即可散热。

hackernews · nitin_flanker · 6月24日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48660178)

**背景**: 传统数据中心，尤其是采用空气冷却的数据中心，通过蒸发冷却消耗大量水。液冷通常能减少用水，但典型系统需要冷却液温度远低于环境温度，从而限制了效率。通过将冷却液温度提高到 45°C，NVIDIA 的设计可以在更长时间内通过干冷器将热量散到空气中，几乎完全消除耗水，并使得废热可用于区域供暖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/">Hotter Than a Hot Tub: The 45°C Breakthrough to Cool AI’s Biggest Machines | NVIDIA Blog</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/data-centers/nvidia-announces-liquid-cooling-system-that-runs-hotter-than-a-hot-tub-promises-to-reduce-electricity-consumption-and-cut-water-use-by-up-to-100-percent-but-sustainability-challenges-remain">Nvidia announces liquid cooling system that runs ‘hotter than a hot tub’ — promises to reduce electricity consumption and cut water use by up to 100%, but sustainability challenges remain | Tom's Hardware</a></li>
<li><a href="https://www.districtenergy.org/topics/datacenters">Data Centers & District Energy - International District ...</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了与区域供暖协同的潜力，指出 45°C 对于供暖环路是可用的，并可能为社区带来数百万美元的价值。一些人质疑与现有液冷数据中心相比真正的创新点是什么，而另一些人则提出了气候依赖性问题——询问“有利气候”对效率意味着什么。还有人提到了 NASA Ames 超级计算设施，该设施也使用高温水冷。

**标签**: `#data center cooling`, `#water conservation`, `#liquid cooling`, `#NVIDIA`, `#sustainability`

---

<a id="item-11"></a>
## [卡马克后悔对 id Software 施压过大](https://twitter.com/ID_AA_Carmack/status/2069799283369345247) ⭐️ 8.0/10

id Software 联合创始人约翰·卡马克反思早期错误，称自己对团队施压过大，导致员工疲惫并缩短了公司的寿命。 这位传奇程序员的反思为游戏开发和创业文化提供了宝贵教训，凸显了实现突破与维持公司健康之间的张力。 卡马克特别提到，在《雷神之锤》开发期间的高强度冲刺虽然造就了一款标志性游戏，但可能“掏空了”id Software 并耗尽了团队精力。

hackernews · shadowtree · 6月24日 15:56 · [社区讨论](https://news.ycombinator.com/item?id=48661825)

**背景**: id Software 以开创第一人称射击游戏而闻名，代表作包括《德军总部 3D》《毁灭战士》和《雷神之锤》。约翰·卡马克因其在 3D 图形方面的技术创新而备受赞誉。该公司以高强度工作文化著称，尤其在 1990 年代初期。

**社区讨论**: 评论者普遍赞同卡马克的自我批评，部分人指出高强度工作导致创意人员流失及后续作品质量下降。另一些人则认为，为了《雷神之锤》这样标志性的游戏，这些牺牲是值得的。

**标签**: `#game development`, `#startup culture`, `#John Carmack`, `#company management`, `#software engineering`

---

<a id="item-12"></a>
## [Nub：通过预加载钩子为 Node.js 带来类似 Bun 的工具集](https://github.com/nubjs/nub) ⭐️ 8.0/10

Zod 的创建者、前 Bun 工程师 Colin McDonnell 发布了 Nub——一个通过--require 预加载钩子为 Node.js 添加类 Bun 功能的工具包（基于 oxc 的转译器、Worker/Temporal 的 polyfill 以及高级模块解析），而无需替换 Node.js 本身。 Nub 通过将现代便利性引入 Node 生态，弥合了 Node.js 与 Bun 之间的开发者体验差距，使团队无需切换运行时即可采用 TypeScript、高级 API 和快速模块解析。 转译器使用 oxc——一个高性能的基于 Rust 的 JavaScript/TypeScript 转换器，打包为 Node-API 插件。Polyfill 包括 Temporal API 和 Worker，所有添加都是纯粹的附加功能——你的代码仍然在原生 Node 的引擎和标准库上运行。

hackernews · colinmcd · 6月24日 14:14 · [社区讨论](https://news.ycombinator.com/item?id=48660267)

**背景**: Node.js 有一个--require 预加载机制，可以在主应用之前运行脚本，以及 module.registerHooks 用于自定义模块解析。Bun 是一个竞争性运行时，默认提供 TypeScript 转译、内置打包和现代 API。Nub 利用这些 Node.js 钩子来复制 Bun 的开发者体验，而无需分支 Node 本身。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance JavaScript tools.</a></li>
<li><a href="https://nodejs.org/api/modules.html">Modules: CommonJS modules | Node.js v26.3.1 Documentation</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Temporal">Temporal - JavaScript | MDN - MDN Web Docs</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极，用户报告了无缝迁移（例如，整个 monorepo 迁移无问题）。一些人注意到'nub'这个名字的幽默（听起来像'n00b'），而技术讨论集中在选择--require 而非--import 以及对 ESM 支持的影响上。

**标签**: `#nodejs`, `#toolkit`, `#developer-experience`, `#transpiler`, `#bun`

---

<a id="item-13"></a>
## [Rust 的 crates.io 发布仍依赖 GitHub](https://infosec.exchange/@mttaggart/116806641273303255) ⭐️ 8.0/10

Rust 社区正在积极讨论 crates.io 对 GitHub 的持续依赖问题，最近合并的 RFC（RFC 3963）旨在将两者解耦。 这种依赖为 Rust 供应链制造了单点故障；解耦将增强安全性和韧性。 合并了 RFC 3963 以推动解耦，实现工作已经开始，但进展依赖于志愿者贡献和资金支持。

hackernews · speckx · 6月24日 19:40 · [社区讨论](https://news.ycombinator.com/item?id=48664733)

**背景**: crates.io 是 Rust 的官方包注册中心，Cargo 是包管理器。目前，发布 crate 需要与 GitHub 交互以更新索引和进行身份验证，从而形成依赖。Rust 项目承认此问题并制定了消除 GitHub 依赖的路线图，但需要大量工作和资金。

**社区讨论**: 社区评论普遍同意依赖是一个问题，但指出由于志愿者驱动的开发，修复起来很困难。一些人强调了供应链风险，并与 PHP 的 Packagist 等其他生态系统进行了比较。其他人指出了官方问题和 RFC 进展，欢迎贡献。

**标签**: `#rust`, `#crates.io`, `#supply-chain security`, `#github dependency`, `#cargo`

---

<a id="item-14"></a>
## [CISA 警告 Lantronix EDS5000 关键漏洞正被利用](https://thehackernews.com/2026/06/cisa-warns-critical-lantronix-eds5000.html) ⭐️ 8.0/10

CISA 已将 Lantronix EDS5000 系列设备中的关键代码注入漏洞 CVE-2025-67038 列入已知被利用漏洞目录，并要求 FCEB 机构在 2026 年 6 月 26 日前完成修复。 该漏洞（CVSS 9.8）允许未经身份验证的远程攻击者在受影响的 EDS5000 设备上以 root 权限执行任意命令，而这类设备广泛用于安全系统、医疗设备和 POS 终端等关键基础设施。 该漏洞源于登录失败时用户名参数未经正确清理，导致命令注入。CISA 的约束性操作指令（BOD 25-01）要求联邦机构在 2026 年 6 月 26 日前完成修复。

rss · The Hacker News · 6月24日 17:19

**背景**: Lantronix EDS5000 系列是机架式设备服务器，用于将串行设备（如安全摄像头、医疗监护仪）连接到以太网。代码注入漏洞发生在用户输入被不当处理并由系统执行时，使攻击者能够运行任意命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lantronix.com/products/eds5000-series/">EDS5000 Series | Serial-to-Ethernet | Lantronix</a></li>
<li><a href="https://cvemon.intruder.io/cves/CVE-2025-67038">CVE-2025-67038 - Overview, Insights & Trends</a></li>
<li><a href="https://vulnerability.circl.lu/vuln/CVE-2025-67038">CVE-2025-67038 - Vulnerability-Lookup</a></li>

</ul>
</details>

**标签**: `#vulnerability`, `#CISA`, `#Lantronix`, `#CVE-2025-67038`, `#security`

---

<a id="item-15"></a>
## [顶级智能代理对手出现](https://thehackernews.com/2026/06/dawn-of-apex-agentic-adversary.html) ⭐️ 8.0/10

一篇新文章警告，AI 驱动的“智能代理对手”能在数秒内发现、武器化并利用漏洞，远超人类防御者的响应速度。 这标志着人类速度威胁时代的终结，过去攻击滞留时间曾给防御者数天或数周的反应时间。组织现在必须采用 AI 速度的防御，否则可能被压垮。 文章将“顶级智能代理对手”描述为一种自主 AI 系统，以机器速度行动，将攻击滞留时间从数天压缩到几乎为零。基于补丁周期和手动响应的传统安全模型正变得过时。

rss · The Hacker News · 6月24日 11:30

**背景**: 智能代理 AI 是指能够追求目标、使用工具并以不同程度自主采取行动的 AI 系统。在网络安全中，“攻击滞留时间”是指攻击者在网络中未被发现的时间。历史上，防御者以天或周计算滞留时间，并依赖这个窗口进行检测和响应。智能代理对手的出现消除了这个窗口，因为 AI 可以在人类反应之前扫描、利用并提升权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agentic_AI">Agentic AI</a></li>
<li><a href="https://www.runzero.com/blog/apex-agentic-adversary/">Dawn of the apex agentic adversary - runZero</a></li>
<li><a href="https://www.packetlabs.net/posts/what-is-attack-dwell-time/">What Is Attack Dwell Time? - Packetlabs</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#artificial intelligence`, `#threats`, `#agentic AI`

---

<a id="item-16"></a>
## [思科统一 CM 漏洞 PoC 发布后遭利用](https://thehackernews.com/2026/06/cisco-unified-cm-flaw-exploited-after.html) ⭐️ 8.0/10

威胁攻击者正在积极利用 CVE-2026-20230，这是思科统一 CM WebDialer 服务中的一个关键 SSRF 漏洞，在概念验证代码公开后遭到利用。 该漏洞允许未经身份验证的远程攻击者进行服务器端请求伪造，可能危及思科统一通信环境，而这些环境对企业语音和视频通信至关重要。 该漏洞的 CVSS 评分为 8.6，可以在无需身份验证的情况下远程利用。概念验证展示了一条文件写入路径，可能导致攻击者获得受影响系统的 root 权限。

rss · The Hacker News · 6月24日 06:50

**背景**: 思科统一通信管理器（CUCM）是一个用于语音、视频和协作服务的本地呼叫控制平台。服务器端请求伪造（SSRF）是一种允许攻击者从服务器向内部资源发送精心构造的请求的漏洞。该特定漏洞位于 CUCM 的 WebDialer 组件中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Cisco_Unified_Communications_Manager">Cisco Unified Communications Manager</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/cisco-unified-cm-sme-flaw-cve-2026-20230-now-exploited-in-attacks/">Cisco Unified CM flaw CVE-2026-20230 now exploited in attacks</a></li>
<li><a href="https://cvereports.com/reports/CVE-2026-20230">CVE-2026-20230: CVE-2026-20230: Server-Side Request Forgery ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#cisco`, `#exploitation`, `#unified-communications`

---

<a id="item-17"></a>
## [Mandiant 披露思科 SD-WAN 零日漏洞获取 root 权限细节](https://www.bleepingcomputer.com/news/security/mandiant-reveals-how-cisco-sd-wan-zero-day-attacks-gained-root-access/) ⭐️ 8.0/10

Mandiant 公开披露了攻击者如何利用 Cisco Catalyst SD-WAN 中的零日漏洞（CVE-2026-20245）在受影响设备上获取 root 权限。 此次披露为企业网络防御者提供了关键情报，因为 SD-WAN 部署广泛，该漏洞可能导致设备完全被攻陷。 该漏洞允许攻击者在目标设备上创建恶意 root 账户，且无需认证。Mandiant 的分析显示，攻击链涉及构造特制的畸形数据包。

rss · BleepingComputer · 6月24日 21:29

**背景**: SD-WAN（软件定义广域网）是一种通过将网络硬件与其控制机制分离来简化 WAN 管理和运营的技术。Cisco Catalyst SD-WAN 是一种流行的企业解决方案，可实现分布位置之间的安全连接。零日漏洞是指在被利用时供应商尚不知晓的缺陷。root 权限代表 Unix/Linux 系统上的最高权限级别，允许完全控制设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisco.com/site/us/en/learn/topics/networking/what-is-sd-wan.html">What Is SD-WAN? - Software-Defined WAN (SDWAN) - Cisco</a></li>
<li><a href="https://www.cisco.com/site/us/en/solutions/networking/sdwan/catalyst/index.html">Cisco Catalyst SD-WAN (Software-Defined WAN) - Cisco</a></li>

</ul>
</details>

**标签**: `#security`, `#zero-day`, `#Cisco`, `#SD-WAN`, `#vulnerability`

---

<a id="item-18"></a>
## [Edge 扩展滥用原生消息传递实现恶意软件投递](https://www.bleepingcomputer.com/news/security/malicious-edge-extension-abuses-native-messaging-as-bridge-to-malware/) ⭐️ 8.0/10

一个名为‘Edgecution’的恶意 Microsoft Edge 扩展在勒索软件攻击中，通过原生消息传递 API 逃逸浏览器沙箱，并部署了一个基于 Python 的后门。 这种新颖的攻击向量绕过了 Edge 的沙箱保护，使得勒索软件可以直接从浏览器部署。它突显了在广泛使用扩展的企业环境中存在的关键安全风险。 该扩展滥用了本用于扩展与本地应用之间合法通信的原生消息传递 API，以执行任意 Python 脚本。这使得攻击者能够在浏览器的受限环境之外运行恶意软件。

rss · BleepingComputer · 6月24日 20:58

**背景**: 浏览器扩展被沙箱化以防止直接访问操作系统。然而，原生消息传递 API 允许扩展与安装在用户计算机上的本地应用程序通信，提供了一个桥梁，如果未妥善保护则可能被利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/concepts/native-messaging">Native messaging | Chrome for Developers</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging">Native messaging - Mozilla - MDN Web Docs</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#Microsoft Edge`, `#Native Messaging`, `#ransomware`

---

<a id="item-19"></a>
## [隐蔽后门 Mistic 与勒索软件访问代理 KongTuke 关联](https://www.bleepingcomputer.com/news/security/stealthy-mistic-backdoor-linked-to-ransomware-access-broker-kongtuke/) ⭐️ 7.0/10

一种名为 Mistic 的新型后门，与勒索软件访问代理 KongTuke（又称 Woodgnat）有关，自 2025 年 4 月以来一直针对保险、教育、IT 和专业服务领域的组织。 该后门为包括 Qilin、Akira 和 Black Basta 在内的多个勒索软件家族提供初始访问权限，对企业网络构成严重威胁，并凸显了访问代理不断演变的策略。 Mistic 支持文件上传/下载、文件操作和命令计划调整，被认为是 KongTuke 使用的另一工具 ModeloRAT 的后续版本或变体。

rss · BleepingComputer · 6月24日 10:41

**背景**: 像 KongTuke 这样的初始访问代理专门入侵企业网络并将其访问权限出售给勒索软件团伙。Mistic 等后门允许持久远程控制，从而窃取数据并随后部署勒索软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/stealthy-mistic-backdoor-linked-to-ransomware-access-broker-kongtuke/">Stealthy Mistic backdoor linked to ransomware access broker ...</a></li>
<li><a href="https://www.security.com/threat-intelligence/new-mistic-backdoor-modelorat">Backdoor.Mistic: New Backdoor May be Linked to Ransomware ...</a></li>
<li><a href="https://www.securityweek.com/new-mistic-rat-opens-door-to-several-ransomware-families/">New ' Mistic ' RAT Opens Door to Several Ransomware... - SecurityWeek</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#backdoor`, `#ransomware`, `#threat intelligence`

---

<a id="item-20"></a>
## [Linux 进程名称伪装技术](https://isc.sans.edu/diary/rss/33102) ⭐️ 7.0/10

SANS ISC 的日记探讨了 Linux 进程名称伪装技术，恶意软件通过修改 argv[0]或/proc/self/comm 来改变显示的进程名，从而逃避检测。 该技术被列为 MITRE ATT&CK T1036，被高级持续性威胁组织（如 Velvet Ant）使用，削弱了对基本进程监控工具的信任，使恶意软件检测更加困难。 在 Linux 上，进程名称伪装可通过 prctl(PR_SET_NAME)系统调用或直接写入/proc/self/comm 实现，使恶意进程能够伪装成如'[kworker/0:1]'的内核线程。

rss · SANS Internet Storm Center · 6月24日 06:29

**背景**: 进程名称伪装是一种防御规避技术，恶意软件通过伪装进程名使其看起来合法。在 Linux 上，进程名存储在 comm 字段中，可在运行时通过 prctl 等系统调用更改。该技术属于 MITRE ATT&CK 框架中更广泛的伪装战术（T1036）的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://attack.mitre.org/techniques/T1036/005/">Masquerading : Match Legitimate Resource Name ... | MITRE ATT&CK</a></li>
<li><a href="https://github.com/gotr00t0day/Linux-Malware-Evasion-Techniques">GitHub - gotr00t0day/ Linux -Malware-Evasion- Techniques : Linux ...</a></li>

</ul>
</details>

**标签**: `#linux`, `#malware obfuscation`, `#cybersecurity`, `#process masquerading`

---