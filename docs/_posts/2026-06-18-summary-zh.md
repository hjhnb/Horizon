---
layout: default
title: "Horizon Summary: 2026-06-18 (ZH)"
date: 2026-06-18
lang: zh
---

> 从 72 条内容中筛选出 18 条重要资讯。

---

1. [美国科学政策危机引发研究人员外流](#item-1)
2. [乐购因博通滥用行为迁移 4 万虚拟机离开 VMware](#item-2)
3. [144 个 Mastra npm 包因账户劫持被入侵](#item-3)
4. [FortiBleed 泄漏暴露了 73,000 台 Fortinet VPN 设备凭证](#item-4)
5. [Lore：Epic Games 开源可扩展版本控制系统](#item-5)
6. [OpenAI 年亏损数十亿美元，营收 130 亿](#item-6)
7. [GLM-5.2 在 Artificial Analysis 上成为领先开源模型](#item-7)
8. [Adam 推出 CADAM：开源 AI CAD，文本生成机械设计](#item-8)
9. [RFC 10008 提出新的 HTTP QUERY 方法](#item-9)
10. [大众汽车通过 Play Integrity 屏蔽 GrapheneOS 用户](#item-10)
11. [Photobucket 索要 5 美元才能下载用户自己的照片](#item-11)
12. [AI 化学家改进药物制造反应](#item-12)
13. [微软确认 Defender 零日漏洞 RoguePlanet，补丁正在开发中](#item-13)
14. [恶意 JetBrains 插件窃取 AI API 密钥](#item-14)
15. [CISA 警告 Joomla JCE 插件漏洞正被利用](#item-15)
16. [黑客利用 Tailscale 和 OpenSSH 在 C2 离线后维持访问](#item-16)
17. [2026 年十大攻击面暴露点](#item-17)
18. [谷歌将于 2026 年起使用英欧用户 IP 地址进行广告个性化](#item-18)

---

<a id="item-1"></a>
## [美国科学政策危机引发研究人员外流](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 9.0/10

《科学美国人》一篇文章报道了美国科学与政治之间契约的破裂，导致严重的资金危机和研究人员离开学术界或国家的智力外流。 这场系统性危机威胁到美国作为全球研究与创新领导者的地位，影响科学进步和下一代科学家的培养。 文章指出，资助经费枯竭，签证限制阻碍外国人才，甚至高度专业化的研究人员（如光镊操作员）都在离开美国。

hackernews · presspot · 6月17日 09:54 · [社区讨论](https://news.ycombinator.com/item?id=48568058)

**背景**: 几十年来，美国科学依赖于一种契约：政府资助基础研究，以换取造福社会的发现。近年来的政治两极分化和预算削减侵蚀了这种信任，使研究人员对自己的职业生涯感到不确定。

**社区讨论**: 评论者分享了离开美国、资助被拒和招聘冻结的个人经历。尽管多数人表达了绝望，但也有人认为混乱为替代资助模式和新联系提供了机会。

**标签**: `#science policy`, `#research funding`, `#U.S. science`, `#academia`, `#brain drain`

---

<a id="item-2"></a>
## [乐购因博通滥用行为迁移 4 万虚拟机离开 VMware](https://arstechnica.com/information-technology/2026/06/tesco-moving-40000-server-workloads-off-vmware-amid-broadcoms-abusive-conduct/) ⭐️ 9.0/10

英国最大超市连锁乐购宣布，因博通自 2023 年收购 VMware 后的“滥用行为”，正在将 4 万个虚拟机工作负载从 VMware 迁移出来。 此举标志着企业对博通激进的许可证变更和成本上涨日益不满，可能加速整个行业向开源或替代虚拟化平台的迁移。 迁移预计耗时 18 个月，并涉及与 Veeam 和 Zerto 等备份软件的兼容性问题。乐购的新虚拟化平台尚未公布，但报道暗示可能是 Proxmox 或 Nutanix。

hackernews · Bender · 6月17日 21:00 · [社区讨论](https://news.ycombinator.com/item?id=48576838)

**背景**: VMware 是领先的虚拟化平台，企业用它在一台物理服务器上运行多个虚拟机。博通在 2023 年收购 VMware 后，取消了许多 SKU 选项、捆绑产品并大幅提高支持成本，促使许多客户探索替代方案。乐购的规模——4 万个虚拟机——使其成为已知的最大迁移之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hossted.com/knowledge-base/articles/vmware-support-costs-skyrocketing-after-broadcom-acquisition-open-source-alternatives-explained/">VMware Support Costs Skyrocketing After Broadcom Acquisition ?</a></li>
<li><a href="https://www.linkedin.com/posts/bedigitaluk_vmware-broadcomacquisition-itstrategy-activity-7318235483476529152-0qSA">How to navigate VMware changes after Broadcom acquisition</a></li>
<li><a href="https://easysam.co.uk/news/broadcom-and-atampt-reach-a-settlement-in-vmware-legal-dispute/">Broadcom and AT&T reach a settlement in VMware legal... - EasySAM</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，博通对 Proxmox 的营销非常有效，许多人认为这验证了迁移趋势。用户质疑 18 个月的时间线和备份兼容性问题，同时注意到这项工作规模巨大。有些人表示迁移路径现在已经成熟，但仍然是一项巨大的工程。

**标签**: `#virtualization`, `#VMware`, `#Broadcom`, `#enterprise migration`, `#cloud infrastructure`

---

<a id="item-3"></a>
## [144 个 Mastra npm 包因账户劫持被入侵](https://thehackernews.com/2026/06/144-mastra-npm-packages-compromised-via.html) ⭐️ 9.0/10

一场名为“easy-day-js”的软件供应链攻击通过劫持一个 npm 贡献者账户，侵入了@mastra/*命名空间下的 144 个 npm 包。多家安全公司（包括 Endor Labs、JFrog 和 Socket）发现了此次攻击。 此次攻击针对的是一个流行的开源 AI 框架，可能影响众多基于 Mastra 构建的 AI 应用。它凸显了 npm 生态系统中单账户被攻破的严重风险，以及加强对包维护者安全措施的必要性。 据内容片段，被劫持的账户名为“ehindero”。@mastra/*范围内的所有 144 个包均受影响，表明这是命名空间级别的入侵。攻击者可能注入了恶意代码以窃取凭证或泄露数据。

rss · The Hacker News · 6月17日 07:38

**背景**: Mastra 是一个开源 TypeScript 框架，用于构建 AI 应用，包括智能体以及与 React、Next.js 和 Node.js 的集成。npm（Node Package Manager）是一个广泛使用的 JavaScript 包注册表。当攻击者劫持维护者账户并发布合法包的恶意版本，从而感染下游用户时，就会发生 npm 供应链攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.npmjs.com/package/mastra">mastra - npm</a></li>
<li><a href="https://mastra.ai/">TypeScript AI Agent Framework & Platform | Mastra</a></li>

</ul>
</details>

**标签**: `#npm`, `#supply-chain-attack`, `#security`, `#Mastra`, `#AI-framework`

---

<a id="item-4"></a>
## [FortiBleed 泄漏暴露了 73,000 台 Fortinet VPN 设备凭证](https://www.bleepingcomputer.com/news/security/fortibleed-leak-exposes-fortinet-vpn-credentials-for-73-000-devices/) ⭐️ 9.0/10

名为 FortiBleed 的数据泄漏暴露了来自 194 个国家的 73,932 个 Fortinet 防火墙 URL 的凭证，可能危及这些 VPN 设备的安全。 此泄漏对使用 Fortinet VPN 的组织构成直接风险，攻击者可能获得未经授权的网络访问，导致数据泄露或勒索软件攻击。这凸显了 VPN 基础设施中持续存在的漏洞。 泄漏的凭证似乎是从先前的信息窃取器数据库转储中汇编而成，专门针对 Fortinet 设备。全球超过 73,000 台设备受到影响，数据正在黑客论坛上传播。

rss · BleepingComputer · 6月17日 15:12

**背景**: FortiGate VPN 被企业广泛用于安全远程访问。FortiBleed 泄漏不是利用新漏洞，而是汇总了先前被盗的凭证，强调了凭证卫生和多因素认证的重要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/fortibleed-leak-exposes-fortinet-vpn-credentials-for-73-000-devices/">FortiBleed leak exposes Fortinet VPN credentials for 73,000 devices.</a></li>
<li><a href="https://cybersecuritynews.com/fortibleed-fortinet-firewalls-compromised/">FortiBleed - 70,000+ Fortinet Firewalls Compromised in Massive ...</a></li>

</ul>
</details>

**标签**: `#security`, `#VPN`, `#vulnerability`, `#data leak`, `#Fortinet`

---

<a id="item-5"></a>
## [Lore：Epic Games 开源可扩展版本控制系统](https://lore.org/) ⭐️ 8.0/10

Epic Games 已开源 Lore，这是一个专为数据和团队前所未有的可扩展性而设计的版本控制系统，旨在成为游戏开发领域 Perforce 的竞争对手。 Lore 提供了 Perforce 的免费开源替代方案，满足了游戏开发中处理大型二进制文件和独占文件锁定的关键需求，而 Git 在这些方面表现不佳。 Lore 并非全新产品，它以前被称为 Unreal Revision Control，并已在 UEFN（Fortnite 的虚幻编辑器）内部使用。它由一个存储子系统和一个版本控制子系统组成。

hackernews · regnerba · 6月17日 14:30 · [社区讨论](https://news.ycombinator.com/item?id=48571081)

**背景**: 像 Git 这样的版本控制系统擅长管理源代码，但在处理大型二进制文件（如纹理、3D 模型）方面存在困难，并且缺乏强大的文件锁定功能。Perforce 是一种专有系统，由于这些原因被广泛用于游戏开发，但在管理复杂性和成本方面存在问题。Lore 旨在结合 Perforce 的可扩展性和 Git 的开放性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/EpicGames/lore">GitHub - EpicGames/lore: Lore is a next-generation, open source revision control system · GitHub</a></li>
<li><a href="https://epicgames.github.io/lore/explanation/system-design/">The Lore Version Control System - Lore Developer Documentation</a></li>
<li><a href="https://www.phoronix.com/news/Epic-Games-Lore-VCS">Epic Games Announces Lore Open-Source Version Control System - Phoronix</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Perforce 的开源替代方案表示兴奋，指出它解决了游戏开发中的实际痛点。一些人强调 Lore 已在 Epic 内部使用，而另一些人则讨论 Git 用户界面不友好以及对文件锁定和大文件支持的需求。

**标签**: `#version control`, `#game development`, `#open source`, `#scalability`, `#perforce`

---

<a id="item-6"></a>
## [OpenAI 年亏损数十亿美元，营收 130 亿](https://arstechnica.com/ai/2026/06/leaked-financial-docs-show-openai-is-losing-billions-of-dollars-a-year/) ⭐️ 8.0/10

泄露的财务文件显示，OpenAI 在 2025 年亏损了数十亿美元，尽管营收达到 130 亿美元，巨大的研发成本是亏损的主要原因。 这一披露凸显了领先 AI 公司面临的财务可持续性挑战，可能影响投资者信心和 AI 行业的商业模式。 文件显示营收 130 亿美元，收入成本 75 亿美元，研发支出是亏损的主要部分。OpenAI 报告有 9 亿周活跃用户，但只有 5000 万付费用户。

hackernews · greenchair · 6月17日 21:31 · [社区讨论](https://news.ycombinator.com/item?id=48577208)

**背景**: OpenAI 是一家以开发 ChatGPT 和其他大型语言模型而闻名的 AI 研究公司。其巨大的研发成本源于训练和运行尖端 AI 模型。尽管收入快速增长，但由于高昂的运营费用，公司尚未实现盈利。

**社区讨论**: 评论者质疑泄露文件缺乏细节，并争论是否应将重点从研发转向降低推理成本。一些人指出，考虑到 DeepSeek 等免费替代品的可用性，将免费用户转化为付费订阅者将面临挑战。

**标签**: `#OpenAI`, `#finance`, `#AI industry`, `#business`, `#economics`

---

<a id="item-7"></a>
## [GLM-5.2 在 Artificial Analysis 上成为领先开源模型](https://artificialanalysis.ai/articles/glm-5-2-is-the-new-leading-open-weights-model-on-the-artificial-analysis-intelligence-index) ⭐️ 8.0/10

由 Z.ai（原智谱 AI）开发的 GLM-5.2 在 Artificial Analysis Intelligence Index 中被评为领先的开源权重模型，以远低于 GPT-5.5 和 Opus 4.7 等专有模型的成本提供接近前沿的性能。 这一突破挑战了专有前沿 AI 模型的主导地位，提高了全球开发者和企业的可及性。开源许可证（MIT）和具有竞争力的定价可能加速 AI 的采用和创新，尤其是在对成本敏感的应用中。 GLM-5.2 Max 版本拥有 7530 亿参数，支持 100 万 token 的上下文窗口，在自主编程和复杂推理方面表现出色。但社区反馈指出，其推理 token 消耗可能很高，一位用户报告称，完成一个简单的编程任务用了 45,000 token 和 15 分钟。

hackernews · himata4113 · 6月17日 09:12 · [社区讨论](https://news.ycombinator.com/item?id=48567759)

**背景**: GLM（通用语言模型）是由 Z.ai（原智谱 AI）开发的一系列大语言模型，该公司自 2025 年 7 月起以 MIT 许可证发布 GLM 模型，使其可自由使用。Artificial Analysis 是一个独立的基准测试平台，从质量、价格、速度和延迟等方面评估 AI 模型，经常被 AI 社区引用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM-5.2">GLM-5.2</a></li>
<li><a href="https://github.com/Z-ai-glm/GLM-5.2">GLM-5.2 Lightweight Installer - GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极，用户称赞 GLM-5.2 以极低的成本实现了接近前沿的性能。但也有人对其推理效率表示担忧，指出某些任务 token 消耗高且处理时间长，呼吁在这方面进行改进。

**标签**: `#GLM-5.2`, `#open weights`, `#AI competition`, `#reasoning efficiency`, `#pricing`

---

<a id="item-8"></a>
## [Adam 推出 CADAM：开源 AI CAD，文本生成机械设计](https://github.com/Adam-CAD/CADAM) ⭐️ 8.0/10

Y Combinator W25 公司 Adam 发布了开源 AI 平台 CADAM，该平台能从自然语言文本提示和图像引用生成参数化 3D CAD 模型，输出 OpenSCAD 代码并带有交互式滑块用于尺寸调整。 该发布将自然语言的易用性与基于代码的 CAD 精度相结合，可能降低机械设计的门槛。作为 YC 孵化的开源项目，它有望加速 AI 辅助工程设计的创新。 该平台通过将 OpenSCAD 编译为 WebAssembly 实现完全在浏览器中运行，使用 React Three Fiber 进行渲染，并通过 Vercel AI SDK 支持多种 LLM，评估中意外发现 Gemini 2.5 Pro 表现最佳。它还包括一个网格模式，用于生成带纹理的 3D 网格。

hackernews · zachdive · 6月17日 16:14 · [社区讨论](https://news.ycombinator.com/item?id=48572553)

**背景**: CAD 中的参数化建模使用尺寸和约束等参数来创建可轻松编辑的模型。OpenSCAD 是一种纯脚本 CAD 工具，模型通过代码定义。AI 编码代理在软件领域取得了成功，但在机械设计的空间推理方面仍面临挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Supabase">Supabase</a></li>

</ul>
</details>

**社区讨论**: 一些用户报告了积极的早期体验，有人说它快速创建了一个衬套密封件。但也存在质疑：一位评论者对实际工程工作的用例提出疑问，提到时间和准确性问题。其他人指出 LLM 在空间推理方面仍然薄弱。

**标签**: `#AI`, `#CAD`, `#open-source`, `#YC`, `#mechanical design`

---

<a id="item-9"></a>
## [RFC 10008 提出新的 HTTP QUERY 方法](https://www.rfc-editor.org/info/rfc10008/) ⭐️ 8.0/10

RFC 10008 标准化了一个名为 QUERY 的新 HTTP 方法，允许携带请求体的安全且幂等的请求，于 2026 年 6 月 15 日发布。 这填补了 HTTP 中长期存在的空白，因为 GET 不能有请求体，而 POST 既不安全也不幂等，从而为复杂查询（如 GraphQL 或大型过滤负载）实现更好的 API 设计和缓存。 QUERY 方法是安全且幂等的，意味着它不会改变服务器状态，多次相同的请求产生相同结果，并且请求体包含在缓存键计算中。

hackernews · schappim · 6月17日 10:51 · [社区讨论](https://news.ycombinator.com/item?id=48568502)

**背景**: 像 GET 这样的 HTTP 方法安全且幂等，但不支持请求体，而 POST 支持请求体但既不安全也不幂等。RFC 10008 引入了 QUERY，将 GET 的安全性与 POST 的请求体能力结合起来，解决了使用带请求体的 GET 或依赖 POST 进行读取操作的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rfc-editor.org/info/rfc10008/">RFC 10008: The HTTP QUERY Method | RFC Editor</a></li>
<li><a href="https://blainsmith.com/articles/rfc-10008-http-query-method/">RFC 10008: The HTTP QUERY Method - Blain Smith</a></li>
<li><a href="https://byteiota.com/rfc-10008-http-query-method-ends-the-post-workaround/">RFC 10008: HTTP QUERY Method Ends the POST Workaround</a></li>

</ul>
</details>

**社区讨论**: 评论者指出了棘手的缓存影响，有人认为将请求体包含在缓存键中很奇怪，并建议仅将逐位比较作为通用策略。另一位评论者希望 HTML 表单能够支持 QUERY，以避免 POST 中出现的重新提交警告。

**标签**: `#HTTP`, `#RFC`, `#web standards`, `#HTTP methods`, `#caching`

---

<a id="item-10"></a>
## [大众汽车通过 Play Integrity 屏蔽 GrapheneOS 用户](https://discuss.grapheneos.org/d/35949-volkswagen-app?page=3) ⭐️ 8.0/10

大众汽车更新了官方应用，要求通过 Google Play Integrity 认证，这实际上阻止了运行 GrapheneOS 等自定义 Android 操作系统的用户使用该应用的完整功能。 此举影响了注重隐私的消费者，他们选择强化版操作系统，并标志着一种趋势：Play Integrity 的强制实施限制了开源 Android 变体以及像 Home Assistant 这样的第三方集成。 大众汽车应用现在将其 API 锁定为仅限通过 Play Protect 认证的设备，这意味着提供替代界面（例如预热汽车）的社区驱动项目已失效。官方应用据称包含 60%的广告，且缺乏之前可通过第三方集成使用的功能。

hackernews · microtonal · 6月17日 15:04 · [社区讨论](https://news.ycombinator.com/item?id=48571526)

**背景**: GrapheneOS 是一个基于 Android 的安全型开源移动操作系统，提供增强的隐私保护和沙箱机制。它默认不包含 Google Play 服务，因此 Play Integrity API——用于验证设备和应用完整性——通常会将这些设备标记为未认证。越来越多的应用使用 Play Integrity 来执行 DRM 和安全策略，但这可能无意中锁定了注重隐私的自定义 ROM 用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Play_Integrity_API">Play Integrity API</a></li>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://developer.android.com/google/play/integrity">Play Integrity API | Android Developers</a></li>

</ul>
</details>

**社区讨论**: 社区成员表达了不满，指出大众的 API 限制破坏了有用的 Home Assistant 集成，而官方应用体验较差。一些人批评欧盟强制安装远程信息处理设备的趋势，另一些人猜测如果英国禁止 VPN，使用 GrapheneOS 可能成为目标。

**标签**: `#privacy`, `#grapheneos`, `#android`, `#volkswagen`, `#api-restrictions`

---

<a id="item-11"></a>
## [Photobucket 索要 5 美元才能下载用户自己的照片](https://www.lutr.dev/want-your-images-back-sure-that-ll-be-5-dollars) ⭐️ 8.0/10

一篇博文批评 Photobucket 向用户收取 5 美元才能下载他们自己的图片，揭露了用户需要支付订阅费才能取回个人数据的做法。 这种做法引发了关于数据所有权和企业道德的担忧，用户多年前上传的图片可能因不付费而无法取回。同时也引发了关于数据可移植性和云服务责任的讨论。 博文作者收到账户将被删除的邮件，并被迫订阅才能下载图片，但发现可以在关闭账户前先下载数据的变通方法。该博文还提到由于讨论热度高，博客本身遭遇了高流量。

hackernews · lutr · 6月17日 13:05 · [社区讨论](https://news.ycombinator.com/item?id=48569954)

**背景**: Photobucket 是 2000 年代流行的图片托管服务，但未能成功盈利，先后被 Fox 和一家初创公司收购。许多用户曾将个人照片存储在该平台，如今面临付费墙才能取回图片，凸显了依赖免费云服务的风险。

**社区讨论**: 评论观点不一：一些用户发现通过关闭账户可以免费下载数据，而另一些则批评这种付费墙是公司贪婪的表现。部分评论者将 Photobucket 的做法与 Google Photos 的免费数据导出服务进行对比，指出在质量和便捷性方面的权衡。

**标签**: `#photobucket`, `#data portability`, `#user rights`, `#tech ethics`, `#paywall`

---

<a id="item-12"></a>
## [AI 化学家改进药物制造反应](https://openai.com/index/ai-chemist-improves-reaction) ⭐️ 8.0/10

OpenAI 与 Molecule.one 展示了一种由 GPT-5.4 驱动的近乎自主的 AI 化学家，成功改进了药物化学中一项具有挑战性的反应。 这代表了 AI 辅助药物发现的潜在飞跃，它将大语言模型与自主实验相结合，加速了复杂化学反应的优化过程。 尽管前景广阔，但公告中提及的 GPT-5.4 是一个推测性的版本号，且缺乏详细的实验数据，因此其全部能力和局限性尚不清楚。

rss · OpenAI Blog · 6月17日 10:00

**背景**: 近乎自主的 AI 化学家将机器人平台与语言模型相结合，以最少的人工干预来规划和执行实验。Molecule.one 的 Maria AI 平台已经将前沿 AI 与微升级别高通量实验相结合用于化学发现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://molecule.one/">molecule.one - Chemistry AI for Autonomous Discovery</a></li>
<li><a href="https://www.science.org/doi/10.1126/sciadv.adj0461">AI-driven robotic chemist for autonomous synthesis of organic molecules | Science Advances</a></li>
<li><a href="https://pubs.acs.org/doi/10.1021/jacs.4c17738">A Multiagent-Driven Robotic AI Chemist Enabling Autonomous Chemical Research On Demand | Journal of the American Chemical Society</a></li>

</ul>
</details>

**标签**: `#AI`, `#chemistry`, `#medicinal chemistry`, `#GPT-5.4`, `#drug discovery`

---

<a id="item-13"></a>
## [微软确认 Defender 零日漏洞 RoguePlanet，补丁正在开发中](https://thehackernews.com/2026/06/microsoft-confirms-rogueplanet-defender_02022423645.html) ⭐️ 8.0/10

微软正式披露了 Microsoft Defender 中的一个权限提升零日漏洞，代号 RoguePlanet，被分配为 CVE-2026-50656，CVSS 评分为 7.8，并确认补丁正在开发中。 该漏洞影响广泛部署在 Windows 系统中的 Microsoft Defender，使其成为数百万用户和组织面临的关键安全问题。权限提升漏洞可能允许攻击者获得更高的系统访问权限，可能导致系统完全被攻陷。 该漏洞位于 Microsoft 恶意软件保护引擎中，虽然 CVSS 评分为 7.8 表示严重性较高，但目前已知未被利用。微软正在开发补丁，但未提供发布日期。

rss · The Hacker News · 6月17日 17:36

**背景**: Microsoft Defender 是 Windows 内置的防病毒和端点保护解决方案，利用 Microsoft 恶意软件保护引擎来检测和阻止威胁。权限提升漏洞允许攻击者以比预期更高的权限运行代码，可能绕过安全边界。这是近期影响该引擎的多个 CVE 之一，突显了维护安全软件的复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.microsoft.com/en-us/topic/microsoft-malware-protection-engine-deployment-information-d5b6158a-6cfd-c2ee-6591-be3693f42f09">Microsoft Malware Protection Engine deployment information</a></li>
<li><a href="https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-antivirus-updates">Microsoft Defender Antivirus security intelligence and ...</a></li>

</ul>
</details>

**标签**: `#security`, `#zero-day`, `#Microsoft Defender`, `#privilege escalation`, `#CVE`

---

<a id="item-14"></a>
## [恶意 JetBrains 插件窃取 AI API 密钥](https://thehackernews.com/2026/06/malicious-jetbrains-plugins-steal-ai.html) ⭐️ 8.0/10

研究人员在 JetBrains Marketplace 上发现 15 个恶意插件，它们伪装成 AI 编程助手，窃取 AI 提供商的 API 密钥。 这个协调的恶意软件活动直接威胁到在 IDE 中使用 AI 的开发者，可能导致数据泄露和 API 密钥被盗带来的经济损失。 这些插件冒充基于 DeepSeek 和其他大型语言模型构建的工具，提供聊天和代码审查等功能，同时秘密窃取密钥。

rss · The Hacker News · 6月17日 13:51

**背景**: JetBrains Marketplace 为 IntelliJ IDEA 等 JetBrains IDE 提供插件。DeepSeek 是一家以高性价比模型闻名的中国 AI 公司。API 密钥是用于访问 AI 服务的凭证，用于身份验证和计费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infosecurity-magazine.com/news/fifteen-jetbrains-marketplace/">Fifteen JetBrains Marketplace Plugins Steal API Keys</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://plugins.jetbrains.com/">IntelliJ IDEA Plugins and Themes | JetBrains Marketplace</a></li>

</ul>
</details>

**标签**: `#security`, `#JetBrains`, `#supply chain attack`, `#AI`, `#malware`

---

<a id="item-15"></a>
## [CISA 警告 Joomla JCE 插件漏洞正被利用](https://thehackernews.com/2026/06/cisa-warns-of-actively-exploited-joomla.html) ⭐️ 8.0/10

美国 CISA 将 Widget Factory Joomla Content Editor (JCE)插件中的一个严重漏洞（CVE-2026-48907，CVSS 评分 10.0）添加到已知被利用漏洞目录，确认正在被积极利用。该漏洞因不恰当的访问控制，允许远程攻击者执行任意 PHP 代码。 该漏洞严重性最高（CVSS 10.0）且已被积极利用，使用 JCE 的网站面临立即被完全入侵的风险。联邦机构被要求修补，所有 Joomla 网站管理员应紧急更新插件，以防止数据泄露和服务器被接管。 该漏洞是 JCE 插件中的一个不恰当访问控制问题，可导致任意 PHP 代码执行。CISA 的 KEV 目录要求美国联邦机构在规定时间内修补，但强烈建议所有用户立即更新。

rss · The Hacker News · 6月17日 05:50

**背景**: Joomla Content Editor (JCE)是 Joomla CMS 的一个流行的所见即所得编辑器扩展，提供增强的内容编辑功能。CISA 的已知被利用漏洞目录是一份确认已在野外被利用的漏洞列表，组织可用于优先修补。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://extensions.joomla.org/extension/jce/">JCE, by Widget Factory Limited - Joomla Extension Directory Home [www.joomlacontenteditor.net] JCE Editor GitHub - widgetfactory/jce: JCE - A Content Editor for Joomla JoomlaForever.com! - Mastering Joomla Content Editor (JCE ... Best Joomla Content Editors ( Free and Paid ) in 2024</a></li>
<li><a href="https://www.cisa.gov/known-exploited-vulnerabilities-catalog">Known Exploited Vulnerabilities Catalog | CISA</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Joomla`, `#CISA`, `#CVE`

---

<a id="item-16"></a>
## [黑客利用 Tailscale 和 OpenSSH 在 C2 离线后维持访问](https://thehackernews.com/2026/06/junior-hacker-used-tailscale-and.html) ⭐️ 7.0/10

一名初级黑客入侵了一家法国小型汽车企业，植入了键盘记录器，并在其使用的 Havoc 命令与控制服务器离线前，在受害者机器上安装了 OpenSSH 和 Tailscale，从而在不依赖 C2 的情况下保持持久访问。 这次攻击展示了一种新颖的持久化技术，绕过了对命令与控制服务器的传统依赖，突显了一种不断演变的规避方法，安全从业者必须在应急响应和防御中加以考虑。 攻击者使用 Havoc 后渗透框架进行初始访问和 C2，随后利用 Tailscale 的网状 VPN 和 OpenSSH 创建一个后门，在 Havoc 服务器次日离线后仍能正常工作。受害者是一家法国小型汽车企业，被盗数据包括银行和电子邮件凭证。

rss · The Hacker News · 6月17日 16:00

**背景**: Tailscale 是一个开源软件定义的网状 VPN，通过创建零配置覆盖网络来简化安全联网。OpenSSH 是广泛用于安全远程 Shell 访问和文件传输的工具。像 Havoc 这样的命令与控制（C2）框架被攻击者用来管理被入侵的系统，但仅依赖 C2 服务器会造成单点故障；像本文这样的替代持久化方法降低了检测风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tailscale">Tailscale - Wikipedia</a></li>
<li><a href="https://havocframework.com/">Havoc</a></li>
<li><a href="https://www.zscaler.com/blogs/security-research/havoc-across-cyberspace">Havoc Across the Cyberspace | Blog | Zscaler</a></li>

</ul>
</details>

**标签**: `#security`, `#persistence`, `#tailscale`, `#openssh`, `#incident-response`

---

<a id="item-17"></a>
## [2026 年十大攻击面暴露点](https://thehackernews.com/2026/06/the-top-10-attack-surface-exposures-in.html) ⭐️ 7.0/10

《黑客新闻》的一篇文章列出了预计在 2026 年出现的十大攻击面暴露点，包括暴露的管理面板和凭据重用，并重点介绍了 MongoBleed 漏洞（CVE-2025-14847），该漏洞允许未认证的攻击者从 MongoDB 服务器内存中泄露敏感数据。 随着利用时间的缩短，这些暴露点成为攻击者的关键切入点；组织必须主动管理攻击面以防止数据泄露。MongoBleed 漏洞表明，即使单个未修补的服务也可能导致大规模数据泄露。 文章未详细列出全部 10 个暴露点，但强调像 MongoBleed（CVE-2025-14847）这样的漏洞可以远程利用且复杂度低，影响多个 MongoDB 版本，允许从未初始化的堆内存中提取凭据和会话令牌。

rss · The Hacker News · 6月17日 10:30

**背景**: 攻击面是指未经授权用户可能尝试进入或提取数据的所有点的总和。暴露的管理面板和重复使用的凭据是常见的弱点。MongoBleed 是 MongoDB 中的一个严重信息泄露漏洞，因类似 Heartbleed 而得名，影响自托管实例，于 2025 年底披露并已被积极利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wiz.io/blog/mongobleed-cve-2025-14847-exploited-in-the-wild-mongodb">MongoBleed: Critical MongoDB Vulnerability CVE-2025-14847 ...</a></li>
<li><a href="https://cybersecuritynews.com/mongobleed-vulnerability/">MongoBleed (CVE-2025-14847) Now Exploited in the Wild ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#attack surface`, `#vulnerability`, `#security`

---

<a id="item-18"></a>
## [谷歌将于 2026 年起使用英欧用户 IP 地址进行广告个性化](https://www.bleepingcomputer.com/news/security/google-to-use-uk-and-eu-user-ip-addresses-for-ad-personalization/) ⭐️ 7.0/10

自 2026 年 8 月 3 日起，谷歌将使用英国、欧洲经济区和瑞士用户的 IP 地址进行广告测量和个性化。这标志着谷歌此前称此类做法“错误”的立场发生逆转。 这一政策变化对数百万英国和欧盟用户的隐私产生重大影响，因为 IP 地址可能暴露位置和浏览习惯。它也反映了监管压力的转变以及 GDPR 下同意规则的演变。 此变化正值英国信息专员办公室（ICO）考虑新的同意规则之际。谷歌此前曾批评使用 IP 地址进行设备识别，但现在计划将其用于广告个性化。

rss · BleepingComputer · 6月17日 21:02

**背景**: 英国信息专员办公室（ICO）是负责执行 GDPR 及其他隐私法的独立数据保护监管机构。谷歌的新政策与关于广告数据使用和同意的持续监管讨论相一致。根据 GDPR，IP 地址被视为个人数据，因为它们可以识别用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Information_Commissioner's_Office">Information Commissioner's Office - Wikipedia</a></li>
<li><a href="https://ico.org.uk/">Information Commissioner's Office (ICO)</a></li>

</ul>
</details>

**标签**: `#privacy`, `#google`, `#ad personalization`, `#regulation`, `#GDPR`

---