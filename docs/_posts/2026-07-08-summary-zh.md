---
layout: default
title: "Horizon Summary: 2026-07-08 (ZH)"
date: 2026-07-08
lang: zh
---

> 从 93 条内容中筛选出 20 条重要资讯。

---

1. [欧盟聊天控制提案：扫描所有消息以查找 CSAM](#item-1)
2. [新的 Januscape Linux 漏洞允许在 Intel/AMD 设备上逃逸虚拟机](#item-2)
3. [新研究：LLM 无法模拟人类偏好](#item-3)
4. [Kokoro：本地 CPU 友好的高质量文本转语音](#item-4)
5. [微软解雇 id Software 的 idTech 团队](#item-5)
6. [欧盟议会二读推进 Chat Control 法律](#item-6)
7. [sqlite-utils 4.0 引入数据库迁移等新功能](#item-7)
8. [AI 推理成本骤降：为智能体重新设计数据系统](#item-8)
9. [新闻简报覆盖重大 AI 模型发布](#item-9)
10. [NVIDIA Isaac GR00T 实现端到端人形机器人策略开发](#item-10)
11. [NVIDIA Vera CPU 提升 AI 工厂吞吐量，加速智能体 AI](#item-11)
12. [日立能源 e-mesh EMS 缓冲区溢出漏洞](#item-12)
13. [CISA 警告日立能源 PROMOD V 存在 HTTP 漏洞](#item-13)
14. [CISA 警告西门子 SINEC OS 存在严重漏洞（CVSS 9.8）](#item-14)
15. [Hydro-Québec 电动车充电后台严重漏洞](#item-15)
16. [RedWing MaaS 将安卓银行欺诈作为 Telegram 租赁服务提供](#item-16)
17. [Google Dialogflow CX 的“Rogue Agent”漏洞允许劫持聊天机器人](#item-17)
18. [DEBULL 钓鱼利用微软设备代码流](#item-18)
19. [公共 GitHub Issue 利用 Agentic Workflows 泄露私有数据](#item-19)
20. [疑似中国黑客利用 Roundcube 漏洞攻击大学](#item-20)

---

<a id="item-1"></a>
## [欧盟聊天控制提案：扫描所有消息以查找 CSAM](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 9.0/10

欧盟的聊天控制提案——1.0 版本已到期但允许自愿扫描，2.0 版本则强制扫描所有私人消息（包括加密消息）以检测儿童性虐待材料（CSAM）——引发了关于隐私和加密的广泛讨论。 这些提案代表了数字监控政策的重大转变，可能破坏端到端加密，并影响欧洲及全球数百万用户的隐私。 聊天控制 1.0 提供了对 ePrivacy 指令的临时豁免，允许服务提供商自愿扫描消息；该豁免已到期，但 Google 和 Meta 等大型科技公司表示将继续扫描。聊天控制 2.0 则将扫描变为强制，并通过客户端扫描扩展到加密内容。

hackernews · gasull · 7月7日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48818311)

**背景**: 儿童性虐待材料（CSAM）指任何涉及未成年人的色情行为视觉描绘。客户端扫描（CSS）是一种在用户设备上在加密前或解密后扫描内容的技术，可能绕过端到端加密保护。欧盟的提案旨在打击 CSAM，但引发了关于大规模监控和削弱加密的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rainn.org/get-the-facts-about-csam-child-sexual-abuse-material/what-is-csam/">What is CSAM? - RAINN</a></li>
<li><a href="https://www.internetsociety.org/wp-content/uploads/2020/03/2022-Client-Side-Scanning-Factsheet-EN.pdf">CC BY-NC-SA 4.0 Client-Side Scanning</a></li>

</ul>
</details>

**社区讨论**: 社区评论强烈反对这些提案。用户们认为，虽然打击 CSAM 很重要，但广泛的扫描方法等同于大规模监控并破坏加密，有人将其比作'独裁权力'的攫取。其他人则对扫描加密消息的技术实现提出质疑，例如客户端扫描或中间人解密。

**标签**: `#privacy`, `#encryption`, `#surveillance`, `#EU legislation`, `#CSAM`

---

<a id="item-2"></a>
## [新的 Januscape Linux 漏洞允许在 Intel/AMD 设备上逃逸虚拟机](https://www.bleepingcomputer.com/news/linux/new-januscape-linux-kernel-flaw-allows-vm-escape-on-intel-amd-devices/) ⭐️ 9.0/10

发现了一个存在 16 年之久的 Linux 内核漏洞，名为 Januscape（CVE-2026-53359），该漏洞允许客户虚拟机逃逸并在宿主机上执行任意代码，影响 Intel 和 AMD 设备。 该漏洞对云和虚拟化安全至关重要，因为它打破了虚拟机与宿主机之间的隔离，可能允许攻击者在多租户云环境中危及多个租户。 该漏洞存在于 KVM 虚拟机管理程序处理 x86 模拟的过程中，影响 2.6.x 至 6.x 版本的 Linux 内核，但通过禁用某些 KVM 功能可能可以进行缓解。

rss · BleepingComputer · 7月7日 12:06

**背景**: 虚拟机逃逸是一种安全漏洞，其中在虚拟机内运行的程序突破隔离环境并与宿主机操作系统交互。KVM（基于内核的虚拟机）是一种广泛使用的开源虚拟机管理程序，已集成到 Linux 中。Januscape 漏洞是一个存在了 16 年的 KVM 逃逸漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/linux/new-januscape-linux-kernel-flaw-allows-vm-escape-on-intel-amd-devices/">New Januscape Linux flaw allows VM escape on Intel, AMD devices</a></li>
<li><a href="https://github.com/V4bel/Januscape">GitHub - V4bel/Januscape · GitHub</a></li>
<li><a href="https://www.securityweek.com/linux-kernel-vulnerability-allows-vm-escape-on-intel-and-amd-systems/">Linux Kernel Vulnerability Allows VM Escape on Intel and AMD Systems - SecurityWeek</a></li>

</ul>
</details>

**标签**: `#linux`, `#kernel`, `#vulnerability`, `#vm-escape`, `#security`

---

<a id="item-3"></a>
## [新研究：LLM 无法模拟人类偏好](https://www.reddit.com/r/artificial/comments/1uq52r8/ai_cant_simulate_human_preferences_new_study/) ⭐️ 9.0/10

一项新研究在 28 项真实研究和 78 个选择任务中测试了大语言模型，发现它们仅 53%的情况下与人类多数一致，几乎与随机猜测无异。 这挑战了业界日益流行的使用 LLM 作为合成用户进行产品测试和评估的趋势，表明真实的人类反馈仍然不可或缺，无法被可靠替代。 添加详细角色设定和思维链推理并未提升表现，反而使输出与真实人类理由的语义相似度下降，因为模型的推理使输出同质化，无法捕捉真实生活经验。

reddit · r/artificial · /u/Complete_Answer · 7月7日 19:19

**背景**: 许多公司一直在探索使用 LLM 作为合成用户来替代人类参与者进行用户研究，以降低成本和时间。思维链推理是一种提示工程技术，通过鼓励逐步推理来提升复杂任务的表现。这项研究实证表明，LLM 无法可靠地复制人类偏好，尤其是那些根植于主观经验的偏好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chain-of-thought_reasoning">Chain-of-thought reasoning</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#human preferences`, `#synthetic users`, `#evaluation`

---

<a id="item-4"></a>
## [Kokoro：本地 CPU 友好的高质量文本转语音](https://ariya.io/2026/03/local-cpu-friendly-high-quality-tts-text-to-speech-with-kokoro/) ⭐️ 8.0/10

一篇博客文章介绍了 Kokoro，这是一个拥有 8200 万参数的开源权重 TTS 模型，可在 CPU 上高效运行，无需 GPU 即可提供高质量的语音合成。该模型已在 GitHub 上发布，支持多种语言和声音。 Kokoro 使得没有昂贵 GPU 的用户也能使用高质量 TTS，支持本地、私密和离线的语音应用。这对于无障碍工具、内容消费以及硬件资源有限的开发者来说至关重要。 尽管体积小巧，Kokoro 在效率和质量上超越了许多更大的模型。它允许手动添加 IPA 发音指南以纠正同形异义词，并可通过 CLI 使用或集成到应用中，用于阅读文章、书籍等。

hackernews · speckx · 7月7日 18:24 · [社区讨论](https://news.ycombinator.com/item?id=48821576)

**背景**: 传统的高质量 TTS 模型通常需要 GPU 加速才能实现实时性能，限制了可及性。Kokoro 是一个轻量级的开源权重模型，拥有 8200 万参数，在 CPU 上运行即可达到与更大模型相当的质量。它代表了高效 AI 模型的增长趋势，使先进技术更加普及。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/hexgrad/kokoro">GitHub - hexgrad/kokoro: https://hf.co/hexgrad/Kokoro-82M</a></li>
<li><a href="https://kokorottsai.com/">Kokoro TTS: Advanced AI Text-to-Speech Model with 82M parameters</a></li>
<li><a href="https://github.com/nazdridoy/kokoro-tts">GitHub - nazdridoy/kokoro-tts: A CLI text-to-speech tool using the ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应热烈，用户称赞 Kokoro 对 CPU 友好以及支持 IPA，用于无障碍产品。一些用户指出其在单词发音和同形异义词方面的局限，但总体评价积极。有用户受 Kokoro 启发创建了自己的工具。

**标签**: `#TTS`, `#text-to-speech`, `#CPU`, `#accessibility`, `#open-source`

---

<a id="item-5"></a>
## [微软解雇 id Software 的 idTech 团队](https://gamefromscratch.com/microsoft-fire-idtech-team-at-id-software/) ⭐️ 8.0/10

据报道，微软已经解雇了 id Software 的 idTech 引擎开发团队。此举可能标志着该工作室内部引擎开发策略的转变。 此次裁员可能加速游戏行业对 Unreal Engine 等第三方引擎的依赖，减少技术多样性。这也引发了对微软是否致力于保留 id Software 独特技术文化的担忧。 idTech 团队负责维护和推进用于《毁灭战士》和《雷神之锤》等作品的引擎。微软尚未官方确认受影响员工的具体人数。

hackernews · bauc · 7月7日 15:33 · [社区讨论](https://news.ycombinator.com/item?id=48819244)

**背景**: idTech 是由 id Software 开发的一系列游戏引擎，以开创性的 3D 图形技术（如《毁灭战士》引擎、《雷神之锤》引擎）而闻名。版本包括 id Tech 5、id Tech 6 及后续迭代。微软于 2021 年收购了 id Software 的母公司 ZeniMax Media，将该工作室纳入 Xbox Game Studios 旗下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech">id Tech - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech_5">id Tech 5 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech_6">id Tech 6 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了对游戏开发同质化趋势的担忧，一些人认为微软用内部创新换取短期成本节约。其他人指出缺乏确凿证据，但批评了 id Software 技术遗产可能丧失的风险。整体情绪对微软的战略方向持负面看法。

**标签**: `#game engines`, `#Microsoft`, `#idTech`, `#layoffs`, `#game development`

---

<a id="item-6"></a>
## [欧盟议会二读推进 Chat Control 法律](https://www.heise.de/en/news/Showdown-in-Strasbourg-The-unexpected-return-of-Chat-Control-1-0-11356680.html) ⭐️ 8.0/10

欧盟议会在周二二读中推进了有争议的 Chat Control（CSAR）法律，周四将进行修正和否决的最终投票。 如果通过，该法律将要求平台扫描私人消息中的儿童性虐待材料，实质上强制客户端扫描并削弱端到端加密，对整个欧盟的数字隐私和安全构成重大威胁。 在二读中，只需在场欧洲议会议员的简单多数即可通过法律，而修正或否决则需要绝对多数（361 票）；许多议员已因暑假离场，使得阻止该法律更加困难。

hackernews · miroljub · 7月7日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=48819008)

**背景**: Chat Control，正式名称为《预防和打击儿童性虐待条例》（CSAR），由欧盟委员会于 2022 年 5 月提出。它旨在通过要求平台使用客户端扫描技术扫描用户通信（包括加密消息）来检测和报告儿童性虐待材料（CSAM）。批评者认为这打破了端到端加密并导致大规模监控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>
<li><a href="https://euroweeklynews.com/2025/11/29/chat-control-approved-certain-eu-countries-will-see-your-private-messages-is-yours-on-the-list/">Chat Control: EU will see your private messages</a></li>
<li><a href="https://stateofsurveillance.org/news/eu-chat-control-expires-april-3-scanning-ends-whats-next-2026/">Chat Control Is Dead. Long Live Chat Control. - State of Surveillance</a></li>

</ul>
</details>

**社区讨论**: 评论者对二读中给予支持方的战术优势表示沮丧，指出否决需要绝对多数而通过只需简单多数。有人引用让-克洛德·容克的言论，批评立法程序故意不透明。还有人对周四能否聚集足够的反对票表示怀疑。

**标签**: `#EU policy`, `#privacy`, `#encryption`, `#surveillance`, `#legislation`

---

<a id="item-7"></a>
## [sqlite-utils 4.0 引入数据库迁移等新功能](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0 已发布，新增数据库迁移、通过新的 db.atomic() 方法实现的嵌套事务，以及对复合外键的支持。 这是自 2020 年 3.0 以来的首次大版本升级，显著增强了 sqlite-utils 管理 SQLite 数据库的能力，使模式变更、并发操作和复杂关系处理对开发者更加容易。它填补了该工具长期的功能空白，惠及 Python 和 SQLite 生态系统。 迁移系统使用 Python 函数和 table.transform() 方法来实现超越 SQLite 有限 ALTER TABLE 的模式变更。嵌套事务通过 db.atomic() 利用 SQLite 保存点实现，复合外键允许在外键约束中引用复合主键。

rss · Simon Willison · 7月7日 19:32

**背景**: SQLite 是一种轻量级的基于文件的数据库引擎，广泛应用于各类应用程序中。sqlite-utils 库提供了用于创建和修改 SQLite 数据库的 Python 接口和命令行工具。数据库迁移是一种对数据库模式进行增量变更的方法，之前是该工具的一个缺失功能。嵌套事务允许在更大事务内执行原子操作，而复合外键则支持引用具有复合主键的表。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/7/sqlite-utils-4/">sqlite-utils 4.0, now with database schema migrations</a></li>
<li><a href="https://sqlite-utils.datasette.io/en/latest/migrations.html">Database migrations - sqlite-utils</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#database migration`, `#python`, `#tools`, `#software release`

---

<a id="item-8"></a>
## [AI 推理成本骤降：为智能体重新设计数据系统](http://bair.berkeley.edu/blog/2026/07/07/intelligence-is-free-now-what/) ⭐️ 8.0/10

GPT-4 级别推理成本从 2023 年初每百万 token 约 30 美元降至今日不足 1 美元，部分提供商甚至低于 0.10 美元，年降幅中位数达 50 倍。这一趋势预示着日常知识工作即将进入近乎免费的智能时代。 这一惊人的成本下降意味着 AI 智能体将成为数据系统的主要工作负载，迫使数据系统在应对智能体用户、管理智能体群以及合成定制系统方面进行根本性重新设计。这一转变对数据基础设施、软件工程和企业自动化产生广泛影响。 加州大学伯克利分校 BAIR 博客的分析提出了三大挑战：为智能体设计的数据系统（不同的工作负载特性）、由智能体构成的数据系统（数千智能体的状态管理与协调）、以及由智能体创建的数据系统（智能体合成可信赖的系统）。该文章将这些视为近乎零推理成本带来的挑战与机遇。

rss · BAIR Blog · 7月7日 09:00

**背景**: AI 推理是指运行已训练模型以生成预测或输出的过程，自 2023 年以来，由于模型效率提升、硬件进步和竞争性定价，其成本大幅下降。AI 智能体是能够自主执行任务（如查询数据库、分析数据或协调工作流）的程序。传统数据系统为人工查询或批处理设计，但智能体引入了大规模并发和长期有状态交互等新模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://epoch.ai/data-insights/llm-inference-price-trends">LLM inference prices have fallen rapidly but unequally across tasks | Epoch AI</a></li>
<li><a href="https://www.startups.com/lexicon/inference-cost">Inference Cost: definition, the per-token economics of running AI, and the 10x-per-year cost decline | Startups.com</a></li>

</ul>
</details>

**标签**: `#AI costs`, `#inference`, `#agents`, `#data systems`, `#trends`

---

<a id="item-9"></a>
## [新闻简报覆盖重大 AI 模型发布](https://www.latent.space/p/ainews-the-field-guide-to-fable) ⭐️ 8.0/10

最新的 AINews 新闻简报覆盖了它称之为迄今为止最重要的 AI 模型发布。 这份简报提供了一个关键 AI 模型发布的精选摘要，帮助专业人士了解该领域的突破。 这份名为《Fable 实地指南》的简报聚焦于一次重大模型发布，并以摘要形式提供快速阅读。

rss · Latent Space · 7月7日 04:44

**标签**: `#AI`, `#model launch`, `#newsletter`, `#machine learning`

---

<a id="item-10"></a>
## [NVIDIA Isaac GR00T 实现端到端人形机器人策略开发](https://developer.nvidia.com/blog/develop-humanoid-robot-policies-end-to-end-with-nvidia-isaac-gr00t/) ⭐️ 8.0/10

NVIDIA 发布了 Isaac GR00T 平台，该平台提供了开发人形机器人策略的端到端工作流，包括基础模型和仿真工具。该平台旨在加速从研究到部署的人形机器人技能开发。 此次发布满足了团队从机器人启动到特定任务技能开发过程中对可重复、高效开发工作流日益增长的需求。通过提供开放的基础模型和仿真框架，NVIDIA 降低了人形机器人研究和商业应用的门槛。 Isaac GR00T 平台包括开放的视觉-语言-动作（VLA）模型 GR00T N1.7，这是一个通用人形机器人技能的基础模型。它还提供仿真环境和数据管道，用于端到端的策略训练。

rss · NVIDIA Developer Blog · 7月7日 17:05

**背景**: 传统的人形机器人策略开发需要劳动密集型的遥操作数据收集，难以规模化。NVIDIA 的 Isaac GR00T 旨在通过提供带有预训练模型和仿真工具的标准化平台来简化这一过程，这建立在之前机器人基础模型工作的基础上。该平台是 NVIDIA 加速人形机器人开发更广泛计划的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/isaac/gr00t">Isaac GR00T - Generalist Robot 00 Technology | NVIDIA Developer</a></li>
<li><a href="https://github.com/Nvidia/Isaac-GR00T">GitHub - NVIDIA/Isaac-GR00T: NVIDIA Isaac GR00T N1.7 - A Foundation Model for Generalist Robots. · GitHub</a></li>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-isaac-gr00t-n1-open-humanoid-robot-foundation-model-simulation-frameworks">NVIDIA Announces Isaac GR00T N1 — the World’s First Open Humanoid Robot Foundation Model — and Simulation Frameworks to Speed Robot Development | NVIDIA Newsroom</a></li>

</ul>
</details>

**标签**: `#robotics`, `#NVIDIA`, `#humanoid`, `#AI`, `#policy learning`

---

<a id="item-11"></a>
## [NVIDIA Vera CPU 提升 AI 工厂吞吐量，加速智能体 AI](https://developer.nvidia.com/blog/nvidia-vera-cpu-boosts-ai-factory-throughput-to-accelerate-agentic-workloads/) ⭐️ 8.0/10

NVIDIA 发布了专为智能体 AI 工作负载设计的高性能 Vera CPU，可为 AI 工厂带来高达 6 倍的 CPU 吞吐量提升。 随着 AI 智能体成为企业工作流的核心，Vera CPU 的专用架构能加速多步推理、工具使用和代码执行，从而推动自主 AI 系统的普及。 Vera CPU 拥有 88 个核心，可部署在包含 256 颗液冷芯片的机架中，面向结合推理、检索和编排的密集 AI 工厂环境。

rss · NVIDIA Developer Blog · 7月7日 15:10

**背景**: AI 工厂是专为训练和运行 AI 模型优化的数据中心，通常使用 GPU 和高带宽互连。智能体 AI 是指能够自主使用工具并采取行动以实现目标的系统，需要多步推理。Vera CPU 是 NVIDIA 首款专为这些智能体工作负载设计的 CPU，旨在卸载并加速不适合 GPU 处理的任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/vera-cpu/">Next Gen Data Center CPU | NVIDIA Vera CPU</a></li>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-unveils-vera-the-cpu-for-agents">NVIDIA Unveils Vera, the CPU for Agents - NVIDIA Newsroom</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/nvidia-unveils-details-of-new-88-core-vera-cpus-positioned-to-compete-with-amd-and-intel-new-vera-cpu-rack-features-256-liquid-cooled-chips-that-deliver-up-to-a-6x-gain-in-cpu-throughput">Nvidia unveils details of new 88-core Vera CPUs positioned to compete ...</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#Vera CPU`, `#AI hardware`, `#agentic AI`, `#AI factory`

---

<a id="item-12"></a>
## [日立能源 e-mesh EMS 缓冲区溢出漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-188-03) ⭐️ 8.0/10

披露了日立能源 e-mesh EMS 版本 4.1.6、4.4.2 和 4.7.0 中存在一个基于堆的缓冲区溢出漏洞（CVE-2026-42945），CVSS 评分为 8.1，可能导致拒绝服务或任意代码执行。 该漏洞影响全球部署的能源行业关键基础设施，成功利用可能导致系统中断或远程代码执行，对电网运行构成重大风险。 漏洞存在于 e-mesh EMS 使用的 NGINX 的 ngx_http_rewrite_module 模块中；利用需要精心构造的 HTTP 请求，并在 ASLR 禁用时可绕过。缓解措施包括将 NGINX 更新到 v1.30.2 或更高版本，并确保 ASLR 已启用。

rss · CISA Cybersecurity Advisories · 7月7日 12:00

**背景**: e-mesh EMS 是日立能源推出的能源管理系统，帮助公用事业和集成商管理分布式能源资源。通用安全咨询框架（CSAF）是一种机器可读的安全公告标准化格式，CISA 使用该格式发布了此公告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hitachienergy.com/news-and-events/blogs/2024/06/it-s-a-showcase-new-e-mesh-updates-and-eks-energy-synergies-at-smarter-e-intersolar-2024">It’s a showcase! New e-mesh™ updates and ... - Hitachi Energy</a></li>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>

</ul>
</details>

**标签**: `#vulnerability`, `#buffer overflow`, `#ICS`, `#Hitachi Energy`, `#EMS`

---

<a id="item-13"></a>
## [CISA 警告日立能源 PROMOD V 存在 HTTP 漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-188-02) ⭐️ 8.0/10

2026 年 7 月 7 日，CISA 发布公告，警告日立能源 PROMOD V 1.0.10 及更早版本存在漏洞（CVE-2026-10763），该产品使用不安全的 HTTP 而非 HTTPS，可能导致凭据窃取和未授权访问。 该漏洞影响全球能源行业，CVSS 评分为 7.1（高），对关键基础设施构成重大风险，敏感数据被拦截可能导致运营中断。 该漏洞源于第三方 Digipede 服务器缺乏 HTTPS 支持。修复方法是将 PROMOD V 升级至 1.0.11 版本，并在 Digipede 服务器上启用 HTTPS。

rss · CISA Cybersecurity Advisories · 7月7日 12:00

**背景**: PROMOD V 是一种用于能源行业的电力系统建模和仿真工具。HTTP 以明文传输数据，容易受到拦截和篡改。HTTPS 对通信进行加密，提供机密性和完整性。通用安全咨询框架（CSAF）是一种用于交换安全公告的标准化格式，CISA 使用它发布漏洞信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://windowsforum.com/threads/cve-2026-10763-promod-v-fix-upgrade-to-1-0-11-and-enable-https.435603/">CVE-2026-10763 PROMOD V Fix: Upgrade to 1.0.11 and Enable ...</a></li>
<li><a href="https://github.com/advisories/GHSA-jm8g-r6p8-h3xf">PROMOD V is using insecure HTTP communication instead of...</a></li>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>

</ul>
</details>

**社区讨论**: 在 Windows 论坛和 GitHub 公告中，用户讨论了立即打补丁的必要性。一些人指出依赖第三方服务器实现 HTTPS 是系统性弱点。总体情绪是急需升级到 1.0.11 并启用 HTTPS。

**标签**: `#cybersecurity`, `#OT`, `#vulnerability`, `#critical infrastructure`, `#CISA`

---

<a id="item-14"></a>
## [CISA 警告西门子 SINEC OS 存在严重漏洞（CVSS 9.8）](https://www.cisa.gov/news-events/ics-advisories/icsa-26-188-05) ⭐️ 8.0/10

CISA 发布公告警告，西门子 SINEC OS V4.0 之前版本存在多个严重漏洞，CVSS 评分为 9.8。西门子建议将 RUGGEDCOM RST2428P 更新至 V4.0 或更高版本。 这些漏洞影响能源、交通等关键基础设施行业，最高严重性评分 9.8 表明无需认证即可远程执行代码。立即修补对于防止 OT/ICS 环境中的利用至关重要。 该公告列出了超过 30 个不同的 CVE 标识符，涉及缓冲区溢出、路径遍历、竞争条件及输入验证不当等漏洞。具体受影响产品是运行 SINEC OS 的 RUGGEDCOM RST2428P 工业以太网交换机。

rss · CISA Cybersecurity Advisories · 7月7日 12:00

**背景**: SINEC OS 是西门子工业网络设备（如 RUGGEDCOM 交换机）的操作系统，这些设备部署在电网、铁路等关键基础设施中。CVSS（通用漏洞评分系统）提供 0-10 的数值评分来评估漏洞严重性，9.8 分属于严重级别。CISA（网络安全与基础设施安全局）定期发布工控系统漏洞公告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.siemens.com/en-us/products/sinec/">SINEC software | Siemens</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System">Common Vulnerability Scoring System - Wikipedia</a></li>
<li><a href="https://ipc2u.com/news/product-news/ruggedcom-rst2428p/">ruggedcom rst2428p - IPC2U Worldwide</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#ICS`, `#Siemens`, `#OT`

---

<a id="item-15"></a>
## [Hydro-Québec 电动车充电后台严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-188-01) ⭐️ 8.0/10

CISA 公告 ICSA-26-188-01 披露了 Hydro-Québec 的 Le Circuit Electrique 充电站后台存在严重漏洞，包括 CVE-2026-20744（CVSS 9.8）和 CVE-2026-42952，可能导致权限提升或拒绝服务。 这些漏洞对电动汽车充电基础设施构成重大风险，攻击者可能破坏充电运营或获得未经授权的访问，影响加拿大交通系统中数千个充电站。 漏洞包括 websocket 端点访问控制不当、缺乏认证尝试速率限制以及会话过期不足。Hydro-Québec 已通过禁用大部分站点的 OCPP 并为剩余站点实施认证来缓解风险。

rss · CISA Cybersecurity Advisories · 7月7日 12:00

**背景**: Le Circuit Electrique 后台是监控和控制加拿大魁北克数千个二级和快速充电站的数字基础设施。OCPP（开放充电点协议）是充电站与后台系统之间的标准通信协议。CISA 的公告凸显了电动汽车充电网络中日益增长的网络安全担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.isssource.com/hydro-quebec-fixes-le-circuit-electrique-charging-station/">Hydro-Québec Fixes Le Circuit Electrique Charging Station - ISSSource</a></li>
<li><a href="https://www.assurantcyber.com/blog/icsa-26-188-01/">Hydro-Québec Le Circuit Electrique charging station backend - ASSURANT™</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerabilities`, `#EV charging`, `#CISA`, `#Hydro-Québec`

---

<a id="item-16"></a>
## [RedWing MaaS 将安卓银行欺诈作为 Telegram 租赁服务提供](https://thehackernews.com/2026/07/redwing-maas-packages-android-bank.html) ⭐️ 8.0/10

Zimperium 的 zLabs 安全研究人员发现了一个名为 RedWing 的新型安卓恶意软件即服务（MaaS）操作，该服务通过 Telegram 频道出租，使低技能犯罪分子能够接管受害者手机、窃取银行凭证并截获一次性验证码。 RedWing 降低了安卓银行欺诈的门槛，使即使是技术不高的攻击者也能发起复杂的攻击，这可能会显著增加移动银行欺诈的数量和复杂程度。 RedWing 似乎是每月 300 美元的恶意软件租赁工具 Oblivion 的新变种。据 Zimperium 称，RedWing 为订阅者提供恶意软件生成器、钓鱼基础设施、可定制的载荷和远程管理工具。

rss · The Hacker News · 7月7日 17:10

**背景**: 恶意软件即服务（MaaS）是一种网络犯罪订阅模式，允许即使是低技能的攻击者通过租用工具、基础设施和支持来发起复杂攻击。RedWing 是一种作为 MaaS 通过 Telegram 提供的安卓间谍软件变种，与俄罗斯威胁行为者有关联。它针对银行应用程序，并通过设备接管窃取登录凭证和一次性验证码，从而绕过双因素认证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zimperium.com/blog/redwing-a-mobile-malware-as-a-service-operation">RedWing: A Mobile Malware-as-a-Service Operation</a></li>
<li><a href="https://www.huntress.com/malware-guide/malware-as-a-service-cybercrime">Malware-as-a-Service (MaaS) | Huntress</a></li>
<li><a href="https://hackread.com/android-malware-oblivion-fake-updates-hijack-phones/">$300 a Month Android Malware ‘Oblivion’ Uses Fake Updates to ...</a></li>

</ul>
</details>

**标签**: `#malware`, `#Android security`, `#banking fraud`, `#MaaS`, `#Telegram`

---

<a id="item-17"></a>
## [Google Dialogflow CX 的“Rogue Agent”漏洞允许劫持聊天机器人](https://thehackernews.com/2026/07/rogue-agent-flaw-could-have-let.html) ⭐️ 8.0/10

安全公司 Varonis 发现 Google Dialogflow CX 中存在一个名为“Rogue Agent”的严重漏洞，攻击者只需对一个启用代码块的代理拥有编辑权限，即可劫持同一 Google Cloud 项目中的其他代理，读取实时对话、窃取用户数据并发送攻击者编写的消息。 此漏洞至关重要，因为 Dialogflow CX 被企业广泛用于构建 AI 驱动的聊天机器人，而攻击仅需低级别的编辑权限，可能导致大规模数据窃取和钓鱼攻击，损害客户信任和敏感信息。 该漏洞利用 Dialogflow CX 剧本中的代码块功能，该功能允许使用内联 Python 代码控制代理行为。Google 已修复此问题，但该漏洞可在无需额外身份验证的情况下，允许未经授权访问项目中的所有代理。

rss · The Hacker News · 7月7日 16:37

**背景**: Dialogflow CX 是 Google Cloud 上的对话式 AI 平台，用于构建虚拟代理，通过自然语言理解 (NLU) 驱动聊天机器人。剧本是定义代理行为的关键组件，而代码块允许开发者嵌入 Python 代码以实现高级控制。“Rogue Agent”漏洞源于同一项目内代理之间的隔离不足。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/rogue-agent-flaw-could-have-let.html">Rogue Agent Flaw Could Have Let Attackers Hijack Google Dialogflow CX Chatbots</a></li>
<li><a href="https://docs.cloud.google.com/dialogflow/cx/docs/concept/playbook/code-block">Code blocks | Dialogflow CX | Google Cloud Documentation</a></li>
<li><a href="https://www.darkreading.com/application-security/dialogflow-cx-rogue-agent-flaw-enabled-ai-chatbot-data-theft">Dialogflow CX 'Rogue Agent' Flaw Enabled AI Chatbot Data Theft</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Google Cloud`, `#Dialogflow`, `#chatbot`

---

<a id="item-18"></a>
## [DEBULL 钓鱼利用微软设备代码流](https://thehackernews.com/2026/07/debull-tooling-abuses-microsoft-device.html) ⭐️ 8.0/10

名为 DEBULL 的钓鱼活动正在滥用微软合法的设备代码流来攻击 Microsoft 365 账户，通过协作主题的诱饵诱骗受害者授予访问权限。 该技术绕过了传统的钓鱼防御，因为它使用了合法的微软登录界面，使用户和安全工具更难检测。它突显了攻击者利用合法 OAuth 流程进行凭证窃取和账户劫持的日益增长的趋势。 该活动在 2026 年 6 月底到 7 月初被观察到，它不依赖虚假密码页面，而是将用户引导到合法的微软设备登录界面。ZeroBEC 报告了这些发现。

rss · The Hacker News · 7月7日 15:14

**背景**: 设备代码流是 OAuth 2.0 的扩展，专为缺乏浏览器的输入受限设备（如智能电视、IoT 设备）设计。它允许设备获取用户代码和 URL，用户随后在另一设备上访问该 URL 进行身份验证。虽然合法，但此流程可能被用于钓鱼攻击：攻击者显示虚假提示要求输入代码，然后使用获取的令牌访问企业资源。微软已引入条件访问策略来阻止设备代码流作为缓解措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/entra/identity/conditional-access/concept-authentication-flows">Authentication flows as a condition in Conditional Access policy - Microsoft Entra ID | Microsoft Learn</a></li>
<li><a href="https://learn.microsoft.com/en-us/entra/identity-platform/v2-oauth2-device-code">OAuth 2.0 device authorization grant - Microsoft identity platform | Microsoft Learn</a></li>
<li><a href="https://datatracker.ietf.org/doc/html/rfc8628">RFC 8628 - OAuth 2.0 Device Authorization Grant</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#phishing`, `#Microsoft 365`, `#device-code flow`, `#attack`

---

<a id="item-19"></a>
## [公共 GitHub Issue 利用 Agentic Workflows 泄露私有数据](https://thehackernews.com/2026/07/public-github-issue-could-trick-github.html) ⭐️ 8.0/10

Noma Security 的研究人员披露了一个漏洞：公开的 GitHub Issue 可以欺骗 GitHub Agentic Workflows，泄露组织的私有仓库数据，且无需凭证或事先访问权限。 该攻击门槛低——任何人都可以提交公开 Issue——且可能导致使用 GitHub Agentic Workflows 且对私有仓库拥有广泛读取权限的组织发生严重数据泄露。 攻击要求组织已授予代理对其所有私有仓库的读取权限；攻击者只需在公开仓库中打开一个看似正常的 Issue。

rss · The Hacker News · 7月7日 14:04

**背景**: GitHub Agentic Workflows 是一项将 AI 能力集成到 CI/CD 中的功能，允许自动化代理执行分类和代码审查等任务。这些工作流可配置仓库读取权限，若权限范围过广，攻击者可通过精心构造的公开 Issue 利用该漏洞窃取私有数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.github.com/gh-aw/">Home | GitHub Agentic Workflows</a></li>
<li><a href="https://docs.github.com/en/copilot/concepts/agents/about-github-agentic-workflows">About GitHub Agentic Workflows</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#github`, `#agentic workflows`, `#data leakage`

---

<a id="item-20"></a>
## [疑似中国黑客利用 Roundcube 漏洞攻击大学](https://thehackernews.com/2026/07/suspected-china-aligned-hackers-exploit.html) ⭐️ 8.0/10

疑似与中国有关的威胁行为者正在积极利用 Roundcube 网络邮件软件中已修补的严重漏洞（特别是 CVE-2024-42009，CVSS 评分 9.3），从美国和加拿大大学的物理和工程系窃取凭据。 此次行动凸显了国家支持的网络间谍活动持续针对学术研究机构，可能危及敏感的知识产权和个人数据。这强调了及时修补 Roundcube 等开源软件的迫切必要性。 CVE-2024-42009 是一个存储型跨站脚本（XSS）漏洞，影响 Roundcube 直至 1.6.7 的版本。攻击者利用此漏洞部署凭据窃取脚本，且该利用发生在补丁发布之后，表明目标机构未能及时修补。

rss · The Hacker News · 7月7日 09:10

**背景**: Roundcube 是一个广泛使用的开源网络邮件客户端，由 PHP 编写，因其易于部署和定制而在教育机构中广受欢迎。CVE-2024-42009 是一个严重的 XSS 漏洞，于 2024 年 8 月公开披露，CVSS 评分为 9.3。国家级威胁行为者常以大学为目标，以获取有价值的研究成果和网络立足点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Roundcube">Roundcube - Wikipedia</a></li>
<li><a href="https://roundcube.net/">Roundcube - Free and Open Source Webmail Software</a></li>
<li><a href="https://www.wiz.io/vulnerability-database/cve/cve-2024-42009">CVE-2024-42009 Impact, Exploitability, and Mitigation Steps | Wiz</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#threat intelligence`, `#Roundcube`, `#vulnerability exploitation`, `#nation-state attacks`

---