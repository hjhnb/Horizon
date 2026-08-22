---
layout: default
title: "Horizon Summary: 2026-08-22 (ZH)"
date: 2026-08-22
lang: zh
---

> 从 77 条内容中筛选出 20 条重要资讯。

---

1. [公民在边境删手机数据被控重罪](#item-1)
2. [NVIDIA AVO 在 ARC-AGI-3 基准测试中取得满分](#item-2)
3. [GitLab 严重漏洞 CVE-2026-19478 披露后即遭积极利用](#item-3)
4. [微软修复 Entra ID 最高严重性漏洞并更正利用状态](#item-4)
5. [科学家发布迄今最大宇宙二维地图，配交互式查看器](#item-5)
6. [意外劫持 e164.arpa 域名，录下打往军事基地的电话](#item-6)
7. [DeepSeek 推出实验性视觉模型 DeepSeek-V4-Flash-Vision-Exp](#item-7)
8. [AI 公司破坏性扫描书籍，稀有图书面临消失风险](#item-8)
9. [机器人迎来 GPT-3 时刻：看一遍演示即可学会，黄仁勋李飞飞参投](#item-9)
10. [Simile AI CEO 称仿真为新的扩展定律](#item-10)
11. [NVIDIA 对 Poolside 的 120 亿美元逆向人才收购引发困惑](#item-11)
12. [AI 模型生成可存活的噬菌体完整基因组](#item-12)
13. [伪装 npm 包投放含 AI 辅助的 RedC2 Linux 后门](#item-13)
14. [微软 Defender 的 BTR.sys 驱动程序可被滥用删除安全软件](#item-14)
15. [泄露的 AWS 密钥可完全控制 9300 多个企业账户](#item-15)
16. [安卓恶意软件通过内置更新程序感染车载主机](#item-16)
17. [思科修复 Crosswork 与 Secure Workload 九项漏洞，其中五项为 CVSS 10.0 严重级别](#item-17)
18. [SynkLoader 恶意软件借微软 Teams 钓鱼活动传播](#item-18)
19. [CISA 下令修补已遭利用的 TrueConf Server 漏洞](#item-19)
20. [黑客滥用 FTP 横幅传播新型 Windows 恶意软件](#item-20)

---

<a id="item-1"></a>
## [公民在边境删手机数据被控重罪](https://www.nytimes.com/2026/08/21/us/politics/samuel-tunick-deleted-phone-felony.html) ⭐️ 9.0/10

据报道，美国公民 Samuel Tunick 因在美国边境检查期间删除手机数据而面临重罪指控。《纽约时报》2026 年 8 月 21 日报道了这一案件，引发了科技界和公民自由团体的广泛关注。 该案可能为旅行者是否有权拒绝或阻挠边境电子设备搜查设立法律先例。它也凸显了政府监控权力与个人数字隐私之间日益紧张的矛盾，尤其是在加密和数据删除方面。 边境人员通常使用 Cellebrite 等取证工具解锁并提取手机数据，而删除文件可能被以妨碍公务或销毁证据罪起诉。图尼克案的具体指控和法律论点尚未完全披露，但该事件涉及在法律意义上加密或删除的数据是否仍算“存在”的问题。

hackernews · floathub · 8月21日 12:10 · [社区讨论](https://news.ycombinator.com/item?id=49386895)

**背景**: 根据美国法律，边境搜查是第四修正案搜查令要求的长期例外，海关官员可以在没有搜查令的情况下检查随身物品。近年来，这一例外扩展至数字设备，执法部门依赖 Cellebrite 等商业取证工具来访问上锁的手机。另一方面，安全删除方法——例如 crypto-erase（通过销毁加密密钥使数据不可读）——已成为保护敏感信息的标准防御手段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cellebrite">Cellebrite - Wikipedia</a></li>
<li><a href="https://www.kingston.com/en/blog/personal-storage/how-to-securely-erase-ssd">How to Securely Erase an SSD Before Sale or Disposal - Kingston Technology</a></li>
<li><a href="https://cellebrite.com/en/premium/">Mobile Device Extraction for Investigators | Cellebrite</a></li>

</ul>
</details>

**社区讨论**: 评论者围绕法律和技术策略展开争论：有人建议使用诱饵密码功能悄悄清除数据，有人讨论在过境前对手机镜像并在之后恢复，还有人表示完全不使用智能手机。此外，一位意大利用户抱怨 archive.ph 被其政府屏蔽，引发了关于监控和审查的更多讨论。

**标签**: `#privacy`, `#border search`, `#digital rights`, `#legal`, `#encryption`

---

<a id="item-2"></a>
## [NVIDIA AVO 在 ARC-AGI-3 基准测试中取得满分](https://developer.nvidia.com/blog/nvidia-avo-reaches-100-on-arc-agi-3-demonstrating-a-frontier-level-general-purpose-architecture-for-long-horizon-autonomous-agents/) ⭐️ 9.0/10

NVIDIA 宣布其 AVO（Agentic Variation Operators）架构在 ARC-AGI-3 基准测试中取得了 100%的满分成绩。该公司将 AVO 描述为一种面向长周期自主智能体的通用架构。 在 ARC-AGI-3 上取得 100%的成绩是代理式 AI（Agentic AI）领域的一个重要里程碑，尤其是像 GPT-5.6 Sol 这样的前沿模型在同一基准测试中仅获得 7.8%。这一成就凸显了周围的智能体脚手架（harness）——而不仅仅是语言模型——对于在新环境中实现类人推理和自主任务执行至关重要。 ARC-AGI-3 是一个交互式推理基准测试，要求智能体探索新颖的 2D 谜题环境、推断目标并规划行动。NVIDIA 的这一声明来自其开发者博客，尚未经过独立验证；博客强调，仅靠前沿语言模型是不够的，围绕它的智能体系统是关键。

rss · NVIDIA Developer Blog · 8月21日 13:00

**背景**: 智能体脚手架（agent harness）是围绕大语言模型（LLM）的软件基础设施，使其能够作为 AI 智能体运行，管理工具使用、记忆、状态持久化和反馈循环；2026 年流行的一个简化表达是“智能体 = 模型 + 脚手架”。ARC-AGI-3 由 ARC Prize 推出，是一个通过新颖、抽象、回合制环境来衡量智能体智能的交互式基准测试。AVO 是 NVIDIA 的一个研究项目，旨在构建一个面向持续自主工作的通用智能体架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/nvidia-avo-reaches-100-on-arc-agi-3-demonstrating-a-frontier-level-general-purpose-architecture-for-long-horizon-autonomous-agents/">NVIDIA AVO Reaches 100% on ARC-AGI-3, Demonstrating...</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#AI`, `#ARC-AGI`, `#Agentic AI`, `#Autonomous Agents`

---

<a id="item-3"></a>
## [GitLab 严重漏洞 CVE-2026-19478 披露后即遭积极利用](https://thehackernews.com/2026/08/gitlab-cve-2026-19478-comes-under.html) ⭐️ 9.0/10

watchTowr 披露，GitLab 中的严重代码注入漏洞 CVE-2026-19478（CVSS 9.4）在公开披露后数日内已被积极利用。该漏洞允许未认证攻击者在特定条件下修改或删除公开可访问的 GitLab 项目并重写其数据。 这一事件意义重大，因为这是一个已被积极利用的严重未认证漏洞，对运行 GitLab（尤其是自管理实例）的组织构成迫在眉睫的威胁。鉴于 GitLab 在软件开发中的广泛使用，成功利用可能导致数据丢失、供应链受损以及 CI/CD 流水线中断。 该漏洞源于 GraphQL 多路复用查询处理中的请求验证不当，使未认证用户能够通过 GET 请求执行变更操作。GitLab 已发布紧急补丁，敦促组织立即应用；watchTowr 研究人员在公告发布后不久即检测到活跃利用。

rss · The Hacker News · 8月21日 07:04

**背景**: GitLab 是一个广泛使用的 DevOps 平台，提供 Git 仓库管理、CI/CD 和项目协作功能。CVE-2026-19478 是一个代码注入漏洞，允许未认证攻击者在特定条件下修改或删除公开项目。GitLab 已修复该问题，但披露后数日内即出现活跃利用，凸显了及时补丁管理的重要性。运行自管理 GitLab 实例的组织风险最高，因为需要自行应用补丁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/gitlab-cve-2026-19478-comes-under.html">GitLab CVE-2026-19478 Comes Under Active Exploitation Within ...</a></li>
<li><a href="https://www.securityweek.com/gitlab-patches-critical-code-injection-vulnerability/">GitLab Patches Critical Code Injection Vulnerability - SecurityWeek</a></li>
<li><a href="https://www.govinfosecurity.com/gitlab-code-injection-flaw-exploited-in-wild-a-32606">GitLab Code Injection Flaw Exploited in the Wild</a></li>

</ul>
</details>

**标签**: `#security`, `#CVE`, `#GitLab`, `#active exploitation`, `#vulnerability`

---

<a id="item-4"></a>
## [微软修复 Entra ID 最高严重性漏洞并更正利用状态](https://www.bleepingcomputer.com/news/microsoft/microsoft-warns-of-max-severity-entra-id-flaw-exploited-in-attacks/) ⭐️ 9.0/10

微软已修复其云端身份与访问管理服务 Entra ID 中的一个最高严重性漏洞。最初的公告将该漏洞标记为“已遭利用”，但微软在 The Hacker News 询问后，已将可利用性评估（Exploitability Assessment）状态更正为“否”。 由于 Entra ID 是 Microsoft 365、Azure 及众多第三方服务的身份验证基础，该平台出现最高严重性漏洞可能令身份验证与授权系统面临攻击风险。尽管微软如今表示该漏洞尚未遭利用，各组织仍应优先部署补丁。 微软在 2026 年 8 月 21 日发布的更新中，将该漏洞可利用性评估（Exploitability Assessment）表格中的“已遭利用”（Exploited）字段从“是”改为“否”。微软还重申该漏洞未在攻击中被利用。

rss · BleepingComputer · 8月21日 11:04

**背景**: Microsoft Entra ID 前身为 Azure Active Directory（Azure AD），是基于云的身份和访问管理（IAM）解决方案，为 Microsoft 365、Azure 及第三方应用提供身份验证与授权服务。它支持单一登录、多因素身份验证、条件访问和身份保护。微软于 2023 年 7 月将 Azure AD 更名为 Entra ID，以与其更广泛的 Entra 产品线保持一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Entra_ID">Microsoft Entra ID</a></li>
<li><a href="https://www.microsoft.com/en-us/msrc/exploitability-index">Microsoft Exploitability Index</a></li>

</ul>
</details>

**标签**: `#security`, `#Microsoft`, `#Entra ID`, `#vulnerability`, `#IAM`

---

<a id="item-5"></a>
## [科学家发布迄今最大宇宙二维地图，配交互式查看器](https://newscenter.lbl.gov/2026/08/10/scientists-release-biggest-2d-map-of-the-universe/) ⭐️ 8.0/10

科学家发布了迄今最全面的宇宙二维地图，如今可通过交互式 Legacy Survey Sky Viewer 查看器访问。这一成果是重要的科学里程碑，预计数年内仍将是最完整的二维宇宙地图。 这张地图为研究人员和公众提供了一种前所未有的方式来探索数十亿个星系及其他天体。它也凸显了大规模数据可视化在天文学和科学计算中日益增长的重要性。 该地图结合了 MzLS、DECaLS 和 BASS 巡天在 g、r、z 光学波段的数据，以及 NEOWISE 的红外数据，覆盖约 14,000 平方度的河外星系天区。在线查看器允许用户缩放到特定坐标，社区成员也分享了深空视图的直接链接。

hackernews · NKosmatos · 8月21日 18:36 · [社区讨论](https://news.ycombinator.com/item?id=49392200)

**背景**: Legacy Surveys 是一组地基巡天项目，结合了三个光学巡天和 NEOWISE 的红外数据，绘制了北半球可见的河外星系天区。它不同于未来在 Vera C. Rubin 天文台进行的 Legacy Survey of Space and Time (LSST)——后者将用十年时间扫描南天天区。二维地图只记录天体在天球上的位置，不包含距离信息；距离需要红移等额外测量才能确定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.legacysurvey.org/">Index | Legacy Survey</a></li>
<li><a href="https://www.legacysurvey.org/viewer">Legacy Survey Sky Browser</a></li>
<li><a href="http://viewer.legacysurvey.org/">Legacy Survey Sky Browser</a></li>

</ul>
</details>

**社区讨论**: 社区反应大多热烈，用户称赞查看器、分享特定坐标链接，并半开玩笑地称其为“Google Space”。一些评论者提出了技术问题，询问能否制作 3D 版本，因为二维地图缺乏距离数据；还有人担心经济压力可能减缓未来的天文学投资。

**标签**: `#astronomy`, `#universe mapping`, `#scientific data`, `#data visualization`, `#legacy survey`

---

<a id="item-6"></a>
## [意外劫持 e164.arpa 域名，录下打往军事基地的电话](https://lina.sh/blog/hijacking-e164-arpa) ⭐️ 8.0/10

作者意外接管了一个过期的 e164.arpa ENUM 区域，并记录了数十万次 DNS 查询，实际上录下了打往军事基地的电话。这一事件显示，在关键的互联网基础设施域名之下，一个被遗忘的子域可能泄露电话元数据。 这暴露了全球 ENUM 电话基础设施中的一个严重漏洞，影响依赖此类查询的运营商、政府机构和军事组织。同时，它也引发了对 .arpa 基础设施域名监管以及电话路由安全性的担忧。 e164.arpa 域名由 IANA 管理，用于 ENUM 服务，该服务将 E.164 电话号码映射为 DNS 名称。作者仅观察了 DNS 查询元数据，并未接通任何电话，但他指出，公共 ENUM 的使用已基本消亡，而私有号码携带服务仍依赖类似的查询。

hackernews · gavide · 8月21日 13:11 · [社区讨论](https://news.ycombinator.com/item?id=49387570)

**背景**: ENUM（电话号码映射）是 IETF 定义的协议，它将标准的 E.164 电话号码转换为 e164.arpa 域名下的 DNS 名称，使基于 IP 的服务能够路由呼叫。.arpa 顶级域保留用于互联网基础设施目的，由 IANA 管理。由于这些 DNS 记录用于定位电话端点，控制委派的 e164.arpa 区域可能让人观察到或重定向与呼叫相关的查询。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telephone_number_mapping">Telephone number mapping - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/.arpa">arpa - Wikipedia</a></li>
<li><a href="https://www.iana.org/domains/arpa">ARPA Domain</a></li>

</ul>
</details>

**社区讨论**: 评论者很欣赏这个故事，但对作者没有面临法律麻烦感到惊讶。有人指出 ENUM 并没有真正消亡，因为私有号码携带服务仍在使用 e164.arpa 风格的查询；还有人希望作者能更进一步，搭建 SIP 服务器。许多人觉得，只有牵扯到军方后问题才引起重视，这很讽刺。

**标签**: `#security`, `#ENUM`, `#telephony`, `#DNS`, `#vulnerability`

---

<a id="item-7"></a>
## [DeepSeek 推出实验性视觉模型 DeepSeek-V4-Flash-Vision-Exp](https://api-docs.deepseek.com/guides/vision/) ⭐️ 8.0/10

DeepSeek 已在其中文 API 平台上发布实验性多模态模型 DeepSeek-V4-Flash-Vision-Exp。该模型新增了图像理解和 OCR 能力，在文本任务上与 DeepSeek-V4-Flash 相当，并在多模态智能体基准上取得显著提升。 该发布填补了 DeepSeek 此前缺少视觉能力的重大空白，使其能与 GPT-4V、Claude 等多模态模型竞争。开发者现在可以将 DeepSeek 用于基于图像的智能体、OCR 和截图驱动的工作流，从而拓展其实际应用范围。 图像会根据其尺寸被转换为 token，并与文本 token 一起计费；在推理前，图像会自动调整大小，使总像素数约为 800×800。对于整页 A4 或 Letter 纸张的 OCR 任务，这一分辨率可能不够用；此外，该模型被标记为实验性，预计存在一些局限。

hackernews · dares2573 · 8月21日 10:33 · [社区讨论](https://news.ycombinator.com/item?id=49386163)

**背景**: 视觉语言模型（VLM）是一种能够同时从图像和文本中解释并生成信息的人工智能系统，是对仅支持文本的大型语言模型（LLM）能力的扩展。OpenAI、Google、Anthropic 和 Microsoft 等主要厂商已将此类能力集成到 GPT-4V、Gemini、Claude 等产品中，社区中也有 LLaVA 等开源视觉语言模型。DeepSeek 之前的模型主要以文本为主，社区曾指出其 API 缺少原生的视觉支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news260821/">DeepSeek-V4-Flash-Vision-Exp Release: Multimodal API Now Live | DeepSeek API Docs</a></li>
<li><a href="https://api-docs.deepseek.com/updates/">Change Log | DeepSeek API Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision-language_model">Vision-language model</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，但也指出了局限性：一位用户对用 DeepSeek 处理 Playwright 截图感到兴奋，另一位用户则报告该模型在简单的时钟识别测试中失败，而一个更小的模型基本能完成。其他用户提到 800×800 的缩放对于整页 OCR 可能不够；还有人指出此前纯文本模型经常幻觉自己有视觉能力，因此这次升级很受欢迎。

**标签**: `#DeepSeek`, `#vision-language-model`, `#AI`, `#LLM`, `#multimodal`

---

<a id="item-8"></a>
## [AI 公司破坏性扫描书籍，稀有图书面临消失风险](https://annas-archive.gl/blog/physical-destruction.html) ⭐️ 8.0/10

据报道，一些 AI 公司为了构建训练数据集，采用破坏性扫描方式，导致书籍被物理损毁。该博客文章呼吁在稀有书籍永久消失之前尽快对其进行扫描保存。 这个问题之所以重要，是因为它凸显了 AI 数据采集与文化保护之间的冲突。如果稀有或独特的书籍在数字化过程中被销毁，可能导致人类书面遗产永久损失。 破坏性扫描比非破坏性方法便宜得多，有时成本可低至十分之一，据说亚马逊和 Anthropic 等公司采用这种做法。而谷歌图书和互联网档案馆使用的非破坏性扫描能保留实体书，但成本更高。

hackernews · Cider9986 · 8月21日 02:37 · [社区讨论](https://news.ycombinator.com/item?id=49383026)

**背景**: 大规模数字化是指将实体图书大规模转化为数字文件，通常用于在线图书馆或 AI 训练。谷歌图书开创了非破坏性扫描，但现在一些 AI 公司为了使用自动进纸扫描仪，会切掉书脊。虽然生成了数字副本，但实体文物本身却消失了，这对于稀有或绝版书籍尤其令人担忧。互联网档案馆提供完全非破坏性的数字化服务，以保护原始资料。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mass_digitization">Mass digitization</a></li>
<li><a href="https://digitization.archive.org/digitization/">Digitization » Internet Archive Digitization Services</a></li>
<li><a href="https://www.erecordsusa.com/destructive-vs-non-destructive-book-scanning">Destructive vs Non-Destructive Book Scanning: Decision Guide</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人认为在书籍还有多个副本时销毁一本并无大碍，也有人指责版权所有者限制了书籍获取。还有不少人指出，非破坏性扫描成本可高出 10 倍，且谷歌图书从未销毁过书籍。总体情绪是对企业为节省成本而牺牲稀有物品保护表示担忧。

**标签**: `#AI`, `#books`, `#copyright`, `#digitization`, `#preservation`

---

<a id="item-9"></a>
## [机器人迎来 GPT-3 时刻：看一遍演示即可学会，黄仁勋李飞飞参投](https://mp.weixin.qq.com/s?__biz=MzI3MTA0MTk1MA==&mid=2652719368&idx=1&sn=d5a0a68f04d7e09d9cabe5c4950db88e) ⭐️ 8.0/10

一家获黄仁勋、李飞飞参投的机器人 AI 公司发布了一款具身基础模型，机器人只需观看一次 3–12 秒的人类演示即可学会新任务，无需训练、微调或手写代码。报道称这是机器人领域的“GPT-3 时刻”。 如果该能力属实，意味着机器人从“手动编程”走向“看演示即学会”，有望大幅降低通用机器人落地门槛，加速具身智能在家庭、工厂和服务场景的普及，并带动更多资本涌入机器人基础模型赛道。 文章将这一模型称为“Agent 原生的具身大脑”，可在单次演示下完成零样本模仿学习，并强调“模型决定上限，数据决定能不能抵达上限”。报道未公开具体算法细节与基准测试结果。

rss · 新智元 · 8月21日 08:09

**背景**: 机器人基础模型（robot foundation model）是融合感知、决策与控制的大型预训练模型。零样本模仿学习的目标是让机器人基于已知任务与未知任务之间的共享特征进行泛化，从而完成从未显式训练过的任务。具身智能（embodied AI）指嵌入物理身体、通过传感器与环境交互并自主执行目标的人工智能系统。所谓“GPT-3 时刻”是指：类似 GPT-3 重塑自然语言处理，一个通用机器人模型有望让机器人通过自然演示而非代码来编程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2312.07843">[2312.07843] Foundation Models in Robotics: Applications ... Awesome Robot Foundation Models 2025–2026 - GitHub Foundation Models in Robotics: Applications, Challenges, and ... Foundation Models for Robotics - Stanford ILIAD GitHub - robotics-survey/Awesome-Robotics-Foundation-Models Robot Foundation Models explained - Humanoid.guide GEN-1.5: Embodied Foundation Models are One-Shot Learners ...</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/embodied-ai/">What is Embodied AI ? | NVIDIA Glossary</a></li>
<li><a href="https://www.preprints.org/manuscript/202306.1353/v1/download">Zero Shot Learning Recent Advances in Robotics</a></li>

</ul>
</details>

**标签**: `#robotics`, `#AI`, `#foundation models`, `#embodied AI`, `#zero-shot learning`

---

<a id="item-10"></a>
## [Simile AI CEO 称仿真为新的扩展定律](https://www.latent.space/p/simile) ⭐️ 8.0/10

在 Latent Space 的采访中，Simile AI 首席执行官、影响深远的 Generative Agents 项目创造者 Joon Sung Park 提出，仿真（simulation）是 AI 新的扩展定律（scaling law），并描述了公司为每个在世的人构建 80 亿数字孪生的目标。 这一论点重新定义了 AI 进展的来源：不仅靠更大的模型和数据，也靠在全球范围内模拟人类行为。如果成功，Simile 的数字孪生可能改变社会科学、政策规划和个性化 AI，同时也会带来隐私和伦理方面的担忧。 这次访谈是高层面的对话，而非技术深潜；Park 还提到，这项使命已从“有趣的探索”转变为“非常严肃的事业”。Simile 的目标是为每一个在世的人——大约 80 亿人——创建数字孪生。

rss · Latent Space · 8月21日 23:37

**背景**: 生成式智能体（generative agents）是由大语言模型驱动的 AI 系统，可以模拟可信的人类行为，Park 早前的工作已展示这一点。人类数字孪生是指个体的动态、数据驱动的虚拟表示，通过持续整合多模态数据来模拟、监测和预测现实世界的结果。传统上，AI 的扩展定律描述的是模型性能如何随算力、数据和参数规模提升；Park 则认为，仿真的深度和广度将是下一个前沿。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2508.13138v1">Human Digital Twin: Data, Models, Applications, and Challenges</a></li>
<li><a href="https://www.nature.com/articles/s41746-025-01910-w">A scoping review of human digital twins in healthcare ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#simulation`, `#generative agents`, `#digital twins`, `#scaling laws`

---

<a id="item-11"></a>
## [NVIDIA 对 Poolside 的 120 亿美元逆向人才收购引发困惑](https://www.latent.space/p/ainews-poolside-gets-12b-reverse) ⭐️ 8.0/10

NVIDIA 与 AI 初创公司 Poolside 达成一项 120 亿美元的“逆向人才收购”协议，据称创始团队以 10 亿美元留在 Poolside，员工以 60 亿美元转入 NVIDIA，同时名为“Infraco”的 neocloud 算力平台扩展到 7 吉瓦。这一非常规结构令外界感到困惑。 这笔交易凸显了 AI 行业中逆向人才收购的日益增长趋势，即大公司无需整体收购即可吸纳人才和技术。这可能重塑初创公司的估值方式和基础设施融资模式，尤其是 neocloud 迈向吉瓦级数据中心。 逆向人才收购通常指初创公司核心成员加入大型企业，而初创公司授权其技术。Neocloud 是为 AI 工作负载而生的专业云服务商；像“Infraco”这样的 7 吉瓦 neocloud 将代表一个超大规模建设，远超典型的超大规模容量。

rss · Latent Space · 8月21日 05:45

**背景**: Poolside AI 是一家基础模型初创公司，由前 GitHub CTO Jason Warner 与软件创业者 Eiso Kant 于 2023 年创立，专注于软件开发的 AI 应用。在 AI 人才争夺战中，逆向人才收购已成为常见策略：大型企业直接聘用明星研究人员并授权其模型，而非收购整个初创公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fastcompany.com/91384816/what-is-the-reverse-acquihire">What is the reverse-acquihire? - Fast Company</a></li>
<li><a href="https://en.wikipedia.org/wiki/Poolside_AI">Poolside AI - Wikipedia</a></li>
<li><a href="https://vast.ai/article/what-is-a-neocloud-business-model-explained">What Is a Neocloud ? The Business Model Explained</a></li>

</ul>
</details>

**标签**: `#AI`, `#NVIDIA`, `#Acquisition`, `#Infrastructure`, `#Compute`

---

<a id="item-12"></a>
## [AI 模型生成可存活的噬菌体完整基因组](https://www.schneier.com/blog/archives/2026/08/ai-is-learning-to-write-genetic-code.html) ⭐️ 8.0/10

人工智能模型成功生成了可存活的噬菌体完整基因组，从约 70 万个设计中选出 285 个进行合成并插入大肠杆菌，最终产生了可存活的噬菌体。这展示了人工智能在基因编码设计方面的重大能力。 这一突破标志着人工智能驱动基因设计的重大进展，对合成生物学和生物安全具有深远影响，因为人工智能现在可以创造自然界不存在的功能性病毒。它可能加速噬菌体疗法和基因工程的研究，同时也引发了对潜在滥用的担忧。 模型以感染大肠杆菌的现有噬菌体ΦX174 为模板。研究人员从约 70 万个设计中选出 285 个有希望的候选，合成相应的 DNA 分子并插入大肠杆菌，观察是否会产生可存活的噬菌体。

rss · Schneier on Security · 8月21日 16:51

**背景**: 噬菌体是感染并在细菌内复制的病毒，是生物圈中最常见和多样化的实体之一。ΦX174 是第一个被测序的 DNA 基因组，由 Fred Sanger 于 1977 年完成，其基因组长度为 5386 个碱基。这一已被充分理解的模式生物为人工智能驱动的基因组设计提供了有用的测试平台，并建立在数十年的合成生物学研究基础之上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bacteriophage">Bacteriophage</a></li>
<li><a href="https://en.wikipedia.org/wiki/ΦX174">ΦX174</a></li>
<li><a href="https://www.neb.com/en-us/products/n3023-x174-virion-dna">ΦX174 Virion DNA</a></li>

</ul>
</details>

**标签**: `#AI`, `#synthetic biology`, `#genetics`, `#biosecurity`, `#bacteriophage`

---

<a id="item-13"></a>
## [伪装 npm 包投放含 AI 辅助的 RedC2 Linux 后门](https://thehackernews.com/2026/08/14-trojanized-npm-packages-drop-redc2.html) ⭐️ 8.0/10

网络安全研究人员发现 14 个伪装成日历和连续打卡工具的恶意 npm 包，它们秘密投放具备 AI 辅助命令与控制（C2）功能的 RedC2 4.0 Linux 后门。当开发人员导入该模块时，恶意负载会执行，并将内置二进制文件作为独立后台进程启动。 此次供应链攻击针对开发人员工作站和构建系统，这些是进入软件供应链的高价值入口。AI 辅助的 C2 集成使后门更具适应性且更难被检测，提高了 npm 安全性和整个生态系统信任的风险。 这些 npm 包伪装成可用的工具，但在模块加载时会定位内置二进制文件，赋予其可执行权限并在后台启动。趋势科技的 TrendAI 报告称，RedC2 4.0 包含 AI 辅助的命令与控制功能，表明攻击者利用机器学习来规避防御并自动化攻击操作。

rss · The Hacker News · 8月21日 18:53

**背景**: npm 是 Node.js 的默认包管理器，也是最大的软件注册表之一，因此成为供应链攻击的主要目标。恶意包通常模仿合法工具来诱骗开发人员安装，从而危害下游项目。RedC2 是一种 Linux 后门，这里提到的“4.0”版本融入了 AI 辅助的 C2——这是恶意软件中日益增长的趋势，利用机器学习使命令与控制通道更具动态性且更难被规避。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.lavx.hu/article/14-trojanized-npm-packages-drop-redc2-4-0-linux-backdoor-with-ai-assisted-c2">14 Trojanized npm packages drop RedC 2 4.0 Linux backdoor with...</a></li>
<li><a href="https://cyberwebspider.com/the-hacker-news/trojanized-npm-packages-linux-backdoor/">AI-Driven Backdoor in npm Packages | Tech News</a></li>

</ul>
</details>

**标签**: `#supply chain`, `#npm`, `#malware`, `#security`, `#backdoor`

---

<a id="item-14"></a>
## [微软 Defender 的 BTR.sys 驱动程序可被滥用删除安全软件](https://thehackernews.com/2026/08/microsoft-defenders-own-driver-can-be.html) ⭐️ 8.0/10

Check Point Research 披露，微软 Defender 自带且经过合法签名的启动时修复驱动程序 BTR.sys 可被重新利用，在 Windows 7 至 Windows 11 25H2 系统上执行任意内核级文件和注册表操作，且无需利用任何软件漏洞。 由于 BTR.sys 是 Windows 的必需组件，无法被加入微软的易受攻击驱动程序阻止列表，也无法通过 WDAC 阻止而不影响 Defender 自身，因此具有管理员权限的攻击者获得了一种可靠的方法，可在众多 Windows 版本上禁用端点安全防护。 这种滥用方式不依赖导入外部驱动程序或利用漏洞，只是复用 Defender 自身已签名的驱动程序，在启动时删除或修改安全软件的文件和注册表项。该技术需要管理员权限，影响 Windows 7 至 Windows 11 25H2 的系统。

rss · The Hacker News · 8月21日 15:52

**背景**: 微软 Defender 包含一个名为 BTR.sys 的启动时修复驱动程序，用于在操作系统完全加载前清除持久性恶意软件。由于它以 Ring 0（内核模式）运行并由微软签名，因此受到 Windows 安全机制的信任。研究人员展示了该驱动程序的功能可被重定向，以执行任意文件和注册表操作，从而将防御工具转变为攻击原语。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/microsoft-defenders-own-driver-can-be.html">Microsoft Defender's Own Driver Can Be Weaponized to Delete ...</a></li>
<li><a href="https://research.checkpoint.com/2026/btr-reforged-weaponizing-defenders-remediation-driver-as-a-kernel-operation-primitive/">BTR Reforged: Weaponizing Defender’s Remediation Driver as...</a></li>
<li><a href="https://threat-intelligence.redeyesecurity.com/blog/defender-btr-sys-boot-driver-abuse-2026.html">Defender's Own BTR.sys Driver Can Delete Your EDR During Boot</a></li>

</ul>
</details>

**标签**: `#security`, `#windows`, `#vulnerability`, `#driver`, `#microsoft defender`

---

<a id="item-15"></a>
## [泄露的 AWS 密钥可完全控制 9300 多个企业账户](https://www.bleepingcomputer.com/news/security/hundreds-of-leaked-aws-keys-give-full-control-over-corporate-accounts/) ⭐️ 8.0/10

安全报告显示，2022 年 8 月至 2026 年 8 月期间，超过 9300 个活跃的 AWS 访问密钥被公开暴露且仍然有效。这些泄露的凭证可能让攻击者完全控制企业的 AWS 账户。 这是高影响的云安全威胁，因为有效的访问密钥绕过了常规登录保护并直接授予 API 访问权限。受影响的企业可能面临数据泄露、资源滥用或账户接管，因此紧急需要轮换密钥并加强监控。 AWS 访问密钥由访问密钥 ID 和秘密访问密钥组成，用于对 AWS CLI 或 API 的编程请求进行签名。这些密钥可能是通过公共代码仓库、日志或存储配置错误暴露的；组织应立即审计 IAM 用户并轮换任何可能已泄露的密钥。

rss · BleepingComputer · 8月21日 15:55

**背景**: AWS 访问密钥是 IAM 用户或 AWS 账户根用户的长期凭证，允许对 AWS 资源进行编程访问。IAM（身份和访问管理）控制谁可以访问 AWS 资源以及可以执行哪些操作，使其成为 DevOps 和云管理员的关键安全服务。最佳实践包括定期轮换密钥、使用临时凭证替代长期密钥。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html">Manage access keys for IAM users - AWS Identity and Access ...</a></li>
<li><a href="https://www.msp360.com/resources/blog/how-to-find-your-aws-access-key-id-and-secret-access-key/">How to find AWS access key ID and secret access key | MSP360</a></li>
<li><a href="https://www.linkedin.com/pulse/aws-iam-best-practices-devops-engineers-venkatesh-jaggaraju-5er9f">AWS IAM Best Practices for DevOps Engineers</a></li>

</ul>
</details>

**标签**: `#AWS`, `#security`, `#cloud`, `#credentials`, `#cybersecurity`

---

<a id="item-16"></a>
## [安卓恶意软件通过内置更新程序感染车载主机](https://thehackernews.com/2026/08/android-car-malware-spreads-through.html) ⭐️ 7.0/10

卡巴斯基研究人员于 2026 年 6 月发现一种新的安卓恶意软件家族，专门感染 DoFun 开发的车载主机固件。该恶意软件通过内置更新程序传播，并利用多阶段下载器实施广告欺诈和组建代理僵尸网络。 这是已知的首批专门针对安卓车载主机的恶意软件活动之一，扩大了汽车攻击面。这表明联网汽车的信息娱乐系统可能被滥用于牟利，并作为大规模僵尸网络中的代理节点。 该恶意软件针对 DoFun 开发的车载主机固件，并通过设备内置的更新机制传播，暗示供应链或更新渠道可能被攻破。卡巴斯基强调，其最终目标是投放多阶段下载器，随后实施广告欺诈并招募代理僵尸网络。

rss · The Hacker News · 8月21日 15:41

**背景**: 车载主机是车辆的中枢信息娱乐和控制组件，常运行安卓系统并连接互联网。代理僵尸网络是由受感染设备组成的网络，通过住宅或其他 IP 地址路由流量，以隐藏恶意活动，常用于广告欺诈或逃避检测。多阶段下载器将恶意功能分成多个阶段，每个阶段下载下一个阶段，以规避安全工具的检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Automotive_head_unit">Automotive head unit - Wikipedia</a></li>
<li><a href="https://www.bitsight.com/blog/mylobot-investigating-proxy-botnet">Mylobot: Investigating a proxy botnet | Bitsight</a></li>
<li><a href="https://www.illumio.com/blog/ransomware-techniques-net-assemblies-multi-stage-attack">Demystifying Ransomware Techniques Using .Net Assemblies: A Multi-Stage Attack - Illumio Cybersecurity Blog | Illumio</a></li>

</ul>
</details>

**标签**: `#malware`, `#Android`, `#cybersecurity`, `#automotive`, `#IoT`

---

<a id="item-17"></a>
## [思科修复 Crosswork 与 Secure Workload 九项漏洞，其中五项为 CVSS 10.0 严重级别](https://thehackernews.com/2026/08/cisco-patches-nine-crosswork-and-secure.html) ⭐️ 7.0/10

思科发布了一轮新的安全更新，修复了 Crosswork Data Gateway、Crosswork Network Controller、Crosswork Planning 和 Secure Workload Software 中的九个漏洞。其中五项漏洞的 CVSS 严重性评分为最高的 10.0，且其中有四项影响 Crosswork 组件，无论设备配置如何。 出现五项 CVSS 10.0 最高严重级别漏洞，意味着受影响产品可能面临严重的远程利用风险，攻击者有可能借此入侵网络管理和工作负载安全基础设施。依赖 Cisco Crosswork 进行网络自动化、并依赖 Secure Workload 实现零信任隔离的企业，应立即优先修补以降低风险。 在这九个漏洞中，有五个的 CVSS 评分为最高值 10.0，属于最严重的风险等级。其中四个漏洞影响 Crosswork Data Gateway、Crosswork Network Controller 和 Crosswork Planning，且不受设备配置影响，表明这些漏洞的暴露无需任何特定配置条件。

rss · The Hacker News · 8月21日 10:03

**背景**: Cisco Crosswork 是一个基于 AI 的网络自动化平台，帮助在多厂商 IP 网络中管理服务和设备生命周期，其组件包括 Data Gateway、Network Controller 和 Planning。Cisco Secure Workload 是一种安全解决方案，通过分段和零信任执行为多云环境中的工作负载提供保护。CVSS 是用于评定安全漏洞严重性的标准化框架，10.0 代表最严重的级别。这些产品通常部署在核心网络和数据中心环境中，因此其中的漏洞影响尤为重大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cisco.com/site/us/en/products/networking/software/crosswork-network-automation/index.html">Cisco Crosswork Network Automation</a></li>
<li><a href="https://www.cisco.com/site/us/en/products/networking/software/crosswork-network-controller/index.html">Cisco Crosswork Network Controller</a></li>
<li><a href="https://www.cisco.com/site/cn/zh/products/security/secure-workload/index.html">Cisco Secure Workload - Cisco</a></li>

</ul>
</details>

**标签**: `#security`, `#cisco`, `#vulnerabilities`, `#patches`, `#CVSS`

---

<a id="item-18"></a>
## [SynkLoader 恶意软件借微软 Teams 钓鱼活动传播](https://www.bleepingcomputer.com/news/security/new-synkloader-malware-pushed-in-microsoft-teams-phishing-campaign/) ⭐️ 7.0/10

安全公司 Expel 发现了一个此前未知的恶意软件家族 SynkLoader，它正通过 Microsoft Teams 钓鱼活动传播。该恶意软件利用伪造的锁屏界面诱骗受害者输入凭据。 这一事件很重要，因为攻击者正越来越多地利用 Microsoft Teams 等受信任的协作平台来投递恶意软件，从而绕过传统的电子邮件安全防护。安全团队需要了解这个新型加载器及其多语言规避技术。 SynkLoader 是一个模块化恶意软件加载器，采用多语言（Python、C#、C++、PowerShell）编写以规避检测。该活动的攻击者冒充 IT 服务台人员，诱骗目标点击恶意链接或打开附件。

rss · BleepingComputer · 8月21日 18:01

**背景**: 钓鱼攻击是一种社会工程学攻击，攻击者伪装成合法实体来诱骗人们泄露敏感信息。恶意软件加载器是一种用于在受害者机器上投放并运行额外载荷（如凭据窃取器）的恶意软件。在此活动中，伪造的锁屏会显示为合法的 Windows 登录界面，当受害者输入密码时，密码便会被发送给攻击者。Microsoft Teams 之所以成为热门的钓鱼载体，是因为来自协作者的消息比传统电子邮件更容易获得信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://radar.offseq.com/threat/synkloader-when-you-throw-in-everything-but-the-kitchen-sink-3503834114e296c8">SynkLoader: when you throw in everything but the kitchen sink - Live Threat Intelligence - Threat Radar | OffSeq.com</a></li>
<li><a href="https://expel.com/blog/synkloader-when-you-throw-in-everything-but-the-kitchen-sink/">SynkLoader: when you throw in everything but the kitchen sink | Expel</a></li>
<li><a href="https://mwalkowski.com/post/phishing-on-the-lock-screen/">Phishing on the lock screen: how a fake Windows 11 page helped capture a user's password during a red team test | Michał Walkowski</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#phishing`, `#Microsoft Teams`, `#credentials`

---

<a id="item-19"></a>
## [CISA 下令修补已遭利用的 TrueConf Server 漏洞](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-actively-exploited-trueconf-server-flaws/) ⭐️ 7.0/10

CISA 已下令美国联邦机构修补 TrueConf Server 中两个已被积极利用的漏洞。Kaspersky 向厂商报告相关攻击后，厂商于 2026 年 6 月 18 日发布了 5.3.9、5.4.9 和 5.5.5 版本修复了这些漏洞。 由于这些漏洞正在真实攻击中被积极利用，CISA 的指令迫使联邦机构迅速修补，同时也警告所有运行 TrueConf Server 的组织。未修补的自托管通信系统是入侵活动的高价值目标。 这些漏洞由 Kaspersky 报告，并已被 PhantomCore 和 Head Mare 等威胁行为者利用。受影响系统通常在 4307/TCP 端口暴露易受攻击的服务，修复版本为 TrueConf Server 5.3.9、5.4.9 和 5.5.5。

rss · BleepingComputer · 8月21日 12:25

**背景**: CISA 是美国网络安全和基础设施安全局，当威胁严重时会向联邦行政部门机构发布紧急指令。TrueConf Server 是一款自托管的视频会议和通信平台，由组织在自己的基础设施上运行。“积极利用”意味着攻击者已经利用这些漏洞入侵系统，因此快速补丁至关重要。Kaspersky 在公开披露前发现攻击并通知了厂商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lifestyleandtech.co.za/smart-tech/article/2026-08-14/organisations-face-new-attacks-via-unpatched-trueconf-videoconferencing-servers-kaspersky-warns">Organisations face new attacks via unpatched TrueConf ...</a></li>
<li><a href="https://thehackernews.com/2026/04/phantomcore-exploits-trueconf.html">PhantomCore Exploits TrueConf Vulnerabilities to Breach Russian...</a></li>
<li><a href="https://dev.to/anoymask/head-mare-breaches-trueconf-from-system-privileges-to-trojanized-legitimate-client-updates-1ke1">Head Mare Breaches TrueConf : From SYSTEM... - DEV Community</a></li>

</ul>
</details>

**标签**: `#security`, `#CISA`, `#vulnerability`, `#patching`, `#TrueConf`

---

<a id="item-20"></a>
## [黑客滥用 FTP 横幅传播新型 Windows 恶意软件](https://www.bleepingcomputer.com/news/security/hackers-abuse-ftp-server-banners-to-deliver-new-windows-malware/) ⭐️ 7.0/10

威胁行为者正利用 FTP 服务器横幅隐藏命令，以传播两种新发现的 Windows 远程访问木马 E4del 和 PINHOLE。MalwareHunterTeam 于 7 月在利用.LNK 快捷方式文件的攻击中首次观察到该技术。 这标志着将 FTP 横幅用作死信解析器的一种新颖且隐蔽的手段，可能绕过不检查横幅内容的安全工具。该发现凸显了攻击者滥用标准互联网协议进行命令与控制的演变趋势。 FTP 横幅通常用于标识服务器软件及版本，但在此次攻击活动中，它们被用于向受感染机器返回编码命令。这两种木马 E4del 和 PINHOLE 此前未被记录，似乎通过网络钓鱼或恶意快捷方式传播。

rss · BleepingComputer · 8月21日 11:00

**背景**: FTP（文件传输协议）服务器在客户端连接时会发送文本横幅，通常包含服务器名称和版本；横幅抓取是管理员和攻击者常用的服务识别技术。死信解析器是指由合法或攻击者控制的服务器，用于存储恶意软件检索的命令，使恶意流量能与正常通信混合，难以被察觉。远程访问木马（RAT）能让攻击者远程控制受害者计算机，实施数据窃取、监控或安装更多恶意软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-abuse-ftp-server-banners-to-deliver-new-windows-malware/">Hackers abuse FTP server banners to deliver new Windows malware</a></li>
<li><a href="https://en.wikipedia.org/wiki/Banner_grabbing">Banner grabbing - Wikipedia</a></li>
<li><a href="https://www.scworld.com/brief/attackers-use-ftp-banners-to-hide-new-e4del-and-pinhole-rats">Attackers use FTP banners to hide new E4del and PINHOLE RATs | brief | SC Media</a></li>

</ul>
</details>

**标签**: `#malware`, `#security`, `#FTP`, `#RAT`, `#threat actors`

---