---
layout: default
title: "Horizon Summary: 2026-07-16 (ZH)"
date: 2026-07-16
lang: zh
---

> 从 69 条内容中筛选出 20 条重要资讯。

---

1. [Stripe 与 Advent 联合出价 530 亿美元收购 PayPal](#item-1)
2. [GPT-Red：通过自我对弈实现 AI 鲁棒性](#item-2)
3. [研究员在周二补丁后发布 Windows 零日漏洞 PoC LegacyHive](#item-3)
4. [Cursor 漏洞：恶意仓库可静默执行代码](#item-4)
5. [ExLlamaV3 v1.0.0：本地 LLM 推理的重大性能升级](#item-5)
6. [Thinking Machines 发布 Inkling 开源权重多模态模型](#item-6)
7. [Telegram 数据中心谜团揭秘](#item-7)
8. [Firefox 在 WebAssembly 中运行：完整浏览器渲染到 Canvas](#item-8)
9. [Claude web_fetch 工具被绕过泄露用户记忆](#item-9)
10. [傅里叶像素让屏幕充当摄像头](#item-10)
11. [CUDA 13.3 引入无进位乘法以加速密码学](#item-11)
12. [模型路由：机器学习部署中的隐藏复杂性](#item-12)
13. [CISA 将两个正在被利用的漏洞加入 KEV 目录](#item-13)
14. [TuxBot v3 进化版：LLM 辅助的物联网僵尸网络](#item-14)
15. [OkoBot 恶意软件通过助记词钓鱼攻击 Ledger 和 Trezor](#item-15)
16. [Firefox、Chrome、Adobe、VMware 修补严重安全漏洞](#item-16)
17. [AsyncAPI npm 包被植入僵尸网络恶意软件](#item-17)
18. [两个 SonicWall SMA 1000 零日漏洞被利用，其中一个可执行管理员命令](#item-18)
19. [Zoom 警告存在严重账户劫持漏洞](#item-19)
20. [AI 漏洞自动贩卖机自动发现零日漏洞](#item-20)

---

<a id="item-1"></a>
## [Stripe 与 Advent 联合出价 530 亿美元收购 PayPal](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 9.0/10

据消息人士称，支付公司 Stripe 与私募股权公司 Advent International 联合提出以超过 530 亿美元的价格收购 PayPal。 这笔收购将整合主要的在线支付平台，可能减少竞争，并影响依赖这些服务的数百万用户和企业。 该报价对 PayPal 的估值超过 530 亿美元，若交易完成，Stripe、PayPal、Venmo、Braintree 和 Xoom 将同属一家公司，引发反垄断担忧。

hackernews · rvz · 7月15日 03:32 · [社区讨论](https://news.ycombinator.com/item?id=48915953)

**背景**: Stripe 是面向互联网企业的领先在线支付处理平台，而 PayPal 是广泛使用的数字钱包和支付系统。两家公司在在线支付领域存在竞争。如此规模的合并将创建一个在非面对面交易中的主导者。

**社区讨论**: 评论者对竞争减少、费用可能上涨以及 Stripe 对某些行业（如大麻和成人内容）的限制政策表示强烈担忧。一些人担心反垄断障碍以及是否需要剥离 Venmo 或 Braintree 等资产。

**标签**: `#fintech`, `#payments`, `#acquisition`, `#competition`, `#stripe`

---

<a id="item-2"></a>
## [GPT-Red：通过自我对弈实现 AI 鲁棒性](https://openai.com/index/unlocking-self-improvement-gpt-red) ⭐️ 9.0/10

OpenAI 推出了 GPT-Red，这是一个自动化的红队测试系统，通过自我对弈生成对抗性提示，以提升 AI 在提示注入和安全性对齐方面的鲁棒性。 这一进展通过自动化发现漏洞直接应对 AI 安全的关键挑战，有望减少红队测试所需的人工成本，并使模型对攻击更具鲁棒性。 GPT-Red 利用自我对弈机制，AI 同时扮演攻击者和防御者，迭代生成并防御提示注入攻击，从而在不依赖人工生成的对抗数据的情况下增强鲁棒性。

rss · OpenAI Blog · 7月15日 10:00

**背景**: 红队测试通过模拟攻击来识别 AI 模型的漏洞。自我对弈是一种让 AI 通过与自身对抗来改进的技术，广泛应用于游戏 AI。提示注入是一种安全漏洞，精心构造的输入会导致大语言模型产生意外行为。GPT-Red 结合这些概念，实现了红队测试的自动化和规模化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/unlocking-self-improvement-gpt-red/">GPT-Red: Unlocking Self-Improvement for Robustness | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#red teaming`, `#self-play`, `#prompt injection`, `#robustness`

---

<a id="item-3"></a>
## [研究员在周二补丁后发布 Windows 零日漏洞 PoC LegacyHive](https://thehackernews.com/2026/07/researcher-drops-new-windows-zero-day.html) ⭐️ 9.0/10

安全研究员 Nightmare-Eclipse 发布了名为 LegacyHive 的概念验证漏洞利用代码，针对 Windows 用户配置文件服务权限提升零日漏洞，时间就在微软 2026 年 7 月补丁星期二之后几小时。 这个公开可用的 PoC 对 Windows 系统构成直接威胁，因为它可能允许低权限攻击者提升至 SYSTEM 权限或访问其他用户账户，特别是对于未打补丁的系统尤为危险。 LegacyHive 漏洞利用滥用用户配置文件服务（ProfSvc）中的任意注册表配置单元加载，并需要另一个标准用户的凭据，但原始 PoC 据称无需此限制。该漏洞据称适用于所有安装了 2026 年 7 月补丁的受支持 Windows 版本。

rss · The Hacker News · 7月15日 11:07

**背景**: Windows 用户配置文件服务（ProfSvc）管理用户账户和环境，在用户登录时加载注册表配置单元。该服务中的漏洞可能允许攻击者加载其他用户的注册表配置单元，从而可能访问敏感数据或提升权限。研究员 Nightmare-Eclipse 被怀疑是一名前微软工程师，此前已发布过多个 Windows 零日漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/researcher-drops-new-windows-zero-day.html">Researcher Drops New Windows Zero-Day PoC Hours After Microsoft...</a></li>
<li><a href="https://cybersecuritynews.com/legacyhive-windows-0-day-vulnerability/">New LegacyHive Windows 0-day Vulnerability Released by...</a></li>
<li><a href="https://securityonline.info/legacyhive-windows-exploit/">LegacyHive: Exploit Code and Full Details Publicly Disclosed for Unpatched Windows Privilege Escalation Flaw</a></li>

</ul>
</details>

**标签**: `#windows`, `#zero-day`, `#security`, `#poc`, `#privilege-escalation`

---

<a id="item-4"></a>
## [Cursor 漏洞：恶意仓库可静默执行代码](https://thehackernews.com/2026/07/cursor-flaw-lets-malicious-cloned.html) ⭐️ 9.0/10

Cursor for Windows 存在一个严重未修补漏洞，当用户打开任意仓库时，会自动执行仓库根目录下的恶意 git.exe 文件，无需用户点击或确认。 该漏洞可让攻击者以用户身份执行代码，可能窃取 SSH 密钥、云令牌和源代码，影响数百万使用这款流行 AI 编辑器的开发者。 该漏洞已知已七个月，但至今未有官方补丁或安全公告，且只要项目保持打开，Cursor 会反复执行该二进制文件。

rss · The Hacker News · 7月15日 10:55

**背景**: Cursor 是由 Anysphere 开发的 AI 代码编辑器，基于 Visual Studio Code 分支。它会在多个位置动态搜索 Git 二进制文件，包括项目根目录。攻击者可在克隆的仓库中放置恶意 git.exe 来利用此行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>
<li><a href="https://www.securityweek.com/unpatched-cursor-vulnerability-exposes-users-to-code-execution/">Unpatched Cursor Vulnerability Exposes Users to Code Execution</a></li>
<li><a href="https://thehackernews.com/2026/07/cursor-flaw-lets-malicious-cloned.html">Cursor Flaw Lets Malicious Cloned Repositories Trigger Windows...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#Cursor`, `#code editor`, `#Windows`

---

<a id="item-5"></a>
## [ExLlamaV3 v1.0.0：本地 LLM 推理的重大性能升级](https://www.reddit.com/r/LocalLLaMA/comments/1uwylut/exllamav3_v100_major_performance_upgrades/) ⭐️ 9.0/10

经过一年多开发，Turboderp 发布了 ExLlamaV3 v1.0.0，包含新的注意力内核（支持在线缓存量化）、对包括 Gemma4 在内的大多数模型的张量并行支持，并且移除了对 flash-attention-2 和 xformers 的依赖。 该版本显著提升了本地运行大语言模型的性能和灵活性，在消费级 GPU 上实现更快推理并扩展模型兼容性。新特性如在线缓存量化和改进的 MoE 调度，为开源推理引擎树立了新标杆。 值得注意的变化包括新的 conv1d 内核替换了 causal_conv1d 依赖、用于减少内存占用的 INT8 GEMV 内核，以及用于更好负载均衡的 MoE 内核票据调度器。注意力内核支持滑动窗口注意力层的双输入和注意力汇聚，KV 缓存量化不再导致减速。

reddit · r/LocalLLaMA · /u/Unstable_Llama · 7月15日 07:17

**背景**: 本地 LLM 推理是在个人硬件上运行大语言模型，需要高效的实现以适配内存和计算限制。ExLlama 是一个针对 Llama 系列模型优化的开源推理库，张量并行将层分布到多个 GPU 以支持更大模型。注意力汇聚是吸收多余注意力的标记，用于稳定 Transformer 中的注意力动态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jarvislabs.ai/blog/scaling-llm-inference-dp-pp-tp">Scaling LLM Inference: Data, Pipeline & Tensor Parallelism in ...</a></li>
<li><a href="https://carnotresearch.medium.com/let-the-chaos-sink-in-481c8a37471e">Let the Chaos Sink In . Balancing attention in transformers | Medium</a></li>
<li><a href="https://pytorch.org/blog/accelerating-moe-model/">Accelerating MoE model inference with Locality-Aware Kernel Design – PyTorch</a></li>

</ul>
</details>

**标签**: `#LLM`, `#inference`, `#performance`, `#local-LLM`, `#open-source`

---

<a id="item-6"></a>
## [Thinking Machines 发布 Inkling 开源权重多模态模型](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines 推出了 Inkling，一个支持音频输入的开源权重多模态模型，专为微调设计，为企业提供了一个强大的可定制基础。 Inkling 填补了开源权重模型中支持音频的空白，使企业能够以较低成本微调多模态模型以完成特定任务，对专有模型构成挑战。 Inkling 不是整体最强的模型，但结合了多模态能力、高效推理以及 Tinker 平台上的微调可用性，支持长上下文窗口并通过 llama.cpp 进行本地推理。

hackernews · vimarsh6739 · 7月15日 18:12 · [社区讨论](https://news.ycombinator.com/item?id=48924912)

**背景**: 开源权重模型公开其训练后的参数，允许任何人下载并微调以用于定制应用。多模态 AI 模型同时处理多种数据类型（如文本、音频、图像），实现更丰富的交互和更广泛的用例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multimodal_learning">Multimodal learning - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区对 Inkling 的音频能力及其作为强大开源权重基础的潜力充满热情，并分享了实用的部署资源。一些评论者将其视为 DeepSeek 和 Z.ai 等模型的竞争对手，而另一些人则反思了现代模型开发日益增加的复杂性。

**标签**: `#open-weights`, `#multimodal`, `#audio`, `#AI`, `#model-release`

---

<a id="item-7"></a>
## [Telegram 数据中心谜团揭秘](https://dev.moe/en/3025) ⭐️ 8.0/10

2022 年的一项调查揭示了 Telegram 数据中心拓扑中未公开的细节，包括 DC3 的诡异空缺以及可能与俄罗斯 FSB 基础设施存在关联。 这对 Telegram 数亿用户构成了严重的安全和隐私担忧，尤其是考虑到 Telegram 标榜的隐私立场及其与俄罗斯国家机构持续存在的基建联系。 调查指出，DC2 负责服务俄罗斯和乌克兰用户且经常宕机，而 DC3 的用途不明；此外，泄露数据显示 Telegram 的基建可能由同时管理 FSB 基础设施的人运营。

hackernews · theanonymousone · 7月15日 13:22 · [社区讨论](https://news.ycombinator.com/item?id=48920475)

**背景**: Telegram 是由杜罗夫兄弟创建的流行通讯应用，采用 MTProto 协议并在全球分布数据中心。由于创始人曾在 2014 年因政府压力离开俄罗斯及此前创办的 VK，关于俄罗斯政府影响力的担忧一直存在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telegram_(software)">Telegram (software) - Wikipedia</a></li>
<li><a href="https://docs.telethon.dev/en/v2/concepts/datacenters.html">Data centers — Telethon 2.0.0a0 documentation</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了 IStories 调查确认了与 FSB 的关联，指出 DC2 宕机在俄语社区中是个常见笑点，并对神秘的 DC3 空缺和 Telegram 架构中的技术债务进行了讨论。

**标签**: `#Telegram`, `#data centers`, `#infrastructure`, `#security`, `#FSB`

---

<a id="item-8"></a>
## [Firefox 在 WebAssembly 中运行：完整浏览器渲染到 Canvas](https://developer.puter.com/labs/firefox-wasm/) ⭐️ 8.0/10

Firefox 被编译为 WebAssembly 并在 <canvas> 元素中渲染，其 Gecko、UI 组件和 Spidermonkey JavaScript 引擎均在 WASM 中运行，并采用一种新颖的 WASM 到 JS 的 JIT 技术来提升性能。 这一演示突破了 WebAssembly 的能力边界，表明即使是像 Firefox 这样复杂的浏览器也能在浏览器内部运行。它为在受限环境中运行完整浏览器或实现递归浏览体验提供了可能性。 该移植花费了超过 25,000 美元的 Opus/Fable 代币用于调试和 JIT 研究，且该浏览器本身不支持 WebAssembly，因此无法稳定地递归嵌套。相关项目 browser.js 提供了更节省内存的浏览器中之浏览器替代方案。

hackernews · coolelectronics · 7月15日 21:00 · [社区讨论](https://news.ycombinator.com/item?id=48926939)

**背景**: WebAssembly（WASM）是一种专为在网页浏览器中高性能执行而设计的二进制指令格式。将 Firefox 这样的完整浏览器编译为 WASM 需要克服巨大的性能挑战，通常需要借助新颖的 JIT 编译技术。本项目使用的 WISP 协议是一种低开销的方法，用于通过 WebSocket 连接代理 TCP/UDP 套接字，从而实现加密通信。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>
<li><a href="https://fable.io/">Fable · JavaScript you can be proud of!</a></li>

</ul>
</details>

**社区讨论**: 评论者尝试在 Firefox-WASM 内部递归运行自身，但结果挂起或不稳定。有些人认为它可用于智能电视等受限设备以绕过限制，另一些人则质疑为一个“有趣实验”花费 25,000 美元是否合理。

**标签**: `#WebAssembly`, `#Firefox`, `#Browser`, `#JIT`, `#Experimental`

---

<a id="item-9"></a>
## [Claude web_fetch 工具被绕过泄露用户记忆](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

安全研究员 Ayush Paul 发现 Claude 的 web_fetch 工具存在一个漏洞，通过诱导 AI 跟踪从恶意蜜罐站点返回的嵌套链接，能够窃取用户私人记忆。Anthropic 已移除 web_fetch 在获取内容中导航链接的能力，从而修复了该漏洞。 该漏洞表明，即使精心设计的 AI 工具限制也可能被社会工程绕过，对 AI 助手用户的隐私构成严重威胁。它凸显了持续对 AI 代理能力进行安全审计的必要性。 该攻击仅对 User-Agent 中包含"Claude-User"的客户端有效，且需要受害者先访问一个恶意页面，该页面提供按字母顺序排列的嵌套链接，逐字符泄露数据。Anthropic 未支付漏洞赏金，因为他们声称已内部发现该问题。

rss · Simon Willison · 7月15日 14:21

**背景**: “致命三重奏”是一种安全条件，指 AI 代理同时拥有私有数据访问权限、暴露于不受信任的输入、并能与外部通信，从而形成完整的攻击面。Claude 的 web_fetch 工具原本设计为仅允许从用户输入或 web_search 结果中获取确切 URL，但一个漏洞允许跟踪获取内容中返回的链接。该攻击利用此漏洞，通过构造蜜罐页面指示代理按字母顺序导航 URL 以泄露用户记忆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://certiv.ai/lethal-trifecta/">Agent Lethal Trifecta - Certiv</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Platform Docs</a></li>

</ul>
</details>

**标签**: `#security`, `#Claude`, `#AI`, `#data exfiltration`, `#prompt injection`

---

<a id="item-10"></a>
## [傅里叶像素让屏幕充当摄像头](https://www.schneier.com/blog/archives/2026/07/a-video-screen-that-is-also-a-camera.html) ⭐️ 8.0/10

瑞士苏黎世联邦理工学院的研究人员开发了一种傅里叶像素，可以同时发射和检测光，使显示屏具备摄像功能。该成果于 2026 年 7 月发表在《自然》杂志上。 这项技术可能彻底改变隐私和监控，因为任何屏幕都可能在没有独立摄像头的情况下观察观看者。它还开创了交互式显示和光学传感的新应用。 傅里叶像素通过操控光强度、振荡相位和偏振，同时生成和感知任意光场。它利用数学傅里叶分析分离出射和入射光，正如《自然》论文中所述。

rss · Schneier on Security · 7月15日 11:04

**背景**: 传统像素要么是发射器（如屏幕），要么是传感器（如摄像头传感器），但不同时具备两者。傅里叶像素是一种新型像素，通过傅里叶分析分离发射和检测的光，从而结合了两种功能。这一突破由苏黎世联邦理工学院的研究人员实现，并在《自然》上报道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://logicity.in/en/blog/eth-zurich-builds-pixels-that-emit-and-detect-light">ETH Zurich builds pixels that emit and detect light | Logicity</a></li>
<li><a href="https://www.zmescience.com/science/nanotechnology-science/this-new-pixel-could-turn-screens-into-cameras/">This New Pixel Could Turn Screens Into Cameras</a></li>

</ul>
</details>

**标签**: `#privacy`, `#surveillance`, `#display technology`, `#optical imaging`, `#ETH Zurich`

---

<a id="item-11"></a>
## [CUDA 13.3 引入无进位乘法以加速密码学](https://developer.nvidia.com/blog/building-faster-cryptography-with-carryless-multiplication-in-nvidia-cuda-13-3/) ⭐️ 8.0/10

NVIDIA CUDA 13.3 增加了对无进位乘法（CLMUL）的原生支持，这是一种在 x86 CPU 上已存在超过十五年的硬件加速基本操作，可在 GPU 上实现更快的密码学运算。 这一新增功能使 GPU 加速密码学在 AES-GCM 认证等操作上的效率接近 CPU 水平，并为区块链、零知识证明和同态加密中的高效多项式运算开辟了新的可能性。 无进位乘法（也称为 XOR 乘法）在乘法过程中丢弃进位，因此非常适合 GF(2) 上的有限域运算。CUDA 13.3 通过新的 `__cuda_clmul` 内建函数暴露该功能，其设计参考了 x86 PCLMULQDQ 指令。

rss · NVIDIA Developer Blog · 7月15日 17:37

**背景**: 无进位乘法是二元多项式算术的基本运算，广泛用于密码学（例如 AES-GCM 模式）和纠错码。超过 15 年来，x86 CPU 一直包含 PCLMULQDQ 指令，而 GPU 此前缺乏直接等效的操作。CUDA 13.3 通过提供利用 GPU 硬件的无进位乘法内建函数填补了这一空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CLMUL_instruction_set">CLMUL instruction set - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Carry-less_multiplication">Carry-less multiplication</a></li>
<li><a href="https://www.intel.com/content/dam/develop/external/us/en/documents/clmul-wp-rev-2-02-2014-04-20.pdf">Intel® Carry-Less Multiplication Instruction and its Usage ...</a></li>

</ul>
</details>

**标签**: `#CUDA`, `#cryptography`, `#GPU computing`, `#carryless multiplication`, `#NVIDIA`

---

<a id="item-12"></a>
## [模型路由：机器学习部署中的隐藏复杂性](https://huggingface.co/blog/ibm-research/model-routing-is-simple-until-it-isnt) ⭐️ 8.0/10

IBM Research 在 Hugging Face 上发表了一篇博客文章，揭示模型路由（即针对给定输入选择使用哪个机器学习模型的过程）尽管看似简单，却充满了隐藏的挑战。 这之所以重要，是因为随着 AI 系统越来越多地依赖多个模型来处理不同任务，有效的路由对于性能、成本和可靠性至关重要，然而许多实践者低估了其难度。 该文章强调了诸如输入分布漂移、模型过时、计算权衡以及需要适应变化的动态路由策略等问题。

rss · Hugging Face Blog · 7月15日 17:27

**背景**: 模型路由是一种机器学习系统中使用的技术，由路由器决定每个请求调用哪个模型（例如大型 vs. 小型 LLM），以平衡准确性和延迟。它在多模型服务平台（如 MLflow 或 SageMaker）中很常见，但生产环境中的复杂性往往来自模型交互、数据漂移和资源限制。

**标签**: `#model routing`, `#machine learning`, `#AI systems`, `#deployment`, `#challenges`

---

<a id="item-13"></a>
## [CISA 将两个正在被利用的漏洞加入 KEV 目录](https://www.cisa.gov/news-events/alerts/2026/07/15/cisa-adds-two-known-exploited-vulnerabilities-catalog) ⭐️ 8.0/10

CISA 于 2026 年 7 月 15 日将 CVE-2023-4346（KNX 协议账户锁定漏洞）和 CVE-2026-46817（Oracle 电子商务套件权限管理漏洞）加入其已知被利用漏洞目录，因为已有活跃利用证据。 这些漏洞正被恶意行为者积极利用，加入 KEV 目录后，根据约束性操作指令 26-04，美国联邦机构必须强制修复，同时也为所有组织提供了优先打补丁的关键指导。 CVE-2023-4346 影响楼宇自动化系统使用的 KNX 协议，CVE-2026-46817 影响 Oracle 电子商务套件；两者均有 CVE 编号表明已知利用。BOD 26-04 要求各机构修复 KEV 目录中列出的、在公开暴露资产上能获得完全控制的漏洞，并检查补丁前是否已被入侵。

rss · CISA Cybersecurity Advisories · 7月15日 12:00

**背景**: CISA 的已知被利用漏洞目录是确认已在野外被积极利用的漏洞列表。2026 年 6 月发布的约束性操作指令 26-04 要求美国联邦民事机构优先修复高风险漏洞，尤其是 KEV 目录中的漏洞。KNX 协议是家庭和楼宇自动化的国际标准，用于控制照明、暖通空调、安防等系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KNX">KNX - Wikipedia</a></li>
<li><a href="https://content.govdelivery.com/accounts/USDHSCISA/bulletins/41b445a">CISA Releases Binding Operational Directive 26-04 on ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#CISA`, `#vulnerability`, `#exploitation`, `#patching`

---

<a id="item-14"></a>
## [TuxBot v3 进化版：LLM 辅助的物联网僵尸网络](https://thehackernews.com/2026/07/tuxbot-v3-evolution-shows-signs-of-llm.html) ⭐️ 8.0/10

Unit 42 的研究人员披露了 TuxBot v3 Evolution，一个物联网僵尸网络框架，显示出在大语言模型（LLM）辅助下开发的迹象，尽管 AI 包含了安全免责声明。 这标志着 AI 驱动的网络威胁的一个显著趋势，降低了恶意软件开发的门槛，并可能增加物联网僵尸网络的规模。 该框架包含原始的 LLM 推理、1,496 个 Telnet 凭据、针对 30 多种物联网设备系列的漏洞利用，并使用模块化的 DDoS 僵尸网络架构，包括 C 语言代理和 Go 语言 C2 服务器。

rss · The Hacker News · 7月15日 18:43

**背景**: 大语言模型（LLM）是在海量文本数据上训练的人工智能系统，能够生成代码。网络犯罪分子越来越多地使用 LLM 来辅助恶意软件开发，尽管安全机制常常试图阻止直接协助。像 Mirai 这样的物联网僵尸网络历史上曾利用易受攻击的设备进行 DDoS 攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/tuxbot-v3-evolution-shows-signs-of-llm.html">TuxBot v3 Evolution Shows Signs of LLM-Assisted IoT Botnet ...</a></li>
<li><a href="https://github.com/PaloAltoNetworks/Unit42-timely-threat-intel/blob/main/2026-05-28-TuxBot-v3-Evolution-Framework-Analysis.txt">Unit42-timely-threat-intel/2026-05-28-TuxBot-v3-Evolution ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#IoT`, `#botnet`, `#LLM`, `#malware`

---

<a id="item-15"></a>
## [OkoBot 恶意软件通过助记词钓鱼攻击 Ledger 和 Trezor](https://thehackernews.com/2026/07/okobot-malware-framework-injects-seed.html) ⭐️ 8.0/10

该攻击通过利用用户对官方软件的信任，直接窃取硬件钱包用户最敏感的数据——助记词，即使在物理设备本身安全的情况下也可能导致资金被盗。 OkoBot 包含超过 20 个恶意载荷，包括 TookPS 和 Rilide 窃取器，并监控基于 Chromium 的浏览器以窃取助记词以外的其他凭证。

rss · The Hacker News · 7月15日 15:30

**背景**: Ledger 和 Trezor 等硬件钱包将加密货币私钥离线存储，但用户需要在配套的桌面应用中输入 12 至 24 个单词的恢复助记词。恶意软件通过向这些应用注入虚假登录提示，诱骗用户泄露助记词，从而使攻击者完全控制钱包。OkoBot 会等到硬件设备连接后才显示钓鱼覆盖层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kaspersky.com.au/about/press-releases/kaspersky-reveals-a-new-malicious-framework-targeting-cryptocurrency-users-with-the-use-of-okospyware">Kaspersky reveals a new malicious framework targeting...</a></li>
<li><a href="https://securelist.com/okobot-framework-targets-cryptocurrency-wallets/120660/">OkoBot framework infection chain | Securelist</a></li>
<li><a href="https://thehackernews.com/2026/07/okobot-malware-framework-injects-seed.html">OkoBot Malware Framework Injects Seed Phrase Phishing Into...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#cryptocurrency`, `#phishing`, `#hardware wallet`

---

<a id="item-16"></a>
## [Firefox、Chrome、Adobe、VMware 修补严重安全漏洞](https://thehackernews.com/2026/07/firefox-chrome-adobe-and-vmware-updates.html) ⭐️ 8.0/10

Mozilla、Google、Adobe 和 VMware 已发布安全更新，修复多个严重漏洞，其中包括两个 Firefox 漏洞（CVE-2026-15718 和 CVE-2026-15719），其利用代码已公开。 这些漏洞影响广泛使用的软件，且利用代码已公开，增加了大规模攻击的风险，用户应立即应用补丁。 Firefox 漏洞涉及 WebAssembly 中的无效指针（CVE-2026-15718）和 DOM 导航中的站点隔离问题（CVE-2026-15719）；提供的资料中未说明 Chrome、Adobe 和 VMware 漏洞的具体细节。

rss · The Hacker News · 7月15日 13:18

**背景**: WebAssembly（Wasm）是一种低级二进制指令格式，旨在网页上实现高性能执行，但其实现中的漏洞可能导致内存损坏。站点隔离是一种安全功能，将不同网站分离到不同进程中以防止跨站点数据窃取，其中的漏洞可能允许攻击者绕过保护措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="https://www.chromium.org/Home/chromium-security/site-isolation/">Site Isolation - The Chromium Projects</a></li>

</ul>
</details>

**标签**: `#security`, `#critical vulnerabilities`, `#Firefox`, `#Chrome`, `#Adobe`, `#VMware`

---

<a id="item-17"></a>
## [AsyncAPI npm 包被植入僵尸网络恶意软件](https://thehackernews.com/2026/07/compromised-asyncapi-npm-packages.html) ⭐️ 8.0/10

@asyncapi 命名空间中的四个 npm 包被攻陷，被发现分发多阶段僵尸网络加载器，多家安全公司已确认。 此次供应链攻击威胁到 AsyncAPI 生态系统，可能影响依赖这些包的事件驱动 API 开发者和用户，凸显了加强 npm 包安全性的必要性。 受影响的包包括 @asyncapi/generator-helpers@1.1.1、@asyncapi/generator-components@0.7.1、@asyncapi/generator@3.3.1 以及 @asyncapi/specs 的 6.11.2 和 6.11.2-alpha.1 版本。该恶意软件是一个多阶段僵尸网络加载器，具有远程访问木马和信息窃取功能。

rss · The Hacker News · 7月15日 09:16

**背景**: AsyncAPI 规范是用于定义事件驱动架构中异步 API 的行业标准。npm 是流行的 JavaScript 包管理器。供应链攻击通过破坏受信任的包来向下游用户分发恶意软件。OX Security、SafeDep、Socket 和 StepSecurity 等安全公司独立发现了此次入侵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.asyncapi.com/">AsyncAPI Initiative for event-driven APIs | AsyncAPI Initiative for event-driven APIs</a></li>
<li><a href="https://github.com/asyncapi/spec">GitHub - asyncapi/spec: The AsyncAPI specification allows you to create machine-readable definitions of your asynchronous APIs. · GitHub</a></li>

</ul>
</details>

**标签**: `#npm`, `#supply chain attack`, `#malware`, `#asyncapi`, `#security`

---

<a id="item-18"></a>
## [两个 SonicWall SMA 1000 零日漏洞被利用，其中一个可执行管理员命令](https://thehackernews.com/2026/07/two-sonicwall-sma-1000-zero-days.html) ⭐️ 8.0/10

SonicWall 发布警告，其 SMA 1000 系列设备中存在两个正在被积极利用的零日漏洞，其中一个漏洞（CVE-2026-15410）可能允许攻击者以管理员身份执行任意命令。另一个漏洞（CVE-2026-15409）是一个服务器端请求伪造（SSRF）漏洞，CVSS 评分为 10.0。 这些漏洞至关重要，因为它们影响广泛用于安全远程访问和零信任实施的 SMA 1000 设备，且已被积极利用，管理员必须立即修补以防止设备完全受损。SSRF 漏洞的 CVSS 10.0 评级凸显了紧迫性。 这两个 CVE 编号为 CVE-2026-15409（SSRF，CVSS 10.0）和 CVE-2026-15410（代码注入，可执行管理员命令）。SonicWall 已发布补丁，管理员应立即应用。目前没有可用的变通方案。

rss · The Hacker News · 7月15日 05:30

**背景**: SonicWall SMA（安全移动访问）1000 系列是专为安全远程访问和零信任网络访问设计的设备。零日漏洞是指在供应商知晓或发布补丁之前就被利用的漏洞。服务器端请求伪造（SSRF）允许攻击者从服务器向内部资源发起请求，可能绕过防火墙。代码注入漏洞可使攻击者执行任意系统命令，通常导致设备完全失控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/two-sonicwall-sma-1000-zero-days.html">Two SonicWall SMA 1000 Zero-Days Exploited, One Could Enable ...</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/07/14/sonicwall-sma-attacks-via-cve-2026-15409-cve-2026-15410/">SonicWall SMA appliances targeted in zero-day attacks (CVE ...</a></li>
<li><a href="https://www.sonicwall.com/products/remote-access/secure-mobile-access-1000-series">Secure Mobile Access (SMA) 1000 Series - SonicWall</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#SonicWall`, `#zero-day`, `#exploitation`

---

<a id="item-19"></a>
## [Zoom 警告存在严重账户劫持漏洞](https://www.bleepingcomputer.com/news/security/zoom-warns-of-critical-account-takeover-vulnerability/) ⭐️ 8.0/10

Zoom 披露了其 Windows 桌面客户端和软件开发工具包中的一个严重漏洞，未经身份验证的攻击者可利用该漏洞劫持账户。 由于 Zoom 被广泛应用于商务和个人通信，成功利用该漏洞可能导致数据泄露和隐私侵犯，因此这一警告至关重要。 该漏洞被评为严重级别，无需身份验证即可利用；影响范围包括 Zoom 的 Windows 桌面客户端和软件开发工具包。初始警告中未提供补丁详情。

rss · BleepingComputer · 7月15日 20:16

**背景**: Zoom 是一款在 COVID-19 疫情期间广泛使用的视频会议平台。账户劫持漏洞使攻击者能够完全控制用户账户，可能访问会议、聊天记录和个人数据。此类严重漏洞需要立即关注和修补。

**标签**: `#security`, `#vulnerability`, `#Zoom`, `#account takeover`, `#CVE`

---

<a id="item-20"></a>
## [AI 漏洞自动贩卖机自动发现零日漏洞](https://www.bleepingcomputer.com/news/security/we-built-a-vulnerability-vending-machine-ai-tokens-in-zero-days-out/) ⭐️ 8.0/10

Intruder 构建了一个 AI 驱动的“漏洞自动贩卖机”，将代码切片与大型语言模型 (LLM) 相结合，自动发现和利用软件漏洞，并通过发现 WordPress 插件中的真实零日漏洞进行了演示。 这标志着自动化漏洞研究的重大进步，可能降低发现高危漏洞的门槛，并促使厂商加快修补漏洞的紧迫性。 该系统使用代码切片将 LLM 输入缩减至仅相关的代码路径，从而能够分析大型代码库，并且发现的零日漏洞已通过负责任的披露方式告知插件供应商。

rss · BleepingComputer · 7月15日 14:01

**背景**: 代码切片是一种技术，可以分离出影响特定关注点（切片标准）的程序语句集，从而降低调试和分析的复杂性。大型语言模型 (LLM) 可以通过代码训练来识别表明漏洞的模式。通过结合这些方法，Intruder 的系统自动化了漏洞发现中繁琐的手动工作，有可能比传统方法更快地发现缺陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/we-built-a-vulnerability-vending-machine-ai-tokens-in-zero-days-out/">We built a vulnerability vending machine : AI tokens in, zero-days out</a></li>
<li><a href="https://en.wikipedia.org/wiki/Program_slicing">Program slicing - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#vulnerability discovery`, `#LLM`, `#zero-day`

---