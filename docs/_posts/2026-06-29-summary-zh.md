---
layout: default
title: "Horizon Summary: 2026-06-29 (ZH)"
date: 2026-06-29
lang: zh
---

> 从 28 条内容中筛选出 11 条重要资讯。

---

1. [GLM 5.2 在网络安全基准测试中击败 Claude](#item-1)
2. [用 Claude Code 获取 MRI 第二意见](#item-2)
3. [布朗大学教授报告大规模 AI 作弊事件](#item-3)
4. [浏览器快捷键拦截波兰字母：技术深度解析](#item-4)
5. [KIDS 法案要求在线平台进行年龄验证](#item-5)
6. [Jon Udell 提议用“代理在循环中”取代“人在循环中”](#item-6)
7. [历史内存价格图表（1960-2026）引发讨论](#item-7)
8. [纽约公共图书馆 5000 份历史菜单可视化](#item-8)
9. [Librepods: 解放 AirPods](#item-9)
10. [OpenAI Codex 敏感文件排除问题仍未解决](#item-10)
11. [KDDI 数据泄露暴露 1420 万电子邮件登录信息](#item-11)

---

<a id="item-1"></a>
## [GLM 5.2 在网络安全基准测试中击败 Claude](https://semgrep.dev/blog/2026/we-have-mythos-at-home-glm-52-beats-claude-in-our-cyber-benchmarks/) ⭐️ 8.0/10

网络安全公司 Semgrep 发布的基准测试显示，开放权重模型 GLM 5.2 在网络安全任务上超越了 Anthropic 的 Claude。 这一结果凸显了开源模型与专有领导者之间日益增长的竞争力，可能会降低安全团队的成本并提高可及性。 GLM 5.2 是一个 744B 参数模型，具有 40B 活跃参数和 100 万 token 的上下文窗口，由 Z.AI 提供。Semgrep 的基准测试评估了模型发现其自有工具 Mythos 曾发现的漏洞的能力。

hackernews · jms703 · 6月28日 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48709670)

**背景**: Semgrep 是一个开源静态分析工具，通过语义模式匹配检测错误和安全漏洞。该公司还维护一个网络安全基准测试，用于评估 AI 模型发现真实漏洞的能力。GLM 5.2 是 Z.AI 最新的开放权重模型，专为长周期编码、推理和智能体任务设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://unsloth.ai/docs/models/glm-5.2">GLM-5.2 - How to Run Locally | Unsloth Documentation</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM-5.2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的社区评论显示出强烈兴趣，用户称赞 GLM 5.2 的成本效益和在实际编程任务中的表现。一些人指出其 753B 参数规模引发了对本地部署硬件需求的疑问。

**标签**: `#GLM 5.2`, `#AI benchmarks`, `#open source LLM`, `#cybersecurity`, `#Claude`

---

<a id="item-2"></a>
## [用 Claude Code 获取 MRI 第二意见](https://antoine.fi/mri-analysis-using-claude-code-opus) ⭐️ 8.0/10

作者使用 Anthropic 开发的 AI 编程代理 Claude Code 分析自己的 MRI 扫描，获取肩部诊断的第二意见，引发了社区关于 AI 在医疗领域可靠性的辩论。 这一实验凸显了像 Claude 这样的 LLM 帮助患者解读医学影像的潜力，但也引发了对信任、准确性以及 AI 驱动诊断伦理影响的严重担忧。 Claude Code 主要是一款软件开发工具，但作者将其重新用于医学图像分析。该帖子获得了 418 条评论，包括一位放射科医生的见解，他指出超声波在检测钙化方面效果不佳。

hackernews · engmarketer · 6月28日 16:35 · [社区讨论](https://news.ycombinator.com/item?id=48708941)

**背景**: Claude 是 Anthropic 开发的一系列大型语言模型，采用宪法 AI 训练以提高伦理合规性。Claude Code 是一个能读取代码库和编辑文件的代理，但用户也在编码之外尝试使用它。使用 AI 获取医疗第二意见存在争议，专家警告不要过度依赖，因为可能存在误诊风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 一位放射科医生评论说，没有完整的 3D 数据集无法做出判断，并指出超声波的局限性。另一位用户分享了自己因过度依赖放射科医生报告而被误诊为结核病的个人经历。讨论围绕信任展开：用户更愿意向 AI 提问澄清而不是向医生提问，但也承认不能完全信任 AI。

**标签**: `#AI`, `#healthcare`, `#radiology`, `#LLM`, `#medical diagnosis`

---

<a id="item-3"></a>
## [布朗大学教授报告大规模 AI 作弊事件](https://english.elpais.com/education/2026-06-28/ai-fraud-at-brown-university-academic-integrity-is-at-risk.html) ⭐️ 8.0/10

此案例凸显了在 AI 时代重新思考传统评估方式的紧迫性，因为开卷考试变得越来越容易被作弊。其结果可能重塑全球大学设计课程和评估学生的方式。 教授指出作弊是通过答案模式的统计异常检测出来的。有关考试的具体细节或涉及的学生人数尚未公布。

hackernews · geox · 6月28日 16:41 · [社区讨论](https://news.ycombinator.com/item?id=48708991)

**背景**: 像 GPT-4 这样的大型语言模型能生成类似人类文本，使学生容易完成开卷作业的答案。随着 AI 工具变得普及，大学正在努力解决如何维护学术诚信的问题。许多机构正在考虑线下监考考试和口头面试作为应对措施。

**社区讨论**: 评论者普遍认为 AI 不是根本问题，而是评估设计的问题。建议包括线下手写考试、一对一面试以及改革评分体系。一些人认为大学不应再为企业免费筛选人才，而另一些人则指出当竞争对手使用 AI 时，从博弈论角度看使用 AI 是不可避免的。

**标签**: `#AI ethics`, `#education`, `#academic integrity`, `#assessment`, `#cheating`

---

<a id="item-4"></a>
## [浏览器快捷键拦截波兰字母：技术深度解析](https://aresluna.org/the-curious-case-of-the-disappearing-polish-s/) ⭐️ 8.0/10

一篇 2015 年的技术文章揭示了浏览器键盘快捷键（如 Ctrl+Alt 或 AltGr 组合键）如何拦截用于输入波兰语变音字母（如'ś'）的按键，导致用户无法正常输入。文章还提出了基于 JavaScript 的修复方案以恢复正确的输入功能。 此问题影响数百万波兰语及其他使用变音符号语言的用户，揭示了浏览器中一个被忽视的国际化问题。它凸显了软件设计中改进键盘事件处理和文化敏感性的必要性。 冲突源于波兰语字母（如'ś'）在波兰键盘布局中通过 AltGr+s 输入，而浏览器常将相同按键组合映射为快捷键（如 Ctrl+Shift+S）。提出的修复方案使用 JavaScript 事件监听器来检测并阻止这些特定组合的浏览器默认行为。

hackernews · colinprince · 6月28日 12:44 · [社区讨论](https://news.ycombinator.com/item?id=48706814)

**背景**: 波兰语使用拉丁字母，并附加了九个变音符号字符，例如'ś'和'ć'。在波兰键盘上，这些字符通常通过 AltGr 键（右 Alt）加基础字母来输入。AltGr 键是欧洲键盘布局中常见的修饰键，用于访问第三级符号，但它可能与同样使用 Alt 或 Ctrl 修饰键的浏览器快捷键发生冲突。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AltGr_key">AltGr key</a></li>
<li><a href="https://www.claviervirtuel.com/en/polish-keyboard">Keyboard Polish online</a></li>

</ul>
</details>

**社区讨论**: 评论者补充了文化背景，指出波兰使用拉丁字母反映了其向西方的靠拢。技术用户报告了 Microsoft Copilot 的类似问题，并讨论了浏览器按键处理的局限性和 Unicode 规范化细节，例如波兰字母'ł'在规范分解形式下不会分解。

**标签**: `#internationalization`, `#Unicode`, `#browser shortcuts`, `#Polish language`, `#software engineering`

---

<a id="item-5"></a>
## [KIDS 法案要求在线平台进行年龄验证](https://www.eff.org/deeplinks/2026/06/kids-act-would-require-age-checks-get-online) ⭐️ 8.0/10

KIDS 法案是一项提议中的美国联邦法案，要求在线平台实施年龄验证措施以限制未成年人访问。 这项立法可能从根本上改变互联网平台处理用户隐私和言论自由的方式，可能影响所有受该法案覆盖的在线服务。 该法案特别针对使用个人信息进行广告、营销或内容推荐的平台，而个人博客或讨论论坛等许多网站可能获得豁免。

hackernews · bilsbie · 6月28日 11:56 · [社区讨论](https://news.ycombinator.com/item?id=48706560)

**背景**: KIDS 法案（儿童互联网设计与安全法案）是在美国国会提出的一项法案，旨在通过要求某些平台进行年龄验证来保护未成年人上网安全。年龄验证通常涉及收集政府身份证或生物特征数据，引发了重大的隐私和监控担忧。电子前哨基金会（EFF）批评该法案威胁公民自由，认为可能导致所有互联网用户被迫进行身份检查。

**社区讨论**: Hacker News 的评论者就法案的适用范围展开辩论，一些人质疑像 HN 这样的网站是否会被覆盖，另一些人则讨论社交媒体与心理健康问题之间缺乏有力证据。还有人对此类立法的政治动机以及西方国家普遍推行类似互联网限制的趋势表示怀疑。

**标签**: `#privacy`, `#legislation`, `#age verification`, `#internet governance`, `#civil liberties`

---

<a id="item-6"></a>
## [Jon Udell 提议用“代理在循环中”取代“人在循环中”](https://simonwillison.net/2026/Jun/28/jon-udell/#atom-everything) ⭐️ 8.0/10

Jon Udell 主张将“人在循环中”的概念重新定义为“代理在循环中”，倡导将 AI 代理邀请到以人为中心的工作流程中，而不是将权力交给机器。 这一观点将叙事从以机器为中心转向以人为中心的 AI 集成，使开发者能够在利用 AI 代理进行代码审查等任务的同时保持控制权。 Udell 强调，代理辅助的过程不应该是黑箱；相反，代理应产生透明、可审查的拉取请求，以适应现有的开发者工作流程。

rss · Simon Willison · 6月28日 21:57

**背景**: 传统的“人在循环中”概念将人类视为 AI 系统的后备监控者，往往暗示由 AI 主导而人类监督。Udell 颠倒了这一观点，断言工作流程属于人类，代理是被邀请的参与者。这与软件开发领域关于代理工程和内外循环范式的广泛讨论相一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.jonudell.net/2026/06/28/doctor-it-hurts-when-agents-create-unreviewable-prs-dont-do-that/">“Doctor, it hurts when agents create unreviewable PRs.” “Don’t do that.”</a></li>
<li><a href="https://www.openhands.dev/blog/20251202-agents-in-the-outer-loop">Agents in the Outer Loop | Dec 02, 2025</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#software development`, `#human-in-the-loop`, `#code review`, `#workflow`

---

<a id="item-7"></a>
## [历史内存价格图表（1960-2026）引发讨论](https://dam.stanford.edu/memory-prices.html) ⭐️ 7.0/10

斯坦福大学发布了一张从 1960 年到 2026 年的内存价格历史图表，展示了每 GB 价格的长期下降趋势，但最近因 AI 和加密货币需求而出现波动和上涨。 这张图表为了解当前内存价格波动提供了重要的历史背景，对消费者、投资者和科技行业都有影响。 图表中的价格未经通胀调整，且早期（1960-1980 年）的数据点是将每 GB 定价回溯应用于当时内存容量远小于 GB 级别的时代。

hackernews · vga1 · 6月28日 18:32 · [社区讨论](https://news.ycombinator.com/item?id=48710092)

**背景**: 内存价格从 1960 年代磁芯存储器的每比特约 1 美元下降到现代 DRAM 的每 GB 几美分，但近年来 AI 和加密货币需求导致价格飙升。磁芯存储器是 1955 年至 1975 年间主流的 RAM 技术，使用铁氧体磁环非易失地存储比特。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Magnetic-core_memory">Magnetic-core memory</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了图表的有效性，指出其未调整通胀、每 GB 单位在早期具有误导性，以及最近的波动与 AI 和加密货币相关。一些人看到 2025 年后价格下跌趋势，但担忧供应侧可能的人为操控。

**标签**: `#memory`, `#pricing`, `#history`, `#hardware`, `#economics`

---

<a id="item-8"></a>
## [纽约公共图书馆 5000 份历史菜单可视化](https://pudding.cool/2026/06/menu-story/) ⭐️ 7.0/10

Pudding 网站制作了一个交互式可视化作品，展示了纽约公共图书馆 Buttolph 收藏中超过 5000 份 1880 年至 1920 年的菜单，揭示了餐饮趋势，如冰淇淋的兴起和水煮菜肴的消失。 这项工作使庞大的历史档案变得易于访问且引人入胜，揭示了美国四十年间餐饮习惯的文化变迁，并为数据驱动的人文学科叙事提供了典范。 该可视化作品包含精选故事和交互式图表，突出了芹菜作为珍品的显著地位和水煮食品的衰退，社区贡献也增添了背景见解。

hackernews · xbryanx · 6月28日 14:44 · [社区讨论](https://news.ycombinator.com/item?id=48707763)

**背景**: 纽约公共图书馆的 Buttolph 收藏是最大的历史菜单档案之一，包含超过 4 万件物品。这个 1880 年至 1920 年的子集捕捉了美国美食、城市化和餐厅文化快速变化的时期。Pudding 的可视化利用数据分析来识别跨年代的模式。

**社区讨论**: 评论者分享了历史趣闻，比如德国用啤酒垫记录啤酒消费（涂改被视为伪造），纽约中餐外卖菜单美学的演变，以及芹菜作为珍品的历史地位，从而用文化背景丰富了数据集。

**标签**: `#data visualization`, `#history`, `#menus`, `#cultural analysis`, `#NYPL`

---

<a id="item-9"></a>
## [Librepods: 解放 AirPods](https://github.com/librepods-org/librepods) ⭐️ 7.0/10

Librepods 是一个开源项目，让 AirPods 在非苹果设备（如 Android 和 Linux）上实现完整功能，包括电池状态、噪声控制、入耳检测和自适应透明度等。 该项目很重要，因为它将 AirPods 用户从苹果生态系统中解放出来，使其在任何设备上都能使用高级功能，解决了用户的普遍痛点，并扩展了 AirPods 的实用性。 该项目以 Android APK 形式提供，也可能有 Linux 版本，但可能面临苹果未来更新封堵的风险。其实现涉及逆向工程苹果的专有蓝牙协议。

hackernews · rbanffy · 6月28日 18:48 · [社区讨论](https://news.ycombinator.com/item?id=48710232)

**背景**: 苹果的 AirPods 拥有专有功能，如无缝配对、电量显示、入耳检测和噪声控制，但由于苹果的专有蓝牙协议，这些功能仅在苹果设备上可用。Librepods 通过逆向工程在其他平台上复制这些功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/librepods-org/librepods">GitHub - librepods-org/librepods: AirPods liberated from ...</a></li>
<li><a href="https://www.theverge.com/news/824953/librepods-apple-airpods-wireless-headphones-android-linux">AirPods ’ best features come to Android and Linux with... | The Verge</a></li>

</ul>
</details>

**社区讨论**: 社区讨论澄清说，AirPods 在非苹果设备上已经可以作为普通蓝牙耳机使用；Librepods 增加了额外功能。一些用户担心苹果未来会封堵这个解决方案，而另一些用户则赞赏这个开源努力。

**标签**: `#open-source`, `#AirPods`, `#Bluetooth`, `#Apple`, `#features`

---

<a id="item-10"></a>
## [OpenAI Codex 敏感文件排除问题仍未解决](https://github.com/openai/codex/issues/2847) ⭐️ 7.0/10

OpenAI Codex 的 GitHub 问题 #2847 要求增加功能以排除 AI 编码代理访问敏感文件，该问题仍处于开放状态并引发社区积极讨论。 该问题凸显了 AI 编码代理的关键安全漏洞：若无适当的文件排除机制，API 密钥和凭证等敏感数据可能被无意上传至模型。这场讨论将影响未来代理如何处理隐私和用户信任。 社区成员认为黑名单方法不足，建议使用系统级解决方案，如文件权限（chmod）或容器化。部分成员已构建内部沙箱工具，例如 NVIDIA 开源的 Rumpelpod，来解决此问题。

hackernews · pikseladam · 6月28日 12:27 · [社区讨论](https://news.ycombinator.com/item?id=48706714)

**背景**: OpenAI Codex 是一个轻量级编码代理，在用户本地机器上运行，执行命令并读取文件。如果敏感文件对 Codex 进程可读，可能会被无意访问。需要适当的沙箱或选择性文件授权来防止数据泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybermediacreations.com/a-way-to-exclude-sensitive-files-issue-still-open-for-openai-codex/">A way to exclude sensitive files issue still open for OpenAI Codex</a></li>

</ul>
</details>

**社区讨论**: 社区意见存在分歧：有人主张使用操作系统级控制（如 chmod 或容器），而另一些人认为只有选择性沙箱才能提供真正的安全。部分评论者警告，鉴于大语言模型的不可预测性，在工具中实现黑名单可能会产生虚假的安全感。

**标签**: `#AI`, `#security`, `#codex`, `#file exclusion`, `#privacy`

---

<a id="item-11"></a>
## [KDDI 数据泄露暴露 1420 万电子邮件登录信息](https://www.bleepingcomputer.com/news/security/data-breach-exposes-up-to-142-million-email-logins-at-six-isps/) ⭐️ 7.0/10

KDDI 公司披露了一起数据泄露事件，攻击者侵入了用于六家日本互联网服务提供商的电子邮件系统，可能暴露了多达 1420 万个电子邮件登录信息。 此次泄露影响多家 ISP 的数百万用户，带来凭证窃取、钓鱼攻击和身份欺诈的风险，并凸显了电信基础设施中的安全漏洞。 泄露涉及除 KDDI 外五家 ISP 使用的电子邮件系统，受影响账户总数高达 1420 万个。攻击者侵入了 KDDI 的一个电子邮件系统。

rss · BleepingComputer · 6月28日 14:13

**背景**: KDDI 是日本主要的电信运营商，为其他 ISP 提供电子邮件服务，因此这是一次供应链泄露。电子邮件登录信息可被用于账户接管，若用户重复使用密码则可能引发进一步攻击。

**标签**: `#cybersecurity`, `#data breach`, `#telecom`, `#email`, `#Japan`

---