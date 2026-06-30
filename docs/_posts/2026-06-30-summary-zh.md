---
layout: default
title: "Horizon Summary: 2026-06-30 (ZH)"
date: 2026-06-30
lang: zh
---

> 从 66 条内容中筛选出 20 条重要资讯。

---

1. [vLLM v0.24.0 发布：支持 MiniMax-M3 并优化 DeepSeek-V4](#item-1)
2. [最高法院裁定地理围栏搜查令需受第四修正案保护](#item-2)
3. [关键 libssh2 CVE-2026-55200 漏洞的公开 PoC 已发布](#item-3)
4. [利用关键 SimpleHelp 漏洞部署 Djinn 窃取器](#item-4)
5. [谷歌 AI 同行评审系统处理约 1 万篇会议论文](#item-5)
6. [EML 树被证明是通用逼近器](#item-6)
7. [火箭实验室收购铱星公司达成里程碑交易](#item-7)
8. [WATaBoy 项目：将 Game Boy 指令即时编译到 WebAssembly，性能超越原生解释器](#item-8)
9. [CUDA 内核启动时 CPU 到 GPU 路径的深入解析](#item-9)
10. [欧洲 ISP 要求版权方为过度屏蔽负责](#item-10)
11. [Ornith-1.0：开放权重 LLM 通过自我脚手架实现编码 SOTA](#item-11)
12. [新发现：含大量零位的脆弱 RSA 密钥已在现实中使用](#item-12)
13. [Mustang Panda 利用 Zoho WorkDrive 攻击印度政府](#item-13)
14. [超过 23.6 万个 DCloud Uni-App 网站用于加密货币诈骗](#item-14)
15. [微软移除 119 个利用隐写术的恶意 Edge 扩展](#item-15)
16. [被劫持的 npm 和 Go 包利用 VS Code 任务部署 Python 信息窃取器](#item-16)
17. [黑客利用 Oracle E-Business Suite 关键漏洞](#item-17)
18. [CISA 将 SimpleHelp 认证绕过漏洞列入已知利用漏洞目录](#item-18)
19. [恶意 Perplexity Chrome 扩展劫持搜索](#item-19)
20. [Gamaredon 利用新恶意软件和云服务滥用扩大对乌克兰攻击](#item-20)

---

<a id="item-1"></a>
## [vLLM v0.24.0 发布：支持 MiniMax-M3 并优化 DeepSeek-V4](https://github.com/vllm-project/vllm/releases/tag/v0.24.0) ⭐️ 9.0/10

vLLM v0.24.0 版本增加了对 MiniMax-M3 模型的支持，并对 DeepSeek-V4 进行了大量性能优化，同时还引入了流式解析引擎、DiffusionGemma 支持以及完善的 Rust 前端。 此版本展示了 vLLM 社区驱动的快速开发，带来了前沿模型支持和显著的推理效率提升，惠及部署大语言模型的开发者和企业。 该版本包含来自 256 位贡献者（其中 77 位新贡献者）的 571 次提交，为 MiniMax-M3 引入了 MXFP4 和 FP8 稀疏 GQA 支持，并通过 FlashInfer 稀疏索引缓存和集群协作 topK 内核等优化了 DeepSeek-V4。

github · khluu · 6月29日 19:41

**背景**: vLLM 是一个高性能的大语言模型推理引擎，旨在实现低延迟和高吞吐量。该版本延续了其支持最新模型和优化性能的趋势，利用 MXFP4 量化和 FlashInfer 内核等技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/RakshitAralimatti/learn-ai-with-me">What’s MXFP4? The 4-Bit Secret Powering OpenAI’s GPT‑OSS Models on Modest Hardware</a></li>
<li><a href="https://github.com/flashinfer-ai/flashinfer">GitHub - flashinfer -ai/ flashinfer : FlashInfer : Kernel Library for LLM...</a></li>
<li><a href="https://trackai.dev/tracks/performance/latency-ttft/">Latency & TTFT | TrackAI</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#release`, `#model support`, `#performance optimization`

---

<a id="item-2"></a>
## [最高法院裁定地理围栏搜查令需受第四修正案保护](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

美国最高法院裁定，地理围栏搜查令（迫使科技公司提供特定区域内设备位置数据）需受第四修正案保护，必须基于可能理由并取得搜查令。 这一里程碑式的决定显著限制了执法部门在无司法监督下获取批量位置数据的能力，为数字隐私树立了关键先例，并可能影响自动车牌识别器等其他监控技术。 此案涉及谷歌的 Sensorvault，法院裁定政府通过地理围栏搜查令获取历史基站位置信息构成第四修正案下的搜查行为。

hackernews · cdrnsf · 6月29日 15:54 · [社区讨论](https://news.ycombinator.com/item?id=48720924)

**背景**: 地理围栏搜查令是一种搜查令，迫使谷歌等公司识别在指定时间段内位于特定地理区域内的所有移动设备。第四修正案保护个人免受不合理的搜查和扣押，该裁决澄清了这种广泛的定位数据请求需要基于可能理由的搜查令。这一决定解决了现代监控能力与宪法隐私保护之间的紧张关系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant - Wikipedia</a></li>
<li><a href="https://gizmodo.com/in-a-win-for-privacy-supreme-court-rules-geofence-warrants-are-a-search-under-4th-amendment-2000778986">In a Win for Privacy, Supreme Court Rules Geofence Warrants Are a ...</a></li>

</ul>
</details>

**社区讨论**: 评论者提到了像彼得雷乌斯事件这样的历史案例，展示了地理定位技术，并提出了该裁决对 Flock 摄像头等产品的影响的担忧。一些人惊讶于巴雷特大法官加入了少数派的反对意见，而另一些人则称赞该决定是隐私的胜利。

**标签**: `#privacy`, `#supreme court`, `#geofence warrants`, `#fourth amendment`, `#law enforcement`

---

<a id="item-3"></a>
## [关键 libssh2 CVE-2026-55200 漏洞的公开 PoC 已发布](https://thehackernews.com/2026/06/public-poc-released-for-critical.html) ⭐️ 9.0/10

针对 libssh2 中的关键漏洞 CVE-2026-55200，已公开了一个概念验证漏洞利用代码。该漏洞允许恶意 SSH 服务器在连接客户端上破坏内存，无需认证或用户交互即可可能导致远程代码执行。 该漏洞至关重要，因为 libssh2 被广泛用于客户端应用程序的 SSH 连接，成功利用可使攻击者在无需任何凭据的情况下远程入侵客户端机器。公开的 PoC 增加了攻击风险，敦促用户尽快修补。 CVE-2026-55200 影响 libssh2 1.11.1 及之前的所有版本，CVSS 4.0 评分为 9.2。该漏洞位于客户端，意味着恶意或被入侵的 SSH 服务器可攻击任何使用 libssh2 的连接客户端。

rss · The Hacker News · 6月29日 07:06

**背景**: libssh2 是一个客户端 C 库，实现了 SSH2 协议，被许多应用程序用于安全远程访问和文件传输。它支持 SCP、SFTP 和端口转发等功能。与服务器端的 SSH 实现不同，libssh2 纯粹是客户端库，因此该漏洞针对的是连接到不可信 SSH 服务器的客户端机器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/libssh2/libssh2">GitHub - libssh2/libssh2: the SSH library · GitHub</a></li>
<li><a href="https://github.com/libssh2/libssh2/releases">Releases · libssh2/libssh2</a></li>
<li><a href="https://www.freshports.org/security/libssh2/">FreshPorts -- security/libssh2: Library implementing the SSH2 protocol</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#libssh2`, `#exploit`, `#SSH`

---

<a id="item-4"></a>
## [利用关键 SimpleHelp 漏洞部署 Djinn 窃取器](https://www.bleepingcomputer.com/news/security/hackers-exploit-critical-simplehelp-flaw-deploy-new-djinn-infostealer-taskweaver-malware/) ⭐️ 9.0/10

攻击者正在积极利用 SimpleHelp 远程支持软件中的一个关键漏洞（CVE-2026-48558），以部署此前未记录的跨平台信息窃取器 Djinn Stealer，该恶意软件针对 Windows、macOS 和 Linux。 这具有重要意义，因为它引入了一个具有广泛平台覆盖范围的新恶意软件家族，可能危及开发者和 AI 工具用户的敏感凭据，并凸显了远程支持软件漏洞的风险。 Djinn Stealer 专注于窃取 AI 开发工具的凭据以及广泛的开发者和基础设施凭据。该入侵链还涉及一个此前未发现的恶意软件样本 TaskWeaver，它是一个 Node.js 后门。

rss · BleepingComputer · 6月29日 14:00

**背景**: SimpleHelp 是 IT 专业人员和 MSP 使用的远程支持和远程访问软件，用于跨平台控制和监控设备。远程支持工具通常是攻击者的目标，因为它们通常具有广泛的系统访问权限。像 CVE-2026-48558 这样的关键漏洞允许远程代码执行，使攻击者能够安装恶意软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-exploit-critical-simplehelp-flaw-deploy-new-djinn-infostealer-taskweaver-malware/">Critical SimpleHelp flaw exploited to deploy new stealer malware</a></li>
<li><a href="https://blackpointcyber.com/blog/a-djinn-in-the-machine-taskweavers-node-js-intrusion-chain/">A Djinn in the Machine: TaskWeaver’s Node.js... - Blackpoint Cyber</a></li>
<li><a href="https://simple-help.com/">SimpleHelp | Remote Support Software by SimpleHelp</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#malware`, `#infostealer`, `#cross-platform`

---

<a id="item-5"></a>
## [谷歌 AI 同行评审系统处理约 1 万篇会议论文](https://www.reddit.com/r/MachineLearning/comments/1uio9rb/googles_agentic_peerreviewer_handled_10k_papers/) ⭐️ 9.0/10

谷歌在 ICML 和 STOC 会议上部署了一个代理型 AI 同行评审系统，在 30 分钟内处理了约 1 万篇论文，新发表的正式论文显示，该系统比零样本提示多检测出 34%的数学错误。 这表明了一种可扩展的 AI 辅助科学同行评审方法，可能减轻人类评审员的负担并在大规模评审中提高错误检测能力。它为 AI 融入顶级会议正式评审流程开创了先例。 该系统被称为“代理型”，意味着它可以自主规划和执行评审流程。改进幅度是与零样本提示相比，零样本提示下 AI 没有先例，这突出了结构化代理工作流的优势。

reddit · r/MachineLearning · /u/Justgototheeffinmoon · 6月29日 10:05

**背景**: 零样本提示是一种技术，即要求大型语言模型在没有具体示例或事先训练的情况下执行任务。代理型 AI 系统更进一步，通过整合规划、工具使用和多步推理来完成复杂目标。在同行评审的背景下，代理系统可以将评审分解为子任务，如检查数学正确性、验证参考文献和总结贡献。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-shot_prompting">Zero-shot prompting</a></li>
<li><a href="https://www.ibm.com/think/topics/zero-shot-prompting">What is zero-shot prompting? - IBM</a></li>

</ul>
</details>

**标签**: `#AI`, `#peer review`, `#machine learning`, `#scientific process`, `#Google`

---

<a id="item-6"></a>
## [EML 树被证明是通用逼近器](https://www.reddit.com/r/MachineLearning/comments/1uipl1t/eml_trees_are_universal_approximators_r/) ⭐️ 9.0/10

一篇新论文证明，由初等函数 exp(x) - ln(y) 构成的 EML 树能够逼近一般函数空间中的任意函数，类似于神经网络的通用逼近定理。 这为使用 EML 树作为通用函数逼近器奠定了严格的理论基础，扩展了符号回归、模拟计算和机器学习的工具集。 该证明依赖于使用 EML 模块显式构造二元运算、多项式和双曲正切函数，并通过基于符号的分解处理了对数定义域限制等技术问题。

reddit · r/MachineLearning · /u/JoeGermany · 6月29日 11:16

**背景**: EML 函数定义为 eml(x,y)=exp(x)-ln(y)，最近被证明可以通过组合生成所有初等函数。通用逼近定理 (UAT) 指出某类函数（如神经网络）可以在紧集上任意好地逼近任何连续函数。本文将 UAT 推广到了 EML 树。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.23179">[2606.23179] EML Trees Are Universal Approximators</a></li>
<li><a href="https://arxiv.org/html/2603.21852v2">All elementary functions from a single operator</a></li>
<li><a href="https://en.wikipedia.org/wiki/Universal_approximation_theorem">Universal approximation theorem - Wikipedia</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#universal approximation`, `#EML trees`, `#function approximation`, `#theory`

---

<a id="item-7"></a>
## [火箭实验室收购铱星公司达成里程碑交易](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 8.0/10

火箭实验室宣布收购铱星通信公司，打造一家完全整合的太空通信与发射公司。 此次垂直整合使火箭实验室能够提供从发射到星座运营的端到端卫星服务，可能重塑航天行业的竞争格局。 该交易将火箭实验室的运载火箭和卫星平台专长与铱星公司现有的低轨星座（66 颗在轨卫星和全球通信服务）相结合。

hackernews · everfrustrated · 6月29日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48719485)

**背景**: 铱星公司运营着独特的低轨卫星星座，提供全球语音和数据覆盖，包括卫星电话和物联网连接。火箭实验室以其 Electron 火箭和 Photon 卫星平台闻名，一直在扩展其太空系统能力。此次收购使火箭实验室能够利用铱星公司已建立的网络和客户群。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Iridium_satellite_constellation">Iridium satellite constellation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rocket_Lab_Photon">Rocket Lab Photon - Wikipedia</a></li>
<li><a href="https://www.iridium.com/network">Network | Iridium</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一。一些人认为这是确保发射需求的战略举措，类似于 SpaceX 利用星链。其他人质疑轨道兼容性，指出铱星卫星在低轨但倾角较高，而 Electron 目前发射至较低轨道。还有人担心火箭实验室失去新西兰身份。

**标签**: `#space`, `#acquisition`, `#satellite communications`, `#Rocket Lab`, `#Iridium`

---

<a id="item-8"></a>
## [WATaBoy 项目：将 Game Boy 指令即时编译到 WebAssembly，性能超越原生解释器](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

一个名为 WATaBoy 的项目证明，将 Game Boy CPU 指令即时编译为 WebAssembly 的性能可以超越原生解释器，在浏览器中实现更快的仿真速度。 这种方法使得无需插件即可在浏览器中实现高性能的 Game Boy 仿真，并突显了 WebAssembly 在典型 Web 应用之外的计算密集型任务中的潜力。 据报道，在此工作负载下，Firefox 比 Chrome 和 Safari 慢 25%，该项目还因出自本科生之手而引人注目。JIT 方法克服了通常约 1000% 的解释开销。

hackernews · energeticbark · 6月29日 15:02 · [社区讨论](https://news.ycombinator.com/item?id=48720190)

**背景**: 传统的 Game Boy 仿真使用解释或提前编译。JIT 编译在运行时将频繁执行的代码转换为原生机器码，从而减少开销。WebAssembly (WASM) 是一种低级二进制格式，在浏览器中以接近原生的速度运行，大多数实现采用 JIT 或 AOT 编译。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.adafruit.com/2019/12/31/emulating-the-original-gameboys-cpu-gameboy-nintendo-gaming-nenharma82/">Emulating the Original Gameboy ’s CPU # Gameboy #Nintendo...</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly - Wikipedia</a></li>
<li><a href="https://hacks.mozilla.org/2017/02/what-makes-webassembly-fast/">What makes WebAssembly fast? – Mozilla Hacks - the Web developer blog</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，16 年前曾有人尝试类似的技术（使用 Dolphin 和 LLVM），但速度很慢。浏览器之间的性能差异（Firefox 较慢）引起了好奇。有评论者认为，这一结果在预料之中，因为 WASM 开销（约 20%）远低于解释器开销（约 1000%）。

**标签**: `#JIT compilation`, `#WebAssembly`, `#Game Boy`, `#emulation`, `#performance`

---

<a id="item-9"></a>
## [CUDA 内核启动时 CPU 到 GPU 路径的深入解析](https://fergusfinn.com/blog/what-happens-when-you-run-a-gpu-kernel/) ⭐️ 8.0/10

一篇博客文章详细描述了从 CUDA 内核启动到 GPU 硬件的完整路径，涵盖了驱动程序交互、门铃寄存器和命令队列管理。它揭示了高级编程与底层操作之间的桥梁。 这次技术深度剖析帮助开发者理解 GPU 编程的性能和调试细节。它还引发了社区关于内核优化和开放文档可用性的讨论。 文章解释了 PCIe BAR 空间中的门铃寄存器和队列元数据描述符（QMD）的作用。一位评论者指出控制码是表查找，而不仅仅是控制字中的位。

hackernews · mezark · 6月29日 13:11 · [社区讨论](https://news.ycombinator.com/item?id=48718863)

**背景**: 在 CUDA 中，启动内核不仅涉及 GPU 执行，还包括 CPU 端的设置：驱动程序构建命令队列并通过门铃寄存器通知 GPU。大多数解释聚焦于 block 和 warp，跳过了这个关键的 CPU 到 GPU 路径。理解这一路径对于优化启动延迟和调试驱动级问题至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/1979637060794095610">PCIe Doorbell Register 为何设计为 Write-Only：架构原理与技术解析</a></li>
<li><a href="https://arxiv.org/html/2604.26889v1">Revealing NVIDIA Closed-Source Driver Command Streams for CPU-GPU ...</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了对门铃寄存器和 QMD 的解释，指出它将 CUDA 语法与硬件提交联系起来。一位用户强调 NVIDIA 的 GitHub 上存在开放的 GPU 文档。另一位观察者指出，专门从事内核优化的公司可能会受到开源解决方案的挑战。

**标签**: `#cuda`, `#gpu`, `#nvidia`, `#hardware`, `#technical-deep-dive`

---

<a id="item-10"></a>
## [欧洲 ISP 要求版权方为过度屏蔽负责](https://torrentfreak.com/european-isps-want-rightsholders-held-accountable-for-overblocking-damage/) ⭐️ 8.0/10

欧洲互联网服务提供商（ISP）呼吁对因过度屏蔽而导致合法内容无法访问的版权方追究法律责任。 这可能会改变互联网治理中的权力平衡，减少滥用删除请求对合法言论的审查和对公众访问的损害。 过度屏蔽指的是由于过于宽泛的法院命令或自动化删除系统导致非侵权内容也被屏蔽，ISP 认为版权方应承担由此产生的损害责任。

hackernews · Brajeshwar · 6月29日 16:07 · [社区讨论](https://news.ycombinator.com/item?id=48721072)

**背景**: 过度屏蔽是一个众所周知的问题，版权执法机制会无意中屏蔽合法内容。在欧洲，版权方经常获得针对 ISP 的广泛屏蔽令，从而导致过度屏蔽。辩论的焦点在于版权方是否应为其执法行为造成的损害负责。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stimson.org/2025/who-controls-your-internet-the-debate-over-dns-blocking/">Who Controls Your Internet? The Debate Over DNS Blocking ...</a></li>
<li><a href="https://www.medianama.com/2026/03/223-cloudflare-legal-chief-piracy-injunctions-overblocking/">Cloudflare legal Chief on Piracy, Injunctions and Overblocking</a></li>

</ul>
</details>

**社区讨论**: 社区评论强烈支持这一举措。bradley13 指出美国缺乏责任追究，londons_explore 强调公民浪费的时间才是真正的损害。Arubis 对时机表示谨慎，认为模型训练公司可能会利用这一转变。

**标签**: `#copyright`, `#internet governance`, `#ISPs`, `#censorship`, `#policy`

---

<a id="item-11"></a>
## [Ornith-1.0：开放权重 LLM 通过自我脚手架实现编码 SOTA](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce 发布了 Ornith-1.0，一个开放权重的 LLM 系列（MIT 许可），通过新颖的自我脚手架技术，在编码基准测试中达到了同类开源模型的最优性能。该系列包含从 9B 到 397B 参数的多个变体，基于 Gemma 4 和 Qwen 3.5 构建。 这一发布显著推动了开放权重编码助手的发展，使得在宽松许可下实现强大的本地自主编码成为可能。它可能加速自主编码工具的研发并减少对专有模型的依赖。 该模型采用了自我脚手架技术，即模型自己编写执行脚手架，在多步骤编码任务上表现强劲。早期用户测试显示，它能流畅处理复杂的代码库查询和工具调用。

rss · Simon Willison · 6月29日 16:17

**背景**: 自我脚手架是指 LLM 生成自己的工作流程代码（脚手架）来分解复杂任务并调用工具，从而提升代理性能。GGUF 是一种专为在消费级硬件上进行本地 LLM 推理而优化的文件格式。MoE（混合专家）是一种每次只激活部分参数的架构，平衡了性能与效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://www.explainx.ai/blog/ornith-1-0-self-scaffolding-agentic-coding-llm-2026">Ornith-1.0: Self-Scaffolding Open Models for Agentic Coding</a></li>

</ul>
</details>

**标签**: `#LLM`, `#coding`, `#open-weight`, `#agentic`, `#benchmark`

---

<a id="item-12"></a>
## [新发现：含大量零位的脆弱 RSA 密钥已在现实中使用](https://www.schneier.com/blog/archives/2026/06/factoring-rsa-keys-with-many-zeros.html) ⭐️ 8.0/10

Trail of Bits 与 badkeys 项目的研究人员发现了一类新的弱 RSA 密钥，其模数包含大量零位，称为“短袖”密钥，并已在现实世界的 TLS、SSH 和 PGP 部署中发现它们。 这一发现揭示了 RSA 密钥生成中一个以前未知的漏洞，攻击者可以利用该漏洞分解此类密钥，可能危及互联网上加密通信和数字签名的安全性。 研究人员使用多项式技术分解稀疏模数，而 badkeys 项目收集的数百万个公钥数据集表明，这些弱密钥不仅存在于理论中，而且在实践中确实存在。

rss · Schneier on Security · 6月29日 16:05

**背景**: RSA 是一种广泛使用的公钥密码系统，其安全性依赖于分解大合数的难度。具有大量零位的模数（稀疏模数）可以使用研究人员开发的专门算法更容易地被分解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.trailofbits.com/2026/06/12/factoring-short-sleeve-rsa-keys-with-polynomials/">Factoring "short-sleeve" RSA keys with polynomials - The Trail of Bits Blog</a></li>
<li><a href="https://github.com/badkeys/badkeys">GitHub - badkeys/badkeys: Tool to find common vulnerabilities in cryptographic public keys · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/RSA_(cryptosystem)">RSA cryptosystem - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#RSA`, `#security`, `#vulnerability`, `#research`

---

<a id="item-13"></a>
## [Mustang Panda 利用 Zoho WorkDrive 攻击印度政府](https://thehackernews.com/2026/06/mustang-panda-uses-zoho-workdrive-as.html) ⭐️ 8.0/10

与中国有关联的 Mustang Panda 组织正在针对印度政府和水电目标开展两场行动，部署了名为 ZOHOMURK 的新型植入程序，该程序利用 Zoho WorkDrive 作为命令与控制信道。 这标志着 Mustang Panda 首次使用 Zoho WorkDrive 作为 C2 基础设施，通过混入合法云流量实现隐蔽通信。针对印度政府和关键能源基础设施的行动凸显了持续的地缘政治网络间谍活动。 ZOHOMURK 植入程序通过硬编码的客户端 ID、密钥和刷新令牌滥用 Zoho WorkDrive 的 OAuth2 API 来获取命令并窃取数据。Acronis 威胁研究部门在印度政府网络中发现了活跃的入侵，包括高级行政人员的机器。

rss · The Hacker News · 6月29日 15:03

**背景**: Mustang Panda 是一个至少自 2012 年以来活跃的、基于中国的高级持续性威胁（APT）组织，以全球范围内的政府、外交和非政府组织为目标。Zoho WorkDrive 是一种云存储服务，当被用作命令通道时，通过模仿正常云流量帮助恶意软件逃避检测。这种被称为“云端寄生”的技术也曾在其他 APT 组织如 ScarCruft 中出现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.acronis.com/en/tru/posts/mustang-panda-targets-indias-government-and-energy-sectors/">Mustang Panda targets India's government and energy sectors with...</a></li>
<li><a href="https://attack.mitre.org/groups/G0129/">Mustang Panda - MITRE ATT&CK®</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#espionage`, `#malware`, `#cloud security`, `#government attacks`

---

<a id="item-14"></a>
## [超过 23.6 万个 DCloud Uni-App 网站用于加密货币诈骗](https://thehackernews.com/2026/06/236000-dcloud-uni-app-sites-used-in.html) ⭐️ 8.0/10

Infoblox 发现超过 23.6 万个网站使用基于 DCloud Uni-App 框架构建的模板，用于运营加密货币诈骗、钓鱼攻击和钱包盗取器。 这一发现揭示了一个合法的开源开发框架被大规模武器化用于金融欺诈，对全球网络安全和在线信任构成重大威胁。 这些诈骗网站包括虚假加密货币交易所、多语言杀猪盘、WhatsApp 钓鱼网络和品牌仿冒页面，全部由 DCloud Uni-App 模板驱动。

rss · The Hacker News · 6月29日 11:57

**背景**: DCloud Uni-App 是一个中国开源跨平台框架（类似于 React Native 或 Flutter），允许开发者通过单一 Vue.js 代码库为移动端、桌面端和网页端构建应用。杀猪盘诈骗通过先与受害者建立信任，再引诱其进行虚假投资；钱包盗取器则诱骗用户授权交易，从而清空其加密货币钱包。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.infoblox.com/blog/threat-intelligence/from-san-pedro-to-salinas-how-a-chinese-framework-dcloud-uni-app-powers-a-global-scam-economy/">DCloud Uni-App: One Framework, 236,000+ Scam Sites</a></li>
<li><a href="https://github.com/dcloudio/uni-app">GitHub - dcloudio/uni-app: A cross-platform framework using ... 236,000 DCloud Uni-App Sites Used in Crypto Scams, Phishing ... DCloud Uni-App Framework Powers 236,000+ Scam ... - GBHackers DCloud Uni-App Scam Network Powers RainbowEx-Style Crypto ... Chinese Development Framework Linked to Global Scam ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#crypto scams`, `#phishing`, `#open-source framework`, `#DCloud Uni-App`

---

<a id="item-15"></a>
## [微软移除 119 个利用隐写术的恶意 Edge 扩展](https://thehackernews.com/2026/06/microsoft-removes-119-edge-extensions.html) ⭐️ 8.0/10

微软从 Edge 扩展商店移除了 119 个恶意扩展，这些扩展利用隐写术将恶意代码隐藏在图片和字体文件中，用于窃取凭据和进行广告欺诈。 这一名为 StegoAd 的行动代表了浏览器扩展中大规模且新颖的隐写术应用，影响了数百万用户，凸显了加强扩展安全性的必要性。 微软将 119 个扩展与一个至少自 2021 年以来活跃的威胁行为者关联；这些扩展在安装后会静置数天，然后激活以窃取凭据并进行广告欺诈。

rss · The Hacker News · 6月29日 08:32

**背景**: 隐写术是一种将数据隐藏在其他媒体（如图像或音频）中的技术，以避免被检测。在恶意软件中，隐写恶意软件利用这种方法隐藏有效载荷或命令，绕过不深入检查媒体文件的传统安全工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stegomalware">Stegomalware - Wikipedia</a></li>
<li><a href="https://www.sentinelone.com/blog/hiding-code-inside-images-malware-steganography/">What is Steganography? - Protecting from Malicious Images</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#Edge`, `#steganography`, `#adware`

---

<a id="item-16"></a>
## [被劫持的 npm 和 Go 包利用 VS Code 任务部署 Python 信息窃取器](https://thehackernews.com/2026/06/hijacked-npm-and-go-packages-use-vs.html) ⭐️ 8.0/10

JFrog 的安全研究人员发现，至少有两个被劫持的 npm 包和一组 Go 包利用 Visual Studio Code 任务在 Windows、Linux 和 macOS 系统上部署基于 Python 的信息窃取器。 此攻击利用 VS Code 任务作为新颖的执行载体，绕过了 npm 生命周期脚本的保护，并针对所有主流操作系统，凸显了软件供应链攻击的日益复杂化。 该攻击避开了常见的 npm 执行路径（如生命周期脚本），以保持与 npm v12 安全加固的兼容性，转而使用恶意的 VS Code tasks.json 文件来执行命令并部署有效载荷。

rss · The Hacker News · 6月29日 05:36

**背景**: npm 包可以包含生命周期脚本（如 preinstall、postinstall），这些脚本在安装时运行，常被攻击者滥用。Visual Studio Code 支持任务配置文件（tasks.json），当打开项目时可执行任意命令。这次活动劫持了合法包并添加恶意 VS Code 任务以部署信息窃取器，绕过了一些安全措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.shield53.com/supply-chain-sabotage-hijacked-npm-and-go-packages-deploy-cross-platform-python-infostealer/">Supply Chain Sabotage: Hijacked npm and Go Packages Deploy ...</a></li>
<li><a href="https://www.threatlocker.com/blog/malicious-vs-code-tasks-json-abuse-enables-multi-stage-infostealer-deployment">VS Code tasks.json abuse enables multi-stage infostealer deployment</a></li>
<li><a href="https://medium.com/@kyle_martin/understanding-and-protecting-against-malicious-npm-package-lifecycle-scripts-8b6129619d7c">Understanding and protecting against malicious npm ... | Medium</a></li>

</ul>
</details>

**标签**: `#security`, `#supply chain`, `#npm`, `#Go`, `#infostealer`

---

<a id="item-17"></a>
## [黑客利用 Oracle E-Business Suite 关键漏洞](https://www.bleepingcomputer.com/news/security/new-oracle-e-business-suite-flaw-now-exploited-in-attacks/) ⭐️ 8.0/10

攻击者正在积极利用 Oracle E-Business Suite 中 Oracle Payments 组件的一个关键漏洞（CVE-2026-46817），据威胁情报公司 Defused 报告。 这对使用 Oracle E-Business Suite 进行财务操作的组织构成直接威胁，因为未经身份验证的远程攻击者可以接管系统。高达 9.8 的 CVSS 评分凸显了立即打补丁的紧迫性。 该漏洞影响 Oracle E-Business Suite 版本 12.2.3 至 12.2.15，允许未经身份验证的攻击者通过 HTTP 访问 File Transmission 端点。Oracle 已发布补丁，缓解措施包括阻止对该端点的外部访问。

rss · BleepingComputer · 6月29日 13:46

**背景**: Oracle E-Business Suite 是一个全面的企业资源规划（ERP）软件套件，大型组织用于财务、供应链和人力资源。Oracle Payments 组件处理支付交易。CVE-2026-46817 是一个关键缺陷，可能导致 Payments 模块被完全接管。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Oracle_E-Business_Suite">Oracle E-Business Suite</a></li>
<li><a href="https://nvd.nist.gov/vuln/detail/CVE-2026-46817">NVD - CVE-2026-46817</a></li>
<li><a href="https://app.opencve.io/cve/CVE-2026-46817">CVE-2026-46817 - Vulnerability Details - OpenCVE</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#oracle`, `#exploitation`, `#CVE`

---

<a id="item-18"></a>
## [CISA 将 SimpleHelp 认证绕过漏洞列入已知利用漏洞目录](https://www.cisa.gov/news-events/alerts/2026/06/29/cisa-adds-one-known-exploited-vulnerability-catalog) ⭐️ 7.0/10

2026 年 6 月 29 日，CISA 将 CVE-2026-48558（SimpleHelp 认证绕过漏洞）添加到其已知利用漏洞（KEV）目录中，原因是存在主动利用的证据。 此次添加凸显了远程支持软件漏洞的风险上升，并强化了快速修复的必要性，特别是对于受 BOD 26-04 约束的联邦机构。 CVE-2026-48558 是 SimpleHelp 远程支持软件中的一个认证绕过漏洞。CISA 的 BOD 26-04 要求联邦机构在三天内修复 KEV 目录中针对公开暴露资产的漏洞。

rss · CISA Cybersecurity Advisories · 6月29日 12:00

**背景**: CISA 的已知利用漏洞（KEV）目录是经过确认已被威胁行为者积极利用的漏洞列表。2026 年 6 月发布的约束性操作指令 26-04（BOD 26-04）要求联邦民事行政部门机构优先修补高风险漏洞，特别是 KEV 目录中涉及公开暴露资产的漏洞。SimpleHelp 提供远程支持和访问软件，常用于 IT 专业人员和 MSP。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simple-help.com/">SimpleHelp | Remote Support Software by SimpleHelp</a></li>
<li><a href="https://content.govdelivery.com/accounts/USDHSCISA/bulletins/41b445a">CISA Releases Binding Operational Directive 26-04 on ...</a></li>
<li><a href="https://cybersecuritynews.com/cisa-patch-vulnerabilities-3-days/">CISA Requires Federal Agencies to Patch Critical ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#CVE-2026-48558`, `#CISA`, `#vulnerability management`, `#exploited vulnerability`

---

<a id="item-19"></a>
## [恶意 Perplexity Chrome 扩展劫持搜索](https://thehackernews.com/2026/06/malicious-perplexity-chrome-extension.html) ⭐️ 7.0/10

微软发现了一个伪装成 Perplexity AI 的恶意 Chrome 扩展，它拦截了搜索查询和地址栏输入，将数据通过攻击者控制的服务器转发。谷歌在负责任披露后将该扩展从 Chrome 网上应用店移除。 此事件凸显了浏览器扩展中的供应链风险，因为用户信任了一个看似合法的 AI 工具。它强调了需要更严格的扩展审查流程和用户警惕。 该扩展记录了地址栏中的每次查询和按键，将用户重定向到真实的搜索结果以逃避检测。其名称借用了 Perplexity，但具体名称未公开。

rss · The Hacker News · 6月29日 18:40

**背景**: 浏览器扩展可以访问敏感用户数据，如浏览历史和搜索查询。恶意扩展通常冒充流行工具，诱骗用户授予权限，从而导致数据窃取或监控。

**标签**: `#security`, `#chrome-extension`, `#phishing`, `#supply-chain-attack`, `#privacy`

---

<a id="item-20"></a>
## [Gamaredon 利用新恶意软件和云服务滥用扩大对乌克兰攻击](https://thehackernews.com/2026/06/gamaredon-expands-ukraine-attacks-with.html) ⭐️ 7.0/10

ESET 观察到俄罗斯 APT 组织 Gamaredon 在 2025 年全年针对乌克兰新目标发起了 35 次不同的鱼叉式网络钓鱼活动，其中大部分发生在下半年，使用了新的恶意软件和云服务滥用技术。 Gamaredon 战术的持续演变凸显了对乌克兰的持久网络威胁，并表明该组织具备适应能力，对政府和民用基础设施构成风险。 这些活动主要发生在 2025 年下半年，ESET 的发现表明 Gamaredon 不断扩充其恶意软件库，并依赖云服务进行指挥和控制。

rss · The Hacker News · 6月29日 11:40

**背景**: Gamaredon，也称为 Primitive Bear 或 ACTINIUM，是一个至少自 2013 年以来活跃的俄罗斯国家资助的高级持续性威胁（APT）组织。它持续将乌克兰和北约实体作为目标，利用鱼叉式网络钓鱼和定制恶意软件进行网络间谍活动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.talosintelligence.com/gamaredonactivities/">Gamaredon - When nation states don’t pay all the bills</a></li>
<li><a href="https://hunt.io/malware-families/apt-gamaredon">Gamaredon APT : Persistent Russian Cyber Espionage</a></li>
<li><a href="https://brandefense.io/blog/gamaredon-group-2025/">Gamaredon Group : A Persistent Russian Espionage... - Brandefense</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#APT`, `#malware`, `#Ukraine`, `#cloud security`

---