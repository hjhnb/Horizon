---
layout: default
title: "Horizon Summary: 2026-07-18 (ZH)"
date: 2026-07-18
lang: zh
---

> 从 51 条内容中筛选出 20 条重要资讯。

---

1. [OpenWrt 曝出严重预认证远程 root 漏洞](#item-1)
2. [Moonshot AI 发布 Kimi K3：最大开源模型，2.8 万亿参数](#item-2)
3. [WordPress 核心严重 wp2shell 远程代码执行漏洞已修复](#item-3)
4. [欧盟命令谷歌向竞争对手 AI 助手开放安卓硬件](#item-4)
5. [CISA 将已遭利用的 SharePoint RCE 零日漏洞加入 KEV](#item-5)
6. [新的 LegacyHive 零日漏洞可让攻击者获得 Windows 管理员权限](#item-6)
7. [CISA 下令修补被利用的 Fortinet 漏洞](#item-7)
8. [在宜居带岩质系外行星上首次探测到大气层](#item-8)
9. [实用 SQLite 技巧：专家模式、备份与凭证管理](#item-9)
10. [社区指责 Kaggle 竞赛中 AI 评审和 AI 提交的漏洞](#item-10)
11. [OpenSSL HollowByte 漏洞通过 11 字节 TLS 请求冻结内存](#item-11)
12. [恶意 Vite npm 包利用区块链 C2](#item-12)
13. [新 NadMesh 僵尸网络瞄准暴露的 AI 服务窃取云凭证](#item-13)
14. [GoldenEyeDog 子团伙与 DigiCert 入侵事件关联](#item-14)
15. [朝鲜黑客在假编码测试中使用 SVG 隐写术](#item-15)
16. [Windows AppResolver 提权：从 AppContainer 到 SYSTEM 的 PoC](#item-16)
17. [Kaiser 护士批评 AI 和监控影响医护质量](#item-17)
18. [Kimi K3 与鹈鹕基准测试的启示](#item-18)
19. [Mozilla 报告分析开源 AI 增长与争论](#item-19)
20. [实时 SSH 蜜罐可视化走红](#item-20)

---

<a id="item-1"></a>
## [OpenWrt 曝出严重预认证远程 root 漏洞](https://www.reddit.com/r/netsec/comments/1uz8qh3/openwrt_preauth_remote_root_exploit/) ⭐️ 10.0/10

一个针对 OpenWrt 的预认证远程 root 漏洞已被公开披露，攻击者无需任何凭据即可获得完全的系统访问权限。 这是一个关键安全漏洞，潜在影响广泛，因为 OpenWrt 运行在数百万台路由器和嵌入式设备上，无需认证的远程代码执行可导致设备完全沦陷。 该漏洞无需认证即可利用，无需登录或凭据，且提供 root 权限，即系统最高权限。帖子未详细说明具体漏洞向量。

reddit · r/netsec · /u/supernetworks · 7月17日 18:56

**背景**: OpenWrt 是一个基于 Linux 的开源操作系统，主要用于无线路由器和接入点等嵌入式设备。它提供完全可写的文件系统和包管理功能，允许广泛定制。由于其广泛用于网络基础设施设备，安全漏洞可能对家庭和企业网络造成严重后果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenWrt">OpenWrt</a></li>
<li><a href="https://openwrt.org/">[OpenWrt Wiki] Welcome to the OpenWrt Project</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#OpenWrt`, `#exploit`, `#remote code execution`

---

<a id="item-2"></a>
## [Moonshot AI 发布 Kimi K3：最大开源模型，2.8 万亿参数](https://www.latent.space/p/ainews-kimi-k3-28t-a50b-the-largest) ⭐️ 9.0/10

Moonshot AI 发布了 Kimi K3，这是一个拥有 2.8 万亿参数、50 亿活跃参数的开源语言模型，声称在性能上与 GPT-5.6 和 Claude Opus 等顶尖模型相当，而定价则与 Sonnet 级别持平。 这标志着开源 AI 领域的一个重要里程碑，因为它是迄今为止发布的最大开源模型，可能使高性能 AI 的获取更加民主化，并挑战美国在该领域的主导地位。 Kimi K3 采用混合专家（MoE）架构，总参数 2.8 万亿，其中活跃参数为 50 亿，其定价与 Anthropic 的 Sonnet 模型相当，而在多项基准测试中性能接近 Opus 水平。

rss · Latent Space · 7月17日 01:46

**背景**: Moonshot AI 是一家成立于 2023 年的北京初创公司，由清华大学校友创立，专注于推进 AGI。像 Kimi K3 这样的大型语言模型通过在大量文本数据上训练，能够执行各种任务。开源模型允许任何人使用、修改和分发该技术，从而促进创新并减少对专有系统的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/17/moonshot-ai-kimi-k3-model-openai-anthropic-china.html">China's Moonshot AI unveils Kimi K3 that rivals OpenAI, Anthropic</a></li>
<li><a href="https://www.nytimes.com/2026/07/17/business/china-ai-moonshot-kimi.html">China’s Moonshot AI Unveils Kimi Model, Threatening ...</a></li>
<li><a href="https://www.geeky-gadgets.com/moonshot-ai-kimi-k3-review/">Kimi K3 Open Source AI Rivals GPT 5.6 Sol with 2.8T ...</a></li>

</ul>
</details>

**标签**: `#open model`, `#AI`, `#large language model`, `#Kimi K3`, `#Moonshot AI`

---

<a id="item-3"></a>
## [WordPress 核心严重 wp2shell 远程代码执行漏洞已修复](https://thehackernews.com/2026/07/new-wp2shell-wordpress-core-flaw-lets.html) ⭐️ 9.0/10

WordPress 核心版本 6.9 和 7.0 中发现了一个名为 wp2shell 的未认证远程代码执行漏洞。WordPress 于周五发布了紧急补丁 6.9.5 和 7.0.2，并启用了强制自动更新以将修复推送到所有受影响站点。 该漏洞允许任何匿名攻击者在没有任何插件的默认 WordPress 安装上执行任意代码，影响了运行这两个最新主要版本的数百万个站点。立即打补丁对于防止大规模利用至关重要。 该漏洞是一个预认证 SQL 注入，导致远程代码执行，由 Assetnote 的 Adam Kues 确认。即使是没有任何插件的干净 WordPress 安装也可以被利用，使其成为近年来最严重的内核漏洞之一。

rss · The Hacker News · 7月17日 21:20

**背景**: WordPress 是全球最流行的内容管理系统，驱动着超过 40%的网站。内核漏洞意味着该缺陷存在于 WordPress 基础软件本身，而非插件或主题中。未认证远程代码执行（RCE）允许攻击者无需任何登录凭证即可完全控制服务器。强制自动更新是 WordPress 的一种机制，即使网站管理员禁用了自动更新，也会自动推送安全更新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/new-wp2shell-wordpress-core-flaw-lets.html">New wp2shell WordPress Core Flaw Lets Unauthenticated Attackers Run Code</a></li>
<li><a href="https://www.aikido.dev/blog/unauthenticated-rce-in-wordpress-wp2shell">Unauthenticated RCE in WordPress core (wp2shell). Patch now!</a></li>
<li><a href="https://www.cyberkendra.com/2026/07/wp2shell-critical-wordpress-flaw-lets.html">WP2Shell: Critical WordPress Flaw Lets Anyone Run Code</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#wordpress`, `#rce`, `#cve`

---

<a id="item-4"></a>
## [欧盟命令谷歌向竞争对手 AI 助手开放安卓硬件](https://thehackernews.com/2026/07/eu-orders-google-to-open-android-mic.html) ⭐️ 9.0/10

欧盟委员会命令谷歌允许竞争对手的 AI 助手平等访问安卓的摄像头、麦克风、屏幕内容、熄屏唤醒词以及通过模拟点击和打字来控制后台应用，这些功能将在 Android 18 中实施，最迟于 2027 年 8 月 1 日生效。 这一里程碑式的监管行动可能打破谷歌在安卓 AI 助手市场的主导地位，促进竞争并为用户提供更多选择。它开创了平台持有者如何在欧盟数字竞争规则下对待第三方服务的先例。 谷歌必须在下一个主要版本 Android 18 中实施这些变更，最迟于 2027 年 8 月 1 日完成。该命令涵盖硬件访问（摄像头、麦克风）、屏幕内容、熄屏时的唤醒词激活，以及通过模拟点击和打字来控制其他后台应用的能力。

rss · The Hacker News · 7月17日 11:44

**背景**: 欧盟委员会一直在执行《数字市场法案》（DMA），以确保数字市场的公平竞争。安卓是全球最流行的移动操作系统，而谷歌的 Gemini 助手目前拥有对系统功能的特权访问。该命令旨在为 Alexa 或 Siri 等第三方 AI 助手创造公平的竞争环境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/develop/background-work/background-tasks/awake">Choose the right API to keep the device awake | Background work | Android Developers</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#Android`, `#AI assistants`, `#antitrust`, `#mobile ecosystem`

---

<a id="item-5"></a>
## [CISA 将已遭利用的 SharePoint RCE 零日漏洞加入 KEV](https://thehackernews.com/2026/07/cisa-adds-exploited-sharepoint-rce-zero.html) ⭐️ 9.0/10

CISA 将 CVE-2026-58644（一个影响 Microsoft SharePoint Server 的关键反序列化远程代码执行漏洞）添加到其已知被利用漏洞（KEV）目录中，要求联邦机构在 2026 年 7 月 19 日前应用补丁。 这非常关键，因为该漏洞已被积极利用，且 CVSS 评分为 9.8，对联邦网络构成直接威胁，如果未及时修补，可能对使用 SharePoint 的组织产生广泛影响。 该漏洞是 Microsoft SharePoint Server 中的一个反序列化缺陷，CVSS 评分为 9.8。CISA 要求联邦民事行政分支机构在 2026 年 7 月 19 日前应用修复。

rss · The Hacker News · 7月17日 06:42

**背景**: 已知被利用漏洞（KEV）目录是由 CISA 维护的权威列表，用于识别已被确认在现实攻击中利用的漏洞，帮助组织优先进行修复。反序列化漏洞发生在应用程序反序列化不可信数据时，可能允许攻击者执行任意代码，导致系统完全受损。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cvefeed.io/cisakev/cisa-known-exploited-vulnerability-catalog">CISA Known Exploited Vulnerabilities (KEV) – CVEFeed Catalog</a></li>
<li><a href="https://portswigger.net/web-security/deserialization">Insecure deserialization | Web Security Academy</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#CISA`, `#SharePoint`, `#zero-day`, `#RCE`

---

<a id="item-6"></a>
## [新的 LegacyHive 零日漏洞可让攻击者获得 Windows 管理员权限](https://www.bleepingcomputer.com/news/security/new-windows-legacyhive-zero-day-exploit-grants-hackers-admin-access/) ⭐️ 9.0/10

安全研究员 Nightmare Eclipse 发布了一个名为 LegacyHive 的概念验证漏洞利用程序，瞄准 Windows 用户配置文件服务中的一个零日漏洞，可在已完全修补的 Windows 系统上将权限提升至管理员级别。 这一点至关重要，因为它为攻击者提供了一种可靠的方法，即使在最新更新的 Windows 系统上也能获得完全系统访问权限，对企业安全构成严重威胁，需要立即采取防御措施。 该漏洞（MSNightmare）利用了 Windows 加载用户 usrClass.dat 文件时访问控制执行不一致的问题，具体涉及 HKEY_CURRENT_USER\Classes 注册表配置单元，从而实现隐秘的权限提升。

rss · BleepingComputer · 7月17日 11:05

**背景**: Windows 用户配置文件服务（ProfSvc）管理用户账户和环境。每个用户都有一个配置文件，其中包含存储在注册表配置单元中的设置和文件关联。LegacyHive 漏洞利用该服务加载 usrClass.dat 配置单元时的缺陷，允许拥有有限访问权限的攻击者加载恶意配置单元，从而获得管理员级别的代码执行权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/windows-legacyhive-0-day-vulnerability/">New Windows LegacyHive 0-Day Vulnerability Allow Hackers to Gain Admin ...</a></li>
<li><a href="https://cyberpress.org/legacyhive-windows-zero-day/">LegacyHive Windows Zero-Day Lets Attackers Hijack Administrator ...</a></li>
<li><a href="https://thehackernews.com/2026/07/researcher-drops-new-windows-zero-day.html">Researcher Drops New Windows Zero-Day PoC Hours After Microsoft Patch ...</a></li>

</ul>
</details>

**标签**: `#security`, `#zero-day`, `#Windows`, `#privilege escalation`, `#vulnerability`

---

<a id="item-7"></a>
## [CISA 下令修补被利用的 Fortinet 漏洞](https://www.bleepingcomputer.com/news/security/cisa-warns-feds-to-patch-exploited-fortinet-fortisandbox-flaws-by-sunday/) ⭐️ 9.0/10

CISA 发布指令，要求联邦机构在周日之前修补 Fortinet FortiSandbox 中两个已被积极利用的漏洞。 这凸显了未修补的 FortiSandbox 漏洞的严重风险，这些漏洞已被积极利用于攻击，并为联邦机构设定了严格的合规截止日期。 这两个漏洞具体存在于 FortiSandbox（一个可与其他安全工具集成的威胁检测平台）中，CISA 要求必须在周日之前完成修补。

rss · BleepingComputer · 7月17日 07:03

**背景**: FortiSandbox 是一种沙箱安全解决方案，通过在隔离环境中执行可疑文件来检测高级威胁。CISA 是负责美国联邦网络安全和基础设施保护的机构。该指令源于这些漏洞已在野外被积极利用，因此立即修补至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fortinet.com/content/dam/fortinet/assets/data-sheets/FortiSandbox.pdf">PDF FortiSandbox Data Sheet</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cybersecurity_and_Infrastructure_Security_Agency">Cybersecurity and Infrastructure Security Agency - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CISA`, `#Fortinet`, `#exploit`

---

<a id="item-8"></a>
## [在宜居带岩质系外行星上首次探测到大气层](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

天文学家利用詹姆斯·韦伯太空望远镜首次确认在岩质系外行星 LHS 1140b 上探测到大气层，该行星位于 49 光年外一颗红矮星的宜居带内。JWST 的发射光谱排除了该行星是迷你海王星的其他解释。 这一发现标志着首次在宜居带的岩质行星上发现大气层，是评估地外生命潜力的关键一步。它展示了 JWST 表征小型系外行星大气层的能力，并挑战了关于活跃红矮星周围大气层保留的假设。 行星 LHS 1140b 大小约为地球的 1.7 倍，每 25 天在其红矮星宜居带内运行一周。JWST 的中红外观测排除了迷你海王星典型的厚氢氦包层，反而支持可能富含氮气或二氧化碳的较薄大气层。

hackernews · neversaydie · 7月17日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=48947560)

**背景**: 红矮星是银河系中最常见的恒星，但由于亮度低，其宜居带非常靠近，行星常遭受强烈恒星耀斑和大气剥离。宜居带是行星表面可能存在液态水的轨道范围，被视为宜居性的关键标准。在 JWST 这一结果之前，许多此类行星被认为是有厚气体包层的迷你海王星，而非拥有大气层的岩质世界。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mini-Neptune">Mini - Neptune - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Habitable_zone">Habitable zone</a></li>
<li><a href="https://en.wikipedia.org/wiki/Red_dwarf_star">Red dwarf star</a></li>

</ul>
</details>

**社区讨论**: 许多评论者对于红矮星附近的岩质行星能保留大气层表示惊讶，最初认为 LHS 1140b 可能是一个沸腾的迷你海王星。其他人则将焦点转向更广泛的影响，如费米悖论和技术文明通信的短暂窗口，一些人主张建造太阳引力透镜望远镜以更仔细研究此类候选行星。

**标签**: `#exoplanets`, `#JWST`, `#astrobiology`, `#astronomy`

---

<a id="item-9"></a>
## [实用 SQLite 技巧：专家模式、备份与凭证管理](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 8.0/10

Julia Evans 的一篇博文汇总了实用的 SQLite 技巧，包括使用 `.expert` 模式推荐索引、采用 `.dump` 和压缩的安全备份策略，以及简化云备份的凭证生成。 这些技巧解决了开发者在 SQLite 使用中的常见痛点，如查询性能优化、无阻塞备份和安全凭证管理，使 SQLite 在生产环境中更易用且更可靠。 `.expert` 模式通过分析查询来推荐索引；使用 `zstd --fast --rsyncable` 压缩的 `.dump` 备份在体积和增量同步方面表现出色；`s3-credentials` 工具可生成仅限特定桶的凭证，避免 AWS 控制台操作。

hackernews · surprisetalk · 7月17日 17:45 · [社区讨论](https://news.ycombinator.com/item?id=48950122)

**背景**: SQLite 是一种轻量级的嵌入式数据库引擎，广泛应用于各种应用程序。它的命令行界面提供了许多实用功能，例如用于索引建议的 `.expert`。在不锁定的情况下备份 SQLite 数据库需要使用 WAL 模式和 `.dump`。管理云凭证通常很繁琐，而 `s3-credentials` 等工具简化了这一过程。

**社区讨论**: 社区对 `.expert` 模式简化索引决策表示赞赏。Simon Willison 分享了他的 `s3-credentials` 工具用于轻松生成凭证。andrewaylett 展示了一个实用的无阻塞备份流程，使用了 `.dump` 和 zstd 压缩。

**标签**: `#SQLite`, `#database`, `#backups`, `#optimization`, `#tools`

---

<a id="item-10"></a>
## [社区指责 Kaggle 竞赛中 AI 评审和 AI 提交的漏洞](https://www.kaggle.com/competitions/kaggle-measuring-agi/discussion/724918#3498423) ⭐️ 8.0/10

Kaggle 竞赛的社区讨论揭露了对 AI 生成的提交和 AI 评审的担忧，认为这些做法损害了公平性，并指控通过提示注入来操纵结果。 这很重要，因为 Kaggle 是一个重要的数据科学平台，竞赛的公正性直接影响职业机会和人们对 AI 评估方法的信任。 该竞赛提供了 2.5 万美元的奖金，社区成员报告称，一些获胜作品使用了提示注入来欺骗 AI 评审宣布它们获胜。

hackernews · twerkmeister · 7月17日 11:30 · [社区讨论](https://news.ycombinator.com/item?id=48946010)

**背景**: Kaggle 是谷歌旗下的在线平台，举办数据科学竞赛，参与者建立模型解决挑战。依赖 AI 评审提交是近期趋势，但缺乏适当保障措施可能被利用。历史上，Kaggle 曾因不道德数据使用和黑盒模型而受到批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kaggle">Kaggle</a></li>
<li><a href="https://www.kaggle.com/datasets">Find Open Datasets and Machine Learning Projects | Kaggle</a></li>

</ul>
</details>

**社区讨论**: 评论者意见分歧：有人认为 AI 有用，但警告不要盲目接受；另一些人则认为 AI 通过允许提示注入攻击毁掉了公平竞争。少数人指出，暴力破解手段在 Kaggle 中一直存在，因此问题并非新鲜。

**标签**: `#AI`, `#Kaggle`, `#hackathons`, `#evaluation`, `#fairness`

---

<a id="item-11"></a>
## [OpenSSL HollowByte 漏洞通过 11 字节 TLS 请求冻结内存](https://thehackernews.com/2026/07/openssl-hollowbyte-flaw-could-freeze.html) ⭐️ 8.0/10

OpenSSL 中一个名为 HollowByte 的拒绝服务漏洞允许未经身份验证的攻击者通过发送特制的 11 字节 TLS 请求冻结服务器内存，可能导致内存耗尽直至进程重启。OpenSSL 在 2026 年 6 月悄悄修复了该漏洞，没有发布 CVE、公告或更新日志条目。 该漏洞影响全球数百万使用 OpenSSL 的服务器，OpenSSL 是安全通信的核心加密库。静默修复和缺乏透明度引发了对关键基础设施中负责任披露和补丁管理的担忧。 在使用 glibc 的系统上，畸形的 TLS 握手导致 OpenSSL 分配最多 131 KB 的内存且从未释放，导致持续的内存耗尽。利用仅需 11 字节的载荷，且不需要身份验证。

rss · The Hacker News · 7月17日 20:20

**背景**: OpenSSL 是一个广泛使用的开源库，实现了用于安全网络通信的 TLS 协议。glibc 内存分配器使用每线程区域系统，如果分配了内存块但未释放，则可能导致内存保持分配状态，就像本例中一样。HollowByte 漏洞通过发送触发分配响应缓冲区但从未释放的 TLS ClientHello 消息来利用此行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hollowbyte-ddos-flaw-bloats-openssl-server-memory-with-11-byte-payload/">HollowByte DDoS flaw bloats OpenSSL server memory with 11-byte payload</a></li>
<li><a href="https://cybersecuritynews.com/openssl-hollowbyte-vulnerability/">OpenSSL "HollowByte" Vulnerability Lets Hackers Crash Servers With Just ...</a></li>
<li><a href="https://thehackernews.com/2026/07/openssl-hollowbyte-flaw-could-freeze.html">OpenSSL HollowByte Flaw Could Freeze Server Memory with 11-Byte TLS ...</a></li>

</ul>
</details>

**标签**: `#security`, `#openssl`, `#vulnerability`, `#denial-of-service`, `#tls`

---

<a id="item-12"></a>
## [恶意 Vite npm 包利用区块链 C2](https://thehackernews.com/2026/07/seven-malicious-vite-npm-packages-use.html) ⭐️ 8.0/10

Checkmarx 的研究人员发现了七个恶意 npm 包，代号 ViteVenom，它们利用 Tron 区块链进行命令与控制（C2），以传播远程访问木马（RAT）。 此次软件供应链攻击针对 Vite 前端工具生态系统，且使用基于区块链的 C2 使基础设施极难被摧毁。 该活动是此前 ChainVeil 恶意软件的扩展，并采用了基于 Tron 区块链的四层 C2 基础设施。

rss · The Hacker News · 7月17日 18:54

**背景**: Vite 是一种现代前端构建工具，提供快速的开发服务器和优化的构建输出。npm 是 JavaScript 的包管理器，开发者可从中安装依赖。基于区块链的命令与控制利用 Tron 等公有账本存储命令，使当局难以关闭。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vite.dev/">Vite | Next Generation Frontend Tooling</a></li>
<li><a href="https://thehackernews.com/2026/02/aeternum-c2-botnet-stores-encrypted.html">Aeternum C2 Botnet Stores Encrypted Commands on Polygon ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tron_(blockchain)">Tron (blockchain)</a></li>

</ul>
</details>

**标签**: `#npm`, `#supply chain attack`, `#Vite`, `#blockchain`, `#malware`

---

<a id="item-13"></a>
## [新 NadMesh 僵尸网络瞄准暴露的 AI 服务窃取云凭证](https://thehackernews.com/2026/07/new-nadmesh-botnet-hunts-exposed-ai.html) ⭐️ 8.0/10

2026 年 7 月初发现了一个名为 NadMesh 的新型 Go 语言僵尸网络，它积极扫描暴露的 AI 服务（如 ComfyUI 和 Ollama），其仪表板声称已获取 3,811 个唯一的 AWS 密钥。 该僵尸网络针对广泛使用但通常安全性较弱的 AI 基础设施，对云安全构成重大威胁，可能导致数据泄露和资源劫持。 NadMesh 使用超过 20 种远程代码执行向量，并集成了 Shodan 收集器以不断填充其扫描队列。该僵尸网络用 Go 编写，代码中标识为 'n4d mesh controller'。

rss · The Hacker News · 7月17日 17:12

**背景**: 像 ComfyUI（基于节点的图像生成界面）和 Ollama（本地大语言模型运行器）这样的 AI 服务通常快速部署而缺乏适当的安全加固，因此成为有吸引力的目标。像 NadMesh 这样的僵尸网络能够自动化大规模发现和利用这些暴露的服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/new-nadmesh-botnet-hunts-exposed-ai.html">New NadMesh Botnet Hunts Exposed AI Services for Cloud Keys and Kubernetes Tokens</a></li>
<li><a href="https://cyberpress.org/nadmesh-targets-ai-servers/">NadMesh Botnet Targets AI and MCP Servers With 20+ Remote Code Execution Vectors</a></li>
<li><a href="https://gbhackers.com/new-nadmesh-botnet/">New NadMesh Botnet Uses 20+ RCE Vectors to Hijack AI and MCP Infrastructure</a></li>

</ul>
</details>

**标签**: `#botnet`, `#cybersecurity`, `#AI services`, `#cloud security`, `#Kubernetes`

---

<a id="item-14"></a>
## [GoldenEyeDog 子团伙与 DigiCert 入侵事件关联](https://thehackernews.com/2026/07/goldeneyedog-subgroup-linked-to.html) ⭐️ 8.0/10

Expel 的研究人员将 2026 年 4 月的 DigiCert 安全事件归因于中国网络犯罪组织 GoldenEyeDog 的子团伙 CylindricalCanine，该团伙窃取了代码签名证书用于签署恶意软件。 此次入侵破坏了人们对主要证书颁发机构的信任，可能引发供应链攻击，因为被盗的代码签名证书可使恶意软件看起来合法。这凸显了中国网络犯罪组织持续针对关键基础设施的威胁。 被盗证书被用于签名名为 Zhong Stealer 的恶意软件变种，大约有 60 个证书被撤销。子团伙 CylindricalCanine 使用修改版的 Gh0st RAT 变种，如 Golden Gh0st Loader 和 Golden Gh0st RAT。

rss · The Hacker News · 7月17日 16:39

**背景**: 代码签名证书是用于验证软件真实性和完整性的数字证书。一旦被盗，它们可能被滥用来签署恶意代码，使其看起来可信。GoldenEyeDog（也称为 APT-Q-27、Dragon Breath）是一个自 2015 年以来以赌博和游戏行业为目标的网络犯罪组织。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/goldeneyedog-subgroup-linked-to.html">GoldenEyeDog Subgroup Linked to DigiCert Breach and Code ...</a></li>
<li><a href="https://expel.com/blog/introducing-cylindricalcanine/">Introducing CylindricalCanine: The GoldenEyeDog subgroup... | Expel</a></li>
<li><a href="https://www.securitricks.com/attackreports/introducing-cylindricalcanine-the-goldeneyedog-subgroup-responsible-for-the-april-digicert-incident">Introducing CylindricalCanine: The GoldenEyeDog subgroup ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#DigiCert`, `#code-signing certificate theft`, `#GoldenEyeDog`, `#APT`

---

<a id="item-15"></a>
## [朝鲜黑客在假编码测试中使用 SVG 隐写术](https://thehackernews.com/2026/07/north-korea-linked-hackers-hide.html) ⭐️ 8.0/10

与 Contagious Interview 活动相关的朝鲜威胁行为者现在利用 SVG 图像文件中的隐写术，通过虚假招聘信息和编码挑战隐藏并投递 OtterCookie 恶意软件。 这种新颖的攻击向量针对软件开发者这一高价值群体，利用对招聘流程的信任并采用复杂的规避技术，增加了凭证和加密货币被盗的风险。 该攻击涉及一个四阶段的有效载荷，包括浏览器凭证窃取器、加密货币钱包窃取器和文件窃取器，全部通过隐写术隐藏在 SVG 旗帜图像中。

rss · The Hacker News · 7月17日 13:48

**背景**: Contagious Interview 活动首次于 2023 年 11 月被报道，涉及朝鲜威胁行为者冒充招聘人员诱骗求职者安装恶意软件。OtterCookie 是与该活动相关的凭证和加密货币钱包窃取器。隐写术是一种将数据隐藏在其他文件（如图像）中的做法，以避免检测。使用 SVG 文件进行隐写术是一种不太常见但有效的技术，因为 SVG 文件可以包含嵌入的 XML 数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/north-korea-linked-hackers-hide.html">Fake Coding Tests Deliver OtterCookie-Aligned Malware Hidden ...</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/03/11/contagious-interview-malware-delivered-through-fake-developer-job-interviews/">Contagious Interview: Malware delivered through fake developer job interviews | Microsoft Security Blog</a></li>
<li><a href="https://any.run/cybersecurity-blog/ottercookie-malware-analysis/">OtterCookie: Analysis of New Lazarus Group Malware</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#steganography`, `#north korea`, `#credential theft`

---

<a id="item-16"></a>
## [Windows AppResolver 提权：从 AppContainer 到 SYSTEM 的 PoC](https://www.reddit.com/r/netsec/comments/1uyzhy8/windows_appresolver_lpe_from_appcontainer_to/) ⭐️ 8.0/10

一个用于 Windows 权限提升漏洞（编号 CVE-2026-50454）的概念验证利用程序已在 GitHub 上发布。该利用程序利用了 Windows AppResolver 中的授权问题，将权限从 AppContainer 沙箱提升至完全的 SYSTEM 权限。 该漏洞展示了从 AppContainer（Windows 核心安全隔离机制）进行的关键沙箱逃逸。成功利用可让恶意软件或攻击者获得对系统的完全控制，对企业和个人 Windows 环境构成严重风险。 该漏洞已在 2026 年 7 月的 Windows 安全更新中被修复。PoC 由 David Carliez 编写并托管在 GitHub 上，可供安全研究人员测试和理解攻击向量。

reddit · r/netsec · /u/ShufflinMuffin · 7月17日 13:18

**背景**: AppContainer 是 Windows 8 引入的沙箱机制，它将进程限制在一组有限的功能内，常用于现代应用和浏览器。本地权限提升（LPE）漏洞允许在低权限上下文（如 AppContainer）中运行的攻击者获得更高权限（例如 SYSTEM）。CVE-2026-50454 是 AppResolver 组件中的一个授权问题，该组件帮助应用程序解析协议处理程序和文件关联。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/DavidCarliez/Windows-AppResolver-LPE-PoC">GitHub - DavidCarliez/ Windows - AppResolver -LPE-PoC: Windows ...</a></li>

</ul>
</details>

**标签**: `#Windows`, `#privilege escalation`, `#security`, `#CVE`, `#AppContainer`

---

<a id="item-17"></a>
## [Kaiser 护士批评 AI 和监控影响医护质量](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

Kaiser Permanente 的护士公开表示，AI 工具和工作场所监控系统损害了他们的工作和患者护理，投诉集中在呼叫中心指标、限制护理的压力以及一个已停用的 AI 共情试点项目上。但也有一些护士和医生报告称，医疗大语言模型有助于翻译、笔记总结并减轻压力。 这凸显了医疗领域 AI 加速采用过程中日益紧张的局势：虽然 AI 能提高效率，但指标滥用和监控可能损害护理质量和员工士气。这场争论反映了在临床环境中平衡技术收益与伦理保障的广泛关切。 该文章主要批评的是非 AI 的指标滥用，比如惩罚长时间通话或限制每次咨询的建议数量，但将其与 AI 混为一谈。2024 年启动的 AI 共情评估试点已经停用，许多护士认为大语言模型工具在实时翻译、笔记总结和快速获取医学文献方面很有价值。

hackernews · gnabgib · 7月17日 22:26 · [社区讨论](https://news.ycombinator.com/item?id=48952880)

**背景**: AI 在医疗领域的应用正在迅速扩展；到 2025 年初，美国 106 个医疗系统中发现了超过 127 个 AI 部署项目，常见的应用包括护士排班算法和环境记录工具。医院内的工作场所监控也在增长，通过数据监控通话时长和患者互动，这可能与以患者为中心的护理相冲突。Kaiser Permanente 是一家大型综合性医疗系统，虽然投资了 AI 工具，但当指标被认为是为了削减成本而非提高质量时，就会引发反弹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nurse.org/news/nursing-ai-watch/">Nursing AI Watch: What's Really Happening With AI in... | Nurse .Org</a></li>
<li><a href="https://www.fiercehealthcare.com/ai-and-machine-learning/chromie-health-earns-2m-pre-seed-funding-launches-sms-ai-powered-staffing">Chromie Health nabs $2M for nurse staffing AI tool</a></li>
<li><a href="https://phys.org/news/2025-05-tougher-workplace-surveillance.html">Being monitored at work ? A new report calls for tougher workplace ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为文章将指标滥用与 AI 混为一谈，指出真正的损害来自削减成本的呼叫中心指标，而非 AI 本身。一些人称赞 AI 笔记工具减轻了医生压力，另一些人则批评用 AI 评估共情能力的想法。少数评论者警告说，保险公司和医疗服务提供者都在用 AI 武装自己，最终伤害的是患者。

**标签**: `#AI in healthcare`, `#workplace surveillance`, `#nursing`, `#Kaiser Permanente`, `#ethics`

---

<a id="item-18"></a>
## [Kimi K3 与鹈鹕基准测试的启示](https://simonwillison.net/2026/Jul/16/kimi-k3/) ⭐️ 7.0/10

Simon Willison 的文章分析了 Kimi K3 在鹈鹕 SVG 基准测试上的表现，发现异常高的 token 计数，暗示存在 85 token 的隐藏系统提示用于推理努力。 这一分析突出了 AI 评估中的关键问题，如隐藏提示和数据污染，影响我们对基准测试结果的解读。它还强调了 Kimi K3、Claude Fable 5 和 GPT-5.6 Sol 等领先模型在成本、速度和质量之间的权衡。 Kimi K3 每 token 成本比 Claude Fable 5 便宜 5 倍，但速度慢 2 倍。隐藏提示很可能是在<think>标记前注入的推理努力提示，虽不影响鹈鹕任务输出，但扭曲了 token 计数。

hackernews · droidjj · 7月17日 14:21 · [社区讨论](https://news.ycombinator.com/item?id=48947717)

**背景**: 鹈鹕基准测试是一个简单的测试，要求 LLM 生成骑自行车的鹈鹕的 SVG 代码，用于探查创造力和指令遵循能力。token 计数不一致可能揭示隐藏的系统提示，因为模型可能在处理用户输入前附加指令。Kimi K3 是 Moonshot AI 的旗舰模型，具有 100 万 token 的上下文窗口，性能媲美美国前沿模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/pelican-bicycle">GitHub - simonw/pelican-bicycle: LLM benchmark: Generate an SVG of a pelican riding a bicycle · GitHub</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://www.cnbc.com/2026/07/17/moonshot-ai-kimi-k3-model-openai-anthropic-china.html">China's Moonshot AI unveils Kimi K3 that rivals OpenAI ... - CNBC</a></li>

</ul>
</details>

**社区讨论**: 评论者对训练数据污染表示怀疑，指出 Simon 自己的博客内容可能出现在训练集中。其他人幽默地提出了对抗性扩展，如 SWE-bench-adversarial-pelican-gen，一些用户分享了成本/速度比较和替代基准测试。

**标签**: `#AI`, `#benchmarks`, `#LLMs`, `#tokenization`, `#prompt engineering`

---

<a id="item-19"></a>
## [Mozilla 报告分析开源 AI 增长与争论](https://stateofopensource.ai/) ⭐️ 7.0/10

Mozilla 发布了一份关于开源 AI 现状的报告，指出开放模型的快速增长，但因其分析浅薄且可能由 LLM 生成而受到批评。 这场辩论突显了开放与封闭 AI 模型之间日益紧张的关系，并质疑了像 Mozilla 这样知名组织发布的报告的可信度。 该报告以 CTO 风格的幻灯片形式呈现，包含大量图表，但批评者称其文字似乎是 LLM 生成的，且分析缺乏深度。

hackernews · rellem · 7月17日 14:31 · [社区讨论](https://news.ycombinator.com/item?id=48947825)

**背景**: 开源 AI 模型，如 Meta 的 Llama 和 Mistral，使用量快速增长，挑战着 OpenAI 和 Anthropic 等公司的专有模型。辩论的核心在于开放模型和封闭模型最终谁将主导 AI 领域。

**社区讨论**: 评论者指出模型使用量大幅转向开放模型，一位用户追踪到 OpenRouter 上 4 个月内 token 增长了 5 倍。其他人批评报告质量，称其阅读体验痛苦且可能是 LLM 生成的，并附上了'pangram'历史链接以暗示 AI 作者身份。

**标签**: `#open source`, `#AI`, `#Mozilla`, `#community debate`, `#LLM`

---

<a id="item-20"></a>
## [实时 SSH 蜜罐可视化走红](https://honeypotlive.cc/) ⭐️ 7.0/10

项目 honeypotlive.cc 提供了一个实时仪表盘，展示 SSH 机器人程序与蜜罐的交互，揭示了公共 IP 地址上的自动攻击。 这种可视化让广大受众看到互联网扫描的持续背景噪音，提高对自动化威胁及 SSH 安全重要性的认识。 该蜜罐模拟虚假 SSH 服务器，记录登录尝试和命令，网站实时显示这些事件；但用户报告聊天界面中存在垃圾信息滥用。

hackernews · tusksm · 7月17日 14:05 · [社区讨论](https://news.ycombinator.com/item?id=48947548)

**背景**: 蜜罐是一种诱饵系统，旨在吸引攻击者并记录其活动以供分析。SSH（安全外壳）是常用于远程服务器管理的协议，因此成为自动机器人寻找脆弱凭证的频繁目标。这种低交互蜜罐记录登录尝试但不允许实际入侵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/droberson/ssh-honeypot">GitHub - droberson/ssh-honeypot: Fake sshd that logs ip ...</a></li>
<li><a href="https://github.com/jaksi/sshesame">An easy to set up and use SSH honeypot, a fake SSH server ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对实时显示表示有趣，但指出垃圾信息迅速填满聊天，掩盖了有趣的模式。一些用户分享了自己的蜜罐项目，另一些则强调公共 IP 上背景噪音的庞大数量。

**标签**: `#security`, `#honeypot`, `#SSH`, `#real-time`

---