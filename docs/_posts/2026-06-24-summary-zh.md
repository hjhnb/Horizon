---
layout: default
title: "Horizon Summary: 2026-06-24 (ZH)"
date: 2026-06-24
lang: zh
---

> 从 78 条内容中筛选出 20 条重要资讯。

---

1. [西门子 SIPROTEC 5 存在任意文件上传漏洞](#item-1)
2. [FortiBleed 从 43 万 FortiGate 防火墙窃取 1.1 亿条凭证](#item-2)
3. [美国行政令要求 2030 年前完成后量子密码迁移](#item-3)
4. [即将到来的循环：重新思考软件开发](#item-4)
5. [Unlimited OCR：一次性长文档解析](#item-5)
6. [Datasette 1.0a35 新增创建/修改表界面和 JSON API](#item-6)
7. [Anthropic 的 Fable 5 模型数日内被越狱](#item-7)
8. [NVIDIA DFlash 推测解码将 Blackwell 推理性能提升 15 倍](#item-8)
9. [IBM Research 发布 CUGA Agent 框架及其 24 个示例](#item-9)
10. [CISA 警告：Hubbell Aclara Metrum 存在关键认证绕过漏洞](#item-10)
11. [CISA 警告西门子产品中的 OpenSSL 缓冲区溢出漏洞](#item-11)
12. [西门子 WinCC 证书管理器漏洞泄露密钥材料](#item-12)
13. [CISA 警告 ABB Freelance 安全锁存在绕过漏洞](#item-13)
14. [CISA 警告西门子 SINEC INS 存在严重漏洞](#item-14)
15. [CISA 警告 B&R OT 产品存在 Linux 内核漏洞](#item-15)
16. [虚假 AI 技能绕过安全扫描，触及 26000 个 Agent](#item-16)
17. [七家中国公司已出货 H100 级 AI 芯片，挑战英伟达](#item-17)
18. [LLM 医疗记录基准测试发现遗漏比幻觉更常见](#item-18)
19. [Mimo 2.5 在双 RTX Pro 6000 上大上下文速度飞快](#item-19)
20. [映射 Qwen 和 Gemma 模型中 KV 缓存量化的 KLD](#item-20)

---

<a id="item-1"></a>
## [西门子 SIPROTEC 5 存在任意文件上传漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-02) ⭐️ 9.0/10

美国网络安全与基础设施安全局（CISA）发布了一份安全公告（ICSA-26-174-02），详细说明了西门子 SIPROTEC 5 设备通过 DIGSI 5 协议存在的任意文件上传漏洞，该漏洞可能导致永久性拒绝服务，CP050、CP150 和 CP300 型号已有固件修复可用。 该漏洞影响关键基础设施中使用的多种 SIPROTEC 5 保护继电器，可能允许经过身份验证的攻击者永久禁用设备，威胁电网稳定性和运行连续性。资产所有者应立即打补丁。 该漏洞（尚未分配 CVE 编号）被评定为高严重性，影响众多设备型号的所有版本；缓解措施包括将大多数设备升级到固件版本 9.90 或更高，将 7ST85/7ST86 CP300 型号升级到 10.00 或更高，这些版本实现了允许列表功能以限制文件上传。

rss · CISA Cybersecurity Advisories · 6月23日 12:00

**背景**: SIPROTEC 5 是西门子的一款数字化保护继电器系列，用于电网的保护、控制和自动化。DIGSI 5 协议是西门子用于配置这些设备的工程软件接口。任意文件上传漏洞允许经过身份验证的用户在未经过当验证的情况下上传恶意配置文件，可能覆盖关键系统文件并导致永久性拒绝服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.assurantcyber.com/blog/icsa-26-174-02/">Siemens SIPROTEC 5 Using DIGSI5 Protocol - ASSURANT™</a></li>
<li><a href="https://www.siemens.com/en-us/products/siprotec/">SIPROTEC Protection Relays | Siemens</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#ICS`, `#Siemens`, `#firmware`

---

<a id="item-2"></a>
## [FortiBleed 从 43 万 FortiGate 防火墙窃取 1.1 亿条凭证](https://thehackernews.com/2026/06/fortibleed-targeted-fortigate-firewalls.html) ⭐️ 9.0/10

一个讲俄语的初始访问代理自 2026 年 2 月起发起 FortiBleed 行动，攻击超过 43 万台 FortiGate 防火墙，通过暴力破解和定制嗅探器窃取超过 1.1 亿条凭证。 这次大规模凭证盗窃对依赖 FortiGate 防火墙保护网络安全的企业构成严重威胁，窃取的凭证可能被用于进一步入侵、勒索软件攻击或数据泄露。该行动的规模凸显了初始访问代理在网络犯罪生态系统中日益增长的威胁。 该行动使用定制的暴力破解流水线和网络嗅探器来识别暴露的 FortiGate 接口，已攻破 194 个国家的超过 43 万台设备。窃取的数据包括 SSL VPN 凭证，这些凭证可直接访问内部网络。

rss · The Hacker News · 6月23日 18:20

**背景**: 初始访问代理（IAB）是专门入侵网络并将访问权限出售给其他威胁行为者（如勒索软件组织）的网络犯罪分子。FortiGate 是 Fortinet 公司流行的企业防火墙品牌，常作为 VPN 网关使用。FortiBleed 行动得名于这次类似漏洞利用的系统性行动，从这些设备中系统性地窃取凭证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/fortibleed-targeted-fortigate-firewalls.html">FortiBleed Targeted FortiGate Firewalls in 110 Million-Credential ...</a></li>
<li><a href="https://cybersecuritynews.com/fortibleed-fortinet-firewalls-compromised/">FortiBleed - 70,000+ Fortinet Firewalls Compromised in Massive ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Initial_access_broker">Initial access broker - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#credential harvesting`, `#FortiGate`, `#firewalls`, `#IAB`

---

<a id="item-3"></a>
## [美国行政令要求 2030 年前完成后量子密码迁移](https://thehackernews.com/2026/06/trump-order-sets-2030-deadline-for.html) ⭐️ 9.0/10

特朗普总统于 6 月 22 日签署第 14409 号行政令，要求联邦机构在 2030 年 12 月 31 日前将高价值系统的密钥建立迁移至后量子密码，数字签名迁移截止日为 2031 年 12 月 31 日。 该行政令设定了硬性截止日期，迫使所有联邦机构进行大规模协调迁移，直接影响网络安全和软件工程实践。它同时应对了'先收后解'威胁——攻击者现在收集加密数据，待量子计算机成熟后再解密。 密钥建立须在 2030 年 12 月 31 日前完成迁移，数字签名在 2031 年 12 月 31 日前。国家安全系统另行安排，不适用这些截止日期。

rss · The Hacker News · 6月23日 15:16

**背景**: 后量子密码（PQC）是指被认为能够抵御量子计算机攻击的加密算法。当前公钥算法如 RSA 和 ECC 会被足够强大的量子计算机利用秀尔算法破解。'先收后解'攻击指攻击者现在存储加密数据，待量子计算机可用时再进行解密。该行政令旨在保护敏感数据免受此类未来威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Harvest_now,_decrypt_later">Harvest now, decrypt later - Wikipedia</a></li>

</ul>
</details>

**标签**: `#post-quantum cryptography`, `#cybersecurity`, `#executive order`, `#quantum computing`, `#federal policy`

---

<a id="item-4"></a>
## [即将到来的循环：重新思考软件开发](https://lucumr.pocoo.org/2026/6/23/the-coming-loop/) ⭐️ 8.0/10

文章认为，软件开发的核心瓶颈在于获取清晰的规格说明，而非实现循环，AI 代理正在将范式从构建软件转向指定软件。 这一观点重新定义了开发者和 AI 代理的角色，强调规格清晰性的真正价值，可能重塑团队动态、工具和教育方式。 作者认为，即使是使用先进的代理，编写多个有缺陷的版本以达成清晰理解的迭代循环也是不可避免的；代理擅长执行清晰的规格，而非定义它们。

hackernews · ingve · 6月23日 11:06 · [社区讨论](https://news.ycombinator.com/item?id=48643180)

**背景**: 在软件开发中，迭代循环指的是编码、测试和基于反馈进行优化的循环。清晰的规格说明是指导实现的蓝图。像 Claude Code 这样的 AI 代理是能自动化部分循环的新兴工具，但它们依赖于清晰的输入。

**社区讨论**: 评论者普遍认为规格清晰性是主要瓶颈。有人指出，当规格清晰时，代理循环效果很好，但定义这些规格需要大量人力且无法完全自动化。还有的讨论了将软件视为生命体的范式转变。

**标签**: `#software development`, `#AI agents`, `#iterative loops`, `#specification`, `#paradigm shift`

---

<a id="item-5"></a>
## [Unlimited OCR：一次性长文档解析](https://github.com/baidu/Unlimited-OCR) ⭐️ 8.0/10

百度 Unlimited OCR 提出了一种新颖的方法，通过防止 KV 缓存线性增长，使模型能够一次性处理整个 PDF 文档而不会耗尽内存。 该方法解决了基于 Transformer 的 OCR 中的关键内存瓶颈，能够无需分块地无缝处理长文档，从而提高准确性并简化文档数字化工作流中的管道设计。 该技术修改了注意力机制，避免缓存所有过去的键值对，而是采用流式处理，在一定点后丢弃旧上下文。该项目是开源的，并基于 Deepseek-OCR 和 PaddleOCR 模型。

hackernews · ingve · 6月23日 11:35 · [社区讨论](https://news.ycombinator.com/item?id=48643426)

**背景**: Transformer 模型顺序生成文本令牌，为了加速推理，它们会缓存之前的键值对（KV 缓存），其大小随序列长度线性增长。对于长文档，这个缓存会迅速耗尽 GPU 内存，迫使开发者将文档分成多页。Unlimited OCR 的创新在于控制缓存增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@minh.hoque/understanding-kv-caching-in-transformers-729271c9b74a">Understanding KV Caching in Transformers - Medium</a></li>
<li><a href="https://arxiv.org/pdf/2603.20397">KV Cache Optimization Strategies for Scalable and Efficient LLM Inference</a></li>

</ul>
</details>

**社区讨论**: 社区讨论积极，重点在于避免内存囤积的巧妙架构技巧。评论者还注意到该项目使用了 Deepseek-OCR 和 PaddleOCR，有人指出其名称参考了《Fate/stay night》中的'无限剑制'。论文已在 arXiv 上发布。

**标签**: `#OCR`, `#deep learning`, `#memory optimization`, `#document parsing`, `#AI`

---

<a id="item-6"></a>
## [Datasette 1.0a35 新增创建/修改表界面和 JSON API](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a35 引入了“创建表”界面和 JSON API，以及用于修改现有表的“修改表”界面和 JSON API。这些功能允许用户直接通过 Web 界面和 API 管理数据库模式。 此版本显著增强了 Datasette 的功能，通过无需原始 SQL 即可进行模式管理，使其成为更完整的数据发布平台。它使用户能够通过友好的交互界面设计和修改数据库表。 创建表 API 支持定义列、主键、自定义列类型、NOT NULL 约束、文字默认值和表达式默认值以及单列外键。修改表 API 支持添加、重命名、重新排序和删除列，以及更改列类型、默认值、约束、主键、外键和重命名表。

rss · Simon Willison · 6月23日 21:34

**背景**: Datasette 是一个开源的多功能工具，用于将数据探索、分析和发布为交互式网站和 API，基于 SQLite 构建。在此次 alpha 版本发布之前，创建或修改表需要直接使用 SQL 或外部工具。此版本将这些模式管理功能引入了 Datasette 核心界面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and ...</a></li>

</ul>
</details>

**标签**: `#datasette`, `#data publishing`, `#SQLite`, `#web API`, `#database`

---

<a id="item-7"></a>
## [Anthropic 的 Fable 5 模型数日内被越狱](https://www.schneier.com/blog/archives/2026/06/anthropics-fable-5-model-jailbroken-within-days.html) ⭐️ 8.0/10

Anthropic 的安全导向模型 Fable 5（Mythos Preview 的带护栏版本）在发布后数日内即被越狱，用户得以绕过旨在防止其被用于网络攻击的限制。 这一事件凸显了即使安全措施是核心设计目标，保护先进 AI 系统仍然面临持久挑战。它突显了 AI 安全研究人员与攻击者之间持续的猫鼠游戏，并对当前护栏技术的可靠性提出了质疑。 Fable 5 专门通过护栏强化以防止被用于生成网络攻击，但越狱仍迅速成功。初始报道未详述具体方法，但此类绕过通常利用微妙的提示操纵或模型漏洞。

rss · Schneier on Security · 6月23日 11:03

**背景**: AI 越狱是指精心构造输入以绕过模型的安全训练和护栏，从而产生受限或有害输出的做法。护栏是实时监控、过滤和控制 AI 输出以防止有害内容的安全机制。尽管已有大量研究，但尚无模型被证明能完全免疫越狱，尤其是在能力不断提升的背景下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/ai-jailbreak/">AI jailbreaking - GeeksforGeeks</a></li>
<li><a href="https://aisecurityandsafety.org/en/guides/jailbreaking-attacks/">Jailbreaking AI Models: Attack Patterns, Examples & Defenses ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#jailbreak`, `#Anthropic`, `#cybersecurity`

---

<a id="item-8"></a>
## [NVIDIA DFlash 推测解码将 Blackwell 推理性能提升 15 倍](https://developer.nvidia.com/blog/boost-inference-performance-up-to-15x-on-nvidia-blackwell-using-dflash-speculative-decoding/) ⭐️ 8.0/10

NVIDIA 宣布了 DFlash 技术，该技术利用轻量级块扩散模型进行并行草稿生成，在 Blackwell 硬件上实现了高达 15 倍的推理加速。 这一突破显著降低了 LLM 推理延迟，对多智能体工作流和实时 AI 应用至关重要，并展示了将先进 GPU 架构与高效解码算法相结合的潜力。 DFlash 采用块扩散模型，单次前向传播即可生成草稿 token，克服了 EAGLE-3 等先前方法的自回归瓶颈。它通过从目标 LLM 提取上下文特征来条件化草稿模型，从而保证输出质量。

rss · NVIDIA Developer Blog · 6月23日 15:00

**背景**: 推测解码通过使用小型草稿模型并行生成 token，再由大型目标模型验证，从而加速 LLM 推理。然而，EAGLE-3 等先前草稿器逐 token 自回归生成，速度提升仅 2-3 倍。DFlash 的并行草稿生成克服了这一限制，而 NVIDIA Blackwell 硬件提供了实现 15 倍性能提升的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2602.06036">DFlash: Block Diffusion for Flash Speculative Decoding</a></li>
<li><a href="https://github.com/z-lab/dflash">DFlash: Block Diffusion for Flash Speculative Decoding - GitHub</a></li>

</ul>
</details>

**标签**: `#inference`, `#speculative decoding`, `#NVIDIA Blackwell`, `#LLM`, `#performance`

---

<a id="item-9"></a>
## [IBM Research 发布 CUGA Agent 框架及其 24 个示例](https://huggingface.co/blog/ibm-research/cuga-apps) ⭐️ 8.0/10

IBM Research 在 Hugging Face Spaces 上发布了 CUGA（可配置通用智能体），并附带了二十多个用于构建智能 AI 应用的工作示例。 此次发布为开发者提供了一个轻量级、开源的框架及其实用示例，降低了构建企业级智能 AI 系统的门槛。 CUGA 采用模块化、多层、多智能体架构，包含一个计划控制器智能体，可将任务分解并编排工作流，示例涵盖多种网络和 API 环境。

rss · Hugging Face Blog · 6月23日 12:51

**背景**: 智能 AI 是指能够自主感知、推理并采取行动以实现目标的 AI 系统。框架（harness）是将模型连接到实际应用的结构化控制层。CUGA 是 IBM 为构建企业级此类系统而提供的开源方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.ibm.com/blog/cuga-agent-framework">Introducing CUGA: The enterprise-ready configurable generalist agent - IBM Research</a></li>
<li><a href="https://www.infoq.com/news/2025/12/ibm-cuga/">IBM Research Introduces CUGA, an Open-Source Configurable Agent Framework on Hugging Face - InfoQ</a></li>
<li><a href="https://mitsloan.mit.edu/ideas-made-to-matter/agentic-ai-explained">Agentic AI, explained | MIT Sloan</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#frameworks`, `#Hugging Face`, `#IBM Research`, `#examples`

---

<a id="item-10"></a>
## [CISA 警告：Hubbell Aclara Metrum 存在关键认证绕过漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-07) ⭐️ 8.0/10

CISA 发布了关于 CVE-2026-1840 的警告（ICSA-26-174-07），该漏洞是 Hubbell Aclara Metrum 蜂窝网络接口中的缺失认证漏洞，攻击者无需凭证即可操纵设备设置并中断通信。 该漏洞影响美国关键能源基础设施，可能使远程攻击者造成运营中断并导致智能电网设备通信丢失。 该漏洞（CWE-306）的 CVSS v3 基础评分为 7.5，影响 v2.1.0.105 之前的版本。Hubbell 已发布固件 v2.1.0.105 来修复此问题，建议用户更新并避免设备暴露于互联网。

rss · CISA Cybersecurity Advisories · 6月23日 12:00

**背景**: Aclara Metrum Cellular 是一款用于电网的 4G LTE 通信模块，用于智能电网应用如 AMI 和停电管理。关键功能缺失认证意味着网络接口无需任何登录，任何具有网络访问权限的人都能更改设置或重启设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://windowsforum.com/threads/cve-2026-1840-hubbell-aclara-web-interface-missing-auth-enables-ot-restarts.429600/">CVE-2026-1840 Hubbell Aclara Web Interface: Missing Auth ...</a></li>
<li><a href="https://news.shield53.com/critical-authentication-gap-in-hubbell-aclara-metrum-puts-us-energy-grid-devices-at-risk/">Critical Authentication Gap in Hubbell Aclara Metrum Puts U.S ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#critical infrastructure`, `#energy`, `#CISA`

---

<a id="item-11"></a>
## [CISA 警告西门子产品中的 OpenSSL 缓冲区溢出漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-03) ⭐️ 8.0/10

CISA 发布了一份关于 OpenSSL（CVE-2025-15467）中基于堆栈的缓冲区溢出漏洞的公告，该漏洞影响众多西门子工业产品，如 SCALANCE 路由器和 AI Lightweight Inference Server。西门子已为部分产品发布补丁，并为其他产品建议了缓解措施。 该漏洞可能允许远程攻击者在关键运营技术系统上造成拒绝服务或执行任意代码。鉴于西门子在工业环境中的广泛使用，利用该漏洞可能破坏基础设施和生产线。 该漏洞（CVE-2025-15467）是 OpenSSL CMS 解析中的基于堆栈的缓冲区溢出，影响 3.0 至 3.6 版本。许多受影响的西门子产品所有版本均被列为易受攻击，部分产品暂无立即修复方案。

rss · CISA Cybersecurity Advisories · 6月23日 12:00

**背景**: 基于堆栈的缓冲区溢出发生在程序向堆栈上的缓冲区写入超过分配大小的数据时，可能覆盖返回地址并导致代码执行。OpenSSL 是一个广泛使用的加密库，实现了 TLS/SSL；其漏洞可能对嵌入它的许多产品产生广泛影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cve.org/CVERecord?id=CVE-2025-15467">CVE Record: CVE-2025-15467</a></li>
<li><a href="https://orca.security/resources/blog/cve-2025-15467-openssl-pre-auth-rce/">CVE-2025-15467: Critical OpenSSL RCE Vulnerability Explained ...</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2025-15467/">CVE-2025-15467: OpenSSL Buffer Overflow Vulnerability</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#OpenSSL`, `#Siemens`, `#CISA`

---

<a id="item-12"></a>
## [西门子 WinCC 证书管理器漏洞泄露密钥材料](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-01) ⭐️ 8.0/10

CISA 披露了西门子 WinCC 证书管理器中的一个高危漏洞 (CVE-2026-24349, CVSS 7.1), 该漏洞因明文存储密钥材料到磁盘, 使攻击者能够提取敏感信息。西门子已针对 SIMATIC WinCC Unified PC Runtime V21 发布修复版本 (Update 2), 并建议立即更新。 该漏洞影响广泛应用于关键基础设施领域（能源、制造、交通等）的工业控制系统，攻击者可能借此破坏加密通信和基于证书的身份验证。及时修补对维持运营安全至关重要。 受影响产品包括 SIMATIC WinCC Unified PC Runtime V16 至 V20 的所有版本，以及 V21 的 Update 2 之前版本。对于 V16–V20 版本，西门子不计划提供修复，建议限制操作员访问并遵循安全指南。

rss · CISA Cybersecurity Advisories · 6月23日 12:00

**背景**: WinCC 证书管理器负责管理西门子 SCADA 系统中加密通信所需的证书。该漏洞源于以明文形式存储密钥材料 (CWE-313)，使本地或远程攻击者能够提取证书和私钥。CSAF（通用安全咨询框架）是 CISA 现用于 ICS 公告的机器可读格式，本公告即采用该格式。

**标签**: `#security`, `#vulnerability`, `#ICS`, `#Siemens`, `#certificate management`

---

<a id="item-13"></a>
## [CISA 警告 ABB Freelance 安全锁存在绕过漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-05) ⭐️ 8.0/10

2026 年 6 月 23 日，CISA 发布公告，警告 ABB Freelance 安全锁中存在 CVE-2025-7064 身份验证绕过漏洞，攻击者可利用未公开的按键组合访问底层 Windows 操作系统功能。 该漏洞影响全球关键制造业基础设施，可能使攻击者绕过安全限制，在 ABB Freelance DCS 环境的操作员控制台上获得未经授权的操作系统访问权限。 该漏洞（CVSS 3.1 基础评分 6.6）影响从 Freelance 2013 到 Freelance 2024 的所有 ABB Freelance 安全锁版本，利用需要物理或本地访问配有现代键盘的操作员站。

rss · CISA Cybersecurity Advisories · 6月23日 12:00

**背景**: ABB Freelance 是一种用于关键制造业过程自动化领域的分布式控制系统（DCS）。其安全锁功能旨在通过阻止对 Windows 桌面的访问，将操作员限制在一组受控的 OT 应用程序内。该漏洞允许使用特殊按键组合绕过该锁，从而可能使攻击者在系统上运行任意命令或恶意软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://windowsnews.ai/article/abb-freelance-security-lock-flaw-lets-attackers-hijack-ot-consoles-patch-now.429597">ABB Freelance Security Lock Flaw Lets Attackers Hijack OT Consoles — Patch Now - Windows News</a></li>
<li><a href="https://library.abb.com/share?cid=9aac115759">ABB Library - Freelance</a></li>
<li><a href="https://www.abb.com/global/en/areas/automation/control-systems/freelance">ABB Freelance DCS | Automation | ABB</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#ICS`, `#ABB`, `#CISA`

---

<a id="item-14"></a>
## [CISA 警告西门子 SINEC INS 存在严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-04) ⭐️ 8.0/10

CISA 发布了咨询报告（ICSA-26-174-04），警告西门子 SINEC INS 在 V1.0 SP2 Update 6 之前版本存在多个漏洞，包括操作系统命令注入（CVE-2026-46746）和路径遍历（CVE-2026-46747），CVSS 评分为 8.8。西门子已发布新版本并建议用户更新至最新版本。 这些漏洞可能允许经过身份验证的远程攻击者在底层操作系统上执行任意命令或访问未授权文件，对能源、交通和制造等工业环境构成高风险。由于 SINEC INS 在全球关键基础设施中部署，紧急修补对于防止潜在 OT 系统入侵至关重要。 最严重的漏洞（CVE-2026-46746，CVSS 8.8）是/api/sftp/uploadFiles 端点中的 OS 命令注入，通过精心构造的目录名可导致以 sinecins 服务用户权限执行 shell 命令。路径遍历漏洞（CVE-2026-46747）影响同一端点的目录列表功能，允许攻击者访问未授权的文件系统位置。

rss · CISA Cybersecurity Advisories · 6月23日 12:00

**背景**: SINEC INS（基础设施网络服务）是西门子用于 OT（运营技术）环境中央网络服务的软件工具，通过统一界面管理和监控网络服务。OS 命令注入（CWE-78）是指应用程序将未净化的用户输入传递给系统 shell，从而允许攻击者执行任意 OS 命令。路径遍历则通过操纵文件路径输入，使攻击者能够读取预期目录之外的文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.siemens.com/us/en/products/automation/industrial-communication/sinec-networkmanagement/sinec-ins-infrastructure-network-services.html">SINEC INS Infrastructure Network Services - Siemens US</a></li>
<li><a href="https://portswigger.net/web-security/os-command-injection">What is OS command injection, and how to prevent it? | Web ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#ICS`, `#Siemens`, `#OT`

---

<a id="item-15"></a>
## [CISA 警告 B&R OT 产品存在 Linux 内核漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-174-06) ⭐️ 8.0/10

CISA 发布了咨询报告（ICSA-26-174-06），详细说明了 B&R 工业自动化产品（包括 Linux for B&R、APROL 和 X20EDS410）存在的多个 Linux 内核漏洞，且已有公开的概念验证利用代码。 这些漏洞可能允许本地攻击者在关键制造业使用的 OT 系统上提升权限，从而可能扰乱全球工业运营。 该咨询报告指出漏洞的 CVSS v3 评分为 7.8，涉及写任意位置条件、越界写入等问题。B&R 已为 APROL 4.4 版本发布补丁，其他受影响产品仍在等待修复。

rss · CISA Cybersecurity Advisories · 6月23日 12:00

**背景**: B&R 工业自动化（现属 ABB 集团）是一家奥地利公司，专注于机器和工厂自动化。其产品如 APROL 过程控制软件和 X20EDS410 边缘设备运行 Linux，并部署在全球工业控制系统中。Linux 内核漏洞可被本地利用以获取更高权限，对 OT 环境构成风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/B&R">B&R - Wikipedia</a></li>
<li><a href="https://www.br-automation.com/en/products/process-control/aprol-software/">APROL software | B&R Industrial Automation</a></li>
<li><a href="https://www.br-automation.com/en/products/plc-systems/x20-system/x20-edge/x20eds410/">X20EDS410 | B&R Industrial Automation</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#CISA`, `#Linux kernel`, `#vulnerabilities`, `#industrial control systems`

---

<a id="item-16"></a>
## [虚假 AI 技能绕过安全扫描，触及 26000 个 Agent](https://thehackernews.com/2026/06/fake-ai-agent-skill-passed-security.html) ⭐️ 8.0/10

安全公司 AIR 构建了一个虚假的 AI agent 技能，该技能通过了所有安全扫描器，并通过技能市场和一个 Instagram 广告触及了约 26000 个 agent，证明了当前审查机制的不足。 这一演示暴露了 AI agent 技能市场的关键安全漏洞，表明恶意技能可能未被检测到就被部署，从而可能危及企业及个人 AI agent 的安全。 该载荷仅设计为收集用户的电子邮件地址作为无害的概念验证，但同样的技术可用于传递更危险的恶意软件，例如凭证窃取或 agent 劫持。

rss · The Hacker News · 6月23日 15:16

**背景**: AI agent 技能市场是允许用户浏览和安装 AI agent 封装能力的平台，类似于智能手机的应用商店。安全扫描器是在安装前分析这些技能中是否存在恶意代码的自动化工具。这一事件表明，当前的扫描器甚至无法检测到简单的恶意模式，引发了对整个生态系统安全性的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/AI_agent_skills_marketplace">AI agent skills marketplace</a></li>
<li><a href="https://mondoo.com/ai-agent-security">AI Agent Skill Security Scanner - Scan Before You Install</a></li>

</ul>
</details>

**标签**: `#security`, `#AI agents`, `#vulnerability`, `#marketplace`, `#malware`

---

<a id="item-17"></a>
## [七家中国公司已出货 H100 级 AI 芯片，挑战英伟达](https://www.reddit.com/r/LocalLLaMA/comments/1udkxde/7_chinese_companies_are_already_shipping/) ⭐️ 8.0/10

根据 Reddit 上的一篇帖子（总结自 CHITEX 首席技术官 Dmitry Shilov 的演讲），至少七家中国公司正在出货性能媲美英伟达 H100 的人工智能加速器，其中多数在过去六个月内上市。 这一进展挑战了英伟达在 AI 硬件市场的主导地位，并可能重塑全球供应链，尤其是在美国对华先进芯片出口管制的背景下。 这些公司分为“三龙”（华为、阿里巴巴、百度）和“四蛇”（纯芯片公司），其中华为的 Ascend 950PR 据称性能超过 H200，阿里巴巴的平头哥（T-Head）计划于 2026 年 1 月开始分拆上市。

reddit · r/LocalLLaMA · /u/awfulalexey · 6月23日 15:50

**背景**: 英伟达 H100 GPU 基于 Hopper 架构，是用于 AI 训练和推理的领先数据中心加速器，但美国出口限制限制了其向中国的销售。作为回应，中国公司开发了自己的高性能替代品，许多员工来自英伟达、AMD 和英特尔，现已出货有竞争力的产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h100/">H100 GPU | NVIDIA</a></li>
<li><a href="https://www.techspot.com/news/112624-china-military-obtained-nvidia-chips-despite-us-export.html">China's military obtained Nvidia chips despite US export controls, report claims | TechSpot</a></li>
<li><a href="https://aichipnav.com/ai-accelerators/nvidia-h100">NVIDIA H100 - AI Accelerator Specs and Overview</a></li>

</ul>
</details>

**标签**: `#Chinese AI chips`, `#NVIDIA competition`, `#AI hardware`, `#semiconductor`, `#export controls`

---

<a id="item-18"></a>
## [LLM 医疗记录基准测试发现遗漏比幻觉更常见](https://www.reddit.com/r/LocalLLaMA/comments/1udlrmf/i_benchmarked_8_llms_for_medical_scribing/) ⭐️ 8.0/10

一项针对 8 个大语言模型在 300 个合成医患对话上的基准测试发现，安全关键事实的遗漏发生率是幻觉的 43 倍——在生成的 2400 份医疗 SOAP 记录中，共出现 520 次遗漏和 12 次幻觉。 这一发现将医疗 AI 安全讨论从常见的幻觉转向更为普遍的遗漏问题，遗漏可能导致漏诊或不安全的护理。同时，它也表明像 DeepSeek 这样的高性价比模型可能需要额外的安全层才能在临床上可用。 该基准测试使用了一个四模型评审团来评估散文质量、幻觉、遗漏的安全事实、成本和速度。显著结果包括 GPT-5.4-mini 在成本和速度上表现出色，Claude Opus 遗漏最少但散文质量较差，Kimi 实现了零确认幻觉但速度慢且成本高。

reddit · r/LocalLLaMA · /u/MajesticAd2862 · 6月23日 16:20

**背景**: SOAP（主观、客观、评估、计划）记录是医疗提供者用于记录患者就诊的标准格式。前沿模型是最先进的通用 AI 模型，能够处理广泛的任务。该基准测试使用 AI 生成的合成医患对话来模拟真实的临床对话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SOAP_note">SOAP note - Wikipedia</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>
<li><a href="https://aclanthology.org/2026.eacl-industry.40/">Synthetic Doctor-Patient Dialogue Generation for Robust ...</a></li>

</ul>
</details>

**标签**: `#LLM benchmarking`, `#medical AI`, `#AI safety`, `#natural language processing`

---

<a id="item-19"></a>
## [Mimo 2.5 在双 RTX Pro 6000 上大上下文速度飞快](https://www.reddit.com/r/LocalLLaMA/comments/1udwabh/mimo_25_is_fast_at_large_context_dual_rtx_pro_6000/) ⭐️ 8.0/10

Mimo 2.5 采用类似 Gemma 3 的 5:1 局部/全局滑动窗口注意力机制，在双 RTX Pro 6000 GPU 上大上下文长度下保持高推理速度，而 MiniMax M3 和 DeepSeek V4 等模型因其自定义内核与消费级 Blackwell GPU 不兼容而大幅降速。 这表明注意力机制设计对本地大模型的实际部署至关重要；采用良好支持注意力模式的模型能在消费级硬件上提供稳定性能，使得以前需要数据中心 GPU 的高上下文长度代理工作成为可能。 Mimo 2.5 在编程基准测试中约 4 分钟完成，与 Opus/Sonnet 相当，而 MiniMax M3 需要约 40 分钟；Step 3.7 Flash（3:1 滑动窗口）在 178k 上下文下也表现良好，约 40 t/s，同时指出 NVFP4 在 SM120 上存在缺陷。

reddit · r/LocalLLaMA · /u/xquarx · 6月23日 22:55

**背景**: 滑动窗口注意力将每个 token 的注意力限制在最近的局部窗口内，相比全局注意力降低计算复杂度；部分模型添加全局层以实现全上下文访问。GGUF 是一种量化模型文件格式，被 llama.cpp 和 Ollama 等本地推理工具使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Attention_Is_All_You_Need">Attention Is All You Need - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/GGUF">GGUF</a></li>
<li><a href="https://mimo.xiaomi.com/mimo-v2-5">MiMo-V2.5 | Xiaomi</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#large-context`, `#attention-mechanism`, `#gpu-performance`, `#mimo`

---

<a id="item-20"></a>
## [映射 Qwen 和 Gemma 模型中 KV 缓存量化的 KLD](https://www.reddit.com/r/LocalLLaMA/comments/1udjvhd/i_mapped_the_kld_of_kv_cache_quantization_for/) ⭐️ 8.0/10

Reddit 用户 crusaderky 发布了一份详细分析，绘制了 Qwen3.6-35B-A3B 和 Gemma4-E2B QAT 模型在不同 KV 缓存量化水平下的 Kullback-Leibler 散度（KLD），并附带了可复现结果的软件。 这项工作提供了关于 KV 缓存压缩与模型质量损失之间权衡的宝贵实证见解，有助于从业者选择最优的量化水平以提高推理效率。 关键发现包括：q8/q8 量化在两种模型上几乎无损失，q4/q4 在 Qwen 上可用但在 Gemma 上灾难性，turbo4 有时优于 q4_0，而 turbo2/3 以高成本实现了极端压缩。

reddit · r/LocalLLaMA · /u/crusaderky · 6月23日 15:12

**背景**: KV 缓存量化通过在推理时以较低精度存储键和值来减少内存使用。Kullback-Leibler 散度（KLD）衡量原始模型和量化模型输出分布之间的差异，作为质量损失的代理指标。量化感知训练（QAT）微调模型以更好地容忍量化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/kv-cache-quantization">Unlocking Longer Generation with Key-Value Cache Quantization</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kullback–Leibler_divergence">Kullback–Leibler divergence - Wikipedia</a></li>

</ul>
</details>

**标签**: `#KV cache quantization`, `#LLM inference`, `#Qwen`, `#Gemma`, `#model optimization`

---