---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> 从 93 条内容中筛选出 20 条重要资讯。

---

1. [WebAssembly 中的 Firefox：浏览器内运行完整浏览器](#item-1)
2. [Thinky 发布 975B-A41B 开源多模态模型](#item-2)
3. [Kimi K3：2.8 万亿参数、1M 上下文模型发布](#item-3)
4. [一加停止在美欧推出新产品](#item-4)
5. [从 Rust 到 Zig 的编译器重写进展](#item-5)
6. [GPT-5.6 Codex 漏洞可在完全访问模式下删除用户文件](#item-6)
7. [Lila Sciences 旨在将实验室转变为 AI 数据中心](#item-7)
8. [AI 隐私保护：从数据控制转向企业问责](#item-8)
9. [NVIDIA Nemotron-3 Embed 在 RTEB 基准测试中排名第一](#item-9)
10. [CISA 警告：AutomationDirect Productivity Suite 存在高危漏洞](#item-10)
11. [n8n 令牌交换漏洞致认证绕过](#item-11)
12. [新型 ClickLock macOS 窃密软件通过频繁杀死应用强迫用户输入密码](#item-12)
13. [代理数据注入攻击欺骗 AI 代理执行错误操作](#item-13)
14. [Daxin 根套件与 Stupig 后门在台湾重现](#item-14)
15. [未修复的 Shark 吸尘器漏洞可让攻击者跨区域控制其他吸尘器](#item-15)
16. [OpenAI 的 GPT-Red 自动化提示注入测试](#item-16)
17. [Zoom 修复可导致账户被接管的关键 Windows 漏洞](#item-17)
18. [Claude Chrome 扩展漏洞允许点击劫持攻击](#item-18)
19. [CISA 要求联邦机构在周六前修补 Oracle 漏洞](#item-19)
20. [DFlash 让 Qwen3.6-27B 提速 2.2 倍且无质量损失](#item-20)

---

<a id="item-1"></a>
## [WebAssembly 中的 Firefox：浏览器内运行完整浏览器](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter 将 Firefox/Gecko 浏览器引擎编译为 WebAssembly，使得该完整浏览器可在另一个浏览器（如 Chrome）中运行。该项目估计使用了价值 25,000 美元的 Claude Opus 和 Fable 模型 AI 代币。 这展示了像完整浏览器引擎这样的复杂原生应用可以移植到 WebAssembly，为基于 Web 的计算和云桌面开辟了新可能性。同时也凸显了 AI 辅助编程在应对大规模移植项目中的重要作用。 所有网络流量通过 Wisp 协议经由 Puter 的服务器代理，因为 WebAssembly 代码无法直接打开网络连接。生成的二进制文件包含一个 233MB 的 gecko.wasm 文件和一个 18MB 的 chrome-assets 归档。

rss · Simon Willison · 7月16日 23:34

**背景**: WebAssembly（WASM）是一种低级二进制指令格式，专为在 Web 浏览器中高性能执行而设计。Wisp 协议由 MercuryWorkshop 开发，是一种轻量级协议，用于通过单个 WebSocket 连接代理 TCP 和 UDP 套接字，对绕过浏览器网络限制至关重要。本项目选择 Firefox 是因为其 Gecko 引擎具有强大的单进程支持，简化了编译过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wire_protocol">Wire protocol</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Compilation`, `#Demonstration`

---

<a id="item-2"></a>
## [Thinky 发布 975B-A41B 开源多模态模型](https://www.latent.space/p/ainews-thinkys-inkling-975b-a41b) ⭐️ 9.0/10

由 Mira Murati 领导的 Thinking Machines Lab 发布了 Inkling 模型，这是一个拥有 975B 总参数（41B 活跃参数）的混合专家多模态模型，采用 Apache 2.0 许可证。他们还宣布了 Inkling-Small（276B-A12B），权重后续发布。 此次发布通过提供大型、多模态且采用宽松许可证的模型，显著增强了开源 AI 生态系统，为中国开源模型提供了竞争替代方案，并巩固了美国开源权重领域的地位。它通过 Tinker 平台支持广泛的微调和定制。 Inkling 是一个混合专家变换器，采用稀疏 MoE、短卷积、嵌入 RMSNorm 和相对位置偏置，在 45 万亿文本、图像、音频和视频 tokens 上训练。它并非前沿模型，而是旨在作为强大的微调基础，其模型卡片异常简洁。

rss · Latent Space · 7月16日 06:18

**背景**: 混合专家（MoE）是一种神经网络架构，每次输入仅激活部分参数，从而在较低计算成本下实现大模型容量。短卷积有助于高效捕获局部上下文，而 RMSNorm 和相对位置偏置则是用于提高变换器训练稳定性和位置理解的技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/mixture-of-transformer-experts-mot">Mixture - of - Transformer - Experts (MoT)</a></li>
<li><a href="https://arxiv.org/abs/2406.08128">[2406.08128] Short-Long Convolutions Help Hardware-Efficient Linear Attention to Focus on Long Sequences</a></li>
<li><a href="https://njudeepengine.github.io/LLM-Blog/2025/06/17/A2-norm-emb/">A2 RMSNorm and Embedding | LLM-Assignment-Doc</a></li>

</ul>
</details>

**标签**: `#multimodal`, `#open-source`, `#large language model`, `#Apache 2.0`, `#AI`

---

<a id="item-3"></a>
## [Kimi K3：2.8 万亿参数、1M 上下文模型发布](https://www.reddit.com/r/LocalLLaMA/comments/1uy3a0q/kimi_k3_released_on_web_and_app/) ⭐️ 9.0/10

月之暗面（Moonshot AI）发布了 Kimi K3，这是一个拥有 2.8 万亿参数和 100 万 Token 上下文窗口的大型语言模型，在编码、智能体任务、长程推理、视觉理解和智能体蜂群能力方面声称达到最先进水平。 如果得到验证，Kimi K3 将是 LLM 能力的一个重大里程碑，在多个领域可能媲美 Claude 和 GPT 等顶级模型，并且计划开放模型权重可能会使前沿 AI 的获取更加民主化。 该模型拥有 2.8 万亿参数和 100 万 Token 上下文窗口，是当前最大的模型之一。据社区报道，在 OpenRouter 上的定价为每百万输出 Token 15 美元，完整模型权重将在未来几天与一份技术报告一起发布。

reddit · r/LocalLLaMA · /u/External_Mood4719 · 7月16日 13:43

**背景**: Kimi K3 是由月之暗面（Moonshot AI）开发的大型语言模型。该模型声称的能力包括智能体任务（能够自主使用工具的 AI）、长程推理（跨长时间的多步规划）和智能体蜂群（多个专门智能体协作）。100 万 Token 的上下文窗口使其能够处理非常长的文档。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is agentic AI? - IBM</a></li>
<li><a href="https://arxiv.org/abs/2512.10739">[2512.10739] Long-horizon Reasoning Agent for Olympiad-Level Mathematical Problem Solving</a></li>
<li><a href="https://www.agent-swarm.dev/">Agent Swarm — Multi-Agent Orchestration for AI Agents</a></li>

</ul>
</details>

**社区讨论**: 社区评论对月之暗面使用 API 数据进行训练（包括企业使用）表示担忧，指出成本高昂（单次渲染 0.25 美元），并讨论中国实验室是否旨在将 AI 智能商品化以销售硬件基础设施。一些人对该模型声称的排名表示怀疑。

**标签**: `#LLM`, `#AI model`, `#Coding`, `#Large-scale AI`, `#Agentic tasks`

---

<a id="item-4"></a>
## [一加停止在美欧推出新产品](https://community.oneplus.com/thread/2170715118587871237) ⭐️ 8.0/10

一加宣布将停止在美国和欧洲推出新产品，但会继续为现有设备提供软件更新和安全补丁。 这标志着一个曾经广受欢迎的智能手机品牌从关键西方市场的重大战略撤退，可能重塑竞争格局，并影响那些现在面临有限升级路径的忠实用户。 该决定仅限于新产品发布；现有设备将在原定支持期内获得定期更新和安全补丁，由 OPPO 提供支持。

hackernews · pilililo2 · 7月16日 10:14 · [社区讨论](https://news.ycombinator.com/item?id=48932539)

**背景**: 一加最初以“不将就”（Never Settle）的手机品牌闻名，提供高端配置、接近原生的安卓系统以及有竞争力的价格，在爱好者中获得了强大追随。随着时间的推移，该公司调整了战略，逐渐靠近 OPPO，并失去了部分对黑客友好的特性，例如轻松的 bootloader 解锁和官方固件镜像的提供。

**社区讨论**: 评论者反应不一：有人纠正误导性标题，指出现有用户的操作仍将继续；另一些人则哀叹该品牌从爱好者根源的衰落，提及诸如停止发布工厂镜像等变化。一名前员工强调了公司高强度的 996 文化，并称赞了近期型号如一加 13 和一加 15 的续航能力。

**标签**: `#OnePlus`, `#smartphone industry`, `#business strategy`, `#tech news`

---

<a id="item-5"></a>
## [从 Rust 到 Zig 的编译器重写进展](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

一篇详细博客描述了将一个 Rust 编译器重写为 Zig 的进展，重点讨论了内存控制、安全性和增量构建性能之间的权衡。 这个在编译器项目中比较 Rust 和 Zig 的实际案例为系统程序员提供了有价值的见解，特别是在安全性与控制之间的权衡方面。 作者强调 Zig 的增量构建速度显著更快，并且对于代码生成等编译器任务，内存控制至关重要，尽管 Zig 的安全检查无法捕获所有释放后使用错误。

hackernews · jorangreef · 7月16日 11:39 · [社区讨论](https://news.ycombinator.com/item?id=48933149)

**背景**: Rust 通过其所有权系统在编译时强制执行内存安全，而 Zig 则提供手动内存管理及可选的运行时安全检查。编译器通常涉及不安全的操作，如发出机器码或二进制补丁，这些操作需要细粒度的内存控制。这次重写使得在实践且性能关键的场景中直接比较这两种系统编程语言成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziglang.org/learn/why_zig_rust_d_cpp/">Why Zig When There is Already C++, D, and Rust? ⚡ Zig Programming Language</a></li>
<li><a href="https://medium.com/@shyamsundarb/memory-safety-in-c-vs-rust-vs-zig-f78fa903f41e">Memory Safety in C++ vs Rust vs Zig | by B Shyam Sundar | Medium</a></li>
<li><a href="https://rustc-dev-guide.rust-lang.org/overview.html">Overview of the compiler - Rust Compiler Development Guide</a></li>

</ul>
</details>

**社区讨论**: steveklabnik 等评论者认为发出机器码本身并不需要不安全代码，质疑重写的必要性。landr0id 指出 Zig 的 ReleaseSafe 无法捕获所有释放后使用或双重释放错误，对其安全性声明提出质疑。其他人赞扬 Zig 的增量构建，但想知道 Rust 何时能赶上。

**标签**: `#Rust`, `#Zig`, `#compilers`, `#systems programming`, `#rewrite`

---

<a id="item-6"></a>
## [GPT-5.6 Codex 漏洞可在完全访问模式下删除用户文件](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

据报道，GPT-5.6 Codex 存在一个漏洞，当启用完全访问模式且未开启沙盒保护（包括自动审查）时，模型可能意外删除用户文件。 该漏洞凸显了具有直接文件系统访问权限的 AI 编程代理存在的严重安全风险，因为即使意图良好的模型也可能犯下灾难性错误。它强调了在生产环境中部署自主代理之前，建立强大的沙盒和审批机制的迫切需要。 该漏洞发生在模型试图覆盖 $HOME 环境变量以定义临时目录时，却错误地删除了 $HOME 目录。此问题出现在未启用沙盒且未开启自动审查的完全访问模式下。

rss · Simon Willison · 7月16日 17:45

**背景**: GPT-5.6 Codex 是 OpenAI 最新的编程代理，能够生成代码、运行命令和搜索仓库。Codex 提供不同的访问模式：只读、自动批准和完全访问。完全访问模式赋予模型无限制的读写文件能力，对自主任务很有用，但若无沙盒保护则很危险。沙盒将代理与主机系统隔离，以防止意外副作用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://vladimirsiedykh.com/blog/codex-cli-approval-modes-2025">Codex CLI approval modes explained: auto vs read only vs...</a></li>
<li><a href="https://northflank.com/blog/how-to-sandbox-ai-agents">How to sandbox AI agents in 2026: MicroVMs, gVisor ...</a></li>

</ul>
</details>

**标签**: `#codex`, `#AI safety`, `#file deletion`, `#coding agents`, `#generative-ai`

---

<a id="item-7"></a>
## [Lila Sciences 旨在将实验室转变为 AI 数据中心](https://www.latent.space/p/the-lab-of-the-future-should-feel) ⭐️ 8.0/10

由 Andy Beam 和 Rafa Gómez-Bombarelli 领导的 Lila Sciences 提出了一种新范式，将科学实验室改造为数据中心，利用机器人生成实验数据来训练 AI 模型。 这种方法可以解锁科学实验中未开发的训练数据源，可能加速材料科学和药物开发等领域的 AI 驱动发现。 这一概念涉及用机器人自动化实验室，持续运行实验，生成高质量标注数据，用于训练 AI 模型进行科学预测和假设生成。

rss · Latent Space · 7月16日 13:30

**背景**: 传统上，AI 模型依赖于互联网或精心策划来源的大型数据集。Lila Sciences 认为，科学实验代表着一种尚未开发的高价值训练数据源，可以通过机器人在受控实验室环境中系统性地生成。

**标签**: `#AI in science`, `#robotics`, `#data generation`, `#scientific discovery`, `#lab automation`

---

<a id="item-8"></a>
## [AI 隐私保护：从数据控制转向企业问责](https://www.schneier.com/blog/archives/2026/07/protecting-privacy-in-an-ai-era.html) ⭐️ 8.0/10

Daniel Solove 在《华尔街日报》中提出，在 AI 时代，让个人控制自己的数据不足以保护隐私，而应像食品和药品安全法一样，让企业承担责任。 这种从个人同意到企业问责的转变可能从根本上改变隐私法的设计方式，使其更有效地对抗大型 AI 公司的系统性数据滥用。 提出的措施包括严格的数据最小化、数据处理者的受托责任、对疏忽或鲁莽 AI 设计的责任、对造成伤害的算法的责任，以及多方利益相关者技术审查。

rss · Schneier on Security · 7月16日 14:34

**背景**: 当前的隐私法规（如 GDPR 和 CCPA）主要依赖通知与同意，要求公司在处理数据前获得用户许可。批评者认为这给个人带来了不切实际的负担，且未能遏制有害的数据实践。Solove 的方法借鉴了食品和药品监管，要求公司在产品面向消费者前证明其安全性。

**标签**: `#privacy`, `#AI`, `#regulation`, `#data protection`, `#accountability`

---

<a id="item-9"></a>
## [NVIDIA Nemotron-3 Embed 在 RTEB 基准测试中排名第一](https://huggingface.co/blog/nvidia/nemotron-3-embed-wins-rteb) ⭐️ 8.0/10

NVIDIA 发布了 Nemotron-3 Embed 系列开放嵌入模型，该模型在检索嵌入基准测试（RTEB）中取得了总体最高分。 这一里程碑为代理检索和 RAG 系统提供了一种高质量、可用于生产的嵌入模型，有望提升 AI 代理在检索任务中的性能。 Nemotron-3 Embed 模型基于变压器架构，采用双向注意力机制，包含 1B 参数的 BF16 版本以及量化后的 NVFP4 变体，以提供部署灵活性。

rss · Hugging Face Blog · 7月16日 16:01

**背景**: 嵌入模型将文本编码为密集向量以进行相似性搜索，是检索增强生成（RAG）和代理检索系统的基础。RTEB 是最近推出的基准测试，专注于评估针对实际应用的检索准确性。代理检索涉及使用大语言模型将复杂查询分解为子查询，以改进检索效果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/nvidia/nemotron-3-embed-wins-rteb">NVIDIA Nemotron 3 Embed Ranks #1 Overall on RTEB, Advancing Agentic Retrieval</a></li>
<li><a href="https://huggingface.co/blog/rteb">Introducing RTEB: A New Standard for Retrieval Evaluation</a></li>
<li><a href="https://github.com/embedding-benchmark/rteb">GitHub - embedding-benchmark/rteb: Retrieval Embedding Benchmark · GitHub</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#embedding`, `#retrieval`, `#AI`, `#benchmark`

---

<a id="item-10"></a>
## [CISA 警告：AutomationDirect Productivity Suite 存在高危漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-197-04) ⭐️ 8.0/10

美国网络安全和基础设施安全局（CISA）发布通报（ICSA-26-197-04），警告 AutomationDirect Productivity Suite v4.6.2.2 及更早版本存在多个高危漏洞，包括越界写入、越界读取和除零错误，本地或物理访问的攻击者可利用这些漏洞导致内存损坏或拒绝服务。 这些漏洞影响全球范围内的关键制造业基础设施，成功利用可能允许攻击者破坏工业控制系统，导致生产中断或安全事故。使用 Productivity Suite 的组织应紧急升级至 v4.7.0.47 或更高版本以降低风险。 该通报列出了六个 CVE 编号（如 CVE-2026-60063），CVSS v3 基础评分为 7.0（高危），且利用需要本地或物理访问工程工作站。AutomationDirect 建议更新至 Productivity Suite v4.7.0.47，若无法立即更新，需实施补偿性控制措施，如断开外部网络连接和限制物理访问。

rss · CISA Cybersecurity Advisories · 7月16日 12:00

**背景**: AutomationDirect Productivity Suite 是一款基于 Windows 的编程和配置软件，用于 AutomationDirect 的 Productivity 系列可编程逻辑控制器（PLC），广泛应用于工业自动化和关键制造业。该软件在工程工作站上运行，与 PLC 通信以编程和监控控制逻辑。此类软件中的漏洞可能危及工业控制系统的完整性和可用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.automationdirect.com/adc/shopping/catalog/programmable_controllers/productivity1000_plcs_(stackable_micro)/productivity1000_accessories/ps-pgmsw">Productivity Suite Windows Programming and... | AutomationDirect</a></li>
<li><a href="https://control.com/technical-articles/how-to-simple-programming-with-automationdirect-productivity-plcs/">How To: Simple Programming with AutomationDirect Productivity ...</a></li>

</ul>
</details>

**标签**: `#CISA`, `#AutomationDirect`, `#ICS`, `#vulnerability`, `#security-advisory`

---

<a id="item-11"></a>
## [n8n 令牌交换漏洞致认证绕过](https://thehackernews.com/2026/07/n8n-token-exchange-flaw-could-let.html) ⭐️ 8.0/10

n8n 企业版实例存在严重安全漏洞，其 JWT 验证忽略`iss`声明，仅基于`sub`声明匹配用户，导致攻击者可使用来自一个签发者的有效令牌，以另一个签发者中`sub`相同的用户身份登录。 该漏洞破坏了多签发者环境中的身份验证，可能导致对敏感工作流和数据的未授权访问，n8n 企业版用户需立即修复。 该漏洞影响配置了信任多个外部令牌签发者的 n8n 企业版实例；修复措施需在匹配用户前，验证`iss`声明是否与预期签发者一致。

rss · The Hacker News · 7月16日 13:33

**背景**: n8n 是一个低代码的工作流自动化平台，具备 AI 能力。JWT（JSON Web 令牌）包含`iss`（签发者）声明，用于标识令牌签发者；正确的验证应同时检查`iss`和`sub`，以防止跨签发者冒充。安全研究人员报告的此漏洞凸显了彻底验证声明的重要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://n8n.io/">n8n.io - AI workflow automation platform</a></li>
<li><a href="https://workos.com/blog/how-to-validate-the-jwt-iss-claim">How to validate the JWT iss claim and why it matters — WorkOS</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#n8n`, `#authentication`, `#JWT`

---

<a id="item-12"></a>
## [新型 ClickLock macOS 窃密软件通过频繁杀死应用强迫用户输入密码](https://thehackernews.com/2026/07/new-clicklock-macos-stealer-kills-apps.html) ⭐️ 8.0/10

一款名为 ClickLock 的新型 macOS 信息窃取恶意软件，每 210 毫秒杀死所有可见应用程序，直到受害者输入系统登录密码；它通过假对话框和 LaunchAgent 持久化机制实现。 ClickLock 引入了一种极具侵略性的社会工程学手段，通过扰乱系统正常使用来强迫用户输入密码，对 macOS 用户构成重大威胁，并展示了一种新型攻击模式。 该恶意软件通过粘贴到终端的命令传播，安装两个 LaunchAgent，并在受害者取消初始虚假密码提示后悄悄退出；下次登录时，它会继续杀死应用直到获取密码。

rss · The Hacker News · 7月16日 12:33

**背景**: LaunchAgent 是由 macOS 的 launchd 管理的后台进程，常用于合法自动化，但常被恶意软件用于持久化。ClickLock 利用这一点安装 LaunchAgent，在每次登录后重新启动其激进的应用杀死程序，使得在不知密码的情况下难以清除。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@durgaviswanadh/understanding-macos-launchagents-and-login-items-a-clear-practical-guide-5c0e39e3a6b3">Understanding macOS LaunchAgents and Login Items: A ... - Medium</a></li>
<li><a href="https://gist.github.com/Matejkob/f8b1f6a7606f30777552372bab36c338">echnical Guide: Building a Modern Launch Agent on macOS</a></li>

</ul>
</details>

**标签**: `#macOS`, `#malware`, `#cybersecurity`, `#infostealer`, `#threat`

---

<a id="item-13"></a>
## [代理数据注入攻击欺骗 AI 代理执行错误操作](https://thehackernews.com/2026/07/new-agent-data-injection-attack-can.html) ⭐️ 8.0/10

研究人员发现了一种新型攻击手段，称为代理数据注入攻击。攻击者通过污染可信数据源（如产品评论或 GitHub 评论），诱使 AI 代理执行意外操作，例如点击“立即购买”或运行任意命令。 该攻击破坏了依赖外部数据的 AI 代理的可靠性，对电商、编程助手等领域的应用构成严重安全风险，因为这些代理代表用户采取行动。 与注入指令的间接提示注入不同，代理数据注入攻击污染的是代理所信任的事实数据，使其在执行请求任务的同时做出错误行动。该攻击详细描述于 2026 年 7 月发表在 arXiv 上的一篇论文中。

rss · The Hacker News · 7月16日 11:32

**背景**: AI 代理是基于 LLM 的系统，能够通过消费外部数据（如评论）并执行操作（如点击按钮）来完成任务。此前的安全研究主要关注间接提示注入（IPI），即未受信任的数据被解释为指令。代理数据注入则是一种更隐蔽的威胁，它污染数据本身，使代理基于虚假信息行动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.05120">Agent Data Injection Attacks are Realistic Threats to AI Agents</a></li>
<li><a href="https://www.linkedin.com/pulse/offensive-ai-llmml-red-teaming-indirect-prompt-injection-harshad-shah-hopnc">Indirect Prompt Injection Attacks : The Silent LLM Threat</a></li>

</ul>
</details>

**标签**: `#AI security`, `#data injection`, `#adversarial attack`, `#AI agents`, `#LLM safety`

---

<a id="item-14"></a>
## [Daxin 根套件与 Stupig 后门在台湾重现](https://thehackernews.com/2026/07/daxin-resurfaces-in-taiwan-alongside.html) ⭐️ 8.0/10

沉寂四年多的 Daxin 内核级根套件在台湾一家制造企业中重新出现，并伴随一个此前未记录的名为 Stupig 的后门。Stupig 作为登录前后门，可通过 Windows 登录进程执行 SYSTEM 级别的命令。 此次重现表明高级威胁行为者仍然活跃并持续改进其工具，对制造业等领域的重点目标构成持续威胁。新型 Stupig 后门引入了隐蔽的预认证能力，可能绕过许多安全控制措施。 两个恶意软件组件均带有 2013 年的编译时间戳，表明长期开发和精密的操作安全性。Daxin 作为内核级根套件，监控传入的 TCP 流量以寻找特定模式，进而劫持这些流量用于命令与控制（C2）通信。

rss · The Hacker News · 7月16日 11:17

**背景**: Daxin 是一种高级 Windows 内核级根套件，由 Symantec 于 2022 年首次记录，被归因于与中国有关的威胁行为者。根套件在操作系统的最低层级运行，能够隐藏自身存在和活动，躲避安全软件的检测。像 Stupig 这样的登录前后门可以在用户登录前执行代码，使检测和分析变得极为困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/daxin-resurfaces-in-taiwan-alongside.html">Daxin Resurfaces in Taiwan Alongside Stupig Pre-Login SYSTEM ...</a></li>
<li><a href="https://hoploninfosec.com/daxin-malware-stupig-backdoor-analysis">Daxin Malware and Stupig Backdoor: Full Technical Analysis</a></li>
<li><a href="https://www.thestack.technology/daxin-chinese-malware-threat-sophisticated-symantec/">Previously undocumented rootkit " Daxin " being deployed by Chinese...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#threat intelligence`, `#China-linked APT`, `#rootkit`

---

<a id="item-15"></a>
## [未修复的 Shark 吸尘器漏洞可让攻击者跨区域控制其他吸尘器](https://thehackernews.com/2026/07/unpatched-shark-vacuum-flaw-could-let.html) ⭐️ 8.0/10

一位化名 tokay0 的研究人员演示了，从 Shark RV2320EDUS 机器人吸尘器中提取证书后，即可获得同一 AWS 区域内其他 Shark 吸尘器的 root 访问权限，从而窃取摄像头画面、房屋地图和 Wi-Fi 密码。 该漏洞暴露了一个严重的物联网安全弱点：单一设备被攻破后，可能波及同一云区域内的众多设备，影响用户隐私和对智能家居设备的信任。 攻击需要物理接触吸尘器以从闪存中提取证书，但一旦获得，即可在同一 AWS 区域内对任何其他 Shark 吸尘器执行远程 root 命令，无需身份验证。

rss · The Hacker News · 7月16日 09:23

**背景**: 许多物联网设备依赖 AWS IoT 等云服务进行通信，并使用证书进行设备身份验证。如果同一区域内的设备使用通用证书或弱信任模型，攻破一台设备就可能使攻击者访问所有设备。该漏洞凸显了物联网生态系统中共享凭证和隔离不足的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://secureiot.house/wolfssl-cve-2026-5194-certificate-forgery-5-billion-iot-devices/">The Encryption Library in 5 Billion Devices Just Broke: CVE ...</a></li>
<li><a href="https://docs.aws.amazon.com/iot-device-defender/latest/devguide/audit-chk-iot-policy-permissive.html">AWS IoT policies overly permissive - AWS IoT Device Defender</a></li>

</ul>
</details>

**标签**: `#security`, `#IoT`, `#vulnerability`, `#robot vacuum`, `#AWS`

---

<a id="item-16"></a>
## [OpenAI 的 GPT-Red 自动化提示注入测试](https://thehackernews.com/2026/07/openais-gpt-red-automates-prompt.html) ⭐️ 8.0/10

OpenAI 公开了 GPT-Red，这是一个内部自动化红队模型，用于规模化发现提示注入漏洞，并利用它对包括 GPT-5.6 Sol 在内的 GPT 模型进行对抗性训练以增强安全性。 提示注入是对大语言模型的一种关键安全威胁，而规模化自动化红队测试可以在部署前主动修复漏洞，为 AI 安全树立新的行业标杆。 OpenAI 表示，之前的模型极易受到 GPT-Red 的提示注入攻击，他们现在使用 GPT-Red 进行对抗性训练以提高模型鲁棒性。

rss · The Hacker News · 7月16日 08:42

**背景**: 提示注入攻击通过将恶意输入伪装成合法提示来操纵大语言模型，可能导致数据泄露或绕过政策。红队测试通过模拟对抗性攻击来发现漏洞，而对抗性训练则利用这些攻击来提高模型的抵抗能力。这种方法是 AI 开发中的主动安全实践。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/prompt-injection">What is a prompt injection attack? - IBM</a></li>
<li><a href="https://www.crowdstrike.com/en-us/cybersecurity-101/cyberattacks/prompt-injection/">What is Prompt Injection? | CrowdStrike</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adversarial_machine_learning">Adversarial machine learning - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI security`, `#prompt injection`, `#red-teaming`, `#OpenAI`, `#LLM`

---

<a id="item-17"></a>
## [Zoom 修复可导致账户被接管的关键 Windows 漏洞](https://thehackernews.com/2026/07/zoom-patches-critical-windows-flaw-that.html) ⭐️ 8.0/10

Zoom 发布了针对 Windows 版 Zoom Workplace 中一个关键漏洞（CVE-2026-53412，CVSS 评分 9.8）的安全更新，该漏洞可能导致账户被接管。 该漏洞为关键等级，影响广泛使用的 Zoom 组件，可能使攻击者无需用户交互即可接管账户。立即打补丁至关重要。 该漏洞影响 Windows 版 Zoom Desktop Client、Zoom VDI Client 和 Zoom Meeting SDK，由不当的输入验证导致。

rss · The Hacker News · 7月16日 07:22

**背景**: Zoom Workplace 是广泛使用的视频电话套件。VDI Client 支持在虚拟桌面环境中使用，Meeting SDK 允许开发者将 Zoom 集成到自定义应用中。CVSS 9.8 分表示一个无需认证即可远程利用的关键漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.zoom.com/hc/en/article?id=zm_kb&sysparm_article=KB0063810">VDI releases and downloads - Zoom</a></li>
<li><a href="https://developers.zoom.us/docs/meeting-sdk/">Zoom Meeting SDK - Meeting SDK - Zoom Developer Docs</a></li>

</ul>
</details>

**标签**: `#Zoom`, `#security vulnerability`, `#patch`, `#account takeover`, `#Windows`

---

<a id="item-18"></a>
## [Claude Chrome 扩展漏洞允许点击劫持攻击](https://www.bleepingcomputer.com/news/security/claude-chrome-extension-flaw-lets-malicious-extensions-trigger-ai-actions/) ⭐️ 8.0/10

Anthropic 的 Claude for Chrome 扩展中存在一个点击劫持漏洞，恶意浏览器扩展可以模拟用户点击，未经同意触发预定义的 AI 操作，可能滥用对 Gmail、Google Docs 和 Salesforce 等已连接服务的访问权限。 该漏洞可能使攻击者代表用户执行未经授权的操作，例如阅读电子邮件或修改文档，危及多个服务中的敏感数据。这突显了拥有广泛权限的 AI 浏览器扩展的安全风险。 该漏洞涉及一种 UI 重定向（点击劫持）技术，恶意扩展通过覆盖透明元素来诱使 Claude 点击其自身界面。Anthropic 建议用户仅从可信来源安装扩展并审查权限。

rss · BleepingComputer · 7月16日 19:26

**背景**: Claude for Chrome 是一款实验性的浏览器扩展，可以随用户一起读取、点击和浏览网站。它通过 API 权限与 Gmail 和 Google Docs 等服务集成。点击劫持是一种攻击类型，用户被诱骗点击与其感知不同的内容，通常导致意外操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://chromewebstore.google.com/detail/claude/fcoeoabgfenejglbffodgkkbkcdhcgfn">Claude - Chrome Web Store</a></li>
<li><a href="https://support.anthropic.com/en/articles/12012173-getting-started-with-claude-for-chrome">Getting Started with Claude for Chrome | Anthropic Help Center</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Claude`, `#Chrome extension`, `#AI`

---

<a id="item-19"></a>
## [CISA 要求联邦机构在周六前修补 Oracle 漏洞](https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-actively-exploited-oracle-flaw-by-saturday/) ⭐️ 8.0/10

CISA 已要求联邦机构在本周六前修补 Oracle E-Business Suite 中一个已被积极利用的严重漏洞。 这一指令突显了针对广泛使用的企业财务应用程序的活跃攻击的严重性，使组织面临数据泄露的风险。 该漏洞可能为 CVE-2025-61882 或 CVE-2026-46817，可远程利用且无需认证，允许完全攻击受影响系统。

rss · BleepingComputer · 7月16日 10:56

**背景**: Oracle E-Business Suite 是一款综合性企业资源规划（ERP）软件，许多大型组织用于财务和运营管理。CISA 的有约束力操作指令要求联邦机构在规定时间内修补已知被利用的漏洞，以保护政府网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.oracle.com/security-alerts/alert-cve-2025-61882.html">Oracle Security Alerts CVE-2025-61882</a></li>
<li><a href="https://thehackernews.com/2026/06/oracle-e-business-suite-flaw-cve-2026.html">Oracle E-Business Suite Flaw CVE-2026-46817 Actively ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Oracle`, `#CISA`, `#patch management`

---

<a id="item-20"></a>
## [DFlash 让 Qwen3.6-27B 提速 2.2 倍且无质量损失](https://www.reddit.com/r/LocalLLaMA/comments/1uyay0w/dflash_makes_qwen36_27b_22x_faster_with_no/) ⭐️ 8.0/10

DFlash 是一种块扩散投机解码方法，在单张 RTX 6000 GPU 上的测试显示，它在处理重复性/结构化任务时能将 Qwen3.6-27B 模型的速度提升至基准的 2.2 倍，且输出质量没有任何下降。 这一优化显著提升了本地部署 LLM 的吞吐量，尤其有利于编码和结构化数据处理任务，使大型模型在不牺牲输出质量的前提下在消费级硬件上更加实用。 DFlash 能并行草拟 15 个 token，在 JSON 任务上达到 152 tok/s（3.4 倍加速），但在创意文本任务中可能因接受率低而低于基准（42 vs 44 tok/s）。与 DFlash 不同，MTP（多 token 预测）从未低于基准，更适合创意写作。

reddit · r/LocalLLaMA · /u/ElmBark · 7月16日 18:22

**背景**: 投机解码通过使用快速草稿模型提议 token，再由目标模型并行验证来加速 LLM 推理。DFlash 是一种块扩散模型，能够同时生成整个 token 块，而像 MTP 这样的自回归草稿器则是顺序预测少量 token。这使得 DFlash 在结构化输出（长 token 序列可预测）上特别快，但在创意文本（猜测常出错）上效果不佳。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2602.06036">[2602.06036] DFlash: Block Diffusion for Flash Speculative ... Boost Inference Performance up to 15x on NVIDIA Blackwell ... DFlash: Block Diffusion for Flash Speculative Decoding The next generation of speculative decoding: DFlash and Spec V2 DFlash: 3x faster LLM inference - baseten.co</a></li>
<li><a href="https://www.opensourceforu.com/2026/06/nvidia-open-sources-dflash-for-faster-llm-inference/">NVIDIA Open Sources DFlash for Faster LLM Inference</a></li>
<li><a href="https://github.com/z-lab/dflash">GitHub - z-lab/dflash: DFlash: Block Diffusion for Flash ...</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#DFlash`, `#speculative decoding`, `#Qwen`, `#optimization`

---