---
layout: default
title: "Horizon Summary: 2026-06-23 (ZH)"
date: 2026-06-23
lang: zh
---

> 从 63 条内容中筛选出 20 条重要资讯。

---

1. [Steam Machine 发布，采用公平预约系统](#item-1)
2. [Trail of Bits 与 OpenAI 推出 Patch the Planet](#item-2)
3. [Moebius: 0.2B 参数图像修补模型媲美 10B 模型](#item-3)
4. [加拿大计划到 2040 年建造多达 10 座核反应堆](#item-4)
5. [Mitchell Hashimoto 再向 Zig 基金会捐款 40 万美元](#item-5)
6. [雪佛龙与微软签署 20 年德州数据中心供电协议](#item-6)
7. [Deno Desktop 支持使用多种后端开发桌面应用](#item-7)
8. [Claude Code 的扩展思考输出是有损摘要](#item-8)
9. [Mythos 后的红队演练：AI 安全与网络安全之辩](#item-9)
10. [NVIDIA 推出 CCCL 运行时，用于 CUDA 的现代 C++运行时](#item-10)
11. [ShapedPlugin Pro 插件遭供应链攻击植入后门](#item-11)
12. [DifyTap 漏洞可跨租户暴露 AI 对话](#item-12)
13. [29 年历史的 Squid 代理漏洞'Squidbleed'泄露 HTTP 请求](#item-13)
14. [新恶意软件加载器 OXLOADER 通过谷歌广告传播 CastleStealer](#item-14)
15. [加拿大间谍机构首次使用威胁减少令清除僵尸网络](#item-15)
16. [FFmpeg 修复影响 Jellyfin 等应用的 PixelSmash 漏洞](#item-16)
17. [FortiBleed 活动使用定制嗅探器窃取 FortiGate 凭据](#item-17)
18. [全局命名空间风险：通用存储桶劫持技术曝光](#item-18)
19. [Unsloth GLM-5.2 本地运行指南](#item-19)
20. [Gartner 演讲警告：遗留基础设施可劫持 AI 代理](#item-20)

---

<a id="item-1"></a>
## [Steam Machine 发布，采用公平预约系统](https://store.steampowered.com/news/group/45479024/view/685257114654870245) ⭐️ 9.0/10

Valve 发布了 Steam Machine，这是一款功能强大的类主机游戏 PC，采用公平预约系统，在数天内接受预约登记以防止机器人抢购。该设备强调开放性，允许用户安装自己的应用和操作系统。 此次发布标志着 Valve 正式进军客厅游戏硬件市场，提供兼具主机体验与 PC 灵活性的产品。公平预约系统优先考虑真实用户而非黄牛和机器人，为硬件发布树立了良好榜样。 Steam Machine 的性能是 Steam Deck 的六倍以上，能够运行整个 Steam 库，包括 AAA 大作。它配备可更换前面板，运行 SteamOS，但用户也可以自由安装其他操作系统。

hackernews · theschwa · 6月22日 17:09 · [社区讨论](https://news.ycombinator.com/item?id=48632884)

**背景**: Steam Machine 是 Valve 继 Steam Deck 掌机之后推出的全新游戏硬件系列，旨在在客厅提供类主机体验，同时保留 PC 的开放性。预约系统通过在多天内接受登记而非单一发布时间来确保公平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://store.steampowered.com/hardware/steammachine">Steam Machine</a></li>
<li><a href="https://www.lttlabs.com/articles/2026/06/22/the-newell-nucleus-steam-machine-ltt-companion-article">The Newell Nucleus : Steam Machine LTT Companion Article | LTT Labs</a></li>

</ul>
</details>

**社区讨论**: 社区对公平预约系统和设备的开放性反应积极，用户赞赏对 Linux 游戏和软件自由安装的重视。一些评论提到营销内容很接地气，并表示愿意购买以支持开放平台。

**标签**: `#steam-machine`, `#valve`, `#gaming-hardware`, `#pc-gaming`

---

<a id="item-2"></a>
## [Trail of Bits 与 OpenAI 推出 Patch the Planet](https://blog.trailofbits.com/2026/06/22/introducing-patch-the-planet/) ⭐️ 9.0/10

Trail of Bits 和 OpenAI 推出了 Patch the Planet 计划，该计划结合 GPT-5.5-Cyber 与人类专家对开源项目进行安全审计，第一周就在 19 个项目中提交了 64 个拉取请求和 51 个问题。 这一举措展示了在人类监督下利用 AI 进行漏洞发现的可扩展模式，可能彻底改变开源安全维护方式，并减轻项目维护者的负担。 第一周涵盖了 cURL、NATS、Sigstore 和 RustCrypto 等项目，已有 37 个拉取请求被合并；除了修复漏洞，贡献还包括添加模糊测试工具、CI 安全扫描和供应链改进。

rss · Trail of Bits Blog · 6月22日 16:50

**背景**: GPT-5.5-Cyber 是 OpenAI 于 2026 年 5 月通过“可信网络访问”计划发布的网络安全专用 AI 模型。Trail of Bits 是一家安全工程公司。Patch the Planet 是 OpenAI“破晓”计划的一部分，旨在保护关键开源基础设施的安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-5-with-trusted-access-for-cyber/">Scaling Trusted Access for Cyber with GPT-5.5 and ... - OpenAI</a></li>
<li><a href="https://trailofbits.com/patch-the-planet/">Patch the Planet · Trail of Bits</a></li>
<li><a href="https://openai.com/index/patch-the-planet/">Patch the Planet : a Daybreak initiative to support open... | OpenAI</a></li>

</ul>
</details>

**标签**: `#AI security`, `#open-source`, `#vulnerability discovery`, `#Trail of Bits`, `#GPT-5.5`

---

<a id="item-3"></a>
## [Moebius: 0.2B 参数图像修补模型媲美 10B 模型](https://hustvl.github.io/Moebius/) ⭐️ 8.0/10

华中科技大学和 VL 的研究人员发布了 Moebius，这是一个 0.2 亿参数的图像修补模型，声称性能可与 100 亿参数模型媲美，并且导出了 ONNX 格式，支持在浏览器中运行推理。 该模型大幅降低了高质量图像修补的计算成本，使得在消费级硬件上运行成为可能，并加速了在照片编辑和物体移除等实际应用中的部署。 该模型输出 512×512 图像，社区成员 simonw 将其导出为 ONNX 格式，制作了浏览器演示（下载约 1.3GB）。但评测者指出，修补区域明显比周围更平滑，且模型在处理新物体时表现不佳。

hackernews · DSemba · 6月22日 13:53 · [社区讨论](https://news.ycombinator.com/item?id=48630171)

**背景**: 图像修补是指用合理的内容填充图像中缺失或被移除的区域。大多数现有顶尖模型拥有数十亿参数，资源消耗大。ONNX（开放神经网络交换格式）是一种开放标准，允许模型跨不同框架和设备导出和运行，包括通过 ONNX Runtime 在浏览器中运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/hustvl/Moebius">GitHub - hustvl/Moebius: [ECCV 2026] Moebius: 0.2B ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：simonw 成功创建了交互式浏览器演示，而 lifthrasiir 则批评指出，虽然对于 0.2B 模型来说令人印象深刻，但质量无法与 10B 模型匹敌，且仅限于 512×512 分辨率。一些用户表示希望对漫画或动漫修补有专门的版本。

**标签**: `#AI`, `#image inpainting`, `#model efficiency`, `#machine learning`, `#ONNX`

---

<a id="item-4"></a>
## [加拿大计划到 2040 年建造多达 10 座核反应堆](https://www.cbc.ca/news/politics/federal-nuclear-strategy-9.7244509) ⭐️ 8.0/10

加拿大政府宣布了一项“核复兴”战略，计划到 2040 年建造多达 10 座新核反应堆，利用其丰富的铀储量及 CANDU 反应堆技术专长。 该计划可大幅提升加拿大的清洁能源产能，为太阳能和风能等间歇性可再生能源提供稳定的基础负荷电力，并支持工业部门和人工智能数据中心日益增长的能源需求。 该战略包括大型 CANDU 反应堆和小型模块化反应堆（SMR），达林顿新核电项目已在进行中。加拿大现有 17 座运行中的 CANDU 反应堆，另有其他反应堆出口至全球。

hackernews · geox · 6月22日 19:06 · [社区讨论](https://news.ycombinator.com/item?id=48634585)

**背景**: CANDU（加拿大氘铀）反应堆是一种加拿大设计的加压重水反应堆，使用天然铀燃料和重水作为慢化剂。该设计于 20 世纪 50 至 60 年代开发，已在加拿大建造并出口至韩国、罗马尼亚和中国等国家。加拿大是全球最大的铀生产国之一，为核能扩张提供了战略优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CANDU_reactor">CANDU reactor</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍表示支持，强调加拿大的铀储量、CANDU 的成熟安全性以及对基础负荷电力的需求。一些人看到了向美国供应能源以及使油砂等工业运营脱碳的潜力。

**标签**: `#nuclear energy`, `#Canada`, `#energy policy`, `#clean energy`, `#infrastructure`

---

<a id="item-5"></a>
## [Mitchell Hashimoto 再向 Zig 基金会捐款 40 万美元](https://mitchellh.com/writing/zig-donation-2026) ⭐️ 8.0/10

Ghostty 终端模拟器的创造者 Mitchell Hashimoto 宣布向 Zig 软件基金会再捐款 40 万美元，此前他已在 2024 年捐出 40 万美元。 这一大额捐赠凸显了人们对 Zig 这一有前景的系统编程语言日益增长的支持，并将资助其持续开发和社区项目。 这笔捐款是 Mitchell 2026 年捐赠承诺的一部分，他强调捐款无附加条件，基金会可根据需要自由分配资金。

hackernews · tosh · 6月22日 13:43 · [社区讨论](https://news.ycombinator.com/item?id=48630020)

**背景**: Zig 是一种现代系统编程语言，专注于性能、安全性和简洁性。Zig 软件基金会是一个非营利组织，支持该语言的发展。Mitchell Hashimoto 因创建用 Zig 编写的快速终端模拟器 Ghostty 而闻名，并且一直是 Zig 生态系统的主要财务支持者。

**社区讨论**: 社区表达了感谢，并讨论了 Ghostty 的价值，有评论指出它带来的实用价值超过了多起收购。同时也有关于 Zig 对 LLM 贡献立场的讨论，一位评论者认为构建语言需要谨慎考虑而非代码数量。

**标签**: `#Zig`, `#open-source funding`, `#systems programming`, `#community support`

---

<a id="item-6"></a>
## [雪佛龙与微软签署 20 年德州数据中心供电协议](https://www.chevron.com/newsroom/2026/q2/chevron-signs-20-year-power-agreement-with-microsoft-for-west-texas-data-center) ⭐️ 8.0/10

雪佛龙与微软签署了一项为期 20 年的电力购买协议，主要为位于德克萨斯州西部的一个新建数据中心供电，电力将主要来自 GE Vernova 和 Solar Turbines 燃气轮机燃烧天然气产生。 该协议凸显了大型科技公司雄心勃勃的碳减排承诺与支持 AI 和云计算不断增长能源需求所需的可靠可调度电力之间的紧张关系。它可能为其他超大规模企业在天然气丰富地区如何平衡可持续发展目标与电网现实树立先例。 该协议依赖大型 GE Vernova 燃气轮机以及 Caterpillar 子公司 Solar Turbines 提供的额外容量。值得注意的是，德克萨斯州西部 Waha 枢纽的天然气价格一直为负值，意味着生产商需要付费让人把气运走，这使得该协议对雪佛龙在经济上具有吸引力。

hackernews · cdrnsf · 6月22日 13:43 · [社区讨论](https://news.ycombinator.com/item?id=48630029)

**背景**: 数据中心需要 7x24 小时不间断地消耗大量电力，要求恒定可靠的电源。天然气是燃烧时排放二氧化碳的化石燃料，而太阳能和风能等可再生能源如果没有储能则具有间歇性。微软公开承诺到 2030 年实现碳负排放，使得这项依赖天然气的协议备受争议。德克萨斯州西部的二叠纪盆地因石油开采产生大量伴生气，由于管道容量不足，这些天然气通常被燃烧或低价出售。

**社区讨论**: 评论者对微软的碳目标与这项化石燃料投资的兼容性表示怀疑，指出太阳能和电池储能在德克萨斯州具有成本效益。其他人则注意到德克萨斯州西部负气价的经济逻辑，一位评论者还指出了使用名为'Solar Turbines'（实际生产燃气轮机）的公司涡轮机的讽刺之处。

**标签**: `#energy`, `#data centers`, `#microsoft`, `#chevron`, `#natural gas`

---

<a id="item-7"></a>
## [Deno Desktop 支持使用多种后端开发桌面应用](https://docs.deno.com/runtime/desktop/) ⭐️ 8.0/10

Deno Desktop 已发布，允许开发者使用 Deno 构建桌面应用，后端选项包括 Chromium Embedded Framework (CEF)、Webview 和原始渲染。计划推出共享运行时，将每个应用的二进制大小降至仅几兆字节。 这扩展了 Deno 的能力，从服务器端和 CLI 应用进入桌面开发领域，使其成为一个更通用的平台。它解决了 Electron 应用中常见的二进制体积臃肿问题，提供了更轻量的替代方案，并保留了 Deno 现有的安全特性。 编译后的二进制文件在编译时固化授予的权限，引发了关于用户透明度的疑问。共享 CEF 运行时旨在避免每个应用捆绑完整的 Chromium，但应用之间的版本冲突仍然是一个挑战。

hackernews · GeneralMaximus · 6月22日 05:38 · [社区讨论](https://news.ycombinator.com/item?id=48626137)

**背景**: Chromium Embedded Framework (CEF) 允许将完整的 Chromium 浏览器嵌入到应用中，而 Webview 提供轻量级的原生网页视图。Deno 是一个构建于 V8 之上的现代 JavaScript 和 TypeScript 运行时，注重安全和 Web 标准。桌面框架常常面临体积与兼容性之间的权衡——Electron 为每个应用捆绑 Chromium，导致二进制文件庞大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chromium_Embedded_Framework">Chromium Embedded Framework - Wikipedia</a></li>
<li><a href="https://github.com/topics/webview">webview · GitHub Topics · GitHub</a></li>
<li><a href="https://deno.com/">Deno , the next-generation JavaScript runtime</a></li>

</ul>
</details>

**社区讨论**: 社区总体上反应热烈，许多人称赞 Deno 的持续创新能力以及该功能的价值。但技术上存在担忧，包括不同应用间的 CEF 版本管理问题，以及如何将编译时权限告知最终用户。有人建议增加“在浏览器中启动”的后端，以完全避免打包浏览器引擎。

**标签**: `#deno`, `#desktop-development`, `#CEF`, `#webview`, `#runtime`

---

<a id="item-8"></a>
## [Claude Code 的扩展思考输出是有损摘要](https://patrickmccanna.net/the-text-in-claude-codes-extended-thinking-output-is-not-authentic/) ⭐️ 8.0/10

一篇文章批评 Claude Code 的“扩展思考”输出是模型推理的有损摘要，而非真实的思维链，引发了透明度和安全方面的担忧。 这很重要，因为隐藏推理削弱了 AI 透明度，并带来了潜在的安全风险，例如在隐藏阶段进行提示注入，影响用户信任和模型问责。 文章指出，摘要存在类似于将 JPEG 转换为 BMP 再转回的数据丢失问题，并且模型可在隐藏推理期间调用函数，从而增加攻击面。

hackernews · 0o_MrPatrick_o0 · 6月22日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=48630535)

**背景**: Claude 模型的扩展思考允许对复杂任务进行更深入的推理，但展示给用户的输出是压缩后的摘要，而非原始思维链。许多 AI 公司隐藏推理输出以保护专有技术，这在 AI 社区引发了透明度和安全性的讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/extended-thinking">Building with extended thinking - Claude API Docs</a></li>
<li><a href="https://claude-world.com/articles/extended-thinking-guide/">Extended Thinking in Claude Code: Unlock Deeper Reasoning</a></li>
<li><a href="https://cobusgreyling.medium.com/taking-ai-transparency-to-a-new-level-with-model-reasoning-traces-80c186453ea1">Taking AI Transparency To a New Level With Model Reasoning Traces | by Cobus Greyling | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者对隐藏推理表达了强烈担忧，一些人拒绝使用隐藏推理的模型，理由是存在提示注入和秘密目标的风险。另一些人认为公司隐藏推理是为了保护研发投入，并指出该问题在美国 AI 模型中普遍存在。

**标签**: `#AI transparency`, `#large language models`, `#Claude`, `#reasoning`, `#security`

---

<a id="item-9"></a>
## [Mythos 后的红队演练：AI 安全与网络安全之辩](https://www.latent.space/p/gray-swan) ⭐️ 8.0/10

OpenAI 董事会成员 Zico Kolter 与 Gray Swan CEO Matt Fredrikson 在播客节目《Mythos 后的红队演练》中讨论了为何 AI 安全与传统的网络安全有本质区别。 此次对话挑战了将 AI 安全视为“加入 AI 的网络安全”的常见框架，强调了间接提示注入等新型漏洞类别，以及专用 AI 安全工具的必要性。 Matt Fredrikson 透露，Gray Swan 的自动化红队工具 Shade 在性能上已超越人类红队成员，并介绍了用于保护 AI 代理的护栏模型 Cygnal。

rss · Latent Space · 6月22日 21:06

**背景**: AI 红队演练是一种模拟攻击 AI 模型以发现漏洞（如越狱和提示注入）的方法。提到的“Mythos”挑战是评估红队能力的基准。Gray Swan 是一家由卡内基梅隆大学研究人员创立的 AI 安全初创公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://daily.dev/posts/red-teaming-after-mythos-zico-kolter-matt-fredrikson-gray-swan-qnxwwrmeg">Red-Teaming after Mythos — Zico Kolter & Matt Fredrikson ...</a></li>
<li><a href="https://www.grayswan.ai/news">Research announcements and press releases for Gray Swan .</a></li>

</ul>
</details>

**标签**: `#AI security`, `#red-teaming`, `#AI safety`, `#cybersecurity`

---

<a id="item-10"></a>
## [NVIDIA 推出 CCCL 运行时，用于 CUDA 的现代 C++运行时](https://developer.nvidia.com/blog/cccl-runtime-a-modern-c-runtime-for-cuda/) ⭐️ 8.0/10

NVIDIA 宣布推出 CCCL 运行时，这是 CUDA 的现代 C++运行时，作为 CCCL 3.2 版本的一部分，为核心 CUDA 运行时和驱动程序功能提供了符合习惯的 C++接口。 这通过提供现代 C++抽象、减少样板代码并使 CUDA 开发与当代 C++实践保持一致，提高了开发者的生产力，使 GPU 编程更加便捷高效。 CCCL 运行时是开源 CUDA 核心计算库（CCCL）的一部分，可在 GitHub 上获取，并与 Thrust 和 CUB 等现有 CCCL 库集成，提供统一的开发体验。

rss · NVIDIA Developer Blog · 6月22日 16:00

**背景**: CCCL（CUDA 核心计算库）是一个包含 Thrust、CUB 和 libcu++等基础 CUDA C++库的统一仓库，提供 GPU 加速算法和并行原语。新的运行时组件引入了更高级的 C++ API，用于设备管理、内存分配和内核启动，简化了常见的 CUDA 编程任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/NVIDIA/cccl">GitHub - NVIDIA/cccl: CUDA Core Compute Libraries · GitHub</a></li>
<li><a href="https://github.com/NVIDIA/cccl/releases">Releases · NVIDIA/cccl</a></li>

</ul>
</details>

**标签**: `#CUDA`, `#C++`, `#GPU computing`, `#NVIDIA`, `#runtime`

---

<a id="item-11"></a>
## [ShapedPlugin Pro 插件遭供应链攻击植入后门](https://thehackernews.com/2026/06/shapedplugin-wordpress-pro-plugins.html) ⭐️ 8.0/10

未知威胁攻击者攻陷了 ShapedPlugin 的构建和发布管道，在通过官方许可更新渠道分发的 Pro 插件版本中注入了后门代码。Wordfence 在一份分析报告中披露了此事。 由于 ShapedPlugin 提供广泛使用的 WordPress 插件，此次供应链攻击可能影响数千个网站，使攻击者能够获得未授权访问，并可能注入更多恶意代码。这凸显了即使使用官方分发渠道，软件供应链仍然存在脆弱性。 此次攻击专门针对 Pro 插件版本，意味着通过官方渠道接收更新的付费用户面临风险。Wordfence 的分析表明，后门是在构建和分发过程中注入的，而非插件本身存在漏洞。

rss · The Hacker News · 6月22日 18:00

**背景**: 供应链攻击涉及侵入软件供应商的开发或分发基础设施，将恶意代码注入合法的软件更新中。WordPress 插件用于扩展网站功能，而像 ShapedPlugin 这样的高级插件通常安装在关键业务网站上。此类攻击可能产生广泛影响，因为所有使用被入侵产品的用户都可能成为潜在受害者。

**标签**: `#supply chain attack`, `#WordPress`, `#security`, `#plugins`, `#backdoor`

---

<a id="item-12"></a>
## [DifyTap 漏洞可跨租户暴露 AI 对话](https://thehackernews.com/2026/06/researchers-detail-difytap-flaws-in.html) ⭐️ 8.0/10

研究人员披露了 Dify 中的四个漏洞，统称为 DifyTap，可让未认证的攻击者读取其他租户应用程序的 AI 对话。 Dify 是一个广泛使用的开源 AI 平台，拥有超过 14.6 万个 GitHub 星标；这些漏洞打破了多租户隔离，可能跨组织和云部署暴露敏感的 AI 对话。 这四个漏洞无需认证即可利用，Zafran Security 已公开技术细节。DifyTap 无需任何前置访问权限即可跨租户窃听 AI 对话。

rss · The Hacker News · 6月22日 16:13

**背景**: Dify 是一个用于构建 LLM 应用的开源平台，包含可视化工作流、RAG 管道和代理功能。多租户环境本应隔离客户数据，但 DifyTap 打破了这种隔离，允许攻击者跨不同工作空间访问私密的 AI 聊天记录和文档。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/researchers-detail-difytap-flaws-in.html">Researchers Detail DifyTap Flaws in Dify That Could Expose AI ...</a></li>
<li><a href="https://news.shield53.com/difytap-four-vulnerabilities-in-popular-ai-workflow-platform-expose-cross-tenant-conversations/">DifyTap: Four Vulnerabilities in Popular AI Workflow Platform ...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerabilities`, `#AI`, `#open-source`, `#Dify`

---

<a id="item-13"></a>
## [29 年历史的 Squid 代理漏洞'Squidbleed'泄露 HTTP 请求](https://thehackernews.com/2026/06/29-year-old-squid-proxy-bug-squidbleed.html) ⭐️ 8.0/10

在 Squid 网络代理中发现了一个名为 Squidbleed 的堆过度读取漏洞，该漏洞源于 1997 年的 FTP 解析更改，允许攻击者泄露包含凭证和会话令牌的明文 HTTP 请求。 该漏洞影响广泛使用的代理服务器的默认配置，可能泄露共享该代理的用户敏感数据，且 29 年来未被发现，突显了长期开源项目的风险。 该漏洞是 Squid 网络代理默认配置中的堆过度读取错误，由 Calif.io 研究人员追溯到 1997 年的 FTP 解析更改，他们在 6 月披露并将其命名为 Squidbleed。

rss · The Hacker News · 6月22日 14:29

**背景**: 堆过度读取发生在程序从堆分配缓冲区读取超出预期的数据时，可能泄漏相邻的内存内容。Squid 是一个广泛使用的开源缓存代理服务器，支持 HTTP、HTTPS、FTP 等协议，常用于提升网络环境性能和安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Buffer_over-read">Buffer over-read - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Squid_proxy_server">Squid proxy server</a></li>
<li><a href="https://www.squid-cache.org/">squid : Optimising Web Delivery</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#squid`, `#proxy`, `#http`

---

<a id="item-14"></a>
## [新恶意软件加载器 OXLOADER 通过谷歌广告传播 CastleStealer](https://thehackernews.com/2026/06/new-oxloader-loader-uses-malicious.html) ⭐️ 8.0/10

Elastic Security Labs 的研究人员发现了一种名为 OXLOADER 的新型恶意软件加载器，该加载器通过恶意谷歌广告进行分发，最终投放 CastleStealer 信息窃取恶意软件。 该活动突显了恶意广告的持续威胁，以及利用 Node.js 等流行软件的虚假广告来诱骗用户，可能使许多系统感染能够窃取敏感数据的信息窃取器。 OXLOADER 利用.reloc 节滥用和多种抗分析技术（反虚拟机、语言检查、MBA 混淆）来逃避检测。CastleStealer 是一款基于.NET 的信息窃取器，能够窃取浏览器凭据、加密货币钱包和其他数据。

rss · The Hacker News · 6月22日 13:20

**背景**: 恶意软件加载器是设计用于隐蔽投放次级恶意软件的初始阶段载荷。像 CastleStealer 这样的信息窃取器从受感染机器收集敏感数据。恶意谷歌广告已成为分发此类恶意软件的常见载体，威胁行为者付费投放模仿合法软件的广告。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/new-oxloader-loader-uses-malicious.html">New OXLOADER Loader Uses Malicious Google Ads to Deliver CastleStealer</a></li>
<li><a href="https://www.elastic.co/security-labs/oxloader-malware-loader-infostealer">OXLOADER: new loader evading detection to drop infostealer — Elastic Security Labs</a></li>
<li><a href="https://blog.gridinsoft.com/oxloader-castlestealer-fake-nodejs-ads/">OXLOADER Malware : Fake Node.js Ads and CastleStealer Risk</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#malware`, `#Google Ads`, `#threat intelligence`

---

<a id="item-15"></a>
## [加拿大间谍机构首次使用威胁减少令清除僵尸网络](https://thehackernews.com/2026/06/canadas-spy-agency-used-first-of-its.html) ⭐️ 8.0/10

加拿大安全情报局（CSIS）于 2024 年 5 月获得联邦法院授权（2024 年 8 月续期），远程清除两个感染加拿大境内设备的外国运营僵尸网络。该裁决的公开版本于 2026 年 6 月 15 日发布，标志着 CSIS 首次将威胁减少令权力用于网络行动。 这为情报机构主动破坏网络威胁确立了重要的法律先例，可能扩大政府对私人网络的干预范围。同时也引发了关于隐私、公民自由以及安全与个人权利平衡的重要问题。 该授权允许 CSIS 在未经用户同意的情况下修改受感染服务器、家庭路由器和物联网设备上的数据。这些僵尸网络由境外运营，行动仅针对加拿大境内的设备。

rss · The Hacker News · 6月22日 09:11

**背景**: 僵尸网络是由攻击者控制的被感染设备组成的网络，用于进行 DDoS 攻击或数据窃取等恶意活动。CSIS 是加拿大主要的民用情报机构，负责国家安全。威胁减少令是允许 CSIS 破坏特定威胁的法律工具，但这是此类权力首次应用于网络安全领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aviatrix.ai/threat-research-center/canadas-spy-agency-botnet-warrant-2024/">CSIS Obtains Warrant to Neutralize Botnet-Infected Devices in ...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#botnet`, `#warrant`, `#Canada`, `#legal precedent`

---

<a id="item-16"></a>
## [FFmpeg 修复影响 Jellyfin 等应用的 PixelSmash 漏洞](https://www.bleepingcomputer.com/news/security/ffmpeg-fixes-pixelsmash-flaw-in-widely-used-video-decoder/) ⭐️ 8.0/10

FFmpeg 发布了一个名为 'PixelSmash' 的漏洞补丁，该漏洞可能允许在 Jellyfin 服务器上远程执行代码，并导致 Kodi、Emby、Nextcloud、PhotoPrism 和 OBS Studio 等应用出现拒绝服务。 此漏洞影响重大，因为 FFmpeg 是一个广泛使用的多媒体库；在 Jellyfin 服务器上远程执行代码的可能性构成了严重的安全风险，而拒绝服务攻击可能中断许多流行的媒体应用。 PixelSmash 漏洞具体位于 FFmpeg 的视频解码器中；成功利用需要特定条件，但这突显了在关键基础设施组件中及时打补丁的重要性。

rss · BleepingComputer · 6月22日 21:05

**背景**: FFmpeg 是一个免费开源的多媒体框架，被无数应用用于录制、转换和流式传输音频和视频。Jellyfin 是一个依赖 FFmpeg 进行转码的媒体服务器。PixelSmash 是指新披露的一个安全漏洞，可通过恶意构造的视频文件触发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://makerstack.co/reviews/photoprism-review/">PhotoPrism Review (2026) - MakerStack</a></li>

</ul>
</details>

**标签**: `#security`, `#ffmpeg`, `#vulnerability`, `#remote-code-execution`, `#denial-of-service`

---

<a id="item-17"></a>
## [FortiBleed 活动使用定制嗅探器窃取 FortiGate 凭据](https://www.bleepingcomputer.com/news/security/fortibleed-campaign-used-custom-fortigate-sniffer-to-steal-credentials/) ⭐️ 8.0/10

一项名为 FortiBleed 的大规模活动正在使用定制的嗅探器从被攻破的 Fortinet FortiGate 防火墙中收集身份验证秘密并窃取凭据，SOCRadar 报告称。 该活动对依赖 FortiGate 防火墙的组织构成重大威胁，因为凭据窃取可能导致进一步的网络入侵和数据泄露。使用定制嗅探器表明威胁行为者技术高超。 FortiBleed 活动针对暴露在互联网上的 FortiGate 防火墙和 SSL VPN 网关，使用多阶段攻击循环不断攻陷新设备。定制嗅探器旨在从网络流量中解析并窃取凭据。

rss · BleepingComputer · 6月22日 20:01

**背景**: FortiGate 防火墙是企业广泛使用的网络安全设备。2024 年，Fortinet 修补了 FortiOS 中的一个关键漏洞 (CVE-2024-21762)，攻击者可能利用该漏洞获得初始访问权限。FortiBleed 活动似乎利用了此类漏洞来部署嗅探器并窃取凭据，然后这些凭据可用于攻击其他设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/fortibleed-campaign-used-custom-fortigate-sniffer-to-steal-credentials/">FortiBleed campaign used custom FortiGate sniffer to steal credentials</a></li>
<li><a href="https://arcticwolf.com/resources/blog/active-fortibleed-campaign-impacting-fortinet-devices-across-194-countries/">Active FortiBleed Campaign Impacting Fortinet Devices... | Arctic Wolf</a></li>
<li><a href="https://socradar.io/blog/what-is-fortibleed/">FortiBleed : Everything You Need to Know</a></li>

</ul>
</details>

**标签**: `#security`, `#Fortinet`, `#credentials`, `#malware`, `#network security`

---

<a id="item-18"></a>
## [全局命名空间风险：通用存储桶劫持技术曝光](https://unit42.paloaltonetworks.com/cloud-bucket-hijacking-risks/) ⭐️ 8.0/10

Unit 42 研究披露了一种通用存储桶劫持技术，该技术利用云存储桶名称的全局唯一性，将数据窃取流重定向到各大云服务提供商。 该漏洞因共享的全局命名空间而影响所有主流云服务提供商，攻击者无需直接侵入受害者云账户即可劫持数据，对云数据安全构成重大威胁。 该技术依赖于攻击者注册那些被引用但原用户不再拥有的存储桶名称（悬空存储桶），并可同样应用于 Amazon S3、Google Cloud Storage 和 Azure Blob Storage。

rss · Unit 42 Threat Research · 6月22日 22:00

**背景**: 云存储桶（如 Amazon S3 存储桶）位于全局命名空间中，这意味着桶名称在同一提供商的所有客户中必须是唯一的。当存储桶被删除但应用程序或文档中仍有引用时，攻击者可以注册相同名称并拦截原本发往原始存储桶的流量，这种情况称为悬空存储桶接管。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.google.com/blog/products/identity-security/best-practices-to-prevent-dangling-bucket-takeovers">Best practices to prevent dangling bucket takeovers | Google Cloud Blog</a></li>
<li><a href="https://www.forbes.com/sites/daveywinder/2025/08/09/now-google-warns-of-cloud-hack-attacks---3-steps-you-must-take/">Now Google Warns Of Cloud Hack Attacks — 4 Steps You Must Take</a></li>

</ul>
</details>

**标签**: `#cloud security`, `#bucket hijacking`, `#data exfiltration`, `#cloud providers`, `#vulnerability`

---

<a id="item-19"></a>
## [Unsloth GLM-5.2 本地运行指南](https://unsloth.ai/docs/models/glm-5.2) ⭐️ 7.0/10

Unsloth 发布了一份指南，详细介绍了如何在本地运行 GLM-5.2，包括量化和卸载步骤，以适配消费级硬件。 GLM-5.2 是拥有百万 token 上下文和强大编程能力的顶尖开源模型，使其能在本地运行将支持隐私保护和离线工作流，但高昂的硬件需求引发了关于可行性和成本的讨论。 完整的 GLM-5.2 模型需要 1.51 TB 磁盘空间和 256 GB 内存用于混合专家卸载，而 Unsloth 提供了量化和 CPU/GPU 卸载功能，使其可在仅 24 GB 显存的系统上运行。

hackernews · TechTechTech · 6月22日 21:21 · [社区讨论](https://news.ycombinator.com/item?id=48636377)

**背景**: GLM-5.2 是 Z.AI 开发的一款混合专家（MoE）语言模型，拥有百万 token 上下文窗口，并在 SWE-bench Pro 和 Terminal-Bench 2.1 等编程基准测试中取得最高分。Unsloth 是一个开源库，通过内存高效技术（包括 4 比特量化和卸载）加速大语言模型的微调和推理，目前支持通过其 Unsloth Studio 界面本地运行 GLM-5.2。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/unslothai/unsloth">GitHub - unslothai/unsloth: Unsloth Studio is a web UI for ... Unsloth Docs | Unsloth Documentation GitHub - 0x7C000/unsloth-LLM: Fine-tuning & Reinforcement ... Unsloth: Train Massive LLMs on Consumer GPUs with 70% Less ... Zero to Production: Step-by-Step Fine-Tuning with Unsloth Unsloth Studio Review: No-Code Local LLM Training (2026)</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM-5.2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://openlm.ai/glm-5.2/">GLM-5.2 | OpenLM.ai</a></li>

</ul>
</details>

**社区讨论**: 社区成员就 GLM-5.2 能否在消费级硬件上实际运行展开辩论：部分接近门槛的用户指出需要重度量化和缓慢的提示处理，而其他人则将其与 API 进行比较，并质疑全速 GPU 设置的成本。还有用户询问用于冷存储的无损压缩可能性。

**标签**: `#GLM-5.2`, `#local LLM`, `#Unsloth`, `#hardware requirements`, `#model inference`

---

<a id="item-20"></a>
## [Gartner 演讲警告：遗留基础设施可劫持 AI 代理](https://thehackernews.com/2026/06/stop-your-legacy-infrastructure-from.html) ⭐️ 7.0/10

在 Gartner 安全与风险管理峰会上，一位演讲者指出一个盲点：攻击者正利用遗留基础设施劫持 AI 代理，从而绕过针对 AI 的安全程序。 由于 71%的组织正在试点 AI 代理，如果遗留系统未得到保护，这种攻击途径可能破坏 AI 部署，给企业安全带来重大风险。 文章指出，AI 代理会继承来自遗留服务器、Active Directory、IAM 和云存储的风险，从而创建绕过模型级安全的攻击路径。

rss · The Hacker News · 6月22日 11:58

**背景**: AI 代理是能够代表用户执行任务的自主程序，通常与现有 IT 基础设施集成。遗留基础设施指的是可能缺乏现代安全控制的陈旧系统，如旧服务器、目录和身份管理工具。攻击者可以通过入侵这些遗留组件来操纵或劫持 AI 代理，这是许多安全程序忽视的威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/06/stop-your-legacy-infrastructure-from.html">Stop Your Legacy Infrastructure from Hijacking Your AI Agents</a></li>
<li><a href="https://www.nist.gov/news-events/news/2025/01/technical-blog-strengthening-ai-agent-hijacking-evaluations">Technical Blog: Strengthening AI Agent Hijacking Evaluations</a></li>
<li><a href="https://www.splunk.com/en_us/blog/industries/tackling-ai-driven-threats-and-legacy-risks.html">Securing Comms Infrastructure: Tackling AI-Driven Threats and ...</a></li>

</ul>
</details>

**标签**: `#AI security`, `#legacy infrastructure`, `#AI agents`, `#cybersecurity`, `#Gartner`

---