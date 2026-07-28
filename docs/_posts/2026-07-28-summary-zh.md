---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> 从 62 条内容中筛选出 20 条重要资讯。

---

1. [月之暗面发布 2.8 万亿参数 Kimi K3 开放权重](#item-1)
2. [英伟达成立 37 方开放安全 AI 联盟，开源 NOOA 框架](#item-2)
3. [vLLM v0.26.0 发布：新增 Inkling 模型族及 DeepSeek-V4 性能优化](#item-3)
4. [Anthropic 呼吁对开放权重模型进行安全测试](#item-4)
5. [便携式 Python 发行版驱动现代工具链](#item-5)
6. [法官驳回谷歌利用 DMCA 阻止搜索数据抓取的企图](#item-6)
7. [沃尔沃/艾彻车队平台严重漏洞导致数百万用户和车辆数据泄露](#item-7)
8. [Paged Out #9 发布：免费技术杂志](#item-8)
9. [Libsm64：将《超级马里奥 64》作为可复用的游戏引擎库](#item-9)
10. [Cognyte 向美国警方出售手机监控车](#item-10)
11. [NVIDIA Ising 实现量子计算机全自动校准](#item-11)
12. [vBulletin 预认证 RCE 漏洞利用代码公开](#item-12)
13. [每周回顾：失控 AI 代理与重大威胁](#item-13)
14. [n8n 沙箱逃逸漏洞允许执行操作系统命令](#item-14)
15. [GitHub 为 Dependabot 添加三天冷却期以减少投毒包风险](#item-15)
16. [黑客利用 FastJson 零日远程代码执行漏洞攻击美国企业](#item-16)
17. [Arista 修补关键 VeloCloud Orchestrator 零日漏洞](#item-17)
18. [新型 Dysphoria DDoS 僵尸网络全球感染 20 万设备](#item-18)
19. [Certighost 概念验证漏洞利用代码发布，可劫持 Windows 域](#item-19)
20. [Spring Boot heapdump 端点泄露敏感机密](#item-20)

---

<a id="item-1"></a>
## [月之暗面发布 2.8 万亿参数 Kimi K3 开放权重](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 9.0/10

此次发布是开放权重大型语言模型的一个重要里程碑，因为 Kimi K3 是迄今为止公开可用的最大模型之一。通过提供对最先进模型的访问，它可能显著加速 AI 社区的研究与开发，尽管修改后的许可证对大型商业用户施加了限制。 Kimi K3 的许可证不再使用“修改版 MIT”标签，并要求任何年收入超过 2000 万美元的模型即服务（MaaS）业务公司签署单独协议。模型权重在使用 MXFP4 量化时约为 1.4 TB，且由于缺乏 FP4 张量核心，预计在 A100 GPU 上运行困难。

rss · Simon Willison · 7月27日 23:39

**背景**: Kimi K3 是由中国 AI 公司月之暗面（Moonshot AI）开发的大型语言模型。它采用混合专家（MoE）架构，每 token 仅激活部分参数以提高效率。之前的模型 Kimi K2 在修改版 MIT 许可下发布，要求大型商业实体进行署名。此类开放权重发布允许研究人员和开发者自行下载、微调和部署模型，从而为开源 AI 生态系统做出贡献。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.moonshot.ai/">Welcome to Moonshot AI. Our mission is to seek the optimal...</a></li>
<li><a href="https://mit-license.org/">MIT License</a></li>

</ul>
</details>

**社区讨论**: 一名 Reddit 用户分享了在 A100、H200 和 B300 GPU 上托管 K3 的计划，指出内存挑战：8 块 A100 仅提供 640 GB，远小于 1.4 TB 的权重，在 KV 缓存之前就需要三个节点。由于缺乏 FP4 支持，他们预计 A100 上性能不佳，但仍计划进行基准测试。

**标签**: `#AI`, `#open-source`, `#large language model`, `#Moonshot`, `#Hugging Face`

---

<a id="item-2"></a>
## [英伟达成立 37 方开放安全 AI 联盟，开源 NOOA 框架](https://thehackernews.com/2026/07/nvidia-forms-37-member-open-secure-ai.html) ⭐️ 9.0/10

英伟达与包括微软、思科在内的 36 家合作伙伴共同成立开放安全 AI 联盟，旨在开发开放的 AI 安全工具，并开源了用于优化 AI 智能体性能的 NOOA 框架。 这一全行业合作标志着 AI 安全领域的范式转变，有望为 AI 安全部署和整个生态系统的信任建立新标准。 该联盟涵盖云、安全、企业软件和 AI 领域的公司，成员包括 CrowdStrike、Hugging Face 和 Red Hat 等；但治理结构和联合成果尚未公布。

rss · The Hacker News · 7月27日 18:10

**背景**: 随着 AI 智能体和模型的普及，AI 安全问题日益突出。开放安全 AI 联盟旨在共享开放技术和工具以保障 AI 系统安全，而 NOOA 则是一个通过优化交互能力来提升 AI 智能体性能的框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/open-secure-ai-alliance/">Industry Leaders Join Open Secure AI Alliance for AI Safety ...</a></li>
<li><a href="https://thehackernews.com/2026/07/nvidia-forms-37-member-open-secure-ai.html">NVIDIA Forms 37-Member Open Secure AI Alliance and Open ...</a></li>
<li><a href="https://blockchain.news/news/nvidia-nooa-ai-agent-performance">NVIDIA's NOOA Framework Boosts AI Agent Performance by Over ...</a></li>

</ul>
</details>

**标签**: `#AI security`, `#open source`, `#industry alliance`, `#NVIDIA`, `#secure AI`

---

<a id="item-3"></a>
## [vLLM v0.26.0 发布：新增 Inkling 模型族及 DeepSeek-V4 性能优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 引入了全新的 Inkling 模型家族，提供包括分段 CUDA 图和 Hopper FA4 注意力在内的完整支持；通过专用内核和融合操作显著提升了 DeepSeek-V4 在各厂商硬件上的性能；并新增了通过 head_dtype 实现的 fp32 lm_head，以提升生成精度。 此次发布显著提升了 LLM 推理的吞吐量和灵活性，尤其针对 DeepSeek-V4 模型和新兴的 Inkling 家族，使生产环境中的部署更快速、延迟更低。 该版本包含来自 212 位贡献者（其中 61 位新贡献者）的 411 次提交，包括专用路由内核（DeepSeek-V4 端到端 TPOT 提升 2.94%）、fused_topk_bias 内核（速度提升 1.5-2 倍）和冗余重复/拷贝移除（端到端 TPOT 提升 1.8%），以及按 KV-cache 组灵活选择注意力后端的新功能和逐步成熟的带有分层二级存储的 KV 卸载功能。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个用于高吞吐量 LLM 推理的开源库，采用了 PagedAttention 和连续批处理等技术。推测解码通过使用草稿模型每步预测多个 token 来加速生成。FlashAttention-4 (FA4) 是针对 Hopper GPU 优化的注意力算法。ModelOpt NVFP4 量化可在保持精度的同时减小模型大小。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>
<li><a href="https://pytorch.org/blog/flexattention-flashattention-4-fast-and-flexible/">FlexAttention + FlashAttention-4: Fast and Flexible – PyTorch</a></li>
<li><a href="https://www.spheron.network/blog/tensorrt-model-optimizer-modelopt-quantization-guide/">NVIDIA TensorRT Model Optimizer (ModelOpt): FP8, INT4, and FP4 Quantization Guide (2026) | Spheron Blog</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#release notes`, `#performance optimization`, `#model support`

---

<a id="item-4"></a>
## [Anthropic 呼吁对开放权重模型进行安全测试](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 发布了一份关于开放权重 AI 模型的政策声明，明确要求对所有能力足够的模型（包括开放权重模型）进行强制性安全测试。该公司强调，它并不主张彻底禁止开放权重模型，而是提议进行监管。 这一来自领先 AI 实验室的立场可能会影响全球 AI 监管，如果安全测试变得过于昂贵或官僚化，可能导致对开放权重模型的事实上的限制。这场辩论凸显了 AI 开发中开放性、安全性和企业利益之间的紧张关系。 Anthropic 的 CEO Dario Amodei 此前曾对禁令表示怀疑，但该声明支持限制向中国销售芯片等措施，暴露出内部矛盾。该政策未明确由谁进行测试或如何管理成本，留下了批评空间。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重 AI 模型是指其训练参数（权重）公开发布的模型，允许任何人下载、运行和微调，但它们通常不包含完整的训练代码或数据，这使其与开源 AI 区分开来。与封闭模型不同，开放权重模型可以在本地使用和修改，这引发了关于在缺乏足够保护的情况下可能被滥用的担忧。Anthropic 的立场是在关于如何平衡 AI 创新与安全的辩论日益激烈的背景下提出的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights : not quite what you’ve been told – Open Source Initiative</a></li>
<li><a href="https://openai.com/global-affairs/open-weights-and-ai-for-all/">Open weights and AI for all | OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区评论高度批评，许多人指责 Anthropic 通过昂贵的测试要求推行事实上的禁令。其他人则指出 Anthropic 立场的虚伪性，注意到 CEO Dario Amodei 过去反对禁令，却支持对中国实施芯片限制。一些评论者认为该声明是保护 Anthropic 商业利益的道德信号。

**标签**: `#AI safety`, `#open-weights`, `#regulation`, `#Anthropic`, `#AI policy`

---

<a id="item-5"></a>
## [便携式 Python 发行版驱动现代工具链](https://gregoryszorc.com/docs/python-build-standalone/main/) ⭐️ 8.0/10

python-build-standalone 项目提供了自包含、高度可移植的 Python 发行版，这些发行版现已被 uv、pipx、Hatch 和 Poetry 等工具广泛采用，用于在不依赖系统安装的情况下捆绑 Python。 这种方法简化了 Python 环境管理和应用分发，使开发者能够更轻松地跨平台交付 Python 应用，并使工具能够按需提供 Python。 这些发行版由 Astral（uv 的创建者）在 astral-sh 组织下维护，支持多个操作系统和架构。一个相关项目 PyOxy 将这些发行版与 Rust 代码结合，生成单文件可执行文件。

hackernews · jcbhmr · 7月27日 18:43 · [社区讨论](https://news.ycombinator.com/item?id=49073942)

**背景**: 传统上，Python 安装依赖系统库且不易迁移。python-build-standalone 项目自动化了构建过程，将所有依赖项打包在一起，生成可移植的二进制文件。这对于需要在不依赖预装解释器的情况下分发 Python 的工具至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49073942">Self-contained highly-portable Python distributions | Hacker News</a></li>
<li><a href="https://gregoryszorc.com/blog/2019/06/24/building-standalone-python-applications-with-pyoxidizer/">Gregory Szorc's Digital Home | Building Standalone Python Applications with PyOxidizer</a></li>

</ul>
</details>

**社区讨论**: 来自 uv、pipx 和其他项目的社区成员确认了广泛采用。Charlie Marsh 指出这些发行版被 uv 和许多其他工具使用。Simon Willison 称赞它们非常适合将 Python 捆绑到桌面应用中。其他人则提到了 PyOxy 和 Cosmopolitan 的跨平台二进制文件等替代方案，总体对项目持积极态度。

**标签**: `#python`, `#tooling`, `#distribution`, `#portable`, `#standalone`

---

<a id="item-6"></a>
## [法官驳回谷歌利用 DMCA 阻止搜索数据抓取的企图](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

美国法官裁定，谷歌不能利用《数字千年版权法》（DMCA）阻止 SerpAPI 抓取其搜索结果，驳回了谷歌关于被抓取数据构成受保护数据库内容的主张。 这一裁决确立了法律先例，限制企业利用版权法阻止网络抓取，保护了开放网络，并支持了依赖搜索数据的第三方服务。 谷歌辩称其搜索结果属于受版权保护的数据库，但法官认为这些结果缺乏版权保护所需的创造性筛选。该裁决仅适用于 DMCA 主张，不涉及其他法律依据。

hackernews · cdrnsf · 7月27日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: DMCA 是美国的一项法律，将旨在规避版权保护措施的技术生产和传播定为犯罪。网络抓取是指从网站自动提取数据的行为，谷歌此前已弃用其公共搜索 API，使得抓取成为第三方获取搜索结果的唯一途径。

**社区讨论**: 评论者指出，谷歌本身建立在抓取开放网络的基础上，却试图阻止抓取，实属讽刺。他们批评谷歌取消了低价 API，然后起诉阻止第三方填补这一空白，并指出被抓取的搜索结果有助于揭露广告诈骗。

**标签**: `#web scraping`, `#DMCA`, `#Google`, `#legal`, `#open web`

---

<a id="item-7"></a>
## [沃尔沃/艾彻车队平台严重漏洞导致数百万用户和车辆数据泄露](https://eaton-works.com/2026/07/27/my-eicher-hack/) ⭐️ 8.0/10

一名安全研究人员在 VE Commercial Vehicles 的 My Eicher 车队管理平台中发现了关键未认证 API，暴露了 74.8 万客户、17.4 万用户、67.6 万车辆以及 250 万个一次性密码（OTP），能够实现账户接管和车队完全控制。 该漏洞对商业车队运营构成严重风险，攻击者可追踪、锁定或劫持卡车和巴士，可能扰乱物流和运输。这凸显了汽车物联网系统日益增长的安全挑战。 该漏洞于 2025 年 7 月被发现并报告给 VE Commercial Vehicles，后者在 2025 年 11 月前悄悄修复了主要问题。研究人员在 12 个月的披露时间后于 2026 年 7 月公布了全部细节。

hackernews · EatonZ · 7月27日 15:08 · [社区讨论](https://news.ycombinator.com/item?id=49070756)

**背景**: My Eicher 是业界首个针对商用卡车和巴士的数字车队管理平台，提供车队追踪、燃油管理和运行时间监控等功能。该平台由沃尔沃集团与艾彻汽车合资企业 VE Commercial Vehicles 运营。这类基于云的系统正越来越多地用于管理大型车队，因此其安全性对安全运营至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eaton-works.com/2026/07/27/my-eicher-hack/">Exploiting Volvo/Eicher’s fleet management platform to gain ...</a></li>
<li><a href="https://daily.dev/posts/exploiting-volvo-eicher-s-fleet-platform-to-gain-control-over-all-users-vehicles-gkfj0eqmw">Exploiting Volvo/Eicher's fleet platform to gain control...</a></li>

</ul>
</details>

**社区讨论**: 社区成员赞扬了研究人员在漫长的披露时间中的耐心，有人指出保护用户的安全与仅仅为公司提供诉讼保护的安全之间的区别。另一位评论者表达了对现代汽车完全依赖云连接的担忧，讲述了一辆宝马因无手机信号而无法启动的经历。还分享了一个 FSF 的维修权视频链接。

**标签**: `#security`, `#automotive`, `#IoT`, `#vulnerability`, `#responsible disclosure`

---

<a id="item-8"></a>
## [Paged Out #9 发布：免费技术杂志](https://pagedout.institute/download/PagedOut_009.pdf) ⭐️ 8.0/10

Paged Out #9 是一本免费的技术杂志（PDF 格式），已发布，内容涵盖底层编程和理论计算机科学，具有浓厚的黑客探索精神。 这本杂志复兴了 Phrack 和 2600 等经典黑客杂志的精神，为分享底层知识和促进社区参与提供了一个设计精良的现代平台。 该杂志包含广泛文章，从幽默的《C 语言婴儿步》到深奥的理论工作——未注明出处的王浩 1960 年代可计算铺砌理论的重新发现，将多米诺问题与停机问题联系起来。

hackernews · laurensr · 7月27日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49070138)

**背景**: Paged Out 是一本免费的社区驱动杂志，专注于底层编程、黑客技术和计算机科学。它常被比作 1990 年代流行的经典黑客杂志 Phrack 和 2600。其中关于可计算铺砌的文章指的是王浩（Hao Wang）提出的王砖（Wang tiles）形式系统，其中多米诺问题（一组砖是否能铺满平面）被证明等价于停机问题，这是可计算性理论中的一个基础结果。

**社区讨论**: 社区反响非常积极，读者称赞该杂志的技术深度、精美的设计以及让人联想到 Phrack 和 2600 的怀旧感。一位评论者强调了未注明出处的王浩可计算铺砌理论的重新发现，认为这是一颗理论计算机科学的瑰宝。

**标签**: `#programming`, `#low-level`, `#hacking`, `#technical magazine`, `#theoretical CS`

---

<a id="item-9"></a>
## [Libsm64：将《超级马里奥 64》作为可复用的游戏引擎库](https://github.com/libsm64/libsm64) ⭐️ 8.0/10

Libsm64 是一个新的开源库，将《超级马里奥 64》的逆向工程代码重新打包成干净、可复用的库，可集成到其他游戏引擎中，使马里奥 64 的角色和机制能出现在外部游戏中。 该项目展示了通过逆向工程实现游戏资产复用的新颖方法，无需依赖专有的元宇宙概念即可实现如《半条命 2》中的马里奥等创意跨界混搭，为游戏模组和实验开辟了可能性。 Libsm64 基于《超级马里奥 64》的完整逆向工程代码，提供了用于运动和渲染的干净 C API。一个“awesome-libsm64”列表展示了使用它的项目，包括一个《半条命 2》中的马里奥演示。

hackernews · klaussilveira · 7月27日 10:04 · [社区讨论](https://news.ycombinator.com/item?id=49067352)

**背景**: 《超级马里奥 64》已通过 SM64 反向工程项目完全反编译为可移植的 C 代码，使其能在各种平台上编译。Libsm64 更进一步，将核心游戏代码打包为可复用的库而非独立游戏，从而易于集成到 Unity 或 Source 等其他引擎中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm 64 / libsm 64 : Mario 64 as a library for use in external...</a></li>

</ul>
</details>

**社区讨论**: 社区反应热烈，评论者称其“不可思议”，并比喻为没有炒作成分的元宇宙承诺。有评论者开玩笑建议将其作为服务出售，其他人则分享了演示视频和使用 libsm64 的项目精选列表链接。

**标签**: `#game development`, `#reverse engineering`, `#emulation`, `#library`, `#open source`

---

<a id="item-10"></a>
## [Cognyte 向美国警方出售手机监控车](https://www.schneier.com/blog/archives/2026/07/cognyte-sells-a-mobile-cell-surveillance-van.html) ⭐️ 8.0/10

以色列监控公司 Cognyte 正在向美国执法机构销售名为 FalcoNet 的移动手机监控车，其中与德克萨斯州的合同价值 450 万美元。 这项技术使警方无需搜查令即可追踪附近所有手机，因其大规模监控能力引发了严重的隐私和宪法问题。 FalcoNet 系统充当基站模拟器，强制附近手机连接，并可隐藏在车辆、背包或直升机中。

rss · Schneier on Security · 7月27日 11:04

**背景**: 基站模拟器，也称为 IMSI 捕捉器或 Stingray，是模仿基站截取手机数据的设备。它们最初为军事情报用途开发，现已被地方执法机构采用，尽管面临隐私和法律挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techstory.in/texas-falconet-surveillance-suvs-privacy-concerns/">Texas Police Deploy $4.5M FalcoNet Surveillance - TechStory</a></li>

</ul>
</details>

**标签**: `#surveillance`, `#privacy`, `#cell-site simulator`, `#law enforcement`, `#Israel`

---

<a id="item-11"></a>
## [NVIDIA Ising 实现量子计算机全自动校准](https://developer.nvidia.com/blog/nvidia-ising-enables-fully-automated-quantum-computer-calibration-with-enhanced-in-context-learning/) ⭐️ 8.0/10

NVIDIA 发布了一款名为 NVIDIA Ising Calibration 的开源视觉语言模型（VLM），该模型能够解读量子处理器的诊断输出，并利用增强的上下文学习实现校准流程的完全自动化。 这一突破将量子计算中关键且耗时的步骤自动化，减少了人工干预，加速了实用量子计算机的研发进程。开源发布使更广泛的研究社区能够利用并改进这项技术。 NVIDIA Ising Calibration 是 NVIDIA 首个开源量子 AI 模型系列的一部分，与 CUDA-Q 平台无缝集成，并针对 NVIDIA GPU 进行了优化，支持 FP8 量化。该模型不仅涵盖校准，还涉及量子纠错。

rss · NVIDIA Developer Blog · 7月27日 16:00

**背景**: 量子计算机需要频繁校准以修正量子比特操作中的漂移和误差，传统上这一过程依赖人工且耗时。视觉语言模型（VLM）能够分析量子处理器诊断的视觉表示（如误差图），并自动确定最优控制调整。上下文学习使 VLM 无需重新训练即可适应新的处理器配置，提高了校准过程的灵活性和可扩展性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.cn/ising">用于量子计算的 AI 模型和框架 | NVIDIA 开发者</a></li>
<li><a href="https://isingai.net/">NVIDIA Ising</a></li>
<li><a href="https://www.linkedin.com/pulse/nvidias-ising-platform-how-ai-finally-tackling-quantum-minu-j-bae-zufje">[Update #9] NVIDIA ’s Ising Platform: How AI Is Finally Tackling...</a></li>

</ul>
</details>

**标签**: `#quantum computing`, `#machine learning`, `#vision language model`, `#automation`, `#NVIDIA`

---

<a id="item-12"></a>
## [vBulletin 预认证 RCE 漏洞利用代码公开](https://thehackernews.com/2026/07/public-exploit-released-for-patched.html) ⭐️ 8.0/10

7 月 27 日，公开的利用代码细节展示了未经身份验证的攻击者如何利用已修补的 vBulletin 6.2.1 及更早版本、6.1.6 及更早版本中的预认证远程代码执行漏洞。 该公开利用代码增加了成千上万未修补的 vBulletin 论坛的风险，攻击者无需任何凭证即可在服务器上执行任意代码，可能导致网站完全被控制。 该漏洞允许未经身份验证的 HTTP 请求到达 PHP 的 eval() 函数，受影响版本包括 vBulletin 6.2.1 及更早版本、6.1.6 及更早版本，未指定更低版本限制。

rss · The Hacker News · 7月27日 14:40

**背景**: vBulletin 是一款广泛使用的商业论坛软件。预认证远程代码执行漏洞允许攻击者无需任何凭证即可在服务器上执行任意代码。PHP 的 eval() 函数会执行传入的任意 PHP 代码，如果攻击者控制的输入能到达 eval()，就可能导致系统完全被攻破。此前 vBulletin 中就曾发现过类似漏洞，例如影响 5.x 版本的 CVE-2019-16759。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/public-exploit-released-for-patched.html">Public Exploit Released for Patched vBulletin Pre-Auth Code Execution Flaw</a></li>
<li><a href="https://www.tenable.com/blog/critical-zero-day-pre-authentication-remote-code-execution-exploit-published-for-5-x-versions">Critical Zero-Day Pre-authentication Remote Code Execution Exploit Published for 5.x Versions of vBulletin - Blog | Tenable®</a></li>

</ul>
</details>

**标签**: `#security`, `#exploit`, `#vBulletin`, `#RCE`, `#vulnerability`

---

<a id="item-13"></a>
## [每周回顾：失控 AI 代理与重大威胁](https://thehackernews.com/2026/07/weekly-recap-rogue-ai-agents-check.html) ⭐️ 8.0/10

The Hacker News 的每周回顾重点介绍了失控 OpenAI 代理威胁、Check Point SmartConsole 严重漏洞（CVE-2026-16232）的积极利用、利用 LLM 幻觉的 slopsquatting 攻击的兴起，以及 ClickFix 社会工程诱饵的增加。 这些事件表明攻击向量不断演变，威胁着企业基础设施和软件供应链，安全团队需要监控 AI 代理行为、及时修补关键漏洞，并教育用户防范复杂的社会工程手段。 Check Point 漏洞是一个身份验证绕过漏洞（CWE-287），CVSS 评分 9.1，已在野外被积极利用。Slopsquatting 涉及注册 LLM 幻觉出的软件包名称，诱骗开发者安装恶意代码。ClickFix 诱饵冒充 CAPTCHA 或 Cloudflare Turnstile，提示用户复制粘贴恶意命令。

rss · The Hacker News · 7月27日 14:10

**背景**: 失控 AI 代理指行为超出预期边界的 AI 系统，可能执行未经授权的操作。Slopsquatting 是“AI slop”和“typosquatting”的合成词——攻击者注册 LLM 可能幻觉出的不存在软件包名称，用户复制 AI 生成的代码后可能无意中安装恶意包。ClickFix 是一种社会工程技术，攻击者诱骗受害者复制粘贴命令以“修复”虚假的网页错误，从而导致恶意软件安装。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/weekly-recap-rogue-ai-agents-check.html">⚡ Weekly Recap: Rogue AI Agents, Check Point Exploit ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Slopsquatting">Slopsquatting</a></li>
<li><a href="https://www.rapid7.com/blog/post/etr-cve-2026-16232-critical-check-point-smartconsole-authentication-bypass-exploited-in-the-wild/">CVE-2026-16232: Critical Check Point SmartConsole ... - Rapid7</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2025/08/21/think-before-you-clickfix-analyzing-the-clickfix-social-engineering-technique/">Think before you Click ( Fix ): Analyzing the ClickFix social engineering...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#AI safety`, `#vulnerability`, `#threat intelligence`

---

<a id="item-14"></a>
## [n8n 沙箱逃逸漏洞允许执行操作系统命令](https://thehackernews.com/2026/07/n8n-sandbox-escape-lets-workflow.html) ⭐️ 8.0/10

n8n 团队修补了一个高严重性的表达式沙箱逃逸漏洞，该漏洞允许经过身份验证的工作流编辑者在服务器上执行操作系统命令。受影响版本包括 2.31.5 之前及 2.32.0 至 2.32.1 之前。 此漏洞可能导致 n8n 实例的服务器完全受损，影响依赖 n8n 进行工作流自动化的组织。鉴于 n8n 的广泛使用，及时打补丁对于防止恶意内部人员或受损账户执行远程代码至关重要。 该漏洞由 Security Joes 在测试之前针对 CVE-2026-27577 的修复时发现，表明这是一个绕过漏洞。n8n 在 2.31.5 和 2.32.1 版本中修复了此问题。

rss · The Hacker News · 7月27日 13:05

**背景**: n8n 是一个开源的工作流自动化平台，允许用户通过可视化编辑器连接应用程序和服务。沙箱逃逸漏洞是指运行在受限环境（沙箱）中的代码突破限制，在主机系统上执行任意命令。在 n8n 中，表达式沙箱用于安全评估用户提供的 JavaScript 表达式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pillar.security/blog/n8n-sandbox-escape-critical-vulnerabilities-in-n8n-exposes-hundreds-of-thousands-of-enterprise-ai-systems-to-complete-takeover">n8n Sandbox Escape : Critical Vulnerabilities in n8n Exposes...</a></li>
<li><a href="https://www.endorlabs.com/vulnerability/cve-2026-27577">Endor Patches | CVE-2026-27577, n8n: Expression Sandbox Escape ...</a></li>

</ul>
</details>

**标签**: `#security`, `#n8n`, `#vulnerability`, `#sandbox escape`, `#CVE`

---

<a id="item-15"></a>
## [GitHub 为 Dependabot 添加三天冷却期以减少投毒包风险](https://thehackernews.com/2026/07/github-adds-3-day-dependabot-cooldown.html) ⭐️ 8.0/10

GitHub 在 Dependabot 中引入默认的三天冷却期，将版本更新拉取请求延迟至新包发布至少三天后。 这一缓解措施解决了关键的供应链安全问题，降低了自动采纳发布后迅速被删除的恶意包的风险，保护了数百万 Dependabot 用户。 冷却期可通过 dependabot.yml 自定义，但安全更新仍会立即交付。自 2026 年 7 月起，此默认设置适用于所有使用 Dependabot 版本更新的仓库。

rss · The Hacker News · 7月27日 08:01

**背景**: 在软件供应链攻击中，攻击者发布恶意包版本，这些版本会被 Dependabot 等自动依赖更新工具迅速采纳。通过引入三天冷却期，GitHub 为社区提供了一个窗口，以便在恶意包广泛传播前发现并移除它们。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/github-adds-3-day-dependabot-cooldown.html">GitHub Adds 3-Day Dependabot Cooldown to Limit Poisoned ...</a></li>
<li><a href="https://github.blog/changelog/2026-07-14-dependabot-version-updates-introduce-default-package-cooldown/">Dependabot version updates introduce default package cooldown</a></li>
<li><a href="https://github.blog/security/supply-chain-security/the-case-for-a-cooldown-why-dependabot-now-waits-before-issuing-version-updates/">The case for a cooldown: Why Dependabot now waits before ...</a></li>

</ul>
</details>

**标签**: `#security`, `#GitHub`, `#Dependabot`, `#supply chain`, `#software updates`

---

<a id="item-16"></a>
## [黑客利用 FastJson 零日远程代码执行漏洞攻击美国企业](https://www.bleepingcomputer.com/news/security/hackers-target-us-firms-in-fastjson-rce-zero-day-attacks/) ⭐️ 8.0/10

这是一起重大安全事件，因为 FastJson 在企业应用中广泛使用，且该零日漏洞可被远程利用而无需认证，可能导致系统完全被控制。 该漏洞影响 FastJson 1.x 版本；FastJson 2.x 是独立的代码库，不受影响。即时缓解措施是设置-Dfastjson.parser.safeMode=true 启用 SafeMode，或切换到 noneautotype 构建变体。

rss · BleepingComputer · 7月27日 23:49

**背景**: FastJson 是由阿里巴巴开发的开源 Java 库，用于将 JSON 字符串与 Java 对象相互转换。由于其速度快且易于使用，在企业应用中非常流行。零日远程代码执行漏洞意味着攻击者可以在没有任何先验访问或认证的情况下，在目标服务器上执行任意代码，通常会导致数据泄露或勒索软件部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-target-us-firms-in-fastjson-rce-zero-day-attacks/">Hackers target US firms in FastJson RCE zero - day attacks</a></li>
<li><a href="https://sanjayseth.com/fastjson-cve-2026-16723-spring-boot-rce-zero-day/">sanjayseth.com/ fastjson -cve-2026-16723-spring-boot-rce- zero - day</a></li>
<li><a href="https://github.com/alibaba/fastjson/wiki">Home · alibaba/ fastjson Wiki · GitHub</a></li>

</ul>
</details>

**标签**: `#security`, `#zero-day`, `#RCE`, `#Java`, `#vulnerability`

---

<a id="item-17"></a>
## [Arista 修补关键 VeloCloud Orchestrator 零日漏洞](https://www.bleepingcomputer.com/news/security/arista-patches-velocloud-orchestrator-zero-day-exploited-in-attacks/) ⭐️ 8.0/10

Arista 已修复了本地部署 VeloCloud Orchestrator 中的一个最高严重级别命令注入零日漏洞（CVE-2026-16812），该漏洞正在被积极利用进行攻击。 该漏洞非常关键，因为它允许未经身份验证的远程攻击者在受影响系统上执行任意命令，其积极利用对使用本地 VeloCloud Orchestrator 的组织构成严重风险。CISA 将其列入已知被利用漏洞目录，突显了修补的紧迫性。 该漏洞的 CVSS 严重性评分为 10.0（最高分），表示无需认证即可远程执行代码。Arista 已发布补丁，管理员应立即应用，尤其是该漏洞已被列入 CISA 的 KEV 目录。

rss · BleepingComputer · 7月27日 22:49

**背景**: VeloCloud Orchestrator 是 Arista SD-WAN 解决方案的集中管理组件，用于跨分布式边缘设备配置、监控和编排网络策略。命令注入漏洞发生在应用程序将未净化的用户输入传递给系统 shell 时，允许攻击者执行任意操作系统命令。该零日漏洞在补丁可用之前已被积极利用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/arista-patches-velocloud-orchestrator-zero-day-exploited-in-attacks/">Arista patches VeloCloud Orchestrator zero-day exploited in ...</a></li>
<li><a href="https://www.arista.com/en/orchestrator-guide-vc-6-1/sd-wan-6-1-arista-velocloud-orchestrator-deployment-and-monitoring-guide">VeloCloud SD-WAN 6.1 - Orchestrator Guide - arista.com VeloCloud SD-WAN 5.2 - Orchestrator Guide - Overview - Arista Arista patches VeloCloud Orchestrator zero-day exploited in ... VeloCloud Orchestrator (VCO) Overview - Dell Technologies VMware VeloCloud SDWAN Components: Detailed Explanation VMware VeloCloud SD-WAN Operator Guide Velocloud Orchestrator API Usage Best Practices Top Stories</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#zero-day`, `#patching`, `#cloud`

---

<a id="item-18"></a>
## [新型 Dysphoria DDoS 僵尸网络全球感染 20 万设备](https://www.bleepingcomputer.com/news/security/new-dysphoria-ddos-botnet-spreads-to-200k-devices-worldwide/) ⭐️ 8.0/10

一种名为 Dysphoria 的新型僵尸网络已感染全球约 20 万台设备，用于发动 DDoS 攻击和流量中继操作，并在 3 月针对 JackSkid 基础设施的执法行动后，采用基于区块链的名称服务以增强抗打击能力。 这标志着僵尸网络在抗打击能力上的重要演变，基于区块链的名称服务使命令与控制更难被切断，对全球网络安全和物联网设备安全构成严重且持续的威胁。 该僵尸网络使用以太坊名称服务（ENS）和 Solana 名称服务（SNS）记录进行命令与控制，并通过受感染设备作为中继路由流量，将控制器隐藏在分发层之后。

rss · BleepingComputer · 7月27日 21:08

**背景**: 僵尸网络是由被远程控制的受感染设备组成的网络，用于发动网络攻击，例如 DDoS 攻击。Dysphoria 由 JackSkid 僵尸网络演变而来，后者于 2025 年 3 月被国际执法机构瓦解。ENS 等基于区块链的名称服务将人类可读名称映射到区块链地址，由于其去中心化特性，取缔难度极大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/new-dysphoria-ddos-botnet-spreads-to-200k-devices-worldwide/">New Dysphoria DDoS botnet spreads to 200k devices worldwide</a></li>
<li><a href="https://www.linux.org.hk/archive/20260727-3618-dysphoria-iot-botnet-adds-blockchain-c2.html">Dysphoria IoT Botnet Adds Blockchain C2 and Victim Relays ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#botnet`, `#DDoS`, `#malware`

---

<a id="item-19"></a>
## [Certighost 概念验证漏洞利用代码发布，可劫持 Windows 域](https://www.bleepingcomputer.com/news/security/new-certighost-poc-exploit-lets-attackers-hijack-windows-domains/) ⭐️ 8.0/10

Certighost 漏洞（CVE-2026-54121）的概念验证利用代码已公开发布，允许经过身份验证的攻击者滥用 Active Directory 证书服务，从而可能危及 Windows 域。 此利用代码直接威胁企业安全，因为 AD CS 是身份管理的核心组件。组织必须紧急应用微软 2026 年 7 月的补丁，以防止域级受损。 该漏洞利用 AD CS 中的回退机制，欺骗证书颁发机构颁发受信任的凭证。该 PoC 于 2026 年 7 月 24 日由研究人员 H0j3n 和 Aniq Fakhrul 在微软 7 月 14 日修补后发布。

rss · BleepingComputer · 7月27日 21:00

**背景**: Active Directory 证书服务 (AD CS) 是 Windows 服务器角色，用于颁发和管理数字证书以实现身份验证和加密。Certighost 漏洞 (CVE-2026-54121) 允许低权限用户通过操纵 AD CS 中的对象解析逻辑来提升权限并模拟域控制器，从而导致域完全受损。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thecybersecguru.com/news/certighost-cve-2026-54121-ad-cs-domain-controller-impersonation/">CertiGhost (CVE-2026-54121): AD CS Flaw Enables Domain ...</a></li>
<li><a href="https://www.csoonline.com/article/4201771/certighost-haunts-microsoft-active-directory-certificate-services.html">Certighost haunts Microsoft Active Directory Certificate ...</a></li>
<li><a href="https://denizhalil.com/2026/07/27/certighost-cve-2026-54121-adcs-privilege-escalation/">Certighost (CVE-2026-54121): AD CS Privilege Escalation</a></li>

</ul>
</details>

**标签**: `#security`, `#Windows`, `#Active Directory`, `#exploit`, `#vulnerability`

---

<a id="item-20"></a>
## [Spring Boot heapdump 端点泄露敏感机密](https://isc.sans.edu/diary/rss/33188) ⭐️ 8.0/10

Spring Boot 的 /actuator/heapdump 端点可被利用来下载堆转储文件，其中包含 API 密钥和数据库密码等敏感数据，构成重大安全风险。 许多开发者在生产环境中仍启用此调试端点而未加保护，可能导致数据泄露。所有启用该端点且未实施安全控制的 Spring Boot 应用都面临风险。 该端点返回一个二进制 .hprof 文件，捕获整个 JVM 堆内存，包括所有内存中的机密信息。攻击者可使用工具解析堆转储并提取凭据。

rss · SANS Internet Storm Center · 7月27日 10:04

**背景**: Spring Boot Actuator 提供了用于监控和管理应用的生产就绪端点。/actuator/heapdump 端点本用于调试内存问题，但常被默认启用。堆转储是 Java 对象在内存中的快照，类似于原生应用的核心转储。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baeldung.com/java-heap-dump-capture">Different Ways to Capture Java Heap Dumps | Baeldung</a></li>
<li><a href="https://docs.spring.io/spring-boot/reference/actuator/index.html">Production-ready Features :: Spring Boot</a></li>

</ul>
</details>

**标签**: `#Spring Boot`, `#security`, `#heapdump`, `#secrets exposure`

---