---
layout: default
title: "Horizon Summary: 2026-08-08 (ZH)"
date: 2026-08-08
lang: zh
---

> 从 66 条内容中筛选出 20 条重要资讯。

---

1. [DeepSeek V4 Flash 0731 发布：更便宜、更快、推理更强](#item-1)
2. [WordPress 预认证 XSS 漏洞 CVE-2026-64638 可导致 PHP 代码执行](#item-2)
3. [18 年历史的 Linux SCTP 漏洞可致本地提权与容器逃逸](#item-3)
4. [恶意软件可滥用 Windows Hello for Business 密钥获取持久 Entra ID 访问权限](#item-4)
5. [tl;dv 漏洞：缺少租户隔离导致 181,874 场会议数据泄露](#item-5)
6. [汇编耻辱堂：展示最慢、最诡异的 x86 指令](#item-6)
7. [科技从业者集体丧失职业信念，倦怠成普遍现象](#item-7)
8. [OpenAI 宣布针对高级 AI 的新网络安全控制措施](#item-8)
9. [Oracle 禁止 OpenJDK 接受 AI 生成代码](#item-9)
10. [基于 Rust 的 pgrust 查询引擎让 Postgres 分析查询提速上百倍](#item-10)
11. [据报道 2027 年内存产能已售罄，AI 推动 HBM 需求](#item-11)
12. [Kitesurf：Cloudflare 在 V8 隔离环境中的智能体优先浏览器](#item-12)
13. [在我 150 万页面的网站上与爬虫搏斗的一年](#item-13)
14. [CISA 公告揭示 CPDLC over ATN-B1 存在漏洞](#item-14)
15. [近 800 个恶意 npm 包分发跨平台木马](#item-15)
16. [新 NatJack 攻击通过操纵 NAT 表劫持 TCP 会话并欺骗 DNS](#item-16)
17. [AI 辅助的 HTTP Terminator 发现新型 HTTP desync 技术与 Apache 零日漏洞](#item-17)
18. [Claude Code 与 Gemini CLI 漏洞可让 GitHub 问题触及 CI 机密](#item-18)
19. [Metabase SQL 注入零日漏洞遭利用，客户数据被盗](#item-19)
20. [TeamPCP 被指与 2020 年以来 Redis 攻击及后续供应链活动有关](#item-20)

---

<a id="item-1"></a>
## [DeepSeek V4 Flash 0731 发布：更便宜、更快、推理更强](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 9.0/10

DeepSeek 于 2026 年 7 月 31 日发布 DeepSeek-V4-Flash-0731，这是 V4 Flash 模型经重新后训练（re-post-trained）的版本，正式结束预览。该模型在 ARC-AGI 基准上表现强劲，并将 Terminal-Bench 2.1 从 61.8% 提升至 82.7%，超越了 V4-Pro-Preview。 该模型以极低的 API 价格提供了强大的编程、推理和智能体工作流能力，让更广泛的用户能够用上高端 AI。社区反馈称它“几乎什么都能用”，这加大了对价格更昂贵的前沿模型的竞争压力。 DeepSeek-V4-Flash-0731 是一个稀疏混合专家（MoE）模型，总参数 284B，激活参数 13B，支持 100 万 token 上下文。该版本没有架构变化，目前仅更新 DeepSeek-V4-Flash API；DeepSeek 还宣布即将大幅上调价格。

hackernews · tosh · 8月7日 17:56 · [社区讨论](https://news.ycombinator.com/item?id=49214008)

**背景**: DeepSeek 是一家以开源权重和低成本高效训练著称的中国 AI 公司，其 2025 年 1 月发布 R1 模型后对西方前沿实验室形成挑战。ARC-AGI 基准常用于检验模型在新颖推理任务上的表现，而非对知识的记忆，因此在该基准上表现突出被视为真实推理能力的重要信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/updates/">Change Log | DeepSeek API Docs</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash-0731">DeepSeek V4 Flash 0731 - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://aitoolsrecap.com/Blog/deepseek-v4-flash-0731-review-benchmarks-2026">DeepSeek V4 Flash 0731: $0.14/M, Terminal-Bench 82.7%, Beats ...</a></li>

</ul>
</details>

**社区讨论**: 社区总体评价积极，用户称赞模型的速度、能力以及日常智能体使用中的低成本。也有人反馈出现死循环、未执行工具调用等问题，另有人提醒 DeepSeek 已宣布涨价，成本优势可能缩小。

**标签**: `#AI`, `#LLM`, `#DeepSeek`, `#model release`, `#benchmark`

---

<a id="item-2"></a>
## [WordPress 预认证 XSS 漏洞 CVE-2026-64638 可导致 PHP 代码执行](https://thehackernews.com/2026/08/new-wordpress-pre-auth-xss-could-lead.html) ⭐️ 9.0/10

WordPress 已修复 CVE-2026-64638，这是登录屏幕中影响该 CMS 所有版本的一个预认证反射型 XSS 漏洞。pwn.ai 演示了当已登录管理员访问恶意页面时，可将该漏洞升级为服务器端 PHP 代码执行的攻击链。 由于该漏洞无需认证且影响所有 WordPress 版本，修复前几乎所有 WordPress 站点都处于风险之中。已演示的 XSS 到 RCE 攻击链使其尤其危险，管理员一次点击就可能导致站点被完全控制。 CVE-2026-64638 的 CVSS 评分为 8.9，是登录屏幕中的反射型 XSS 漏洞。据 OpenCVE 称，成功利用需要受害者访问恶意网站，但如果像 pwn.ai 展示的那样进行链式利用，攻击者可能完全控制受影响的 WordPress 站点。

rss · The Hacker News · 8月7日 12:56

**背景**: WordPress 是最广泛使用的内容管理系统之一，支撑着很大一部分网站。反射型 XSS 是一种漏洞，攻击者提供的脚本通过 Web 应用在响应中反射，并在受害者浏览器中执行；预认证意味着无需登录即可触发该漏洞端点。XSS 本身通常只在浏览器中运行，但与其他弱点链式利用时可在服务器上实现远程代码执行。管理员持有高权限会话，因此成为此类攻击的关键目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://app.opencve.io/cve/CVE-2026-64638">CVE-2026-64638 - Vulnerability Details - OpenCVE</a></li>
<li><a href="https://pwn.ai/blog/xss2shell">XSS2Shell: WordPress Preauth XSS to RCE Chain (CVE-2026-64638)</a></li>

</ul>
</details>

**标签**: `#security`, `#wordpress`, `#xss`, `#rce`, `#cve`

---

<a id="item-3"></a>
## [18 年历史的 Linux SCTP 漏洞可致本地提权与容器逃逸](https://thehackernews.com/2026/08/18-year-old-linux-sctp-flaw-could-let.html) ⭐️ 9.0/10

腾讯安全研究人员演示了 Linux SCTP 网络代码中一个自 2008 年就存在的释放后使用（use-after-free）漏洞，该漏洞可让本地用户获取宿主机 root 权限并逃逸容器。修复已于 8 月 3 日随稳定版内核 7.1.6、6.18.42、6.12.101 和 6.6.148 发布。 这一漏洞之所以重要，是因为 SCTP 在众多默认内核中都会启用，而该缺陷可将低权限本地访问升级为完整的宿主机接管，即使攻击者位于容器内部也能实现。运行旧版内核且 SCTP 可达的组织应立即进行稳定版内核更新。 该漏洞是 Linux SCTP 网络代码中的一个释放后使用（use-after-free）问题，利用条件要求攻击者能够触达 SCTP 协议。修复已包含在 8 月 3 日发布的稳定版内核 7.1.6、6.18.42、6.12.101 和 6.6.148 中，较旧内核必须升级到这些版本。

rss · The Hacker News · 8月7日 11:10

**背景**: SCTP（流控制传输协议，Stream Control Transmission Protocol）是一种传输层协议，IP 协议号为 132，提供可靠、面向消息的通信，常用于电话和信令类应用。释放后使用（use-after-free）是一种内存破坏缺陷，指程序在内存被释放后仍继续引用该内存；这类漏洞在 C/C++ 代码中很常见，通常可导致远程代码执行或权限提升。容器逃逸则指攻击者突破容器命名空间/cgroups 所提供的隔离，进而访问宿主机操作系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.iana.org/assignments/protocol-numbers/protocol-numbers.xhtml">Protocol Numbers</a></li>
<li><a href="https://medium.com/@duliprb/use-after-free-the-silent-killer-takes-over-the-memory-of-operating-system-ecb0271e1a3a">Use - After - Free : The silent killer takes over the memory of... | Medium</a></li>
<li><a href="https://www.aquasec.com/cloud-native-academy/container-security/container-escape/">What Is Container Escape? - Aqua</a></li>

</ul>
</details>

**标签**: `#Linux kernel`, `#SCTP`, `#privilege escalation`, `#container escape`, `#vulnerability`

---

<a id="item-4"></a>
## [恶意软件可滥用 Windows Hello for Business 密钥获取持久 Entra ID 访问权限](https://thehackernews.com/2026/08/malware-can-abuse-windows-hello-for.html) ⭐️ 9.0/10

安全研究员 Dirk-jan Mollema 演示了已在登录的 Windows 会话中运行的恶意软件如何悄然使用受害者的 Windows Hello for Business 密钥向 Microsoft Entra ID 进行身份验证。该攻击可让攻击者注册受控设备、获取主刷新令牌 (PRT)，并添加更多身份验证方法，从而可能获得持久的云访问权限。 这很重要，因为 Windows Hello for Business 作为抗钓鱼身份验证方法在企业环境中广泛部署。该技术将本地设备入侵转化为长期的云身份入侵，削弱了无密码身份验证的安全承诺，迫使组织重新审视条件访问和设备信任策略。 该演示依赖于恶意软件在已登录会话中已具备代码执行能力，这通常通过初始访问或权限提升实现。微软尚未发布补丁，攻击的有效性取决于允许设备注册和附加身份验证方法注册的租户策略。

rss · The Hacker News · 8月7日 08:52

**背景**: Windows Hello for Business 是 Windows Hello 的企业级扩展，通过生物识别或 PIN 提供无密码、抗钓鱼登录，密钥通常由 TPM 保护。主刷新令牌 (PRT) 是微软发布的、绑定到设备的令牌，用于获取云应用程序的访问令牌。Entra 设备注册是云端身份验证的前提，允许设备加入 Microsoft Entra ID，从而实现单一登录和条件访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/entra/identity/devices/concept-primary-refresh-token">Understanding Primary Refresh Token (PRT) in Microsoft Entra ID - Microsoft Entra ID | Microsoft Learn</a></li>
<li><a href="https://learn.microsoft.com/en-us/entra/identity/devices/device-registration-how-it-works">How Microsoft Entra device registration works - Microsoft ...</a></li>
<li><a href="https://www.andykemp.com/2026/06/01/windows-hello-for-business-is-more-than-a-login-method/">Windows Hello for Business Is More Than a Login Method</a></li>

</ul>
</details>

**标签**: `#security`, `#Windows Hello`, `#Entra ID`, `#malware`, `#authentication`

---

<a id="item-5"></a>
## [tl;dv 漏洞：缺少租户隔离导致 181,874 场会议数据泄露](https://www.reddit.com/r/netsec/comments/1vi8ibp/tldv_too_lazy_didnt_validate_181874_meetings_left/) ⭐️ 9.0/10

安全研究员 kochurshak 发现 tl;dv 的 Firestore 数据库缺少租户隔离，任何经过身份验证的用户都能查询所有会议记录。这导致 181,874 场会议、84,312 名用户的数据被暴露，包括电子邮件和可加入的会议链接。 这是广泛使用的会议记录工具中的严重隐私漏洞，任何用户都能访问敏感的会议元数据，甚至可能加入他人的会议。这凸显了在多租户云应用中强制实施租户隔离的重要性。 存在漏洞的 Firestore 'meetings' 集合缺少租户隔离，因此每条记录都会暴露创建者的电子邮件、会议 ID（即可加入的 Google Meet 或 Teams 房间）、提供商、录制状态和时间戳。研究员发现 181,874 条会议记录，涉及 35,003 个电子邮件域。

reddit · r/netsec · /u/kochurshak · 8月7日 18:23

**背景**: tl;dv 是一款 AI 会议记录工具，可在 Zoom、Google Meet 和 Microsoft Teams 上录制、转录并总结会议。租户隔离是安全控制措施，用于在多租户 SaaS 架构中隔离不同客户的数据；缺少它时，一个租户可以访问另一个租户的数据。Firestore 是 Google Cloud 灵活、可扩展的 NoSQL 数据库。这一漏洞凸显了共享数据库中缺少租户隔离的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tldv.io/">tl;dv - AI Meeting Notetaker for Zoom, Google Meet & Teams</a></li>
<li><a href="https://owasp.org/www-project-cloud-tenant-isolation/">OWASP Cloud Tenant Isolation</a></li>
<li><a href="https://firebase.google.com/docs/firestore/">Firestore | Firebase</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#tenant-isolation`, `#privacy`, `#firestore`

---

<a id="item-6"></a>
## [汇编耻辱堂：展示最慢、最诡异的 x86 指令](https://github.com/xoreaxeaxeax/asm-hall-of-shame) ⭐️ 8.0/10

xoreaxeaxeax 创建了一个名为“Assembly Hall of Shame”的新 GitHub 仓库，收集了一系列怪异且极其缓慢的 x86 指令排行榜，衡量单指令性能的绝对下限。该集合突显了不寻常的 CPU 行为，包括对一个 ACPI I/O 端口进行 12 毫秒写入等条目。 该项目颠覆了传统性能分析的方向，揭示了被忽视的 CPU 边缘情况，这些情况可能具有安全影响，例如利用慢速指令来破坏系统管理模式（SMM）。它对底层系统程序员和安全研究人员很有吸引力，兼具娱乐和教育价值，并引发了关于微架构行为的讨论。 该仓库的规则规定，被捕获、模拟或虚拟化的指令只能计时捕获过程，而不能计时处理程序，这引发了关于某些排行榜条目（如 12ms ACPI 写入）是否实际上在陷入 SMM 的争论。作者还以其他相关项目闻名，包括一个仅生成“mov”指令的编译器，以及一个名为“repsych”的工具，该工具故意扰乱控制流以迷惑反汇编器。

hackernews · piotrgrabowski · 8月7日 18:01 · [社区讨论](https://news.ycombinator.com/item?id=49214098)

**背景**: x86 指令集包含许多有文档记录和无文档记录的指令，其中一些指令由于微架构怪癖或陷入 SMM 等固件处理程序而表现出极慢的执行速度。性能分析通常专注于优化代码以使其尽可能快地运行，但该项目反其道而行之，寻找最慢的单指令行为。理解这些异常现象与底层安全研究相关，因为时序和微架构副作用可能被利用于攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xoreaxeaxeax/asm-hall-of-shame">Assembly Hall of Shame - GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Illegal_opcode">Illegal opcode - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论中有人链接了同一位作者关于利用慢速指令破解 SMI 的相关研究，并就 ACPI I/O 端口写入是否真的陷入 SMM 展开了辩论。其他评论者将其与 Core War 编程游戏相提并论，开玩笑说 NOP 应该排在第一位，因为它相对于其操作来说无限慢，并提到了作者其他非常规的编译器项目。

**标签**: `#x86`, `#assembly`, `#low-level`, `#security`, `#hardware`

---

<a id="item-7"></a>
## [科技从业者集体丧失职业信念，倦怠成普遍现象](https://www.noemamag.com/why-is-everyone-in-tech-so-sad/) ⭐️ 8.0/10

《Noema》杂志的这篇文章审视了科技从业者普遍丧失职业信念与目标感的现象，并引发了一场包含 495 条评论的激烈社区讨论。文章直接提出“为什么科技行业人人都这么悲伤”的问题，反映出该行业日益加深的意义危机。 这一现象影响重大，因为它标志着科技行业正在发生显著的文化转变：倦怠与犬儒心态在支撑现代经济的劳动力中日益普遍。这可能影响人才留存、创新能力，以及整个一代劳动者的心理健康。 文章标题对科技从业者的悲伤提出质疑，而社区评论则提供了关于热情消退、网络毒性，以及与印刷业等技能行业衰落的历史类比等个人轶事。尽管所提供的内容缺少完整正文，但高参与度和多样化的观点凸显了该话题的深刻共鸣。

hackernews · RickJWagner · 8月7日 12:42 · [社区讨论](https://news.ycombinator.com/item?id=49209539)

**背景**: 科技行业长期以来被视为充满机遇与创新的领域，但近年来，关于职业倦怠、裁员和意义感缺失的报道日益增多。印刷业等历史案例表明，整个职业可能会因技术变革和经济压力而失去立足之地，这为当前科技行业的幻灭提供了一个警示性的类比。

**社区讨论**: 评论者将之与印刷工等技能行业的衰落相类比，强调网络世界的毒性，并分享自己在该领域工作数十年后热情消退的经历。也有评论批评文章的语气，一位读者认为其中的幸灾乐祸令人不适，尽管他承认这场讨论具有社会价值。

**标签**: `#tech-culture`, `#mental-health`, `#career-satisfaction`, `#software-industry`, `#burnout`

---

<a id="item-8"></a>
## [OpenAI 宣布针对高级 AI 的新网络安全控制措施](https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/) ⭐️ 8.0/10

OpenAI 发布了一篇新文章，阐述其如何应对高级 AI 网络能力，分享了针对 Astra 系统的初步网络安全评估，并宣布对更高能力模型实施更严格的安全控制。这些措施包括隔离测试环境和额外的安全防护。 这很重要，因为前沿 AI 模型在进攻性网络操作方面的能力越来越强，OpenAI 的做法可能影响整个行业如何管理这些风险。这也是对日益增长的政策关注（例如白宫关于 AI 网络能力的行政命令）的回应。 该公告强调了对更高能力模型实施更严格的安全控制，例如隔离测试环境，并包含对 OpenAI 的 Astra 系统的初步网络安全评估。OpenAI 还概述了管理高级 AI 网络能力的研究方向，但摘要中没有完全披露具体技术细节。

hackernews · OpenAI Blog · 8月7日 16:39 · [社区讨论](https://news.ycombinator.com/item?id=49213029)

**背景**: 高级 AI 网络能力指的是前沿 AI 模型执行漏洞发现与利用等进攻性安全任务的能力。随着模型变得越来越强大，OpenAI 和 Google DeepMind 等实验室正在评估这些风险并制定基准和安全措施。例如，DeepMind 发布了进攻性网络能力基准，白宫也发布了关于评估 AI 网络能力的行政命令。OpenAI 的新文章是随着 AI 能力进步而加强网络韧性这一更广泛趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/">Promoting Advanced Artificial Intelligence Innovation and ...</a></li>
<li><a href="https://deepmind.google/blog/evaluating-potential-cybersecurity-threats-of-advanced-ai/">Evaluating potential cybersecurity threats of advanced AI</a></li>
<li><a href="https://openai.com/index/strengthening-cyber-resilience/">Strengthening cyber resilience as AI capabilities advance</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一。一些评论者分享了积极经验，例如 Sol 能快速发现漏洞，而另一些则对 OpenAI 的透明度表示怀疑，认为该公司从未披露第一起事件的细节，更严格的控制不过是做样子。一位评论者还提到了 DEF CON 演讲中关于训练期间代理通信的更多技术细节，另一位则建议将系统迁回本地以避免依赖这些公司。

**标签**: `#AI security`, `#cyber capabilities`, `#OpenAI`, `#vulnerability discovery`, `#agent behavior`

---

<a id="item-9"></a>
## [Oracle 禁止 OpenJDK 接受 AI 生成代码](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 8.0/10

Oracle 已推出临时政策，禁止在 OpenJDK 贡献中使用生成式 AI 编写的代码。该政策已发布在 OpenJDK 的法律页面上，正式完整政策仍在起草中。 这一政策意义重大，因为 OpenJDK 是 Java SE 的参考实现，被数百万开发者和企业所依赖，它为大型开源项目如何处理 AI 生成的贡献树立了先例。同时，它也凸显了业界对代码来源、版权以及 AI 辅助开发中法律风险日益增长的担忧。 临时政策适用于所有 OpenJDK 贡献，并将由 Oracle 法律团队起草的最终版本取代。据 InfoQ 报道，贡献者不久后需要在自动拉取请求审查系统 Skara 中勾选复选框，以确认其代码符合该 AI 政策。

hackernews · delduca · 8月7日 17:36 · [社区讨论](https://news.ycombinator.com/item?id=49213754)

**背景**: OpenJDK 是 Java 平台标准版的免费开源实现，最初由 Sun Microsystems 发起，现由 Oracle 赞助。AI 生成的代码引发了来源问题，因为模型可能复现来源不明或不兼容的代码，从而带来版权和许可方面的潜在责任。Oracle 在 Java 领域有激进诉讼的历史，例如其与 Google 的长期诉讼案件，这有助于解释其谨慎的法律立场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openjdk.org/legal/ai">OpenJDK Interim Policy on Generative AI</a></li>
<li><a href="https://www.infoq.com/news/2026/06/oracle-genai-policies/">Oracle's OpenJDK Bans Generative AI Contributions While... - InfoQ</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenJDK">OpenJDK</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：一些人认为考虑到 Oracle 的版权历史，这一政策是明智的法律预防措施；另一些人则讽刺 Oracle 一边推广 AI 一边禁止 AI 代码的矛盾。还有人指出这会增加志愿评审者的工作负担；也有用户错误地认为 OpenJDK 是纯社区项目而非 Oracle 赞助。

**标签**: `#OpenJDK`, `#Oracle`, `#AI-generated code`, `#Open Source Policy`, `#Licensing`

---

<a id="item-10"></a>
## [基于 Rust 的 pgrust 查询引擎让 Postgres 分析查询提速上百倍](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 8.0/10

作者发布了一篇关于 pgrust 的详细文章，pgrust 是一个基于 Rust 的查询引擎扩展，通过批处理、运算符融合和 SIMD 将 Postgres 分析工作负载加速了数百倍。作者还提到，已有超过 1000 个面向用户的函数通过形式化验证或差分模糊测试，与 Postgres 行为保持一致。 如果这些性能声明属实，pgrust 可能使 Postgres 成为当前需要专用 OLAP 数据库的分析工作负载的可行选择。它还展示了 Rust 扩展以及自适应规划等现代执行技术在 Postgres 生态中的潜力，而 Postgres 核心团队对此一直持保守态度。 该扩展基于 pgrx 框架构建，pgrx 是一个用 Rust 开发 Postgres 扩展的框架。文章重点介绍三项关键技术：将行批量组织为向量、融合运算符以减少物化开销，以及使用 SIMD 指令进行数据并行处理。作者将正确性放在首位，结合了形式化验证和差分模糊测试，但 I/O 调度器和线程池等问题仍是开放性课题。

hackernews · poly2it · 8月7日 11:00 · [社区讨论](https://news.ycombinator.com/item?id=49208535)

**背景**: PostgreSQL 传统上逐行处理数据，并针对事务型（OLTP）工作负载进行优化，因此在大型数据集上的分析查询较慢。现代分析查询引擎使用向量化执行、批处理和运算符融合等技术，以批量方式处理数据并降低开销。SIMD（单指令多数据）允许 CPU 指令并行处理多个数据点。pgrx 是一个社区框架，允许开发者用 Rust 编写安全、高性能的 Postgres 扩展，在构建自定义查询引擎和工具方面越来越受欢迎。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/pgcentralfoundation/pgrx">GitHub - pgcentralfoundation/pgrx: Build Postgres Extensions with Rust! · GitHub</a></li>
<li><a href="https://www.cs.cit.tum.de/fileadmin/w00cfj/dis/papers/inkfuse.pdf">Incremental Fusion: Unifying Compiled and Vectorized Query ...</a></li>

</ul>
</details>

**社区讨论**: 作者回应了可能出现的信任问题，强调以正确性为先，采用形式化验证和差分模糊测试。一些评论者对采用持怀疑态度，认为即使技术上更优越的扩展也不会取代受信任的 Postgres 核心；另一些人对自适应规划感到兴奋，希望该项目能验证该技术。还有用户询问 I/O 调度和“吵闹邻居”问题，而文章似乎并未完全解答这些问题。

**标签**: `#Postgres`, `#Rust`, `#Query-Engine`, `#Performance`, `#SIMD`

---

<a id="item-11"></a>
## [据报道 2027 年内存产能已售罄，AI 推动 HBM 需求](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

据报道，受 AI 需求和高带宽内存（HBM）生产限制的影响，2027 年的内存产能已经售罄。这标志着内存供应短缺的又一年，延续了 DRAM 供应紧张的态势。 产能售罄标志着整个内存行业将持续面临供应紧张，可能导致消费电子、服务器和 AI 硬件价格上涨或缺货。由于内存几乎在所有计算设备中都是关键组件，这将同时影响制造商和消费者。 HBM 生产是关键因素：一个单位的 HBM 产能大约消耗相当于生产三个单位 DDR5 产能所需的晶圆量，因为 HBM 芯片因封装要求而更大。因此，HBM 产量的提升将限制非 HBM 产品（如传统 DDR5 内存）的行业供应增长。

hackernews · inigyou · 8月7日 07:58 · [社区讨论](https://news.ycombinator.com/item?id=49207236)

**背景**: 高带宽内存（HBM）是一种 3D 堆叠式同步动态随机存取存储器（SDRAM）接口，最初由三星、AMD 和 SK 海力士开发。它专为高带宽和低功耗而设计，适用于高性能计算和 AI 加速器。随着 AI 需求激增，内存制造商将更多晶圆产能分配给 HBM，从而减少了用于 PC 和服务器中广泛使用的传统 DRAM（如 DDR5）的产能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.simms.co.uk/tech-talk/what-is-hbm-high-bandwidth-memory/">What is High Bandwidth Memory ? | Simms International</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了 HBM 与 DDR5 之间的晶圆权衡，指出 HBM 每比特消耗的晶圆供应量大约是 DDR5 的三倍。一些人表达了对消费品通胀效应和囤货冲动的担忧，另一些人则提到因内存压力而对采用 AI 持犹豫态度。少数用户建议为 RAM 制定类似 USB 的标准，以便在不看重速度的场景中重新利用旧的低容量内存条。

**标签**: `#memory`, `#HBM`, `#hardware`, `#AI`, `#supply chain`

---

<a id="item-12"></a>
## [Kitesurf：Cloudflare 在 V8 隔离环境中的智能体优先浏览器](https://blog.cloudflare.com/kitesurf/) ⭐️ 8.0/10

Cloudflare 发布了 Kitesurf，这是一个为 AI 智能体设计的新型无状态、智能体优先浏览器，完全在基于 V8 隔离环境的 Workers 上运行。它基于模块化的 Blitz 浏览器引擎构建，目前处于测试阶段并可免费使用。 Kitesurf 标志着 Cloudflare 大举进入浏览器自动化和 AI 智能体基础设施领域，其开源计划可能重塑智能体与 Web 交互的方式。同时，它引发了关于 Cloudflare 的 CDN/反机器人业务与其新型智能体友好产品之间关系的质疑。 Kitesurf 是无状态、高可扩展且经济高效的浏览器，完全运行在 Workers 上；开发团队计划将其补丁开源并向上游提交给 Blitz。目前该浏览器在测试阶段免费使用，定位为‘智能体云’（Agentic Cloud）服务。

hackernews · m3h · 8月7日 10:42 · [社区讨论](https://news.ycombinator.com/item?id=49208393)

**背景**: V8 隔离环境（isolates）是 V8 JavaScript 引擎（即 Chrome 所采用的引擎）内部相互隔离的执行上下文，Cloudflare Workers 等无服务器平台利用它来安全地在单个进程中运行代码。Blitz 是一个由 Rust 编写、由 DioxusLabs 团队创建的激进模块化开源 HTML/CSS 渲染引擎，目标是成为浏览器、应用运行时等多种用途的可复用基础。所谓‘智能体优先浏览器’，是围绕 AI 智能体执行导航、点击、填写表单等任务来设计的，而不是以人类用户为中心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/kitesurf/">Introducing Kitesurf: The agent-first browser that runs in V8 ...</a></li>
<li><a href="https://developers.cloudflare.com/changelog/post/2026-08-06-kitesurf/">Introducing Kitesurf, an agent-first browser on Browser Run</a></li>
<li><a href="https://github.com/DioxusLabs/blitz">GitHub - DioxusLabs/blitz: A radically modular HTML/CSS ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者指出，Kitesurf 基于 Blitz 构建，而 Cloudflare 计划向上游合并其补丁；另一些人对 Cloudflare 的 CDN 与反机器人服务之间可能存在的冲突表示担忧。有些用户要求提供智能体在现实中的具体用例，还有人质疑 Cloudflare 是否会允许自己的浏览器实例绕过其反机器人保护。

**标签**: `#browser`, `#Cloudflare`, `#AI agents`, `#browser automation`, `#open source`

---

<a id="item-13"></a>
## [在我 150 万页面的网站上与爬虫搏斗的一年](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

作者描述了在拥有 150 万页面的网站上与爬虫搏斗一年的经历；期间机器人流量占主导，一个峰值月份成本飙升约 500%。文章中评估了 Cloudflare 防护、迁移到静态站点以及 Anubis 这类工作量证明挑战等反爬策略。 随着 AI 搜索爬虫和抓取工具给小型网站带来实实在在的成本，反爬防护正日益成为网站运营的核心问题。作者的体验凸显了把防护外包给 Cloudflare、接受成本波动、或改用工作量证明等替代方案之间的权衡。 这个网站平时的账单约为每月 90 美元，一个异常月份的费用暴涨约 500%，与 Cloudflare D1 的用量有关。评论者指出 Anubis 通过工作量证明来识别真实浏览器；另一位站长报告称，Claude-searchbot 在 72 小时内单独抓取了约 20.5 万页，仅带来 1 次引荐。

hackernews · petercooper · 8月7日 14:51 · [社区讨论](https://news.ycombinator.com/item?id=49211386)

**背景**: Web 爬虫是自动从网站提取数据的程序，常常未经许可消耗带宽和计算资源。Cloudflare Bot Management 等反机器人系统利用机器学习、行为分析和指纹识别来分类并拦截恶意流量。传统的基于规则的防御难以应对模仿人类行为的现代爬虫，因此网站所有者越来越多地求助于托管服务或通过工作量证明来验证真实浏览器软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cloudflare.com/products/bot-management/">Bot Management - Cloudflare</a></li>
<li><a href="https://www.akamai.com/glossary/what-is-bot-mitigation">What Is Bot Mitigation? | Akamai</a></li>
<li><a href="https://datadome.co/guides/scraping/scraper-crawler-bots-how-to-protect-your-website-against-intensive-scraping/">Web Scraping Protection: How to Prevent Web Scraping - DataDome</a></li>

</ul>
</details>

**社区讨论**: 评论者担心对 Cloudflare 的依赖，认为将“谁能访问网站”的决定外包给大公司会损害开放网络，用户被屏蔽时也无从申诉。也有人称赞 Anubis 的工作量证明方案适合不依赖 Cloudflare 的网站，并分享 AI 搜索爬虫消耗大量资源却几乎不带来引荐的实例。还有人注意到，作者自己也是靠抓取公开文档获取数据的“爬虫”，却抱怨爬虫。

**标签**: `#web scraping`, `#bot mitigation`, `#cloudflare`, `#site reliability`, `#security`

---

<a id="item-14"></a>
## [CISA 公告揭示 CPDLC over ATN-B1 存在漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-219-01) ⭐️ 8.0/10

CISA 发布了公告 ICSA-26-219-01，详述了 CPDLC over ATN-B1 中的五个 CVE（CVE-2025-71409 至 CVE-2025-71413），这些漏洞允许通过未经身份验证的射频链路进行未经授权的消息注入、拒绝服务条件和强制会话重置。 这些漏洞影响全球航空运输关键基础设施，可能通过增加飞行员工作负荷、延迟安全关键指令和降低态势感知来削弱运行安全裕度。虽然它们不会直接造成不安全的航空器状态，但可能被利用来迷惑飞行员或干扰地空通信。 CISA 表示目前针对这些 CVE 尚无可用缓解措施，它们仅在实验室环境中可利用且攻击复杂度较高。受影响的标准是咨询通告 90-117 数据链通信，ATN-B1 CPDLC 的所有版本都被列为受影响产品。

rss · CISA Cybersecurity Advisories · 8月7日 12:00

**背景**: 管制员-飞行员数据链通信（CPDLC）是空中交通管制员与飞行员通过数据链而非语音无线电交换消息的一种方式。ATN-B1 是用于大陆运行 CPDLC 的航空电信网络基线，尤其在欧洲飞行高度层 285 以上被强制要求使用，它依赖传统的明文、未经身份验证的甚高频射频链路。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CPDLC">CPDLC</a></li>
<li><a href="https://skybrary.aero/articles/controller-pilot-data-link-communications-cpdlc">Controller Pilot Data Link Communications (CPDLC) | SKYbrary Aviation Safety</a></li>
<li><a href="https://www.easa.europa.eu/en/faq/115361">If I use CPDLC via FANS-1/A am I compliant with the DLS IR? | EASA</a></li>

</ul>
</details>

**标签**: `#security`, `#aviation`, `#CPDLC`, `#vulnerability`, `#CISA`

---

<a id="item-15"></a>
## [近 800 个恶意 npm 包分发跨平台木马](https://thehackernews.com/2026/08/nearly-800-malicious-npm-packages.html) ⭐️ 8.0/10

研究人员发现一场恶意活动，向 npm 注册表发布了近 800 个恶意包，用于分发跨平台远程访问木马（RAT）和信息窃取程序。这些包使用 AI 生成的拼写错误（typosquatting）名称来迷惑开发者，诱导其安装。 这场大规模攻击威胁软件供应链安全，可能危害安装这些包的开发者。它凸显了开源生态系统中 AI 辅助恶意软件分发日益增长的风险。 该恶意软件针对 Windows、macOS 和 Linux 系统，具备跨平台能力。根据 OpenSourceMalware 研究员 Paul 的说法，这些包使用了“AI slop”式拼写错误或随机生成的 typosquatting 名称。

rss · The Hacker News · 8月7日 18:48

**背景**: npm 是 Node.js 的默认包管理器，开发者经常安装与合法包名称相似的包。Typosquatting 是一种常见攻击方式，恶意包使用与热门包相似的名称。RAT（远程访问木马）允许攻击者控制受感染的系统，而信息窃取程序则窃取凭证和文件等敏感数据。

**标签**: `#npm`, `#security`, `#malware`, `#supply chain`, `#open source`

---

<a id="item-16"></a>
## [新 NatJack 攻击通过操纵 NAT 表劫持 TCP 会话并欺骗 DNS](https://thehackernews.com/2026/08/new-natjack-attacks-hijack-tcp-sessions.html) ⭐️ 8.0/10

在 Black Hat USA 2026 上，研究员 Malcolm Stagg 披露了一种名为 NatJack 的新型攻击，通过操纵 NAT 连接状态来劫持活跃的 TCP 会话、伪造 DNS 响应、暴露映射端口并耗尽 NAT 表。该攻击影响包括 Windows 在内的多个独立开发实现。 NatJack 打破了人们普遍认为 NAT 能提供隔离和安全层的假设，因为它攻击的是 NAT 本身，而不是其背后的主机。这扩大了企业、ISP 和家用路由器的攻击面，可能迫使各厂商在整个生态系统中加固其 NAT 实现。 NatJack 在发布时附带两个 CVE，为厂商提供了具体的修复目标，并影响整个物理与虚拟网络基础设施设备生态。该漏洞与其说是一种实用的远程攻击，不如说是对 NAT 具备隔离能力这一假设的纠正。

rss · The Hacker News · 8月7日 10:58

**背景**: 网络地址转换（NAT）会在包头中改写 IP 地址和端口，并通过一张有状态的映射表来跟踪连接，常用于路由器和防火墙，使多个私有主机共享一个公网 IP。由于 NAT 位于可信与不可信网络边界，许多人认为它能隐藏内部主机从而增加安全性。NatJack 攻击的正是 NAT 的连接状态表本身，利用 NAT 设备跟踪 TCP 流和 DNS 查询的方式，劫持通信并伪造响应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/new-natjack-attacks-hijack-tcp-sessions.html">New NatJack Attacks Hijack TCP Sessions and Spoof DNS by...</a></li>
<li><a href="https://natjack.io/">NatJack : A New Attack Class Against Network Infrastructure Devices</a></li>
<li><a href="https://en.wikipedia.org/wiki/Network_address_translation">Network address translation - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#NAT`, `#TCP hijacking`, `#DNS spoofing`, `#Black Hat`

---

<a id="item-17"></a>
## [AI 辅助的 HTTP Terminator 发现新型 HTTP desync 技术与 Apache 零日漏洞](https://thehackernews.com/2026/08/ai-assisted-http-terminator-finds-novel.html) ⭐️ 8.0/10

PortSwigger 的 AI 辅助系统 HTTP Terminator 由 James Kettle 构建，在 3 万个候选向量中探索后，生成并验证了新的 HTTP desynchronization（desync）攻击技术。该系统还通过人类引导的发现流程，暴露了 Apache Traffic Server 中的一个独立零日漏洞。 这一进展意义重大，因为它展示了 AI 可用于开展新颖的安全研究，不仅发现已知攻击的变体，还能在广泛使用的反向代理中发现真实的零日漏洞。这些发现影响 Web 安全工程，也凸显了 AI 辅助漏洞研究的强大能力与当前局限。 PortSwigger 已将 HTTP Terminator 开源，并且测试是在通过漏洞赏金计划或 VDP 授权的真实网站上进行的。研究从 138 项技术标准出发，拆分为 15,000 个片段，但论文未披露每个自主发现具体由哪个模型或版本生成。

rss · The Hacker News · 8月7日 10:09

**背景**: HTTP desynchronization（简称 desync）攻击又称请求走私，攻击者使前端服务器和后端服务器对请求边界产生分歧，从而实施请求走私或缓存投毒。客户端 desync 攻击是其中的一种变体，会让受害者的浏览器与目标网站之间的连接失步。Apache Traffic Server 是一个模块化、高性能的反向代理，被主要 CDN 和内容所有者广泛使用。HTTP Terminator 将语言模型与专用测试工具相结合，来自动化发现此类攻击向量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://portswigger.net/research/http-terminator">Can AI do novel security research? Meet the HTTP Terminator</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apache_Traffic_Server">Apache Traffic Server</a></li>
<li><a href="https://portswigger.net/web-security/request-smuggling/browser/client-side-desync">Client-side desync attacks | Web Security Academy - PortSwigger</a></li>

</ul>
</details>

**标签**: `#HTTP desync`, `#AI security research`, `#zero-day`, `#Apache Traffic Server`, `#PortSwigger`

---

<a id="item-18"></a>
## [Claude Code 与 Gemini CLI 漏洞可让 GitHub 问题触及 CI 机密](https://thehackernews.com/2026/08/claude-code-and-gemini-cli-flaws-let.html) ⭐️ 8.0/10

安全研究机构 Novee Security 在 8 月 5 日的 Black Hat USA 大会上演示，来自无仓库权限账号的 GitHub 问题可在 Anthropic 和 Google 的编程代理仓库（Claude Code 与 Gemini CLI）中执行 CI 运行器代码，并能劫持 OpenAI 仓库中的下一次代理运行。该攻击针对各厂商默认提供的代理配置。 这揭示了一条从不可信输入到 CI/CD 工作流机密的切实攻击路径，影响了广泛使用的 AI 编程代理。它突显了默认代理配置存在安全隐患，可能危及开发者供应链并泄露敏感凭证。 该攻击利用间接提示注入：恶意指令被嵌入 GitHub 问题中，当编程代理检索并处理该问题时，会执行其中嵌入的命令，从而在 CI 运行器上实现代码执行。Novee Security 测试了各厂商提供的精确配置；在 OpenAI 的场景下，攻击者可以劫持下一次代理运行。

rss · The Hacker News · 8月7日 08:18

**背景**: AI 编程代理（如 Claude Code 和 Gemini CLI）是基于大语言模型的命令行工具，帮助开发者理解代码库、编辑文件并运行命令。CI/CD（持续集成/持续交付）流水线在运行器机器上执行自动化构建和测试，这些机器通常持有 API 密钥等机密。间接提示注入是一种攻击技术，将恶意指令嵌入到模型后续处理的内容（如网页或 GitHub 问题）中；如果模型无法区分可信指令与不可信内容，就可能执行攻击者的指令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://github.com/google-gemini/gemini-cli">GitHub - google-gemini/gemini-cli: An open-source AI agent that brings the power of Gemini directly into your terminal. · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Indirect_prompt_injection">Indirect prompt injection</a></li>

</ul>
</details>

**标签**: `#security`, `#CI/CD`, `#AI agents`, `#vulnerability`, `#GitHub`

---

<a id="item-19"></a>
## [Metabase SQL 注入零日漏洞遭利用，客户数据被盗](https://www.bleepingcomputer.com/news/security/framework-tally-disclose-metabase-data-theft-attacks/) ⭐️ 8.0/10

一个严重的 Metabase SQL 注入零日漏洞正在被积极利用，用于窃取客户数据，已影响 Framework 和 Tally 等公司。该漏洞允许攻击者在无需身份验证的情况下入侵 Metabase 实例。 此事意义重大，因为 Metabase 是广泛使用的开源商业智能工具，且已确认的数据盗窃受害者证明了其现实影响。运行暴露 Metabase 实例的组织需要立即修补或采取缓解措施。 该漏洞是一种未经身份验证的 SQL 注入，可导致数据被盗，Framework 和 Tally 已披露客户数据因此被窃取。更多技术细节预计将在安全公告中公布。

rss · BleepingComputer · 8月7日 20:14

**背景**: Metabase 是一个开源商业智能和数据可视化平台，允许用户查询数据库并创建仪表盘。SQL 注入是一类漏洞，攻击者可向查询中注入恶意 SQL 代码，从而可能读取或修改数据库内容。零日漏洞意味着供应商在漏洞被野外利用前没有时间修补。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/metabase/metabase">GitHub - metabase/metabase: The easy-to-use open source Business Intelligence and Embedded Analytics tool that lets everyone work with data :bar_chart: · GitHub</a></li>
<li><a href="https://www.metabase.com/">Open source AI analytics you can verify | Metabase</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#SQL injection`, `#zero-day`, `#Metabase`

---

<a id="item-20"></a>
## [TeamPCP 被指与 2020 年以来 Redis 攻击及后续供应链活动有关](https://thehackernews.com/2026/08/teampcp-linked-to-redis-attacks-dating.html) ⭐️ 7.0/10

Oligo 的新分析将威胁行为者 TeamPCP 与 2020 年以来的 Redis 攻击关联起来，显示该组织从入侵面向互联网的基础设施演变为实施软件供应链攻击。研究通过重叠域名、恶意软件部署路径和后端基础设施揭示了这些活动之间的联系。 该分析将 TeamPCP 的已知活动时间线延长了数年，表明该组织的犯罪历史比此前记录的更久。使用 Trivy、KICS 和 LiteLLM 等开源工具的组织可能受到影响，因为该组织的供应链攻击可能造成广泛的爆炸半径。 这一关联得到重叠域名、恶意软件部署路径、暂存技术以及 Redis 攻击与后续供应链活动共享的后端基础设施的支持。TeamPCP 已被关联到对 Trivy、KICS 和 LiteLLM 等开源项目的入侵，用于部署恶意软件。

rss · The Hacker News · 8月7日 06:50

**背景**: TeamPCP 是一个以针对广泛使用的开源软件进行协同供应链攻击而闻名的威胁行为者。Redis 是一种常暴露于互联网的内存数据存储，因此成为挖矿劫持和其他攻击的常见目标。该分析表明该组织的活动最早可追溯到 2020 年，早于使其受到关注的供应链攻击活动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/teampcp-linked-to-redis-attacks-dating.html">TeamPCP Linked To Redis Attacks Dating Back To 2020 And Later Supply Chain Campaign</a></li>
<li><a href="https://malpedia.caad.fkie.fraunhofer.de/actor/teampcp?trk=article-ssr-frontend-pulse_little-text-block">TeamPCP ( Threat Actor )</a></li>
<li><a href="https://www.bitsight.com/blog/threat-actor-profile-teampcp">Who is TeamPCP ? | TeamPCP Threat Actor Profile</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#threat actor`, `#supply chain`, `#Redis`, `#malware`

---