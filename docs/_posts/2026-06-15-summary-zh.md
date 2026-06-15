---
layout: default
title: "Horizon Summary: 2026-06-15 (ZH)"
date: 2026-06-15
lang: zh
---

> 从 37 条内容中筛选出 11 条重要资讯。

---

1. [里约热内卢自研大模型被发现是现有模型的混合体](#item-1)
2. [用本地 ML 在 M1 Max 上索引 669GB GoPro 视频](#item-2)
3. [形式化方法：代码验证的未来？](#item-3)
4. [AI 不会取代软件工程师，数据显示](#item-4)
5. [FBI 与 Google 及 Black Lotus Labs 捣毁 AI 驱动钓鱼服务](#item-5)
6. [小米 MiMo V2.5 利用 DFlash 实现 1000-3000 tps](#item-6)
7. [EAGLE 投机解码支持已合并到 llama.cpp](#item-7)
8. [双 DGX Spark 运行 DeepSeek V4 Flash 达到 40+ tk/s](#item-8)
9. [Kage：将任意网站归档为单个二进制文件供离线查看](#item-9)
10. [2014 年演讲预测 JavaScript 命运与全球灾难](#item-10)
11. [Paul Graham 谈如何创造亿万财富](#item-11)

---

<a id="item-1"></a>
## [里约热内卢自研大模型被发现是现有模型的混合体](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

一项调查发现，里约热内卢的 IT 公司 IplanRIO 发布的自研微调模型 Rio-3.5-Open-397B，实际上是大约 60%的 Nex-N2 Pro 和 40%的 Qwen3.5-397B-A17B 的加权混合，且未进行额外训练。 这一争议凸显了开源 AI 开发中透明度和适当归因的重要性，尤其是当政府实体声称自研创新时，可能削弱社区的信任。 Rio 模型中的每个权重张量在所有层和组件上都与 Nex 和 Qwen 的 0.6/0.4 混合相同，这种模式在其他微调模型中未见，表明未进行进一步训练。

hackernews · unrvl22 · 6月14日 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48528371)

**背景**: 模型合并是一种将多个微调 LLM 的权重组合以提高性能而无需额外训练的技术。这已成为开源社区的常见做法，但需要适当披露合并的模型。里约案例引发争议，因为市政实体将混合模型呈现为自研开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2408.07666">[2408.07666] Model Merging in LLMs, MLLMs, and Beyond ...</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs - NVIDIA Developer</a></li>

</ul>
</details>

**社区讨论**: 社区评论中既有解释也有批评：有人认为上传的模型可能不包含蒸馏步骤，而另一些人则谴责缺乏归因。详细的技术分析确认了所有层上的混合模式。

**标签**: `#AI`, `#LLM`, `#open-source`, `#model merging`, `#controversy`

---

<a id="item-2"></a>
## [用本地 ML 在 M1 Max 上索引 669GB GoPro 视频](https://news.ycombinator.com/item?id=48528029) ⭐️ 8.0/10

作者利用开源 ML 模型在 M1 Max 上构建本地管道，索引了 669GB 的 GoPro 视频，实现了基于文本的搜索并将精彩片段直接导出到达芬奇时间线。 该项目表明，在消费级硬件上进行强大且隐私保护的视频索引是可行的，减少了对云服务的依赖，并能从大量个人视频档案中高效检索内容。 该管道分析了 57,537 帧（每秒 1 帧），计算时间约 67.7 小时，使用了 Whisper 等模型进行转录和视觉模型进行场景描述。

hackernews · iliashad · 6月14日 15:13

**背景**: 传统视频索引依赖云端 AI 服务，引发隐私和成本问题。现在，像 M1 Max 这样包含专用媒体引擎的强大硬件上的本地 ML 模型，使得设备端处理变得可行。Whisper 和视觉 Transformer 等开源工具能够自动执行转录和场景分析，而无需将数据发送到设备外。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2021/10/introducing-m1-pro-and-m1-max-the-most-powerful-chips-apple-has-ever-built/">Introducing M1 Pro and M1 Max: the most powerful ... - Apple</a></li>
<li><a href="https://github.com/byjlw/video-analyzer">GitHub - byjlw/video-analyzer: Analyze videos using LLMs ...</a></li>
<li><a href="https://www.aitoolnet.com/edit-mind">Edit Mind - Local Video Indexer & AI Search - Aitoolnet</a></li>

</ul>
</details>

**社区讨论**: 评论中对本地 AI 能力表示兴奋，asenna 指出有类似项目。一些用户对计算时间提出实用性疑问，而另一些则指出 DaVinci Resolve 21 已内置 AI 索引（IntelliSearch）。少数人批评示例中的精彩片段不够精彩。

**标签**: `#machine learning`, `#video indexing`, `#local AI`, `#GoPro`, `#M1 Max`

---

<a id="item-3"></a>
## [形式化方法：代码验证的未来？](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street 的博客文章探讨了形式化方法在编程中的作用，特别是用于验证 AI 生成的代码，将人类工作从编写代码转变为验证。 随着 AI 生成大量代码，确保正确性变得至关重要；形式化方法提供数学保证来补充传统测试，可能改变软件可靠性的格局。 文章讨论了定理证明、类型系统和实践经验，社区评论提到了 Boyer-Moore 等历史证明助手和 Scala 3 中的现代方法，也对形式化规约是否只是另一种测试提出了质疑。

hackernews · eatonphil · 6月14日 12:35 · [社区讨论](https://news.ycombinator.com/item?id=48526633)

**背景**: 形式化方法是在数学上严谨的技术，用于规约、开发和验证软件与硬件系统。它们包括定理证明、模型检测和抽象解释，旨在证明正确性而不仅仅是测试错误。随着 AI 生成代码的兴起，验证成为瓶颈，形式化方法可以应对这一挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods</a></li>
<li><a href="https://web.mit.edu/16.35/www/lecturenotes/FormalMethods.pdf">Introducing Formal Methods - MIT</a></li>
<li><a href="https://arxiv.org/abs/2601.18944">[2601.18944] Neural Theorem Proving for Verification ... kindatechnical () | Formal Verification in Software ... Proof assistant - Wikipedia Different Theorem Proving System (TPS) - GeeksforGeeks formal.methods.08.theorem.proving.program.verification Automated theorem proving and proof verification Lean Programming Language</a></li>

</ul>
</details>

**社区讨论**: 社区评论观点不一：有人分享了在证明自动化方面的历史经验并指出所需的人力投入，也有人质疑形式化规约是否比测试更有价值，担心它们会复制同样的错误。一条评论强调形式化方法有助于防止 AI 生成代码中的“名词增生”。

**标签**: `#formal methods`, `#verification`, `#AI-generated code`, `#programming languages`, `#theorem proving`

---

<a id="item-4"></a>
## [AI 不会取代软件工程师，数据显示](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan 和 Sayash Kapoor 发表了一篇文章，认为数据并不支持 AI 导致软件工程大规模裁员的说法。他们指出，纽约州要求 WARN 法案文件中披露 AI 相关裁员的第一年，没有一家公司勾选 AI 选项。 这篇文章挑战了 AI 将消除软件工程工作的普遍担忧，表明该职业的核心涉及决策、责任和 AI 无法复制的深度人类理解。它为科技工作者提供了基于证据的安慰，并为 AI 对劳动力影响的政策辩论提供了信息。 作者指出了软件工程中的三个真正瓶颈：决定构建什么、验证并对交付物负责，以及对代码库、业务和环境的深度人类理解。他们指出，AI 加快了编码速度，但并未加快需要这些人类技能的更广泛的工程任务。

rss · Simon Willison · 6月14日 23:54

**背景**: 文章聚焦于软件工程这一因监管壁垒低而特别容易受到 AI 冲击的职业。尽管大型语言模型等 AI 技术取得了进步，但纽约州 WARN 法案的就业数据显示没有 AI 相关的裁员，这表明其他职业甚至更有保障。

**标签**: `#AI`, `#software engineering`, `#job displacement`, `#technology ethics`, `#labor market`

---

<a id="item-5"></a>
## [FBI 与 Google 及 Black Lotus Labs 捣毁 AI 驱动钓鱼服务](https://www.bleepingcomputer.com/news/security/fbi-disrupts-massive-ai-powered-phishing-service-using-a-million-urls/) ⭐️ 8.0/10

FBI 与 Google 及 Lumen 旗下 Black Lotus Labs 合作，捣毁了一个名为'Outsider Enterprise'的中国钓鱼即服务平台，该平台利用 AI 生成了超过一百万个恶意 URL。 此次行动凸显了 AI 在网络犯罪中日益增长的作用，以及公私合作在打击威胁全球用户的复杂大规模钓鱼操作方面的有效性。 该行动涉及数千个用于窃取信用卡数据和密码的钓鱼网站，协调努力导致了基础设施的查封和服务的中断。

rss · BleepingComputer · 6月14日 14:36

**背景**: 钓鱼即服务（PhaaS）是一种基于订阅的网络犯罪模式，熟练的攻击者提供现成的钓鱼工具包，包括虚假登录页面、电子邮件模板和托管服务，使即使是新手也能发起攻击。Black Lotus Labs 是 Lumen Technologies 旗下的威胁情报团队，利用全球网络可见性来检测和破坏恶意活动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Phishing_as_a_service">Phishing as a service</a></li>
<li><a href="https://www.lumen.com/en-us/security/black-lotus-labs.html">Black Lotus Labs | Lumen Technologies</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#phishing`, `#AI-powered`, `#FBI`, `#law enforcement`

---

<a id="item-6"></a>
## [小米 MiMo V2.5 利用 DFlash 实现 1000-3000 tps](https://www.reddit.com/r/LocalLLaMA/comments/1u5jtr8/xiaomi_is_now_serving_mimo_v25_at_10003000tps/) ⭐️ 8.0/10

小米宣布其 MiMo V2.5 模型利用 DFlash 和持久化内核技术实现了每秒 1000-3000 token 的推理速度。DFlash 模型已经发布，完整开源版本承诺即将推出。 这一性能突破可大幅降低大语言模型推理的延迟，使实时应用更加可行。开源发布的承诺可能加速高效推理方法在整个行业的采用。 加速归功于 DFlash，它使用草稿模型通过块扩散并行生成多个 token，并结合减少内核启动开销的持久化内核。该模型支持高达 100 万 token 的上下文和原生多模态理解。

reddit · r/LocalLLaMA · /u/Dany0 · 6月14日 12:26

**背景**: DFlash 是一种推测解码技术，通过并行预测多个 token 实现 3 倍更快的 LLM 推理，超越了 EAGLE 的 2 倍加速。持久化内核使 GPU 内核实例在多次启动间保持运行，以最小化调度开销。MiMo V2.5 是小米的全模态模型，具有智能体能力，支持文本、图像、视频和音频理解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baseten.co/blog/dflash-faster-llm-inference/">DFlash : 3x faster LLM inference</a></li>
<li><a href="https://mimo.xiaomi.com/mimo-v2-5">MiMo-V2.5 | Xiaomi</a></li>
<li><a href="https://huggingface.co/XiaomiMiMo/MiMo-V2.5">XiaomiMiMo/MiMo-V2.5 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#Xiaomi`, `#MiMo`, `#DFlash`, `#open-source`

---

<a id="item-7"></a>
## [EAGLE 投机解码支持已合并到 llama.cpp](https://www.reddit.com/r/LocalLLaMA/comments/1u5z4j0/eagle_support_merged_into_llamacpp/) ⭐️ 8.0/10

EAGLE 投机解码框架已合并到 llama.cpp 仓库中，使用户能够通过利用外推隐藏状态的草稿头来加速本地硬件上的 LLM 推理。 此次集成将最先进的投机解码方法引入最流行的本地 LLM 推理引擎之一，可使许多用户的延迟降低 2-3 倍，并使消费者硬件上的 LLM 推理更加快速。 EAGLE（Extrapolation Algorithm for Greater Language-model Efficiency）使用附加在目标模型层上的轻量级草稿头来每步预测多个令牌，包含多个版本：EAGLE-1（ICML'24）、EAGLE-2（EMNLP'24）和 EAGLE-3（NeurIPS'25）。

reddit · r/LocalLLaMA · /u/Diablo-D3 · 6月14日 22:45

**背景**: 投机解码是一种针对大型语言模型的推理时优化技术：一个小型草稿模型提出多个候选令牌，然后目标模型在单次前向传播中验证它们。该技术保留了原始输出分布，同时将延迟降低约 2-3 倍。EAGLE 相较于 Medusa 等早期方法的改进在于，它通过从目标模型的隐藏状态进行外推，而不是使用单独的草稿模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/EAGLE_speculative_decoding">EAGLE (speculative decoding)</a></li>
<li><a href="https://arxiv.org/abs/2401.15077">[2401.15077] EAGLE: Speculative Sampling Requires Rethinking Feature Uncertainty</a></li>
<li><a href="https://github.com/SafeAILab/EAGLE">GitHub - SafeAILab/EAGLE: Official Implementation of EAGLE-1 (ICML'24), EAGLE-2 (EMNLP'24), and EAGLE-3 (NeurIPS'25). · GitHub</a></li>

</ul>
</details>

**标签**: `#llama.cpp`, `#EAGLE`, `#speculative decoding`, `#LLM inference`, `#performance optimization`

---

<a id="item-8"></a>
## [双 DGX Spark 运行 DeepSeek V4 Flash 达到 40+ tk/s](https://www.reddit.com/r/LocalLLaMA/comments/1u5g9pr/dual_dgx_sparks_40tks_single_1m_350_tks_agg/) ⭐️ 8.0/10

这证明大型 MoE 模型可以以适合智能体使用的速度本地运行，缩小了高级 AI 应用中本地推理和云端推理之间的差距。 该配置需要一根 180 美元的线缆，通过 ConnectX-7 网卡实现 200 Gb/s 连接，并使用 FP8 量化和 vLLM。基准测试显示，其聚合吞吐量优于 RTX Pro 6000 和 Mac M2 Ultra。

reddit · r/LocalLLaMA · /u/elsung · 6月14日 09:07

**背景**: NVIDIA DGX Spark 是一款紧凑型 AI 超级计算机，提供千万亿次 AI 性能和 128GB 统一内存，专为边缘 AI 和本地推理设计。DeepSeek V4 Flash 是 DeepSeek V4 的高效变体，优化了推理速度，同时将质量损失降至最低。ConnectX-7 是一种高性能网卡，支持高达 400 Gb/s 的传输速率，可实现低延迟的多节点连接。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DGX_Spark">DGX Spark</a></li>
<li><a href="https://codersera.com/blog/run-deepseek-v4-flash-locally-full-2026-setup-guide/">Run DeepSeek V4 Flash Locally: Full 2026 Setup Guide</a></li>
<li><a href="https://grokipedia.com/page/NVIDIA_ConnectX-7">NVIDIA ConnectX-7</a></li>

</ul>
</details>

**社区讨论**: 该帖子感谢了社区贡献者 Aiden 和 Antirez，并包含详细的基准测试和提供配置方法的 GitHub 仓库。总体反馈积极，用户称赞这一成就是在大型 MoE 模型本地推理方面的一个里程碑。

**标签**: `#deepseek`, `#dgx-spark`, `#local-llm`, `#inference-speed`, `#multi-node`

---

<a id="item-9"></a>
## [Kage：将任意网站归档为单个二进制文件供离线查看](https://github.com/tamnd/kage) ⭐️ 7.0/10

Kage 是一款新的命令行工具，可将任意网站转换为单个可执行二进制文件以供离线查看，并可选生成演示 GIF。 这通过将整个站点打包到一个二进制文件中简化了离线网页存档，无需服务器或网络连接即可轻松共享和查看。 该工具使用单独的 serve 命令来查看存档，演示 GIF 由同一作者的另一个项目 ascii-gif 生成。

hackernews · tamnd · 6月14日 17:25 · [社区讨论](https://news.ycombinator.com/item?id=48529990)

**背景**: 像 SingleFile 这样的网页存档工具将页面保存为单个 HTML 文件，而 Kage 则创建一个包含所有资源的二进制文件。这种方法对于在没有网络连接的地方离线访问文档、原型或维基很有用。

**社区讨论**: 评论者表示对使用 Kage 归档原型和公司维基很感兴趣。一些建议改进，例如无需单独服务器即可查看存档，并认为其在简单性上优于 SingleFile，但指出 SingleFile 更强大。

**标签**: `#offline`, `#web-archiving`, `#CLI-tool`, `#open-source`

---

<a id="item-10"></a>
## [2014 年演讲预测 JavaScript 命运与全球灾难](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript) ⭐️ 7.0/10

Gary Bernhardt 在 2014 年的演讲《JavaScript 的诞生与死亡》预测 JavaScript 将成为编译目标，并预见了 2020-2025 年间的一场全球灾难；随着 WebAssembly 的兴起和 COVID-19 大流行，这些预测正被重新审视。 该演讲证明具有惊人的先见性：JavaScript 确实通过 asm.js 和后来的 WebAssembly 成为编译目标，而一场全球灾难（COVID-19）也在预测的时间范围内发生；这凸显了预测技术演进的难度以及某些预测的惊人准确性。 该演讲设想了一种未来，JavaScript 仅用作中间表示，开发者使用其他语言编写并编译为 JS；它还戏谑地预测了一场由 JavaScript 运行时漏洞引发的全球灾难，评论者指出这与大流行相似。

hackernews · subset · 6月14日 12:38 · [社区讨论](https://news.ycombinator.com/item?id=48526661)

**背景**: Asm.js 于 2013 年引入，是 JavaScript 的一个严格子集，旨在作为 C/C++等语言的编译目标，使其能在浏览器中高效运行。随后 WebAssembly 取代了 asm.js，提供了一种以接近原生速度运行的二进制格式。Emscripten 是一个编译器工具链，可将 C/C++代码转换为 WebAssembly 或 asm.js。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asm.js">Asm.js</a></li>
<li><a href="https://en.wikipedia.org/wiki/Emscripten">Emscripten</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Games/Tools/asm.js">asm.js - Game development | MDN</a></li>

</ul>
</details>

**社区讨论**: 评论者注意到该演讲对 2020-2025 年间全球灾难的诡异预测，有人说‘他预测错了类型，这很 JavaScript。’其他人讨论了 WebAssembly 进展缓慢以及仍需 JavaScript 胶水代码，还有人称该演讲为‘杰作’。

**标签**: `#javascript`, `#webassembly`, `#future of web`, `#historical analysis`, `#community discussion`

---

<a id="item-11"></a>
## [Paul Graham 谈如何创造亿万财富](https://paulgraham.com/earn.html) ⭐️ 7.0/10

Paul Graham 发表了一篇题为《如何赚十亿美元》的文章，认为初创公司可以通过创新和创造价值合法地创造巨额财富，这引发了 Hacker News 上的激烈辩论。 这篇文章突显了硅谷围绕财富不平等和极端财富积累伦理的持续紧张关系，影响着企业家和公众如何看待初创公司的成功。 这篇文章在 Hacker News 上获得了 417 个点赞和 1262 条评论，显示出极高的参与度；讨论揭示了两种对立的观点，有人为财富的道德性辩护，也有人批评财富掠夺。

hackernews · kingstoned · 6月14日 11:50 · [社区讨论](https://news.ycombinator.com/item?id=48526360)

**背景**: Paul Graham 是著名创业加速器 Y Combinator 的联合创始人。他的文章经常塑造创业思维。这场辩论涉及的是：十亿美元的财富是通过创造价值“赚来的”，还是涉及剥削，这是经济讨论中反复出现的主题。

**社区讨论**: 评论者表达了复杂的情绪：有人为 Graham 的观点辩护，认为初创公司创造真正的价值；也有人批评该文章忽视了负面外部性，如就业岗位流失和财富掠夺。还有少数人指出'赚取'一词在语义上的差异。

**标签**: `#wealth`, `#startups`, `#paul-graham`, `#economics`, `#entrepreneurship`

---