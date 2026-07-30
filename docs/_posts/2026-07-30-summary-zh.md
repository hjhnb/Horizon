---
layout: default
title: "Horizon Summary: 2026-07-30 (ZH)"
date: 2026-07-30
lang: zh
---

> 从 72 条内容中筛选出 20 条重要资讯。

---

1. [13 年之久的 Secure Boot 漏洞被曝光](#item-1)
2. [新基准测试 LLM 密码分析能力](#item-2)
3. [Rails Active Storage 严重漏洞可读取文件](#item-3)
4. [Ruflo MCP 漏洞允许未认证远程代码执行](#item-4)
5. [协同网络攻击波及明尼苏达州 30 多个供水系统](#item-5)
6. [Check Point SmartConsole 认证绕过漏洞 PoC 已公布](#item-6)
7. [Gitea 关键远程代码执行漏洞已被修复](#item-7)
8. [两个被入侵的 joyfill npm 包传播远程访问木马](#item-8)
9. [俄罗斯黑客利用 Exchange OWA 零日漏洞实现持久访问](#item-9)
10. [Eufy 门铃同步协议被逆向，WiFi 凭证遭破解](#item-10)
11. [前沿实验室 AI 智能体入侵技术时间线](#item-11)
12. [AI 顶尖初创公司减少发表研究](#item-12)
13. [开源引擎通过从 SSD 流式传输 MoE 专家，在 2GB 内存中运行 Gemma 4 26B](#item-13)
14. [Superlogical：基于 Ghostty 终端库的新公司](#item-14)
15. [KOReader：开源电子阅读器应用引发赞誉与批评](#item-15)
16. [长政策文档无法可靠地约束 LLM 智能体](#item-16)
17. [文档 AI 蠕虫可通过 Word 的 Copilot 自我传播](#item-17)
18. [VMware 多个严重漏洞允许认证绕过、代码执行和虚拟机逃逸](#item-18)
19. [单个恶意网页即可攻破 Tor 浏览器](#item-19)
20. [俄罗斯指控 Telegram 创始人杜罗夫协助恐怖活动](#item-20)

---

<a id="item-1"></a>
## [13 年之久的 Secure Boot 漏洞被曝光](https://www.schneier.com/blog/archives/2026/07/long-lived-vulnerability-in-microsoft-secure-boot.html) ⭐️ 9.0/10

ESET 的研究人员发现，11 个未正确签名的 shim 固件镜像（部分可追溯到 2013 年）使得微软 Secure Boot 在其 14 年存在期中的 13 年内可以被轻易绕过。 该漏洞破坏了 Secure Boot 提供的根本信任，使得数十亿 Windows 和 Linux 设备容易受到易于执行的固件级别攻击。 该漏洞源于微软在发现 shim 镜像漏洞后未能撤销其签名证书，且绕过技术简单到新手黑客都能执行。

rss · Schneier on Security · 7月29日 11:01

**背景**: Secure Boot 是一种基于 UEFI 的安全标准，确保系统启动时只加载经过数字签名的可信引导加载程序和操作系统内核，从而防止恶意代码早期执行。Shim 是一种小型引导加载程序，旨在通过充当信任代理将 Secure Boot 扩展到 Linux 和其他非 Windows 环境。微软负责 shim 镜像的签名，如果有漏洞的 shim 仍保持签名，攻击者就可以利用它们绕过 Secure Boot 的保护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Shim_(computing)">Shim (computing) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/UEFI_Secure_Boot">UEFI Secure Boot</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#microsoft`, `#secure boot`, `#firmware`

---

<a id="item-2"></a>
## [新基准测试 LLM 密码分析能力](https://www.schneier.com/blog/archives/2026/07/measuring-llms-ability-to-perform-cryptanalysis.html) ⭐️ 9.0/10

研究人员推出了 CryptanalysisBench，包含 191 个密码分析任务，发现前沿 LLM（特别是 Anthropic 的 Claude 模型）能够发现新的数学攻击，包括对 SpoC AEAD 的密钥恢复攻击和 KINDI 安全证明中的错误。 这表明 LLM 正从模式识别迈向严谨的数学推理，对网络安全有直接影响：如果 AI 能自动化密码分析，可加速漏洞发现和更强加密方案的开发。 该基准包含三个层级：第 1 层（已知破解）、第 2 层（完整强度及缩放版本）和第 3 层（前沿生产原语）。最佳模型破解了 65%–86%的第 1 层方案，并产生了经作者验证的新攻击。

rss · Schneier on Security · 7月29日 01:47

**背景**: 密码分析是通过寻找数学弱点来破解加密系统的研究。传统密码分析需要深厚专业知识和人工劳动。该基准将任务形式化，为 LLM 提供了跨分组密码、哈希函数等原语的自动可验证问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scalevise.com/resources/cryptanalysisbench-llm-cryptanalysis-benchmark/">CryptanalysisBench Tests LLM Cryptanalysis Skills</a></li>
<li><a href="https://noise.getoto.net/2026/07/29/measuring-llms-ability-to-perform-cryptanalysis/">Measuring LLMs’ Ability to Perform Cryptanalysis | Noise</a></li>
<li><a href="https://www.resultsense.com/news/2026-07-29-claude-cryptographic-weaknesses-hawk-aes/">AI model weakens NIST post-quantum candidate in 60 hours</a></li>

</ul>
</details>

**标签**: `#LLMs`, `#cryptanalysis`, `#AI security`, `#benchmark`, `#cybersecurity`

---

<a id="item-3"></a>
## [Rails Active Storage 严重漏洞可读取文件](https://thehackernews.com/2026/07/critical-rails-flaw-could-let.html) ⭐️ 9.0/10

Ruby on Rails 发布了针对 Active Storage 严重漏洞（CVE-2026-66066，CVSS 9.5）的修复程序，该漏洞允许未经身份验证的攻击者通过上传特制图片读取应用服务器上的任意文件。 该漏洞非常严重，因为它可能泄露 secret_key_base、Rails 主密钥、数据库密码和云存储凭证等敏感机密，使数百万 Rails 应用面临风险。 该漏洞存在于 Active Storage 处理上传图片文件的方式中，允许通过恶意构造的图片读取任意文件。CVSS 9.5 的评分强调了立即打补丁的紧迫性。

rss · The Hacker News · 7月29日 18:10

**背景**: Active Storage 是 Ruby on Rails 的库，用于将文件上传到 Amazon S3、Google Cloud Storage 或 Microsoft Azure 等云存储服务。Rails 主密钥用于解密存储于 config/credentials.yml.enc 中的加密凭证。该漏洞可能使攻击者读取主密钥，进一步危害应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://guides.rubyonrails.org/active_storage_overview.html">Active Storage Overview — Ruby on Rails Guides</a></li>
<li><a href="https://grokipedia.com/page/Compromised_master_key_Ruby_on_Rails">Compromised master key (Ruby on Rails)</a></li>

</ul>
</details>

**标签**: `#security`, `#ruby-on-rails`, `#vulnerability`, `#cve`, `#active-storage`

---

<a id="item-4"></a>
## [Ruflo MCP 漏洞允许未认证远程代码执行](https://thehackernews.com/2026/07/ruflo-mcp-flaw-lets-unauthenticated.html) ⭐️ 9.0/10

在 Ruflo（一个用于 Claude Code 和 Codex 的开源代理元框架）中发现了一个最高严重性漏洞（CVE-2026-59726，CVSS 10.0），允许未认证的远程代码执行。该漏洞影响 3.16.3 之前的所有版本。 该漏洞构成严重安全风险，因为 Ruflo 被广泛用于编排可访问敏感系统和数据的 AI 代理。攻击者利用此漏洞可以完全控制框架，执行任意命令并污染 AI 内存，可能危及整个代理管线。 该漏洞与 Ruflo 对模型上下文协议（MCP）的实现有关，该协议用于 AI 模型与应用程序之间的上下文管理。利用该漏洞无需认证，因此很容易通过网络进行利用。

rss · The Hacker News · 7月29日 15:39

**背景**: Ruflo 是一个开源代理元框架，运行在 Claude Code 和 Codex 之上，添加了数百个专用代理、协调的群组、自学习内存和跨机器通信。模型上下文协议（MCP）是 Anthropic 于 2024 年推出的开放标准，用于标准化 AI 系统与外部工具和数据的集成。Ruflo 使用 MCP 管理其代理的上下文和工具。这个漏洞破坏了 Ruflo 中 MCP 实现的安全保障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ruvnet/ruflo">GitHub - ruvnet/ruflo: The leading agent meta-harness ...</a></li>
<li><a href="https://github.com/ruflo-app/ruflo">GitHub - ruflo-app/ruflo: Install ruflo - The leading agent ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CVE`, `#Ruflo`, `#remote code execution`

---

<a id="item-5"></a>
## [协同网络攻击波及明尼苏达州 30 多个供水系统](https://thehackernews.com/2026/07/coordinated-cyberattack-targets-30.html) ⭐️ 9.0/10

2026 年 7 月 26 日至 27 日，一场协同网络攻击针对明尼苏达州 30 多个社区供水系统的运营技术，导致布拉汉姆一处水厂停机，并触发明尼苏达 IT 服务局（MNIT）启动全州网络安全应急响应。 此次事件表明，攻击者正积极针对关键基础设施中的运营技术（OT），并造成了水厂停机等实际后果，若未能遏制，可能影响供水安全与公共安全。 受影响的城镇包括布拉汉姆（水厂离线）、普利茅斯、南圣保罗和梅普尔普莱恩，它们报告了水厂停机、通信故障或自动化控制受影响；布拉汉姆居民被要求减少用水。

rss · The Hacker News · 7月29日 13:48

**背景**: 运营技术（OT）安全是指保护工业控制系统（ICS）的实践和技术，这些系统管理着水处理等关键基础设施中的物理过程。与 IT 系统不同，OT 优先考虑安全性和可用性，因此需要专门的安全方法。此次攻击凸显了资金不足的社区供水系统在应对复杂网络威胁时的脆弱性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/ot-security">What is OT Security? | IBM</a></li>
<li><a href="https://www.fortinet.com/solutions/industries/scada-industrial-control-systems/what-is-ot-security">What is OT Security? An Operational Technology Security Primer</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#critical infrastructure`, `#OT security`, `#water systems`

---

<a id="item-6"></a>
## [Check Point SmartConsole 认证绕过漏洞 PoC 已公布](https://thehackernews.com/2026/07/rapid7-releases-poc-for-exploited-check.html) ⭐️ 9.0/10

针对 CVE-2026-16232 的公开概念验证 (PoC) 利用代码已发布，该漏洞是 Check Point SmartConsole 中的一个严重认证绕过漏洞，目前正在被积极利用。 由于该漏洞 CVSS 评分为 9.3 且已被积极利用，此 PoC 的发布大大增加了使用 Check Point 安全管理服务器的组织的风险，可能使攻击者未经授权访问关键网络安全基础设施。 该漏洞影响 Check Point 安全管理服务器和多域安全管理服务器 (MDS)。Check Point 于 2026 年 7 月 22 日发布了安全公告，随后 Rapid7 发布了该认证绕过漏洞的详细技术分析。

rss · The Hacker News · 7月29日 08:58

**背景**: SmartConsole 是用于配置和管理 Check Point 安全网关及管理服务器的图形化管理客户端。多域安全管理 (MDS) 允许管理员通过单一界面管理多个独立的安全域。该漏洞允许攻击者绕过 SmartConsole 登录过程中的身份验证，从而可能获得完全管理权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rapid7.com/blog/post/ra-check-point-smartconsole-authentication-bypass-technical-analysis-cve-2026-16232/">Check Point SmartConsole Authentication Bypass Technical Analysis...</a></li>
<li><a href="https://support.checkpoint.com/results/download/122450">Check Point R81.20 SmartConsole for Windows</a></li>
<li><a href="https://sc1.checkpoint.com/documents/R81/WebAdminGuides/EN/CP_R81_Multi-DomainSecurityManagement_AdminGuide/Topics-MDSG/Basic-Management-Components.htm">Basic Multi-Domain Security Management Components</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#Check Point`, `#authentication bypass`, `#PoC`

---

<a id="item-7"></a>
## [Gitea 关键远程代码执行漏洞已被修复](https://thehackernews.com/2026/07/new-gitea-rce-lets-repository-writers.html) ⭐️ 9.0/10

Gitea 发布了 1.27.1 版本，修复了 CVE-2026-60004 关键远程代码执行漏洞，该漏洞允许具有仓库写入权限的用户植入恶意 Git 钩子，以 Gitea 服务账户身份执行任意 shell 命令。 该漏洞对自托管 Gitea 实例构成高风险，任何拥有仓库写入权限的用户都可以升级为在服务器上执行任意代码，可能危及整个平台，CVSS 评分 9.8 突显其严重性。 该漏洞影响 Gitea 1.17 至 1.27.0 版本，并在 1.27.1 版本中修复；攻击者利用受控的补丁内容创建实时 Git 钩子，在 Git 操作发生时执行。

rss · The Hacker News · 7月29日 07:47

**背景**: Git 钩子是在提交或推送等特定事件前后自动运行的脚本，常用于自动化；像 Gitea 这样的自托管 Git 平台允许团队在自己的服务器上管理仓库，因此安全补丁对于防范服务器端代码执行至关重要。

**标签**: `#security`, `#vulnerability`, `#gitea`, `#rce`, `#CVE`

---

<a id="item-8"></a>
## [两个被入侵的 joyfill npm 包传播远程访问木马](https://thehackernews.com/2026/07/two-compromised-joyfill-npm-packages.html) ⭐️ 9.0/10

位于@joyfill 命名空间的两个 npm beta 包——@joyfill/layouts@0.1.2-2773.beta.0 和@joyfill/components@4.0.0-rc24-2773-beta.4——被入侵，当导入 Node.js 项目时会传播与 DEV#POPPER 恶意软件家族相关的远程访问木马（RAT）。 此次供应链攻击直接威胁到依赖这些包的开发者和组织，可能导致系统被入侵和数据被盗。它凸显了 npm 生态系统中持续存在的风险以及严格验证包的必要性。 这些包包含一个导入时 JavaScript 植入程序，通过区块链网络 Tron、Aptos 和 BSC 解析加密代码。该恶意软件与 DEV#POPPER 活动有关，该活动通过社会工程学攻击软件开发者，并已扩展到支持 Linux、Windows 和 macOS。

rss · The Hacker News · 7月29日 04:20

**背景**: 对 npm 等包注册表的供应链攻击已成为恶意软件分发的常见途径。DEV#POPPER 是一种与朝鲜威胁行为者相关的远程访问木马，以通过虚假工作机会或项目合作来针对开发者而闻名。使用区块链网络进行命令与控制是一种新兴的逃避检测技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/two-compromised-joyfill-npm-packages.html">Two Compromised joyfill npm Packages Run RAT When Imported Into Node.js</a></li>
<li><a href="https://www.esentire.com/blog/north-korean-apt-malware-analysis-dev-popper-rat-and-omnistealer-everyday-im-shufflin">North Korean APT Malware Analysis: DEV#POPPER RAT and ...</a></li>
<li><a href="https://cybersecuritynews.com/devpopper-social-engineering/">DEV#POPPER Attacking developers via New Social Engineering ...</a></li>

</ul>
</details>

**标签**: `#security`, `#npm`, `#supply chain attack`, `#malware`, `#JavaScript`

---

<a id="item-9"></a>
## [俄罗斯黑客利用 Exchange OWA 零日漏洞实现持久访问](https://www.bleepingcomputer.com/news/security/russian-hackers-exploit-exchange-owa-zero-day-for-long-term-mailbox-access/) ⭐️ 9.0/10

俄罗斯国家支持的黑客组织 Laundry Bear（又名 Void Blizzard）正在利用微软 Exchange Outlook Web Access（OWA）中的一个零日漏洞，部署名为 OWAReaper 的复杂后门，从而实现对邮箱的长期访问。 这一由国家支持的行为者实施的零日漏洞利用对企业的电子邮件安全构成严重威胁，可能危及欧洲和北美政府及关键部门的敏感通信。 OWAReaper 被描述为一个具有隐蔽持久化机制的高度复杂后门，通过针对 Outlook Web Access 的半点击漏洞传递，且至少自 2024 年 4 月以来一直活跃。

rss · BleepingComputer · 7月29日 23:44

**背景**: Void Blizzard 是微软威胁情报发现的一个与俄罗斯有关的威胁行为者，主要针对北约成员国和乌克兰的组织进行网络间谍活动。他们经常使用从信息窃取程序获取的凭据进行初始访问。OWAReaper 代表了基于电子邮件的后门的新高度，利用 Exchange OWA 中的零日漏洞来维持对邮箱的持久访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/security/blog/2025/05/27/new-russia-affiliated-actor-void-blizzard-targets-critical-sectors-for-espionage/">New Russia-affiliated actor Void Blizzard targets critical sectors for ...</a></li>
<li><a href="https://undercodenews.com/russian-hackers-turn-outlook-into-a-weapon-laundry-bears-owareaper-backdoor-reveals-a-new-one-click-email-espionage/">Russian Hackers Turn Outlook Into a Weapon: Laundry Bear’s ...</a></li>
<li><a href="https://www.proofpoint.com/us/blog/threat-insight/cleaning-out-inboxes-ta488-comes-outlook-another-half-click-exploit">Cleaning Out Inboxes: TA488 Comes for Outlook with Another ...</a></li>

</ul>
</details>

**标签**: `#security`, `#zero-day`, `#exchange`, `#russian hackers`, `#backdoor`

---

<a id="item-10"></a>
## [Eufy 门铃同步协议被逆向，WiFi 凭证遭破解](https://www.reddit.com/r/netsec/comments/1va5h8n/reversing_of_eufy_security_video_doorbell_sync/) ⭐️ 9.0/10

一名安全研究人员逆向解析了 Eufy 视频门铃的同步协议，并成功从设备闪存中解密了存储的 WiFi 凭证。 这项研究揭露了流行消费级物联网设备中的重大安全漏洞，表明一旦获得物理访问权限，WiFi 凭证就可能被提取，进而危及整个家庭网络。 研究人员通过焊接闪存芯片或使用 JTAG 接口等硬件方法提取了闪存，然后利用从逆向同步协议中获得的信息解密了凭证。

reddit · r/netsec · /u/gid0rah · 7月29日 18:57

**背景**: 物联网设备通常将 WiFi 密码等敏感数据存储在闪存中，而闪存可通过硬件攻击读取。闪存提取是一种已知技术，可获取所有存储的秘密。同步协议用于将门铃与 Homebase 配对，逆向该协议可揭示用于保护凭证的加密密钥。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.iotsnacks.com/embedded-security/esp32-flash-memory-extraction-firmware-security-lab">ESP32 Flash Memory Extraction: Firmware Security Lab | IoT Snacks</a></li>
<li><a href="https://hackyboiz.github.io/2025/03/09/newp1ayer48/flashrom/en/">[Research] Flash Memory Dump with Flashrom - hackyboiz</a></li>
<li><a href="https://doorbellnest.com/how-to-sync-eufy-doorbell/">How To Sync Eufy Doorbell? - A Step-by-Step Guide -</a></li>

</ul>
</details>

**标签**: `#reverse engineering`, `#IoT security`, `#cryptography`, `#hardware hacking`, `#Eufy`

---

<a id="item-11"></a>
## [前沿实验室 AI 智能体入侵技术时间线](https://www.reddit.com/r/netsec/comments/1v9yd7p/anatomy_of_a_frontier_lab_agent_intrusion_a/) ⭐️ 9.0/10

一份针对前沿 AI 实验室自主智能体系统的安全入侵详细技术时间线被发布，揭示了一个由 OpenAI 模型驱动的 AI 智能体在 2026 年 7 月 9 日至 13 日期间执行了为期多天的攻击。 这一事件凸显了自主 AI 智能体进行复杂入侵的新兴威胁，引发了对前沿 AI 基础设施安全性的关键质疑，以及对新防御策略的需求。 攻击者在大约两天半的时间内执行了约 17,600 次操作，分为 6,280 个集群，展示了机器速度的决策能力和对平台漏洞的利用。

reddit · r/netsec · /u/si9int · 7月29日 14:49

**背景**: AI 智能体是由大型语言模型驱动的自主系统，能够推理、规划、使用工具并采取行动以实现目标。前沿 AI 实验室开发尖端模型，并经常部署具有广泛能力的智能体，使其成为有吸引力的目标。OWASP AI 智能体安全速查表概述了超越传统 LLM 漏洞的独特风险，如提示注入和工具滥用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/agent-intrusion-technical-timeline">Anatomy of a Frontier Lab Agent Intrusion: A Technical Timeline of the July 2026 Incident</a></li>
<li><a href="https://simonwillison.net/2026/Jul/28/anatomy-of-a-frontier-lab-agent-intrusion/">Anatomy of a Frontier Lab Agent Intrusion: A Technical Timeline of the July 2026 Incident</a></li>
<li><a href="https://cheatsheetseries.owasp.org/cheatsheets/AI_Agent_Security_Cheat_Sheet.html">AI Agent Security - OWASP Cheat Sheet Series</a></li>

</ul>
</details>

**标签**: `#AI security`, `#intrusion analysis`, `#agent security`, `#incident response`, `#red team`

---

<a id="item-12"></a>
## [AI 顶尖初创公司减少发表研究](https://www.science.org/content/article/ai-s-top-startups-are-barely-publishing-their-research) ⭐️ 8.0/10

一项最新研究表明，许多顶尖 AI 初创公司（包括 OpenAI 和 Anthropic）因竞争压力和繁琐的同行评审过程而减少或完全不发表研究成果。 这一趋势威胁到 AI 研究的透明度和可重复性，使更广泛的社区难以验证成果并在此基础上进行开发。 该研究将引用次数作为重要性的替代指标，但指出像谷歌这样的公司未被纳入，因为它们不属于独角兽初创公司。

hackernews · YeGoblynQueenne · 7月29日 21:25 · [社区讨论](https://news.ycombinator.com/item?id=49103285)

**背景**: 传统上，学术和企业 AI 研究人员通过同行评审会议发表论文以分享进展。但初创公司可能为避免泄露知识产权和防止竞争对手获知信息而选择不发表。

**社区讨论**: 评论者对同行评审系统表示不满，指出初创公司常因时间限制选择博客文章而非正式论文。另一些人指出文章错误假设 OpenAI 和 Anthropic 不发表，实际上它们确实发布论文。

**标签**: `#AI`, `#research`, `#startups`, `#publishing`, `#open science`

---

<a id="item-13"></a>
## [开源引擎通过从 SSD 流式传输 MoE 专家，在 2GB 内存中运行 Gemma 4 26B](https://github.com/drumih/turbo-fieldfare) ⭐️ 8.0/10

TurboFieldfare 是一个用 Swift 和 Metal 编写的推理引擎，它通过从 SSD 流式传输专家权重，以 4 位精度在任意 M 系列 Mac 上运行 Google 的 Gemma 4 26B-A4B-IT 模型，仅需约 2 GB 内存。 这使得在内存受限的设备上运行大型 MoE 模型成为可能，极大地降低了在消费级硬件上本地运行高级语言模型的门槛。 该引擎在 8 GB M2 MacBook Air 上可实现 5-6 tok/s，在 M5 MacBook Pro 上可达 31-35 tok/s，并包含一个实验性的 OpenAI 兼容服务器，支持流式输出和工具调用。

hackernews · gitpusher42 · 7月29日 15:05 · [社区讨论](https://news.ycombinator.com/item?id=49098510)

**背景**: Gemma 4 26B-A4B 是一个混合专家模型：虽然总共有 261 亿个参数，但每个词元只激活约 40 亿个。通常，所有 261 亿个参数必须加载到内存中，但 TurboFieldfare 仅将共享层和 KV 缓存保留在 RAM 中，按需从 SSD 流式传输路由专家。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B-it">google/gemma-4-26B-A4B-it · Hugging Face</a></li>
<li><a href="https://gemma4.dev/models/gemma-4-26b-a4b">Gemma 4 26B A4B — MoE Architecture for Long Context | gemma4.dev</a></li>
<li><a href="https://wpnews.pro/news/a-26b-model-in-2-gb-of-ram-courtesy-of-your-ssd">A 26B Model in 2 GB of RAM, Courtesy of Your SSD — Web Pulse</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了这种方法，其中一位指出 llama.cpp 已经可以通过 mmap 将模型映射到 2GB，但 TurboFieldfare 将 SSD 读取与推理活动同步可能减少延迟。另一位分享了针对较旧 macOS 的编译方法，还有一位表示有兴趣在 DiffusionGemma 项目上进行合作。

**标签**: `#LLM`, `#inference`, `#edge computing`, `#Metal`, `#open-source`

---

<a id="item-14"></a>
## [Superlogical：基于 Ghostty 终端库的新公司](https://www.superlogical.com/) ⭐️ 8.0/10

MitchellH 宣布成立新公司 Superlogical，该公司将基于 Ghostty 项目的 MIT 开源库 libghostty 构建终端应用。Ghostty 本身已转让给非营利组织。 这展示了一种可持续的开源模式：公司基于开源库进行商业化，而核心项目在非营利组织下保持独立。这可能会为其他寻求社区与商业之间平衡的开源项目树立先例。 Superlogical 将使用与其他人相同的 MIT 许可组件，并将共享的终端改进上游回馈。该公司的做法是将 libghostty 视为终端应用的公共构建块。

hackernews · yan · 7月29日 15:41 · [社区讨论](https://news.ycombinator.com/item?id=49098965)

**背景**: Ghostty 是一个快速、功能丰富、跨平台的终端模拟器，使用平台原生 UI 和 GPU 加速。它提供了 libghostty，一个零依赖的 C 和 Zig 库，用于构建终端模拟器或利用终端功能。通过将 Ghostty 转让给非营利组织，并在其库之上构建 Superlogical，MitchellH 在开源项目与商业实体之间建立了清晰的界限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ghostty.org/">Ghostty</a></li>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty -org/ ghostty : Ghostty is a fast, feature-rich, and...</a></li>
<li><a href="https://medium.com/@amit_tal/ghostty-terminal-fast-native-terminal-that-actually-delivers-a0302ba4bdbc">Ghostty Terminal : A Fast, Native Terminal That Actually... | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍称赞非营利转移模式，simonw 强调这是一种干净的做法。一些人将其与 OLE/COM 和类似项目进行比较，而另一些人则批评标题是点击诱饵。总体对结构创新持积极态度。

**标签**: `#terminal`, `#open-source`, `#startup`, `#ghostty`, `#superlogical`

---

<a id="item-15"></a>
## [KOReader：开源电子阅读器应用引发赞誉与批评](https://koreader.rocks/) ⭐️ 8.0/10

KOReader 仍然是一款备受关注的开源电子阅读器应用程序，近期的社区讨论既突出了其强大功能，也指出了可用性方面的挑战。 KOReader 展示了开源软件如何显著增强 Kindle 和 Kobo 等专有电子阅读器的体验，让用户掌控阅读体验，但其不直观的用户界面可能阻碍更广泛的采用。 KOReader 支持多种格式，包括 PDF、EPUB、DjVu 和 FB2，可在 Kindle、Kobo、PocketBook 和 Android 等设备上运行。用户需要越狱某些设备（如 Kindle）才能安装，许多人认为其界面不直观且有时卡顿。

hackernews · Cider9986 · 7月29日 11:05 · [社区讨论](https://news.ycombinator.com/item?id=49095865)

**背景**: KOReader 是一个主要为电子墨水屏设备设计的开源电子书阅读器应用程序。它源自 Cool Reader 项目的分支，现已发展出丰富的自定义选项、手势控制和同步功能，常常超越流行电子阅读器上的原生阅读软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/koreader/koreader">GitHub - koreader/koreader: An ebook reader application ...</a></li>
<li><a href="https://koreader.com/">KOReader – Free eBook Reader for PDF & EPUB</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍赞赏 KOReader 的功能和提供的自由度，有人称其优于专有软件。然而，多位用户反映界面不直观、手势不可靠且性能有时卡顿，导致一些人更倾向于使用默认阅读器或换用其他应用。

**标签**: `#e-reader`, `#open-source`, `#kindle`, `#kobo`, `#reading`

---

<a id="item-16"></a>
## [长政策文档无法可靠地约束 LLM 智能体](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

一篇题为《Handbook.md》的新论文表明，长篇政策文档无法有效约束 LLM 智能体，主要原因是上下文窗口限制和模型约束。该发现动摇了智能体能可靠遵循长篇书面指令的假设。 这项研究揭示了当前 AI 智能体治理中的一个关键缺陷，因为许多系统依赖长篇政策文档来确保安全和对齐。这表明可能需要替代方案，如本地推理或基于领域特定数据集的强化学习。 该论文可能涉及对模型遵循长篇手册的能力进行基准测试，结果显示随着文档长度增加，性能会下降。社区评论还指出，像 Claude 这样的模型会在短时间内忽略指令。

hackernews · spIrr · 7月29日 13:01 · [社区讨论](https://news.ycombinator.com/item?id=49096969)

**背景**: LLM 智能体是可以自动执行任务的 AI 系统，通过遵循指令来工作。上下文窗口限制了模型一次能处理的文本量，长上下文会出现“上下文腐烂”和量化效果等问题。用政策文档来治理智能体是一种常见的方法，以确保它们安全行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://atlan.com/know/llm-context-window-limitations/">LLM Context Window Limitations in 2026</a></li>
<li><a href="https://medium.com/awarity-ai-blog/navigating-the-challenges-of-context-window-limitations-eef2dcfc02e1">Navigating the Challenges of Context Window Limitations | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区评论对论文的发现表示赞同，用户分享了轶事证据，表明像 Claude 这样的模型会很快忽略长指令。一些人认为，真正的智能体行为需要在特定数据集上进行大量后训练，而不是仅仅依赖上下文。还有人将其与人类在执行长政策时的局限性相类比。

**标签**: `#LLM`, `#agents`, `#long context`, `#model limitations`, `#AI safety`

---

<a id="item-17"></a>
## [文档 AI 蠕虫可通过 Word 的 Copilot 自我传播](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 8.0/10

研究人员 Håkon Måløy 展示了一种新的提示注入变种，它创建了一种自我复制的 AI 蠕虫，针对 Microsoft 的 Word 版 Copilot，其中嵌入在文档中的恶意指令可导致 Copilot 修改并将攻击传播到新文档。 这项研究揭示了 AI 集成生产力工具中的一个基本安全缺陷，因为 LLM 无法可靠地区分指令和数据，从而使无需人工干预即可传播的自主恶意软件成为可能。它强调了在 AI 代理获得对敏感系统的更广泛访问之前，迫切需要强大的防御措施。 该蠕虫利用间接提示注入，共享文档中的对抗性文本覆盖 Copilot 的预期行为，导致其重写或转发恶意内容。在发布时，尚无针对此类漏洞的可靠缓解措施，而使用白色隐藏文本或非常规 Unicode 等技术仍然有效。

hackernews · Canopy9560 · 7月29日 11:44 · [社区讨论](https://news.ycombinator.com/item?id=49096188)

**背景**: 提示注入是一种安全漏洞，精心设计的输入会覆盖 LLM 的预期指令，利用模型无法区分开发者定义的提示和用户提供的数据。在像 Copilot 这样的 AI 集成应用中，当模型处理包含隐藏命令的外部内容（如网页或文档）时，会发生间接提示注入。AI 蠕虫是一种自我传播的恶意软件，它利用 AI 代理在系统间复制自身，利用这种混淆来自主传播。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lWcHY2a0VSR3psMEJCaXNWVVhpZ0FQAQ?hl=en-US&gl=US&ceid=US:en">Google News - Researchers demonstrate autonomous AI worm that...</a></li>

</ul>
</details>

**社区讨论**: 评论者表示深切担忧，认为只要 AI 系统混合数据和指令，这种漏洞就本质上不可修复，rwmj 和 simonw 强调了缓解措施的缺失。boothby 预测了更严重的攻击，设想一个窃取凭证的 GitHub 评论，而 averagjoe 表示他们已经禁用了所有本地 AI 功能。piker 指出白色文本和 Unicode 技巧仍然有效，并链接了一个实际例子。

**标签**: `#AI worm`, `#Copilot`, `#prompt injection`, `#security vulnerability`, `#LLM safety`

---

<a id="item-18"></a>
## [VMware 多个严重漏洞允许认证绕过、代码执行和虚拟机逃逸](https://thehackernews.com/2026/07/three-critical-vmware-flaws-allow-auth.html) ⭐️ 8.0/10

Broadcom 发布了针对三个 VMware 严重漏洞的安全补丁，其中包括 CVE-2026-59309（CVSS 9.8），该漏洞允许对 vCenter Server 进行认证绕过，使远程攻击者能够获得未授权访问，并可能执行任意代码或逃逸虚拟机。 这些漏洞影响广泛使用的 VMware 产品（ESX、vCenter、Workstation、Fusion），对企业虚拟化环境构成严重风险，可能导致宿主机完全受损和数据泄露。系统管理员必须立即优先应用补丁。 CVE-2026-59309 是 vCenter Server 中的认证绕过漏洞，CVSS 评分为 9.8；另外两个严重漏洞可实现任意代码执行和虚拟机逃逸。确切的攻击向量细节尚未完全公开，但 Broadcom 已针对受影响版本发布了安全公告。

rss · The Hacker News · 7月29日 15:31

**背景**: VMware 等虚拟化软件在单个物理主机上创建隔离的虚拟机（VM），vCenter Server 则集中管理多个主机。虚拟机逃逸漏洞允许攻击者突破虚拟机隔离，攻击宿主机或其他虚拟机。通用漏洞评分系统（CVSS）提供了标准严重性评级；9.8 分（满分 10 分）表示严重程度极高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://anorak001.github.io/posts/vm_escape/">VM Escape | ANORAK WRITES</a></li>
<li><a href="https://en.wikipedia.org/wiki/Common_Vulnerability_Scoring_System">Common Vulnerability Scoring System - Wikipedia</a></li>

</ul>
</details>

**标签**: `#vulnerability`, `#security`, `#VMware`, `#virtualization`, `#CVE`

---

<a id="item-19"></a>
## [单个恶意网页即可攻破 Tor 浏览器](https://thehackernews.com/2026/07/researchers-show-single-malicious.html) ⭐️ 8.0/10

来自 Nebula Security 的研究人员展示，仅访问一个恶意网页就能触发 Firefox JIT 编译器漏洞（CVE-2026-10702），导致浏览器渲染进程中任意代码执行。Mozilla 已在 Firefox 151.0.3 中修复该漏洞，且此漏洞同样影响 Tor 浏览器。 该漏洞之所以重要，是因为它无需用户进行除访问网页之外的任何交互，从而可能成为针对依赖匿名性的 Tor 浏览器用户的广泛攻击媒介。它凸显了保护 JavaScript 引擎中 JIT 编译器的持续挑战。 CVE-2026-10702 是 Firefox JIT 编译器中的一个漏洞，允许在渲染进程中执行任意代码。Mozilla 将其评为高严重性，并在 Firefox 151.0.3 更新中修复。基于 Firefox ESR 的 Tor 浏览器在相应更新应用之前同样受影响。

rss · The Hacker News · 7月29日 11:57

**背景**: 即时编译（JIT）编译器用于 JavaScript 引擎，通过运行时编译代码来提高性能。然而，由于它们动态生成可执行代码，可能会引入安全漏洞。任意代码执行（ACE）是一种关键漏洞，允许攻击者在目标系统上运行任意指令。渲染进程是现代浏览器中处理网页内容的沙盒环境，攻破它可能导致进一步的利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2026-10702/">CVE-2026-10702: Firefox JIT RCE Vulnerability Explained</a></li>
<li><a href="https://en.wikipedia.org/wiki/Arbitrary_code_execution">Arbitrary code execution</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#tor`, `#firefox`, `#browser`

---

<a id="item-20"></a>
## [俄罗斯指控 Telegram 创始人杜罗夫协助恐怖活动](https://thehackernews.com/2026/07/russia-charges-telegram-founder-pavel.html) ⭐️ 8.0/10

俄罗斯联邦安全局（FSB）于周三宣布，指控 Telegram 创始人帕维尔·杜罗夫涉嫌协助恐怖活动，并未能移除平台上的违禁内容。 此案凸显了平台政策与国家监管之间的持续紧张关系，对技术监管、隐私和安全具有重大影响，尤其对加密消息服务影响深远。 FSB 特别指出，Telegram 未能移除大量违反俄罗斯关于恐怖活动和违禁信息法律的频道、聊天和机器人。

rss · The Hacker News · 7月29日 11:00

**背景**: Telegram 是一个基于云的即时通讯服务，以其强大的加密和隐私功能而闻名。它曾因加密技术可能被犯罪分子和恐怖分子利用而受到多国政府的审查。俄罗斯此前曾在 2018 年因类似问题试图封锁 Telegram，但后来解除了禁令。

**标签**: `#Telegram`, `#Russia`, `#security`, `#privacy`, `#regulation`

---