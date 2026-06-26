---
layout: default
title: "Horizon Summary: 2026-06-26 (ZH)"
date: 2026-06-26
lang: zh
---

> 从 70 条内容中筛选出 20 条重要资讯。

---

1. [首个完整赫库兰尼姆卷轴被 AI 读取](#item-1)
2. [德国法院裁定谷歌对 AI 摘要负责](#item-2)
3. [CISA 警告 pynetdicom 库存在严重路径遍历漏洞](#item-3)
4. [互联网的“证件时代”威胁隐私](#item-4)
5. [Zig 新的 bitCast 语义与 LLVM 后端改进](#item-5)
6. [OpenAI 研究：AI 智能体提升工作生产力](#item-6)
7. [论文揭示 LLM 角色混淆导致提示注入攻击](#item-7)
8. [NVIDIA 通过描述符堆提升 Vulkan 资源绑定效率](#item-8)
9. [混合模型更擅长预测哪些词元](#item-9)
10. [CISA 警告 Daktronics 控制器存在严重漏洞](#item-10)
11. [CISA 发布施耐德电气 PowerLogic P7 漏洞公告](#item-11)
12. [EVoke 充电站管理系统存在严重漏洞](#item-12)
13. [CISA 警告 Horner Cscape 存在高危漏洞](#item-13)
14. [拥有千万安装量的 Chrome 广告拦截器被发现存在潜伏脚本注入漏洞](#item-14)
15. [Gaslight macOS 恶意软件利用提示注入逃避 AI 分析](#item-15)
16. [CVE-2025-52465 GeoServer 任意文件写入漏洞](#item-16)
17. [CargoWise WebTracker 漏洞泄露加密密钥](#item-17)
18. [CISA 将两个正被利用的漏洞加入 KEV 目录](#item-18)
19. [CISA 警告 Delta DTM Soft 存在反序列化漏洞](#item-19)
20. [CISA 警告 OHIF DICOM 查看器存在 SSRF 漏洞](#item-20)

---

<a id="item-1"></a>
## [首个完整赫库兰尼姆卷轴被 AI 读取](https://scrollprize.org/firstscroll) ⭐️ 10.0/10

首次，利用高分辨率 X 射线断层扫描和机器学习，完整阅读了赫库兰尼姆卷轴 PHerc.1667，无需物理展开。 这一突破为历史研究开辟了新领域，证明人工智能可以从被认为无法阅读的碳化卷轴中恢复失传文本，有可能揭示数千部古代著作。 该卷轴是维苏威挑战赛的一部分，该挑战赛提供 70 万美元大奖，用于阅读完整卷轴中的段落；获胜团队使用墨水检测模型和虚拟展开技术，解码了提及 Aristocreon 的斯多葛学派论著。

hackernews · verditelabs · 6月25日 15:48 · [社区讨论](https://news.ycombinator.com/item?id=48675179)

**背景**: 赫库兰尼姆纸莎草卷轴在公元 79 年维苏威火山喷发时被碳化，变得脆弱且无法打开。传统方法无法阅读它们，但现在高分辨率 CT 扫描结合机器学习可以实现虚拟展开和墨水检测，无需物理操作即可揭示文本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://greekreporter.com/2026/06/26/herculaneum-scroll-complete-text-ai/">Herculaneum Scroll's Complete Text Deciphered Using AI After ...</a></li>
<li><a href="https://www.theregister.com/offbeat/2026/06/25/they-read-the-scroll-thing-ai-helps-decipher-ancient-document-charred-by-vesuvius/5262525">They read the scroll thing! AI helps decipher ancient ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应充满敬畏和兴奋，许多人评论这对历史发现的深远影响。维苏威挑战赛的一名团队成员主动回答问题，而其他人则反思卷轴从古代到现代人工智能的非凡旅程。一些人希望赫库兰尼姆仍有更多卷轴埋藏，等待被阅读。

**标签**: `#AI archaeology`, `#Herculaneum scrolls`, `#machine learning`, `#historical text recovery`, `#digital restoration`

---

<a id="item-2"></a>
## [德国法院裁定谷歌对 AI 摘要负责](https://www.schneier.com/blog/archives/2026/06/ai-and-liability.html) ⭐️ 9.0/10

德国法院裁定，谷歌需为其 AI 生成的搜索摘要中的错误信息承担责任，驳回了用户应自行核实 AI 内容的辩护理由。 这一里程碑式的裁决将 AI 输出视为公司商业活动的表达，可能重塑所有部署生成式 AI 企业的责任标准。 法院明确驳回了 AI 幻觉对用户显而易见的论点，并将谷歌的 AI 概览视为发布者内容而非传输者传输。

rss · Schneier on Security · 6月25日 17:03

**背景**: 历史上，互联网平台被分为传输者（不对传输内容负责）或发布者（对发布内容负责）。谷歌的 AI 概览从搜索结果中生成合成摘要，有时会出现所谓的幻觉错误。该裁决将 AI 生成的内容重新归类为发布者级别的言论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_AI_Overviews">Google AI Overviews</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI liability`, `#legal`, `#Google`, `#internet publishing`, `#AI regulation`

---

<a id="item-3"></a>
## [CISA 警告 pynetdicom 库存在严重路径遍历漏洞](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-176-01) ⭐️ 9.0/10

CISA 发布了一份公告（ICSMA-26-176-01），指出 pynetdicom 库 1.0.0 至 3.0.4 版本存在一个严重的路径遍历漏洞（CVE-2026-56445，CVSS 9.1），允许未经身份验证的攻击者写入任意文件。 该漏洞影响医疗基础设施中广泛使用的 DICOM 网络库，可能使远程攻击者破坏医学影像系统和患者数据的完整性。 漏洞位于 qrscp 应用程序的 C-STORE 处理程序中，该程序在 os.path.join() 中使用了攻击者提供的 DICOM 数据集路径而未进行清理。供应商未响应 CISA 的缓解请求，目前尚无补丁可用。

rss · CISA Cybersecurity Advisories · 6月25日 12:00

**背景**: DICOM 是医学影像数据交换的国际标准，全球医院广泛使用。pynetdicom 是一个实现 DICOM 网络协议的 Python 库，可用于创建 DICOM 客户端和服务器。路径遍历漏洞允许攻击者在预期目录之外写入文件，可能导致远程代码执行或数据损坏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/pydicom/pynetdicom">GitHub - pydicom/pynetdicom: A Python implementation of the DICOM networking protocol · GitHub</a></li>
<li><a href="https://pypi.org/project/pynetdicom/0.8.1/">pynetdicom · PyPI</a></li>
<li><a href="https://en.wikipedia.org/wiki/DICOM">DICOM - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#pydicom`, `#path-traversal`, `#CISA`

---

<a id="item-4"></a>
## [互联网的“证件时代”威胁隐私](https://expression.fire.org/p/the-papers-please-era-of-the-internet) ⭐️ 8.0/10

一篇批评性文章指出，网络上日益增多的身份验证要求，类似于“请出示证件”的制度，正在侵蚀隐私和用户自主权。文章强调了政府和平台强制要求年龄验证和上传身份证件，从而带来监控风险。 这之所以重要，是因为强制在线验证可能使大规模监控常态化，抑制自由表达，并导致敏感数据泄露。这场辩论关乎软件工程、政策以及基本数字权利。 文章既考虑了隐私风险，也考虑了潜在的技术解决方案，例如匿名凭证，它允许证明属性（如年龄）而不透露身份。文章指出，即使是极简的验证也可能被滥用于跟踪和歧视。

hackernews · bilsbie · 6月25日 21:44 · [社区讨论](https://news.ycombinator.com/item?id=48679608)

**背景**: 在线身份验证在年龄限制内容、金融服务和社交媒体中变得普遍。传统上，这需要上传政府身份证件或提供个人数据，为攻击者创建了集中式的蜜罐。隐私倡导者警告说，会出现一个“证件时代”的互联网，其中每个行为都与经过验证的真实世界身份相关联。

**社区讨论**: 评论者表达了不同的观点：一些人强调技术解决方案，如匿名凭证和零知识证明来保护隐私，而另一些人则认为公众看不到直接的危害，因此接受了这种权衡。少数人主张使用气隙系统来维持信任，但总体情绪是，这是一场关键的斗争，值得更多关注。

**标签**: `#privacy`, `#age verification`, `#digital identity`, `#internet policy`, `#surveillance`

---

<a id="item-5"></a>
## [Zig 新的 bitCast 语义与 LLVM 后端改进](https://ziglang.org/devlog/2026/#2026-06-25) ⭐️ 8.0/10

Zig 引入了新的 @bitCast 语义，这些语义与字节序无关，在所有目标上行为一致，并改进了 LLVM 后端以生成更好的代码。 这一改变消除了 bitcasting 中的字节序依赖性，使 Zig 更具可移植性并减少细微错误，同时 LLVM 后端的改进提升了生成代码的质量和性能。 新的 @bitCast 语义解释逻辑位模式而不考虑目标字节序，这意味着从 [2]u8 到 u16 的 bitcast 在所有目标上产生相同的结果，并且任意宽度整数类型现在受益于改进的 LLVM 降级策略。

hackernews · kouosi · 6月25日 14:19 · [社区讨论](https://news.ycombinator.com/item?id=48673825)

**背景**: Zig 的 @bitCast 函数将给定值的位重新解释为另一种类型。以前，其结果因目标平台的字节序（内存中字节的顺序）而异，导致可移植性问题。新的语义使 bitCast 纯粹是逻辑上的，忽略内存表示。LLVM 是 Zig 用于生成机器代码的后端；所描述的改进包括更好地降低任意位宽整数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziglang.org/devlog/2026/?2026-06-25">Devlog Zig Programming Language</a></li>
<li><a href="https://news.ycombinator.com/item?id=48673825">Zig 's New BitCast Semantics and LLVM Back End... | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区的反应非常积极，用户称赞了与字节序无关的行为和详细的解释。一些人对任意宽度整数的实用性提出疑问，但总体而言，这一改变被视为可移植性和代码清晰度的重大改进。

**标签**: `#Zig`, `#compiler`, `#systems programming`, `#semantics`, `#LLVM`

---

<a id="item-6"></a>
## [OpenAI 研究：AI 智能体提升工作生产力](https://openai.com/index/how-agents-are-transforming-work) ⭐️ 8.0/10

OpenAI 发布了一篇研究论文，展示了 AI 智能体如何执行更长、更复杂的任务，从而在多个角色中提升生产力。 这项研究标志着向能够处理复杂工作流的自主 AI 系统转变，可能革新工作效率和任务分配方式。 该论文特别指出，AI 智能体能够处理更长和更复杂的任务，表明在智能体编排和工具使用方面取得了进展。

rss · OpenAI Blog · 6月25日 02:00

**背景**: AI 智能体是能够自主使用可用工具执行任务的系统，超越了简单的语言处理，包括决策和问题解决。它们被设计用于规划和执行多步骤工作流，这与标准聊天机器人不同。OpenAI 的这项研究基于这一概念，展示了实际的生产力提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/ai-agents">What Are AI Agents ? | IBM</a></li>
<li><a href="https://lfomendes.medium.com/weekly-reading-ai-agents-8414e387bfd8">Weekly reading: AI Agents . The portuguese version of this... | Medium</a></li>

</ul>
</details>

**标签**: `#AI`, `#agents`, `#research`, `#productivity`

---

<a id="item-7"></a>
## [论文揭示 LLM 角色混淆导致提示注入攻击](https://www.schneier.com/blog/archives/2026/06/interesting-paper-exploring-prompt-injection.html) ⭐️ 8.0/10

一项新的研究论文表明，大型语言模型（LLM）之所以容易受到提示注入攻击，是因为它们学习角色块的风格模式，而不仅仅依赖角色标签，这使得当前的安全措施存在根本缺陷。 这一发现挑战了当前基于角色标签的 LLM 安全架构，并表明防御提示注入需要全新的方法，因为模型缺乏真正的角色感知能力。 该论文引入了‘角色探针’来测量 LLM 内部如何感知文本角色，并表明模型根据文本听起来的样子而非其标记的角色来混淆文本来源，从而使得大规模细微注入攻击成为可能。

rss · Schneier on Security · 6月25日 11:23

**背景**: 提示注入是一种网络安全攻击手段，恶意输入会导致 LLM 产生非预期行为。LLM 使用角色标签（如系统、用户、助手）来区分指令和用户输入。然而，这篇论文表明模型实际上学习的是每个角色块中文本的风格，而不仅仅是标签，从而导致角色混淆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://arxiv.org/abs/2603.12277">[2603.12277] Prompt Injection as Role Confusion - arXiv.org</a></li>
<li><a href="https://role-confusion.github.io/">Prompt Injection as Role Confusion</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#LLM security`, `#AI safety`, `#role confusion`

---

<a id="item-8"></a>
## [NVIDIA 通过描述符堆提升 Vulkan 资源绑定效率](https://developer.nvidia.com/blog/streamlining-resource-binding-with-end-to-end-support-for-vulkan-descriptor-heaps/) ⭐️ 8.0/10

NVIDIA 发布了一篇博客文章，详细介绍了 Vulkan 的新扩展 VK_EXT_descriptor_heap，该扩展通过端到端支持描述符堆来简化着色器中的资源绑定。 该扩展降低了 CPU 开销并简化了资源绑定过程，使 Vulkan 更接近 DirectX 12 的描述符堆模型，从而可能提升图形密集型应用的性能。 VK_EXT_descriptor_heap 扩展重构了描述符系统，允许 GPU 直接内存访问描述符，消除了传统描述符集的间接性，从而实现更高效的着色器执行。

rss · NVIDIA Developer Blog · 6月25日 22:25

**背景**: 在 Vulkan 中，着色器通过描述符访问纹理和缓冲区等资源，描述符被组织成描述符集并通过复杂的协议进行绑定。受 DirectX 12 启发的新的描述符堆扩展提供了一个扁平的、可直接访问的描述符内存模型，减少了 CPU 工作并提高了灵活性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/streamlining-resource-binding-with-end-to-end-support-for-vulkan-descriptor-heaps/">Streamlining Resource Binding with End-to-End Support for ...</a></li>
<li><a href="https://web.archive.org/web/20260123163251/https://www.khronos.org/blog/vulkan-introduces-roadmap-2026-and-new-descriptor-heap-extension">Vulkan Introduces Roadmap 2026 and New Descriptor Heap Extension</a></li>
<li><a href="https://docs.vulkan.org/guide/latest/descriptor_heap.html">Descriptor Heap :: Vulkan Documentation Project</a></li>

</ul>
</details>

**标签**: `#Vulkan`, `#GPU`, `#graphics programming`, `#descriptor heaps`, `#NVIDIA`

---

<a id="item-9"></a>
## [混合模型更擅长预测哪些词元](https://huggingface.co/blog/allenai/hybrid-token-prediction) ⭐️ 8.0/10

艾伦人工智能研究院的博客文章分析了混合语言模型在词元层面的预测优势，发现与纯 Transformer 或状态空间模型相比，混合模型在预测专有名词和长距离依赖关系等特定词元类型上表现更优。 这一发现有助于研究人员和实践者为需要精确词元预测的任务选择最优模型架构，可能在代码生成、长文本推理等应用中提高语言模型的效率和性能。 该分析可能比较了结合自注意力机制和结构化状态空间模型（如 Mamba）的混合模型与纯 Transformer 或 SSM 基线模型，使用了每词元困惑度或预测准确率等指标。

rss · Hugging Face Blog · 6月25日 16:11

**背景**: 混合语言模型将自注意力机制与结构化状态空间模型（如 Mamba）相结合，以在计算效率和建模质量之间取得平衡，特别是在长序列任务中。这些模型已展现出良好的性能，但此前缺乏对每词元性能的详细分析。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.04800">[2510.04800] Hybrid Architectures for Language Models ...</a></li>

</ul>
</details>

**标签**: `#hybrid models`, `#token prediction`, `#language models`, `#AI research`

---

<a id="item-10"></a>
## [CISA 警告 Daktronics 控制器存在严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-04) ⭐️ 8.0/10

CISA 于 2026 年 6 月 25 日发布公告（ICSA-26-176-04），警告 Daktronics 控制器固件中存在严重漏洞，未经身份验证的攻击者可获得系统的 root 级别访问权限和完全控制权。 这些漏洞影响广泛应用于商业设施、应急服务和医疗等关键基础设施领域的 Daktronics DMP 系列控制器，可能导致远程系统接管和公共安全系统中断。 公告列出了三个漏洞：路径遍历（CVE-2026-28701，CVSS 7.7/9.3）、不受限制的文件上传以及硬编码凭据，综合 CVSS v3 评分为 8.1。受影响的固件包括 VFC-DMP-5000、DMP-5000 和 DMP-8000 版本低于 8.117.x.x、9.43.x.x 或 10.34.x.x。

rss · CISA Cybersecurity Advisories · 6月25日 12:00

**背景**: Daktronics 是数字显示系统的领先制造商，其 DMP 系列控制器用于管理体育场馆、交通枢纽和紧急通知系统中的大型 LED 显示屏。这些控制器通常运行专有固件，并部署在全球各地。公告中使用的 CSAF 格式支持机器可读的漏洞信息共享。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.shield53.com/critical-firmware-flaws-in-daktronics-controllers-open-door-to-full-root-access/">Critical Firmware Flaws in Daktronics Controllers Open Door ...</a></li>
<li><a href="https://www.daktronics.com/en-us/support/kb/000003770">DMP: How do I update the controller firmware? - Daktronics</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#ICS`, `#CISA`, `#firmware`

---

<a id="item-11"></a>
## [CISA 发布施耐德电气 PowerLogic P7 漏洞公告](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-07) ⭐️ 8.0/10

美国网络安全与基础设施安全局（CISA）于 2026 年 6 月 25 日发布了一份安全公告（ICSA-26-176-07），详细说明了施耐德电气 PowerLogic P7 保护与控制平台中的多个漏洞，包括 CVE-2026-9716（空指针解引用）、操作系统命令注入和可达断言。这些漏洞可能导致未授权执行特权命令或人机界面（HMI）及配置功能丧失，从而威胁关键服务的正常运行。 PowerLogic P7 在全球范围内的能源、商业设施和关键制造等关键基础设施领域广泛部署。利用这些漏洞可能导致系统运行失控和基本服务中断，因此立即修复对于运营技术（OT）安全团队至关重要。 这些漏洞影响 PowerLogic P7 0.2.003.001.000 及之前版本，CVSS v3 基础评分为 7.5（高）。厂商修复版本为固件 V02.004.001，推荐的缓解措施包括限制对端口 8080 和 3702 的网络访问、监控 wsApp 上的异常 SOAP 请求以及遵循最小权限原则。

rss · CISA Cybersecurity Advisories · 6月25日 12:00

**背景**: 施耐德电气 PowerLogic P7 是一款专为复杂电气网络应用设计的保护与控制平台，常用于中压电力系统。CISA 的工业控制系统公告提供结构化的漏洞信息，帮助资产所有者保护工控系统。本公告采用通用安全公告框架（CSAF）格式，以实现安全信息的自动化交换。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.buildings.com/products/energy-management/product/33005674/schneider-electric-powerlogic-p7">PowerLogic P 7 | Buildings</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#ICS`, `#OT`, `#CISA`

---

<a id="item-12"></a>
## [EVoke 充电站管理系统存在严重漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-02) ⭐️ 8.0/10

CISA 发布了威胁公告 ICSA-26-176-02，指出 EVoke Systems 充电站管理系统存在多个严重漏洞（CVSS 9.4），包括关键功能缺少认证、未限制过多认证尝试、会话过期不足以及凭据保护不足。攻击者可利用这些漏洞获得未授权的管理控制权或导致服务中断。 电动汽车充电基础设施对能源和交通领域至关重要，EVoke CSMS 的全球部署使得这些漏洞风险显著。成功利用可中断充电服务或使攻击者控制充电站，影响关键基础设施安全。 所有版本的 EVoke CSMS 均受影响，漏洞包括 CVE-2026-40702（WebSocket 端点未认证）。厂商建议迁移至 OCPP 安全配置文件 2 或 3，但旧型号充电器可能无法升级。

rss · CISA Cybersecurity Advisories · 6月25日 12:00

**背景**: 充电站管理系统（CSMS）用于通过 OCPP 等协议监控和控制 EV 充电站。关键功能缺乏认证使攻击者可绕过安全检查，而未限制过多认证尝试则允许暴力破解攻击。这些是常见的 Web 应用漏洞，CWE 将其归类为 CWE-306 和 CWE-307。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cwe.mitre.org/data/definitions/307.html">CWE-307: Improper Restriction of Excessive Authentication ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#vulnerability`, `#EV charging`, `#ICS`, `#CISA`

---

<a id="item-13"></a>
## [CISA 警告 Horner Cscape 存在高危漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-03) ⭐️ 8.0/10

CISA 发布公告（ICSA-26-176-03），详细描述了 Horner Automation Cscape 版本低于 10.2 SP3 中存在的一个高危越界读取漏洞（CVE-2026-12897），该漏洞可能允许本地攻击者泄露信息并执行任意代码。 该漏洞影响全球关键制造业广泛使用的工业控制系统软件，对关键基础设施安全构成重大威胁。利用该漏洞可能导致运营中断、数据泄露或进一步入侵 ICS 网络。 该漏洞通过解析特制的 CSP 文件触发，CVSS v3.1 基本评分为 7.8（高危），向量字符串为 AV:L/AC:L/PR:N/UI:R/S:U/C:H/I:H/A:H。Horner Automation 已发布 Cscape 10.2 SP3 作为修复版本。

rss · CISA Cybersecurity Advisories · 6月25日 12:00

**背景**: Horner Automation Cscape 是一款 PLC 编程软件，结合图形化梯形图逻辑和操作员界面开发，广泛应用于全球工业控制系统。越界读取是指程序读取超出分配内存缓冲区边界的数据，可能导致敏感信息泄露或任意代码执行。该漏洞归类于 CWE-125。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hornerautomation.com/cscape-software-free/cscape-software/">Cscape Software - Horner Automation</a></li>

</ul>
</details>

**标签**: `#CISA`, `#vulnerability`, `#ICS`, `#out-of-bounds read`, `#Horner Automation`

---

<a id="item-14"></a>
## [拥有千万安装量的 Chrome 广告拦截器被发现存在潜伏脚本注入漏洞](https://thehackernews.com/2026/06/chrome-ad-blocker-with-10m-installs.html) ⭐️ 8.0/10

该漏洞使超过 1000 万用户面临潜在远程代码执行风险（如果潜伏注入路径被激活），凸显了流行浏览器扩展中固有的供应链风险。 注入能力依赖于一个名为“trusted-create-element”的自定义脚本规则，该扩展目前在 Chrome 网上应用商店拥有“精选”徽章；但目前尚未观察到活跃利用。

rss · The Hacker News · 6月25日 14:12

**背景**: Chrome 扩展可以请求广泛权限来修改网页，广告拦截器通常使用内容脚本和声明性规则。潜伏脚本注入路径意味着存在执行任意 JavaScript 的底层代码，但并未主动投递恶意负载。研究人员通过手动代码审查而非动态分析发现了这些路径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/chrome-ad-blocker-with-10m-installs.html">Chrome Ad Blocker with 10M+ Installs Found with Dormant ...</a></li>
<li><a href="https://netcrook.com/written_article?slug=dormant-script-injection-in-popular-chrome-add-on&lang=en">A Popular Chrome Add-On Was Found to Have Dormant Script ...</a></li>

</ul>
</details>

**标签**: `#security`, `#chrome extension`, `#ad blocker`, `#JavaScript injection`, `#vulnerability`

---

<a id="item-15"></a>
## [Gaslight macOS 恶意软件利用提示注入逃避 AI 分析](https://thehackernews.com/2026/06/new-gaslight-macos-malware-uses-prompt.html) ⭐️ 8.0/10

一种名为 Gaslight 的新型基于 Rust 的 macOS 恶意软件被发现，它嵌入了提示注入负载，以欺骗 AI 辅助恶意软件分析工具中止或拒绝分析。 这种新颖的规避技术针对网络安全分析中日益使用的大型语言模型（LLM），可能削弱对 AI 辅助威胁检测的信任，并突显了针对 AI 系统的新攻击向量。 Gaslight 是一个用 Rust 实现的后门和信息窃取器，最初于 2025 年 6 月初在 Apple XProtect 更新后被检测到。提示注入字符串模仿诸如“忽略所有之前的指令”之类的指令，以混淆基于 LLM 的分析工具。

rss · The Hacker News · 6月25日 09:23

**背景**: 提示注入是一种针对大型语言模型的安全漏洞，恶意输入操纵模型的行为或绕过安全过滤器。在网络安全领域，AI 工具越来越多地用于自动化恶意软件分析，而该恶意软件利用这种依赖，通过欺骗 AI 错误分类或忽略恶意代码来实施攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.checkpoint.com/2025/ai-evasion-prompt-injection/">New Malware Embeds Prompt Injection to Evade AI Detection ...</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection - OWASP Foundation</a></li>
<li><a href="https://cyberpress.org/gaslight-backdoor-misleads-analysts/">macOS.Gaslight Rust Backdoor Uses Prompt Injection to Mislead ...</a></li>

</ul>
</details>

**标签**: `#malware`, `#macOS`, `#prompt injection`, `#AI safety`, `#cybersecurity`

---

<a id="item-16"></a>
## [CVE-2025-52465 GeoServer 任意文件写入漏洞](https://www.reddit.com/r/netsec/comments/1ufdc3k/cve202552465_geoserver_arbitrary_file_write/) ⭐️ 8.0/10

已披露的新漏洞 CVE-2025-52465 允许在 GeoServer 中进行任意文件写入。该安全问题已在 Reddit 的 r/netsec 上发布。 该漏洞可能允许攻击者将文件写入服务器上的任意位置，从而可能导致远程代码执行或数据损坏。GeoServer 被广泛用于共享地理空间数据，因此这给许多组织带来了重大风险。 该任意文件写入漏洞影响基于 Java 的开源服务器 GeoServer。CVE 编号为 CVE-2025-52465，但提供的内容中未详细说明受影响的版本或补丁。

reddit · r/netsec · /u/AlbatrossMaximum4489 · 6月25日 15:30

**背景**: GeoServer 是一个用 Java 编写的开源服务器，允许用户使用开放标准共享、处理和编辑地理空间数据。任意文件写入漏洞是一种安全缺陷，攻击者可以在通常无法访问的位置创建或修改文件，这通常是由于不正确的输入清理或路径遍历造成的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GeoServer">GeoServer</a></li>
<li><a href="https://geoserver.org/">GeoServer</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CVE`, `#GeoServer`, `#file-write`

---

<a id="item-17"></a>
## [CargoWise WebTracker 漏洞泄露加密密钥](https://www.reddit.com/r/netsec/comments/1uf7h8g/cargowise_webtracker_the_keys_were_in_the_cargo/) ⭐️ 8.0/10

CargoWise WebTracker（一个物流跟踪平台）被发现存在严重安全漏洞，其加密密钥遭到泄露，攻击者可能利用此漏洞破坏系统安全。 此漏洞对依赖 CargoWise 的全球物流系统构成重大风险，泄露的密钥可能导致未经授权访问敏感货运数据并扰乱供应链运营。该披露突显了关键基础设施软件中持续存在的安全问题。 该漏洞由用户 Mempodipper 在 netsec 子论坛上公布，但完整的技术细节和概念验证尚未公开。泄露的加密密钥可用于解密通信、伪造身份或在系统中获取更高权限。

reddit · r/netsec · /u/Mempodipper · 6月25日 11:34

**背景**: CargoWise WebTracker 是 CargoWise One 平台的一个模块，为物流客户提供实时货运可见性。它允许客户跟踪货物、报关单和仓库收据。加密密钥对于保护传输中和静态数据至关重要；其泄露可能破坏平台的整个安全体系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://logixboard.com/cargowise/3pl-resources/how-do-you-set-up-cargowise-web-tracker-notifications/">How Do You Set Up CargoWise Web Tracker ... | Logixboard</a></li>
<li><a href="https://resources.sfltech.ai/webtracker-and-bpo-ecosystem/">Webtracker and BPO Ecosystem – SFL Tech</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#CargoWise`, `#websecurity`, `#cryptography`

---

<a id="item-18"></a>
## [CISA 将两个正被利用的漏洞加入 KEV 目录](https://www.cisa.gov/news-events/alerts/2026/06/25/cisa-adds-two-known-exploited-vulnerabilities-catalog) ⭐️ 7.0/10

CISA 因发现活跃利用证据，将 CVE-2026-12569（PTC Windchill 和 FlexPLM 输入验证不当漏洞）以及 CVE-2026-20230（Cisco Unified Communications Manager 服务端请求伪造漏洞）添加至其已知被利用漏洞（KEV）目录。 这些漏洞对联邦企业及各类组织构成重大风险，经常成为恶意网络行为者的攻击目标。将其加入 KEV 目录后，依据 BOD 26-04，美国联邦机构必须进行强制修复，CISA 建议所有组织优先修补。 CVE-2026-12569 影响 PTC Windchill 和 FlexPLM，可能导致远程代码执行；CVE-2026-20230 是 Cisco Unified Communications Manager 中的 SSRF 漏洞，可导致服务端攻击。两个漏洞均有 CVE 标识符和明确的缓解指南。

rss · CISA Cybersecurity Advisories · 6月25日 12:00

**背景**: CISA 的已知被利用漏洞（KEV）目录是已确认被威胁行为者积极利用的漏洞列表。根据具有约束力的操作指令（BOD）26-04，联邦机构必须在公开暴露且利用后可完全控制的资产上优先修复 KEV 中的漏洞。PTC Windchill 是广泛用于制造业的产品生命周期管理（PLM）软件，而 Cisco Unified Communications Manager 是一款呼叫控制与统一通信平台。

**标签**: `#cybersecurity`, `#vulnerabilities`, `#CISA`, `#CVE`, `#SSRF`

---

<a id="item-19"></a>
## [CISA 警告 Delta DTM Soft 存在反序列化漏洞](https://www.cisa.gov/news-events/ics-advisories/icsa-26-176-06) ⭐️ 7.0/10

CISA 发布了关于 CVE-2026-12578 的公告（ICSA-26-176-06），该漏洞是 Delta Electronics DTM Soft 中的反序列化漏洞，CVSS v3.1 评分为 7.8，可导致任意代码执行。 该漏洞影响全球的关键制造业基础设施，成功利用可能允许攻击者执行任意代码，从而可能破坏工业运营。 所有版本的 DTM Soft 均受影响；Delta Electronics 正在修复，目前建议采取缓解措施，如不打开未经请求的项目文件、避免以管理员身份运行软件。

rss · CISA Cybersecurity Advisories · 6月25日 12:00

**背景**: 反序列化不受信任的数据是指应用程序在反序列化数据时未进行适当验证，可能允许攻击者注入恶意对象。Delta Electronics DTM Soft 是一款用于配置和管理 Delta DT 系列温度控制器的软件工具，广泛应用于工业自动化领域。该漏洞尤其令人担忧，因为它影响了关键制造业中广泛部署的产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://owasp.org/www-community/vulnerabilities/Deserialization_of_untrusted_data">Deserialization of untrusted data | OWASP Foundation</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#ICS`, `#critical manufacturing`, `#CISA`

---

<a id="item-20"></a>
## [CISA 警告 OHIF DICOM 查看器存在 SSRF 漏洞](https://www.cisa.gov/news-events/ics-medical-advisories/icsma-26-176-02) ⭐️ 7.0/10

2026 年 6 月 25 日，CISA 发布公告（ICSMA-26-176-02），警告 OHIF DICOM Web Viewer 框架 3.12.0 及更早版本中存在 SSRF 漏洞（CVE-2026-12473，CVSS 8.2），攻击者可通过精心构造的链接窃取临床医生的身份验证令牌。 该漏洞对全球医疗基础设施构成严重风险，因为 OHIF 是广泛使用的开源医学影像平台。被利用可能导致未经授权访问敏感患者数据并危及临床医生会话。 该 SSRF 漏洞影响默认配置中的两个数据源（DICOMWebProxy 和 DICOMJSON），它们会在没有验证的情况下获取任意 URL，导致 OIDC 承载令牌发送到攻击者控制的服务器。DICOMweb 数据源不受影响，修复版本 3.12.2 已发布，需要为经过身份验证的环境配置白名单。

rss · CISA Cybersecurity Advisories · 6月25日 12:00

**背景**: 服务器端请求伪造（SSRF）是一种漏洞，允许攻击者使服务器端应用程序向意外位置（通常是内部服务）发送请求。OHIF（开放健康影像基金会）查看器是一个全球使用的基于 Web 的开源医学影像平台，用于查看 DICOM 图像。该公告强调了医疗领域的风险：攻击者可能利用 SSRF 窃取身份验证令牌并访问患者数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://portswigger.net/web-security/ssrf">What is SSRF (Server-side request forgery)? Tutorial ... Server Side Request Forgery (SSRF) in Depth - GeeksforGeeks Server Side Request Forgery (SSRF) - Security | MDN Server-Side Request Forgery Prevention Cheat Sheet - OWASP Home | AntiSSRF Documentation SSRF Detection and Remediation: Finding Server-Side Request…</a></li>
<li><a href="https://viewer.ohif.org/">OHIF Viewer</a></li>

</ul>
</details>

**标签**: `#security`, `#medical-imaging`, `#DICOM`, `#CISA`, `#vulnerability`

---