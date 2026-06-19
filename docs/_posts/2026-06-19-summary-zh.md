---
layout: default
title: "Horizon Summary: 2026-06-19 (ZH)"
date: 2026-06-19
lang: zh
---

> 从 75 条内容中筛选出 20 条重要资讯。

---

1. [Noam Shazeer 加入 OpenAI](#item-1)
2. [CISA 敦促立即加固 Fortinet 设备应对 FortiBleed 漏洞](#item-2)
3. [Rust 实现安全 GPU 推理，性能媲美 vLLM](#item-3)
4. [发现 1 万个 GitHub 仓库分发特洛伊木马](#item-4)
5. [Elkjøp 因强制同意作为会员条件被罚 180 万欧元](#item-5)
6. [药物再利用大幅降低成本](#item-6)
7. [W Social 具有可信度吗？欧洲数字主权闹剧的批评](#item-7)
8. [Modos 推出 60Hz 彩色电子纸显示器](#item-8)
9. [Gerrymandle：每日重划选区拼图游戏](#item-9)
10. [GLM-5.2 引入 IndexShare 实现百万 Token 稀疏推理](#item-10)
11. [恶意软件注入违禁文本逃避 AI 分析](#item-11)
12. [CISA 报告施耐德电气多款 ICS 产品存在漏洞](#item-12)
13. [CISA 警告罗克韦尔历史数据库严重漏洞](#item-13)
14. [AVer PTC 摄像头存在严重 RCE 漏洞](#item-14)
15. [CISA 警告施耐德 RTU 存在路径遍历漏洞](#item-15)
16. [F5 发布补丁修复 NGINX 关键远程代码执行漏洞](#item-16)
17. [微软披露利用 USB LNK 和 Tor C2 的 Windows 剪贴板恶意软件](#item-17)
18. [DragonForce 黑客滥用 Microsoft Teams 中继隐藏 C2 流量](#item-18)
19. [Klue OAuth 漏洞导致 Icarus 窃取 Salesforce 数据](#item-19)
20. [警方清理近 1.5 万个与 Evil Corp 相关的 SocGholish 感染网站](#item-20)

---

<a id="item-1"></a>
## [Noam Shazeer 加入 OpenAI](https://twitter.com/NoamShazeer/status/2067400851438932297) ⭐️ 9.0/10

Noam Shazeer，里程碑论文《Attention Is All You Need》的合著者、前谷歌 Gemini 联合负责人，于 2026 年 6 月 18 日加入 OpenAI。 此举意义重大，因为 Shazeer 是 transformer 架构（现代大多数 AI 系统的基础）的关键人物。他加入 OpenAI 可能加速其研发，并可能重塑 OpenAI 与谷歌之间的竞争格局。 Shazeer 此前于 2024 年通过与 Character.AI（他联合创立的公司）的许可/人才协议重返谷歌，据报道该交易价值 27 亿美元。他随后担任 Gemini 联合负责人，之后再次离开加入 OpenAI。

hackernews · lukasgross · 6月18日 00:26 · [社区讨论](https://news.ycombinator.com/item?id=48578913)

**背景**: Noam Shazeer 是 2017 年论文《Attention Is All You Need》的八位合著者之一，该论文提出了 transformer 模型——一种彻底改变自然语言处理的神经网络架构。他在谷歌工作了二十多年，随后离开并联合创立了聊天机器人公司 Character.AI。他重返谷歌的时间很短，此次加入 OpenAI 标志着顶尖 AI 人才的持续流动。

**社区讨论**: 社区对 Shazeer 在重返谷歌后不久再次离开表示惊讶，猜测其可能原因是他的政治言论。一些评论者提供了他的职业背景，其他人则分享了进一步讨论的链接。

**标签**: `#AI`, `#OpenAI`, `#Google`, `#transformer`, `#machine learning`

---

<a id="item-2"></a>
## [CISA 敦促立即加固 Fortinet 设备应对 FortiBleed 漏洞](https://www.cisa.gov/news-events/alerts/2026/06/18/cisa-urges-hardening-fortinet-devices-after-reports-credential-exposure) ⭐️ 9.0/10

2026 年 6 月 18 日，CISA 发布紧急通告，要求所有 Fortinet 客户立即加固其 FortiGate 防火墙和 SSL VPN 网关，原因是名为 FortiBleed 的全球凭证泄露活动已暴露约 74,000 台设备的凭证。 该通告标志着一项针对政府和私营部门广泛使用的 Fortinet 设备的严重活跃威胁，攻击者可能通过泄露的 VPN 凭证获得未授权网络访问。受影响组织需立即采取行动，防止数据泄露和横向移动。 CISA 建议五项具体措施：终止所有活跃会话并重置凭证、强制使用 PBKDF2 密码哈希算法、审查日志可疑活动、启用抗钓鱼多因素认证，以及通过限制管理接口暴露来缩小攻击面。值得注意的是，FortiBleed 并非需要补丁的漏洞，而是利用已暴露的凭证，因此未分配 CVE 编号。

rss · CISA Cybersecurity Advisories · 6月18日 12:00

**背景**: FortiGate 是 Fortinet 公司流行的下一代防火墙，常被用作远程访问的 SSL VPN 网关。FortiBleed 活动指约 74,000 台面向互联网的 Fortinet 设备凭证被泄露，这些凭证可能通过恶意软件或之前的入侵获取。PBKDF2 是一种密钥派生函数，通过多次加盐哈希密码来显著减慢密码破解速度，使存储的凭证更难被利用。该通告强调切换到 PBKDF2 以替换较弱的旧版哈希。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://socradar.io/blog/socradar-free-fortibleed-exposure-checker/">SOCRadar Launches Free FortiBleed Exposure Checker and Publishes the Most Extensive Dataset on the Fortinet Credential Leak</a></li>
<li><a href="https://cybelangel.com/blog/fortibleed-6-things-to-know/">FortiBleed: 6 Things to Know About the Fortinet Credential Leak</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pbkdf2">PBKDF2 - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#CISA`, `#Fortinet`, `#credential exposure`, `#VPN security`

---

<a id="item-3"></a>
## [Rust 实现安全 GPU 推理，性能媲美 vLLM](https://www.reddit.com/r/MachineLearning/comments/1u9j7md/fearless_concurrency_on_the_gpu_safe_gpu/) ⭐️ 9.0/10

论文介绍了 cuTile Rust 和 Grout，这是一个利用 Rust 的所有权模型保证 GPU 内核内存安全和无数据竞争的推理引擎，吞吐量可与 vLLM 和 SGLang 媲美。 随着 GPU 代码越来越多由 AI 生成，确保其可信性至关重要；这项工作提供了一种编写安全、高性能 GPU 内核的实用方法，可能减少 AI/ML 系统中的错误和安全漏洞。 Grout 目前仅支持 batch-1 推理和 NVIDIA GPU，代码降级到 CUDA Tile IR。虽然大部分内核仍使用不安全路径，但可以迁移到安全变体，安全 GEMM 性能与手写内核相差不到 0.3%。

reddit · r/MachineLearning · /u/Exciting_Suspect9088 · 6月18日 21:36

**背景**: cuTile Rust 是一个基于 tile 的 GPU 编程库，将 Rust 的所有权和借用规则扩展到 GPU 内核，在编译时确保内存安全。它降级到 CUDA Tile IR，这是一种用于基于 tile 的 GPU 计算的底层中间表示。Grout 是构建在 cuTile Rust 上的研究性推理引擎，演示了 Qwen3 模型的端到端安全推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/NVlabs/cutile-rs">GitHub - NVlabs/cutile-rs: cuTile Rust provides a safe, tile ...</a></li>
<li><a href="https://arxiv.org/abs/2606.15991">[2606.15991] Fearless Concurrency on the GPU</a></li>
<li><a href="https://docs.nvidia.com/cuda/tile-ir/latest/index.html">Tile IR — Tile IR - NVIDIA Documentation Hub</a></li>

</ul>
</details>

**标签**: `#Rust`, `#GPU Programming`, `#Machine Learning`, `#Memory Safety`, `#CUDA`

---

<a id="item-4"></a>
## [发现 1 万个 GitHub 仓库分发特洛伊木马](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 8.0/10

一名研究人员发现了约 1 万个 GitHub 仓库正在分发特洛伊木马，利用自动化代理攻击软件供应链。 这种大规模的攻击构成严重的供应链风险，可能影响成千上万的软件项目和用户。随着重大选举临近，这一时机加剧了对虚假信息和数字破坏的担忧。 该攻击专门针对自动化代理（如 AI 编码助手和 CI/CD 流水线），而非人类用户。恶意仓库从合法项目克隆，并频繁更新以保持可见性。

hackernews · theorchid · 6月18日 11:45 · [社区讨论](https://news.ycombinator.com/item?id=48583928)

**背景**: 软件供应链攻击涉及将恶意代码注入受信任的软件组件。GitHub 是开源协作的主要平台，但其易复制的特点使攻击者能够通过创建看似合法的仓库来传播恶意软件，这些仓库会被代理自动发现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cyberadviserblog.com/2024/05/xz-utils-supply-chain-attack-sheds-light-on-vulnerabilities-in-widely-adopted-open-source-system/">XZ Utils Supply Chain Attack Sheds Light on Vulnerabilities in Widely Adopted Open Source System | CyberAdviser</a></li>
<li><a href="https://www.microsoft.com/en-us/securityengineering/opensource/ossthreats">OSS Supply Chain Threats</a></li>

</ul>
</details>

**社区讨论**: 社区表达了警惕，并分享了个人项目被劫持的经历。评论者讨论了攻击的复杂程度，指出其针对的是自动化代理而非人类，并将其与选举安全和 AI 工具完整性的更广泛担忧联系起来。

**标签**: `#malware`, `#supply-chain-attack`, `#github`, `#cybersecurity`, `#open-source`

---

<a id="item-5"></a>
## [Elkjøp 因强制同意作为会员条件被罚 180 万欧元](https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/) ⭐️ 8.0/10

挪威数据保护局对电子零售商 Elkjøp 处以 180 万欧元罚款，原因是该公司要求顾客同意接收营销信息作为加入其客户俱乐部的条件，违反了 GDPR 关于同意必须自由给予的规定。 这一里程碑式的执法确认了在 GDPR 下将同意与服务访问捆绑是非法的，为各公司重新评估其在忠诚度计划及类似方案中的同意实践树立了先例。 罚款源于 Elkjøp 回复中的一句话：“为了接收营销/优惠，成为客户俱乐部会员是一个条件。”数据保护局认为这使同意变得有条件且无效。该案件从投诉到最终裁决历时五年。

hackernews · speckx · 6月18日 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48589501)

**背景**: 根据《通用数据保护条例》（GDPR），数据处理的同意必须是自由给予的、具体的、知情的且明确的。强制同意，即同意数据使用是获得服务的先决条件，不被视为自由给予。挪威数据保护局以优先考虑用户隐私权而闻名。

**社区讨论**: 评论者赞赏该个人的坚持，并指出挪威数据保护局一贯做出对用户有利的裁决。一些人表示，行使隐私权常常使个人处于不利地位，尤其是在美国。评论中分享了官方裁决和翻译的链接以帮助理解。

**标签**: `#GDPR`, `#privacy`, `#consent`, `#data protection`, `#tech regulation`

---

<a id="item-6"></a>
## [药物再利用大幅降低成本](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

医院和大学正在重新利用现有药物，例如用抗癌药治疗黄斑变性，成本比开发新药或使用品牌替代品低达 90%。 这挑战了高昂的药品定价模式，可能使治疗更可及和负担得起，尤其对于罕见病——开发新药无利可图。 例如，Avastin（贝伐珠单抗）治疗黄斑变性每剂约 50 美元，而类似且专为眼部注射包装的 Lucentis 每剂约 1500 美元。但未经制造商同意，仍存在监管和制造障碍。

hackernews · giuliomagnifico · 6月18日 10:33 · [社区讨论](https://news.ycombinator.com/item?id=48583386)

**背景**: 药物再利用（Drug repurposing）是指研究现有药物的新治疗用途。由于药物安全性已知，可减少时间和成本，并跳过早期研究阶段。这一策略对忽略疾病和罕见病尤其有价值。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Drug_repurposing">Drug repurposing</a></li>
<li><a href="https://www.nature.com/articles/nrd.2018.168">Drug repurposing: progress, challenges and recommendations | Nature Reviews Drug Discovery</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了具体例子，如 Avastin 与 Lucentis 以及艾司氯胺酮（Spravato）与氯胺酮，指出专利修改如何抬高成本。一些人表达了对 Cures Within Reach 等非营利组织的支持，而另一些人指出监管障碍阻碍了在没有制造商合作的情况下更广泛采用。

**标签**: `#drug repurposing`, `#healthcare innovation`, `#pharmaceutical pricing`, `#drug development`, `#macular degeneration`

---

<a id="item-7"></a>
## [W Social 具有可信度吗？欧洲数字主权闹剧的批评](https://blog.elenarossini.com/w-social-public-institutions-and-the-theater-of-european-digital-sovereignty/) ⭐️ 8.0/10

一篇批评性的博文质疑欧洲社交网络 W Social 的真实性，并将其与基于 AT Protocol 的开源非营利替代方案 Eurosky 进行对比。 这一分析引发了关于欧洲数字主权努力是真实的还是政治表演的辩论，强调了公共机构在平台选择中透明度的重要性。 W Social 是一家有限责任公司，创始人来自金融行业；而由 Stichting Modal 运营的 Eurosky 完全透明，拥有公开路线图。博文指出，W Social 获得了大量媒体报道和欧盟高级政客的支持，而 Eurosky 并未获得同等关注。

hackernews · nemoniac · 6月18日 12:46 · [社区讨论](https://news.ycombinator.com/item?id=48584497)

**背景**: AT Protocol（ATproto）是一种用于社交网络的去中心化协议，最初由 Bluesky 开发。它支持用户可移植性和互操作性。Eurosky 是一个基于 ATproto 的欧洲网络，由一家非营利基金会运营；而 W Social 是一个商业闭源平台，声称支持欧洲数字主权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AT_Protocol">AT Protocol</a></li>
<li><a href="https://eurosky.tech/">Eurosky - Building a thriving open social web for Europe</a></li>

</ul>
</details>

**社区讨论**: 社区评论对 W Social 持高度怀疑态度，将其比作‘带欧洲口音的 TruthSocial’，并指出其创始人的金融背景。用户质疑其突然获得的媒体报道和政客支持，认为它可能是政治工具而非真正的开放平台。

**标签**: `#European digital sovereignty`, `#social media`, `#W Social`, `#AT Protocol`, `#policy`

---

<a id="item-8"></a>
## [Modos 推出 60Hz 彩色电子纸显示器](https://spectrum.ieee.org/modos-e-paper-monitor) ⭐️ 8.0/10

两人初创公司 Modos 开发了一款 13.3 英寸彩色电子纸显示器，分辨率为 3200x2400，刷新率达 60Hz，目前正在筹集生产资金。 这款显示器显著推动了电子纸技术的发展，使其适用于一般计算任务和户外使用，相比 LCD/OLED 可能减轻眼疲劳并降低功耗。 该显示器采用 Carta 电子纸面板，支持触摸输入并通过 USB-C 连接。高刷新率可能影响电子纸介质的寿命，因为其物理特性会随时间退化。

hackernews · Vinnl · 6月18日 11:41 · [社区讨论](https://news.ycombinator.com/item?id=48583897)

**背景**: 电子纸是一种反射式显示技术，利用环境光，仅在图像变化时耗电。传统电子纸刷新率较低（约 10-15 Hz），但近年 Dasung 等厂商推出了 60Hz 面板，突破了这一限制。Modos 的显示器将高分辨率、彩色和 60Hz 刷新率集成于便携形态中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.androidauthority.com/modos-flow-e-ink-paper-60hz-display-3677057/">Someone made a portable 60Hz E-Ink display that you can game on - Android Authority</a></li>
<li><a href="https://www.theverge.com/2025/1/23/24350334/dasung-paperlike-103-display-monitor-screen-e-ink-60hz">Dasung’s new portable E Ink monitor has a 60Hz refresh rate | The Verge</a></li>
<li><a href="https://www.flatpanelshd.com/news.php?subaction=showfull&id=1738737073">Samsung's new 75" display has near-zero power... - FlatpanelsHD</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区对 Modos 的规格感到兴奋，有人认为这是电子纸响应速度的一大进步。但也有担忧认为 60Hz 下面板寿命可能缩短，因为每个像素的机械切换有寿命限制。其他人则对替代显示技术实现低功耗户外设备持乐观态度。

**标签**: `#e-paper`, `#display technology`, `#hardware`, `#startup`, `#innovation`

---

<a id="item-9"></a>
## [Gerrymandle：每日重划选区拼图游戏](https://gerrymandle.cc/) ⭐️ 8.0/10

“Gerrymandle”游戏在 Hacker News 上发布，这是一款每日拼图游戏，玩家通过重新划分选区来争取更公平的结果，同时了解不公正选区划分的概念。 它以有趣且易于上手的方式引发了关于选举公平性和不公正选区划分的重要讨论，有可能成为公民教育课堂的教学工具。 游戏设定了一条规则：如果一个选区出现平局，则没有人赢得该选区——这虽是简化，但有助于传达核心概念。游戏重在趣味性而非完全的现实主义。

hackernews · realmofthemad · 6月18日 14:16 · [社区讨论](https://news.ycombinator.com/item?id=48585739)

**背景**: 不公正选区划分（gerrymandering）是指为了给某一政党或群体带来不公平的优势而操纵选区边界的行为。这种做法破坏了选举的公平性和代表性。这款游戏通过交互式拼图模拟这一过程，让玩家体验其复杂性。

**社区讨论**: 评论区称赞该游戏的创意设计及其作为课堂活动的潜力，有人建议用于高中公民教育。也有人指出平局规则不够现实，但可以接受。还有人分享了关于公平选区划分的数学解决方案。

**标签**: `#puzzle`, `#gerrymandering`, `#education`, `#civics`, `#game`

---

<a id="item-10"></a>
## [GLM-5.2 引入 IndexShare 实现百万 Token 稀疏推理](https://sebastianraschka.com/blog/2026/glm-5-2-indexshare.html) ⭐️ 8.0/10

GLM-5.2 是开源权重模型的更新，引入了 IndexShare——一种跨层共享索引的稀疏注意力机制，通过跨解码器层复用路由索引，实现了百万 Token 的高效推理，降低了路由开销。 这一进展降低了开源权重模型处理长文本推理的成本，解决了百万 Token 序列处理中的关键扩展瓶颈。它有望推动文档分析、代码仓库等长输入场景的实际应用。 IndexShare 基于 YOCO 架构，跨层共享 KV 缓存和路由索引，避免了重复的密集全局注意力和重计算。该稀疏注意力专门用于 DSA（直接稀疏注意力）推理，针对高达 100 万 Token 的上下文窗口。

rss · Sebastian Raschka · 6月18日 09:16

**背景**: 大型语言模型（LLM）以称为 token 的块处理输入；上下文窗口决定了模型一次能考虑多少 token。长上下文推理计算成本高昂，因为标准注意力机制随序列长度呈二次方扩展。稀疏注意力通过仅关注相关 token 子集来降低成本，但路由开销可能成为瓶颈。IndexShare 通过一次计算 token 级 top-k 选择并在各层复用索引来分摊路由开销。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.06467v1">[2606.06467v1] You Only Index Once: Cross-Layer Sparse Attention with Shared Routing</a></li>
<li><a href="https://www.latent.space/p/ainews-glm-52-the-top-frontend-coding">[AINews] GLM-5.2: the top Frontend Coding model in the world, IndexShare for Speculative Decoding</a></li>

</ul>
</details>

**标签**: `#long-context attention`, `#sparse attention`, `#GLM`, `#open-weight model`, `#efficient inference`

---

<a id="item-11"></a>
## [恶意软件注入违禁文本逃避 AI 分析](https://www.schneier.com/blog/archives/2026/06/embedding-forbidden-text-in-spyware-to-discourage-ai-analysis.html) ⭐️ 8.0/10

恶意软件开发者正在向间谍软件中嵌入关于核武器和生物武器的文本，以欺骗 AI 分析工具拒绝处理该代码，该发现最初由 Socket.dev 的研究人员报告。有效载荷以一个大型 JavaScript 块注释开头，其中包含虚假的系统指令和触发政策的内容，导致 AI 扫描器忽略实际的恶意代码。 这种新颖的逃避技术利用了 AI 语言模型内置的安全过滤和拒绝机制，可能削弱 AI 驱动的恶意软件分析流程。如果成功，可能导致一波类似的对抗性攻击，迫使安全工具重新设计处理不可信输入的方式。 违禁文本被放置在 JavaScript 块注释 (/* ... */) 内，因此不影响运行时执行，但会迷惑那些将文件开头直接输入语言模型而未隔离不可信数据的 AI 模型。实际恶意代码随后以一个包含字符代码数组和 ROT 风格替换函数的 try{eval(...)}包装器开始。

rss · Schneier on Security · 6月18日 11:04

**背景**: 基于 AI 的恶意软件分析通常使用语言模型检查代码片段，但这些模型具有安全过滤器，拒绝处理与大规模杀伤性武器等主题相关的内容。对抗性样本——精心设计以导致误分类的输入——是机器学习系统已知的漏洞，而这种技术是针对内容过滤器而非分类边界的新变种。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2412.12217v1">Comprehensive Survey on Adversarial Examples in Cybersecurity: Impacts ...</a></li>
<li><a href="https://ieeexplore.ieee.org/document/10806701">A Survey on Adversarial Attacks for Malware Analysis</a></li>

</ul>
</details>

**标签**: `#malware`, `#AI security`, `#evasion`, `#cybersecurity`

---

<a id="item-12"></a>
## [CISA 报告施耐德电气多款 ICS 产品存在漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-07) ⭐️ 8.0/10

CISA 于 2026 年 6 月 18 日发布公告（ICSA-26-169-07），详细说明了施耐德电气 Easergy、EcoStruxure、PowerLogic 和 Saitel 产品中的多个漏洞，主要是标记为 CVE-2026-4827 的不当输入验证缺陷。 这些漏洞可能使攻击者能够破坏依赖施耐德电气工业控制系统的关键基础设施环境中的运行，并访问敏感数据。立即修补对于防止潜在利用至关重要。 该公告列出了数十个受影响的产品版本，包括 Easergy MiCOM 继电器、EcoStruxure 电力自动化系统、PowerLogic 保护继电器和 Saitel 设备，固件版本均低于特定阈值。施耐德电气已在公告中提供了补救指南。

rss · CISA Cybersecurity Advisories · 6月18日 12:00

**背景**: 施耐德电气是能源管理和自动化领域的全球领导者，提供广泛应用于关键基础设施的工业控制系统（ICS）。通用安全咨询框架（CSAF）标准允许 CISA 发布机器可读的公告，促进自动化漏洞管理。不当的输入验证漏洞可能允许攻击者注入恶意数据，从而导致系统崩溃或未授权访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.se.com/us/en/product-range/137943580-powerchute-serial-shutdown/">PowerChute Serial Shutdown | Schneider Electric USA</a></li>
<li><a href="https://www.schneider-electric.com/en/product-range-presentation/60772-easergy-micom-p63x">Easergy MiCOM P63x | Schneider Electric</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#ICS`, `#Schneider Electric`, `#OT security`

---

<a id="item-13"></a>
## [CISA 警告罗克韦尔历史数据库严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-03) ⭐️ 8.0/10

CISA 发布了关于罗克韦尔自动化 FactoryTalk Historian Site Edition (SE) 版本 11 及更早版本中三个漏洞（CVE-2025-13036、CVE-2025-44019、CVE-2025-36539）的公告，这些漏洞可能导致身份验证令牌被盗、拒绝服务或系统崩溃。 FactoryTalk Historian SE 在全球关键制造业中广泛使用，最高评分漏洞 (CVSS 7.7) 允许绕过身份验证，可能使攻击者能够未经授权访问敏感的工业数据和控制系统。 这些漏洞包括竞态条件 (CWE-362) 和未捕获异常问题；对于 CVE-2025-13036，攻击者可反复向登录端点发送请求以获取有效身份验证令牌。罗克韦尔已发布补丁 (BF32850)，并建议升级到已修复版本。

rss · CISA Cybersecurity Advisories · 6月18日 12:00

**背景**: FactoryTalk Historian Site Edition 是一种工业数据历史记录软件，用于捕获、存储和分析来自制造设备的时间序列数据。它通常部署在制造业等关键基础设施领域。这些漏洞是 CISA 作为其工业控制系统 (ICS) 公告的一部分披露的，旨在提醒运营商注意运营技术中的安全缺陷。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rockwellautomation.com/en-us/products/software/factorytalk/operationsuite/historian/site-edition.html">FactoryTalk Historian Site Edition - Rockwell Automation</a></li>
<li><a href="https://www.rockwellautomation.com/en-us/products/software/factorytalk/operationsuite/historian.html">Operational Historian Software | FactoryTalk | US - Rockwell Automation</a></li>
<li><a href="https://www.rockwellautomation.com.cn/products/software/factorytalk/operationsuite/historian/site-edition.html">FactoryTalk Historian Site Edition - Rockwell Automation</a></li>

</ul>
</details>

**标签**: `#security`, `#industrial control systems`, `#Rockwell Automation`, `#vulnerability`, `#CISA`

---

<a id="item-14"></a>
## [AVer PTC 摄像头存在严重 RCE 漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-01) ⭐️ 8.0/10

CISA 披露了影响多个 AVer PTC 摄像头型号（包括 PTC500S、PTC115、PTC500+和 PTC115+）的严重远程代码执行漏洞（CVE-2026-40624），CVSS 评分为 9.8。 这些摄像头广泛部署在全球政府、商业和医疗设施中，该漏洞允许未经身份验证的远程攻击者执行任意代码，对关键基础设施构成重大风险。 该漏洞源于输入验证不当（CWE-552），通过特制 Web 请求导致任意代码执行，AVer 已发布固件修复程序。

rss · CISA Cybersecurity Advisories · 6月18日 12:00

**背景**: AVer PTC 摄像头是用于视频会议、教育和广播的专业自动跟踪 PTZ 摄像头。PTZ 摄像头支持远程平移、倾斜和变焦控制。通用安全公告框架（CSAF）是一种用于漏洞披露的机器可读格式，CISA 在此公告中使用了该格式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://presentation.aver.com/model/ptc500s">PTC500S - Professional Auto Tracking Camera | AVer Global</a></li>
<li><a href="https://www.csaf.io/">Common Security Advisory Framework (CSAF) | Home</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CISA`, `#IoT`, `#camera`

---

<a id="item-15"></a>
## [CISA 警告施耐德 RTU 存在路径遍历漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-169-04) ⭐️ 8.0/10

CISA 发布了咨询报告 ICSA-26-169-04，披露了施耐德电气 EasyLogic T150 和 Saitel DP RTU 固件中存在一个路径遍历漏洞（CVE-2026-6865），该漏洞可能导致未经授权访问敏感文件。 该漏洞影响广泛部署于能源和关键制造业的远程终端单元，可能暴露工业控制系统（ICS）和运营技术（OT）环境中的敏感数据。 该漏洞影响 EasyLogic T150 固件版本至 11.06.31 以及 Saitel DP 固件版本至 11.06.36；修复版本分别为 11.06.32 和 11.06.37，更新后需重启设备。

rss · CISA Cybersecurity Advisories · 6月18日 12:00

**背景**: 远程终端单元（RTU）是微处理器控制的设备，用于与远程地点的物理设备接口，常见于电网、油气管道和水务系统。路径遍历漏洞是指应用程序未能正确清理用户提供的文件路径，导致攻击者能够访问预期目录之外的文件。本咨询是 CISA 持续保护 ICS/OT 系统的一部分，此前该产品系列已披露过其他漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.se.com/uk/en/product-range/62685-easylogic-t150/">EasyLogic T150 - Schneider Electric UK</a></li>

</ul>
</details>

**标签**: `#vulnerability`, `#ICS`, `#cybersecurity`, `#Schneider Electric`

---

<a id="item-16"></a>
## [F5 发布补丁修复 NGINX 关键远程代码执行漏洞](https://thehackernews.com/2026/06/f5-patches-two-critical-nginx-open.html) ⭐️ 8.0/10

F5 发布了 NGINX Open Source 的带外安全更新，修复了两个严重漏洞，包括 CVE-2026-42530（CVSS 9.2），该漏洞允许远程未认证攻击者通过 ngx_http_v3_module 中的释放后使用缺陷执行代码。 这些严重漏洞影响了最广泛使用的 Web 服务器之一，可实现远程代码执行，可能导致系统完全被攻陷。依赖 NGINX 的组织必须立即打补丁。 漏洞 CVE-2026-42530 是 ngx_http_v3_module 中的释放后使用漏洞，该模块默认不构建，需通过 --with-http_v3_module 参数启用。成功利用需要服务器使用 HTTP/3 和 QUIC 协议。

rss · The Hacker News · 6月18日 17:32

**背景**: 释放后使用是一种内存破坏漏洞，程序在释放内存后继续使用指针，可能导致任意代码执行。ngx_http_v3_module 提供对 HTTP/3（基于 QUIC 的最新 HTTP 协议版本）的实验性支持。该模块是可选的，不在默认 NGINX 构建中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://my.f5.com/manage/s/article/K000161616">NGINX ngx_http_v3_module vulnerability CVE-2026-42530</a></li>
<li><a href="https://nginx.org/en/docs/http/ngx_http_v3_module.html">Module ngx_http_v3_module - nginx</a></li>

</ul>
</details>

**标签**: `#nginx`, `#security`, `#vulnerability`, `#CVE`, `#F5`

---

<a id="item-17"></a>
## [微软披露利用 USB LNK 和 Tor C2 的 Windows 剪贴板恶意软件](https://thehackernews.com/2026/06/microsoft-details-windows-clipper.html) ⭐️ 8.0/10

微软披露了一项自 2026 年 2 月以来活跃的加密货币剪贴板恶意软件行动，该行动利用 USB LNK 文件进行传播，并通过 Tor 隐藏服务进行命令与控制通信。 该行动通过窃取剪贴板数据针对加密货币用户，其使用基于 Tor 的 C2 使得检测和清除难度大增，对加密货币社区构成严重威胁。 该恶意软件利用 Windows Script Host 和 ActiveX 启动捆绑的 Tor 代理，LNK 蠕虫载荷会隐藏 USB 驱动器上的原始文档文件，并创建恶意快捷方式，诱骗用户执行恶意软件。

rss · The Hacker News · 6月18日 14:30

**背景**: 剪贴板恶意软件监控系统剪贴板中的加密货币钱包地址，并将其替换为攻击者控制的地址以窃取资金。LNK 蠕虫是一种可通过 USB 驱动器传播的恶意快捷方式文件。Tor 隐藏服务（.onion 地址）提供匿名且难以被清除的 C2 通信渠道。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/microsoft-details-windows-clipper.html">Microsoft Details Windows Clipper Malware Campaign Using USB LNK Worm ...</a></li>
<li><a href="https://www.microsoft.com/en-us/security/blog/2026/06/17/crypto-clipper-uses-tor-worm-like-propagation-for-persistence-control/">Crypto Clipper uses Tor and worm-like propagation for persistence and ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#cryptocurrency`, `#Windows`, `#Tor`

---

<a id="item-18"></a>
## [DragonForce 黑客滥用 Microsoft Teams 中继隐藏 C2 流量](https://thehackernews.com/2026/06/dragonforce-hackers-abuse-microsoft.html) ⭐️ 8.0/10

赛门铁克和 Carbon Black 的研究人员发现，DragonForce 勒索软件组织部署了一种名为 Backdoor.Turn 的自定义 Go 语言远程访问木马，该木马通过 Microsoft Teams 的 TURN 中继基础设施路由命令与控制流量以逃避检测。 这种新技术使攻击者能够将恶意流量与合法的 Microsoft 365 网络活动混合，使检测变得极其困难。这凸显了勒索软件组织滥用可信云服务隐藏 C2 流量的日益增长趋势。 Backdoor.Turn 是已知首个滥用 Microsoft Teams TURN 中继的恶意软件。该攻击针对一家美国大型服务公司，攻击者还利用了此前未知的华为驱动程序漏洞。

rss · The Hacker News · 6月18日 13:30

**背景**: Microsoft Teams 使用 TURN（围绕 NAT 的中继遍历）中继来通过中继媒体流量优化音频/视频通话。攻击者可以将命令与控制流量注入这些中继，从而混入合法的 Teams 流量中，绕过网络安全控制。赛门铁克威胁猎人团队和 Carbon Black 提供了此活动的分析。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/dragonforce-hackers-abuse-microsoft.html">DragonForce Hackers Abuse Microsoft Teams Relays to Hide ...</a></li>
<li><a href="https://threat-modeling.com/ransomware-microsoft-teams-relay-abuse-june-2026/">Ransomware Gangs Abusing Microsoft Teams Relays to Hide ...</a></li>
<li><a href="https://x.com/Cyber_O51NT/status/2066878223753875951">Backdoor.Turn, a Go-based RAT, first-known to abuse Microsoft Teams TURN relays to mask C2 traffic, while attackers also exploited a previously unknown Huawei driver vulnerability.</a></li>

</ul>
</details>

**标签**: `#ransomware`, `#Microsoft Teams`, `#C2 concealment`, `#Go malware`, `#threat intelligence`

---

<a id="item-19"></a>
## [Klue OAuth 漏洞导致 Icarus 窃取 Salesforce 数据](https://www.bleepingcomputer.com/news/security/klue-oauth-breach-linked-to-icarus-salesforce-data-theft-attacks/) ⭐️ 8.0/10

市场情报平台 Klue 遭遇 OAuth 漏洞，导致 Icarus 威胁行为者从多个组织窃取 Salesforce CRM 数据，并正在进行勒索活动。 此次事件凸显了 OAuth 令牌窃取绕过 MFA 的威胁，以及利用可信集成访问敏感 CRM 数据的风险，影响众多组织。 Icarus 组织最早于 2026 年 4 月出现，利用被盗的 OAuth 令牌访问 Salesforce 实例，并开始对受影响组织进行勒索。

rss · BleepingComputer · 6月18日 14:19

**背景**: OAuth 令牌允许应用无需密码访问用户数据。一旦被盗，攻击者可以绕过 MFA，持续访问 Salesforce 等服务。此类攻击在 2026 年越来越常见。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/klue-oauth-breach-linked-to-icarus-salesforce-data-theft-attacks/">Klue OAuth breach linked to 'Icarus' Salesforce data theft attacks - Bleeping Computer</a></li>
<li><a href="https://www.scworld.com/brief/icarus-threat-actors-exploit-klue-oauth-breach-to-steal-salesforce-data">Icarus threat actors exploit Klue OAuth breach to steal Salesforce data | brief | SC Media</a></li>
<li><a href="https://socradar.io/free-tools/ransomware-intelligence/groups/icarus">icarus - Ransomware Group | RansomwareRadar — SOCRadar Labs</a></li>

</ul>
</details>

**标签**: `#security`, `#data breach`, `#Salesforce`, `#OAuth`, `#threat actor`

---

<a id="item-20"></a>
## [警方清理近 1.5 万个与 Evil Corp 相关的 SocGholish 感染网站](https://www.bleepingcomputer.com/news/security/law-enforcement-nukes-socgholish-malware-from-nearly-15-000-sites/) ⭐️ 8.0/10

国际执法机构清理了近 1.5 万个被 SocGholish 恶意软件感染的 WordPress 网站，并摧毁了 100 多台与俄罗斯犯罪集团 Evil Corp 相关的服务器。 此次行动严重破坏了用于传播勒索软件和间谍活动的重大僵尸网络，展示了针对一个多产的俄罗斯网络犯罪集团的有效国际合作。 SocGholish 恶意软件通过伪装成虚假浏览器更新的路过式下载传播，而 Evil Corp 是一个位于俄罗斯的犯罪集团，以 WastedLocker 和 BitPaymer 等勒索软件闻名。

rss · BleepingComputer · 6月18日 13:25

**背景**: SocGholish 是一种于 2018 年首次发现的恶意软件下载器，利用被入侵的网站传播勒索软件或信息窃取程序等次级载荷。Evil Corp 是一个俄罗斯网络犯罪集团，于 2019 年被美国起诉，在全球造成超过 1 亿美元的损失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://redcanary.com/threat-detection-report/threats/socgholish/">SocGholish | Red Canary Threat Detection Report</a></li>
<li><a href="https://www.nationalcrimeagency.gov.uk/who-we-are/publications/732-evil-corp-behind-the-screens/file">October 2024 Evil Corp: Behind the Screens</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#law enforcement`, `#malware`, `#WordPress`, `#Evil Corp`

---