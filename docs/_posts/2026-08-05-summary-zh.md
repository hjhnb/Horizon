---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> 从 62 条内容中筛选出 20 条重要资讯。

---

1. [Keyv 及多个 npm 包在 Shai-Hulud 供应链攻击中遭入侵](#item-1)
2. [Keyv 相关的 npm 蠕虫感染数百个包，植入 Claude Code 和 VS Code 钩子](#item-2)
3. [ChainDrop npm 供应链攻击感染超过 1,300 个软件包](#item-3)
4. [Waymo 在达拉斯全面开放无人驾驶网约车服务](#item-4)
5. [DeepSeek V4 Flash 在单块 AMD MI300X 上运行，速度超 150 tokens/s](#item-5)
6. [Oxide Computer 获 4.45 亿美元 D 轮融资，发力本地云硬件](#item-6)
7. [Xbox 宕机致光盘游戏无法游玩，引发 DRM 与所有权争论](#item-7)
8. [智源与北大用一句话实现音视频联合编辑](#item-8)
9. [Qwen 3.8 Max（2.4T）与 27B 开源权重模型主打编程与智能体协作](#item-9)
10. [世界动作模型：NVIDIA 机器人操作的新范式](#item-10)
11. [CISA 警告 Thermo Fisher 基因分析仪存在 DNA 数据篡改漏洞](#item-11)
12. [CISA 警告：Acrisure KARR BT 和 DR-100 设备存在硬编码密钥漏洞](#item-12)
13. [Vibe Hacking 让新手攻击者也能利用 AI 发动高级攻击](#item-13)
14. [谷歌移除 3 个 ADK AI 工作流：恶意 Issue 触发特权代理](#item-14)
15. [cPanel 严重漏洞可让托管客户以数据库 root 身份执行 SQL](#item-15)
16. [Open VSX 市场 77 个恶意扩展窃取开发者信息](#item-16)
17. [前沿 AI 系统 NOVA 发现超 1.4 万个开源零日漏洞](#item-17)
18. [Talos 通过对端点日志的分析揭示攻击者如何利用 AI 编程工具](#item-18)
19. [Bugtraq 漏洞披露邮件列表回归](#item-19)
20. [硬件黑客指南：在亚马逊最畅销路由器上实现预认证栈溢出](#item-20)

---

<a id="item-1"></a>
## [Keyv 及多个 npm 包在 Shai-Hulud 供应链攻击中遭入侵](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 9.0/10

一款名为 Shai-Hulud 的自复制蠕虫在一场正在进行的供应链攻击中入侵了 Keyv 及多个相关 npm 包。该事件在 79 个包名中投毒了 353 个版本，并植入仓库钩子以窃取开发者和 CI 凭据。 Keyv 是一个被数百个下游项目广泛使用的键值存储库，此次入侵可能在整个 JavaScript 生态系统中产生连锁影响。由于该蠕虫还会窃取凭据，即使完成初步清理，组织仍面临后续接连失陷的高风险。 安全公告显示，该蠕虫已影响超过 500 个包，CISA 也已针对 npm 生态发布指南。恶意程序通过保留仓库钩子实现持久化，可能不断生成新的恶意提交，令彻底修复变得困难。

hackernews · cimi_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**背景**: npm 是 JavaScript 的默认包管理器，像 Keyv 这样的包通常会被作为依赖自动安装。在此次攻击中，被入侵的包会在安装阶段执行恶意代码，使蠕虫能够自我复制、窃取凭据，然后推送新的恶意版本或修改代码仓库。此类供应链攻击利用的是开发者与所依赖的开源包之间的信任关系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/keyv-linked-npm-worm-poisons-hundreds.html">Keyv-Linked npm Worm Poisons Hundreds of Packages, Plants Claude Code ...</a></li>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem | CISA</a></li>
<li><a href="https://unit42.paloaltonetworks.com/npm-supply-chain-attack/">"Shai-Hulud" Worm Compromises npm Ecosystem in Supply Chain Attack (Updated November 26)</a></li>

</ul>
</details>

**社区讨论**: 讨论区的评论很活跃，且对防范方式看法不一：有人分享用于检测供应链攻击的工具 Packj，也有人呼吁暂停使用 pre-install 钩子。还有人推荐 devcontainers 作为更安全的开发实践，另一些人则批评 npm 脆弱的依赖模式，并建议 GitHub 直接阻止该蠕虫的代码外传仓库。

**标签**: `#security`, `#npm`, `#supply chain`, `#open source`, `#package management`

---

<a id="item-2"></a>
## [Keyv 相关的 npm 蠕虫感染数百个包，植入 Claude Code 和 VS Code 钩子](https://thehackernews.com/2026/08/keyv-linked-npm-worm-poisons-hundreds.html) ⭐️ 9.0/10

一种以窃取凭据为目的的 npm 蠕虫从 keyv@6.0.0 开始传播，并于 2026 年 8 月 4 日扩散至多个组织的数百个包。SafeDep 验证了 79 个包名下的 353 个被投毒版本，更广泛的监测显示 442 个版本涉及 353 个包名，而 Aikido 则报告至少有 868 个包受影响。 这是一起大规模的软件供应链攻击，通过窃取凭据并在广泛使用的 npm 包中植入恶意钩子，可能危及开发环境。它影响了开发者、企业以及更广泛的开源生态系统，凸显了依赖链攻击日益增长的风险。 该蠕虫为 Claude Code 和 VS Code 植入了恶意钩子，并从 Keyv 和 Cacheable 命名空间传播到其他组织。具体感染途径尚不明确，但多家安全公司证实了其规模：SafeDep 验证了 79 个包名下的 353 个被投毒版本，而 Aikido 则报告至少有 868 个包受影响。

rss · The Hacker News · 8月4日 13:30

**背景**: npm 是 Node.js 的默认包管理器，一个被攻破的包可以通过依赖链级联影响成千上万的项目。keyv 是一个流行的键值存储包，支持多种后端，因此成为高价值攻击目标。Claude Code 是 Anthropic 推出的终端 AI 编程工具，而 SafeDep 是一个扫描开源包恶意代码的安全平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.npmjs.com/package/keyv">keyv - npm</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://safedep.io/platform/">SafeDep Platform: Centralized Supply Chain Security for Your...</a></li>

</ul>
</details>

**标签**: `#npm`, `#supply-chain`, `#malware`, `#security`, `#open-source`

---

<a id="item-3"></a>
## [ChainDrop npm 供应链攻击感染超过 1,300 个软件包](https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/) ⭐️ 9.0/10

名为 ChainDrop 的自传播恶意软件已入侵 npm 上超过 1,300 个软件包，这些软件包每月合计下载量达 20 亿次。该攻击被认为是一种供应链蠕虫，通过感染依赖项进行扩散。 这是规模最大的 npm 供应链攻击之一，对 JavaScript 生态造成了大规模影响。任何使用受影响软件包的开发者或组织都可能面临凭据、机密和基础设施泄露的风险。 该恶意软件会搜索本地环境中的云凭据、基础设施机密、开发者访问令牌、AI 相关配置文件以及加密货币钱包。根据 StepSecurity 的报告，共有 444 个软件包和 2,212 个版本被投毒，起始于 keyv@6.0.0。

rss · BleepingComputer · 8月4日 15:24

**背景**: npm 是 Node.js 的默认包管理器，也是最大的软件注册表，拥有数百万个软件包和每月数十亿次的下载量。供应链攻击利用了开发者与开源依赖之间的信任关系：当流行软件包被攻陷时，恶意软件可以传播到每个依赖它的项目中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/">Massive ChainDrop npm supply-chain attack infects hundreds of packages</a></li>
<li><a href="https://www.stepsecurity.io/blog/chaindrop-npm-worm">ChainDrop npm Worm: Bun-loaded CI/CD credential harvester with Ethereum ...</a></li>
<li><a href="https://www.csoonline.com/article/4205276/chaindrop-credential-stealing-worm-infects-over-400-npm-packages.html">ChainDrop credential stealing worm infects over 400 npm packages</a></li>

</ul>
</details>

**标签**: `#security`, `#npm`, `#supply-chain`, `#malware`, `#javascript`

---

<a id="item-4"></a>
## [Waymo 在达拉斯全面开放无人驾驶网约车服务](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo 的无人驾驶网约车服务现已在德克萨斯州达拉斯向所有用户开放。这使得达拉斯成为又一座任何人无需排队即可乘坐全自动驾驶汽车的城市。 这标志着无人驾驶汽车在美国主要大都市区的商业化部署又迈出了重要一步。达拉斯低密度、以汽车为中心且公共交通有限的城市布局，使其成为无人驾驶技术一个具有挑战性但重要的试验场。 Waymo 此前已在凤凰城、旧金山和洛杉矶等城市运营，并在达拉斯进行了一段时间的测试。目前该服务已向达拉斯地区（包括 DFW 大都会区部分地区）的公众全面开放，无需等待名单或特殊访问权限。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**背景**: Waymo 是一家源自谷歌无人驾驶汽车项目的自动驾驶技术公司。其无人驾驶网约车服务 Waymo One 集成了传感器、摄像头和人工智能，可在某些区域无需安全驾驶员即可运行。达拉斯是美国最大的都会圈之一，公共交通不完善，因此成为自动驾驶公司的重要扩展目标。

**社区讨论**: 社区反应总体积极但观点多样。有用户称赞 Waymo 的驾驶行为和可靠性优于人类驾驶员；一位商业房地产从业者认为无人驾驶汽车可成为有效的可负担住房政策工具；也有人担心其对本地的经济影响，因为支付给无人驾驶汽车的费用可能不如支付给人类司机的钱那样在本地流通。

**标签**: `#autonomous vehicles`, `#Waymo`, `#Dallas`, `#transportation`, `#AI deployment`

---

<a id="item-5"></a>
## [DeepSeek V4 Flash 在单块 AMD MI300X 上运行，速度超 150 tokens/s](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

一个演示项目展示了在单块 AMD MI300X GPU 上运行 DeepSeek V4 Flash，在 256k 上下文窗口下实现超过每秒 150 token 的速度。该方案利用 MI300X 的 192GB HBM 容纳模型，并据称保留了完整的推理权重。 这表明大型混合专家模型可以在单个加速器上高效运行，从而降低硬件门槛和部署成本。它也彰显了 AMD MI300X 在对成本敏感的 LLM 推理场景中，是 Nvidia 的有力替代选择。 DeepSeek V4 Flash 总参数为 284B、激活参数 13B，原生支持 100 万 token 上下文；演示采用 256k 上下文窗口作为实用取舍。MI300X 是 OAM 模块，配备 192GB HBM3，通常以 8 卡整机形式出售而非单卡购买，因此“单块 MI300X”通常指云端或租赁方式获得。

hackernews · zhoutong · 8月4日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49166386)

**背景**: DeepSeek V4 Flash 是 DeepSeek 推出的面向效率优化的混合专家语言模型，总参数 284B，每个 token 仅激活 13B，因此推理快速且成本较低。AMD MI300X 是一款数据中心 GPU，配备 192GB HBM 并采用 CDNA 3 架构，与 Nvidia 的数据中心产品直接竞争。量化是将 LLM 权重压缩进有限显存的常用技术，不过该演示声称使用模型原生的 MXFP4 量化，而非有损降级。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek-ai/DeepSeek-V4-Flash · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amd_MI300X">Amd MI300X</a></li>
<li><a href="https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html">AMD Instinct™ MI300X Accelerators</a></li>

</ul>
</details>

**社区讨论**: 评论者指出单块 MI300X 无法单独购买，它以 8 卡整机形式出售、价格约 25 万欧元，因此实验通常依靠云服务或租赁。有用户质疑为何未引用能在更少显存中运行同一模型的先前工作 DwarfStar，另有人建议采用 144GB 显存的 MI350P PCIe 卡作为更易获取的替代方案。一位评论者称赞了 256k 上下文（相比原 1M）的实用取舍，同时保留了完整权重并实现超过 150 token/s 的速度。

**标签**: `#deepseek`, `#amd-mi300x`, `#llm-inference`, `#quantization`, `#hardware`

---

<a id="item-6"></a>
## [Oxide Computer 获 4.45 亿美元 D 轮融资，发力本地云硬件](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 8.0/10

根据新的 SEC Form D 文件，Oxide Computer Company 融资 4.45 亿美元，社区消息称这是 D 轮融资。此前该公司已在 2023 年完成 4400 万美元 A 轮、2025 年完成 1 亿美元 B 轮、2026 年完成 2 亿美元 C 轮。 这轮大规模融资表明投资者对 Oxide 的押注充满信心——即企业希望以自有本地硬件的形式获得超大规模云的能力。作为一家挑战集中式云范式的知名硬件初创公司，这笔资金为 Oxide 扩大生产、销售和工程团队提供了充足空间。 SEC Form D 文件仅披露了累计融资金额，未提供更多交易条款；目前没有公开估值或参投方信息。社区评论记录了陡峭的融资轨迹：从 2026 年的 2 亿美元 C 轮到本轮的 4.45 亿美元。

hackernews · depr · 8月4日 20:13 · [社区讨论](https://news.ycombinator.com/item?id=49174407)

**背景**: Oxide Computer Company 正在打造其所谓的全球首款商用云计算机——一种将硬件与软件相结合的机架级服务器设计，融合了云超大规模技术的创新。该公司的口号是'Own Your Cloud'（拥有你的云），产品面向希望在本地部署基础设施并享有云时代运营体验的组织。Oxide 在开发者社区中以工程底蕴深厚著称，团队包括 Bryan Cantrill 和 Adam Leventhal 等领导者，还运营着社区评论中提到的热门播客'Oxide and Friends'。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oxide.computer/blog/oxide-unveils-the-worlds-first-commercial-cloud-computer">Oxide Unveils the World's First Commercial Cloud Computer</a></li>
<li><a href="https://www.linkedin.com/company/oxidecomputer">Oxide Computer Company - LinkedIn</a></li>
<li><a href="https://github.com/oxidecomputer">Oxide Computer Company - GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极但并非一致。支持者称赞产品概念和创始团队的工程背景，一位评论者表示对工程师 Jessie Frazelle 参与的工作有充分的信任；但也有人质疑 Oxide 是否真的在销售硬件。最尖锐的批评来自一位自称工程副总裁的评论者，他说其公司每年在 AWS 上花费 90 万美元，却从未收到 Oxide 对销售咨询的回应。

**标签**: `#funding`, `#hardware`, `#cloud`, `#startup`, `#Oxide`

---

<a id="item-7"></a>
## [Xbox 宕机致光盘游戏无法游玩，引发 DRM 与所有权争论](https://birchtree.me/blog/xbox-goes-down-you-cant-play-games-you-own-on-disc/) ⭐️ 8.0/10

一次 Xbox 服务中断期间，玩家发现自己无法启动甚至包括光盘版在内的所购游戏，因为主机需要进行服务器端验证。这一事件引发了一场关于 DRM、数字所有权和玩家权益的大型社区讨论（571 分、613 条评论）。 这一事件表明，现代主机上即使是“实体”光盘也依然依赖于服务器端 DRM，削弱了“真正拥有”游戏的概念。它影响所有玩家，也让关于游戏保存、二手交易和消费者权益的长期争论变得更加紧迫。 微软长期以来要求 Xbox One 光盘游戏必须联网“验证”才能完成安装，这一 DRM 机制可追溯至 2013 年。2022 年 9 月，微软取消了在 Xbox Series X 上运行 Xbox One 光盘时的强制在线检查，但当服务器验证不可用时，宕机仍可能导致游戏无法启动。

hackernews · surprisetalk · 8月4日 12:01 · [社区讨论](https://news.ycombinator.com/item?id=49167448)

**背景**: Always-on DRM（数字版权管理）要求消费者在使用产品时保持与服务器的连接，即使在离线单人模式下也是如此。微软的 Xbox One 最初计划推行激进的 DRM 限制，但在 2013 年公众强烈反对后，微软取消了其中多项要求，包括 24 小时在线签核。然而，光盘安装的在线验证仍持续多年，此类宕机事件表明，即使实体介质也可能因服务器依赖而无法访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theverge.com/2022/9/19/23356855/xbox-series-x-game-disc-drm-online-check-in">Microsoft eased up on one DRM hurdle for disc games on Xbox | The Verge</a></li>
<li><a href="https://www.flatpanelshd.com/news.php?subaction=showfull&id=1663671757">Microsoft backtracks on controversial DRM scheme for Xbox game discs - FlatpanelsHD</a></li>
<li><a href="https://en.wikipedia.org/wiki/Always-on_DRM">Always-on DRM - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者们表达了失望，认为现代游戏正沿着电视、电影和音乐行业的道路滑向丧失所有权的境地。许多人认为真正的争议核心应是有权永久持有游戏、离线游玩、备份、转售和传给后代，而非单纯物理版与数字版之争。还有人指出，GameCube 和 PS3 等老主机至今仍可离线游玩，而现代系统的在线验证会在服务器故障时把玩家锁在门外。

**标签**: `#DRM`, `#digital ownership`, `#gaming`, `#Xbox`, `#consumer rights`

---

<a id="item-8"></a>
## [智源与北大用一句话实现音视频联合编辑](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247909661&idx=3&sn=93d5f6e39859c6c9c378533ba3009898) ⭐️ 8.0/10

智源（BAAI）与北京大学合作提出一种端到端方法，可用一句自然语言指令同时编辑视频中的画面和声音。该成果由“北大与元空 AI Agent 联合实验室”出品，并标注在 SIGGRAPH Asia'26 名下发布。 音视频联合编辑一直很有挑战性，以往方法常把画面和声音分开处理，难以保持同步。这项工作指向一条更统一的端到端路径，创作者有望仅用一句话同时修改画面与声音，从而降低多模态内容制作的门槛。 文章强调该系统让画面与声音在同一个端到端生成过程中共同响应指令，但未在摘要中给出详细技术方案。这篇文章同时也是一则招聘启事，联合实验室开放 3 个岗位（含实习），并称“不设边界”。

rss · 量子位 · 8月4日 09:00

**背景**: 智源（BAAI），即北京智源人工智能研究院，是中国的一家非营利 AI 研究机构。传统视频编辑往往把画面轨道和音轨分开处理，因此在生成式编辑中让两者保持同步很困难；而端到端生成框架则从一条自然语言指令出发，直接生成编辑后的画面与声音。SIGGRAPH Asia 是计算机图形学与交互技术领域的顶级国际会议，因此与其关联的发布具有较强的学术信号意义。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Beijing_Academy_of_Artificial_Intelligence">Beijing Academy of Artificial Intelligence - Wikipedia</a></li>

</ul>
</details>

**标签**: `#audio-video editing`, `#multimodal generation`, `#deep learning`, `#SIGGRAPH`, `#natural language`

---

<a id="item-9"></a>
## [Qwen 3.8 Max（2.4T）与 27B 开源权重模型主打编程与智能体协作](https://www.latent.space/p/ainews-qwen-38-max24t-and-27b-new) ⭐️ 8.0/10

阿里巴巴的 Qwen 团队发布了 Qwen 3.8 Max，这是一个 2.4 万亿参数、支持 100 万上下文窗口的模型，同时还推出了面向编程和协作式 AI 工作流的 27B 模型。Max 目前以预览版形式通过 API 提供，但其开放权重尚未发布。 此次发布通过一个前沿规模模型增强了开源权重生态系统，让开发者和企业在构建编程助手和智能体系统时拥有更多选择，而不必依赖封闭 API。这也表明开放权重模型提供商之间的竞争正在加剧，可能加速 AI 工具领域的创新。 据报道，Qwen 3.8 Max 是阿里巴巴首个超过 1 万亿参数、原生支持图像、视频和文档处理的模型，其编程能力据称可与 Fable 5 和 Grok 4.5 相媲美，但推理速度是一个明显的瓶颈。截至目前，Max 还没有官方的基准测试表、许可证或独立评分，27B 模型的规格细节在公告中也披露有限。

rss · Latent Space · 8月4日 03:49

**背景**: 开放权重模型是指其训练参数被公开发布的 AI 模型，任何人都可以下载、运行或微调它们。阿里巴巴的 Qwen 系列已成为该领域的重要参与者，与其他开放和封闭模型展开竞争。2.4T 参数的 Qwen 3.8 Max 代表了该系列的一次重大规模跃升，其对编程和协作使用的聚焦反映了行业对专用、可部署 AI 系统的广泛需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techsy.io/en/blog/qwen-3-8">Qwen3.8-Max: 2.4T Params, 1M Context, No Weights Yet</a></li>
<li><a href="https://www.buildfastwithai.com/blogs/qwen3-8-preview-2-4t-params-open-weights-release">Qwen3.8 Preview: 2.4T Params, Open Weights, Release</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**标签**: `#Qwen`, `#open-weights`, `#LLM`, `#coding`, `#AI`

---

<a id="item-10"></a>
## [世界动作模型：NVIDIA 机器人操作的新范式](https://developer.nvidia.com/blog/beyond-vlas-how-world-action-models-reshape-robot-manipulation/) ⭐️ 8.0/10

NVIDIA 博客提出了“世界动作模型”（WAM），这是一种基于视频世界模型而非视觉语言模型的范式，旨在提升机器人操作的泛化能力。该思路与开放模型 NVIDIA Cosmos 3 相关联，后者采用 Mixture-of-Transformers 架构。 这标志着从反应式的视觉-语言-动作（VLA）策略向预测式世界模型的转变，有助于实现对新型任务、机器人和环境的零样本迁移。它有可能显著提升机器人在真实世界操作中应对未知条件的能力。 WAM 利用学习到的物理动态而非语义映射，以应对物体形状、位置或光照变化导致的失败。相关研究如 Dream-Tac 还提出了触觉感知的世界动作模型，用于处理接触密集的操控任务。

rss · NVIDIA Developer Blog · 8月4日 16:00

**背景**: 视觉-语言-动作（VLA）模型由 Google DeepMind 的 RT-2 开创，通过在机器人轨迹上微调视觉语言模型来整合视觉、语言与动作。它们实现了较强的语义泛化，但学习的是反应式的观测到动作映射，没有显式建模物理世界的变化过程。世界模型以动作（如语言指令、机器人动作等）为条件预测未来状态，而世界动作模型则将预见的未来与可执行的机器人动作结合起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/beyond-vlas-how-world-action-models-reshape-robot-manipulation/">Beyond VLAs: How World Action Models Reshape Robot Manipulation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision_language_action_model">Vision language action model</a></li>
<li><a href="https://arxiv.org/abs/2605.12090">[2605.12090] World Action Models: The Next Frontier in ... [2606.08737] Dream-Tac: A Unified Tactile World Action Model ... Beyond VLAs: How World Action Models Reshape Robot ... From World Models to World Action Models: A Concise Tutorial ... Pretrained to Imagine, Fine-Tuned to Act: The Rise of World ... GitHub - NTUMARS/Awesome-World-Model-for-Robotics-Policy Images Top Stories</a></li>

</ul>
</details>

**标签**: `#robotics`, `#world models`, `#robot manipulation`, `#vision-language-action models`, `#NVIDIA`

---

<a id="item-11"></a>
## [CISA 警告 Thermo Fisher 基因分析仪存在 DNA 数据篡改漏洞](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-216-01) ⭐️ 8.0/10

CISA 发布了编号为 ICSMA-26-216-01 的公告，披露了 Thermo Fisher Applied Biosystems 基因分析仪软件中的高危漏洞 CVE-2026-17583，CVSS 评分为 8.4。成功利用该漏洞可能允许攻击者修改.fsa/.hid 输出文件并篡改 DNA 数据，导致检测结果不准确。 这些基因分析仪广泛用于临床诊断、法医鉴定和科研领域；被篡改的 DNA 数据可能导致误诊、错误的司法结论或错误的研究结果。该公告凸显了生命科学和医疗基础设施面临的日益增长的网络安全风险。 受影响的产品包括 3500/3500xL、3730/3730xL、SeqStudio、3130 系列的数据采集软件以及 GeneMapper ID-X 软件等。Thermo Fisher 已发布安全更新，通过添加数字签名来帮助验证数据文件完整性，例如 3500/3500xL 系列数据采集软件 4.0.3 版本。

rss · CISA Cybersecurity Advisories · 8月4日 12:00

**背景**: Applied Biosystems 基因分析仪用于 Sanger 测序和片段分析，生成包含 DNA 序列数据的.fsa 和.hid 输出文件。.fsa 扩展名通常与用于表示核苷酸序列的 FASTA 文本格式相关，而且这些文件可以通过常规工具进行编辑。由于缺乏完整性校验或数字签名，对这些文件的恶意修改难以被察觉。受影响仪器广泛应用于全球的医疗、法医和科研实验室。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/FASTA_format">FASTA format - Wikipedia</a></li>
<li><a href="https://filext.com/file-extension/FSA">FSA File Extension - What is it? How to open an FSA file?</a></li>
<li><a href="https://www.thermofisher.com/hk/en/home/life-science/sequencing/sanger-sequencing/sanger-dna-sequencing/sanger-sequencing-data-analysis.html">Sanger Sequencing and Fragment Analysis Software</a></li>

</ul>
</details>

**标签**: `#security`, `#CISA`, `#vulnerability`, `#medical devices`, `#DNA analysis`

---

<a id="item-12"></a>
## [CISA 警告：Acrisure KARR BT 和 DR-100 设备存在硬编码密钥漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-216-01) ⭐️ 8.0/10

CISA 发布了一份公告（ICSA-26-216-01），披露了 CVE-2026-18411——一个存在于 Acrisure KARR BT 和 DR-100 车辆安全系统中的高危（CVSS 8.1）硬编码加密密钥漏洞。问题在于设备间共享的蓝牙认证密钥，使蓝牙范围内的攻击者能够发出未授权车辆命令，包括解锁车门和禁用发动机。 由于这些设备在全球范围内部署，且涉及交通运输关键基础设施领域，成功利用该漏洞可能让攻击者远程控制车门锁止和发动机禁用等车辆核心功能。该公告也凸显了汽车防盗和 IoT 设备中存在的一类更广泛的风险：一旦设备安装在车辆上，硬编码且共享的密钥往往难以修补。 受影响的固件版本为：KARR BT 固件早于 July_20_2026、DR-100 固件早于 July_20_2026。Acrisure Protection Group 已于 2026 年 7 月 20 日发布固件更新，用户需按照 KARR Security 固件更新说明操作；该漏洞由加州大学圣迭戈分校的团队报告，成员包括 Aaron Schulman、Jerry Yu 和 Yibo Wei 等。

rss · CISA Cybersecurity Advisories · 8月4日 12:00

**背景**: 硬编码加密密钥（CWE-321）是指直接嵌入设备固件或软件中的加密或认证密钥。由于同类设备间共享同一密钥，攻击者只需从一台设备提取密钥，即可冒充系统或绕过其认证。CISA 以 CSAF（通用安全公告框架）格式发布工控系统公告，这是一种可机读的 JSON 格式，可自动化交换安全漏洞信息。该公告涉及交通运输关键基础设施领域，而车辆防盗与追踪设备依赖蓝牙认证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cqr.company/web-vulnerabilities/hard-coded-cryptographic-keys/">Hard-coded Cryptographic Keys | CQR</a></li>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>
<li><a href="https://www.autonews.com/retail/finance-insurance/cgr-acrisure-sold-hackable-antitheft-devices-that-made-cars-easier-to-steal-20260723/">Acrisure sold auto dealers millions of hackable anti-theft devices for cars</a></li>

</ul>
</details>

**标签**: `#CISA`, `#ICS advisory`, `#vulnerability`, `#hard-coded key`, `#vehicle security`

---

<a id="item-13"></a>
## [Vibe Hacking 让新手攻击者也能利用 AI 发动高级攻击](https://thehackernews.com/2026/08/when-vibe-hacking-turns-ai-into-junior.html) ⭐️ 8.0/10

这篇文章解释了“氛围黑客”（vibe hacking）如何利用大型语言模型生成并执行攻击，使技术能力较低的攻击者也能实施复杂的网络攻击，从而打破了攻击能力与技术专长成正比的长期假设。 这之所以重要，是因为安全团队传统上按攻击者的技术水平来评估威胁；如果 AI 消除了技能门槛，那么从业余者到国家行为者的所有对手都可能构成严重风险。威胁模型与防御优先级必须适应新手攻击者也拥有高级 AI 能力的局面。 氛围黑客结合了无代码技术与 LLM 生成的载荷，使攻击者能够自动创建勒索软件、编造钓鱼信息，并模仿组织内部的沟通风格。由于恶意内容不断变化且独一无二，这类 AI 驱动的攻击可以超越传统的端点检测与响应（EDR）及基于签名的防御。

rss · The Hacker News · 8月4日 11:30

**背景**: 氛围黑客是“氛围编程”（vibe coding）的演变，后者允许非程序员借助对话式 AI 生成软件。在网络安全领域，攻击者利用基于语言和行为数据训练的 LLM，以极少的手动操作来自动化并调整攻击。这降低了攻击门槛，使“脚本小子”也能执行以往需要高级对手才能完成的攻击，从而迫使人们重新思考网络安全风险评估方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.uscsinstitute.org/cybersecurity-insights/blog/vibe-hacking-the-next-frontier-in-ai-cybersecurity-threats">Vibe Hacking: The Next Frontier in AI Cybersecurity Threats</a></li>
<li><a href="https://delinea.com/blog/vibe-hacking-vibe-coding">Vibe Hacking: The Evil Twin of Vibe Coding</a></li>
<li><a href="https://www.threatlocker.com/blog/vibe-hacking-how-ai-driven-cybercrime-outpaces-edr-and-signature-defenses">Vibe hacking: How AI-driven cybercrime outpaces EDR and signature defenses | ThreatLocker Blog</a></li>

</ul>
</details>

**标签**: `#AI security`, `#cybersecurity`, `#vibe hacking`, `#adversarial AI`, `#threat modeling`

---

<a id="item-14"></a>
## [谷歌移除 3 个 ADK AI 工作流：恶意 Issue 触发特权代理](https://thehackernews.com/2026/08/google-deletes-3-adk-ai-workflows-after.html) ⭐️ 8.0/10

谷歌在 Pillar Security 研究人员演示了一次实际的提示注入攻击后，从其 Agent Development Kit（ADK）Python 仓库中删除了三个 AI 智能体工作流。一个公开的 GitHub Issue 能够操纵分类智能体，触发一个有特权的代码修复机器人，以 adk-bot 身份发布/adk-issue-fix。 这一事件展示了在大型公司中对 AI 智能体的一次真实提示注入攻击，凸显了智能体 AI 系统会带来超越传统软件的新安全风险。它对使用 ADK 或类似智能体框架构建 AI 工作流的开发者和组织很重要，因为它表明需要适当的沙箱和权限控制。 该攻击利用了目标机器人被识别为协作者这一事实，因此注入的评论满足了仓库的权限检查，并触发了特权/adk-issue-fix 工作流。三个受影响的工作流已从公共 ADK 仓库中删除，但文章中未披露补丁或 CVE。

rss · The Hacker News · 8月4日 11:16

**背景**: Agent Development Kit（ADK）是谷歌推出的开源、代码优先框架，用于在 Python、TypeScript、Go、Java 和 Kotlin 中构建、调试和部署 AI 智能体。提示注入是一种网络安全攻击手段，攻击者将恶意指令隐藏在数据或内容中，诱使大模型执行非预期行为；当智能体处理网页内容（如 GitHub Issue）时，就可能发生间接提示注入。在本案例中，一个读取公开 GitHub Issue 的分类智能体被操纵，发出了一个命令，随后由权限更高的自动化机器人执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://adk.dev/">Agent Development Kit (ADK)</a></li>
<li><a href="https://github.com/google/adk-python">GitHub - google/adk-python: An open-source, code-first Python toolkit ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**标签**: `#security`, `#AI agents`, `#prompt injection`, `#Google ADK`, `#vulnerability`

---

<a id="item-15"></a>
## [cPanel 严重漏洞可让托管客户以数据库 root 身份执行 SQL](https://thehackernews.com/2026/08/new-cpanel-critical-flaw-could-let.html) ⭐️ 8.0/10

cPanel 已修补一个严重漏洞 CVE-2026-58048，该漏洞允许已认证的托管客户以数据库 root 权限执行 SQL 语句。该修复已在一次定向安全更新中发布，该更新还封堵了另外两条越过账户边界的路径。 该漏洞跨越了 cPanel 账户与服务器管理数据库身份之间的权限边界，可能使客户访问或修改其他用户的数据。鉴于 cPanel 在共享托管中的广泛使用，此漏洞对托管服务商及其客户构成严重风险。 该漏洞的 CVSS 4.0 评分为 9.4，表明其严重程度为严重。cPanel 的安全更新解决了数据库 root 上下文问题，同时修复了另外两条绕过账户边界的路径。

rss · The Hacker News · 8月4日 10:36

**背景**: cPanel 是一种广泛使用的网站托管控制面板，允许客户通过隔离的账户环境管理网站、电子邮件和数据库。在 MySQL 中，root 账户是具有跨所有数据库广泛权限的超级用户。托管环境中的权限边界将每个客户可执行的操作与管理操作分开；跨越该边界可能导致未经授权访问敏感数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.mysql.com/doc/refman/8.4/en/default-privileges.html">2.9.4 Securing the Initial MySQL Account</a></li>
<li><a href="https://www.cpanel.net/">Web Hosting Control Panel & Server Management Tools | cPanel</a></li>

</ul>
</details>

**标签**: `#cPanel`, `#security`, `#vulnerability`, `#privilege escalation`, `#CVE`

---

<a id="item-16"></a>
## [Open VSX 市场 77 个恶意扩展窃取开发者信息](https://www.bleepingcomputer.com/news/security/77-open-vsx-extensions-found-harvesting-developer-info/) ⭐️ 8.0/10

研究人员在 Open VSX 市场发现 77 个恶意扩展，这些扩展伪装成合法开发工具，同时窃取系统和环境信息。这些扩展会传输安装它们的主机及开发环境的相关数据。 Open VSX 是微软 Visual Studio 市场之外被广泛使用的厂商中立替代方案，服务于 VSCodium 和 Eclipse Theia 等编辑器。此次供应链攻击损害了开发者的信任，也表明 IDE 扩展市场仍是分发恶意软件的高风险途径。 这些恶意扩展伪装成合法工具，同时窃取开发者系统和环境数据。VS Code 及其衍生编辑器默认会自动更新扩展，因此被攻陷的扩展一旦发布就可能迅速扩散。

rss · BleepingComputer · 8月4日 18:50

**背景**: Open VSX 是由 Eclipse 基金会维护的开源、厂商中立扩展注册表，为微软 Visual Studio 市场提供了一个公开托管的替代方案。由于扩展在 IDE 内以与开发者相同的权限运行，它们实际上属于供应链依赖。近期的安全研究指出，泄露的访问令牌或恶意扩展更新可让攻击者向大量安装用户分发恶意软件。这一发现进一步加剧了人们对 IDE 扩展市场安全性的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsroom.eclipse.org/news/community-news/eclipse-open-vsx-free-marketplace-vs-code-extensions">Eclipse Open VSX: A Free Marketplace for VS Code Extensions | The Eclipse Foundation</a></li>
<li><a href="https://www.wiz.io/blog/supply-chain-risk-in-vscode-extension-marketplaces">Supply Chain Risk in VSCode Extension Marketplaces | Wiz Blog</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain`, `#VS Code`, `#Open VSX`, `#malware`

---

<a id="item-17"></a>
## [前沿 AI 系统 NOVA 发现超 1.4 万个开源零日漏洞](https://unit42.paloaltonetworks.com/frontier-ai-vulnerability-burst/) ⭐️ 8.0/10

Palo Alto Networks Unit 42 宣布，其自动化 AI 智能体系统 NOVA 已在开源软件供应链中发现超过 1.4 万个此前未知的漏洞。NOVA 实现了从漏洞发现、验证到报告的全流程自动化。 这标志着零日漏洞发现工业化的一次重大飞跃，意味着攻击者和防御者都能以远超人类能力的规模进行漏洞搜寻。此举可能重塑开源安全实践，并给维护者带来更大的快速修复压力。 NOVA 全称为 Network and Open-Source Vulnerability Analyzer（网络与开源漏洞分析器），被描述为一个基于专有 AI 框架、由多个领先模型驱动的智能体研究系统。该系统不仅能发现缺陷，还能对其进行验证，并生成可操作的报告。

rss · Unit 42 Threat Research · 8月4日 13:00

**背景**: 零日漏洞是指软件供应商尚不知晓、且没有可用补丁的安全缺陷，因此对网络犯罪利用和安全防御研究都具有极高价值。此前，大规模发现零日漏洞主要依赖人工代码审计、模糊测试和运气。开源软件是现代软件供应链的基石，因此能够自动扫描海量代码的系统具有巨大的安全影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://unit42.paloaltonetworks.com/frontier-ai-vulnerability-burst/">The Frontier AI Vulnerability Burst: Industrializing Autonomous...</a></li>

</ul>
</details>

**标签**: `#AI security`, `#vulnerability discovery`, `#zero-day`, `#open source`, `#supply chain`

---

<a id="item-18"></a>
## [Talos 通过对端点日志的分析揭示攻击者如何利用 AI 编程工具](https://blog.talosintelligence.com/keep-going-bro-youve-got-this-a-data-driven-look-at-how-adversaries-are-weaponizing-ai/) ⭐️ 8.0/10

Cisco Talos 收集并分析了运行 Claude Code、Codex、Cursor 和 Gemini 等云 AI 编程工具的攻击者端点上的提示词日志。这份基于数据的报告具体揭示了攻击者在实际操作中如何利用 AI。 这是首批针对真实敌对 AI 使用的实证研究之一，将讨论从猜测提升到了实际证据层面。它帮助安全社区了解新兴的攻击模式，并为抵御 AI 辅助的网络犯罪提供参考。 该分析涵盖了多种 AI 编程助手，包括 Anthropic 的 Claude Code、OpenAI 的 Codex、Cursor 和 Google 的 Gemini。提示词日志直接来自受感染或攻击者控制的端点，为观察攻击者行为提供了独特视角。

rss · Cisco Talos Blog · 8月4日 10:00

**背景**: Claude Code、Codex 和 Cursor 等基于云的 AI 编程工具是代理式助手，能够通过自然语言提示帮助开发者编辑文件、运行命令和理解代码库。随着这些工具在软件开发中日益普及，攻击者也在越来越多地利用它们来自动化恶意任务、编写漏洞利用代码或加速攻击。Talos 的报告正是通过检查威胁行为者实际使用的提示词来洞察这一趋势，为防御者提供了宝贵的情报。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://openai.com/codex/">Codex in ChatGPT | AI Coding Agents for Software ... - OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>

</ul>
</details>

**标签**: `#AI security`, `#threat intelligence`, `#adversarial AI`, `#LLM abuse`, `#cybersecurity`

---

<a id="item-19"></a>
## [Bugtraq 漏洞披露邮件列表回归](https://www.reddit.com/r/netsec/comments/1vfpmhg/bugtraq_is_back/) ⭐️ 8.0/10

传奇的 Bugtraq 漏洞披露邮件列表通过 Reddit 用户 /u/loselasso 的发帖宣布回归。目前细节不多，但这一公告确认了这一历史悠久的网络安全列表正在复活。 Bugtraq 曾是漏洞研究与披露的基础性渠道，其回归为安全研究人员和从业者提供了一个熟悉的共享和讨论漏洞的场所。这有助于复兴那种在现代平台中被碎片化的开放、社区驱动的漏洞披露文化。 该公告发布在 Reddit 的 r/netsec 社区，标题为“Bugtraq is back 🥹”，目前没有更多技术细节。Bugtraq 此前运行了 27 年才关闭，以厂商安全公告和漏洞利用讨论而闻名。

reddit · r/netsec · /u/loselasso · 8月4日 22:48

**背景**: Bugtraq 是最早且最有影响力的计算机安全电子邮件列表之一，内容涵盖漏洞、厂商公告、利用方法和修复方案。它后来先后归 SecurityFocus 和赛门铁克（Symantec）/博通（Broadcom）所有，并在运营 27 年后于 2020 年关闭。许多重大安全事件最初都是在 Bugtraq 和 Full-Disclosure 等类似列表上公布的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bugtraq">Bugtraq - Wikipedia</a></li>
<li><a href="https://www.zdnet.com/article/iconic-bugtraq-security-mailing-list-shuts-down-after-27-years/">Iconic BugTraq security mailing list shuts down after 27 years | ZDNET</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability disclosure`, `#bugtraq`, `#infosec`, `#mailing list`

---

<a id="item-20"></a>
## [硬件黑客指南：在亚马逊最畅销路由器上实现预认证栈溢出](https://www.reddit.com/r/netsec/comments/1vfdep6/hardware_hacking_from_zero_to_a_preauth_stack/) ⭐️ 8.0/10

一篇新的 Reddit 帖子提供了详细的硬件黑客操作指南，从物理分析开始，到在亚马逊最畅销路由器中发现并利用一个预认证的栈缓冲区溢出漏洞。该指南演示了攻击者如何在不提供任何凭据的情况下实现代码执行。 路由器无处不在且安全性往往较弱，畅销型号上的预认证溢出漏洞对许多家庭构成严重风险。该指南降低了安全研究人员学习硬件利用的门槛，可能促成更多物联网漏洞被发现和修复。 该指南包含了固件提取、UART 调试和漏洞分析等实践步骤，最终构造出预认证栈缓冲区溢出。该溢出在认证之前即可触达，意味着无需登录凭据即可远程触发。

reddit · r/netsec · /u/Internal-Key64 · 8月4日 15:21

**背景**: 硬件黑客（hardware hacking）是指通过物理方式接触设备来提取固件并寻找漏洞，常用技术包括 UART 和 JTAG。栈缓冲区溢出发生在向调用栈上的固定大小缓冲区写入超量数据时，可能覆盖返回地址，导致任意代码执行。'预认证'意味着漏洞在设备要求认证之前就能被触发，因此特别危险。亚马逊最畅销路由器是常见的物联网攻击目标，此类指南有助于研究人员理解设备的攻击方式并加强防护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ethicalhackinginstitute.com/blog/how-do-hackers-exploit-network-devices-like-routers-and-switches">How Do Hackers Exploit Network Devices Like Routers and ...</a></li>
<li><a href="https://github.com/adamhlt/TL-WR841N">GitHub - adamhlt/TL-WR841N: TL-WR841N Router Hardware Hacking ...</a></li>
<li><a href="https://labs.watchtowr.com/stack-overflows-heap-overflows-and-existential-dread-sonicwall-sma100-cve-2025-40596-cve-2025-40597-and-cve-2025-40598/">Stack Overflows, Heap Overflows, and Existential Dread (SonicWall ...</a></li>

</ul>
</details>

**标签**: `#security`, `#hardware hacking`, `#buffer overflow`, `#exploitation`, `#IoT`

---