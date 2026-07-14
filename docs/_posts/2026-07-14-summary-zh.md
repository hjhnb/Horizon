---
layout: default
title: "Horizon Summary: 2026-07-14 (ZH)"
date: 2026-07-14
lang: zh
---

> 从 55 条内容中筛选出 20 条重要资讯。

---

1. [NVIDIA Ising 解码将颜色代码逻辑错误率降低超过 300 倍](#item-1)
2. [OpenAI GPT-5.6 Sol、Terra、Luna 现已在 Amazon Bedrock 上可用](#item-2)
3. [CISA 警告俄罗斯路由器攻击威胁](#item-3)
4. [MemGhost 攻击通过电子邮件在 AI 智能体中植入虚假记忆](#item-4)
5. [苹果 SpeechAnalyzer API 基准测试：速度更快，精度略降](#item-5)
6. [世嘉 CD 游戏 Silpheed 的技术分析](#item-6)
7. [Telegram 的 t.me 域名因法律调查被暂停](#item-7)
8. [Samsung Health 威胁用户选择退出 AI 训练则删除数据](#item-8)
9. [Climate.gov 被毁，开放数据拯救了它](#item-9)
10. [对 15 款电子垃圾 GPU 进行现代 AI 工作负载基准测试](#item-10)
11. [CISA 公布 GitHub 凭证泄露事件教训](#item-11)
12. [NVIDIA 使用引导式生成模型估算极端事件概率](#item-12)
13. [两个 Joomla 扩展零日漏洞被加入 CISA 的 KEV 目录](#item-13)
14. [黑客在 Jscrambler npm 包中植入信息窃取恶意软件](#item-14)
15. [欧盟与英国制裁俄罗斯 GRU 黑客](#item-15)
16. [Trail of Bits 发布 Rust 安全测试指南](#item-16)
17. [检测到针对 MCP 服务器和 AI 凭证的主动扫描](#item-17)
18. [CrashStealer macOS 恶意软件通过公证的 dropper 绕过 Gatekeeper](#item-18)
19. [Google 和 Microsoft 因发现休眠数据收集器而下架 ModHeader 扩展](#item-19)
20. [Forg365 钓鱼服务平台针对 Microsoft 365 使用高级技术](#item-20)

---

<a id="item-1"></a>
## [NVIDIA Ising 解码将颜色代码逻辑错误率降低超过 300 倍](https://developer.nvidia.com/blog/nvidia-ising-decoding-cuts-color-code-logical-error-rates-by-over-300x/) ⭐️ 9.0/10

NVIDIA 推出了一种迭代 Ising 解码器，与以往方法相比，将颜色代码的逻辑错误率降低了 300 倍以上。这一突破在最近的 arXiv 论文中详细阐述，将量子纠错解码映射到经典哈密顿量优化问题。 逻辑错误率的显著降低使容错量子计算更接近现实，因为颜色代码是可扩展量子架构的主要候选方案。NVIDIA 的方法通过实现更高效的纠错，可能大大加速实用量子计算机的进展。 Ising 解码器利用迭代算法优化经典自旋哈密顿量，自然处理颜色代码中相关的 X 和 Z 错误。该技术在 NVIDIA GPU 上进行了演示，并在 GitHub 上开源了训练教程。

rss · NVIDIA Developer Blog · 7月13日 19:00

**背景**: 量子计算机极易受到噪声影响，需要量子纠错（QEC）码来检测和纠正错误。颜色代码是一种拓扑 QEC 码，具有单步逻辑操作等优势，但传统上逻辑错误率较高。Ising 解码方法将解码问题重新表述为经典 Ising 模型的基态搜索，从而能够在 GPU 上进行高效的并行计算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.12301">[2606.12301] An iterative Ising decoder for quantum error ...</a></li>
<li><a href="https://github.com/NVIDIA/Ising-Decoding">GitHub - NVIDIA/Ising-Decoding: A set of training recipes for ...</a></li>

</ul>
</details>

**标签**: `#quantum computing`, `#error correction`, `#NVIDIA`, `#quantum error correction`, `#decoding`

---

<a id="item-2"></a>
## [OpenAI GPT-5.6 Sol、Terra、Luna 现已在 Amazon Bedrock 上可用](https://aws.amazon.com/blogs/machine-learning/openai-gpt-5-6-sol-terra-and-luna-are-now-generally-available-on-amazon-bedrock/) ⭐️ 9.0/10

OpenAI 发布了其 GPT-5.6 模型系列——包括 Sol、Terra 和 Luna——现已在 Amazon Bedrock（AWS 的基础模型托管服务）上正式可用。这是这些模型首次通过亚马逊平台提供。 此次整合通过 AWS 安全且可扩展的基础设施，将 OpenAI 最先进的模型带给更广泛的用户，使企业能够以企业级安全性和可靠性部署前沿 AI。这加强了 OpenAI 与 AWS 的合作关系，可能加速生成式 AI 在商业应用中的普及。 GPT-5.6 包含三个能力层级：Sol（最高）、Terra（均衡）和 Luna（高效），每个层级具有不同的性能和成本特征。这些模型现已搭载在 Amazon Bedrock 的下一代推理引擎上，该引擎专为高性能、安全性和可靠性设计。

rss · AWS Machine Learning Blog · 7月13日 21:01

**背景**: Amazon Bedrock 是 AWS 提供的一项完全托管服务，通过单一 API 访问来自多个供应商的基础模型。OpenAI 的 GPT-5.6 于 2026 年 7 月发布，作为一个分层模型系列，接替了 GPT-5.5，其中 Sol、Terra 和 Luna 提供递增的能力级别，以适应不同的使用场景和预算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vellum.ai/blog/gpt-5-6-benchmarks-explained">GPT - 5 . 6 Sol vs Terra vs Luna : Which Tier Should You Actually Use?</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>

</ul>
</details>

**标签**: `#AI`, `#AWS`, `#GPT-5.6`, `#Amazon Bedrock`, `#OpenAI`

---

<a id="item-3"></a>
## [CISA 警告俄罗斯路由器攻击威胁](https://www.cisa.gov/news-events/cybersecurity-advisories/aa26-194a) ⭐️ 9.0/10

CISA 与 17 个国际合作伙伴联合发布警告，详细说明俄罗斯 FSB 第十六中心如何利用配置不当和有漏洞的路由器入侵关键基础设施网络，并提供了具体的攻击手法与防御措施。 该警告凸显了俄罗斯国家支持的网络行为者对基础网络设备的持续性高威胁，敦促立即采取措施保护路由器，防止关键行业遭受连锁式入侵。 该警告由 NSA、FBI、ASD's ACSC 等 18 家机构联合发布，基于长达十年的 Berserk Bear/Dragonfly 活动模式，强调默认凭据和未修补漏洞是主要攻击途径。

rss · CISA Cybersecurity Advisories · 7月13日 12:00

**背景**: 俄罗斯联邦安全局第十六中心是其信号情报部门，十多年来一直在全球范围内针对网络设备进行网络行动。本次警告补充了联邦调查局 2025 年发布的公共服务公告，为防御者提供了更详细的技术细节。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Federal_Security_Service">Federal Security Service - Wikipedia</a></li>
<li><a href="https://www.ic3.gov/PSA/2025/PSA250820">Internet Crime Complaint Center (IC3) | Russian Government Cyber Actors Targeting Networking Devices, Critical Infrastructure</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#russia`, `#router`, `#critical infrastructure`, `#CISA`

---

<a id="item-4"></a>
## [MemGhost 攻击通过电子邮件在 AI 智能体中植入虚假记忆](https://thehackernews.com/2026/07/new-memghost-attack-plants-persistent.html) ⭐️ 9.0/10

该攻击揭示了使用持久性记忆的 AI 智能体存在关键漏洞，可在用户不知情的情况下进行长期操控，威胁到 AI 助手在敏感领域的可信度。 MemGhost 植入虚假记忆，在智能体的记忆中隐藏更改，并影响未来响应，且对话中不留可见痕迹。该攻击利用了智能体无法区分合法用户指令与注入提示的缺陷。

rss · The Hacker News · 7月13日 13:49

**背景**: 具有持久性记忆的 AI 智能体会存储过去的交互记录以个性化未来响应。记忆投毒是一种攻击方式，将对抗性内容写入智能体的长期记忆，从而破坏其行为。提示注入利用模型无法区分开发者指令与用户输入的缺陷，允许隐藏命令。MemGhost 通过一封电子邮件结合了这些技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/new-memghost-attack-plants-persistent.html">New MemGhost Attack Plants Persistent False Memories in AI ...</a></li>
<li><a href="https://www.nowosci.ai/en/article/memghost-attack-plants-fake-ai-memories">Researchers Demonstrate MemGhost, an Attack That Plants Fake ...</a></li>
<li><a href="https://news.shield53.com/memghost-why-persistent-memory-in-ai-agents-creates-a-new-class-of-invisible-attack-surface/">MemGhost: Why Persistent Memory in AI Agents Creates a New ...</a></li>

</ul>
</details>

**标签**: `#AI security`, `#memory poisoning`, `#prompt injection`, `#vulnerability`, `#AI agents`

---

<a id="item-5"></a>
## [苹果 SpeechAnalyzer API 基准测试：速度更快，精度略降](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 8.0/10

苹果在 iOS 26 和 macOS 26 中推出的全新 SpeechAnalyzer API（取代 SFSpeechRecognizer）与 Whisper 模型及其前身进行了基准测试，结果显示速度大约快三倍，且在 LibriSpeech 上精度具有竞争力。 此基准测试意义重大，因为它首次提供了苹果设备端语音转文本 API 的独立性能对比，可能影响转录应用的未来以及注重隐私的语音处理。 该 API 在 LibriSpeech 的干净和嘈杂部分均击败了所有测试的 Whisper 模型（包括 Whisper Small），速度约为 Small 的三倍。但社区部分成员建议与 Nvidia 的 Nemotron 或 Parakeet 等新模型进行比较。

hackernews · get-inscribe · 7月13日 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48894752)

**背景**: 苹果的 SpeechAnalyzer 是在 iOS 26 和 macOS 26 中引入的新设备端语音转文本 API，取代了旧的 SFSpeechRecognizer。它注重隐私和速度。Whisper 是 OpenAI 的开源语音识别模型，广泛用于转录。该基准测试由第三方转录应用 Inscribe 团队进行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/videos/play/wwdc2025/277/">Bring advanced speech -to-text to your app with... - Apple Developer</a></li>
<li><a href="https://get-inscribe.com/blog/apple-speech-api-benchmark.html">Apple 's New Speech API vs Whisper: The First Real Benchmark</a></li>
<li><a href="https://asibiont.com/en/blog/apple-speechanalyzer-protiv-whisper-chto-izmenilos-v-mire-vibe-coding-v-2026-godu">Apple 's New SpeechAnalyzer API Benchmarked... — ASI Biont Blog</a></li>

</ul>
</details>

**社区讨论**: 评论指出，虽然该 API 更快，但部分用户仍会坚持使用 Whisper 以保证离线精度；也有人认为苹果的入局可能颠覆现有基于 Whisper 的付费应用。建议包括与 Nvidia 的 Nemotron 和 Parakeet 等新模型进行比较。

**标签**: `#Apple`, `#speech recognition`, `#benchmark`, `#Whisper`, `#API`

---

<a id="item-6"></a>
## [世嘉 CD 游戏 Silpheed 的技术分析](https://fabiensanglard.net/silpheed/index.html) ⭐️ 8.0/10

Fabien Sanglard 发布了一篇关于世嘉 CD 游戏 Silpheed 的详细技术分析，探讨了其独特的 FMV 渲染和声音硬件。 这项分析提供了宝贵的见解，展示了开发者如何在有限硬件上实现逼真的类 3D 视觉效果，为现代爱好者保留了复古游戏工程知识。 文章解释了 Silpheed 如何使用预渲染的全动态视频来模拟多边形图形，并讨论了世嘉 CD 通过 Mega Drive 扩展端口进行的音频混合。

hackernews · ibobev · 7月13日 14:52 · [社区讨论](https://news.ycombinator.com/item?id=48893639)

**背景**: 世嘉 CD 是 Mega Drive 的附加设备，支持基于光盘的游戏，具有增强的图形和音频。全动态视频（FMV）游戏使用预录的视频文件而非实时 3D 渲染。Silpheed 以其将 FMV 与游戏玩法无缝集成而闻名，营造出控制电影的感觉。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sega_CD">Sega CD - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Full-motion_video">Full-motion video - Wikipedia</a></li>
<li><a href="https://www.hardcoregaming101.net/silpheed/">Silpheed – Hardcore Gaming 101</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了文章的深度，有人回忆说 Silpheed 感觉像'在控制一部电影'。另一个人纠正了声音设置的描述，指出 Mega Drive I 的扩展端口会混合外部音频。还有用户警告了 YouTube 链接参数的隐私影响。

**标签**: `#retro gaming`, `#game development`, `#sega cd`, `#technical analysis`, `#engineering`

---

<a id="item-7"></a>
## [Telegram 的 t.me 域名因法律调查被暂停](https://www.whois.com/whois/t.me) ⭐️ 8.0/10

Telegram 的 t.me 域名已被暂停，WHOIS 记录显示其状态代码包含 clientRenewProhibited 和 serverDeleteProhibited，这些代码通常在法律纠纷或待删除期间启用。 此次暂停影响全球 Telegram 用户使用的所有 t.me 链接，凸显了依赖第三方域名的风险，同时也引发对 Telegram 选择以不透明著称的 GoDaddy 作为注册商的担忧。 域名状态代码包括 clientRenewProhibited、serverDeleteProhibited 等，ICANN 解释这些代码不常见，通常在法律纠纷期间启用。Telegram 创始人 Pavel Durov 尚未发布官方声明。

hackernews · Tiberium · 7月13日 19:52 · [社区讨论](https://news.ycombinator.com/item?id=48897878)

**背景**: 域名状态代码（也称 EPP 状态代码）由注册局和注册商用来指示域名的状态。客户状态代码由注册商设置，服务器状态代码由注册局设置。像 clientRenewProhibited 这样的代码会阻止续费，很少出现，通常由法律纠纷或待删除引起。ICANN 负责协调全球域名系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.icann.org/resources/pages/epp-status-codes-2014-06-16-en">EPP Status Codes | What Do They Mean, and Why Should I Know? - ICANN</a></li>
<li><a href="https://en.wikipedia.org/wiki/ICANN">ICANN</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：一位用户对使用重定向系统感到庆幸，另一位则指出 Durov 尚未发布公告。有用户详细分析了 ICANN 状态代码，强调其在法律纠纷中的罕见使用。一些人对 Telegram 依赖以不透明著称的 GoDaddy 表示惊讶。

**标签**: `#domain suspension`, `#Telegram`, `#ICANN`, `#legal investigation`, `#DNS`

---

<a id="item-8"></a>
## [Samsung Health 威胁用户选择退出 AI 训练则删除数据](https://neow.in/cWsyMTV3) ⭐️ 8.0/10

三星宣布，在 Samsung Health 应用中，用户如果选择退出 AI 训练，其所有健康数据（包括睡眠、用药、医疗记录和周期追踪详情）将被完全删除。 该政策引发了严重的隐私和数据所有权担忧，迫使用户在丢失个人健康数据或同意将其用于 AI 训练之间做选择。这为大型科技公司在 AI 背景下处理用户数据同意问题树立了一个先例。 涉及的数据类别包括睡眠、用药、医疗记录和周期追踪。选择退出的用户在数据删除后将无法恢复，且该政策似乎适用于现有和未来的数据。

hackernews · bundie · 7月13日 20:01 · [社区讨论](https://news.ycombinator.com/item?id=48897991)

**背景**: Samsung Health 是三星 Galaxy 设备预装的一款流行的健康和健身追踪应用。该公司计划利用用户健康数据训练其 AI 模型，这一做法引发了关于同意和数据隐私的争论。与一些允许用户选择退出但仍保留数据的服务不同，三星的做法更为激进。

**社区讨论**: 评论者表达了愤怒和不信任，称该政策对用户不友好，并将其与 Google 在 AI 训练方面的做法相比较。一些人讽刺地指出，删除可能有助于移除不想要的数据，而另一些人则批评 Samsung Health 现有的问题，如广告和糟糕的数据导出功能。

**标签**: `#privacy`, `#AI training`, `#health data`, `#Samsung`, `#data ethics`

---

<a id="item-9"></a>
## [Climate.gov 被毁，开放数据拯救了它](https://werd.io/climate-gov-was-destroyed-open-data-saved-it/) ⭐️ 8.0/10

美国政府的 Climate.gov 网站被摧毁或下线，但开放数据倡议和社区主导的救援工作通过分布式存档保存了公共数据。 这一事件凸显了政府托管的数据在政治或行政变动面前的脆弱性，并强调了开放数据和分布式存档在确保公共资助信息长期可获取方面的关键作用。 正如社区评论所指出的，这次救援依赖捐赠和志愿者努力，引发了对税收之外数据保存可持续资金的质疑。

hackernews · benwerd · 7月13日 19:57 · [社区讨论](https://news.ycombinator.com/item?id=48897945)

**背景**: 政府数据，如气候记录，通常发布在官方网站上，这些网站可能因政策变化或预算削减而关闭。开放数据倡议主张使这些数据自由可用且易于恢复。像 Data Rescue Project 这样的项目和 IPFS 这样的分布式存储系统有助于将数据存档并分布在多个节点上，降低丢失风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datarescueproject.org/">Data Rescue Project</a></li>
<li><a href="https://www.mlanet.org/article/accessing-public-data-removed-from-us-government-websites/">Accessing Public Data Removed from US Government Websites - MLA</a></li>

</ul>
</details>

**社区讨论**: 评论者对数据救援表示感谢，但质疑长期可持续性，指出维持当前的监测和分析需要大量资源。一些人主张默认将政府数据置于公共领域，并建议使用 IPFS 发布静态内容以防止未来损失。

**标签**: `#open data`, `#government data`, `#data preservation`, `#climate data`, `#public domain`

---

<a id="item-10"></a>
## [对 15 款电子垃圾 GPU 进行现代 AI 工作负载基准测试](https://esologic.com/benchmarking-tesla-gpus/) ⭐️ 8.0/10

一篇文章对 15 款老旧 GPU（包括 Tesla K80 和 P40）进行了现代 AI 推理任务基准测试，使用 llama.cpp，结果表明某些电子垃圾 GPU 仍能为 LLM 部署提供高性价比性能。 这很重要，因为它帮助爱好者和小型团队找到运行本地大语言模型的廉价硬件，降低了 AI 实验和自建部署的门槛。 基准测试涵盖了 Llama 3.1 8B 和 Qwen 2.5 7B 等模型的 token 生成速度和内存带宽，其中 Tesla P100 和 P40 展现了出人意料的高性价比表现。

hackernews · eso_logic · 7月13日 13:48 · [社区讨论](https://news.ycombinator.com/item?id=48892638)

**背景**: 电子垃圾 GPU 是指不再受现代驱动支持或已从数据中心退役的老旧显卡。像 llama.cpp 这样的工具可以通过将计算卸载到 GPU，使得即使在中低端硬件上也能运行 LLM 推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://esologic.com/benchmarking-tesla-gpus/">Benchmarking Tesla GPUs - esologic</a></li>
<li><a href="https://www.cmunroe.us/blog/23-tesla-p4-ollama-stack">Two Tesla P4s, an Old Dell, and a Local LLM Stack | #!/bin/coding</a></li>
<li><a href="https://www.hivenet.com/post/best-7-gpus-for-llm-inference-and-fine-tuning">Best GPUs for LLM inference and fine-tuning in 2026 | Hivenet</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Tesla P4 因低功耗和 8GB 显存而成为隐藏的宝石，并讨论了使用多 GPU 构建更大显存池的方法。一些人就老款 Nvidia Tesla 卡与较新的 AMD Radeon Pro 卡在 LLM 推理上的取舍展开了辩论。

**标签**: `#GPU benchmarking`, `#AI inference`, `#e-waste hardware`, `#LLM deployment`, `#machine learning`

---

<a id="item-11"></a>
## [CISA 公布 GitHub 凭证泄露事件教训](https://krebsonsecurity.com/2026/07/lessons-learned-from-cisas-recent-github-leak/) ⭐️ 8.0/10

CISA 发布了一份事后分析报告，详细说明了一名承包商在公共 GitHub 仓库中泄露内部凭证（包括 AWS GovCloud 密钥）近六个月后才被通知的情况。 这一事件凸显了事件响应和凭证管理中的关键漏洞，影响了所有安全团队，尤其是那些处理政府云环境的团队。 泄露内容包括数十个 CISA 内部凭证，例如 AWS GovCloud 密钥，并在 KrebsOnSecurity 通知该机构之前暴露了近半年。

rss · Krebs on Security · 7月13日 15:03

**背景**: AWS GovCloud 是为美国政府机构设计的专用云环境，旨在满足法规和合规要求。GitHub 是一个广泛使用的版本控制和代码托管平台，敏感数据泄露是常见的安全问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aws.amazon.com/govcloud-us/">AWS GovCloud (US) - Amazon Web Services</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#data leak`, `#CISA`, `#GitHub`, `#incident response`

---

<a id="item-12"></a>
## [NVIDIA 使用引导式生成模型估算极端事件概率](https://developer.nvidia.com/blog/extreme-event-likelihoods-with-guided-generative-models/) ⭐️ 8.0/10

NVIDIA 提出了一种新方法，利用引导式生成模型高效估算罕见、高影响事件的概率，相比传统蒙特卡洛采样大幅降低了计算成本。 该方法可显著改善气候科学、结构工程、金融等领域中的风险评估，这些领域对极端事件概率的估算至关重要但计算成本高昂。 引导式生成模型融动物理约束或目标导向，将采样集中在极端事件上，避免了暴力蒙特卡洛方法的低效。

rss · NVIDIA Developer Blog · 7月13日 15:00

**背景**: 极端事件概率估算传统上依赖极值理论或暴力蒙特卡洛仿真。蒙特卡洛方法需要大量模型运行，当每次运行涉及昂贵的物理仿真时成本过高。引导式生成模型提供了一种智能采样输入空间的方法，聚焦于产生极端输出的区域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/extreme-event-likelihoods-with-guided-generative-models/">Extreme Event Likelihoods with Guided Generative Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/Extreme_value_theory">Extreme value theory - Wikipedia</a></li>

</ul>
</details>

**标签**: `#generative models`, `#extreme events`, `#risk estimation`, `#machine learning`, `#NVIDIA`

---

<a id="item-13"></a>
## [两个 Joomla 扩展零日漏洞被加入 CISA 的 KEV 目录](https://thehackernews.com/2026/07/icagenda-and-balbooa-forms-joomla-flaws.html) ⭐️ 8.0/10

美国 CISA 已将 iCagenda 和 Balbooa Forms 这两个 Joomla 扩展中的两个最高严重性漏洞（CVSS 10.0）添加到其已知被利用漏洞目录中，此前有报告称这些漏洞已被作为零日漏洞在野外积极利用。 这些零日漏洞允许通过任意文件上传实现远程代码执行，对使用这些扩展的 Joomla 网站构成严重风险，而它们被纳入 CISA 的 KEV 目录意味着修补工作具有高优先级。 这两个漏洞在 CVSS 评分系统中均被评为 10.0 分，且正在被积极利用；CVE-2026-48939 影响 iCagenda，而 Balbooa Forms 的漏洞尚未分配 CVE 标识符。

rss · The Hacker News · 7月13日 05:36

**背景**: Joomla 是一个流行的开源内容管理系统（CMS），可以通过第三方扩展来增强功能，例如 iCagenda（用于活动管理）和 Balbooa Forms（表单构建器）。零日漏洞是指在供应商发布修复程序之前就被利用的漏洞。CISA 的已知被利用漏洞（KEV）目录是一个已确认在野外被利用的漏洞列表，组织利用它来优先进行修补。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisa.gov/known-exploited-vulnerabilities-catalog">Known Exploited Vulnerabilities Catalog | CISA</a></li>
<li><a href="https://extensions.joomla.org/extension/forms/">Forms, by Balbooa.com - Joomla Extension Directory</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#Joomla`, `#zero-day`, `#CISA`, `#vulnerabilities`

---

<a id="item-14"></a>
## [黑客在 Jscrambler npm 包中植入信息窃取恶意软件](https://www.bleepingcomputer.com/news/security/hackers-backdoor-jscrambler-npm-package-with-infostealer-malware/) ⭐️ 8.0/10

黑客发布了 Jscrambler 的 npm 包恶意版本，下载量近 1500 次，其中包含旨在窃取敏感信息的信息窃取恶意软件。 这次针对安全公司 npm 包的供应链攻击凸显了 JavaScript 生态系统中持续存在的风险，可能危及依赖 Jscrambler 进行客户端安全性的项目。 恶意包在 npm 上可用，下载量近 1500 次；目前尚不清楚它活跃了多久以及目标是什么具体数据。

rss · BleepingComputer · 7月13日 19:44

**背景**: Jscrambler 提供客户端安全解决方案，包括代码完整性和防篡改。信息窃取恶意软件是一种秘密从受感染系统收集凭证、财务数据和个人信息的恶意软件。针对 npm 等包注册表的供应链攻击已成为分发恶意软件的常见途径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.npmjs.com/package/jscrambler?activeTab=explore">jscrambler - npm</a></li>
<li><a href="https://en.wikipedia.org/wiki/Infostealer">Infostealer - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#npm`, `#supply chain attack`, `#malware`

---

<a id="item-15"></a>
## [欧盟与英国制裁俄罗斯 GRU 黑客](https://www.bleepingcomputer.com/news/security/eu-and-uk-hit-russia-with-first-joint-cyber-sanctions-package/) ⭐️ 8.0/10

欧盟和英国联合对与俄罗斯 GRU 有关的多个个人和实体实施制裁，指控他们策划了针对欧洲的网络攻击。 这标志着欧盟和英国首次联合实施网络制裁，表明西方对国家级网络威胁的统一回应，并可能威慑未来的攻击。 制裁针对数十名被指控协调黑客网络、对欧洲发动攻击的个人和实体，但本报告未披露具体名单。

rss · BleepingComputer · 7月13日 11:19

**背景**: GRU 是俄罗斯军事情报机构，曾与多起网络攻击有关，包括干预选举和破坏关键基础设施。这些制裁是追究国家支持黑客责任、保护欧洲网络安全的更广泛努力的一部分。

**标签**: `#cybersecurity`, `#sanctions`, `#Russia`, `#GRU`, `#hacking`

---

<a id="item-16"></a>
## [Trail of Bits 发布 Rust 安全测试指南](https://blog.trailofbits.com/2026/07/13/rust-proof-your-code-with-our-new-testing-handbook-chapter/) ⭐️ 8.0/10

Trail of Bits 在其测试手册中新增了一个关于 Rust 程序安全测试的章节，详细介绍了内部使用的工具和技术。 该资源为开发者和安全专业人员提供了可操作的指导，帮助识别和缓解 Rust 代码中的漏洞，满足了系统编程中对安全性日益增长的需求。 该章节涵盖了静态分析、模糊测试等技术，依托于 Trail of Bits 在审计 Rust 应用方面的丰富经验。

rss · Trail of Bits Blog · 7月13日 11:00

**背景**: Rust 是一种以内存安全著称的系统编程语言，但逻辑错误或不安全代码仍可能导致安全问题。Trail of Bits 是一家领先的安全公司，进行安全审计并发布开源工具以促进安全开发。

**标签**: `#Rust`, `#security testing`, `#static analysis`, `#fuzzing`, `#software engineering`

---

<a id="item-17"></a>
## [检测到针对 MCP 服务器和 AI 凭证的主动扫描](https://isc.sans.edu/diary/rss/33150) ⭐️ 8.0/10

安全研究人员观察到针对模型上下文协议（MCP）服务器和 AI 助手凭证的网络侦察活动显著增加，表明恶意行为者正在积极扫描这些资产。 此威胁直接影响使用集成 MCP 的 AI 编程助手的开发者和组织，因为凭证泄露可能导致数据泄露或供应链攻击。随着 2025 年 MCP 的快速采用，攻击面也在扩大。 扫描目标针对暴露文件访问、数据库查询和代码管理等能力的 MCP 服务器。攻击者可能利用配置错误的服务器或弱认证来窃取凭证或执行未授权操作。

rss · SANS Internet Storm Center · 7月13日 04:22

**背景**: 模型上下文协议（MCP）是由 Anthropic 于 2024 年 11 月推出的开放标准，规范了 AI 助手连接外部工具和数据源的方式。到 2025 年，Claude Code、GitHub Copilot 和 Cursor 等主要 AI 编程助手均已集成 MCP，使其成为 AI 开发工作流中的关键组件。这种广泛采用创造了新的攻击向量，恶意行为者目前正在积极探测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/docs/learn/server-concepts">Understanding MCP servers - Model Context Protocol</a></li>
<li><a href="https://iplogger.org/blog/someone-is-scanning-for-your-mcp-servers-and-ai-assistant-credentials-mon-jul-13th/">Urgent Threat Alert: Malicious Actors Actively Scanning for ...</a></li>

</ul>
</details>

**标签**: `#security`, `#AI`, `#MCP`, `#credentials`, `#scanning`

---

<a id="item-18"></a>
## [CrashStealer macOS 恶意软件通过公证的 dropper 绕过 Gatekeeper](https://thehackernews.com/2026/07/crashstealer-macos-malware-uses.html) ⭐️ 7.0/10

研究人员发现了一种名为 CrashStealer 的 macOS 信息窃取恶意软件，它使用经过签名和苹果公证的 dropper 来通过 Gatekeeper 检查。该恶意软件用原生 C++实现，并伪装成苹果的崩溃报告工具。 该恶意软件绕过了 macOS 核心安全功能 Gatekeeper，表明被公证的应用仍可能包含恶意内容。这凸显了在公证之外需要额外的安全层，因为攻击者滥用了苹果的信任机制。 该 dropper 以名为'Werkbit.app'的公证磁盘映像分发，开发者 ID 为'Emil Grigorov (WWB7JA7AQV)'。CrashStealer 在本地验证受害者的登录密码后，才会窃取凭据、钥匙串数据和加密货币钱包。

rss · The Hacker News · 7月13日 17:36

**背景**: Gatekeeper 是 macOS 的一项安全功能，它在运行前验证下载的应用，强制要求代码签名和公证。公证是指苹果扫描应用中的恶意内容。然而，此案例表明，如果恶意负载隐藏在后续阶段，被公证的应用仍可能包含恶意软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/crashstealer-macos-malware-uses.html">CrashStealer macOS Malware Uses Notarized Dropper to Pass Gatekeeper Checks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gatekeeper_(macOS)">Gatekeeper (macOS)</a></li>
<li><a href="https://appleinsider.com/articles/25/12/23/malware-bypassed-macos-gatekeeper-by-abusing-apples-notarization-proccess">Malware bypassed macOS Gatekeeper by abusing Apple's notarization proccess</a></li>

</ul>
</details>

**标签**: `#macOS`, `#malware`, `#cybersecurity`, `#Gatekeeper`, `#info-stealer`

---

<a id="item-19"></a>
## [Google 和 Microsoft 因发现休眠数据收集器而下架 ModHeader 扩展](https://thehackernews.com/2026/07/google-and-microsoft-pull-modheader.html) ⭐️ 7.0/10

Google 和 Microsoft 从其应用商店下架了 ModHeader 浏览器扩展，原因是安全研究人员在其官方版本中发现了一个隐藏的浏览历史收集器，但该收集器处于休眠状态，尚未确认任何数据泄露。 此事件凸显了针对浏览器扩展的供应链攻击风险日益增长，一个拥有 160 万安装量的流行扩展可能被利用来窃取敏感浏览数据，凸显了加强扩展审核和监控的必要性。 这个休眠收集器包含一个空白的允许列表，使其保持非活跃状态，因此实际上从未收集或传输任何浏览域名；然而，官方商店版本中存在此类代码表明该扩展的开发或更新流程可能已被攻破。

rss · The Hacker News · 7月13日 17:17

**背景**: 浏览器扩展是修改和增强浏览器功能的小型软件程序，但如果被攻破，它们也可能带来安全风险。近期的供应链攻击表明，恶意代码可以通过扩展的更新机制注入到合法的扩展中，在用户不知情的情况下影响数百万用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/new-supply-chain-attack-targeting-chrome-extensions/">New Supply Chain Attack Targeting Chrome Extensions To Inject ...</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/chrome-extensions-with-1-million-installs-hijack-targets-browsers/">Chrome extensions with 1 million installs hijack targets’ browsers</a></li>

</ul>
</details>

**标签**: `#security`, `#browser extension`, `#privacy`, `#supply chain attack`

---

<a id="item-20"></a>
## [Forg365 钓鱼服务平台针对 Microsoft 365 使用高级技术](https://thehackernews.com/2026/07/forg365-phaas-targets-microsoft-365.html) ⭐️ 7.0/10

一个名为 Forg365 的新型钓鱼服务平台出现，通过结合设备代码钓鱼、中间人攻击（AitM）、AI 辅助诱饵创建以及入侵后的邮箱操作，针对 Microsoft 365 账户。 Forg365 代表了钓鱼服务平台的一次复杂演进，整合了多种高级绕过技术，能够击败多因素认证（MFA）并逃避检测，对使用 Microsoft 365 的组织构成重大威胁。 Forg365 通过 Telegram 分发，月费 400 美元或年费 3800 美元，利用设备代码钓鱼（利用合法的 Microsoft 认证流程）和 AitM 代理，在 MFA 完成后窃取会话 Cookie。

rss · The Hacker News · 7月13日 13:03

**背景**: 设备代码钓鱼利用 Microsoft 为无浏览器设备设计的合法认证流程，诱骗用户输入代码，从而让攻击者获取会话。中间人攻击（AitM）将攻击者置于用户与服务之间的代理位置，即使在 MFA 完成后也能截获认证令牌和会话 Cookie。钓鱼服务平台（PhaaS）如 Forg365 通过提供现成的基础设施和工具，以订阅费用降低了攻击者的门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huntress.com/blog/device-code-phishing-ai-mfa-bypass">How EvilTokens Turbocharges Old School Phishing with AI | Huntress</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/threat-intelligence/what-is-an-adversary-in-the-middle-aitm-attack/">What is an AitM (Adversary-in-the-Middle) Attack? - SentinelOne</a></li>
<li><a href="https://attack.mitre.org/techniques/T1557/">Adversary-in-the-Middle, Technique T1557 - Enterprise | MITRE ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#phishing`, `#Microsoft 365`, `#PhaaS`

---