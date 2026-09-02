---
layout: default
title: "Horizon Summary: 2026-09-02 (ZH)"
date: 2026-09-02
lang: zh
---

> 从 86 条内容中筛选出 20 条重要资讯。

---

1. [Anthropic 发布 Claude Fable 5.1 与 Mythos 5.1 并大幅降低缓存读取价格](#item-1)
2. [1.5 小时训练的小型 Transformer 在 ARC 上超越众多 LLM](#item-2)
3. [OpenAI 的 Astra 首个达到关键网络能力阈值](#item-3)
4. [FBI 调查暗网出售 1.53 亿张驾照事件](#item-4)
5. [攻击者利用 Langflow 与 Rails 严重漏洞窃取凭证并开展 C2 活动](#item-5)
6. [丹·卢评估艾德·齐特龙 AI 怀疑论预测的准确性](#item-6)
7. [Google Play 要求 AnkiDroid 移除 Open Collective 捐赠链接](#item-7)
8. [Codex 桌面应用捆绑了 LibreOffice、Python 和 Node.js](#item-8)
9. [新工具让 48GB Mac 运行 104GB Qwen3.8-Flash-Next，速度约 12 tok/s](#item-9)
10. [Atlas：World Labs 发布可生成 3D 场景的空间智能世界模型](#item-10)
11. [Python 3.15.0 候选版本 2 发布，十月正式版前的最后阶段](#item-11)
12. [CISA 警示罗克韦尔 Historian ME 存在可远程执行代码的漏洞](#item-12)
13. [攻击者利用 JFrog Artifactory 严重漏洞铸造管理员令牌](#item-13)
14. [恶意 Packagist 包通过 iOS 间谍软件窃取加密货币钱包种子](#item-14)
15. [攻击者窃取 METR API 密钥，消耗 60 万美元 AI 额度](#item-15)
16. [Aesto Health 数据泄露影响超过 950 万名患者](#item-16)
17. [黑客劫持 BGP 推送恶意 Virtualizor 更新](#item-17)
18. [近 22,000 台 Exchange 服务器面临邮箱劫持漏洞风险](#item-18)
19. [CISA 警告罗克韦尔 RSLinx Classic 存在拒绝服务漏洞](#item-19)
20. [CISA 警告罗克韦尔自动化 PLC 存在拒绝服务漏洞](#item-20)

---

<a id="item-1"></a>
## [Anthropic 发布 Claude Fable 5.1 与 Mythos 5.1 并大幅降低缓存读取价格](https://www.anthropic.com/claude-fable-and-mythos-5-1) ⭐️ 9.0/10

Anthropic 发布了 Claude Fable 5.1 和 Claude Mythos 5.1，改进了写作风格并提升了科学表现。此次发布还将缓存读取价格从每百万 token 1 美元大幅降至 0.25 美元。 这次发布意义重大，因为它同时带来了能力提升和大幅降价，可能压低 LLM API 整体定价的上限。依赖重复上下文的开发者和企业将最受益，而更强的科学能力也可能扩大 Claude 在科研和技术领域的应用。 缓存读取价格从每百万 token 1 美元降至 0.25 美元，意味着 Fable 5.1 的缓存读取成本仅为 Claude Opus（0.5 美元/百万 token）的一半。三个破坏性变更疑似修复了意外泄露思维链（chain-of-thought）的问题，例如通过伪造的“think_deeply”工具可能让模型输出原始思考内容。

hackernews · denysvitali · 9月1日 17:53 · [社区讨论](https://news.ycombinator.com/item?id=49525378)

**背景**: 提示缓存（prompt caching）是 LLM API 的一项技术，它保存提示词中经常重复使用的部分（如系统指令和上下文），这样每次调用时无需重新处理，从而降低成本和延迟。系统卡（system card）是 AI 实验室推行的一种透明度文档，说明模型的预期用途、局限、风险、评估和红队测试结果。理解这些概念有助于解释为何缓存读取降价对高频 API 用户至关重要，以及为何 Anthropic 在发布模型时同时公布了系统卡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@med.el.harchaoui/what-is-prompt-caching-reduce-llm-cost-by-90-ba1e129cda42">What is Prompt Caching : Reduce LLM cost by 90 | Medium</a></li>
<li><a href="https://futureagi.com/glossary/prompt-caching/">What Is Prompt Caching ? Definition & FutureAGI Guide (2026)</a></li>
<li><a href="https://geratools.com/ai-system-card-generator">AI System Card Generator — Gera Tools</a></li>

</ul>
</details>

**社区讨论**: 一位 Anthropic 员工表示 Fable 5.1 在写作风格上改进明显，不再那么像“典型 Claude”。Simon Willison 测试了推理努力级别，发现 xhigh 表现不错，但 max 生成一幅“鹈鹕”图花了近 14 分钟；另一位评论者指出，除了 Terminal-Bench-Science 外，基准提升并不明显；还有评论认为这些破坏性变更很可能是在修复思维链泄露问题。

**标签**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#Model Release`

---

<a id="item-2"></a>
## [1.5 小时训练的小型 Transformer 在 ARC 上超越众多 LLM](https://mvakde.github.io/blog/44-on-arc-1/) ⭐️ 9.0/10

一个从头开始训练仅 1.5 小时的小型自回归 Transformer，在 ARC 基准上取得了有竞争力的成绩，超越了众多需要巨大训练成本的大型语言模型（LLM）。该模型并非 LLM，而是为特定任务构建的紧凑型 Transformer。 这一结果挑战了当前主流的扩展范式，表明复杂的推理任务可能不需要庞大的模型和数据规模。它可能使高级 AI 推理研究对小实验室和独立研究者变得更加可及和高效。 该模型并非 LLM，而是一个从头构建的小型自回归 Transformer。作者将性能提升归因于现代架构选择（SwiGLU、RMSNorm）、改进的数据多样性和洗牌，以及从 4 层扩展到 8 层。作者还澄清，在 ARC 评估谜题上训练是允许的，因为 ARC 是元学习基准，而非在测试标签上训练。

hackernews · porridgeraisin · 9月1日 09:52 · [社区讨论](https://news.ycombinator.com/item?id=49519939)

**背景**: 抽象推理语料库（ARC）是 François Chollet 在 2019 年提出的 AGI 基准，由基于网格的视觉推理谜题组成，测试 AI 系统从少量示例中推断抽象规则的能力，属于流体智力的一种形式。传统上，在 ARC 上取得高分通常需要大型语言模型或需要巨大计算资源的复杂系统。这项工作表明，一个小得多的模型也能具有竞争力，可能改变人们对推理任务所需规模的假设。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Abstraction_and_Reasoning_Corpus">Abstraction and Reasoning Corpus</a></li>
<li><a href="https://github.com/fchollet/ARC-AGI">GitHub - fchollet/ARC-AGI: The Abstraction and Reasoning Corpus</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC -AGI-3</a></li>

</ul>
</details>

**社区讨论**: 作者与评论者互动，澄清该模型并非 LLM，并说明 ARC 的设计允许在评估谜题上训练，这并不等同于在测试标签上训练。一些评论者赞扬了这一结果，但指出样本效率低下仍是现代 LLM 的主要问题，并将这些架构调整称为“挤柠檬”。其他人则祝贺作者取得的成就，并对未来研究表示期待。

**标签**: `#ARC`, `#transformer`, `#machine learning`, `#efficiency`, `#AI research`

---

<a id="item-3"></a>
## [OpenAI 的 Astra 首个达到关键网络能力阈值](https://openai.com/index/path-to-astra) ⭐️ 9.0/10

OpenAI 宣布，Astra 是首个在其 Preparedness Framework 下达到“关键网络安全能力阈值”的模型，并加强了发布安全措施。 这一里程碑触发了 OpenAI 安全框架中强制性的开发保障和更严格的审查。它为前沿 AI 实验室如何处理具有潜在攻击性网络能力的模型开创了先例。 根据框架，“关键阈值”要求模型能在无需人工干预的情况下，识别并开发针对多种加固的真实关键系统的功能性零日漏洞利用，或能基于高层目标设计并执行端到端的新型网络攻击策略。Astra 达到阈值意味着 OpenAI 必须暂停进一步开发，直到制定出达到“关键”标准的控制措施。

rss · OpenAI Blog · 9月1日 13:00

**背景**: OpenAI 的 Preparedness Framework 是一个用于追踪、评估和防范前沿 AI 灾难性风险的结构化流程。它定义了网络安全能力阈值，达到“关键”等级将触发额外的开发与部署安全措施。本次公告是这些承诺的首次实际激活。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/">Responding to the next frontier of critical cyber capabilities | OpenAI</a></li>
<li><a href="https://openai.com/index/updating-our-preparedness-framework/">Our updated Preparedness Framework | OpenAI</a></li>
<li><a href="https://www.csoonline.com/article/4207311/openai-says-astra-could-reach-critical-cyber-capability-tightens-safeguards.html">OpenAI says Astra could reach ‘critical’ cyber capability, tightens safeguards | CSO Online</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI safety`, `#cybersecurity`, `#frontier models`, `#Preparedness Framework`

---

<a id="item-4"></a>
## [FBI 调查暗网出售 1.53 亿张驾照事件](https://krebsonsecurity.com/2026/09/fbi-probes-service-selling-153m-drivers-licenses/) ⭐️ 9.0/10

一个暗网服务正在出售超过 1.53 亿张美国和加拿大驾照的扫描件，FBI 新奥尔良办事处已就此展开正式调查。据称这些图像来自路易斯安那州一家身份验证公司。 此事件暴露了海量高度敏感的身份证明文件，使数百万人面临身份盗窃和欺诈风险。同时也引发了人们对收集和存储此类数据的身份验证公司安全措施的严重担忧。 该服务据称包含来自美国和加拿大的 1.53 亿张驾照扫描件，似乎是从路易斯安那州一家广泛使用的身份验证公司获取图像。KrebsOnSecurity 的报道基于对驾照信息出现在该服务上可供购买的受害者的采访。

rss · Krebs on Security · 9月1日 22:40

**背景**: 暗网是互联网中无法通过普通搜索引擎索引的部分，常被用于非法活动。身份验证公司会收集驾照等敏感证件以确认用户身份，因此成为黑客攻击的重点目标。此类数据一旦泄露，犯罪分子便可能将其用于身份盗窃、欺诈或进一步的安全攻击。

**标签**: `#security`, `#data breach`, `#identity theft`, `#privacy`, `#FBI`

---

<a id="item-5"></a>
## [攻击者利用 Langflow 与 Rails 严重漏洞窃取凭证并开展 C2 活动](https://thehackernews.com/2026/09/attackers-exploit-critical-langflow-and.html) ⭐️ 9.0/10

VulnCheck 发现，威胁攻击者正在积极利用两个严重漏洞：Langflow 的 CVE-2026-0768 和 Ruby on Rails 的 CVE-2026-66066。其中 Langflow 漏洞是未经验证的远程代码执行漏洞，可让攻击者窃取凭据、令牌和密钥；Rails 漏洞则被用于命令与控制（C2）活动。 这些是在广泛使用的框架中已被积极利用的严重漏洞，其中 CVE-2026-0768 的 CVSS 评分为 9.8。任何运行未修补 Langflow 或 Rails 应用的组织都面临凭证泄露、数据受损和网络被接管的风险。 CVE-2026-0768 源于对用户输入的验证不当，允许攻击者以 root 用户身份执行任意 Python 代码。报告将 CVE-2026-66066 与命令与控制行为关联起来，整个攻击活动还包括对暴露系统的凭证探测。

rss · The Hacker News · 9月1日 07:22

**背景**: Langflow 是一个开源低代码平台，用户可通过拖拽式界面构建 AI 智能体和工作流，常用于智能体（Agentic）与检索增强生成（RAG）应用。凭证探测通常指撞库（Credential Stuffing）或凭证收割（Credential Harvesting）等攻击，即利用已泄露的用户名和密码尝试未授权访问其他系统。Ruby on Rails 是广泛使用的服务端 Web 框架，因此其漏洞对寻求命令与控制立足点的攻击者很有吸引力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.langflow.org/">Langflow | Low-code AI builder for agentic and RAG applications</a></li>
<li><a href="https://www.crowdstrike.com/en-us/cybersecurity-101/cyberattacks/credential-harvesting/">What Is Credential Harvesting? | CrowdStrike</a></li>
<li><a href="https://www.ibm.com/think/topics/langflow">What is LangFlow? | IBM</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CVE`, `#Langflow`, `#Ruby on Rails`

---

<a id="item-6"></a>
## [丹·卢评估艾德·齐特龙 AI 怀疑论预测的准确性](https://danluu.com/zitron/) ⭐️ 8.0/10

丹·卢的文章剖析了艾德·齐特龙在 2024-2025 年间的 AI 怀疑论预测，将其与实际行业进展对比，并引发了一场 402 条评论的辩论。 这篇文章之所以重要，是因为它探讨了 AI 话语如何被炒作和悲观论调共同塑造，并突显了对专家预测进行问责的难度。这对任何关注 AI 行业叙事或依据专家预测做决策的人都有意义。 该分析着眼于齐特龙在 2024-2025 年间预测的原文，而非转述。评论者补充说，超大规模云厂商将 AI 投资带来的估值收益部分计入'其他收入'，这使得对泡沫的评估更加复杂。

hackernews · jatins · 9月1日 18:35 · [社区讨论](https://news.ycombinator.com/item?id=49526069)

**背景**: 艾德·齐特龙是一位科技评论员，经常主张 AI 产业被过度炒作并即将崩溃；而丹·卢是知名工程师和随笔作家，善于用数据和细读分析科技行业的言论。这场辩论反映了 AI 信奉者与怀疑者之间更广泛的文化分裂，而该文章正位于这种紧张关系的中心。

**社区讨论**: 评论者大多持分析态度：有人要求对 AI 领袖的预测进行类似核查，也有人认为齐特龙已变得和他批评的吹捧者一样教条。一种反复出现的观点是，读者常把自己的看法替换为齐特龙的观点，而超大规模云厂商的会计处理也令泡沫判断更加复杂。

**标签**: `#AI`, `#skepticism`, `#predictions`, `#Dan Luu`, `#tech industry`

---

<a id="item-7"></a>
## [Google Play 要求 AnkiDroid 移除 Open Collective 捐赠链接](https://github.com/ankidroid/Anki-Android/issues/21656) ⭐️ 8.0/10

Google Play 已要求 AnkiDroid 从 Android 应用中移除其 Open Collective 捐赠链接，理由是 Play 计费政策。这一要求在项目的 GitHub 问题页引发了社区讨论。 这会影响依赖捐赠来支持开发的开源项目，因为应用商店政策可能限制开发者与用户的沟通方式。事件凸显了集中式应用商店管控与开源项目可持续资金支持之间的张力。 Google 的政策规定，Play 计费“不得用于包含……免税捐赠的付款”，但 Open Collective 的捐赠并非可抵税捐赠，这使得合规问题变得复杂。AnkiDroid 之前也遇到过类似情况：2019 年 WireGuard 因捐赠链接被 Play Store 下架。

hackernews · hexa555 · 9月1日 10:11 · [社区讨论](https://news.ycombinator.com/item?id=49520022)

**背景**: Open Collective 是一个开源众筹与财务管理平台，帮助社区透明地收款和花钱，通常通过财政托管方式运作。它在开源项目中很受欢迎，让项目无需单独注册法人实体即可接收和管理捐赠。Google Play 要求应用在收取数字内容或服务费用时使用 Play 计费系统，链接外部支付或捐赠平台可能被视为违规。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open_Collective">Open Collective</a></li>
<li><a href="https://opencollective.com/">Raise, manage and disburse money with full... - Open Collective</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者普遍批评 Google 的决定，有人指出 2019 年 WireGuard 也因类似原因被 Play Store 下架，并认为软件不应受垄断性应用商店的绝对控制。也有人澄清 Open Collective 并非 501(c)(3) 慈善机构，捐赠不可抵税，因此对 Google 的“免税捐赠”政策如何适用提出疑问。还有一些人感谢 AnkiDroid，并表示这则新闻提醒他们去捐赠。

**标签**: `#open-source`, `#google-play`, `#policy`, `#donations`, `#app-store`

---

<a id="item-8"></a>
## [Codex 桌面应用捆绑了 LibreOffice、Python 和 Node.js](https://simonwillison.net/2026/Sep/1/codex-libreoffice/) ⭐️ 8.0/10

2026 年 9 月 1 日，Simon Willison 发现 OpenAI Codex 桌面应用（已更名为 ChatGPT）在 ~/.cache/codex-runtimes/codex-primary-runtime 中存储了约 1.7GB 的捆绑运行时。其中包括完整的 Python 和 Node.js 安装，以及 Poppler、git 和 LibreOffice 办公套件的原生二进制文件。 这一发现揭示了 OpenAI 依赖本地捆绑的开源工具（如 LibreOffice）来处理文档，以确保与旧版 Office 文件的兼容性。同时，它也引发了关于依赖膨胀和 AI 桌面应用磁盘占用不断增大的讨论，这会影响到普通用户和开发者。 其中最大的组成部分是原生二进制文件（约 771 MB），包括 libreoffice-headless（约 429.7 MB）、node（约 446.4 MB）、python（约 440.6 MB）、poppler（约 187.9 MB）和 git（约 148.1 MB）。plugins/documents 文件夹包含了指导 Codex 如何定位和使用这些二进制的 skills 文件。

rss · Simon Willison · 9月1日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49527396)

**背景**: Codex 是 OpenAI 的编程代理，可以在用户机器上本地执行任务。桌面应用（已更名为 ChatGPT）捆绑了“primary runtime”运行时，其中包含自包含的依赖项，以便在无需用户自行安装的情况下处理文档转换和脚本执行。LibreOffice 是一个开源办公套件，2010 年从 OpenOffice.org 分叉而来；Poppler 是一个 PDF 渲染库。Simon Willison 使用 OmniDiskSweeper（macOS 磁盘占用分析工具）发现了这个大型缓存文件夹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Poppler_(software)">Poppler (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/OmniDiskSweeper">OmniDiskSweeper - Wikipedia</a></li>
<li><a href="https://poppler.freedesktop.org/">Poppler</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者大多并不意外，但也提出了担忧：有人表示自己也捆绑 LibreOffice 来读取旧版 XLS 文件，还有人质疑这些工具是随应用预装还是按需下载。一些用户指出，LibreOffice 是个庞大但可靠的依赖，还有人猜测捆绑的 LibreOffice 可能解释了某些 MS Office 文件渲染不佳的问题。另有评论认为，如果 AI 生成 Office 文档成为常态，微软 Office 可能会沦为纯粹的查看器，这对微软构成潜在威胁。

**标签**: `#OpenAI`, `#Codex`, `#LibreOffice`, `#Desktop App`, `#Dependencies`

---

<a id="item-9"></a>
## [新工具让 48GB Mac 运行 104GB Qwen3.8-Flash-Next，速度约 12 tok/s](https://github.com/carloslfu/slotstream) ⭐️ 8.0/10

一位独立开发者发布了 slotstream，这是一个基于 MLX/Swift 构建的苹果原生开源工具，可让最低 16GB 统一内存的 Mac 运行 4 比特量化、体积约 104GB 的 Qwen3.8-Flash-Next（125B 参数）模型。在 48GB Mac 的演示中，它通过结合专家卸载与 SSD 流式加载，达到了约 12 token/秒的生成速度。 这表明在消费级 Mac 上运行 100B 以上参数的 MoE 模型是可行的，内存容量从硬性限制变成了可调的速度取舍。它可以让更多开发者和爱好者不必购买昂贵的大型 GPU 服务器即可体验最前沿的大模型。 该工具使用 MLX 与 Swift 构建，带有自动模式，可在内存占用和速度之间自动权衡，作者表示下一步将移植 MTP 模块用于投机解码。125B 模型采用 4 比特量化，形成约 104GB 的工作集，工具会按需进行流式加载和专家卸载。

hackernews · carloslfu · 9月1日 16:42 · [社区讨论](https://news.ycombinator.com/item?id=49524447)

**背景**: 这项技术针对混合专家（MoE）大模型，这类模型虽然参数量巨大，但每次推理只激活其中少数专家。专家卸载会把常用专家放在内存中，按需从较慢的存储加载其他专家；SSD 流式加载则把 SSD 当作 RAM 的扩展来流式读取权重。MLX 是苹果为 Apple Silicon 统一内存架构打造的机器学习框架，让 CPU 和 GPU 共享同一块内存。先前诸如 MoE-Infinity 的研究也提醒，并非所有 MoE 模型都适合专家卸载，取决于其局部路由行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2505.16056">[2505.16056] Not All Models Suit Expert Offloading: On Local ... Not All Models Suit Expert Offloading: On Local Routing ... Not All Models Suit Expert Offloading: On Local Routing ... GitHub - EfficientMoE/MoE-Infinity: PyTorch library for cost ... GitHub - MoE-Inf/awesome-moe-inference: Curated collection of ... NOTA M SUITEXPERTOFFLOADING: ONLO CALR CONSISTENCY OFMIXTURE ... Guide to optimizing inference performance of large MoE models ...</a></li>
<li><a href="https://www.mindstudio.ai/blog/ssd-streaming-ai-models-ram-dial">SSD Streaming for AI Models: How to Turn RAM from a Wall into a Dial | MindStudio</a></li>
<li><a href="https://mlx-framework.org/">MLX</a></li>

</ul>
</details>

**社区讨论**: 社区整体反响热烈，有用户希望这类工作能让未来的 32GB M6 Mac 真正可用于本地大模型。也有运行 16GB M3 的用户怀疑 16GB 上 5 token/秒的说法，认为除非忽略热降频，否则难以实现；还有人批评 README 更像随意的会话日志，缺乏对新用户的友好介绍。一位 48GB M5 用户表示更想要更大的上下文窗口，另一位则询问 Flash-Next 相对 Qwen3.8-27B 在代码能力上有哪些提升。

**标签**: `#LLM inference`, `#MLX`, `#memory optimization`, `#on-device AI`, `#expert offloading`

---

<a id="item-10"></a>
## [Atlas：World Labs 发布可生成 3D 场景的空间智能世界模型](https://www.worldlabs.ai/blog/atlas) ⭐️ 8.0/10

World Labs 发布了 Atlas，这是一个面向空间智能的世界模型，能够从稀疏图像输入生成逼真的 3D 场景。据社区观察者称，该模型可以用手机拍摄的约十几张图像重建房屋等空间，并且也能处理视频输入。 Atlas 可能加快机器人、游戏和语义理解领域的进展，让 AI 系统能够从有限的视觉数据中推断出完整的 3D 环境。它还可能降低 3D 内容创作的成本，并为 AI 带来新的空间推理能力。 博客读者指出，在视频演示中，时间在相机移动时似乎保持冻结，并且在推进之前模型会回到真实视角，这表明时间一致性可能仍有限。World Labs 的一位联合创始人已加入讨论，回答关于 Atlas 的问题。

hackernews · johnsutor · 9月1日 17:36 · [社区讨论](https://news.ycombinator.com/item?id=49525160)

**背景**: 世界模型是 AI 系统通过学习感官数据来建立对环境的内部模拟，从而支持预测和规划；它们已成为深度学习的重要研究方向，例如 Google DeepMind 的 Genie。空间智能广义上指感知、理解和推理三维空间的能力。Atlas 针对的是稀疏视角 3D 重建，即模型必须仅从少量输入图像推断完整场景几何形状这一难题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://grokipedia.com/page/Advances_in_spatial_intelligence_in_AI_20242025">Advances in spatial intelligence in AI (2024–2025)</a></li>

</ul>
</details>

**社区讨论**: 评论者总体持乐观态度：有人认为 Atlas“令人难以置信”，可用于快速制作游戏地图原型；另有人表示这似乎是迄今为止从稀疏图像重建 3D 空间最好的模型。其他人则提出更细致的问题，例如潜在空间能否支持语义提取、时间一致性是否真的足够强，以及“世界模型”这个词到底意味着什么。

**标签**: `#world-models`, `#spatial-intelligence`, `#3d-reconstruction`, `#ai-research`, `#robotics`

---

<a id="item-11"></a>
## [Python 3.15.0 候选版本 2 发布，十月正式版前的最后阶段](https://simonwillison.net/2026/Sep/1/python-315-rc-2/) ⭐️ 8.0/10

Python 3.14 和 3.15 的发布经理 Hugo van Kemenade 宣布了 Python 3.15.0 的第二个候选版本（RC2），这是十月正式版发布前的最后一个 RC。公告强烈鼓励第三方项目维护者在 RC 阶段构建并发布适用于 Python 3.15 的 wheels 到 PyPI。 这一里程碑标志着 Python 3.15 进入代码冻结期：从现在到正式发布，只允许修复合法的错误修复。它的重要性在于，第三方包需要在十月前准备好预编译的 wheels，而提前测试 RC 有助于在正式发布前发现兼容性问题。 目前 GitHub Actions 尚未提供该 RC 版本，需要关注 actions/python-versions 仓库的更新。在此之前，可以使用给出的矩阵配置，通过 allow-prereleases 和 check-latest 选项，让 CI 自动从 RC1 切换到 RC2，并在正式版发布后切换到稳定版。

rss · Simon Willison · 9月1日 14:59

**背景**: Python wheel 是 Python 的标准打包格式，它是预先构建好的、无需编译即可安装的文件，因此比源码分发包安装更快、更可靠。PyPI（Python Package Index）是 Python 开发者在其中发布和查找可安装包的官方公共仓库。RC 阶段意味着功能已冻结，只会接受错误修复，因此这是生态维护者验证兼容性的关键窗口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://realpython.com/python-wheels/">What Are Python Wheels and Why Should You Care? – Real Python</a></li>
<li><a href="https://pythonwheels.com/">Python Wheels</a></li>

</ul>
</details>

**标签**: `#Python`, `#release candidate`, `#programming languages`, `#ecosystem`, `#software development`

---

<a id="item-12"></a>
## [CISA 警示罗克韦尔 Historian ME 存在可远程执行代码的漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-244-06) ⭐️ 8.0/10

CISA 发布了公告 ICSA-26-244-06，披露了罗克韦尔自动化 Historian ME 中的两个漏洞——一个越界写入（CVE-2025-12768）和一个基于栈的缓冲区溢出（CVE-2026-12661），可能导致远程代码执行。受影响的版本包括 Series B 5.202 和 Series C 7.101，CVSS v3.1 基础评分为 8（高危）。 这一点很重要，因为 Historian ME 在全球范围内的关键基础设施领域广泛部署，包括化工、制造业、食品与农业、医疗保健以及水务系统。具有低级别认证的攻击者可能利用越界写入漏洞在工业控制系统上执行任意代码，从而可能扰乱运营。 CVE-2025-12768 是一个越界写入漏洞（CWE-787），CVSS 评分为 8.0；CVE-2026-12661 则是基于栈的缓冲区溢出漏洞。罗克韦尔自动化建议用户升级到已修复版本或遵循其安全最佳实践；该公告未提及已有人在野外利用这些漏洞。

rss · CISA Cybersecurity Advisories · 9月1日 12:00

**背景**: 罗克韦尔自动化 Historian ME（FactoryTalk Historian Machine Edition）是一种软件解决方案，用于在过程、离散和混合制造环境中收集、存储、分析和可视化生产数据。越界写入（CWE-787）是指程序在分配的缓冲区边界之外写入数据，可能导致系统崩溃或允许攻击者执行恶意代码。CISA 的工业控制系统公告（ICSA）是美国政府在工业控制系统漏洞披露方面的一项工作，并使用 CSAF JSON 格式提供机器可读的安全警报。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.controleng.com/ec-factorytalk-historian-machine-edition-me/">EC: FactoryTalk Historian Machine Edition (ME) - Control Engineering</a></li>
<li><a href="https://securityboulevard.com/2022/06/what-is-an-out-of-bounds-read-and-out-of-bounds-write-error/">What Is An Out-of-Bounds Read and Out-of-Bounds Write Error? - Security Boulevard</a></li>

</ul>
</details>

**标签**: `#security`, `#CISA`, `#ICS`, `#Rockwell Automation`, `#vulnerability`

---

<a id="item-13"></a>
## [攻击者利用 JFrog Artifactory 严重漏洞铸造管理员令牌](https://thehackernews.com/2026/09/attackers-exploit-critical-jfrog.html) ⭐️ 8.0/10

威胁行为者正在积极利用 JFrog Artifactory 中的 CVE-2026-82329（CVSS 9.8）认证绕过漏洞，该漏洞在公开披露后数天内即遭利用。watchTowr 观察到攻击者利用该漏洞枚举令牌，并在默认配置上铸造管理员级访问令牌。 该漏洞允许未经认证的攻击者在广泛使用的 DevOps 制品仓库中获得管理员权限，可能导致供应链受到破坏。从披露到被积极利用的时间极短，凸显了组织立即修复补丁的紧迫性。 该漏洞存在于 JFrog Artifactory 的默认配置中，可通过/access/api/v1/tokens 端点触发，该端点向未经认证的攻击者返回 HTTP 200 并列出所有令牌。CVE-2026-82329 的 CVSS 评分为 9.8，属于严重级别，影响使用默认设置的实例。

rss · The Hacker News · 9月1日 17:53

**背景**: JFrog Artifactory 是一个流行的二进制仓库管理器，开发团队用它来存储和管理软件制品、容器和依赖项。认证绕过漏洞意味着软件访问控制可以被绕过；在此案例中，未经认证的攻击者只要具备网络访问能力，就能在没有有效凭据的情况下获得管理员权限。JFrog 已发布补丁，但攻击者迅速逆向分析了修复方案，并在许多用户应用更新之前开发出漏洞利用代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cvefeed.io/vuln/detail/CVE-2026-82329">CVE - 2026 - 82329 - Potential authentication bypass leading to...</a></li>
<li><a href="https://github.com/dinosn/cve-2026-82329-jfrog-artifactory">GitHub - dinosn/ cve - 2026 - 82329 - jfrog - artifactory : CVE - 2026 - 82329 ...</a></li>
<li><a href="https://thehackernews.com/2026/09/attackers-exploit-critical-jfrog.html">Attackers Exploit Critical JFrog Artifactory Flaw to Mint Admin Tokens Days After Disclosure</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CVE`, `#JFrog`, `#exploit`

---

<a id="item-14"></a>
## [恶意 Packagist 包通过 iOS 间谍软件窃取加密货币钱包种子](https://thehackernews.com/2026/09/13-malicious-packagist-packages-target.html) ⭐️ 8.0/10

网络安全研究人员在 Packagist 上发现了 13 个恶意的 Composer 主题包，这些包会向越南电影和漫画流媒体网站注入 JavaScript。注入的代码会在未修补的 iPhone 上部署间谍软件，以窃取加密货币钱包种子。 这次供应链攻击会危害那些安装了恶意包的开发者，使其网站成为感染访客未修补 iPhone 的传播媒介。它对加密货币资产构成直接威胁，并凸显了在 PHP 生态系统中加强依赖关系管理的必要性。 注入的 JavaScript 会对访客执行两种操作：移动广告欺诈和赌博重定向，此外还会投放针对未修补 iOS 设备的间谍软件。这些包伪装成主题包，对流媒体网站开发者来说看起来合法。

rss · The Hacker News · 9月1日 14:07

**背景**: Packagist 是 Composer（PHP 的依赖管理工具）的默认仓库。开发者经常使用 Composer 安装库，而官方仓库中的恶意包会构成严重的供应链风险。在此案例中，攻击链可能利用了旧版 iOS 中的已知漏洞，因此只有未修补的 iPhone 会受到影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://packagist.org/">Packagist .org</a></li>
<li><a href="https://getcomposer.org/doc/00-intro.md">Introduction - Composer</a></li>

</ul>
</details>

**标签**: `#supply-chain`, `#malware`, `#security`, `#Packagist`, `#cryptocurrency`

---

<a id="item-15"></a>
## [攻击者窃取 METR API 密钥，消耗 60 万美元 AI 额度](https://thehackernews.com/2026/09/attackers-steal-metr-api-key-and.html) ⭐️ 8.0/10

评估前沿 AI 模型的非营利组织 METR 披露了两起安全事件：外部攻击者入侵其系统，窃取了一个 API 密钥，并消耗了约 60 万美元的 AI 计算额度。据信没有敏感信息被泄露。 该事件说明了 API 密钥泄露在重度使用 AI 的组织中可能造成的真实财务风险——被盗的凭据可被迅速用于消耗昂贵的计算资源。这也凸显了整个 AI 生态系统中加强密钥管理、监控和访问控制的必要性。 攻击者利用被盗密钥消耗了约 60 万美元的 AI 计算额度后才被发现。METR 表示没有证据表明敏感信息受损，但报告中提到了两起独立的安全事件。

rss · The Hacker News · 9月1日 09:05

**背景**: METR（Model Evaluation and Threat Research，即模型评估与威胁研究）是一家总部位于加州伯克利的非营利机构，评估前沿 AI 模型自主完成长周期代理任务的能力；这类任务需要大量顺序步骤和可观的计算资源。由于这类评估高度依赖付费 AI API，METR 等组织持有可访问昂贵云 AI 资源的 API 密钥。一旦这些密钥被窃取，攻击者可能造成巨额账单或滥用底层模型。该案例凸显了 AI 基础设施中日益增长的一类安全风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/METR">METR - Wikipedia</a></li>
<li><a href="https://metr.org/">METR</a></li>
<li><a href="https://www.ai21.com/glossary/ai-agent/what-are-long-horizon-tasks/">What are Long-Horizon Tasks? | AI21</a></li>

</ul>
</details>

**标签**: `#security`, `#AI`, `#API key`, `#incident response`, `#METR`

---

<a id="item-16"></a>
## [Aesto Health 数据泄露影响超过 950 万名患者](https://www.bleepingcomputer.com/news/security/aesto-health-says-data-breach-affects-over-95-million-patients/) ⭐️ 8.0/10

Aesto LLC（以 Aesto Health 名义运营）披露了一起影响超过 950 万人的数据泄露事件。该泄露近日被发现，使其成为今年报告的最大规模的医疗相关泄露事件之一。 这一泄露事件凸显了医疗数据所面临的持续威胁，此类数据极其敏感且在黑市上很有价值。受影响患者面临身份盗窃和医疗欺诈的风险，该事件也加剧了医疗行业大规模数据泄露的趋势。 该披露未说明具体暴露的信息类型，但医疗数据通常包含姓名、社会安全号码和病历记录。此次泄露影响超过 950 万人，且为近期报告，但事件响应和通知细节仍然有限。

rss · BleepingComputer · 9月1日 19:28

**背景**: 医疗行业组织经常成为网络犯罪分子的目标，因为患者数据是机密的，可被用于敲诈、保险欺诈或在暗网市场上转售。在 HIPAA 等法规要求下，美国医疗行业报告的泄露事件数量不断上升，相关实体必须通知受影响个人。截至报道时，Aesto Health 尚未披露该网络安全事件的根本原因。

**标签**: `#cybersecurity`, `#data breach`, `#healthcare`, `#privacy`

---

<a id="item-17"></a>
## [黑客劫持 BGP 推送恶意 Virtualizor 更新](https://www.bleepingcomputer.com/news/security/hackers-push-malicious-virtualizor-update-in-bgp-hijacking-attack/) ⭐️ 8.0/10

攻击者劫持了 Virtualizor 更新基础设施的 BGP 路由，将更新请求重定向到恶意服务器，从而向用户推送了被篡改的更新。这起供应链攻击影响了 Virtualizor VPS 管理软件的用户。 这是一起利用互联网路由基础设施固有信任的高级供应链攻击。它展示了 BGP 劫持如何被武器化以破坏软件更新机制，可能影响大量 VPS 托管服务商及其客户。 此次攻击的目标是 Virtualizor，一个托管服务商常用的基于 Web 的 VPS 控制面板。通过劫持 Virtualizor 更新服务器的 BGP 路由，攻击者能够在合法更新下载到达最终用户之前，拦截并替换为恶意文件。

rss · BleepingComputer · 9月1日 14:45

**背景**: BGP（边界网关协议）是互联网中在不同自治系统之间传递流量的路由协议。它依赖网络之间的相互信任，当一个网络恶意地宣告了它并不拥有的 IP 前缀时，去往该前缀的流量就会被重定向，这就是所谓的 BGP 劫持攻击。Virtualizor 是一款用于管理虚拟专用服务器（VPS）的控制面板，其更新机制通常从自有服务器获取新版本。此次事件凸显了攻击者将目标对准软件更新渠道以分发恶意软件的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cloudflare.com/learning/security/glossary/bgp-hijacking/">What is BGP hijacking? - Cloudflare</a></li>
<li><a href="https://en.wikipedia.org/wiki/BGP_hijacking">BGP hijacking - Wikipedia</a></li>
<li><a href="https://www.virtualizor.com/">Virtualizor – Cloud Control Panel</a></li>

</ul>
</details>

**标签**: `#security`, `#BGP hijacking`, `#supply chain attack`, `#Virtualizor`, `#cybersecurity`

---

<a id="item-18"></a>
## [近 22,000 台 Exchange 服务器面临邮箱劫持漏洞风险](https://www.bleepingcomputer.com/news/security/nearly-22-000-microsoft-exchange-servers-vulnerable-to-hijack-attacks/) ⭐️ 8.0/10

近 22,000 台暴露在互联网上的 Microsoft Exchange 服务器仍未修补 CVE-2026-62911——这是一个高危的身份验证绕过漏洞。微软在 2026 年 8 月的 Patch Tuesday 中已修复该漏洞，但许多服务器尚未应用更新。 该漏洞能让攻击者绕过身份验证并劫持受影响服务器上的所有邮箱，可能导致数据窃取、钓鱼攻击和供应链攻击。系统管理员和安全团队应尽快修补暴露的 Exchange 服务器以防被利用。 该漏洞 CVE-2026-62911 是一种通过捕获-重放(Capture-Replay)实现的身份验证绕过，允许已授权的攻击者在网络上提升权限。只有安装了 2026 年 8 月安全更新的服务器才受到保护；未修补的服务器应被视为存在即时风险。

rss · BleepingComputer · 9月1日 12:38

**背景**: 身份验证绕过漏洞使攻击者能够跳过登录过程，未经授权访问系统或数据。在 Microsoft Exchange Server 中，捕获-重放攻击会记录并重放有效的身份验证消息以冒充用户。邮箱劫持随后可被用来读取敏感邮件、发起定向钓鱼或破坏业务流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/nearly-22-000-microsoft-exchange-servers-vulnerable-to-hijack-attacks/">Nearly 22,000 Microsoft Exchange servers vulnerable to hijack attacks</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2026-62911/">CVE-2026-62911: Exchange Server Auth Bypass Vulnerability</a></li>
<li><a href="https://cybersecuritynews.com/exchange-servers-remain-exposed-2026-62911/">Over 21,000 Microsoft Exchange Servers Remain Exposed to Active CVE-2026-62911 Exploitation</a></li>

</ul>
</details>

**标签**: `#security`, `#Microsoft Exchange`, `#vulnerability`, `#cybersecurity`

---

<a id="item-19"></a>
## [CISA 警告罗克韦尔 RSLinx Classic 存在拒绝服务漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-244-01) ⭐️ 7.0/10

CISA 发布了公告（ICSA-26-244-01），披露了 Rockwell Automation RSLinx Classic 4.50 及更早版本中的多个漏洞。这些漏洞（CVE-2026-9621、CVE-2026-9622、CVE-2026-9624、CVE-2026-9625）可能被利用造成拒绝服务（DoS）条件。 RSLinx Classic 是关键制造环境中广泛部署的通信服务器，因此可利用的远程拒绝服务漏洞可能会干扰全球工业运营。加上 8.6 的高 CVSS 评分以及无需认证即可通过网络利用，升级到 4.60 版本成为 OT/ICS 安全团队的优先事项。 该公告将 CWE-190（整数溢出或回绕）、CWE-191（整数下溢）和 CWE-120（经典缓冲区溢出）列为主要原因。精心构造的 CIP 数据包可使 RSLinx Classic 服务崩溃；罗克韦尔已在 4.60 版本中修复这些问题，并建议无法升级的用户采取安全最佳实践。

rss · CISA Cybersecurity Advisories · 9月1日 12:00

**背景**: RSLinx Classic 是罗克韦尔自动化推出的工厂通信解决方案，为多种 Rockwell Software 和 Allen-Bradley 应用程序提供 Allen-Bradley 可编程控制器访问，是自动化领域安装最广泛的通信服务器之一。CISA 定期发布针对工业控制系统产品的 ICS 公告，并常使用 CSAF 格式以支持漏洞信息的自动化共享。整数溢出和缓冲区溢出漏洞通常是程序错误处理数据大小所致，被利用后可能导致崩溃或未授权代码执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://literature.rockwellautomation.com/idc/groups/literature/documents/gr/linx-gr001_-en-e.pdf">RSLinx Classic Getting Results Guide</a></li>
<li><a href="https://bin95.com/articles/automation/rslinx-plc-communication.htm">What is RSLinx classic for PLC communication?</a></li>
<li><a href="https://cwe.mitre.org/data/definitions/680.html">CWE - CWE-680: Integer Overflow to Buffer Overflow (4.20)</a></li>

</ul>
</details>

**标签**: `#ICS`, `#security`, `#CISA`, `#Rockwell Automation`, `#vulnerability`

---

<a id="item-20"></a>
## [CISA 警告罗克韦尔自动化 PLC 存在拒绝服务漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-244-05) ⭐️ 7.0/10

CISA 发布了针对 CVE-2021-42260 的公告 ICSA-26-244-05，该漏洞影响罗克韦尔自动化的 ControlLogix、CompactLogix、GuardLogix 和 Compact GuardLogix 控制器。罗克韦尔建议更新到固件 34.015 或更高版本以修复该问题。 这些可编程逻辑控制器在全球关键制造行业广泛部署，漏洞可能导致控制器故障并中断工业流程。虽然 CVSS 评分为 7.5，但运营中断的潜在风险使得受影响设施急需修补。 该漏洞属于“不可达退出条件的循环”（无限循环），由恶意构造的数据触发，导致重大不可恢复故障（MNRF）。安全控制器需要重新下载程序才能恢复，非安全控制器需要二级复位；修复固件版本为 34.015 及更高版本。

rss · CISA Cybersecurity Advisories · 9月1日 12:00

**背景**: 可编程逻辑控制器（PLC）是用于自动化装配线和机械等机电过程的工业计算机。罗克韦尔的 Logix 家族，包括 ControlLogix 和 CompactLogix，广泛应用于制造业。CISA 的工业控制系统公告为关键基础设施运营商提供漏洞信息和修复指导。CVE-2021-42260 是这一具体漏洞的公共标识符。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2021-42260">NVD - CVE - 2021 - 42260</a></li>
<li><a href="https://www.rockwellautomation.com/en-us/products/hardware/programmable-controllers/1756controllogix5580.html">ControlLogix 5580 Controllers | Rockwell Automation | US</a></li>

</ul>
</details>

**标签**: `#security`, `#ICS`, `#vulnerability`, `#Rockwell Automation`, `#CISA`

---