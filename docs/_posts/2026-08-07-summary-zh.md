---
layout: default
title: "Horizon Summary: 2026-08-07 (ZH)"
date: 2026-08-07
lang: zh
---

> 从 82 条内容中筛选出 20 条重要资讯。

---

1. [Zapscape KVM 漏洞可致特权 L1 Guest 逃逸至 Linux 主机](#item-1)
2. [新型中断注入攻击绕过英特尔与 AMD CPU 的 Spectre v2 防御](#item-2)
3. [CISA 警示：TeamCity 关键 RCE 漏洞 CVE-2026-63077 遭活跃利用](#item-3)
4. [Snowflake 黑客就影响超 1 亿人的数据泄露认罪](#item-4)
5. [新 TONTOU CPU 攻击绕过 Spectre v2 修复，泄露 Linux 密码哈希](#item-5)
6. [AMD 收购 AI 芯片初创公司 Taalas，将模型硬编码进硅片](#item-6)
7. [OpenAI 改进 GPT-5.6 Sol，并扩大免费用户对 GPT-5.6 Luna 的访问](#item-7)
8. [Qwen3.8 Max 登顶 Agentic 指数，前沿 AI 竞争加剧](#item-8)
9. [Datasette 1.0a38 修复可暴露私有表的 SQL 注入漏洞](#item-9)
10. [CryptoJS 弱随机数生成器致 5 个加密钱包应用损失 570 万美元](#item-10)
11. [AI 推荐投毒：“Ask AI”深度链接注入隐藏提示词](#item-11)
12. [攻击者将 khunt 编译进 Oracle，将 SQL 注入升级为 Windows SYSTEM 访问](#item-12)
13. [AWS、Google、Vercel 智能体漏洞绕过模型监管](#item-13)
14. [Zbtlink 路由器出厂预装后门，可开启未授权 Root Shell](#item-14)
15. [往返一致性让双向扩散模型自测推算误差](#item-15)
16. [用《马力欧卡丁车》角色属性解释帕累托最优与权衡](#item-16)
17. [Herdr 加入 Y Combinator，运行时保持开源](#item-17)
18. [品味成为 AI 时代软件工程仅存的人类特质](#item-18)
19. [FCC 取消广播电视所有权全国上限](#item-19)
20. [Datasette 0.65.3 移植 SQL 注入安全修复](#item-20)

---

<a id="item-1"></a>
## [Zapscape KVM 漏洞可致特权 L1 Guest 逃逸至 Linux 主机](https://thehackernews.com/2026/08/new-zapscape-kvm-flaw-could-let.html) ⭐️ 9.0/10

一个名为 Zapscape（CVE-2026-64561）的新 Linux 内核漏洞，可让拥有 L1 客户机内核权限的攻击者突破 KVM 隔离，在宿主机上执行任意代码。该漏洞影响 KVM/x86 的 shadow MMU，在向不可信客户机开放嵌套虚拟化时可被利用。 这是一个关键的 guest 到 host 逃逸漏洞，打破了虚拟化的核心安全边界，可能让攻击者完全控制宿主机。云服务商、数据中心以及任何向多租户环境暴露嵌套虚拟化的 KVM 部署都需要紧急修补。 该漏洞位于 x86 KVM shadow MMU 的影子页表管理代码中，该代码负责在嵌套分页不可用或被禁用时将客户机物理地址转换为主机物理地址。它只在向不可信租户暴露嵌套虚拟化（L1 guest）时适用；若不启用嵌套虚拟化，则无法触达此攻击面。

rss · The Hacker News · 8月6日 17:58

**背景**: KVM（基于内核的虚拟机）是 Linux 内核的虚拟化基础设施。在嵌套虚拟化中，L0 Hypervisor 运行一个 L1 客户机，该客户机自身充当 Hypervisor 并运行 L2 客户机。KVM/x86 shadow MMU 为这类客户机维护影子页表，Zapscape 漏洞就存在于这条代码路径中；2026 年早些时候披露的 16 年历史漏洞 Januscape（CVE-2026-53359）同样位于 shadow MMU 代码中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.kernel.org/virt/kvm/x86/mmu.html">The x86 kvm shadow mmu — The Linux Kernel documentation</a></li>
<li><a href="https://docs.kernel.org/virt/kvm/x86/running-nested-guests.html">Running nested guests with KVM — The Linux Kernel documentation</a></li>
<li><a href="https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html">16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host on Intel...</a></li>

</ul>
</details>

**标签**: `#security`, `#kernel`, `#virtualization`, `#KVM`, `#vulnerability`

---

<a id="item-2"></a>
## [新型中断注入攻击绕过英特尔与 AMD CPU 的 Spectre v2 防御](https://thehackernews.com/2026/08/new-interrupt-injection-attack-can.html) ⭐️ 9.0/10

MIT CSAIL 的研究人员 Daniël Trujillo 和 Mengjia Yan 公布了一种名为 INTERRUPT INJECTION 的新攻击，它允许一个无特权的 Linux 程序精确定时硬件中断，在 Spectre v2 防御运行之后重新污染分支预测器。该技术在一台运行 Linux 6.14 且启用所有默认 Spectre v2 缓解措施的 AMD Zen 2 机器上得到验证，并且还在两款 Intel CPU 上触发了内核误预测。 这种攻击破坏了当前 Spectre v2 缓解措施的核心假设，表明在内核使用分支预测器之前，如果中断可以落在清理后的间隙中，仅对分支预测器进行净化是不够的。由于它同时影响 Intel 和 AMD 处理器，并且可以由无特权用户执行，因此对系统安全构成重大的实际威胁，需要新的防御策略。 该攻击针对基于中和（neutralization）的缓解措施，例如 AMD 的 Safe-RET，这些措施依赖于净化或隔离分支预测器状态。研究人员发现，如果中断处理在中和与使用之间执行，中断返回路径就会成为 Spectre v2 防御的一部分；在 Zen 2 上，这个可利用窗口只有两条指令、六个字节长。

rss · The Hacker News · 8月6日 16:17

**背景**: 现代 CPU 使用分支预测器来猜测条件跳转的结果，以保持指令流水线满载，但 2018 年公开的 Spectre 漏洞表明，这种推测执行可能通过侧信道泄露敏感数据。Spectre v2 缓解措施的原理是在跨越特权边界（例如从用户态进入内核态）时中和或隔离分支预测器。然而，这些基于中和的防御在净化预测器与内核实际使用它之间留下了一个小的时间窗口，而新的中断注入攻击恰好利用这个间隙重新污染预测器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/new-interrupt-injection-attack-can.html">New Interrupt Injection Attack Can Bypass Spectre v 2 Defenses on...</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/new-tontou-cpu-attack-bypasses-spectre-v2-fixes-leaks-linux-password-hashes/">New TONTOU CPU attack bypasses Spectre v 2 fixes, leaks Linux...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Branch_predictor">Branch predictor - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#Spectre`, `#CPU`, `#side-channel`, `#research`

---

<a id="item-3"></a>
## [CISA 警示：TeamCity 关键 RCE 漏洞 CVE-2026-63077 遭活跃利用](https://thehackernews.com/2026/08/cisa-flags-teamcity-cve-2026-63077-rce.html) ⭐️ 9.0/10

CISA 已标记 CVE-2026-63077 为正在被活跃利用的漏洞，这是 JetBrains TeamCity 本地服务器中的一个严重未认证远程代码执行漏洞。该漏洞属于不可信数据反序列化问题，CVSS 评分为 9.8，影响 2026.1.3 和 2025.11.7 之前的版本。 TeamCity 被广泛用于 CI/CD 流水线，许多本地实例可能暴露在互联网上。未认证的 RCE 攻击者可接管构建服务器，可能导致供应链攻击，因此安全团队必须立即修补。 根据 NVD，该漏洞存在于 2026.1.3 和 2025.11.7 之前的 JetBrains TeamCity 中，可通过代理轮询协议实现远程代码执行。攻击者只需具有 HTTP(S)访问权限即可利用，9.8 的 CVSS 评分反映了无需认证的特点。

rss · The Hacker News · 8月6日 06:51

**背景**: TeamCity 是 JetBrains 的持续集成/持续交付（CI/CD）工具，用于自动化构建、测试和部署。不可信数据反序列化是一种编程弱点，应用程序在未验证的情况下反序列化恶意数据，从而导致代码执行。CISA 通常会将活跃利用的漏洞加入已知被利用漏洞目录，以提醒机构和组织及时修补。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2026-63077">NVD - CVE - 2026 - 63077</a></li>
<li><a href="https://www.rapid7.com/db/vulnerabilities/cve-2026-63077/">CVE - 2026 - 63077 : Deserialization of... | Rapid7 Vulnerability Database</a></li>
<li><a href="https://owasp.org/www-community/vulnerabilities/Deserialization_of_untrusted_data">Deserialization of untrusted data | OWASP Foundation</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CVE`, `#JetBrains TeamCity`, `#RCE`

---

<a id="item-4"></a>
## [Snowflake 黑客就影响超 1 亿人的数据泄露认罪](https://thehackernews.com/2026/08/snowflake-hacker-pleads-guilty-over.html) ⭐️ 9.0/10

26 岁的加拿大人康纳·莱利·穆卡在华盛顿州西雅图联邦法院认罪，承认涉及 2024 年 Snowflake 数据泄露的计算机欺诈、电信欺诈、严重身份盗窃及相关共谋指控。此次入侵影响了至少 165 家组织，并暴露了超过 1 亿人的记录，包括 AT&T 客户的通话和短信历史。 这标志着 2024 年最具影响力的网络犯罪案件之一取得了重大法律进展，表明针对云数据提供商的国际黑客可以被起诉并追究责任。它向业界发出强烈信号，凸显云数据泄露的严重性以及保护客户环境安全的重要性。 来自安大略省基奇纳的穆卡承认窃取了超过 1 亿 AT&T 用户的通话和短信历史记录，并个人获利至少 49.5 万美元。认罪涉及计算机欺诈、电信欺诈、严重身份盗窃和共谋罪名。

rss · The Hacker News · 8月6日 06:04

**背景**: Snowflake 是一个广泛使用的云数据平台，帮助组织以可扩展的方式存储、共享和分析大量数据。2024 年，一系列入侵活动针对 Snowflake 客户，通常通过滥用窃取的凭证以及未启用强多因素认证的账户，导致超过 160 家组织机构的数据遭到泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.snowflake.com/en/">Snowflake AI Data Cloud</a></li>
<li><a href="https://www.snowflake.com/en/why-snowflake/what-is-data-cloud/">The AI Data Cloud Explained - Snowflake</a></li>
<li><a href="https://www.datacamp.com/blog/what-is-snowflake">What Is Snowflake? A Beginner’s Guide to the Cloud-Based Data ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#data-breach`, `#Snowflake`, `#hacking`, `#legal`

---

<a id="item-5"></a>
## [新 TONTOU CPU 攻击绕过 Spectre v2 修复，泄露 Linux 密码哈希](https://www.bleepingcomputer.com/news/security/new-tontou-cpu-attack-bypasses-spectre-v2-fixes-leaks-linux-password-hashes/) ⭐️ 9.0/10

研究人员公布了一种名为 TONTOU 的新型推测执行攻击，可绕过最新的 Spectre v2 缓解措施。概念验证漏洞利用能够从 Linux 机器上泄露密码哈希。 这表明当前 Spectre v2 防御措施仍不完善，许多 CPU 和操作系统仍面临侧信道数据窃取的风险。如果被利用，该攻击可能危及受影响 Linux 系统上的敏感凭据（如密码哈希），影响云服务商和企业。 据报道，研究人员在应用了最新 Spectre v2 缓解措施的 AMD Zen 2 主机上验证了 TONTOU 攻击，该攻击包含失效和重定向等阶段。确切的 CPU 影响范围以及是否已分配 CVE 尚未完全披露。

rss · BleepingComputer · 8月6日 18:03

**背景**: Spectre 是 2018 年发现的一类 CPU 漏洞，利用推测执行和分支预测通过侧信道泄露特权数据。Spectre v2（分支目标注入，CVE-2017-5715）针对间接分支；操作系统厂商和 CPU 制造商部署了 retpoline、IBRS 和 eIBRS 等缓解措施。然而，研究人员已多次发现绕过方法，包括 2022 年的分支历史注入（BHI/Spectre-BHB），现在又出现了 TONTOU，这表明硬件防御仍是持续的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/new-tontou-cpu-attack-bypasses-spectre-v2-fixes-leaks-linux-password-hashes/">New TONTOU CPU attack bypasses Spectre v2 fixes, leaks Linux...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spectre_(security_vulnerability)">Spectre (security vulnerability) - Wikipedia</a></li>
<li><a href="https://docs.kernel.org/admin-guide/hw-vuln/spectre.html">Spectre Side Channels — The Linux Kernel documentation</a></li>

</ul>
</details>

**标签**: `#security`, `#CPU`, `#Spectre`, `#side-channel`, `#Linux`

---

<a id="item-6"></a>
## [AMD 收购 AI 芯片初创公司 Taalas，将模型硬编码进硅片](https://www.theregister.com/systems/2026/08/06/amd-acquires-ai-chip-startup-taalas-to-boost-inference-performance-by-etching-models-into-silicon/5284344) ⭐️ 8.0/10

AMD 于 2026 年 8 月 6 日宣布收购多伦多初创公司 Taalas，该公司将 AI 模型权重直接蚀刻到硅片中用于推理。Taalas 基于台积电 6nm 工艺的 HC1 测试芯片据称能以每秒 16,960 个 token 运行 Llama 3.1 8B，比 Nvidia GPU 快 48 倍。 此次收购增强了 AMD 在快速增长的 AI 推理市场中的地位，加剧了与 Nvidia 的竞争。将模型硬编码到硅片中可以大幅降低延迟和成本，但也引发了关于新模型版本能否快速得到支持的问题。 Taalas 的技术将模型权重以掩模 ROM 形式嵌入芯片，并配以 SRAM 作为 KV 缓存，使每个加速器专用于单一模型。AMD 计划将 Taalas 的芯片与其 Instinct GPU 集成到 Helios 机架中，让 GPU 处理通用任务，而专用芯片加速推理。

hackernews · itvision · 8月6日 20:23 · [社区讨论](https://news.ycombinator.com/item?id=49201970)

**背景**: AI 推理是运行已训练模型以生成预测或响应的过程，正成为数据中心的主要工作负载。传统 GPU 是通用处理器，而针对特定模型硬编码的芯片可以实现更高的每瓦特和每美元效率。但这种芯片只能运行其蚀刻时对应的精确模型版本，因此模型的快速迭代可能使它们很快过时，多位行业观察者已经指出了这一点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/08/06/amd-buys-taalas-startup-that-hardwires-ai-models-into-its-silicon.html">AMD buys chip startup that hardwires AI models into its ...</a></li>
<li><a href="https://www.reuters.com/business/amd-deepens-ai-inference-bet-with-taalas-deal-chip-race-heats-up-2026-08-06/">AMD deepens AI inference bet with Taalas deal as chip race ...</a></li>
<li><a href="https://aiweekly.co/alerts/amd-acquires-taalas-startup-etching-ai-weights-into-silicon">AMD Acquires Taalas, Startup Etching AI Weights Into Silicon</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了兴奋与怀疑的混合情绪：有人开玩笑说黑市上会出现烧录了模型权重的芯片，也有人对 OpenAI 或 Anthropic 没有先采取此举感到意外。数人指出模型快速更新换代可能使蚀刻芯片在上市时便已过时，还有人提到 AI 模型的“峰值性能”与“可靠性能”之间常被忽视的区别。

**标签**: `#AI hardware`, `#inference`, `#AMD`, `#acquisitions`, `#silicon`

---

<a id="item-7"></a>
## [OpenAI 改进 GPT-5.6 Sol，并扩大免费用户对 GPT-5.6 Luna 的访问](https://openai.com/index/improving-gpt-5-6-sol-in-chatgpt/) ⭐️ 8.0/10

OpenAI 宣布更新 ChatGPT，提升 GPT-5.6 Sol 的准确性和一致性，同时扩大免费用户对 GPT-5.6 Luna 的访问权限。此举似乎也让更多用户能用上“思考”（Think）推理开关。 通过让免费用户用上具备推理能力的模型并改进 GPT-5.6 Sol 的体验，OpenAI 实际上正在将前沿推理能力商品化。这可能会扩大对现实世界的影响，而不仅仅局限于付费订阅者，并重塑与 Anthropic Claude 等竞争对手的格局。 GPT-5.6 是一系列按能力从低到高排列的模型，包括 Luna、Terra 和 Sol 三个变体；其中 Luna 定位为面向日常任务的快速、低成本模型，而 Sol 是能力最强的变体，在编程、科学和网络安全方面表现出色。OpenAI 表示，由于政府限制，GPT-5.6 最初于 2026 年 6 月仅向少数可信合作伙伴开放预览，直到 2026 年 7 月 9 日才全面发布。

hackernews · OpenAI Blog · 8月6日 17:02 · [社区讨论](https://news.ycombinator.com/item?id=49199357)

**背景**: GPT-5.6 是 OpenAI 最新的大语言模型系列，于 2026 年 7 月 9 日发布，是 GPT-5.x 系列的后继产品。其中 Luna 变体被视为 GPT-5.4 Mini 在经济型市场的继任者，而 Sol 则代表新一代前沿模型。ChatGPT 的默认免费模型似乎正转向 GPT-5.6 Luna——它更快、更便宜，但能力不如 Sol。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6_Sol">GPT-5.6 Sol</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>

</ul>
</details>

**社区讨论**: 评论者给出了截然不同的解读：有人称赞免费开放推理能力是改变世界的举措，也有人认为这表明 AI 商品化压力加剧，并预测行业将转向 B2B 营销和付费 API。公告还引发了关于将 ChatGPT 模型称为“AGI”是否合理的争论，一些用户则对需要手动选择推理级别感到不满。

**标签**: `#OpenAI`, `#GPT-5.6`, `#ChatGPT`, `#AI Access`, `#Free Tier`

---

<a id="item-8"></a>
## [Qwen3.8 Max 登顶 Agentic 指数，前沿 AI 竞争加剧](https://artificialanalysis.ai/?intelligence=agentic-index) ⭐️ 8.0/10

阿里巴巴的 Qwen3.8 Max 在 Artificial Analysis 的 Agentic 指数中升至第一位，超过了 Claude Opus 5 等前沿模型。这一排名变化反映了中国开源权重模型在智能体能力上的快速进步。 这标志着一款中国开源权重模型在智能体性能上领先的重大里程碑，加剧了 AI 排行榜顶端的竞争。它表明中美前沿模型的差距已经缩小，可能影响全球企业采用决策和 AI 研究重点。 Qwen3.8 Max 是一个 2.4 万亿参数的稀疏混合专家（MoE）模型，每个 token 大约激活 950 亿参数，拥有 100 万 token 的上下文窗口，支持文本、图像和视频输入。Agentic 指数衡量工具使用、规划、自主性和复杂问题解决能力；该模型于 2026 年 7 月通过 Token Plan 开始预览发布。

hackernews · apitman · 8月6日 18:44 · [社区讨论](https://news.ycombinator.com/item?id=49200652)

**背景**: Artificial Analysis Agentic 指数是一个独立基准，评估 LLM 在智能体工作流中的表现，重点关注工具使用、规划、自主性和复杂问题解决能力。它是更广泛的 Artificial Analysis 智能指数的一部分，该指数还包括基于 GPQA 等汇总基准的通用智能指数。开源权重的 Qwen3.8 系列包括旗舰规模的 Max 模型，以及预期面向本地部署的更小变体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openlm.ai/qwen3.8/">Qwen3.8 | OpenLM.ai</a></li>
<li><a href="https://aicybr.com/blog/qwen-3-8-max-complete-guide">Qwen 3.8 Max: Complete Benchmark Guide vs GPT-5.6, Claude ...</a></li>
<li><a href="https://artificialanalysis.ai/models/capabilities/agentic">Best AI for Agentic Tasks: LLM Leaderboard | Artificial Analysis</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Qwen 的进步表示兴奋，有人称赞其排查问题的能力，也有人希望更小的 3.8 模型能让本地智能体变得可行。然而，一些人质疑基准的一致性，指出在反复访问时 Qwen 和 Claude Opus 5 的榜首位置会互换，还有人认为任何将 Opus 5 排在第一的基准都缺乏公信力。

**标签**: `#AI`, `#LLM`, `#Benchmarks`, `#Qwen`, `#Agentic`

---

<a id="item-9"></a>
## [Datasette 1.0a38 修复可暴露私有表的 SQL 注入漏洞](https://simonwillison.net/2026/Aug/6/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a38 于 2026 年 8 月 6 日发布，修复了一个 SQL 注入漏洞，该漏洞可能允许拥有任何公共表访问权限的用户执行原始 SQL 查询，从而在混合公共/私有权限的数据库中获得对私有表的只读访问权。此修复也已在 Datasette 0.65.3 中提供。 此安全修复对于在同一数据库中同时提供公共表和私有表的 Datasette 实例至关重要，否则这些实例可能通过精心构造的 SQL 注入攻击泄露敏感数据。运行此类配置的管理员应立即升级，或禁用 execute-sql 权限作为临时解决方案。 该漏洞影响使用 Datasette 权限系统且数据库访问权限混合的实例，漏洞会绕过 execute-sql 权限限制。官方建议的缓解措施是，在无法立即升级的情况下，禁用受影响数据库上的 execute-sql 权限。

rss · Simon Willison · 8月6日 18:24

**背景**: Datasette 是一个用于探索和发布数据的开源工具，允许用户通过网络界面查询 SQLite 数据库。其权限系统提供表级别的访问控制，但通过 execute-sql 权限执行的原始 SQL 可能绕过这些控制，这使得 SQL 注入漏洞成为可能。Datasette 1.0 仍处于 alpha 阶段，0.65.x 是当前稳定版本线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.datasette.io/en/stable/authentication.html">Authentication and permissions - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2025/Nov/4/datasette-10a20/">A new SQL-powered permissions system in Datasette 1.0a20</a></li>

</ul>
</details>

**标签**: `#security`, `#sql-injection`, `#datasette`, `#release`, `#vulnerability`

---

<a id="item-10"></a>
## [CryptoJS 弱随机数生成器致 5 个加密钱包应用损失 570 万美元](https://thehackernews.com/2026/08/cryptojs-weak-rng-behind-57-million-in.html) ⭐️ 8.0/10

Coinspect 将 570 万美元的加密钱包资金流失追溯到 CryptoJS 库中存在 12 年的弱随机数生成器 CryptoJS.lib.WordArray.random()。该漏洞影响了五个使用它生成 BIP39 恢复短语的加密钱包应用，自 5 月下旬以来发生了两次大规模盗窃。 这说明了广泛使用的 JavaScript 库中的随机数缺陷如何直接导致加密货币盗窃，影响依赖客户端密钥生成的开发者与用户。570 万美元的实际损失凸显了在安全敏感场景中使用非加密安全随机数生成器的真实后果。 该漏洞具体是 CryptoJS.lib.WordArray.random()，它不是加密安全的随机数生成器。根据 Coinspect 的链上分析，自 5 月下旬以来的两次清扫只是被盗金额的下限，任何使用该函数生成密钥、令牌、会话标识符或随机数的应用都可能受影响。

rss · The Hacker News · 8月6日 11:49

**背景**: CryptoJS 是一个流行的 JavaScript 加密库，BIP39 恢复短语是用于生成加密货币钱包密钥的助记词种子。如果随机数生成器提供的熵不足，生成的恢复短语会变得可预测，使攻击者能够暴力破解或猜测钱包私钥。该问题在 12 年前 random()函数被加入该库时引入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/cryptojs-weak-rng-behind-57-million-in.html">CryptoJS Weak RNG Behind $5.7 Million in Drains Affects Five ...</a></li>
<li><a href="https://illbloom.org/articles/cryptojs-vulnerability/">Technical Disclosure: The CryptoJS Randomness Vulnerability</a></li>
<li><a href="https://github.com/brix/crypto-js/security/advisories/GHSA-rg76-677x-56q9">CryptoJS .lib.WordArray. random () uses a weak PRNG (Ill Bloom)</a></li>

</ul>
</details>

**标签**: `#security`, `#cryptography`, `#javascript`, `#cryptocurrency`, `#vulnerability`

---

<a id="item-11"></a>
## [AI 推荐投毒：“Ask AI”深度链接注入隐藏提示词](https://thehackernews.com/2026/08/ai-recommendation-poisoning-how-ask-ai.html) ⭐️ 8.0/10

研究人员发现了一类新的提示注入攻击，滥用商业网站上预填好的“Ask AI”深度链接，悄悄篡改大语言模型（LLM）的记忆。他们观察到，生产环境的网站在营销页和竞品对比页的“Ask AI”按钮中嵌入了隐藏的注入载荷。 这一攻击意义重大，因为载荷在点击层执行，而不是在被抓取的网页内容中执行，因此绕过了针对检索时注入的防御。由于攻击面覆盖了网络上的每一个超链接，它给基于 LLM 的助手带来广泛风险，并可能为了利益而扭曲产品推荐。 该攻击不需要恶意软件、窃取的凭据或零日漏洞；它滥用的是几乎所有主流 AI 助手中内置的标准预填深度链接功能。微软研究人员此前曾描述过用于推广目的的类似“AI 推荐投毒”技术，表明这是一个日益增长的趋势。

rss · The Hacker News · 8月6日 11:30

**背景**: 提示注入是一种针对大语言模型的安全漏洞，通过精心构造恶意提示来操纵模型行为并绕过安全过滤器。在此攻击中，用户点击“Ask AI”按钮时，预填的深度链接会把攻击者控制的文本传给助手，从而污染模型记忆或影响后续推荐。早前研究已表明，仅通过查询交互就能破坏 LLM 智能体，而 OWASP 也将提示注入列为关键的 LLM 漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/02/10/ai-recommendation-poisoning/">Manipulating AI memory for profit: The rise of AI Recommendation Poisoning | Microsoft Security Blog</a></li>
<li><a href="https://thehackernews.com/2026/02/microsoft-finds-summarize-with-ai.html">Microsoft Finds “Summarize with AI” Prompts Manipulating Chatbot Recommendations</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#AI security`, `#LLM`, `#cybersecurity`, `#adversarial attacks`

---

<a id="item-12"></a>
## [攻击者将 khunt 编译进 Oracle，将 SQL 注入升级为 Windows SYSTEM 访问](https://thehackernews.com/2026/08/attackers-compile-khunt-inside-oracle.html) ⭐️ 8.0/10

攻击者利用了面向公众的 Web 应用中的 SQL 注入漏洞入侵 Oracle 数据库，然后利用 Oracle 内置的 Java 编译器直接在数据库内部构建了 khunt 后渗透工具包。该工具包以存储的 schema 对象形式运行，全程未向磁盘写入任何可执行文件。 这一事件意义重大，因为它将经典的 SQL 注入变成了一种隐蔽的、基于内存的后渗透平台，大多数基于磁盘的防病毒工具都无法检测到。安全团队和 Oracle 管理员需要将数据库 JVM 活动及 Java 存储过程作为潜在的恶意软件执行途径加以监控。 据报告，攻击者在 Oracle 数据库引擎内部执行命令后，获得了底层 Windows 服务器的 SYSTEM 级访问权限。Huntress 将该工具包追踪为 khunt；这一技术利用了 Oracle 内置的 Java JVM，该 JVM 允许 Java 存储过程在数据库内存空间中执行。

rss · The Hacker News · 8月6日 09:19

**背景**: SQL 注入几十年来一直是 Web 应用最严重的漏洞之一，但这次攻击展示了一种新变化：攻击者不是仅仅窃取数据，而是利用 Oracle 内置的 Java 环境编译并托管一个完整的后渗透工具包。Oracle Java 存储过程是预编译的 Java 程序，存储在数据库内部，由数据库 JVM 执行，通常以类形式存放在 blob 字段中。这为攻击者提供了一个合法的、不落盘的执行环境，并可能借此转向宿主操作系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/attackers-compile-khunt-inside-oracle.html">Attackers Compile khunt Inside Oracle to Turn SQL Injection Into...</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-run-khunt-post-exploitation-toolkit-from-oracle-database/">Hackers run khunt post - exploitation toolkit from Oracle database</a></li>
<li><a href="https://www.csoonline.com/article/4206096/attackers-hid-malware-inside-oracle-database-after-sql-injection-breach.html">Attackers hid malware inside Oracle Database after SQL ...</a></li>

</ul>
</details>

**标签**: `#security`, `#SQL injection`, `#Oracle`, `#post-exploitation`, `#malware`

---

<a id="item-13"></a>
## [AWS、Google、Vercel 智能体漏洞绕过模型监管](https://thehackernews.com/2026/08/aws-google-and-vercel-patch-agent-flaws.html) ⭐️ 8.0/10

研究人员披露了 AWS、Google 和 Vercel 智能体基础设施中的安全漏洞，这些漏洞允许不受信任或伪造的指令直接到达智能体工具，而无需验证模型回合是否授权。在多种攻击路径中，模型根本未运行，因此系统提示、内容过滤器和模型级护栏从未有机会介入。 这些漏洞非常严重，因为它们绕过了 AI 智能体的基本安全层，可能导致未授权的工具调用和数据泄露。基于这些平台构建应用的组织必须重新评估其智能体安全态势，因为标准的模型级护栏无法有效防御这些攻击。 受影响的产品包括 Amazon Bedrock 智能体、Vercel AI SDK 以及 Google 的智能体基础设施。部分攻击路径在完全不执行模型的情况下触发工具，这意味着模型层的提示注入防御被完全绕过。

rss · The Hacker News · 8月6日 08:57

**背景**: AI 智能体是使用大型语言模型来解释请求并调用外部工具的系统。提示注入是一种已知的攻击技术，恶意指令被嵌入模型处理的数据中。传统防御依赖模型来过滤此类指令，但这些漏洞表明工具调用可以在没有模型监管的情况下发生。AWS 和 Vercel 已发布关于提示注入的安全指南，但这些漏洞揭示了智能体基础设施中仍存在的安全缺口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.aws.amazon.com/bedrock/latest/userguide/prompt-injection.html">Prompt injection security - Amazon Bedrock</a></li>
<li><a href="https://aws.amazon.com/blogs/machine-learning/securing-amazon-bedrock-agents-a-guide-to-safeguarding-against-indirect-prompt-injections/">Securing Amazon Bedrock Agents: A guide to safeguarding ...</a></li>
<li><a href="https://ofriperetz.dev/articles/vercel-ai-sdk-prompt-injection-vulnerability">Your Vercel AI SDK App Has a Prompt Injection Vulnerability — in...</a></li>

</ul>
</details>

**标签**: `#security`, `#AI agents`, `#cloud`, `#vulnerability`, `#LLM`

---

<a id="item-14"></a>
## [Zbtlink 路由器出厂预装后门，可开启未授权 Root Shell](https://thehackernews.com/2026/08/chinese-made-zbtlink-routers-ship-with.html) ⭐️ 8.0/10

VulnCheck 的安全研究人员披露了一个名为 ENDLESSDOORS 的出厂预装后门，该后门嵌入在至少 20 款 Zbtlink 路由器型号中。该后门影响 Zbtlink 过去两年多发布的所有 21 个固件镜像，并会自动尝试与中国服务器进行通信。 这种供应链后门使远程攻击者无需身份验证即可获得受影响路由器的 Root 访问权限，从而可能进行监视、网络横向渗透和组建僵尸网络。这凸显了消费级网络设备固件被植入恶意代码的风险日益增大，尤其对使用这些中国制造设备的用户影响严重。 该植入物会在开机时自动启动，并尝试以每 35 秒一次的频率与命令控制服务器联系以接收远程命令。Zbtlink 目前可用的所有 21 个固件镜像均受影响，时间跨度超过两年。

rss · The Hacker News · 8月6日 08:05

**背景**: 后门是一种绕过正常身份验证、暗中获取系统未授权访问权限的隐藏机制。未认证的 Root Shell 意味着攻击者无需任何凭证即可获得操作系统最高级别的控制权。命令与控制（C2）信标是受感染设备定期向攻击者服务器发送通信以获取指令的行为。此类供应链攻击通常发生在制造或固件开发过程中被植入恶意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=n6bPTTp3gng">CVE-2026-24061 PoC: Unauthenticated Remote Root Shell ... Root via Telnet: Active Exploitation of CVE-2026-24061 (GNU ... CVE-2025-55182: React2Shell - Unauthenticated RCE in React ... Chinese-Made Zbtlink Routers Ship With Backdoor That Opens ... GitHub - sh4den/CVE-2026-24061: Proof of Concept: CVE-2026 ... GitHub - franckferman/CVE_2026_24061: GNU InetUtils telnetd ...</a></li>
<li><a href="https://www.extrahop.com/resources/attacks/c-c-beaconing">What is C2 Beaconing? Definition & Prevention - ExtraHop</a></li>
<li><a href="https://attack.mitre.org/tactics/TA0011/">Command and Control, Tactic TA0011 - MITRE ATT&CK®</a></li>

</ul>
</details>

**标签**: `#security`, `#backdoor`, `#supply chain`, `#routers`, `#firmware`

---

<a id="item-15"></a>
## [往返一致性让双向扩散模型自测推算误差](https://www.reddit.com/r/MachineLearning/comments/1vh2gn1/roundtrip_consistency_bidirectional_diffusion/) ⭐️ 8.0/10

研究者提出一个双向条件潜在扩散模型，通过方向标志控制系统在时间上前向或后向演化。他们引入“往返一致性”——即先向前再向后滚动后与初始状态的偏差——作为无需测量、自监督的测试时滚动误差代理。 这为生成模型在部署时提供了一种实用的置信度信号，无需集成、留出数据或控制方程，对视频生成和数字孪生等长期预测任务很有价值。研究还表明一个双向模型可以胜过两个单向专用模型，从而可能降低训练成本。 在 LE-PDE-UQ 湍流 Navier-Stokes 基准测试上，单个双向模型以十分之一的训练成本达到十个模型集成的准确率的 1.3 倍以内，并取得了最好的免训练像素级校准效果。代码、数据生成脚本和分析均已开源在 GitHub，论文也有项目主页。

reddit · r/MachineLearning · /u/Clean-Hovercraft5825 · 8月6日 12:10

**背景**: 扩散模型通过迭代去噪随机噪声来生成样本，并常以自回归方式把预测结果作为输入来实现预测。由于部署时没有真实值，这种长时滚动会不断累积误差。往返一致性利用了所学动力学的可逆性：如果模型既能向前也能向后演化，那么先前进再返回应回到起点，因此偏差可作为自监督误差信号。该工作在 CELEBV-HQ 视频和代表数字孪生场景的湍流等离子体场上验证了该方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2608.00675v1">Round-Trip Consistency: Bidirectional Diffusion Models Can ...</a></li>
<li><a href="https://arxiv.org/abs/2608.00675">[2608.00675] Round-Trip Consistency: Bidirectional Diffusion ...</a></li>
<li><a href="https://github.com/alexscheinker/round-trip-consistency">GitHub - alexscheinker/round-trip-consistency: Bidirectional ...</a></li>

</ul>
</details>

**标签**: `#diffusion models`, `#self-supervised learning`, `#generative modeling`, `#digital twins`, `#uncertainty estimation`

---

<a id="item-16"></a>
## [用《马力欧卡丁车》角色属性解释帕累托最优与权衡](https://www.mayerowitz.io/blog/mario-meets-pareto) ⭐️ 7.0/10

文章《Mario Meets Pareto》利用《马力欧卡丁车》的角色属性——特别是速度与加速之间的权衡——来说明帕累托最优与帕累托前沿。它将每个角色映射到非支配选择的边界上，表明没有任何角色能同时最大化两项属性。 这个通俗易懂的示例能帮助开发者和决策者理解多目标优化，即改进一个指标往往会损害另一个指标。文章获得的高度关注（843 分、147 条评论）表明它引起了技术受众（包括 Hacker News 读者）的共鸣。 《马力欧卡丁车》中的帕累托前沿包括像库巴（Bowser）和大金刚（Donkey Kong）这样位于边界上的角色，它们优先考虑速度而非加速；均衡型角色则位于边界内部。这映射到现实中的产品设计，权衡决定了高效选项的集合。

hackernews · theanonymousone · 8月6日 11:24 · [社区讨论](https://news.ycombinator.com/item?id=49195231)

**背景**: 帕累托效率（或称帕累托最优）是一个经济学概念，描述的是无法在不使任何他人变差的情况下让某人变得更好的状态。在多目标优化中，帕累托前沿（Pareto frontier）是所有那些没有任何解在所有目标上都优于另一个解的解的集合，而集合之外的每个解都被集合内至少一个解所支配。这一概念广泛用于工程和决策中，以将选择范围缩小到高效的权衡方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pareto_optimality">Pareto optimality</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pareto_frontier">Pareto frontier</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pareto_efficiency">Pareto efficiency - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对这个概念作了进一步延伸：有人指出，开发者经常在团队并未真正处于帕累托前沿时宣称“想要 X 就必须放弃 Y”，这是一种错误的约束。另一位评论者描述了在《魔兽世界》怀旧服中使用帕累托前沿剪枝来优化装备搭配；而一位速通玩家指出，顶级《马力欧卡丁车》速通会偏好库巴等边界角色。还有一位父亲幽默地补充说，许多家长优化的是“既能保持竞争力，又输给小孩”的车手选择。

**标签**: `#pareto-frontier`, `#optimization`, `#algorithms`, `#trade-offs`, `#mario-kart`

---

<a id="item-17"></a>
## [Herdr 加入 Y Combinator，运行时保持开源](https://herdr.dev/blog/herdr-is-joining-y-combinator/) ⭐️ 7.0/10

面向多智能体编码的开源终端多路复用器 Herdr 宣布加入 Y Combinator，作为其种子前融资的一部分。该公司强调其运行时将继续保持开源。 这一里程碑表明，投资者对多智能体编码领域的开发者工具兴趣日益浓厚，这是一个拥挤但新兴的市场。这也说明开源工具在获得风险投资的同时，仍能保持其开放核心模式。 据创始人称，Herdr 最近将其许可证从 AGPL 改为 Apache 2.0，以便任何人都可以无后顾之忧地自由使用该工具。该公告发布之际，涌现了一批 YC 支持的竞争对手，例如 Superset、cmux 和 Emdash。

hackernews · collinmanderson · 8月6日 19:14 · [社区讨论](https://news.ycombinator.com/item?id=49201003)

**背景**: 终端多路复用器允许用户在一个窗口内运行多个终端会话，并可分离或重新附加会话，这是开发者长期以来使用的工具。多智能体编码是一种较新的工作流程，多个 AI 智能体并行处理不同的编码任务，而开发者在旁编排协调。Herdr 正处于这两大趋势的交汇点，为 AI 编码智能体提供了基于终端的编排层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Terminal_multiplexer">Terminal multiplexer - Wikipedia</a></li>
<li><a href="https://addyosmani.com/blog/code-agent-orchestra/">AddyOsmani.com - The Code Agent Orchestra - what makes multi-agent coding work</a></li>
<li><a href="https://www.howtogeek.com/terminal-multiplexers-explained/">Terminal Multiplexers Explained, and Why You'd Use One</a></li>

</ul>
</details>

**社区讨论**: 评论者们对创始人 Can 获得种子前融资表示祝贺，其中一位表示 Herdr 已成为其在终端中编排智能体的默认方式。其他人则对拥挤的市场表示担忧，列出了竞争的 YC 初创公司，并质疑为何将许可证从 AGPL 改为 Apache。还有讨论认为，风投融资可能威胁到该工具的开源性质。

**标签**: `#Y Combinator`, `#open source`, `#developer tools`, `#AI agents`, `#startup funding`

---

<a id="item-18"></a>
## [品味成为 AI 时代软件工程仅存的人类特质](https://notashelf.dev/posts/taste-is-all-thats-left) ⭐️ 7.0/10

notashelf 发表的《Taste Is All That's Left》一文认为，随着 AI 将常规编码自动化，品味与判断力成为人类仅存的核心素质。这篇文章在 Hacker News 上获得了 7.0/10 的高分，并引发资深开发者的热烈讨论。 这一观点将 AI 对软件工程的影响从“执行能力”重新定义为“决策与取舍能力”，可能改变工程师与团队对自身价值的评估方式。它印证了资深开发者的担忧，并提醒业界应将关注点从代码如何编写转向代码背后的判断。 文章区分了技术技能与品味，指出品味主导自动化无法替代的审美与选择。评论区有人提到，LLM 虽然能解决眼前问题，但在数月、多人的规模上却难以产出有价值的东西，其写作质量也往往缺乏“信号”。

hackernews · tsak · 8月6日 17:01 · [社区讨论](https://news.ycombinator.com/item?id=49199346)

**背景**: 在软件工程中，“品味”指超越框架知识和编码效率的设计判断力，它决定一个系统是否简洁、优雅、易于维护。技术品味不同于技术能力：技术强的人可能品味差，技术弱的人也可能品味好。随着 AI 编程工具从生成代码演进到生成完整应用，工程师的核心价值正从“写代码”转向“做选择”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.seangoedecke.com/taste/">What is "good taste " in software engineering ?</a></li>
<li><a href="https://medium.com/data-science-collective/taste-still-matters-why-software-engineers-need-more-than-ai-skills-in-2025-d227add52d36">Taste Still Matters: Why Software Engineers Need More... | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论总体高度共鸣，资深开发者 mdwelsh 表示自己通过大量错误才磨练出品味，并质疑仅靠 AI 代理搭建的演示是否真的“内里优秀”。hellojomp 引用苏珊·桑塔格《坎普札记》中的话，指出品味支配一切自由而非机械的人类反应；boron1006 则对 LLM 的写作质量感到沮丧，认为其长期产出几乎没有任何“信号”。也有观点反问：只要软件能运行，谁还在乎它是怎么建造的。

**标签**: `#AI`, `#software-engineering`, `#taste`, `#judgment`, `#programming`

---

<a id="item-19"></a>
## [FCC 取消广播电视所有权全国上限](https://www.nbcnews.com/business/media/federal-communications-commission-scraps-limit-broadcast-tv-ownership-rcna587641) ⭐️ 7.0/10

FCC 已投票取消对广播电视电台所有权的全国性限制，包括 39%家庭覆盖率上限。此举推翻了一项长期存在的所有权限制，为大型广播集团收购更多电视台打开了大门。 这一监管变化可能加速媒体整合，使少数大公司控制更多地方电视台，并削弱地方新闻的多样性。它还重新引发了关于 FCC 是否有法定权力改变这一由国会设定的上限的法律争议。 批评者指出，国会制定的法规明确禁止 FCC 改变这一上限，而最高法院近期削弱“Chevron deference”（谢弗林遵从原则）可能动摇该机构的规则制定权。此次取消全国上限似乎并未触及同一市场内的地方所有权上限。

hackernews · pseudolus · 8月6日 18:22 · [社区讨论](https://news.ycombinator.com/item?id=49200390)

**背景**: FCC 的广播所有权规则长期以来限制单一实体可拥有的电视台数量以及这些电视台能够覆盖的美国家庭数量，目的是促进竞争、本地化和观点多样性。媒体整合一直是一个令人担忧的问题，因为所有权集中可能减少新闻和娱乐领域中独立声音的数量。在流媒体时代，有人认为广播电视的相关性正在下降，也有人认为所有权规则仍然重要，因为广播公司使用公共频谱并继续在本地新闻中扮演重要角色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nationalinterest.org/blog/techland/why-the-fccs-broadcast-ownership-rules-still-matter-in-a-new-tech-driven-media-era">Why the FCC ’s Broadcast Ownership Rules ... - The National Interest</a></li>
<li><a href="https://en.wikipedia.org/wiki/Media_consolidation">Media consolidation</a></li>

</ul>
</details>

**社区讨论**: 评论者大多对这一决定持怀疑态度。有人指出，前众议院多数党领袖 Tom DeLay 撰文表示，此举违反了他参与制定的法规；有人质疑在最高法院削弱 Chevron deference 之后 FCC 是否有权这样做；还有人认为广播电视已基本无关紧要，并担忧频谱使用问题。另有人指出，同一市场内的所有权上限可能仍然保留。

**标签**: `#FCC`, `#media ownership`, `#regulation`, `#broadcast TV`

---

<a id="item-20"></a>
## [Datasette 0.65.3 移植 SQL 注入安全修复](https://simonwillison.net/2026/Aug/6/datasette-2/#atom-everything) ⭐️ 7.0/10

Datasette 0.65.3 backports a SQL injection security fix from 1.0a38 to the 0.65.x series.

rss · Simon Willison · 8月6日 18:22

**标签**: `#datasette`, `#security`, `#sql-injection`, `#release`

---