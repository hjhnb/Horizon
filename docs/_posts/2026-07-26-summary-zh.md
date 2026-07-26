---
layout: default
title: "Horizon Summary: 2026-07-26 (ZH)"
date: 2026-07-26
lang: zh
---

> 从 32 条内容中筛选出 20 条重要资讯。

---

1. [sglang v0.5.16：引入 DSpark 与 975B 参数 Inkling 模型支持](#item-1)
2. [vLLM v0.26.0 发布，支持 Inkling 模型并进行重大优化](#item-2)
3. [Fastjson 1.x 未修补的远程代码执行漏洞正遭积极攻击](#item-3)
4. [开放权重 AI 的 Kubernetes 时刻](#item-4)
5. [Android 可能限制设备端 ADB 访问](#item-5)
6. [大语言模型引发数学家的存在危机](#item-6)
7. [Ruff v0.16.0：默认 lint 规则从 59 条增加到 413 条](#item-7)
8. [Claude Opus 5 展现强提示注入抵抗力](#item-8)
9. [恶意广告活动利用 Bun 运行库在浏览器中组装恶意软件](#item-9)
10. [Cl0p 关联方利用 PTC Windchill 和 FlexPLM 远程代码执行漏洞](#item-10)
11. [Claude 5 新上下文工程规则](#item-11)
12. [针对 Flock 监控摄像头的公民抵抗运动](#item-12)
13. [Fedora 45 发布流程详解](#item-13)
14. [GitLab RCE PoC 暴露未打补丁的服务器](#item-14)
15. [保险钓鱼攻击已演变为实时账户劫持](#item-15)
16. [DevMan 勒索软件即服务平台集中化载荷构建与支付](#item-16)
17. [Steam 论坛 ClickFix 攻击传播 XMRig 加密矿工](#item-17)
18. [恶意网站通过 JavaScript 在浏览器内存中组装恶意软件](#item-18)
19. [ShinyHunters 数据泄露助长 2000 美元性勒索诈骗](#item-19)
20. [OpenAI 确认 ChatGPT 全球宕机](#item-20)

---

<a id="item-1"></a>
## [sglang v0.5.16：引入 DSpark 与 975B 参数 Inkling 模型支持](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 9.0/10

sglang v0.5.16 引入了新型投机解码算法 DSpark，在 DeepSeek-V4-Pro 上达到 383.7 tok/s，并新增对 975B 参数多模态 MoE 模型 Inkling 的支持，输入吞吐量高达 71.7k tok/s。 DSpark 通过自适应调整验证窗口大小，在投机解码领域达到新标杆，显著提升大语言模型的推理吞吐量。对 Inkling 的支持使得高效部署最大规模的开源权重多模态 MoE 模型成为可能，推动了可扩展 AI 推理的前沿。 DSpark 采用置信度驱动的块草稿，在 TP8 B300 上达到接受长度约 5、383.7 tok/s 的速率；Inkling 是一个 975B 参数、41B 活跃参数的多模态模型，支持文本、图像和音频，上下文长度 1M token。此次发布还包括默认对 SWA/Mamba 的 UnifiedRadixTree、GLM-5.2 的 DSA 缓存层拆分，以及移除 QServe 和 FBGEMM FP8 后端。

github · Qiaolin-Yu · 7月25日 00:13

**背景**: 投机解码通过使用小型草稿模型生成候选 token，再由目标模型并行验证，从而加速 LLM 推理。混合专家（MoE）模型每个 token 只激活部分参数，使得总参数量更大但计算量可控。sglang 是一个针对 LLM 服务优化的开源推理引擎，支持多种模型架构和硬件后端。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.05147">DSpark: Confidence-Scheduled Speculative Decoding with Semi ...</a></li>
<li><a href="https://models.dev/models/thinkingmachines/inkling/">Inkling pricing, providers, and specs | Models .dev</a></li>
<li><a href="https://www.techtimes.com/articles/319236/20260628/deepseek-releases-dspark-speculative-decoding-makes-v4-85-percent-faster.htm">DeepSeek Releases DSpark: Speculative Decoding Makes V4 Up to 85 ...</a></li>

</ul>
</details>

**标签**: `#speculative decoding`, `#inference optimization`, `#large language models`, `#sglang`, `#MoE`

---

<a id="item-2"></a>
## [vLLM v0.26.0 发布，支持 Inkling 模型并进行重大优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 版本发布，包含来自 212 位贡献者的 411 次提交，全面支持新的 Inkling 模型家族，显著提升 DeepSeek-V4 性能，为生成模型引入 fp32 lm_head，提供灵活的注意力后端，并成熟了 KV 卸载与分层次要存储功能。 这一版本标志着 LLM 推理服务的重大进步，增加了前沿模型支持和性能优化，惠及从小规模微调到大规模生产系统的多种部署场景。 值得注意的技术细节包括：Inkling 的分段 CUDA 图支持、为 DeepSeek-V4 提供 2.94% 端到端 TPOT 提升的专用路由内核、通过 head_dtype 实现的 fp32 lm_head 并带有 ROCm 快速路径、每个 KV 缓存组可选注意力后端，以及支持多模态视频和音频的 Rust 前端。

github · khluu · 7月25日 10:38

**背景**: vLLM 是一个开源的高吞吐量 LLM 服务引擎，利用 PagedAttention 高效管理 KV 缓存内存。Inkling 模型家族是 Thinking Machines Lab 发布的一款广泛的多模态基础模型，采用 Apache 2.0 许可证。FlashAttention-4 (FA4) 是针对 Hopper 和 Blackwell GPU 的内核协同设计，通过多阶段流水线提升注意力性能。NVFP4 是一种用于 Blackwell GPU 的 4 位浮点量化方法，属于 NVIDIA ModelOpt 库的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://arxiv.org/abs/2603.05451">[2603.05451] FlashAttention-4: Algorithm and Kernel ... FlexAttention + FlashAttention-4: Fast and Flexible – PyTorch Gemma 4 Update: FA4, Tool Calling, Vision (July 2026 ... We reverse-engineered Flash Attention 4 - modal.com FlashAttention-4: Algorithm and Kernel Pipelining Co-Design ... Lecture 09 - Hopper FA3 FA4.md - GitHub</a></li>
<li><a href="https://build.nvidia.com/spark/nvfp4-quantization">NVFP4 Quantization | DGX Spark</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#release`, `#performance`, `#model serving`

---

<a id="item-3"></a>
## [Fastjson 1.x 未修补的远程代码执行漏洞正遭积极攻击](https://thehackernews.com/2026/07/fastjson-1x-rce-vulnerability-targeted.html) ⭐️ 9.0/10

阿里巴巴 Fastjson 1.x 库中存在一个关键的未修补远程代码执行漏洞（CVE-2026-16723，CVSS 9.0），目前正被积极用于针对 Spring Boot 应用的攻击。 该漏洞允许攻击者在受影响的系统上无需认证即可执行任意代码，对大量依赖 Fastjson 的 Java 应用（尤其是 Spring Boot 服务）构成严重威胁。 该漏洞影响 Fastjson 1.2.68 至 1.2.83 版本，通过恶意 JSON 请求绕过 AutoType 限制，以 Java 进程权限实现远程代码执行。

rss · The Hacker News · 7月25日 12:52

**背景**: Fastjson 是流行的 Java JSON 解析与序列化库，广泛用于企业应用。因其 AutoType 功能允许动态类加载，历史上多次出现反序列化漏洞。此漏洞尚无补丁，用户只能依赖临时缓解措施或升级至 Fastjson 2.x。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2026-16723">NVD - CVE - 2026 - 16723</a></li>
<li><a href="https://github.com/alibaba/fastjson">GitHub - alibaba/fastjson: FASTJSON 2.0.x has been released ...</a></li>
<li><a href="https://securityonline.info/cve-watchtower/?cve_detail=CVE-2026-16723-admin&source=ADMIN">CVE Watchtower • Daily CyberSecurity</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Fastjson`, `#RCE`, `#Java`

---

<a id="item-4"></a>
## [开放权重 AI 的 Kubernetes 时刻](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

Tobi Knaup 的一篇文章认为，开放权重 AI 模型正变得像 Kubernetes 对于云计算那样基础，引发了社区关于模型治理、定价和协作开发的讨论。 这一类比凸显了开放权重模型在推动 AI 民主化和创新方面日益重要的作用，正如 Kubernetes 标准化了容器编排一样，这些讨论反映了 AI 行业在监管、定价和开放协作方面的真实矛盾。 开放权重模型仅发布训练后的权重，而不包含训练数据或代码，这使得按来源禁止模型变得困难；社区评论指出，专有模型的定价波动使开放权重模型成为成本合理性的基准。

hackernews · tknaup · 7月25日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: 开放权重 AI 模型是神经网络的训练参数（权重）被公开发布的模型，任何人都可以下载并运行它们，但与开源 AI 不同，它们通常不包含训练代码或数据集。Kubernetes 是一个开源容器编排平台，已成为部署和管理容器化应用的事实标准，展示了开放基础设施如何成为基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**社区讨论**: 评论者就禁止中国模型的可行性展开辩论，有人指出权重只是数字，无法追溯来源。另一位批评专有模型定价不透明，称赞开放权重模型提供了成本基准。还有一位设想像 Linux 那样的协作模型开发，指出如果制作模型成本高昂，公司可能会共享并贡献给一个开放模型。

**标签**: `#open-weight AI`, `#Kubernetes`, `#model governance`, `#AI industry`, `#open source`

---

<a id="item-5"></a>
## [Android 可能限制设备端 ADB 访问](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

一项新提案建议限制设备端 Android 调试桥 (ADB) 访问，可能限制通过 TCP/IP 从设备本身进行连接的能力。 此项更改可能严重影响依赖无线 ADB 进行调试的 Android 开发者，同时旨在减少恶意行为者的攻击面。 该限制可能要求身份验证或限制连接到特定 IP 地址或接口，类似于现有的 USB ADB 控制。

hackernews · shscs911 · 7月25日 06:57 · [社区讨论](https://news.ycombinator.com/item?id=49045159)

**背景**: Android 调试桥 (ADB) 是一个命令行工具，允许开发者与 Android 设备进行通信以进行调试和安装。它可以通过 USB 或 TCP/IP（无线）运行。目前，需要启用开发者选项和“USB 调试”，但无线 ADB 可以在没有额外设备限制的情况下启用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge - Wikipedia</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge ( adb ) | Android Studio | Android Developers</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人认为攻击向量不现实，因为需要启用开发者模式和远程 ADB；另一些人则担心这是进一步锁定平台的步骤。少数用户建议限制到 VPN 等受信任网络作为平衡解决方案。

**标签**: `#Android`, `#ADB`, `#developer tools`, `#security`, `#mobile development`

---

<a id="item-6"></a>
## [大语言模型引发数学家的存在危机](https://kirwinhampshire.substack.com/p/the-dark-night-of-mathematics) ⭐️ 8.0/10

Kirwin Hampshire 的一篇文章探讨了大语言模型如何让数学家质疑自身角色，建议从直接证明定理转向策展 AI 生成的数学洞见。 这预示着知识工作者更广泛的存在危机，因为人工智能威胁到数学等领域人类技艺的内在价值，促使人们从根本上重新评估工作和创造力。 文章认为，发现数学的情感满足感与其难度和社交属性相关，而大语言模型正在削弱这一点。文章提出，数学家可能演变为机器生成结果的策展人而非创作者。

hackernews · rmdmphilosopher · 7月25日 15:54 · [社区讨论](https://news.ycombinator.com/item?id=49048681)

**背景**: 大语言模型（如 GPT-4）已被应用于自动定理证明，在 Lean 和 Coq 等系统中辅助生成形式化证明。尽管显示出潜力，但目前在复杂形式化证明上仍显吃力，常需人类引导。这一技术挑战了数学家作为新定理唯一发现者的传统角色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aclanthology.org/2024.nlp4science-1.18/">Benchmarking Automated Theorem Proving with Large Language Models</a></li>
<li><a href="https://arxiv.org/abs/2409.14274">[2409.14274] Proof Automation with Large Language Models</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了不同反应：有人欢迎这一转变，认为这解放了他们去探索更多问题；也有人哀叹学习和构造证明的快乐丧失。一个共同主题是所有知识工作者都将面临类似的认同危机，前进之路在于改变与工作的关系并专注于更高层次的策展。

**标签**: `#mathematics`, `#AI impact`, `#knowledge work`, `#LLMs`, `#philosophy`

---

<a id="item-7"></a>
## [Ruff v0.16.0：默认 lint 规则从 59 条增加到 413 条](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Astral 于 7 月 23 日发布了 Ruff v0.16.0，将默认 lint 规则从 59 条大幅增加到 413 条，规则总数达到 968 条，导致许多使用未固定 Ruff 依赖的项目 CI 失败。 此次发布大幅收紧了默认 Python 代码检查规则，无需任何配置即可捕获更多严重问题（如语法错误和运行时错误），但同时会破坏现有 CI 流水线，迫使开发者更新代码或固定 Ruff 版本。 自 v0.1.0 以来，规则数从 708 条增加到 968 条，新默认值启用了 413 条规则。Simon Willison 的项目中有一个报告了 1618 个错误，其中 1538 个可自动修复，剩余问题需要手动审查，例如无时区的 datetime 和盲捕获异常。

rss · Simon Willison · 7月25日 22:44

**背景**: Ruff 是一个用 Rust 编写的极速 Python 代码检查器和格式化工具，由 Astral 开发（最近被 OpenAI 收购）。与 Flake8 或 Pylint 等传统工具不同，Ruff 将覆盖样式、正确性和安全性的数百条规则打包进单一二进制文件。默认规则是指无需任何配置文件即可启用的规则；从 59 条增加到 413 条意味着许多项目将看到新的警告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/linter/">The Ruff Linter | Ruff</a></li>
<li><a href="https://pypi.org/project/ruff/">An extremely fast Python linter and code formatter, written in Rust.</a></li>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ ruff : An extremely fast Python linter and code...</a></li>

</ul>
</details>

**标签**: `#Python`, `#Ruff`, `#linting`, `#tooling`

---

<a id="item-8"></a>
## [Claude Opus 5 展现强提示注入抵抗力](https://simonwillison.net/2026/Jul/25/boris-cherny/#atom-everything) ⭐️ 8.0/10

Boris Cherny 宣布，根据系统卡中详细说明的评估和红队测试结果，Claude Opus 5 是 Anthropic 迄今为止最难被提示注入的模型。 这标志着 AI 安全的重大进步，因为提示注入是大语言模型的一个关键漏洞；更强的抵抗力使 Claude Opus 5 在需要严格输入完整性的实际应用中更加安全。 该声明得到了 Claude Opus 5 系统卡第 73 页的支持，该卡显示了在提示注入评估和红队测试中的强劲表现。

rss · Simon Willison · 7月25日 00:42

**背景**: 提示注入攻击利用语言模型无法区分可信指令和不可信用户输入的弱点，可能导致意外行为。红队测试是一种系统性的对抗性测试方法，用于在部署前主动识别此类漏洞。Claude Opus 5 是 Anthropic 的最新旗舰模型，其对提示注入的抵抗力是一项关键的安全改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>
<li><a href="https://www.weforum.org/stories/2025/06/red-teaming-and-safer-ai/">What is 'red teaming' and how can it lead to safer AI? | World Economic Forum</a></li>

</ul>
</details>

**标签**: `#prompt-injection`, `#anthropic`, `#claude`, `#generative-ai`, `#ai`

---

<a id="item-9"></a>
## [恶意广告活动利用 Bun 运行库在浏览器中组装恶意软件](https://thehackernews.com/2026/07/malvertising-sends-malware-in-pieces.html) ⭐️ 8.0/10

名为 SourTrade 的恶意广告活动自 2024 年底以来一直活跃，它利用合法的 Bun 运行库将 Windows 可执行文件分割成碎片，通过在线广告分发，然后在受害者的浏览器中重新组装恶意软件。 这种新技术避免了传统的基于文件的检测，因为从未从单个 URL 提供完整的恶意文件，而且组装过程发生在一个可能被列入白名单的 JavaScript 运行库中，给安全防御带来了重大挑战。 该活动通过冒充 TradingView、Solana 和 Luno 等平台，专门针对零售交易者，并于 2026 年 7 月 23 日由安全公司 Confiant 详细披露。

rss · The Hacker News · 7月25日 18:48

**背景**: Bun 是一个现代的 JavaScript 运行库，以其速度和打包能力著称，这里被用作在浏览器中执行代码的合法平台。恶意广告是一种将恶意代码隐藏在在线广告中的技术，通常通过广告网络传播，以感染查看或点击广告的用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Malvertising">Malvertising - Wikipedia</a></li>

</ul>
</details>

**标签**: `#malvertising`, `#malware`, `#bun runtime`, `#security`, `#browser exploit`

---

<a id="item-10"></a>
## [Cl0p 关联方利用 PTC Windchill 和 FlexPLM 远程代码执行漏洞](https://thehackernews.com/2026/07/cl0p-affiliates-target-internet-exposed.html) ⭐️ 8.0/10

Cl0p 勒索软件关联方正在积极利用暴露于互联网的 PTC Windchill 和 FlexPLM 部署中的一个未认证远程代码执行漏洞（CVE-2026-12569），通过部署 JSP 网页木马并窃取敏感数据进行勒索。 此活动针对制造业和产品生命周期管理中使用的关键企业系统，可能导致知识产权被盗和运营中断，并凸显了 Cl0p 这一多产勒索软件团伙的持续威胁。 攻击链结合了 FlexPLM 的 WSDL 端点中的预认证信息泄露和 Windchill 登录 Servlet 中的服务器端缺陷，从而实现未认证的远程代码执行。PTC 已为所有受支持版本发布补丁，CISA 也发布了通告（ICSA-26-085-03）。

rss · The Hacker News · 7月25日 10:14

**背景**: PTC Windchill 是一款产品生命周期管理（PLM）软件，大型制造商用它来管理产品数据和流程。FlexPLM 是其面向零售业的变体。Cl0p（也称为 FIN11、Lace Tempest）是一个臭名昭著的勒索软件团伙，以利用企业软件漏洞而闻名。此漏洞（CVE-2026-12569）允许未认证攻击者在受影响的服务器上执行任意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ptc.com/en/about/trust-center/advisory-center/active-advisories/windchill-flexplm-rce-vulnerability">Customer & Partner Updates: Remote Code Execution Vulnerability in PTC’s Windchill and FlexPLM Solutions | June 2026 | PTC</a></li>
<li><a href="https://www.cisa.gov/news-events/ics-advisories/icsa-26-085-03">PTC Windchill Product Lifecycle Management | CISA</a></li>
<li><a href="https://cybersecuritynews.com/cl0p-hackers-exploit-windchill/">Cl0p Hackers Exploit Windchill Servers to Steal Companies' Secret ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#ransomware`, `#CVE`, `#PTC`, `#vulnerability`

---

<a id="item-11"></a>
## [Claude 5 新上下文工程规则](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 7.0/10

Anthropic 宣布了针对 Claude 5 代模型的新上下文工程规则，将焦点从提示工程转向管理更广泛的上下文配置以生成期望的模型行为。 这一变化标志着开发者与大型语言模型交互方式的重大演进，有望提高可靠性和任务性能。然而，社区对供应商锁定及 Claude 5 错误率增加的担忧可能限制其采用。 新规则强调上下文工程而非传统提示工程，侧重于在模型的上下文窗口内组织信息。一些用户报告称，Claude 5 比之前版本错误更多且消耗更多 token。

hackernews · mellosouls · 7月25日 20:42 · [社区讨论](https://news.ycombinator.com/item?id=49051361)

**背景**: 上下文工程是一种较新的实践，涉及管理输入 AI 模型上下文窗口的信息，而非仅仅编写单个提示。它旨在创建从多个来源收集和组织相关细节的系统，以引导模型行为。随着模型能力增强和上下文窗口扩大，这种方法日益受到重视。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents">Effective context engineering for AI agents \ Anthropic</a></li>
<li><a href="https://www.datacamp.com/blog/context-engineering">Context Engineering: A Guide With Examples | DataCamp</a></li>
<li><a href="https://cloud.google.com/discover/ai-context-engineering">What Is AI context engineering? | Google Cloud</a></li>

</ul>
</details>

**社区讨论**: 社区反馈褒贬不一：一些用户担心新规则是 Anthropic 工具的锁定策略，而另一些用户则报告 Claude 5 错误率和 token 消耗增加。还有人质疑过度依赖 Claude 的自动记忆功能，该功能可能产生不合逻辑的跳跃。

**标签**: `#Claude 5`, `#context engineering`, `#AI models`, `#Anthropic`, `#prompt engineering`

---

<a id="item-12"></a>
## [针对 Flock 监控摄像头的公民抵抗运动](https://www.theguardian.com/us-news/ng-interactive/2026/jul/25/flock-surveillance-cameras) ⭐️ 7.0/10

公民们正在物理破坏 Flock Safety 公司的太阳能监控摄像头，常使用如带纸板的泳池捞网等简易工具，这反映了对大规模监控的草根抵抗。 这一运动表明公众对监控技术日益不信任，尤其是在执法滥用被曝光后，可能影响美国关于隐私与安全的辩论。 Flock 摄像头是太阳能供电、安装在电线杆上的，常用于执法部门；然而，警察滥用（如追踪前伴侣）加剧了抵制。

hackernews · bookofjoe · 7月25日 19:02 · [社区讨论](https://news.ycombinator.com/item?id=49050538)

**背景**: Flock Safety 是一家向警方和社区销售 AI 摄像头网络的公司，声称有助于减少犯罪。但隐私倡导者警告大规模监控和缺乏监督。类似警察局长用 Flock 跟踪前妻的事件削弱了信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnet.com/home/security/when-flock-comes-to-town-why-cities-are-axing-the-controversial-surveillance-technology/">When Flock Comes to Your Town: I Asked Experts What to Do... - CNET</a></li>
<li><a href="https://trafficvision.live/blog/flock-cameras">Flock Cameras : What They Are & Can You Watch... | TrafficVision.Live</a></li>

</ul>
</details>

**社区讨论**: 评论者对这种公民行动表示强烈支持，引用政府的虚伪和反对监控的必要性。一些人提出了幽默的应对措施，另一些人引用了关于自由的历史名言。

**标签**: `#surveillance`, `#privacy`, `#activism`, `#ethics`

---

<a id="item-13"></a>
## [Fedora 45 发布流程详解](https://supakeen.com/weblog/the-fedora-45-sausage-factory/) ⭐️ 7.0/10

supakeen 发布了一篇详细博文，以 Fedora 45 为例，从头到尾介绍了 Fedora 发布构建流程，从源代码到 ISO 镜像生成。 这份文档对于故障排查和新贡献者入门非常宝贵，它揭示了 Fedora 的发布工程流水线，帮助用户理解构建系统变化如何影响最终发行版。 该博文用“香肠工厂”比喻构建流水线，评论指出它帮助追踪了 Fedora 版本间的文件权限变化。同时也为希望参与 Fedora 发布工程的贡献者提供了起点。

hackernews · 6581 · 7月25日 11:04 · [社区讨论](https://news.ycombinator.com/item?id=49046525)

**背景**: Fedora 是一个快速迭代的 Linux 发行版，依靠定期的冻结和里程碑发布（Alpha、Beta、Final）来管理质量。发布工程是一个专业领域，负责将软件包组装成完整的操作系统，新成员需要逐步获取特殊权限。这篇博文填补了该流程端到端文档的空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fedoraproject.org/wiki/ReleaseEngineering/Overview">ReleaseEngineering/Overview - Fedora Project Wiki</a></li>
<li><a href="https://docs.fedoraproject.org/en-US/infra/release_guide/">Fedora Release Engineering :: Fedora Docs</a></li>

</ul>
</details>

**社区讨论**: 评论总体正面：cube00 认为该指南对排查文件权限问题非常有用；hangrybear666 询问何处可以参与贡献。少数无关评论提到了 IBM 的蓝洗白和“Beefy Miracle”昵称。

**标签**: `#Fedora`, `#release engineering`, `#documentation`, `#Linux`, `#open source`

---

<a id="item-14"></a>
## [GitLab RCE PoC 暴露未打补丁的服务器](https://thehackernews.com/2026/07/researcher-publishes-gitlab-rce-poc.html) ⭐️ 7.0/10

研究员 depthfirst 于 7 月 24 日发布了一个针对 GitLab 远程代码执行 (RCE) 漏洞的有效利用程序，该漏洞已于 6 月 10 日修复，允许具有推送权限的认证用户在自管理的 GitLab 18.11.3 服务器上以 git 用户身份执行命令。 该公开漏洞利用程序增加了运行未打补丁的 GitLab 实例的组织的风险，攻击者可以利用有限的权限获得代码执行能力。这凸显了及时打补丁的重要性，尤其是对于自管理部署。 该漏洞利用需要具有项目推送权限的认证用户，通过提交一个特制的 Jupyter 笔记本并打开其提交差异，触发堆泄漏并以 git 用户身份实现远程代码执行。该漏洞影响 GitLab 版本 18.11.3，并在后续版本中修复。

rss · The Hacker News · 7月25日 10:14

**背景**: GitLab 是一个流行的 DevOps 平台，具有 CI/CD 功能。远程代码执行漏洞允许攻击者在服务器上运行任意命令，可能导致数据泄露或横向移动。如果未及时更新，自管理实例尤其面临风险。

**标签**: `#GitLab`, `#RCE`, `#security`, `#exploit`, `#vulnerability`

---

<a id="item-15"></a>
## [保险钓鱼攻击已演变为实时账户劫持](https://thehackernews.com/2026/07/ctm360-research-reveals-how-insurance.html) ⭐️ 7.0/10

CTM360 的研究显示，针对保险公司的钓鱼活动已从传统的凭证窃取演变为实时账户劫持，攻击者立即使用窃取的凭证接管账户。 这一转变标志着钓鱼战术的重大升级，使攻击更加即时且更难检测，给保险公司和投保人带来更大风险。 研究指出，攻击者不再收集凭证以备后用，而是通过中间人攻击实时获取会话令牌并绕过多因素认证。

rss · The Hacker News · 7月25日 10:14

**背景**: 传统钓鱼攻击诱骗受害者输入登录凭据，攻击者之后再使用这些凭据。而实时账户劫持则利用反向代理等技术，在登录过程中拦截凭据和会话令牌，从而实现立即的账户接管。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/ctm360-research-reveals-how-insurance.html">CTM360 Research Reveals How Insurance Phishing Has Evolved Into...</a></li>
<li><a href="https://netspider.io/man-in-the-middle-phishing/">Man-in-the-Middle phishing</a></li>
<li><a href="https://izoologic.com/threat-advisory/mass-telegram-account-hijacking-via-supply-chain-phishing-campaign/">Mass Telegram account hijacking via supply-chain phishing campaign</a></li>

</ul>
</details>

**标签**: `#phishing`, `#cybersecurity`, `#account hijacking`, `#insurance`, `#threat research`

---

<a id="item-16"></a>
## [DevMan 勒索软件即服务平台集中化载荷构建与支付](https://thehackernews.com/2026/07/devman-raas-portal-centralizes-payload.html) ⭐️ 7.0/10

DevMan 勒索软件运营者推出了一个中央化网页门户，供附属成员生成载荷、管理受害者及处理付款，标志着该操作从混乱向更专业的勒索软件即服务平台转变。 这种集中化降低了网络犯罪分子发起勒索软件攻击的门槛，可能增加攻击的数量和复杂度，并使防御者更难追踪和破坏该操作。 该门户整合了载荷生成、财务管理和受害者监督功能；该操作被 PRODAFT 追踪为 Funky Mantis，DevMan 于 2025 年 4 月首次出现，曾是其他勒索软件即服务组织的附属成员，之后才推出自己的平台。

rss · The Hacker News · 7月25日 09:53

**背景**: 勒索软件即服务是一种网络犯罪商业模式，勒索软件开发者向附属成员提供恶意软件和基础设施，附属成员实施攻击并分享赎金收益。DevMan 最初是 Qilin 和 RansomHub 等组织的附属成员，后来发展出自己的勒索软件即服务操作，配有精美的网页门户、泄露博客和受害者名单。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/devman-raas-portal-centralizes-payload.html">DevMan RaaS Portal Centralizes Payload Builds, Victim Management...</a></li>
<li><a href="https://ctrlaltint3l.github.io/threat+research/Devman-RaaS/">How not to run a RaaS Operation - Ctrl-Alt-Int3l</a></li>
<li><a href="https://meterpreter.org/funky-mantis-ransomware/">Funky Mantis Ransomware Runs a Full RaaS Platform</a></li>

</ul>
</details>

**标签**: `#ransomware`, `#cybersecurity`, `#RaaS`, `#cybercrime`

---

<a id="item-17"></a>
## [Steam 论坛 ClickFix 攻击传播 XMRig 加密矿工](https://www.bleepingcomputer.com/news/security/steam-forum-clickfix-attacks-infect-gamers-with-xmrig-cryptominers/) ⭐️ 7.0/10

攻击者利用 Steam 讨论论坛进行 ClickFix 社会工程攻击，诱骗游戏玩家执行命令，从而下载并运行 XMRig 加密矿工。 该攻击针对庞大的游戏用户群体，这些用户可能安全意识较薄弱，攻击将他们的系统变成隐蔽的矿机并降低性能。这凸显了游戏社区中社会工程攻击的日益复杂化。 ClickFix 技术显示虚假错误消息，并提供看似修复的恶意 PowerShell 命令。有效负载是 XMRig，这是一个常用于加密劫持的开源 Monero 矿工。

rss · BleepingComputer · 7月25日 22:37

**背景**: ClickFix 是一种社会工程技巧，利用用户急于解决技术问题的心理，诱骗他们复制并运行恶意命令。XMRig 是合法的 Monero 挖矿软件，但网络犯罪分子经常在未经用户同意的情况下部署它来窃取计算资源。在 Steam 这样的可信平台上结合这两种手段，使得攻击极具欺骗性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/security/blog/2025/08/21/think-before-you-clickfix-analyzing-the-clickfix-social-engineering-technique/">Think before you Click (Fix): Analyzing the ClickFix social engineering ...</a></li>
<li><a href="https://www.checkpoint.com/cyber-hub/threat-prevention/what-is-malware/xmrig-malware/">XMRig Malware - Check Point Software</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#cryptomining`, `#Steam`, `#malware`, `#social-engineering`

---

<a id="item-18"></a>
## [恶意网站通过 JavaScript 在浏览器内存中组装恶意软件](https://www.bleepingcomputer.com/news/security/malicious-sites-use-javascript-to-build-malware-in-browser-memory/) ⭐️ 7.0/10

一场大规模恶意广告活动利用假冒的 Solana、Luno 和 TradingView 网页，通过恶意 JavaScript 指令让浏览器在内存中直接组装恶意软件，绕过了基于文件的传统检测。 这种技术实现了无文件恶意软件的执行，能够逃避杀毒软件和取证分析，对加密货币交易平台用户构成严重威胁，也凸显了内存级威胁检测的必要性。 该活动自 2024 年底以来一直活跃，具有区域性目标，利用恶意 JavaScript 在浏览器端进行代码组装，无需向磁盘写入任何文件。

rss · BleepingComputer · 7月25日 15:21

**背景**: 无文件恶意软件是一种仅存在于计算机 RAM 中的变种，它避免写入硬盘以逃避传统杀毒软件。该攻击利用浏览器的 JavaScript 引擎，完全在内存中构造并执行恶意软件，使得基于文件的签名或取证工具极难检测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fileless_malware">Fileless malware - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#malvertising`, `#JavaScript`, `#malware`, `#browser`

---

<a id="item-19"></a>
## [ShinyHunters 数据泄露助长 2000 美元性勒索诈骗](https://www.bleepingcomputer.com/news/security/shinyhunters-data-leaks-fuel-2-000-sextortion-email-scam/) ⭐️ 7.0/10

威胁行为者正在利用 ShinyHunters 黑客组织数据泄露中暴露的电子邮件地址，发送要求支付 2000 美元比特币的性勒索邮件。 这一骗局表明，过去的数据泄露如何被武器化用于定向勒索，增加了数百万已泄露凭据用户的风险。 这些邮件通常声称拥有受害者的不雅视频，并要求比特币付款，利用真实泄露的电子邮件地址来显得可信。

rss · BleepingComputer · 7月25日 14:16

**背景**: ShinyHunters 是一个自 2020 年以来进行大规模数据泄露的臭名昭著的网络犯罪组织，包括窃取超过 500 GB 的微软源代码。性勒索诈骗涉及威胁发布私密照片除非支付赎金，通常利用泄露的个人数据来恐吓受害者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ShinyHunters">ShinyHunters - Wikipedia</a></li>
<li><a href="https://www.ic3.gov/PSA/2026/PSA260515">Internet Crime Complaint Center (IC3) | ShinyHunters: Cyber Criminal Group Attacks Learning Management System</a></li>

</ul>
</details>

**标签**: `#security`, `#data breach`, `#phishing`, `#sextortion`

---

<a id="item-20"></a>
## [OpenAI 确认 ChatGPT 全球宕机](https://www.bleepingcomputer.com/news/artificial-intelligence/openai-confirms-chatgpt-is-down-worldwide/) ⭐️ 7.0/10

OpenAI 已确认 ChatGPT 正在经历全球性宕机，导致数百万用户无法访问该服务。 此次宕机影响了包括依赖 ChatGPT 处理日常任务的个人和企业在内的庞大用户群体，凸显了对集中式 AI 服务的依赖。 此次宕机似乎是全球性的，影响了网页界面和 API，但 OpenAI 尚未说明原因或预计恢复时间。

rss · BleepingComputer · 7月25日 09:31

**背景**: ChatGPT 是 OpenAI 基于大型语言模型开发的聊天机器人，于 2022 年 11 月推出。它迅速成为全球最受欢迎的 AI 服务之一，用于写作、编程和回答问题等任务。此类宕机会打乱许多依赖 ChatGPT 的用户和企业的正常工作流程。

**标签**: `#ChatGPT`, `#OpenAI`, `#outage`, `#AI service`

---