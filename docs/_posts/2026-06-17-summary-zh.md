---
layout: default
title: "Horizon Summary: 2026-06-17 (ZH)"
date: 2026-06-17
lang: zh
---

> 从 96 条内容中筛选出 20 条重要资讯。

---

1. [NVIDIA Blackwell 在 MLPerf Training 6.0 中表现卓越](#item-1)
2. [CISA 警告 Rockwell FLEX I/O 适配器存在严重漏洞](#item-2)
3. [机械手表内部机制的互动深度解析](#item-3)
4. [停止在浏览器会话中使用 JWT](#item-4)
5. [苹果域名变更可能使‘隐藏邮件地址’更易被屏蔽](#item-5)
6. [Meta 将核心工程师调往 AI 数据标注](#item-6)
7. [Qwen-Robot Suite：面向具身智能的基础模型套件](#item-7)
8. [SubQ 1.1 Small：线性扩展的稀疏注意力机制](#item-8)
9. [AI 模型出口管制削弱美国网络防御](#item-9)
10. [警方滥用 Flock 摄像头进行跟踪](#item-10)
11. [罗克韦尔控制器存在 CIP 拒绝服务漏洞](#item-11)
12. [CISA 警告 Rockwell RSLinx Classic 存在高危拒绝服务漏洞](#item-12)
13. [CISA 警告 Rockwell PavilionX 存在授权缺失漏洞](#item-13)
14. [Vertex AI SDK 漏洞致模型上传可被桶蹲点劫持](#item-14)
15. [Rokarolla 安卓恶意软件攻击 217 个银行和加密应用](#item-15)
16. [攻击者利用三个 Fortinet FortiSandbox 漏洞](#item-16)
17. [SprySOCKS 后门新增 Windows 变体，采用驱动级隐身](#item-17)
18. [CISA 将遭利用的 LiteSpeed cPanel 插件漏洞列入 KEV](#item-18)
19. [恶意 JetBrains 插件盗窃 AI API 密钥](#item-19)
20. [Anthropic 的 Claude Code 数据：领域知识胜过编码技能](#item-20)

---

<a id="item-1"></a>
## [NVIDIA Blackwell 在 MLPerf Training 6.0 中表现卓越](https://developer.nvidia.com/blog/nvidia-blackwell-tops-mlperf-training-6-0-with-industry-leading-scale-and-performance/) ⭐️ 9.0/10

NVIDIA 的 Blackwell GPU 平台在 MLPerf Training v6.0 所有基准测试中均获得最高分，在训练吞吐量和可扩展性方面超越了之前的架构和竞争对手。 这一结果巩固了 NVIDIA 在 AI 训练硬件领域的主导地位，验证了 Blackwell 架构在大规模 AI 工作负载中的效率，将影响数据中心采购决策和 AI 研究能力。 基准测试包括 GPT-3 和 BERT-Large 等模型；Blackwell 系统在某些任务上的性能比上一代 Hopper 提升了高达 2 倍。

rss · NVIDIA Developer Blog · 6月16日 15:11

**背景**: MLPerf 是 MLCommons 制定的行业标准基准测试套件，用于衡量 AI 训练和推理性能。NVIDIA 的 Blackwell 架构于 2024 年推出，拥有 2080 亿个晶体管，采用定制的 TSMC 4NP 工艺制造，在计算密度和能效上实现了显著提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://mlcommons.org/benchmarks/training/">MLCommons MLPerf Training Benchmark</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/">The Engine Behind AI Factories | NVIDIA Blackwell Architecture</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#Blackwell`, `#MLPerf`, `#AI training`, `#benchmarks`

---

<a id="item-2"></a>
## [CISA 警告 Rockwell FLEX I/O 适配器存在严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-167-05) ⭐️ 9.0/10

CISA 披露了 Rockwell Automation FLEX I/O EtherNet/IP 适配器（1794-AENTR 和 1794-AENTRXT 版本 2.012）中的两个严重漏洞（CVE-2026-0646 和 CVE-2026-0647），可能导致拒绝服务和未授权访问。厂商建议更新至 2.013 版本。 这些漏洞影响关键制造业中广泛部署的工业自动化设备，对全球运营技术（OT）安全构成风险。成功利用可能中断生产线，并需要手动干预才能恢复。 CVE-2026-0646 是一种内存释放不当漏洞（CWE-401），CVSS v3.1 基础评分为 7.5，导致适配器故障并失去 I/O 连接。CVE-2026-0647 涉及关键功能缺少认证，综合 CVSS v3 评分为 9.4。

rss · CISA Cybersecurity Advisories · 6月16日 12:00

**背景**: Rockwell Automation 的 FLEX I/O EtherNet/IP 适配器作为 I/O 模块与 EtherNet/IP 网络之间的桥梁，使用通用工业协议（CIP）进行实时数据交换。披露的公告遵循 CISA 的通用安全咨询框架（CSAF）格式，该格式标准化了漏洞信息共享。正确的内存管理和认证对于工业控制系统避免停机至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://literature.rockwellautomation.com/idc/groups/literature/documents/um/1794-um066_-en-e.pdf">User Manual Original Instructions FLEX I/O Dual-port EtherNet/IP Adapters</a></li>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#ICS`, `#vulnerability`, `#Rockwell Automation`, `#CISA`

---

<a id="item-3"></a>
## [机械手表内部机制的互动深度解析](https://ciechanow.ski/mechanical-watch/) ⭐️ 8.0/10

ciechanow.ski 发布了一篇互动文章，通过逐步动画和清晰文字解释机械手表的内部工作原理，所有代码均使用原生 HTML、CSS 和 JS 实现。 这篇文章为在线教育树立了高标准，让机械手表原理变得人人可懂，而其轻量级实现证明，复杂的交互并非总需要现代框架。 文章使用纯 HTML、CSS 和 JavaScript，无任何外部库，在 iPhone 7 上也能正常工作，展现了极佳的向后兼容性。

hackernews · razin · 6月16日 11:26 · [社区讨论](https://news.ycombinator.com/item?id=48553550)

**背景**: 机械手表由主发条提供动力，主发条缓慢释放能量驱动齿轮系。擒纵机构逐步释放齿轮系，而摆轮和游丝以精确频率振荡，从而调节计时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Escapement">Escapement - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Balance_spring">Balance spring - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mechanical_watch">Mechanical watch - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者们一致称赞文章的教育清晰度和作者使用原生代码的技巧。一位用户受到启发制作了真实的手表机芯分解视图，另一位教师称赞其循序渐进的讲解方式罕见而有价值。

**标签**: `#interactive-article`, `#mechanical-watch`, `#education`, `#engineering`, `#physics`

---

<a id="item-4"></a>
## [停止在浏览器会话中使用 JWT](https://gist.github.com/samsch/0d1f3d3b4745d778f78b230cf6061452) ⭐️ 8.0/10

一篇批判性分析文章反对在基于浏览器的用户会话中使用 JSON Web Token，引发了关于其安全性及与传统会话令牌相比是否合适的社区辩论。 这场辩论促使开发者重新审视常见的认证实践，可能减少因验证不足和令牌撤销问题导致账户被盗的漏洞。 该 gist 引用了其他帖子，声称 JWT 从根本上不安全，而社区成员指出 JWT 在服务间通信等场景中，通过设置短有效期仍有合理用途。

hackernews · dzonga · 6月16日 16:49 · [社区讨论](https://news.ycombinator.com/item?id=48558147)

**背景**: JSON Web Token 是一种紧凑的、URL 安全的令牌格式，用于身份验证和信息交换。它由头部、载荷和签名组成，可使用共享密钥或公私钥对进行签名。然而，在浏览器会话中使用时，常见陷阱包括令牌有效期过长、缺乏撤销机制以及签名验证过程中的漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://portswigger.net/web-security/jwt">JWT attacks | Web Security Academy</a></li>
<li><a href="https://www.vaadata.com/en/blog/jwt-json-web-token-vulnerabilities-common-attacks-and-security-best-practices/">JWT: Vulnerabilities, Attacks & Security Best Practices</a></li>
<li><a href="https://stytch.com/blog/jwts-vs-sessions-which-is-right-for-you/">JWTs vs . sessions : which authentication approach is right for you?</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同意 JWT 不适用于浏览器会话，但为其在服务间通信中的使用辩护。有人认为由于 JWT 会过期，撤销列表的大小比完整会话存储小，因此是可行的。另有人指出，将 JWT 有效期限制在 5-15 分钟并配合刷新模型可以降低风险。

**标签**: `#authentication`, `#JWT`, `#security`, `#web development`, `#sessions`

---

<a id="item-5"></a>
## [苹果域名变更可能使‘隐藏邮件地址’更易被屏蔽](https://arseniyshestakov.com/2026/06/16/apple-is-about-to-make-hide-my-email-useless/) ⭐️ 8.0/10

苹果将在今年夏天晚些时候将‘通过 Apple 登录’和‘隐藏邮件地址’的电子邮件域名统一为@private.icloud.com。这一变化使得网站可以轻松屏蔽来自该域名的所有别名，从而削弱了隐私保护效果。 ‘隐藏邮件地址’是 iCloud+ 用户的重要隐私功能，可让用户的个人邮箱保持私密。如果网站开始屏蔽所有 @private.icloud.com 地址，用户可能无法在许多网站上使用该服务。 此前，‘隐藏邮件地址’的别名使用 @icloud.com 域名，而‘通过 Apple 登录’使用 @private.icloud.com。统一域名后，一个域就可以被列入黑名单，而之前屏蔽 @icloud.com 会影响到普通的 iCloud 邮件用户。

hackernews · SXX · 6月16日 18:37 · [社区讨论](https://news.ycombinator.com/item?id=48559935)

**背景**: ‘隐藏邮件地址’允许 iCloud+ 订阅者生成随机电子邮件地址，并将其转发到真实收件箱，从而避免暴露个人邮箱。网站可以屏蔽他们认为有风险的电子邮件域名，例如已知的临时邮箱或别名服务。苹果将所有别名整合到一个域名下，无意中让网站更容易实施全面屏蔽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/news/?id=sus6t6ab">New domain for Sign in with Apple and iCloud+ Hide My Email</a></li>
<li><a href="https://support.apple.com/en-us/105078">How to use Hide My Email with Sign in with Apple</a></li>

</ul>
</details>

**社区讨论**: 评论显示反应不一：有些用户认为这一变化会使‘隐藏邮件地址’效果降低，而另一些人则认为屏蔽此类邮件的网站本身就不可信。一位用户建议使用自定义域名加通配别名作为替代方案。

**标签**: `#apple`, `#privacy`, `#email`, `#icloud`, `#hide-my-email`

---

<a id="item-6"></a>
## [Meta 将核心工程师调往 AI 数据标注](https://newsletter.pragmaticengineer.com/p/why-is-meta-destroying-its-engineering) ⭐️ 8.0/10

一篇文章声称，Meta 正在强制将核心团队的 30%-50% 的工程师调往 AI 数据标注和 RLHF 任务，这令员工大为不满。 此举突显了整个行业对 AI 的狂热，可能会损害 Meta 的工程文化、效率和士气，并可能为其他科技公司树立一个令人担忧的先例。 这种调动让高薪的软件工程师从事通常由低成本工人完成的数据标注工作，表明资源利用效率低下，且对核心产品的关注度下降。

hackernews · throwarayes · 6月16日 16:42 · [社区讨论](https://news.ycombinator.com/item?id=48558045)

**背景**: 数据标注是训练 AI 模型的关键步骤，传统上外包给低成本劳动力。RLHF（基于人类反馈的强化学习）是一种用于微调语言模型的技术。Meta 向 AI 的激进转型导致了内部紧张，工程文化被牺牲以换取 AI 的快速发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://snorkel.ai/data-labeling/">Data Labeling: A Complete Guide | Snorkel AI</a></li>

</ul>
</details>

**社区讨论**: 评论意见不一：一些前员工称 Meta 的自建团队效率低下，而另一些人则对如此高的调动比例表示怀疑。更广泛的担忧是，对 AI 的狂热正在加剧整个行业的毒性氛围。

**标签**: `#Meta`, `#engineering culture`, `#AI`, `#industry trends`, `#software engineering`

---

<a id="item-7"></a>
## [Qwen-Robot Suite：面向具身智能的基础模型套件](https://qwen.ai/blog?id=qwen-robotsuite) ⭐️ 8.0/10

阿里巴巴通义千问团队发布了 Qwen-Robot Suite，包含三个基础模型——Qwen-RobotNav、Qwen-RobotManip 和 Qwen-RobotWorld，分别用于机器人导航、操作和世界建模。 该套件标志着向集成具身智能迈出了重要一步，使开发者能够利用较小的模型构建完整的机器人系统，并实现大规模生产。这使通义千问在快速增长的机器人基础模型市场中占据关键地位。 Qwen-RobotNav 基于 Qwen3-VL 构建，提供 2B、4B 和 8B 三种参数规模。该套件涵盖导航、视觉-语言-动作（VLA）操作以及视频世界建模。

hackernews · ilreb · 6月16日 13:15 · [社区讨论](https://news.ycombinator.com/item?id=48554814)

**背景**: 机器人基础模型旨在提供可适应各种任务的通用能力，类似于文本领域的大型语言模型。具身 AI 需要能够感知、推理并在物理世界中行动的模型。通义千问的套件解决了三个核心方面：导航（移动）、操作（交互）和世界建模（预测）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://qwen.ai/home">Qwen</a></li>
<li><a href="https://digg.com/tech/6lxnua01">Alibaba's Qwen team releases Qwen - Robot Suite , a three-model...</a></li>
<li><a href="https://www.marktechpost.com/2026/06/16/meet-qwen-robotsuite-three-embodied-ai-models-for-vla-manipulation-video-world-modeling-and-navigation/">Meet Qwen -RobotSuite: Three Embodied AI Models... - MarkTechPost</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍积极，用户对大规模生产的潜力和战略重要性表示兴奋。有人询问替代方案以及快速处理接球等技术细节，也有人敦促欧洲加快步伐。

**标签**: `#AI`, `#Robotics`, `#Foundation Models`, `#Qwen`, `#Physical World Intelligence`

---

<a id="item-8"></a>
## [SubQ 1.1 Small：线性扩展的稀疏注意力机制](https://subq.ai/subq-1-1-small-technical-report) ⭐️ 8.0/10

SubQ 1.1 Small 提出了一种学习型稀疏注意力机制（SSA），其计算量随上下文长度线性扩展，在百万 token 长度下，相比 FlashAttention-2 可减少 64.5 倍计算量，推理速度快 56 倍。 这项工作表明，架构创新可以大幅降低长上下文 LLM 推理的成本，有望使大规模模型在实际应用中更易用且更高效。 SubQ 1.1 Small 在高达 1200 万 token 的 Needle in a Haystack 测试中取得高分，但 RULER 基准测试结果未超过 128k token，表明其在细粒度检索方面可能存在局限性。

hackernews · EDM115 · 6月16日 14:50 · [社区讨论](https://news.ycombinator.com/item?id=48556163)

**背景**: 传统注意力机制的计算复杂度为 O(n²)，导致长上下文推理成本高昂。稀疏注意力通过选择性关注部分 token 来降低复杂度，通常达到 O(n)或 O(n log n)。相关工作包括 BigBird、DeepSeek Sparse Attention（DSA）等。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@vishal09vns/sparse-attention-dad17691478c">Demystifying Sparse Attention : A Comprehensive Guide... | Medium</a></li>
<li><a href="https://www.emergentmind.com/topics/sparse-attention-mechanism">Sparse Attention Mechanism</a></li>
<li><a href="https://lzwjava.github.io/deepseek-sparse-attention-en">DeepSeek Sparse Attention Explained</a></li>

</ul>
</details>

**社区讨论**: 社区对加速效果和线性扩展表示兴趣，但多位评论者因缺乏架构细节和代码开源而持怀疑态度，对比之下更开放的中国实验室。还有人建议需要更好的长上下文基准测试，如长问答。

**标签**: `#LLM`, `#sparse attention`, `#architecture`, `#efficiency`, `#context length`

---

<a id="item-9"></a>
## [AI 模型出口管制削弱美国网络防御](https://simonwillison.net/2026/Jun/16/fable-5-export-controls/#atom-everything) ⭐️ 8.0/10

一项出口管制禁令针对 Claude Fable 5 修复含漏洞代码的能力，将合法的安全审计等同于越狱，安全专家 Kate Moussouris 指出这一点。 该政策可能阻碍防御性网络安全，阻止 AI 执行防御者日常依赖的关键“发现、修复、测试”循环。 研究人员使用了带有已知 CVE 的开源代码和故意植入的漏洞，要求 Fable 5“修复这段代码”；尽管经过多步骤手动处理，输出仍被视为被禁的越狱行为。

rss · Simon Willison · 6月16日 05:20

**背景**: AI 出口管制是限制先进 AI 模型跨境传输的法规，通常以国家安全为由。AI 越狱是指绕过内置安全护栏以获取受限响应。争议产生的原因在于修复代码是核心防御能力，而非攻击能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2024/06/04/ai-jailbreaks-what-they-are-and-how-they-can-be-mitigated/">AI jailbreaks: What they are and how they can be mitigated</a></li>

</ul>
</details>

**标签**: `#AI`, `#export controls`, `#cybersecurity`, `#policy`

---

<a id="item-10"></a>
## [警方滥用 Flock 摄像头进行跟踪](https://www.schneier.com/blog/archives/2026/06/flock-cameras-are-being-used-for-stalking.html) ⭐️ 8.0/10

美国各地已有超过十几起记录在案的案例，显示警察非法使用 Flock 监控摄像头跟踪个人，据 404 Media 和 Bruce Schneier 报道。 这种对监控技术的滥用破坏了公众信任，并引发了关于执法部门获取强大监控工具的严重隐私和伦理问题。 这些案例涉及警察使用 Flock 的自动车牌识别（ALPR）系统进行个人跟踪，而非用于合法的执法目的。

rss · Schneier on Security · 6月16日 11:03

**背景**: Flock Safety 是一家美国公司，向执法部门和社区提供 ALPR 和视频监控系统。该技术捕获并存储车牌数据，警官可通过软件访问。此前几年也有类似滥用报告，凸显了监控范围过大的系统性风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://www.cnet.com/home/security/when-flock-comes-to-town-why-cities-are-axing-the-controversial-surveillance-technology/">When Flock Surveillance Comes to Your Town: Everything ... - CNET</a></li>

</ul>
</details>

**标签**: `#privacy`, `#surveillance`, `#law enforcement`, `#ethics`

---

<a id="item-11"></a>
## [罗克韦尔控制器存在 CIP 拒绝服务漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-167-03) ⭐️ 8.0/10

美国 CISA 于 2026 年 6 月 16 日发布公告 ICSA-26-167-03，警告罗克韦尔自动化 CompactLogix 5370、Compact GuardLogix 5370、ControlLogix 5570 和 GuardLogix 5570 控制器存在拒绝服务漏洞（CVE-2026-11317），可导致重大不可恢复故障（MNRF）。该漏洞源于发送特制 CIP 消息时的不当资源关闭或释放。 该漏洞严重性高（CVSS 7.5），影响全球关键制造行业广泛使用的工业控制器，被利用可能导致对连接设备的控制或监视丢失，且恢复需要重新下载程序。 受影响产品包括 CompactLogix 5370 至版本 34.016、Compact GuardLogix 5370 至 35.015、ControlLogix 5570 至 35.015 以及 GuardLogix 5570 版本 36.012。罗克韦尔建议分别更新至 34.016、35.015、36.012 和 37.011 版本。内存较小的设备更易受影响。

rss · CISA Cybersecurity Advisories · 6月16日 12:00

**背景**: 通用工业协议（CIP）是工业自动化中广泛使用的通信协议，用于控制器和 I/O 模块等设备间的数据交换。重大不可恢复故障（MNRF）是罗克韦尔控制器中的一种严重错误状态，会导致设备重启，可能中断连接的操作。通用安全咨询框架（CSAF）是一种用于共享安全公告的机器可读格式，本 CISA 公告即采用该格式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Common_Industrial_Protocol">Common Industrial Protocol - Wikipedia</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2024-21916/">CVE-2024-21916: ControlLogix 5570 Controller DoS Vulnerability</a></li>

</ul>
</details>

**标签**: `#vulnerability`, `#ICS`, `#cybersecurity`, `#Rockwell Automation`, `#denial-of-service`

---

<a id="item-12"></a>
## [CISA 警告 Rockwell RSLinx Classic 存在高危拒绝服务漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-167-02) ⭐️ 8.0/10

CISA 发布了一份针对 CVE-2020-13573 的安全公告，该漏洞影响 Rockwell Automation RSLinx Classic 版本 <=4.50.00，可导致堆栈缓冲区溢出并造成拒绝服务。 该漏洞影响全球关键基础设施领域，包括能源、制造业和水务系统，可能导致运营中断。 该漏洞的 CVSS v3 基础评分为 7.5（高危），无需身份验证或用户交互即可利用。Rockwell 建议升级到 4.60.00 版本或应用补丁 BF31213。

rss · CISA Cybersecurity Advisories · 6月16日 12:00

**背景**: RSLinx Classic 是一款通信驱动程序，允许第三方软件通过 OPC DA 或 DDE 访问 Rockwell Automation 控制器，广泛应用于工业控制系统。CISA 以通用安全咨询框架（CSAF）格式提供机器可读的安全公告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://commerce.rockwellautomation.com/rockwell/en/INR/p/9355-RSLC/bundleBrand">RSLinx Classic</a></li>
<li><a href="https://github.com/cisagov/CSAF">GitHub - cisagov/CSAF: CISA CSAF Security Advisories CSAF Specification Common Security Advisory Framework Version 2.0 - OASIS Open Images What is the Common Security Advisory Framework (CSAF)? Technical Guideline TR-03191: Common Security Advisory ...</a></li>

</ul>
</details>

**标签**: `#ICS`, `#vulnerability`, `#Rockwell Automation`, `#denial of service`, `#security advisory`

---

<a id="item-13"></a>
## [CISA 警告 Rockwell PavilionX 存在授权缺失漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-167-01) ⭐️ 8.0/10

CISA 发布了 ICS 公告（ICSA-26-167-01），指出 Rockwell Automation FactoryTalk Analytics PavilionX 7.01 之前版本存在授权缺失漏洞（CVE-2025-14272），CVSS v3 基础评分 7.0（高危）。 该漏洞可能允许未经身份验证的攻击者执行用户和角色管理等特权操作，对全球关键制造基础设施构成重大风险。 该漏洞源于 API 端点中的授权执行不当，CVSS v4 评分为 8.3（高危）。Rockwell 建议更新至 7.01 或更高版本，更多缓解措施见 SD1777 公告。

rss · CISA Cybersecurity Advisories · 6月16日 12:00

**背景**: FactoryTalk Analytics PavilionX 是一种模型预测控制（MPC）软件，用于工业自动化中实时优化复杂过程。CISA 的公告采用通用安全咨询框架（CSAF）格式，这是一种用于自动化安全公告交换的机器可读标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rockwellautomation.com/en-us/products/software/factorytalk/operationsuite/pavilionX.html">PavilionX Model Predictive Control (MPC) | FactoryTalk | US</a></li>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>

</ul>
</details>

**标签**: `#CISA`, `#vulnerability`, `#OT security`, `#Rockwell Automation`, `#ICS`

---

<a id="item-14"></a>
## [Vertex AI SDK 漏洞致模型上传可被桶蹲点劫持](https://thehackernews.com/2026/06/google-vertex-ai-sdk-flaw-let-attackers.html) ⭐️ 8.0/10

Unit 42 发现 Google Vertex AI Python SDK 存在一个漏洞，攻击者可通过桶蹲点技术劫持机器学习模型上传，并在 Google 基础设施内执行远程代码。 该漏洞严重，因为它可实现跨租户远程代码执行，可能危及多个客户的模型和数据。它突显了共享云存储命名空间和 ML 工作流中不安全的反序列化风险。 该攻击名为"中间泡菜"，利用桶名全局唯一的特性，攻击者可以预先注册一个受害者 Vertex AI SDK 将来会使用的桶名。SDK 随后反序列化攻击者上传的恶意 pickle 文件，实现代码执行。

rss · The Hacker News · 6月16日 19:05

**背景**: 桶蹲点是一种攻击，攻击者先于合法用户声明云存储桶名，因为桶名是全局唯一的。在此漏洞中，Vertex AI Python SDK 使用了可预测的桶命名模式，使得攻击者可以创建一个该名称的桶。当受害者随后触发模型上传时，SDK 会写入攻击者的桶，然后攻击者可以上传一个恶意 pickle 文件，SDK 会反序列化该文件，导致远程代码执行。Pickle 文件是一种 Python 序列化格式，已知在反序列化不可信数据时存在危险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/transform/how-to-combat-bucket-squatting-in-five-steps">How to combat bucket squatting in five steps | Google Cloud Blog</a></li>
<li><a href="https://focalsecurity.io/blog/mitigating-bucket-squatting-gcp/">Mitigating Bucket Squatting in Google Cloud | Focal Security</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#google-cloud`, `#vertex-ai`, `#cloud-computing`

---

<a id="item-15"></a>
## [Rokarolla 安卓恶意软件攻击 217 个银行和加密应用](https://thehackernews.com/2026/06/new-rokarolla-android-malware-steals.html) ⭐️ 8.0/10

Zimperium 的 zLabs 安全研究人员发现了一种名为 Rokarolla 的新型安卓银行木马，它利用 137 条远程命令攻击 217 个银行和加密货币应用。 该恶意软件标志着移动威胁的重大升级，因为它能够窃取 PIN 码、短信验证码和加密货币钱包资金，可能给受害者造成重大经济损失。 Rokarolla 可以读取和发送短信，重写剪贴板内容以重定向加密货币支付，甚至禁用 Google Play 保护以逃避检测。

rss · The Hacker News · 6月16日 13:10

**背景**: 安卓银行木马是一类众所周知的恶意软件，用于窃取凭据和财务信息。然而，Rokarolla 展示了超越典型银行木马的先进能力，例如近乎完全控制设备以及针对加密货币钱包。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.darkreading.com/endpoint-security/rokarolla-android-trojan">Rokarolla Android Trojan Levels Up to Full Device Control</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/new-rokarolla-android-malware-targets-217-banking-crypto-apps/">New Rokarolla Android malware targets 217 banking, crypto apps</a></li>
<li><a href="https://zimperium.com/blog/rokarolla-android-banker-with-complete-device-takeover-capabilities">Rokarolla : Android Banker with Complete Device Takeover Capabilities</a></li>

</ul>
</details>

**标签**: `#malware`, `#android security`, `#banking trojan`, `#cryptocurrency`, `#mobile threats`

---

<a id="item-16"></a>
## [攻击者利用三个 Fortinet FortiSandbox 漏洞](https://thehackernews.com/2026/06/attackers-exploit-three-fortinet.html) ⭐️ 8.0/10

据威胁情报公司 Defused Cyber 报告，攻击者正在积极利用 Fortinet FortiSandbox 中的三个漏洞，其中包括一个严重的路径遍历漏洞（CVE-2026-39813，CVSS 9.1）。 这些漏洞正被积极利用，对使用 FortiSandbox 进行威胁检测的组织构成重大风险，需要紧急修补以防止入侵。 最严重的漏洞 CVE-2026-39813 是 FortiSandbox JRPC API 中的路径遍历漏洞，CVSS 评分为 9.1。另外两个被利用的 CVE 是 CVE-2026-39808 和 CVE-2026-25089。

rss · The Hacker News · 6月16日 10:30

**背景**: 路径遍历漏洞允许攻击者通过操纵文件路径输入来访问预期目录之外的文件。FortiSandbox 是一个网络威胁检测平台，可在沙盒环境中分析可疑文件。安全产品中的此类漏洞尤其危险，因为它们可用于绕过防御措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Path_traversal_vulnerability">Path traversal vulnerability</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#fortinet`, `#fortisandbox`, `#CVE`

---

<a id="item-17"></a>
## [SprySOCKS 后门新增 Windows 变体，采用驱动级隐身](https://thehackernews.com/2026/06/china-linked-sprysocks-backdoor-expands.html) ⭐️ 8.0/10

ESET 发现了两个以前仅存在于 Linux 系统的 SprySOCKS 后门的 Windows 变体，名为 WIN_DRV 和 WIN_PLUS，它们具备基于驱动的隐身能力以及硬编码的命令与控制配置。 此次扩展标志着与中国关联的威胁行为者能力的显著提升，使他们能够以隐蔽、持久的后门针对政府机构的 Windows 系统，引发了全球网络安全的担忧。 Windows 变体支持通过 TCP 和 UDP 进行通信，内部标记为 WIN_DRV 和 WIN_PLUS。它们与 Trochilus 远程访问木马和 RedLeaves 后门具有相似之处。

rss · The Hacker News · 6月16日 09:44

**背景**: SprySOCKS 最初于 2023 年被发现为 Linux 后门，基于名为 Trochilus 的 Windows 恶意软件。它提供典型的后门功能，如系统信息收集和远程 shell 访问。新的 Windows 变体采用了基于驱动的隐身技术，可能用于逃避检测并在受感染系统上保持持久性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/china-linked-sprysocks-backdoor-expands.html">China-Linked SprySOCKS Backdoor Expands to Windows with...</a></li>
<li><a href="https://arstechnica.com/security/2023/09/never-before-seen-linux-backdoor-is-a-windows-malware-knockoff/">Chinese hackers have unleashed a never-before-seen Linux backdoor</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#backdoor`, `#Windows`, `#malware`, `#threat intelligence`

---

<a id="item-18"></a>
## [CISA 将遭利用的 LiteSpeed cPanel 插件漏洞列入 KEV](https://thehackernews.com/2026/06/cisa-flags-litespeed-cpanel-plugin-flaw.html) ⭐️ 8.0/10

CISA 将 CVE-2026-54420（LiteSpeed cPanel 用户端插件中一个已被积极利用的权限提升漏洞）加入其已知被利用漏洞（KEV）目录，要求联邦民事行政分支（FCEB）机构在 2026 年 6 月 18 日前完成修复。 此漏洞至关重要，因为它允许 root 权限提升且已被积极利用，使成千上万的网络托管服务器面临风险。联邦机构被强制要求补丁，凸显了所有使用 LiteSpeed 与 cPanel 的组织面临的严重性和紧迫性。 该漏洞（CVSS 8.5）存在于面向终端用户的 LiteSpeed cPanel 插件中，允许未经身份验证的攻击者将权限提升至 root。CISA 的指令适用于 FCEB 机构，截止日期为 2026 年 6 月 18 日。

rss · The Hacker News · 6月16日 05:41

**背景**: LiteSpeed cPanel 插件是一个配套工具，允许网络托管提供商和终端用户通过 cPanel 管理 LiteSpeed Web Server 的安装。CISA 的已知被利用漏洞（KEV）目录跟踪已在野外被积极利用的漏洞，联邦机构必须在指定截止日期前修复目录中列出的漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.litespeedtech.com/lsws/cp/cpanel/whm-litespeed-plugin/cpanel-plugin/">cPanel Plugin | WHM Plugin | Control Panel Plugins ...</a></li>
<li><a href="https://www.cpanel.net/blog/products/how-to-install-litespeed-web-server-and-litespeed-cache-on-cpanel/">How To Install LiteSpeed Web Server and LiteSpeed Cache on cPanel</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CISA`, `#cPanel`, `#privilege-escalation`

---

<a id="item-19"></a>
## [恶意 JetBrains 插件盗窃 AI API 密钥](https://www.bleepingcomputer.com/news/security/malicious-jetbrains-marketplace-plugins-steal-ai-api-keys-from-developers/) ⭐️ 8.0/10

在 JetBrains Marketplace 上发现至少 15 个恶意插件，专门窃取开发者使用的 AI API 密钥，例如 OpenAI、Anthropic 等服务的密钥。 该攻击针对软件供应链，可能危及成千上万开发者及其组织的 AI 项目安全。 这些插件伪装成实用的开发工具并上传至官方市场；一旦安装，便会将存储的 API 密钥外泄至攻击者控制的服务器。

rss · BleepingComputer · 6月16日 21:54

**背景**: JetBrains Marketplace 是 JetBrains IDE（如 IntelliJ IDEA 和 PyCharm）的官方插件仓库。开发者常将 API 密钥存储在 IDE 设置或环境变量中，这使得它们成为供应链攻击的有利可图的目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://plugins.jetbrains.com/">IntelliJ IDEA Plugins and Themes | JetBrains Marketplace</a></li>
<li><a href="https://marketplace-support.jetbrains.com/hc/en-us">JetBrains Marketplace</a></li>

</ul>
</details>

**标签**: `#security`, `#supply-chain-attack`, `#jetbrains`, `#developer-tools`, `#AI`

---

<a id="item-20"></a>
## [Anthropic 的 Claude Code 数据：领域知识胜过编码技能](https://www.reddit.com/r/artificial/comments/1u7u9ju/anthropic_just_published_data_from_400k_claude/) ⭐️ 8.0/10

Anthropic 发布了研究报告，分析了约 40 万次 Claude Code 会话，显示律师、会计师等非工程师在编码任务上的成功率仅比专业软件工程师低 7 个百分点。 这一发现挑战了传统软件工程学位的价值，表明领域知识比纯粹编码能力更为关键，可能重塑招聘实践和软件开发工作的本质。 专家与中级用户之间的差距被称为“微小”，调试技能的使用率在七个月内下降了近一半，而平均任务价值提升了约 27%。

reddit · r/artificial · /u/Direct-Attention8597 · 6月16日 23:52

**背景**: Claude Code 是 Anthropic 的自主编码工具，能够理解代码库、编辑文件并运行命令。它基于 Claude 构建，Claude 是一个使用宪法 AI 进行伦理合规训练的大型语言模型。研究表明，AI 辅助编码工具正在降低非程序员参与软件开发的门槛。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#Claude Code`, `#AI productivity`, `#software engineering`, `#domain expertise`

---