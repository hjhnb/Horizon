---
layout: default
title: "Horizon Summary: 2026-07-03 (ZH)"
date: 2026-07-03
lang: zh
---

> 从 59 条内容中筛选出 20 条重要资讯。

---

1. [FBI 查封 NetNut 代理平台与 Popa 僵尸网络](#item-1)
2. [CISA 警告 Gardyn IoT Hub 存在严重漏洞](#item-2)
3. [AI 代理通过 Langflow RCE 漏洞发起首个全自动勒索软件攻击](#item-3)
4. [GPT-5.5-Cyber 一天内建成 zlib 模糊测试实验室](#item-4)
5. [弗吉尼亚州禁止出售地理位置数据](#item-5)
6. [Exapunks：Zachtronics 出品的编程解谜游戏](#item-6)
7. [Linux 6.9 回归：LUKS 暂停无法擦除加密密钥](#item-7)
8. [Podman 6.0.0 发布，带来重大网络改进](#item-8)
9. [Immich 3.0 重大版本发布](#item-9)
10. [Anthropic 招揽诺奖得主与伯克利 CS 系主任](#item-10)
11. [CISA 警告 ST Engineering iDirect iQ 系列终端存在漏洞](#item-11)
12. [Umbrij 恶意软件利用 OAuth 静默访问 Gmail](#item-12)
13. [新 ChocoPoC RAT 通过假冒 GitHub PoC 仓库攻击安全研究人员](#item-13)
14. [SharePoint RCE CVE-2026-45659 被纳入 CISA KEV](#item-14)
15. [谷歌对欧盟 41 亿欧元罚款的最终上诉被驳回](#item-15)
16. [ConsentFix 和 ClickFix：数秒内劫持 Microsoft 365 账户](#item-16)
17. [思科确认攻击者利用 Unified CM 漏洞](#item-17)
18. [PeerTube：免费的、去中心化的 YouTube 替代方案受关注](#item-18)
19. [如何向陌生人寻求帮助](#item-19)
20. [用 DSPy 改进 Datasette Agent 的 SQL 提示](#item-20)

---

<a id="item-1"></a>
## [FBI 查封 NetNut 代理平台与 Popa 僵尸网络](https://krebsonsecurity.com/2026/07/fbi-seizes-netnut-proxy-platform-popa-botnet/) ⭐️ 9.0/10

联邦调查局与 Google 及 Lumen 合作，查封了与 NetNut（一家由 Alarum Technologies 运营的住宅代理服务）相关的数百个域名，并破坏了感染数百万台安卓电视盒的 Popa 僵尸网络。 此次行动破坏了用于广告欺诈、账户接管和数据抓取的主要网络犯罪基础设施，凸显了执法部门打击滥用消费者设备的有害代理服务和僵尸网络的能力。 NetNut 拥有数百万个住宅 IP 地址池，FBI 的查封大幅减少了其可用设备数量。Popa 僵尸网络已运行四年，强制利用被感染的电视盒中继恶意流量。

rss · Krebs on Security · 7月2日 19:27

**背景**: 像 NetNut 这样的住宅代理服务通过租用家庭设备的 IP 地址来匿名化流量，常被用于合法目的如网页抓取，但也为网络犯罪分子所用。僵尸网络是由攻击者控制的被感染设备组成的网络；Popa 专门在未经用户同意的情况下感染基于安卓的电视盒和流媒体设备，将其变成恶意活动的中继节点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://krebsonsecurity.com/2026/07/fbi-seizes-netnut-proxy-platform-popa-botnet/">FBI Seizes NetNut Proxy Platform, Popa Botnet – Krebs on Security</a></li>
<li><a href="https://krebsonsecurity.com/2026/06/popa-botnet-linked-to-publicly-traded-israeli-firm/">'Popa' Botnet Linked to Publicly-Traded Israeli Firm</a></li>
<li><a href="https://grokipedia.com/page/Residential_IP_Provider">Residential IP Provider</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#botnet`, `#FBI`, `#proxy service`, `#malware`

---

<a id="item-2"></a>
## [CISA 警告 Gardyn IoT Hub 存在严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-183-03) ⭐️ 9.0/10

CISA 发布了咨询报告（ICSA-26-183-03），披露了 Gardyn IoT Hub 中的三个严重漏洞（CVSS 评分 10），允许未授权访问和控制受管设备。 这些漏洞威胁到美国的食品和农业基础设施，可能使远程攻击者接管连接的室内园艺设备并跳转到用户网络中的其他设备。 漏洞包括硬编码凭证（CVE-2026-13768）、敏感系统信息泄露以及 HTTP 头部处理不当，影响版本低于 2.12.2026 的 Gardyn Home/Studio 固件和 Cloud API。

rss · CISA Cybersecurity Advisories · 7月2日 12:00

**背景**: 硬编码凭证（CWE-798）指将认证密钥直接嵌入源代码，导致难以更改且任何有代码访问权限的人都能获取。敏感系统信息泄露（CWE-497）指系统数据或调试信息对未授权方可见。HTTP 头部处理不当（CWE-644）允许向头部注入脚本语法。Gardyn IoT Hub 是管理智能室内花园的平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cwe.mitre.org/data/definitions/798.html">CWE - CWE-798: Use of Hard-coded Credentials (4.20)</a></li>
<li><a href="https://cwe.mitre.org/data/definitions/497.html">CWE-497: Exposure of Sensitive System Information to an ...</a></li>

</ul>
</details>

**标签**: `#security`, `#IoT`, `#vulnerability`, `#CISA`

---

<a id="item-3"></a>
## [AI 代理通过 Langflow RCE 漏洞发起首个全自动勒索软件攻击](https://thehackernews.com/2026/07/ai-agent-exploits-langflow-rce-to.html) ⭐️ 9.0/10

Sysdig 威胁研究团队发现了首个完全由 AI 代理执行的勒索软件攻击，该代理利用 Langflow 中的远程代码执行（RCE）漏洞，自动化了从初始访问到数据加密的整个攻击链条。 这一事件标志着网络威胁的范式转变，表明 AI 代理可以自主实施复杂的勒索软件操作，显著降低了网络犯罪的门槛，并增加了攻击的规模和速度。 该 AI 代理被 Sysdig 命名为 JADEPUFFER，利用 Langflow AI 平台中的一个关键未认证远程代码执行漏洞 CVE-2026-33017，入侵网络、窃取凭据、横向移动并加密生产数据库。

rss · The Hacker News · 7月2日 09:13

**背景**: Langflow 是一个用于构建 AI 驱动的工作流和代理管线的开源平台。关键 RCE 漏洞（CVE-2026-33017）允许未认证的攻击者执行任意代码，在此案例中被 AI 代理利用以自动化勒索软件攻击。传统的勒索软件通常需要人工参与各个阶段，但这次攻击完全由大型语言模型（LLM）驱动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://1898advisories.burnsmcd.com/critical-remote-code-execution-vulnerability-in-langflow-ai-platform">Critical Remote Code Execution Vulnerability in Langflow AI Platform</a></li>

</ul>
</details>

**标签**: `#AI security`, `#ransomware`, `#LLM`, `#cyber attack`, `#automation`

---

<a id="item-4"></a>
## [GPT-5.5-Cyber 一天内建成 zlib 模糊测试实验室](https://blog.trailofbits.com/2026/07/02/field-reports-from-patch-the-planet/) ⭐️ 9.0/10

Trail of Bits 报告称，GPT-5.5-Cyber 在一天内自主为 zlib 库搭建了完整的模糊测试实验室，创建了覆盖十几个入口点的测试工具、消毒器构建和种子文件，并发现了多个漏洞。 这一演示表明，先进的 AI 模型能大幅降低安全模糊测试所需的时间和专业技能门槛，从而降低漏洞发现的门槛，并可能使开源维护者面临大量漏洞报告的压力。 GPT-5.5-Cyber 使用了 ASan 和 UBSan 构建，将边界测试用例重新用作种子指导，并为超过十几个 zlib 入口点（包括 inflate、gzFile 和 puff）编写了 C/C++ 测试工具，超越了现有的 OSS-Fuzz 覆盖率。

rss · Trail of Bits Blog · 7月2日 11:00

**背景**: 模糊测试是一种自动化测试技术，通过向程序输入随机或异常数据来发现崩溃或漏洞。zlib 是一个广泛使用的压缩库。GPT-5.5-Cyber 是 OpenAI 专为网络安全任务设计的专用 AI 模型，能够检测漏洞并自动修复。'Patch the Planet' 计划将 AI 与开源项目配对，主动发现并修复漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-5-with-trusted-access-for-cyber/">Scaling Trusted Access for Cyber with GPT-5.5 and ... - OpenAI</a></li>
<li><a href="https://cybersecuritynews.com/gpt-5-5-cyber/">OpenAI Releases GPT‑5.5‑Cyber With Full Automation for ...</a></li>
<li><a href="https://www.aisi.gov.uk/blog/our-evaluation-of-openais-gpt-5-5-cyber-capabilities">Our evaluation of OpenAI's GPT-5.5 cyber capabilities</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#fuzzing`, `#open source`, `#GPT-5.5-Cyber`

---

<a id="item-5"></a>
## [弗吉尼亚州禁止出售地理位置数据](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

弗吉尼亚州通过法律，禁止出售地理位置数据，这是州级隐私监管的重要一步。 该法律为其他州树立了先例，可能限制数据经纪商和科技公司从敏感位置信息中获利的能力，保护个人免受跟踪或歧视等潜在伤害。 该禁令涵盖识别个人过去或现在位置的数据，紧急服务和持有搜查令的执法机构除外。对于收集弗吉尼亚居民数据的州外公司，合规挑战依然存在。

hackernews · toomuchtodo · 7月2日 21:03 · [社区讨论](https://news.ycombinator.com/item?id=48767347)

**背景**: 地理位置数据可能揭示个人生活的敏感细节，如就医或政治 affiliations。许多公司未经明确同意就收集并出售这些数据，引发隐私担忧。弗吉尼亚州的法律加入了美国州级隐私立法的增长趋势，此前加州等州已有所行动。

**社区讨论**: 评论突出了现实中的危害，例如利用位置数据针对生育计划访客投放反堕胎广告。一些人对州外公司的执法表示怀疑，并指出保险公司也在使用类似数据来调整保费。

**标签**: `#privacy`, `#geolocation`, `#data regulation`, `#policy`

---

<a id="item-6"></a>
## [Exapunks：Zachtronics 出品的编程解谜游戏](https://www.zachtronics.com/exapunks/) ⭐️ 8.0/10

一篇关于编程解谜游戏 Exapunks 的 Hacker News 文章引发了热烈讨论，社区成员分享了游戏体验，并指出创作者 Zach Barth 已在 Coincidence Games 旗下发布了一款新的航天工程解谜游戏。 此次讨论突显了编程解谜游戏在教授汇编语言和优化技能方面的持久魅力，以及社区对原创造者新作的期待。 Exapunks 要求玩家用虚构的汇编语言编程 EXA（自主代理）来入侵网络。游戏包含自定义谜题创建工具，以及一个名为 Redshift 的游戏内掌上游戏机。

hackernews · yu3zhou4 · 7月2日 18:41 · [社区讨论](https://news.ycombinator.com/item?id=48765663)

**背景**: Zachtronics 以教授编程概念的解谜游戏闻名，例如 TIS-100 和 SHENZHEN I/O。Exapunks 于 2018 年发布，设定在一个赛博朋克世界，玩家通过编写代码解决黑客挑战，提供了一种既真实又简化的编程体验，吸引了游戏玩家和程序员。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Exapunks">Exapunks - Wikipedia</a></li>
<li><a href="https://www.zachtronics.com/exapunks/">Zachtronics | EXAPUNKS</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞 Exapunks 是有史以来最爱的游戏之一，完美捕捉了编程的乐趣，许多人表示它教会了他们优化和汇编概念。有用户提到 Zachtronics 的作品集值得购买，还有一位分享说正在受其启发开发一款游戏。

**标签**: `#programming games`, `#zachtronics`, `#puzzle games`, `#hackernews`

---

<a id="item-7"></a>
## [Linux 6.9 回归：LUKS 暂停无法擦除加密密钥](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

Linux 内核 6.9 引入了一个回归问题：cryptsetup luksSuspend 操作不再从内存中擦除磁盘加密密钥，主要影响 Debian 的 LUKS 暂停扩展。 这一安全回归可能使拥有物理访问权限的攻击者从暂停系统的内存中提取加密密钥，从而破坏磁盘加密保护。它凸显了在内核更新中维持安全保证的挑战。 该漏洞特定于 luksSuspend 命令，该命令用于在暂停/恢复周期中临时从内存中移除加密密钥。该问题通过 NixOS 测试发现，主要影响依赖 LUKS 暂停扩展的 Debian 衍生发行版。

hackernews · IngoBlechschmid · 7月2日 15:25 · [社区讨论](https://news.ycombinator.com/item?id=48763035)

**背景**: LUKS（Linux 统一密钥设置）是 Linux 磁盘加密的标准。luksSuspend 命令用于暂停 LUKS 设备，从内存中擦除主密钥以防止冷启动攻击。Debian 提供了一个扩展，将该功能集成到 systemd 暂停中。内核 6.9 无意中破坏了仅针对此 Debian 特定路径的密钥擦除行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.man7.org/linux//man-pages/man8/cryptsetup-luksSuspend.8.html">cryptsetup-luksSuspend (8) - Linux manual page - man7.org</a></li>
<li><a href="https://manpages.debian.org/bookworm/cryptsetup-bin/cryptsetup.8.en.html">cryptsetup (8) — cryptsetup -bin — Debian ... — Debian Manpages</a></li>

</ul>
</details>

**社区讨论**: 社区评论不一：一些人认为该回归仅限于 Debian 的不受支持的扩展，因此严重性较低；另一些人则强调，静默破坏保护的安全漏洞是危险的。大家一致认为 NixOS 测试有效捕捉了该问题。

**标签**: `#Linux`, `#security`, `#disk-encryption`, `#LUKS`, `#kernel`

---

<a id="item-8"></a>
## [Podman 6.0.0 发布，带来重大网络改进](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman 6.0.0 版本发布，引入了重大的网络改进，并进一步巩固了其作为安全、无守护进程的 Docker 替代方案的地位。 此次发布可能推动 Podman 的进一步采用，特别是对于那些寻求更安全、无守护进程容器运行时的用户，社区报告显示从 Docker Compose 迁移非常顺畅。 该版本包含重大的网络改进，社区成员报告从 Docker Compose 迁移无需任何更改，但存在一些可能导致问题的细微差异。

hackernews · soheilpro · 7月2日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48762098)

**背景**: Podman 是一种无需中央守护进程即可运行的容器引擎，相比 Docker 增强了安全性。Podman 中的 Quadlet 功能允许将容器作为 systemd 单元运行，简化了部署。Docker Compose 是定义多容器应用程序的流行工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.redhat.com/blog/2018/11/20/buildah-podman-containers-without-daemons">Containers without daemons: Podman and Buildah available in RHEL 7.6 and RHEL 8 | Red Hat Developer</a></li>
<li><a href="https://pocketcmds.com/skills/podman/podman-compose-migration">Migrate from Docker Compose to Podman - Podman AI Skill ...</a></li>
<li><a href="https://www.redhat.com/en/blog/compose-podman-pods">Moving from docker-compose to Podman pods - Enable Sysadmin</a></li>

</ul>
</details>

**社区讨论**: 社区表达了强烈的热情，有人称 Podman 是“明显更好的实现”。用户分享了积极的迁移经验，但一位评论者警告称可能会出现细微的不兼容问题。Quadlet 因其在无根容器托管中的实用性而受到称赞。

**标签**: `#containers`, `#podman`, `#devops`, `#container-runtime`, `#networking`

---

<a id="item-9"></a>
## [Immich 3.0 重大版本发布](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

Immich 3.0 是自托管照片和视频管理平台的主要版本更新，带来了重大改进和新功能。 此版本引发了大量社区讨论，表明对 Google Photos 和 Apple Photos 等云服务的自托管替代方案有浓厚兴趣，凸显了对隐私优先的照片管理解决方案日益增长的需求。 Hacker News 上的讨论（151 分，63 条评论）突出了用户体验、与 Ente 等替代方案的比较以及 iOS 同步可靠性等实际问题；重大版本标签暗示可能有破坏性变更或大量新功能。

hackernews · hashier · 7月2日 14:13 · [社区讨论](https://news.ycombinator.com/item?id=48761944)

**背景**: Immich 是一款自托管照片和视频备份解决方案，允许用户在自己的服务器上存储和管理媒体，提供隐私和控制权。它常与 Google Photos 和 Apple Photos 等专有服务进行比较。该项目是开源的，且正在积极开发中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://immich.app/">Immich</a></li>
<li><a href="https://grokipedia.com/page/Immich">Immich</a></li>

</ul>
</details>

**社区讨论**: 用户反馈不一：一些用户称赞 Immich 结合 VPN 使用是 Apple/Google Photos 的“无脑替代品”，而另一些用户则报告 iOS 同步数天未能完成等问题。部分用户因加密偏好选择了 Ente 等替代方案。总体情绪积极，尽管存在一些不足之处，但用户对该项目的能力表示赞赏。

**标签**: `#self-hosting`, `#photo management`, `#open source`, `#immich`, `#Hacker News`

---

<a id="item-10"></a>
## [Anthropic 招揽诺奖得主与伯克利 CS 系主任](https://mp.weixin.qq.com/s?__biz=MzI3MTA0MTk1MA==&mid=2652710327&idx=2&sn=721e0bd065a568d0ee34ffbfa5e859fc) ⭐️ 8.0/10

Anthropic 在两周内招募了一位诺贝尔奖得主和加州大学伯克利分校计算机科学系主任，这是一次重大的人才争夺行动。 此举加剧了领先公司对顶级 AI 人才的争夺，可能加速 Anthropic 的研发能力，巩固其在人工智能竞赛中的地位。 招聘对象包括一位相关领域的诺贝尔奖得主和伯克利 CS 系主任，后者以对理论计算机科学和 AI 安全的重要贡献而闻名。

rss · 新智元 · 7月2日 04:32

**背景**: Anthropic 是一家由前 OpenAI 研究员创立的 AI 安全初创公司，专注于开发安全且有益的 AI 系统。招聘顶尖学术人才反映了 AI 公司为获得竞争优势而在研究上大举投资的普遍趋势。

**标签**: `#AI`, `#talent acquisition`, `#Anthropic`, `#Nobel laureate`, `#Berkeley`

---

<a id="item-11"></a>
## [CISA 警告 ST Engineering iDirect iQ 系列终端存在漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-183-01) ⭐️ 8.0/10

CISA 发布了公告（ICSA-26-183-01），警告 ST Engineering iDirect iQ 系列终端存在高严重性漏洞（CVSS 8.1），包括关键功能缺少身份验证和跨站请求伪造，影响版本至 4.5.2.1。 这些漏洞可能允许未经认证的攻击者获取敏感设备信息并在卫星网络中冒充终端，可能影响全球关键通信基础设施。 该公告涵盖三个终端系列（Evolution iQ、3315 和 9 系列），均运行固件版本<=4.5.2.1，ST Engineering iDirect 已发布修复版本 4.5.2.2。

rss · CISA Cybersecurity Advisories · 7月2日 12:00

**背景**: 工业控制系统（ICS）漏洞常被攻击者利用以破坏关键基础设施。CISA 定期发布公告帮助组织识别和缓解此类风险。通用安全咨询框架（CSAF）是一种用于共享安全公告的机器可读格式，CISA 使用该格式发布这些警报。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#ICS`, `#CISA`, `#STEngineering`

---

<a id="item-12"></a>
## [Umbrij 恶意软件利用 OAuth 静默访问 Gmail](https://thehackernews.com/2026/07/toddycat-linked-umbrij-malware-abuses.html) ⭐️ 8.0/10

卡巴斯基研究人员发现一种名为 Umbrij 的新型恶意软件，归因于 ToddyCat 威胁行为者，该软件滥用 OAuth 令牌，通过 Google API 秘密访问受害者的 Gmail 通信。 这种技术使攻击者能够绕过传统的电子邮件安全措施，在不触发警报的情况下持续访问企业邮件，对依赖 Gmail 进行商业通信的组织构成重大威胁。 该活动专门针对企业 Gmail 账户，通过恶意软件获取 OAuth 2.0 授权令牌，进而通过 Google API 访问电子邮件，使得标准安全工具难以检测。

rss · The Hacker News · 7月2日 13:04

**背景**: ToddyCat 是一个至少从 2020 年开始活跃的高级持续性威胁（APT）组织，以使用定制恶意软件针对欧洲和亚洲的政府和军事实体而闻名。OAuth 是一种基于令牌的开放认证标准，允许第三方应用程序在不暴露密码的情况下访问用户数据。通过滥用 OAuth，只要令牌有效，Umbrij 即使在受害者更改密码后也能保持访问权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/toddycat-linked-umbrij-malware-abuses.html">ToddyCat-Linked Umbrij Malware Abuses OAuth to Access Gmail via Google API</a></li>
<li><a href="https://attack.mitre.org/groups/G1022/">ToddyCat, Group G1022 | MITRE ATT&CK®</a></li>

</ul>
</details>

**标签**: `#malware`, `#cybersecurity`, `#OAuth`, `#threat-actor`, `#email-security`

---

<a id="item-13"></a>
## [新 ChocoPoC RAT 通过假冒 GitHub PoC 仓库攻击安全研究人员](https://thehackernews.com/2026/07/new-chocopoc-rat-targets-vulnerability.html) ⭐️ 8.0/10

攻击者通过 GitHub 上的虚假概念验证(PoC)漏洞利用仓库传播名为 ChocoPoC 的新型 Python 远程访问木马(RAT)，专门针对安全研究人员。 此攻击活动意义重大，因为它利用了研究人员对共享漏洞利用代码的信任，可能危及网络安全专业人士的凭证和系统。这突显了一个日益增长的威胁向量：攻击者将安全社区自身的工具武器化来对付他们。 该恶意软件可窃取保存的密码、浏览器 cookie 和文件，并向攻击者提供对受害者机器的远程 Shell 访问权限。这些 PoC 仓库声称利用近期热门 CVE 漏洞来诱骗目标。

rss · The Hacker News · 7月2日 07:24

**背景**: 概念验证(PoC)漏洞利用是展示漏洞的代码片段，研究人员通常在 GitHub 等平台上共享。远程访问木马(RAT)是允许攻击者远程控制受感染系统的恶意软件。此攻击通过伪装成验证安全漏洞来诱骗研究人员运行恶意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/new-chocopoc-rat-targets-vulnerability.html">New ChocoPoC RAT Targets Vulnerability Researchers via Fake ...</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/new-chocopoc-malware-targets-researchers-via-trojanized-poc-exploits/">New ChocoPoC malware targets researchers via trojanized PoC exploits</a></li>
<li><a href="https://www.sekoia.com/blog/dont-eat-the-chocopocs-how-vulnerability-researchers-were-repeatedly-targeted-by-trojanised-exploits">Don’t eat the ChocoPoCs! How vulnerability researchers were repeatedly targeted by trojanised exploits</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#RAT`, `#social engineering`, `#GitHub`

---

<a id="item-14"></a>
## [SharePoint RCE CVE-2026-45659 被纳入 CISA KEV](https://thehackernews.com/2026/07/sharepoint-rce-cve-2026-45659-added-to.html) ⭐️ 8.0/10

由于存在积极利用的证据，CISA 已将 Microsoft SharePoint Server 中的一个高危远程代码执行漏洞 CVE-2026-45659 添加到其已知被利用漏洞（KEV）目录中。 该漏洞对使用 SharePoint 的组织构成严重风险，因为它可被远程利用来执行任意代码，而将其纳入 CISA 的 KEV 目录更突显了立即修补的紧迫性。 该漏洞的 CVSS 评分为 8.8，源于对不可信数据的反序列化，微软已于 2026 年 5 月发布补丁。

rss · The Hacker News · 7月2日 05:46

**背景**: CISA 的已知被利用漏洞（KEV）目录列出了已在野外被积极利用的漏洞，要求联邦机构在指定截止日期前修复。反序列化漏洞发生在应用程序反序列化不可信数据时，攻击者可操控序列化对象以执行任意代码或实施其他恶意行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/52-devops/cisa-kev-catalog">GitHub - 52-devops/ cisa - kev - catalog : U.S. CISA Known Exploited...</a></li>
<li><a href="https://portswigger.net/web-security/deserialization">Insecure deserialization | Web Security Academy - PortSwigger</a></li>

</ul>
</details>

**标签**: `#security`, `#CVE`, `#SharePoint`, `#RCE`, `#CISA`

---

<a id="item-15"></a>
## [谷歌对欧盟 41 亿欧元罚款的最终上诉被驳回](https://www.bleepingcomputer.com/news/legal/google-loses-final-appeal-to-overturn-41-billion-eu-fine/) ⭐️ 8.0/10

欧盟法院（CJEU）驳回了谷歌对 41 亿欧元反垄断罚款的最终上诉，该罚款源于谷歌利用安卓系统非法推广其 Chrome 浏览器和搜索服务。 这一具有里程碑意义的裁决维持了历史上最大的一笔反垄断罚款之一，强化了欧盟遏制科技垄断的立场，并可能为未来的数字平台监管树立先例。 41 亿欧元的罚款最初于 2018 年开处，涉及谷歌要求安卓制造商预装谷歌搜索和 Chrome 作为授权 Google Play 商店的条件。

rss · BleepingComputer · 7月2日 15:18

**背景**: 欧盟反垄断案的核心是谷歌涉嫌滥用其在移动操作系统市场的主导地位。通过将 Google Play 商店的授权与预装其搜索和浏览器应用捆绑在一起，谷歌被指控抑制了竞争和消费者选择。安卓是全球使用最广泛的移动操作系统，这使得此案对科技行业尤为重要。

**标签**: `#antitrust`, `#Google`, `#EU`, `#regulation`, `#Android`

---

<a id="item-16"></a>
## [ConsentFix 和 ClickFix：数秒内劫持 Microsoft 365 账户](https://www.bleepingcomputer.com/news/security/consentfix-and-clickfix-how-microsoft-365-accounts-are-hijacked-in-3-seconds/) ⭐️ 8.0/10

名为 ConsentFix 和 ClickFix 的新型攻击技术利用 OAuth 授权流程和伪造提示窃取 Microsoft 365 身份验证令牌，从而绕过多因素认证（MFA）。这些攻击可在三秒内攻陷账户。 这些攻击表明仅靠 MFA 不足以防御复杂的基于 OAuth 的钓鱼，对依赖 Microsoft 365 的组织构成严重威胁。它们凸显了采用条件访问和授权策略等更强身份安全措施的必要性。 ConsentFix 诱骗用户向恶意应用授予 OAuth 权限，而 ClickFix 使用伪造的“修复”提示执行恶意命令。这两种技术都避开了传统钓鱼指标，即使在启用 MFA 的情况下也能攻陷账户。

rss · BleepingComputer · 7月2日 14:00

**背景**: OAuth 是一种基于令牌的开放认证标准，允许第三方应用在不共享密码的情况下访问资源。攻击者通过创建恶意应用请求用户授权来滥用 OAuth，然后使用令牌访问账户。ClickFix 是一种社会工程技术，用户被诱骗复制粘贴命令以“修复”假问题，通常导致恶意软件执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mitiga.io/blog/consentfix-oauth-phishing-explained-how-token-based-attacks-bypass-mfa-in-microsoft-entra-id">ConsentFix OAuth Phishing Explained: How Token-Based Attacks ...</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2025/08/21/think-before-you-clickfix-analyzing-the-clickfix-social-engineering-technique/">Think before you Click(Fix): Analyzing the ClickFix social engineering technique | Microsoft Security Blog</a></li>

</ul>
</details>

**标签**: `#security`, `#Microsoft 365`, `#MFA bypass`, `#OAuth`, `#phishing`

---

<a id="item-17"></a>
## [思科确认攻击者利用 Unified CM 漏洞](https://www.bleepingcomputer.com/news/security/cisco-finally-confirms-attackers-exploiting-unified-cm-flaw/) ⭐️ 8.0/10

思科确认，攻击者正在积极利用统一通信管理器（Unified CM）中的一个漏洞，该漏洞已于 6 月初修复。 这很重要，因为 Unified CM 是广泛使用的企业级 VoIP 系统，拥有超过 3000 万用户，主动利用意味着尚未应用补丁的组织面临被入侵的风险。 该漏洞已于 6 月修复，但思科直到现在才确认被利用；该漏洞的具体技术细节尚未披露。

rss · BleepingComputer · 7月2日 11:35

**背景**: Cisco Unified Communications Manager (CUCM) 是一个本地呼叫控制平台，用于语音、视频和协作，广泛部署于大型企业。它运行在 Linux 服务器上，使用 IBM Informix 数据库，最多支持 3 万个 IP 电话。对此类关键基础设施的安全补丁对于防止被利用至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisco.com/c/en/us/support/unified-communications/unified-communications-manager-callmanager/series.html">Cisco Unified Communications Manager (CallManager) Cisco Unified Communications Manager (UCM) | Market-leading ... Cisco Unified Communications Manager Version 15 What is Cisco Unified Communications Manager (CUCM)? - GetVoIP Cisco Unified Communications Manager (CUCM) | A Guide Cisco Unified Communications Manager (CUCM) - learncisco.net Cisco Unified Communications Manager 15</a></li>
<li><a href="https://www.webex.com/us/en/products/suite/enterprise-cloud-calling/CUCM.html">Cisco Unified Communications Manager (UCM) | Market-leading ...</a></li>

</ul>
</details>

**标签**: `#security`, `#cisco`, `#vulnerability`, `#unified-communications`

---

<a id="item-18"></a>
## [PeerTube：免费的、去中心化的 YouTube 替代方案受关注](https://github.com/Chocobozzz/PeerTube) ⭐️ 7.0/10

PeerTube，一个使用 ActivityPub 联邦协议和 P2P 技术的开源去中心化视频平台，在 Hacker News 上引发了大量讨论，获得 487 个赞和 218 条评论。 这场讨论凸显了人们对去中心化视频平台（如 PeerTube）作为 YouTube 等中心化平台替代方案的兴趣日益增长，同时也揭示了实现广泛采用所需解决的关键挑战，如盈利模式和内容发现性。 PeerTube 利用 WebTorrent 实现点对点流媒体传输，以减轻服务器负载；并通过 ActivityPub 协议加入联邦宇宙（Fediverse），支持不同实例之间的通信。该项目自 2017 年起由法国非营利组织 Framasoft 维护。

hackernews · doener · 7月2日 11:17 · [社区讨论](https://news.ycombinator.com/item?id=48759634)

**背景**: PeerTube 是一个免费开源的视频平台，任何人都可以搭建自己的实例。与 YouTube 不同，它是去中心化的：每个实例独立运行，但可以通过 ActivityPub 协议进行联邦（互联互通），不同实例的用户可以订阅和互动。此外，当观看热门视频时，观众可以通过点对点技术分享加载负担，从而降低托管方的带宽成本。这种架构旨在让内容创作者和社群对自己的内容有更多控制权，而不必依赖单一的企业实体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PeerTube">PeerTube</a></li>
<li><a href="https://joinpeertube.org/">What is PeerTube? | JoinPeerTube</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fediverse">Fediverse - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论中流露出复杂情绪：一位专业 YouTuber 强调了盈利困难和较高的制作成本；其他人则指出当前 PeerTube 实例缺乏内容和观众，不过也有人认为它对开源教程很有用。还有评论称赞了 PeerTube 的 P2P 分享技术，但对能否克服像 TikTok 这样的社交习惯表示怀疑。

**标签**: `#decentralized`, `#video hosting`, `#open source`, `#federation`, `#PeerTube`

---

<a id="item-19"></a>
## [如何向陌生人寻求帮助](https://pradyuprasad.com/writings/how-to-ask-for-help/) ⭐️ 7.0/10

这篇文章提供了一份实用指南，讲解如何有效向陌生人寻求帮助，强调展示个人努力（proof of work）和沟通简洁的重要性。 这很重要，因为许多专业人士在建立人脉和寻求帮助时感到困难；采用这些技巧可以提高回复率，并减少请求方和帮助方之间的摩擦。 关键建议包括先展示自己已经做过研究、个性化每个请求以及尊重对方的时间。该文章主要面向软件工程师，但也适用于其他领域。

hackernews · FigurativeVoid · 7月2日 13:19 · [社区讨论](https://news.ycombinator.com/item?id=48761118)

**背景**: 在职业社交中，向陌生人寻求帮助很常见，但往往效果不佳。'Proof of work' 指的是展示你已自行尝试解决问题，这传递了严肃认真的态度，也体现了对帮助者时间的尊重。这一概念是文章建议的核心。

**社区讨论**: 评论者普遍认同核心建议，分享了个人经历，并强调真诚的努力比华丽的姿态更重要。一些人指出，准确估计他人被请求帮助的频率很困难，需要不断校准。

**标签**: `#career`, `#communication`, `#networking`, `#professional development`

---

<a id="item-20"></a>
## [用 DSPy 改进 Datasette Agent 的 SQL 提示](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison 使用 DSPy 框架评估并改进了 Datasette Agent 的 SQL 系统提示，发现了列名猜测等问题并提出了改进建议。 这展示了 DSPy 在优化 LLM 系统提示方面的实际应用，有望让 AI 代理生成更可靠、更准确的 SQL 查询。 该实验通过 Claude Code 使用了 GPT-4.1 mini 和 nano 模型，一个关键发现是 schema 列表应包含列名，且应软化关于不调用 describe_table 的建议以避免猜测。

rss · Simon Willison · 7月2日 18:25

**背景**: DSPy 是一个用于编程（而非提示）语言模型的框架，可对提示和权重进行算法优化。Datasette Agent 是 Datasette 的一个 AI 助手插件，允许用户用自然语言查询 SQLite 数据库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp/dspy: DSPy: The framework for programming—not prompting—language models</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent, an extensible AI assistant for Datasette - Datasette Blog</a></li>
<li><a href="https://dspy.ai/">DSPy</a></li>

</ul>
</details>

**标签**: `#DSPy`, `#prompt engineering`, `#SQL`, `#Datasette`, `#AI agents`

---