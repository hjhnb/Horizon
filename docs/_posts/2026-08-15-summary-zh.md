---
layout: default
title: "Horizon Summary: 2026-08-15 (ZH)"
date: 2026-08-15
lang: zh
---

> 从 58 条内容中筛选出 14 条重要资讯。

---

1. [Qwen 3.8 27B：开源权重本地大模型推理表现惊艳](#item-1)
2. [GLM-5.3：前沿编程模型展现涌现式网络攻防能力](#item-2)
3. [执法部门黑客行动进入‘Going Dark’时代](#item-3)
4. [Firefox 成为唯一仍支持 uBlock Origin 的主流浏览器](#item-4)
5. [别分类，去“幻觉”：LLM 标签生成新技巧](#item-5)
6. [Gemini 3.7 Flash 让谷歌 DeepMind 重回 AI 前沿](#item-6)
7. [GLM-5.3 分析：中国实验室以创新而非蒸馏保持前沿](#item-7)
8. [若市场拒绝 OpenAI 和 Anthropic，美国应将其国有化](#item-8)
9. [黑客利用 macOS 屏幕共享漏洞安装门罗币挖矿程序](#item-9)
10. [高危 SAP Commerce Cloud RCE 漏洞已遭攻击利用](#item-10)
11. [Kimi K3、Qwen3.8、DeepSeek-V4-Pro、GLM-5.3 于一个月内相继发布](#item-11)
12. [为什么 Claude Opus 5 用起来感觉更差](#item-12)
13. [RingCentral 数据泄露暴露 160 万账户信息](#item-13)
14. [苹果就雇佣间谍软件攻击发送新的威胁通知](#item-14)

---

<a id="item-1"></a>
## [Qwen 3.8 27B：开源权重本地大模型推理表现惊艳](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 9.0/10

阿里巴巴 Qwen 团队发布了 Qwen 3.8 27B，这是一个 FP8 量化、面向消费级硬件本地部署的开源权重语言模型。社区测试显示其推理能力出色，有用户称这是继 Gemma 4 之后第二个通过其私有基准测试的本地模型。 这一发布表明能力较强的开源权重大模型如今可以在日常笔记本和台式机上运行，可能减少对云端 AI 服务的依赖。这也凸显了阿里等非美国模型提供商的竞争力增强，可能重塑本地 AI 生态格局。 这个 27B 参数模型采用 FP8 格式（见 Hugging Face 仓库），社区基准测试因硬件而异：有用户报告在 RTX 5090 上使用 ninfer 引擎获得约 138 tokens/s，大约是朴素 llama.cpp 配置速度的两倍。还有用户指出其 VRAM 使用效率似乎低于 Gemma 4 或 Glimmer，且 Qwen 3.8 的压缩式'电报体'思考轨迹可能影响多 token 预测（MTP）。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**背景**: Qwen 是阿里云开发的大语言模型系列，首个 Qwen 模型于 2023 年 4 月以通义千问（Tongyi Qianwen）名称发布。开源权重大模型会公开训练参数，使任何人都可以在本地运行或微调。本地运行 LLM 需要使用 llama.cpp 等推理引擎，或 ninfer 等专用工具，后者在 RTX 5090 等特定硬件上可能更快。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://huggingface.co/Qwen">Qwen (Qwen)</a></li>
<li><a href="https://medium.com/@digitalpower/should-you-run-llms-locally-d4f9dfc09481">Should you run LLMs locally ?. When local AI models... | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区反馈以积极为主。有用户报告 Qwen 3.8 27B 是除 Gemma 4 之外首个正确通过其私有基准测试的本地模型，尽管在启用 MTP 时消耗了更多 token 并花费 12 分 30 秒。另一名用户称赞模型的图像生成质量，认为它在笔记本上运行的模型中画出了最好的鹈鹕插图。不过也有用户提出一些保留意见，例如 VRAM 占用更高，以及独特的思考轨迹模式可能影响 MTP 预测。

**标签**: `#LLM`, `#Qwen`, `#Local AI`, `#Open-weights`, `#Inference`

---

<a id="item-2"></a>
## [GLM-5.3：前沿编程模型展现涌现式网络攻防能力](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

智谱（Z.ai）发布了旗舰级开放权重编程模型 GLM-5.3，据称在关键网络安全测试中超越了 Anthropic 的 Mythos 5。该模型展现出涌现式网络能力，包括自主红队测试与漏洞利用，并支持 100 万 token 的上下文长度。 这一发布表明，编程模型正演变为能够自主开展安全研究的通用智能体，可能重塑攻防安全与漏洞披露的格局。它同时也加剧了中国与西方 AI 实验室在网络安全领域的竞争。 GLM-5.3 基于 GLM-5.2 并通过后训练改进而来，其权重预计将在两周内发布。社区测试显示，它能在红队场景中执行 WordPress 插件的 0-day 漏洞利用、远程代码执行（RCE）以及内核漏洞利用的适配。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**背景**: 涌现能力（emergent abilities）是指较小模型中不存在、但在更大模型中出现的技能，这一概念出自 2022 年的一篇开创性论文。自主红队 AI 智能体已从研究演示走向商业产品，能够独立在真实系统中发现并验证漏洞。GLM-5.3 是智谱开放权重 GLM 系列的一部分，使其成为 OpenAI GPT 系列和 Anthropic Claude 等封闭前沿模型的挑战者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scmp.com/tech/big-tech/article/3364077/zhipu-launches-flagship-model-glm-53-china-seeks-mythos-level-edge-cyber-defence">Zhipu launches flagship model GLM-5.3 as China seeks Mythos-level edge in cyber defence | South China Morning Post</a></li>
<li><a href="https://openlm.ai/glm-5.1/">GLM-5.3 | OpenLM.ai</a></li>
<li><a href="https://arxiv.org/abs/2206.07682">[2206.07682] Emergent Abilities of Large Language Models</a></li>

</ul>
</details>

**社区讨论**: 社区反应既兴奋又担忧：有用户报告了令人印象深刻的真实红队测试结果，认为 GLM-5.3 的实力已逼近顶级模型；也有用户担心大规模自动化漏洞扫描的伦理与成本问题。还有人指出该模型本质上是“GLM 5.2 加后训练魔法”，并期待权重发布后进行本地部署。

**标签**: `#AI/ML`, `#Cybersecurity`, `#Language Models`, `#Frontier Research`, `#Open Source`

---

<a id="item-3"></a>
## [执法部门黑客行动进入‘Going Dark’时代](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 8.0/10

密码学家 Matthew Green 在一篇博客文章中探讨了普遍加密如何推动执法部门转向黑客攻击，并质疑可利用软件漏洞的数量最终是否会触及上限。文章还分析了这一转变对监控和公民自由的政策影响。 这篇文章围绕政府黑客攻击的可持续性重新定义了‘Going Dark’（信息黑暗）辩论，这对监控政策、公民自由和安全研究生态至关重要。它还凸显了执法需求与推动更强加密之间的紧张关系。 文章认为，执法部门可能正接近可供黑客攻击使用的‘有用漏洞’数量上限。社区评论者对此提出质疑，指出 AI 生成的代码可能引入更多漏洞，并提供了关于物理窃听成本的历史背景。

hackernews · vslira · 8月14日 20:52 · [社区讨论](https://news.ycombinator.com/item?id=49304447)

**背景**: “Going Dark”（信息黑暗）问题指的是，由于强加密保护通信，执法部门正在丧失部分监控能力。历史上，窃听需要铺设物理线路，而现在执法机构越来越多地使用网络调查技术（NITs）和键盘记录器等黑客手段来访问加密设备。争论的焦点在于，政府是应该削弱加密，还是依赖利用软件漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cdt.org/insights/going-dark-versus-a-golden-age-for-surveillance/">‘ Going Dark ’ Versus a ‘Golden Age for Surveillance’ - Center for...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Government_hacking">Government hacking - Wikipedia</a></li>
<li><a href="https://www.congress.gov/crs-product/R44827">Law Enforcement Using and Disclosing Technology Vulnerabilities | Congress.gov | Library of Congress</a></li>

</ul>
</details>

**社区讨论**: 评论者观点不一：有人质疑漏洞上限，认为 AI 生成的代码会成为新的漏洞来源；有人引用历史上窃听的昂贵成本，说明政府监控从来不是免费或轻而易举的事。还有人带着讽刺语气欢迎任何阻碍大规模监控的因素，也有人将精英黑客行动与私营部门的基本安全失职进行对比。

**标签**: `#cryptography`, `#law enforcement`, `#privacy`, `#security`, `#surveillance`

---

<a id="item-4"></a>
## [Firefox 成为唯一仍支持 uBlock Origin 的主流浏览器](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

Firefox 已成为唯一仍完整支持 uBlock Origin 的主流浏览器，此前 Chrome 已停用 Manifest V2 扩展。这让 Firefox 成为希望继续使用原版 uBlock Origin 广告拦截器的用户的唯一主流选择。 这之所以重要，是因为广告拦截是核心隐私工具，而 Chrome 转向 Manifest V3 削弱了动态过滤能力。关心广告和追踪问题的用户可能需要转向 Firefox，从而影响浏览器市场格局。 uBlock Origin 依赖被 Manifest V3 限制的阻塞式 webRequest API；轻量版 uBlock Origin Lite 则改用 declarativeNetRequest。Mozilla 表示 Firefox 会继续支持阻塞式 webRequest API，因此完整的 uBlock Origin 仍可用。

hackernews · DemiGuru · 8月14日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49303202)

**背景**: 浏览器扩展构建在名为 WebExtensions 的平台上，该平台提供用于与网页交互的 API。Manifest V3 由 Google 于 2020 年推出，是该平台的最新版本，用限制更多的 declarativeNetRequest 规则取代了功能强大的 webRequest API。Chrome 一直在逐步淘汰 Manifest V2 扩展，这导致许多用户的 uBlock Origin 失效。Mozilla 也在实现 Manifest V3，但采取不同策略，保留了较强的广告拦截能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.mozilla.org/en/firefox/firefox-manifest-v3-adblockers/">Mozilla’s approach to Manifest V3: What’s different and why it matters for extension users | The Mozilla Blog</a></li>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://dev.to/notearthian/whats-the-difference-between-manifest-v2-and-v3-in-browser-extensions-3b10">What's the Difference Between Manifest V2 and V3 in browser extensions? - DEV Community</a></li>

</ul>
</details>

**社区讨论**: 评论者大多批评 Google 的决定，有人指出扩展本应让用户做到浏览器不允许的事情。还有人指出，依赖世界上最大广告公司之一的 Chrome 具有讽刺意味。一些用户称赞 Firefox 对热门扩展进行额外代码审查，至少一位用户表示 uBlock Origin Lite 使用起来没有明显问题。

**标签**: `#ad-blocking`, `#Firefox`, `#uBlock Origin`, `#browsers`, `#privacy`

---

<a id="item-5"></a>
## [别分类，去“幻觉”：LLM 标签生成新技巧](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 8.0/10

Doug Turnbull 提出了一种新方法：让 LLM 先“幻觉”出一些可能的标签，再通过向量嵌入（vector embeddings）将这些想象出的标签映射到现有标签库中最接近的标签。这样就不必把上千个标签的完整词汇表一次性喂给模型。 这种方法为标签空间非常大或不断变化的分类问题提供了实用方案，比如给拥有 1,800 多个标签的博客打标签。它能减小提示词规模、降低成本，同时利用嵌入的语义理解能力，对搜索和内容组织等任务很有价值。 Simon Willison 提到他的博客有 1,856 个标签，数量太多，无法一次塞进提示词。这个方法的思路是让模型先想象出可能合适的标签，再用嵌入在现有标签库中找到最接近的真实标签；提示词中会包含标签结构的示例来引导输出。

rss · Simon Willison · 8月14日 21:54

**背景**: 传统的 LLM 分类通常会给模型一个固定的标签列表并让它从中选择，但当标签有几百上千个时，这种做法就变得不现实。向量嵌入（vector embedding）把单词或句子表示成保留语义信息的数值向量，系统可以通过计算向量之间的距离来找到相似项。“幻觉”在 AI 中通常指模型编造出貌似合理但错误的信息；这个技巧刻意利用了幻觉来生成候选标签，再通过嵌入将它们对接到真实的标签集合上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/nlp/what-are-vector-embeddings/">What are Vector Embeddings? - GeeksforGeeks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)">Hallucination (artificial intelligence) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#LLM`, `#embeddings`, `#tagging`, `#classification`, `#AI`

---

<a id="item-6"></a>
## [Gemini 3.7 Flash 让谷歌 DeepMind 重回 AI 前沿](https://www.latent.space/p/ainews-gemini-37-flash-brings-gdm) ⭐️ 8.0/10

谷歌 DeepMind 发布了 Gemini 3.7 Flash，这是其 Gemini 模型系列的新成员，标志着其在 AI 模型竞赛中的重新发力。该模型以更低的成本提供更强的智能，并可通过 Databricks AI Gateway 等平台使用。 此次发布表明谷歌 DeepMind 重回 AI 开发的前沿，与 OpenAI 和 Anthropic 等竞争对手展开较量。对于企业和开发者而言，它为大规模、智能体类及推理密集型任务提供了高性价比的选择。 官方 Gemini 模型页面将 Gemini 3.7 Flash 列为谷歌 DeepMind 当前模型系列的一部分，并可集成到 Databricks AI Gateway 等企业平台。该页面还提到了预测收入、识别关键客户以及做出投资决策等用例。

rss · Latent Space · 8月14日 05:30

**背景**: 谷歌 DeepMind（GDM）是谷歌的人工智能研究部门，由 DeepMind 与谷歌大脑合并而成。Gemini 系列是其多模态大语言模型家族，Flash 变体旨在平衡性能与效率。标题中“让 GDM 重回前沿”的说法表明该组织此前可能遭遇挫折或关注度下降，而此次发布则使其重新受到瞩目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3.7 Flash - Google DeepMind</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models">Models - Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google DeepMind`, `#Gemini`, `#Model Release`, `#AI News`

---

<a id="item-7"></a>
## [GLM-5.3 分析：中国实验室以创新而非蒸馏保持前沿](https://www.interconnects.ai/p/glm-53-how-chinese-labs-keep-stride) ⭐️ 8.0/10

Nathan Lambert 发表了一篇新分析，认为 GLM-5.3 表明中国 AI 实验室正通过真正的创新而非蒸馏来取得进步。GLM-5.3 是智谱（Z.ai）最新旗舰模型，完全通过后训练在 GLM-5.2 基础上改进。 这一分析挑战了“中国 AI 模型只是衍生品”的常见说法，对全球 AI 竞争和开源权重模型生态具有重要影响。它也凸显了后训练与智能体能力在前沿模型开发中日益增长的重要性。 GLM-5.3 与 GLM-5.2 共用同一基础模型，所有改进均来自后训练，包括在复杂软件工程和智能体任务方面的进步。截至 2026 年 7 月，该模型尚未正式发布，仅由团队负责人唐杰通过社区预告透露过。

rss · Interconnects · 8月14日 21:23

**背景**: 知识蒸馏是一种让较小的“学生”模型学习复制较大“教师”模型行为的技术，过去许多中国 AI 模型被怀疑是从 GPT-4 等西方前沿模型蒸馏而来。GLM 是智谱 AI（Z.ai）推出的开源权重模型系列。Lambert 的分析认为，GLM-5.3 以纯后训练取得进步并在智能体任务上表现优异，体现了独特的创新路径。这也与开源权重模型日益挑战封闭系统的全球趋势相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kie.ai/blog/what-is-glm-5-3">What Is GLM - 5 . 3 ? Z. ai 's Next Open-Weight Model</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM - 5 . 3 - Overview - Z. AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#GLM`, `#Chinese Labs`, `#Model Development`, `#Frontier Research`

---

<a id="item-8"></a>
## [若市场拒绝 OpenAI 和 Anthropic，美国应将其国有化](https://www.schneier.com/blog/archives/2026/08/if-the-markets-reject-openai-and-anthropic-the-us-should-nationalize-them.html) ⭐️ 8.0/10

Bruce Schneier 和 Nathan E. Sanders 在《卫报》发表的文章提出，如果市场力量损害 OpenAI 和 Anthropic 的公共利益使命，美国政府应考虑将其国有化。 这一提议意义重大，因为它挑战了“以利润为导向的私营 AI 实验室足以维护公共利益”的主流假设，并将国有化作为 AI 治理的一个主流政策选项提上议程。 作者指出，OpenAI 和 Anthropic 成立之初旨在对抗不安全的公司 AI 开发，但自身也被市场激励所同化。他们建议，如果这些公司不能将公共利益置于投资者价值之上，国有化应作为备选方案。

rss · Schneier on Security · 8月14日 11:03

**背景**: OpenAI 和 Anthropic 是两家以安全为核心使命的大型 AI 实验室。OpenAI 于 2015 年作为非营利组织成立，后来转向“利润上限”模式；Anthropic 则由担心 AI 失控的 OpenAI 前研究人员创立。如今两者都已成为大型企业，这引发了人们对市场激励是否会压倒其最初公共利益目标的担忧。

**标签**: `#AI policy`, `#OpenAI`, `#Anthropic`, `#regulation`, `#nationalization`

---

<a id="item-9"></a>
## [黑客利用 macOS 屏幕共享漏洞安装门罗币挖矿程序](https://www.bleepingcomputer.com/news/security/hackers-exploit-macos-screen-sharing-flaw-to-deploy-monero-miner/) ⭐️ 8.0/10

据荷兰国家网络安全中心（NCSC）警告，攻击者正在积极利用 macOS 屏幕共享功能中的身份验证绕过漏洞，安装门罗币（Monero）加密货币挖矿程序。该警告是在该漏洞的公开利用代码发布后发布的。 这一事件意义重大，因为它代表针对 macOS 内置功能的野外主动攻击，使受影响的 Mac 面临未经授权访问和资源被劫持的风险。公开漏洞利用代码降低了其他攻击者的门槛，NCSC 的警告也表明个人和组织面临切实威胁。 该漏洞是 macOS 屏幕共享功能中的身份验证绕过，允许攻击者在没有有效凭据的情况下进行远程访问。攻击者利用此漏洞部署门罗币（XMR）矿工，可能使用 CPU 密集型的 RandomX 算法，该算法旨在抵抗 ASIC 挖矿。

rss · BleepingComputer · 8月14日 14:59

**背景**: 门罗币是一种注重隐私的加密货币，采用工作量证明（PoW）共识机制；其挖矿过程在 CPU 和 GPU 上运行，且交易难以追踪，因此常被非法挖矿者选用。屏幕共享是 macOS 内置功能，允许用户远程查看和控制另一台 Mac。身份验证绕过漏洞（归入 CWE-287 类缺陷）可让攻击者无需提供有效凭据即可获得访问权限，完全跳过正常登录过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.getmonero.org/get-started/mining/">Mining Monero | Monero - secure, private, untraceable</a></li>
<li><a href="https://support.apple.com/guide/mac-help/share-the-screen-of-another-mac-mh14066/mac">Share the screen of another Mac - Apple Support</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/identity-security/authentication-bypass/">What Is Authentication Bypass? Techniques & Examples</a></li>

</ul>
</details>

**标签**: `#security`, `#macOS`, `#exploit`, `#cryptocurrency mining`, `#vulnerability`

---

<a id="item-10"></a>
## [高危 SAP Commerce Cloud RCE 漏洞已遭攻击利用](https://www.bleepingcomputer.com/news/security/max-severity-sap-commerce-cloud-flaw-now-targeted-in-attacks/) ⭐️ 8.0/10

据威胁情报公司 Defused 称，三天前刚修复的一个 SAP Commerce Cloud 最高严重级别远程代码执行漏洞，目前已被攻击者积极利用。 这一事件非常关键，因为该漏洞属于最高严重级别的远程代码执行漏洞，攻击者有可能完全控制受影响的 SAP Commerce Cloud 实例。使用该平台的企业必须立即应用补丁，以防止数据泄露和系统被入侵。 该漏洞影响 SAP Commerce Cloud，这是一个曾名为 hybris、由 SAP 于 2013 年收购的电子商务平台。Defused 报告称，补丁发布后不久就出现了主动利用行为，这凸显了紧急缓解措施的必要性。

rss · BleepingComputer · 8月14日 13:45

**背景**: SAP Commerce Cloud 是一款面向 B2B 和 B2C 企业的云电子商务解决方案，可提供统一的购买体验。远程代码执行（RCE）漏洞允许攻击者在服务器上运行任意代码，可能导致数据窃取、勒索软件或系统完全失守。由于该漏洞目前已遭积极利用，所有受影响企业及时打补丁都刻不容缓。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sap.com/products/crm/commerce-cloud.html">SAP Commerce Cloud Overview | SAP E- Commerce Software</a></li>
<li><a href="https://www.sap.com/products/acquired-brands/what-is-hybris.html">What is hybris | e- Commerce Software from SAP</a></li>

</ul>
</details>

**标签**: `#security`, `#SAP`, `#vulnerability`, `#RCE`, `#exploit`

---

<a id="item-11"></a>
## [Kimi K3、Qwen3.8、DeepSeek-V4-Pro、GLM-5.3 于一个月内相继发布](https://www.reddit.com/r/LocalLLaMA/comments/1vo9k39/less_than_a_month_kimi_k3_qwen38/) ⭐️ 8.0/10

一篇 Reddit 帖子指出，Kimi K3、Qwen3.8、DeepSeek-V4-Pro-0813 和 GLM-5.3 这四款国产大语言模型均在不到一个月内发布。帖中列出了它们的参数量，分别为 2.8T、2.4T、1.6T 和 743B。 如此密集的发布节奏凸显了中国大语言模型研发的激烈程度，也加剧了全球 AI 竞争的态势。开发者和企业现在可以在极短的时间内评估多款更近期、更具能力的模型。 帖子显示这些模型分别为 Kimi K3（2.8T 参数）、Qwen3.8（2.4T）、DeepSeek-V4-Pro-0813（1.6T）和 GLM-5.3（743B）。该帖更像是一份非正式的社区汇总，而非官方联合公告，并且没有附带基准测试对比。

reddit · r/LocalLLaMA · /u/chibop1 · 8月14日 14:57

**背景**: 中国的 AI 实验室，如月之暗面（Kimi）、阿里巴巴（Qwen）、DeepSeek 和智谱（GLM），一直在快速迭代大语言模型。在一个月内密集发布多款旗舰模型，意味着新参数规模和新能力上线的速度已超过很多团队的评测节奏。2026 年的第三方对比（如 Artificial Analysis）显示，这些模型在智能、数学和代码等基准上互有领先。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lovableapp.org/blog/qwen-38-max-vs-glm-52-vs-kimi-k3-vs-deepseek-v4-flash">Qwen 3.8 Max vs GLM 5.2 vs Kimi K3 vs DeepSeek V4 Flash (2026 ...</a></li>
<li><a href="https://www.elser.ai/news/kimi-k3-vs-deepseek-v4-vs-qwen3-8">Kimi K3 vs DeepSeek V4 vs Qwen3.8: A Practical 2026 Model ...</a></li>
<li><a href="https://dev.to/van_massey/kimi-k3-vs-deepseek-v4-pro-vs-qwen-38-which-open-weight-model-should-developers-choose-in-2026-5h69">Kimi K3 vs DeepSeek V4 Pro vs Qwen 3.8: Which Open-Weight ...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#China`, `#AI models`, `#DeepSeek`, `#Qwen`

---

<a id="item-12"></a>
## [为什么 Claude Opus 5 用起来感觉更差](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 7.0/10

一篇发布在 mun-logadan.github.io 上的博客文章认为，Anthropic 的 Claude Opus 5 使用一种省略式、面向智能体的沟通风格，因此对人类用户来说感觉更不舒适，尽管它更强大。相关的 Hacker News 讨论获得了 747 分和 685 条评论，反映出社区对该话题的浓厚兴趣。 这次用户的反感凸显了在为智能体到智能体（agent-to-agent）工作流优化 AI 模型与保留人类友好体验之间日益增长的矛盾。这可能会影响从业者在前沿模型之间的选择，并促使模型提供商重新考虑其后训练（post-training）的优先级。 评论者特别批评 Opus 5 使用无生命名词作句子主语、抽象的措辞，以及过度“坦白”错误。一些用户表示已经转向 OpenAI 的“Sol”模型，另一些人则推测其后训练（post-training）现在面向的是智能体而非人类。

hackernews · numeri · 8月14日 10:12 · [社区讨论](https://news.ycombinator.com/item?id=49296740)

**背景**: Claude Opus 5 是 Anthropic 最新的前沿大语言模型，旨在处理复杂的推理和智能体任务。“省略式”（elliptical）语言会省略词语或有意让逻辑联系变得隐晦，因此听起来可能很抽象或简洁。“面向智能体”（agent-oriented）意味着输出是为 AI 智能体——能够自主追求目标并采取行动的程序——使用的，而不是为了便于人类阅读。这篇博客及相关讨论反映了 AI 助手究竟应该为人类交互还是为最高任务效率进行优化的更广泛争论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types | Google ...</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-agents-vs-ai-assistants">AI agents vs. AI assistants - IBM</a></li>

</ul>
</details>

**社区讨论**: 总体而言，评论者大多认同批评：许多人觉得 Opus 5 的风格让人疲惫且过度煽情，有人甚至因此转向 OpenAI 的 Sol。一些人推测该模型不再以人类读者为主要受众，而是写给其他智能体看的；另一些人则警告说，如果体验不改善，企业用户可能会放弃 Anthropic。

**标签**: `#AI`, `#LLM`, `#Claude Opus 5`, `#Human-Computer Interaction`, `#Model Behavior`

---

<a id="item-13"></a>
## [RingCentral 数据泄露暴露 160 万账户信息](https://www.bleepingcomputer.com/news/security/ringcentral-data-breach-exposed-info-of-16-million-accounts/) ⭐️ 7.0/10

据 Have I Been Pwned 披露，ShinyHunters 黑客组织在 7 月入侵 RingCentral 后窃取了 160 万个账户的个人信息。在现有内容中，该泄露事件是由 HIBP 公开披露，而非 RingCentral 自行公布。 此次泄露影响了知名云通信平台的大量用户，可能暴露敏感的个人信息。同时，它也凸显了以勒索为目的的黑客组织对 SaaS 服务商及其客户构成的持续威胁。 该事件据称发生在 7 月，泄露的数据现已被 Have I Been Pwned 收录，供受影响用户查询。本条新闻没有社区评论，因此无法了解公众的具体反应。

rss · BleepingComputer · 8月14日 10:52

**背景**: ShinyHunters 是一支自 2019 年以来活跃的黑客组织，以大规模数据泄露和勒索行为闻名。Have I Been Pwned (HIBP) 是一个广泛使用的泄露通知服务，用户可用它查询自己的账户是否在已知的数据泄漏中遭泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ShinyHunters">ShinyHunters - Wikipedia</a></li>

</ul>
</details>

**标签**: `#data breach`, `#security`, `#RingCentral`, `#privacy`, `#incident response`

---

<a id="item-14"></a>
## [苹果就雇佣间谍软件攻击发送新的威胁通知](https://www.bleepingcomputer.com/news/apple/apple-sends-new-threat-notification-alerts-over-mercenary-spyware-attacks/) ⭐️ 7.0/10

苹果已向疑遭雇佣间谍软件单独针对的 iPhone 用户发送了新一轮威胁通知。这些通知警告用户其设备可能已被入侵，并包含推送通知组件。 这很重要，因为像 Pegasus 这样的雇佣间谍软件被政府用来监视记者、律师和活动人士，因此这些提醒对高风险人群而言是至关重要的早期预警。这也进一步体现了苹果在防御国家支持监控方面的作用。 苹果的威胁通知独立于常规安全更新，专门面向可能被雇佣间谍软件单独针对的用户。用户应通过苹果官方支持页面核实通知真伪，尤其是现在这类提醒会以推送通知形式出现。

rss · BleepingComputer · 8月14日 01:19

**背景**: 雇佣间谍软件是商业监控软件，例如 NSO 集团的 Pegasus，它可被秘密安装到 iPhone 和 Android 设备上。这类软件通常出售给政府，并被用来针对记者、异见人士和活动人士，常利用零日漏洞实现远程访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-us/102174">About Apple threat notifications and protecting against ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware) - Wikipedia</a></li>
<li><a href="https://lifehacker.com/tech/how-to-tell-if-that-apple-threat-notification-is-legit">How to Tell If That Apple 'Threat Notification' Is Legit</a></li>

</ul>
</details>

**标签**: `#security`, `#apple`, `#spyware`, `#ios`, `#threat notification`

---