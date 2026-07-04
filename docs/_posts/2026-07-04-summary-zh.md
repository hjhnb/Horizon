---
layout: default
title: "Horizon Summary: 2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> 从 68 条内容中筛选出 18 条重要资讯。

---

1. [调查间谍软件的欧洲议员遭 Pegasus 黑客攻击](#item-1)
2. [Bad Epoll Linux 漏洞使非特权用户获取 root 权限](#item-2)
3. [SearXNG：一款注重隐私的元搜索引擎](#item-3)
4. [本地运行顶级大模型的硬件指南](#item-4)
5. [工厂只是一个房间：思维转变](#item-5)
6. [Wordgard：ProseMirror 创建者推出的新富文本编辑器](#item-6)
7. [Ubicloud 为何对 PostgreSQL 使用严格内存过量提交](#item-7)
8. [开源 AI 差距地图收录 421 个项目](#item-8)
9. [HAT-4D：单目视频生成 4D 交互场景](#item-9)
10. [FatFs 库漏洞威胁数百万嵌入式设备](#item-10)
11. [朝鲜黑客利用伪造的 Rollup polyfill npm 包窃取开发者秘密](#item-11)
12. [NetNut 代理网络中断，200 万设备被切断](#item-12)
13. [Mistral 发布 Leanstral-1.5，顶级形式验证模型](#item-13)
14. [llama.cpp 推出散射采样器平滑 top-K 令牌](#item-14)
15. [新型 Avalon 恶意软件框架集成 CrownX 勒索软件功能](#item-15)
16. [Armored Likho 使用 BusySnake 窃密软件攻击政府和电力行业](#item-16)
17. [PamStealer 恶意软件利用虚假 Maccy 网站和 PAM 检查窃取密码](#item-17)
18. [ARToken 钓鱼即服务平台曝光 EvilTokens 的 Microsoft 365 钓鱼工具包](#item-18)

---

<a id="item-1"></a>
## [调查间谍软件的欧洲议员遭 Pegasus 黑客攻击](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 9.0/10

根据 Citizen Lab 的新报告，欧洲议会调查间谍软件的委员会的一名成员在 2022 年和 2023 年三次被 Pegasus 间谍软件入侵。 这一事件表明，国家支持的攻击者甚至敢于针对高级调查人员，凸显了商业间谍软件对民主机构和法治的普遍威胁。 感染发生在 2022 年 10 月 21 日和 2023 年 3 月 6 日至 7 日，第一次感染与针对欧洲流亡记者的已知 Pegasus 活动重叠，表明客户有权在多个欧洲国家进行间谍活动。

hackernews · ledoge · 7月3日 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: Pegasus 是以色列公司 NSO Group 开发的强大间谍软件，能够远程入侵移动设备，获取信息、通话、位置和摄像头。该软件仅出售给政府客户，并被以色列列为武器，但多次被滥用于针对全球记者、活动家和政治家。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/NSO_Group">NSO Group</a></li>

</ul>
</details>

**社区讨论**: 评论指出，希腊和其他欧盟国家此前曾滥用 Pegasus，有用户认为此次攻击可能源自欧盟内部而非外部。还有讨论涉及欧洲议会议员缺乏个人设备与工作设备的分离。

**标签**: `#cybersecurity`, `#espionage`, `#Pegasus`, `#European Parliament`, `#surveillance`

---

<a id="item-2"></a>
## [Bad Epoll Linux 漏洞使非特权用户获取 root 权限](https://thehackernews.com/2026/07/new-bad-epoll-linux-kernel-flaw-lets.html) ⭐️ 9.0/10

一个名为 Bad Epoll（CVE-2026-46242）的严重 Linux 内核漏洞被披露，该漏洞允许非特权本地用户在受影响系统（包括 Android 设备）上获取 root 权限。该缺陷是 epoll 子系统中的一个释放后使用（use-after-free）竞态条件，补丁已发布。 该漏洞之所以关键，是因为它影响 Linux 桌面、服务器和 Android 设备，可导致任意代码以 root 权限执行。由于 epoll 在高性能网络应用中广泛使用，影响范围可能非常巨大。 Bad Epoll 漏洞是一个释放后使用（use-after-free）的竞态条件，当多个线程并发操作 epoll 文件描述符时触发。在 kernelCTF 上利用的 130 多个漏洞中，只有大约十个适合用于 Android root 提权，而 Bad Epoll 就是其中之一。

rss · The Hacker News · 7月3日 19:40

**背景**: epoll 是 Linux 内核中用于可扩展 I/O 事件通知的系统调用，可监控多个文件描述符的 I/O 事件。它常用于高性能网络应用，如 Web 服务器和数据库系统。Bad Epoll 漏洞与 Anthropic 的 Mythos AI 近期发现的另一个 bug 位于同一内核代码区域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/new-bad-epoll-linux-kernel-flaw-lets.html">New " Bad Epoll " Linux Kernel Flaw Lets Unprivileged Users Gain Root...</a></li>
<li><a href="https://bitnewsbot.com/linux-bad-epoll-bug-grants-any-user/">Linux ' Bad Epoll ' Bug Grants Any User Root Access</a></li>
<li><a href="https://en.wikipedia.org/wiki/Epoll">epoll - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#Linux kernel`, `#vulnerability`, `#privilege escalation`, `#CVE`

---

<a id="item-3"></a>
## [SearXNG：一款注重隐私的元搜索引擎](https://github.com/searxng/searxng) ⭐️ 8.0/10

SearXNG 是一个开源的元搜索引擎，能在保护用户隐私的前提下聚合多个搜索引擎的结果，并在自托管和 AI 代理使用场景中获得了大量社区关注。 该工具提供了一种尊重隐私的集中式搜索引擎替代方案，其与 TinySearch 等 AI 代理的集成突显了它在本地模型中高效上下文检索方面的潜力。 SearXNG 支持 JSON 输出以便程序化使用，但用户可能会遇到搜索速度较慢以及来自 DuckDuckGo 或 Brave 等下游搜索引擎的偶尔验证码问题。

hackernews · theanonymousone · 7月3日 20:15 · [社区讨论](https://news.ycombinator.com/item?id=48779454)

**背景**: 元搜索引擎聚合多个搜索引擎的结果，而不是维护自己的索引。自托管意味着软件运行在用户自己的服务器上，从而完全控制数据和隐私。SearXNG 是早期 Searx 项目的分支，其原始创建者已离开该项目，转而采用不同的方法开发 Hister。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Metasearch_engine">Metasearch engine</a></li>
<li><a href="https://vibecodersdictionary.com/terms/s/self-hosted">Self - Hosted — Meaning , Examples & ELI5 | Vibecoder Dictionary</a></li>

</ul>
</details>

**社区讨论**: Searx 的原始创建者指出了元搜索概念的局限性，并引用了他们的新项目 Hister。一些用户表达了用许多小型跟踪器替换一个集中式跟踪器的担忧，而另一些用户则称赞该工具的日常可靠性及其在构建 RAG 应用中的用途。此外，TinySearch 被强调为一种能够优化 AI 代理上下文的集成方案。

**标签**: `#search engine`, `#privacy`, `#open-source`, `#metasearch`, `#self-hosted`

---

<a id="item-4"></a>
## [本地运行顶级大模型的硬件指南](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

Jamesob 发布了一份指南，介绍如何在本地运行最先进的大语言模型，并提供从约 3000 美元到超过 40000 美元（含 4 张 GPU）的硬件方案。 该指南帮助用户了解在家运行前沿 AI 模型的可行性与成本，对隐私保护、离线使用以及避免订阅费用具有重要意义。 高端方案需四块单价 12000 美元的 GPU，总成本约 5 万至 5.5 万美元，且常依赖量化来将模型装入内存，这会降低模型质量。

hackernews · livestyle · 7月3日 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 本地运行大语言模型需要大量显存；例如，约 300 亿参数的模型可能需要 48GB 显存。量化技术通过降低模型精度来减少内存占用，但会牺牲输出质量。另外还有统一内存架构（如 Apple M 系列）或云服务等替代方案。

**社区讨论**: 评论者警告本地搭建仍然非常昂贵，质量通常不如云 API，且可能存在安全风险（后门）。有人建议中等方案，如 48GB 统一内存的 Mac 或双 RTX 3090，并指出 4 万美元足以支付 16 年以上的 Claude Opus 订阅费用。

**标签**: `#LLM`, `#local`, `#hardware`, `#AI`, `#cost-analysis`

---

<a id="item-5"></a>
## [工厂只是一个房间：思维转变](https://interconnected.org/home/2026/07/03/factories) ⭐️ 8.0/10

一篇随笔提出，制造业不需要庞大的基础设施，工厂可以是像任何房间一样简单、可进入的空间。 这种观点可能使制造业民主化，让更多个人和小型企业能够本地生产商品，促进创新并降低进入门槛。 文章通过个人轶事和技术讨论挑战了工厂是庞大复杂设施的普遍认知。它强调，简化制造的关键不仅是技术，更是思维方式的转变。

hackernews · arbesman · 7月3日 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48776035)

**背景**: 传统上，工厂与大型建筑、重型机械和装配线联系在一起。这篇随笔反驳了这种说法，认为许多制造过程可以在更小、更灵活的空间中完成。这一概念与小规模制造和创客文化等趋势相符。

**社区讨论**: 评论分享了经营小型工厂的个人经历，并将快餐厨房比作高效的工厂。大家普遍认为制造业可以比通常假设的更简单，但有一条评论指出，简单的工厂并不保证商业成功。

**标签**: `#manufacturing`, `#mindset`, `#technology`, `#community discussion`

---

<a id="item-6"></a>
## [Wordgard：ProseMirror 创建者推出的新富文本编辑器](https://wordgard.net/) ⭐️ 8.0/10

Marijn Haverbeke（ProseMirror 的创建者）发布了 Wordgard 0.1，这是一个全新的浏览器端语义化富文本编辑器系统，融合了九年来 ProseMirror 开发的经验，并采用了重新设计的架构。 Wordgard 因其来自广受使用的编辑器框架 ProseMirror 的备受尊敬的作者而具有重要意义，它承诺提供更强大的编程接口来构建自定义编辑器，可能影响基于 Web 的富文本编辑的未来，并在 ProseMirror 用户中引发迁移讨论。 Wordgard 不是一个自由格式的 HTML 编辑器，而是一个语义化编辑器，让开发者精确控制内容结构。从 ProseMirror 没有直接的升级路径，迁移需要大量重构，因为许多概念共享但不完全相同。

hackernews · indy · 7月3日 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48772573)

**背景**: ProseMirror 是一个经过实战检验的 Web 语义化富文本编辑框架，被用作 Tiptap 等编辑器的核心。它提供了轻量级核心，但学习曲线陡峭。Wordgard 是同一位作者 Marijn Haverbeke 的新迭代版本，旨在解决限制并融合受 ProseMirror v6 重新设计启发的改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wordgard.net/">Wordgard</a></li>
<li><a href="https://marijnhaverbeke.nl/blog/wordgard-0.1.html">Wordgard Release 0.1</a></li>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**社区讨论**: 社区表现出浓厚兴趣，许多人询问 Wordgard 背后的动机及其与 ProseMirror 的差异。用户指出缺乏升级路径，并称赞其设计。一些人讨论了 ProseMirror 中静态类型化的挑战以及 Wordgard 方法的潜在优势。

**标签**: `#rich-text-editor`, `#web-development`, `#prosemirror`, `#javascript`, `#open-source`

---

<a id="item-7"></a>
## [Ubicloud 为何对 PostgreSQL 使用严格内存过量提交](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud 发布了一篇博客文章，详细解释了为何将 Linux 配置为严格内存过量提交（vm.overcommit_memory=2），以防止 OOM killer 终止 PostgreSQL 进程。 这对数据库管理员很重要，因为不当的内存过量提交设置可能导致 PostgreSQL 在内存压力下崩溃，引发停机或数据丢失。Ubicloud 的建议为提高数据库可靠性提供了实用策略。 在严格过量提交模式（vm.overcommit_memory=2）下，内核拒绝超过 RAM 和交换空间总和的分配。这防止了 OOM killer 的运行，但可能导致内存紧张时进程 fork 失败。文章警告该设置应在非生产环境中充分测试。

hackernews · furkansahin · 7月3日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48774509)

**背景**: Linux 默认使用内存过量提交（vm.overcommit_memory=0），允许进程分配超过物理 RAM 的虚拟内存。当内存耗尽时，OOM killer 会终止进程以释放内存，这可能会意外杀死 PostgreSQL。将 vm.overcommit_memory 设置为 2 会禁用过量提交，因此内核拒绝超过可用内存的分配，防止 OOM killer 触发，但要求应用程序妥善处理分配失败。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baeldung.com/linux/overcommit-modes">Linux Overcommit Modes - Baeldung Overcommit Accounting — The Linux Kernel documentation Overcommit Accounting — The Linux Kernel documentation How to check if kernel overcommit is enabled in Linux | LabEx What is vm.overcommit_memory parameter? - Red Hat Customer Portal How to Optimize Memory (vm.swappiness, overcommit) on Ubuntu</a></li>
<li><a href="https://access.redhat.com/solutions/68612">What is vm.overcommit_memory parameter? - Red Hat Customer Portal</a></li>
<li><a href="https://linuxhandbook.com/oom-killer/">What is Out of Memory Killer (OOM Killer) in Linux?</a></li>

</ul>
</details>

**社区讨论**: 社区评论既表示支持也提醒谨慎。一些用户报告模式 2 稳定了 PostgreSQL，但可能导致分配大量虚拟内存的应用程序出现问题。其他人强调在预发布环境中测试设置并仔细调整过量提交比例的重要性。博客作者也承认标题过于强烈，模式 2 可能不适用于所有场景。

**标签**: `#PostgreSQL`, `#OOM killer`, `#memory management`, `#Linux`, `#database operations`

---

<a id="item-8"></a>
## [开源 AI 差距地图收录 421 个项目](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

非营利组织 Current AI 在巴黎人工智能行动峰会上成立，发布了开源 AI 差距地图 v0.1，该地图索引了来自 228 家组织的 421 个开源 AI 产品（包括 266 个软件工具、85 个模型、50 个数据集和 20 个硬件项目），以及超过 24,000 个其他工件。 这份全面的地图提供了开源 AI 生态系统急需的概览，帮助开发者、研究人员和政策制定者识别差距和机遇。它凸显了公益 AI 基础设施投资的增长，Current AI 已获得 4 亿美元承诺。 该地图将产品分为 14 个类别，涵盖三个层次：模型组件、产品/用户体验和基础设施。底层数据以 MIT 许可证发布在 GitHub 上，包含 1,184 个 YAML 文件及模式文件和笔记；可通过 Datasette Lite 进行探索。

rss · Simon Willison · 7月3日 22:04

**背景**: Current AI 于 2025 年 2 月在巴黎人工智能行动峰会上作为全球非营利合作伙伴成立，已获得超过 4 亿美元承诺，目标是在五年内筹集 25 亿美元。差距地图旨在系统性地编录开源 AI 项目，以了解当前格局并识别资源不足的领域。人工智能行动峰会聚集了 100 多个国家，讨论道德和可持续的 AI 发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.currentai.org/">Current AI | Building Public Interest AI Technology Together</a></li>
<li><a href="https://www.multiminds.eu/news/ai-action-summit-paris-global-talk-with-local-impact/">AI Action Summit Paris : global talk with local impact | MultiMinds</a></li>

</ul>
</details>

**标签**: `#open source`, `#AI`, `#ecosystem mapping`, `#Current AI`

---

<a id="item-9"></a>
## [HAT-4D：单目视频生成 4D 交互场景](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247901356&idx=3&sn=54ee94026f76691a380cd3ea214e0def) ⭐️ 8.0/10

上海交通大学等机构提出 HAT-4D 框架，能够从单目视频中重建 4D 多物体交互场景，有望替代昂贵的百万级动捕棚。 这一突破降低了 4D 场景捕捉的门槛，让无法承担高昂动捕设备的创作者、游戏开发者和研究人员也能使用，并为 AR/VR、影视和机器人领域带来新可能。 HAT-4D 利用视觉语言模型（VLM）智能体构建交互知识图谱（IKG），编码长期物理变化和交互线索，能处理单目视频中常见的严重遮挡和深度模糊问题。

rss · 量子位 · 7月3日 03:43

**背景**: 传统的 4D 场景重建需要昂贵的多相机系统或动捕棚。单目视频 4D 重建因深度模糊、遮挡和复杂运动而极具挑战。HAT-4D 采用智能体方法，利用 VLM 进行场景理解来解决这些问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2606.28215v1">HAT-4D: Lifting Monocular Video for 4D Multi-Object ...</a></li>
<li><a href="https://github.com/Lijiaxin0111/HAT-4D-Lifting-Monocular-Video-for-4D-Multi-Object-Interactions-via-Human-Agent-Collaboration/tree/main/">Lijiaxin0111/HAT-4D-Lifting-Monocular-Video-for-4D ... - GitHub</a></li>

</ul>
</details>

**标签**: `#4D reconstruction`, `#monocular video`, `#computer vision`, `#AI research`, `#Shanghai Jiao Tong University`

---

<a id="item-10"></a>
## [FatFs 库漏洞威胁数百万嵌入式设备](https://thehackernews.com/2026/07/unpatched-flaws-disclosed-in-filesystem.html) ⭐️ 8.0/10

安全公司 runZero 披露了 FatFs 文件系统库中的七个未修补漏洞，该库被用于数百万嵌入式设备中。 这些漏洞影响大量设备，因为 FatFs 广泛嵌入在安全摄像头、无人机、工业控制器和加密钱包中，可能允许攻击者破坏设备操作。 这些漏洞允许在设备读取恶意构造的 FAT/exFAT 文件系统时执行远程代码或拒绝服务。目前尚未发布补丁，使得许多设备面临风险。

rss · The Hacker News · 7月3日 20:19

**背景**: FatFs 是一个用于嵌入式系统的小型可移植文件系统库，支持 FAT/exFAT 格式。由于其内存占用小，被用于许多低功耗设备。该库通常嵌入固件中，缺乏更新机制，使得修补困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/FatFs">FatFs - Wikipedia</a></li>
<li><a href="https://elm-chan.org/fsw/ff/">FatFs - Generic FAT Filesystem Module</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerabilities`, `#embedded systems`, `#FatFs`, `#runZero`

---

<a id="item-11"></a>
## [朝鲜黑客利用伪造的 Rollup polyfill npm 包窃取开发者秘密](https://thehackernews.com/2026/07/north-korea-linked-npm-packages-mimic.html) ⭐️ 8.0/10

与朝鲜有关的威胁行为者发布了两个恶意 npm 包，名为 'rollup-packages-polyfill-core' 和 'rollup-runtime-polyfill-core'，它们冒充合法的 'rollup-plugin-polyfill-node' 项目，以窃取开发者凭据并实现远程访问。 此次攻击针对 npm 软件供应链，可能使众多无意中安装恶意包的项目受损，并表明国家背景的攻击者在模仿合法开源工具方面的日益成熟。 这些恶意包由 JFrog 发现，它们高度模仿合法的 Rollup polyfill 插件，包括其描述、仓库元数据和结构，使得不经仔细检查很难区分。

rss · The Hacker News · 7月3日 16:07

**背景**: Rollup 是一个 JavaScript 模块打包工具，而 polyfill 是提供较旧环境中缺失功能的代码片段。npm 供应链攻击涉及将恶意代码插入开发者下载的包中，这些代码可以随后传播到依赖项目中。类似的攻击（如 2025 年 9 月的 Shai-Hulud 事件）凸显了 npm 生态系统日益增长的威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/north-korea-linked-npm-packages-mimic.html">North Korea-Linked npm Packages Mimic Rollup Polyfills to ...</a></li>
<li><a href="https://www.npmjs.com/package/rollup-plugin-polyfill-node">rollup-plugin-polyfill-node - npm</a></li>
<li><a href="https://unit42.paloaltonetworks.com/monitoring-npm-supply-chain-attacks/">The npm Threat Landscape: Attack Surface and Mitigations (Updated June 2)</a></li>

</ul>
</details>

**标签**: `#security`, `#npm`, `#supply-chain-attack`, `#north-korea`, `#malicious-packages`

---

<a id="item-12"></a>
## [NetNut 代理网络中断，200 万设备被切断](https://www.bleepingcomputer.com/news/security/netnut-proxy-network-disrupted-2-million-infected-devices-cut-off/) ⭐️ 8.0/10

一项涉及谷歌和执法部门的联合行动中断了 NetNut 住宅代理网络，切断了约 200 万台受感染 Android 设备（包括智能电视和流媒体盒子）的访问。 这次中断消除了网络犯罪分子用来通过住宅 IP 匿名化其活动的主要工具，并凸显了针对僵尸网络和代理网络的联合打击行动的有效性。 NetNut 网络与 Popa 僵尸网络有关，该僵尸网络向智能电视和流媒体盒子等消费设备分发恶意软件；FBI 于 2026 年 6 月 19 日查封了该平台。

rss · BleepingComputer · 7月3日 17:50

**背景**: 住宅代理网络通过真实的住宅 IP 地址路由互联网流量，使恶意活动看起来合法。它们通常用于网络爬取和广告欺诈，但也常被网络犯罪分子用来隐藏踪迹。像 NetNut 这样的服务从受感染的设备获取 IP，而用户并不知情。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://krebsonsecurity.com/2026/07/fbi-seizes-netnut-proxy-platform-popa-botnet/">FBI Seizes NetNut Proxy Platform, Popa Botnet – Krebs on Security</a></li>
<li><a href="https://www.fbi.gov/investigate/cyber/alerts/2026/evading-residential-proxy-networks-protecting-your-devices-from-becoming-a-tool-for-criminals">Evading Residential Proxy Networks: Protecting Your Devices from Becoming a Tool for Criminals | Federal Bureau of Investigation</a></li>
<li><a href="https://netnut.io/">NetNut - High Quality Proxies Network For Web Data Collection</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#botnet`, `#Android`, `#proxy network`, `#malware`

---

<a id="item-13"></a>
## [Mistral 发布 Leanstral-1.5，顶级形式验证模型](https://www.reddit.com/r/LocalLLaMA/comments/1umgdhx/mistral_released_leanstral15119ba6b/) ⭐️ 8.0/10

Mistral 发布了 Leanstral-1.5-119B-A6B，采用 Apache-2.0 许可，仅 6.5B 活跃参数，在 miniF2F、PutnamBench、FATE-H（87%）和 FATE-X（34%）等正式验证基准上达到最优水平。该模型还在 57 个代码仓库中发现了 5 个此前未知的 bug。 该模型通过开源许可和高效架构使先进的形式验证技术更易于普及，有望在实际应用中提升软件可靠性和自动定理证明能力。 Leanstral-1.5 拥有 119B 总参数但每次推理仅激活 6.5B，采用混合专家（MoE）架构。训练采用三阶段流程：中间训练、监督微调以及使用 CISPO 算法的强化学习，CISPO 通过裁剪重要性采样权重实现稳定训练。

reddit · r/LocalLLaMA · /u/Tall-Ad-7742 · 7月3日 14:44

**背景**: 形式验证是通过数学手段证明软件或硬件满足其形式化规范的过程，能捕捉传统测试可能遗漏的缺陷。Lean 是一种交互式定理证明器，用于编写和验证数学证明与代码。CISPO（Clipped Importance Sampling Policy Optimization）是一种强化学习算法，通过裁剪重要性采样权重来提高训练稳定性，与 PPO 等方法不同。FATE 基准系列评估模型在不同难度级别的代数定理证明能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.mistral.ai/models/model-cards/leanstral-1-5">Leanstral 1.5 - Mistral AI | Mistral Docs</a></li>
<li><a href="https://www.emergentmind.com/topics/cispo-algorithm">CISPO: Clipped Importance Sampling RL - emergentmind.com</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#theorem proving`, `#Mistral`, `#AI models`, `#open-source`

---

<a id="item-14"></a>
## [llama.cpp 推出散射采样器平滑 top-K 令牌](https://www.reddit.com/r/LocalLLaMA/comments/1umqgnl/particle_scattering_sampler_for_llamacpp/) ⭐️ 8.0/10

llama.cpp 新增了一项实验性散射采样器，它在排名靠前的令牌之间局部平滑概率分布，从而在不提升尾部概率的情况下减少生成结果的刻板性。 与调整温度相比，该技术提供了对 LLM 创造性的更精细控制，有望在不牺牲多样性的前提下提升需要连贯性的任务的输出质量。 散射采样器在令牌排名上应用高斯核，在邻近排名之间交换概率质量，并可通过可选的碰撞门控以一定概率生效；它被放置在 top-k、min-p 等过滤采样器之后。

reddit · r/LocalLLaMA · /u/Pristine_Income9554 · 7月3日 21:19

**背景**: llama.cpp 是一个开源的 C/C++ 实现，用于在消费级硬件上高效运行 LLM 推理。采样是在生成过程中选择下一个令牌的机制；常见的采样器如温度和 top-k 通过修改模型的输出分布来控制随机性和连贯性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml-org/llama.cpp: LLM inference in C/C++</a></li>
<li><a href="https://deepwiki.com/ggml-org/llama.cpp/2.3-configuration-and-parameters">Configuration and Parameters | ggml-org/llama.cpp | DeepWiki</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#sampling`, `#local-llm`, `#inference`, `#generative-ai`

---

<a id="item-15"></a>
## [新型 Avalon 恶意软件框架集成 CrownX 勒索软件功能](https://thehackernews.com/2026/07/new-avalon-malware-framework-packs.html) ⭐️ 7.0/10

Blackpoint Cyber 的研究人员发现了一个此前未记录的模块化恶意软件框架 Avalon，它通过多阶段钓鱼链传播，并集成了 CrownX 勒索软件功能。 Avalon 将凭证窃取、横向移动和勒索软件整合在一个框架中，代表了攻击复杂性的显著升级，能够绕过传统安全控制。 该恶意软件使用 Proton Drive、ISO 镜像、LNK 文件和 MSBuild 来禁用 Windows 事件跟踪（ETW）、窃取凭证并部署 CrownX 勒索软件，此外还具有恢复破坏和远程访问功能。

rss · The Hacker News · 7月3日 18:55

**背景**: 模块化恶意软件框架是一种工具包，允许攻击者根据需要选择和组合不同的功能模块（如凭证窃取、横向移动、勒索软件）。多阶段钓鱼链使用一系列电子邮件或诱饵逐步交付有效载荷，通过不在单一步骤中暴露全部意图来逃避检测。Avalon 的模块化特性使其能适应多种攻击场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/new-avalon-malware-framework-packs.html">New Avalon Malware Framework Packs CrownX Ransomware Capabilities</a></li>
<li><a href="https://blackpointcyber.com/blog/avalons-path-from-legal-lure-to-crownx-ransom-capabilities/">Vibe Coded Extortion: Avalon’s Path from Legal Lure to CrownX ...</a></li>
<li><a href="https://news.shield53.com/avalon-malware-framework-when-ransomware-becomes-a-swiss-army-knife/">Avalon Malware Framework: When Ransomware Becomes a Swiss ...</a></li>

</ul>
</details>

**标签**: `#malware`, `#cybersecurity`, `#ransomware`, `#phishing`, `#framework`

---

<a id="item-16"></a>
## [Armored Likho 使用 BusySnake 窃密软件攻击政府和电力行业](https://thehackernews.com/2026/07/armored-likho-targets-government.html) ⭐️ 7.0/10

卡巴斯基发现了一个此前未被记录的威胁行为者 Armored Likho，该组织使用名为 BusySnake 的新型基于 Python 的窃密恶意软件，针对俄罗斯、巴西和哈萨克斯坦的政府机构和电力行业。 这一发现突显了以经济为目的的网络犯罪与国家支持的间谍活动日益融合，对多个国家的基础设施构成严重风险。网络安全专业人员必须相应更新其威胁模型和防御措施。 Armored Likho 将针对个人的金融动机攻击与针对组织的定向网络间谍活动相结合，使用鱼叉式钓鱼邮件和 AI 生成的加载器。BusySnake 是一种基于 Python 的窃密程序，旨在从受感染的系统中窃取敏感数据。

rss · The Hacker News · 7月3日 13:36

**背景**: 威胁行为者是指实施网络攻击的个人或团体，其动机从经济收益到政治间谍活动不等。BusySnake 是一种信息窃取型恶意软件，能够秘密从受感染设备中提取凭据、文件和其他敏感信息。此次攻击针对政府和能源等关键行业，表明对手具有复杂的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/armored-likho-targets-government.html">Armored Likho Targets Government Agencies, Power Sector with BusySnake Stealer</a></li>
<li><a href="https://www.itsecuritynews.info/armored-likho-digging-a-snake-pit-inside-the-covert-busysnake-stealer-campaign/">Armored Likho digging a snake pit: inside the covert BusySnake ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#threat actor`, `#government`, `#espionage`, `#malware`

---

<a id="item-17"></a>
## [PamStealer 恶意软件利用虚假 Maccy 网站和 PAM 检查窃取密码](https://thehackernews.com/2026/07/pamstealer-uses-fake-maccy-sites-and.html) ⭐️ 7.0/10

网络安全研究人员 Jamf 威胁实验室发现了一种名为 PamStealer 的新型 macOS 信息窃取器，该恶意软件通过冒充 Maccy 剪贴板管理器的虚假网站分发，并利用可插入认证模块（PAM）验证并窃取登录密码。 该恶意软件通过使用 PAM 检查验证密码而不生成外部进程，展示了一种先进的技术，使其比典型的 macOS 窃取器更隐蔽。这凸显了 macOS 威胁的日益复杂化，以及用户验证软件来源的必要性。 PamStealer 分两个阶段投递：首先是一个磁盘映像中的编译版 AppleScript（.scpt）文件，然后是后续载荷。它完全通过 PAM 进行密码验证，无需调用 dscl、security 或 osascript 等进程，这在 macOS 恶意软件中较为罕见。

rss · The Hacker News · 7月3日 08:03

**背景**: Maccy 是一款合法的 macOS 开源剪贴板管理器，用于存储复制历史。PAM（可插入认证模块）是 macOS 用于认证的框架，允许应用程序在无需生成独立进程的情况下验证密码。通过利用 PAM，PamStealer 可以在不引起进程监控怀疑的情况下检查窃取的密码是否正确，从而更难被检测到。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/pamstealer-uses-fake-maccy-sites-and.html">PamStealer Uses Fake Maccy Sites and PAM Checks to Steal Mac ...</a></li>
<li><a href="https://arstechnica.com/security/2026/07/new-pamstealer-macos-malware-uses-clever-tradecraft-to-remain-stealthy/">Newly discovered PamStealer isn’t your typical macOS malware</a></li>

</ul>
</details>

**标签**: `#macOS`, `#malware`, `#cybersecurity`, `#information stealer`

---

<a id="item-18"></a>
## [ARToken 钓鱼即服务平台曝光 EvilTokens 的 Microsoft 365 钓鱼工具包](https://www.bleepingcomputer.com/news/security/artoken-phaas-exposes-eviltokens-microsoft-365-phishing-toolkit/) ⭐️ 7.0/10

一个名为 ARToken 的新型钓鱼即服务（PhaaS）平台被发现，它作为 EvilTokens 钓鱼工具包的关联方，专门针对 Microsoft 365 用户。研究人员得以深入了解其广泛的功能，包括设备代码钓鱼和绕过多重身份验证（MFA）。 这一发现凸显了能够绕过 MFA 的 PhaaS 平台日益复杂化，对依赖 Microsoft 365 的组织构成重大威胁。它强调了需要先进的检测手段和用户意识来应对此类凭证窃取技术。 ARToken 与 EvilTokens（一个自 2026 年 2 月起就在 Telegram 上推广的设备代码钓鱼工具包）共享基础设施和运营模式。该平台利用 Cloudflare Workers 和伪造的 SharePoint 租户，诱骗用户在真实的 Microsoft 登录页面上进行身份验证，从而有效绕过 MFA。

rss · BleepingComputer · 7月3日 14:12

**背景**: 钓鱼即服务（PhaaS）平台为网络犯罪分子提供现成的工具来开展钓鱼活动，降低了技术门槛。设备代码钓鱼是一种攻击者诱骗受害者在合法认证页面上输入设备代码的技术，常用于混合身份环境。EvilTokens 专门利用这种方法入侵 Microsoft 365 账户而无需窃取密码。ARToken 作为其关联面板的曝光，让人们罕见地一窥这种复杂钓鱼操作的内部运作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/artoken-phaas-exposes-eviltokens-microsoft-365-phishing-toolkit/">ARToken PhaaS exposes EvilTokens' Microsoft 365 phishing toolkit</a></li>
<li><a href="https://blog.talosintelligence.com/artoken-inside-an-eviltokens-affiliate-panel-targeting-microsoft-365/">ARToken: Inside an EvilTokens affiliate panel targeting Microsoft 365</a></li>

</ul>
</details>

**标签**: `#phishing`, `#cybersecurity`, `#Microsoft 365`, `#PhaaS`, `#threat intelligence`

---