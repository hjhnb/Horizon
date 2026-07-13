---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> 从 37 条内容中筛选出 11 条重要资讯。

---

1. [Geohot 对 LLM 炒作的细致批评](#item-1)
2. [Claude Code 在读取提示前发送 3.3 万 tokens；OpenCode 仅 7 千](#item-2)
3. [Terry Tao 谈用 LLM 编码代理构建应用](#item-3)
4. [开源 AI 面临 6 个月的生存考验](#item-4)
5. [苹果起诉 OpenAI 窃取商业秘密](#item-5)
6. [将 J-lens 应用于 Qwen3-8B 监控静默推理](#item-6)
7. [小米悄然在 Hugging Face 发布 MiMo-V2.5-DFlash](#item-7)
8. [三行代码修复 llama.cpp 中 Tesla P100 的 fp16 精度问题](#item-8)
9. [Voodoo Quant 声称比 Unsloth Dynamic 2.0 KLD 提升 95%](#item-9)
10. [消息称 DeepSeek 正研发自有 AI 芯片](#item-10)
11. [RedHook 恶意软件滥用无线 ADB 获取 Shell 访问权限](#item-11)

---

<a id="item-1"></a>
## [Geohot 对 LLM 炒作的细致批评](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 9.0/10

工程师 geohot 在一篇博客文章中表达了对 LLM 的喜爱，同时谴责了前沿 AI 实验室的炒作和过高估值，认为这些实验室可能无法捕获他们所创造的价值。 这一观点挑战了 AI 作为必然万亿美元机遇的叙事，突显了价值创造与捕获之间可能存在的脱节，这可能会重塑投资和开源生态。 Geohot 的主要论点是前沿实验室不太可能捕获他们创造的价值，这与以往的技术浪潮类似。他还指出，LLM 带来的生产力提升是真实的，但可能导致开源贡献的碎片化。

hackernews · therepanic · 7月12日 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48883343)

**背景**: 大型语言模型 (LLM) 是在海量文本数据上训练的 AI 系统，能生成类似人类的文本。OpenAI、Anthropic 等前沿实验室开发尖端模型，但因定价和炒作而受到批评。Geohot (George Hotz) 是知名工程师和 comma.ai 创始人，以其技术见解备受尊重。随着模型能力增强，关于 LLM 炒作与真正实用性的辩论日益激烈。

**社区讨论**: 评论者大多赞同 geohot 关于价值捕获的论点，一些人分享了使用 LLM 做小众项目的个人体验，认为进入了‘按需定制’时代。其他人对模型的快速改进（如 Sonnet 4）表示乐观，但仍对 AGI 时间线持怀疑态度。

**标签**: `#LLMs`, `#hype`, `#open source`, `#productivity`, `#frontier labs`

---

<a id="item-2"></a>
## [Claude Code 在读取提示前发送 3.3 万 tokens；OpenCode 仅 7 千](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

一项对比研究表明，Claude Code 在读取用户初始提示之前，会在系统提示和编排开销中传输约 33,000 个 tokens，而 OpenCode 仅使用约 7,000 个 tokens。 这种显著的 token 低效直接增加了开发者使用 Claude Code 的 API 成本，可能使其在编码任务中不如 OpenCode 等替代方案经济。这也引发了对 AI 编码工具在丰富上下文与成本效益之间设计权衡的思考。 Claude Code 的开销归因于激进的系统提示和 sub-agent 编排，它会生成多个 sub-agent，快速消耗 tokens。该研究捕获了工具与 Anthropic 端点之间的所有请求，在多个任务中确认了这一模式。

hackernews · systima · 7月12日 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48883275)

**背景**: 像 Claude Code 和 OpenCode 这样的智能编码工具利用大语言模型自主执行编码任务。它们依赖系统提示来定义行为，并常常使用 sub-agent 编排来处理复杂任务，即生成多个专门化的代理。每个 sub-agent 都会增加自身的 tokens 开销，而缓存策略旨在减少冗余 tokens。tokens 用量直接转化为成本，因为大多数大语言模型 API 按 tokens 计费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/subagent-orchestration">Subagent orchestration: The complete 2025 guide for AI workflows</a></li>
<li><a href="https://github.com/pleasedodisturb/awesome-llm-token-optimization">pleasedodisturb/awesome-llm-token-optimization - GitHub</a></li>
<li><a href="https://www.tokenoptimize.dev/guides/llm-token-optimization-strategies">LLM Token Optimization Strategies: The Complete Guide for 2026</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出 sub-agent 是 token 消耗的主要来源，有用户反馈单个任务曾启动 7 个 sub-agent。一些人怀疑 Anthropic 故意增加 token 用量以推动订阅，另一些人则认为工具质量和往返次数比原始提示大小更重要。原作者承认了方法上的批评，并计划增加定性比较和可复现的输入输出。

**标签**: `#token-efficiency`, `#AI-coding-tools`, `#Claude-Code`, `#OpenCode`, `#developer-experience`

---

<a id="item-3"></a>
## [Terry Tao 谈用 LLM 编码代理构建应用](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

在一篇博客文章中，菲尔兹奖得主 Terry Tao 分享了他使用现代 LLM 编码代理（如 Claude Code）为研究论文构建交互式可视化的经验。他发现这些工具在非关键任务中出奇地有效，但建议对信任保持谨慎。 Tao 的认可为 LLM 编码代理作为软件开发实用工具（尤其是在低风险环境中）增添了可信度。这凸显了学术领域对 AI 辅助编程的日益接受，以及区分关键任务代码与辅助代码的重要性。 Tao 特别指出，这些代理可接受用于生成并非论文核心结果的辅助可视化。他警告用户不应盲目信任生成的代码，因为错误仍可能发生。

hackernews · subset · 7月12日 11:09 · [社区讨论](https://news.ycombinator.com/item?id=48880170)

**背景**: 基于 LLM 的编码代理是将大型语言模型封装在代理框架中的工具，可实现自主的代码生成、规划和执行。它们在软件开发的原型设计和低风险任务中变得流行。Terry Tao 是著名数学家、菲尔兹奖得主，他的博客经常探讨研究工具与技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/components-of-a-coding-agent">Components of A Coding Agent - by Sebastian Raschka, PhD</a></li>
<li><a href="https://arxiv.org/html/2508.00083v1">A Survey on Code Generation with LLM-based Agents</a></li>

</ul>
</details>

**社区讨论**: 评论中既有幽默也有认可，用户分享了自己的积极体验，例如为计算机科学课程创建可视化。其他人注意到一位菲尔兹奖得主使用让非专家也能编程的工具的讽刺之处，同时一致认为 LLM 编码代理对非关键任务有价值。

**标签**: `#LLMs`, `#coding agents`, `#software development`, `#AI-assisted programming`, `#Terry Tao`

---

<a id="item-4"></a>
## [开源 AI 面临 6 个月的生存考验](https://www.interconnects.ai/p/6-months-to-live-for-open-models) ⭐️ 8.0/10

一位知名 AI 研究员指出，开源 AI 模型正进入一个决定其长期生存能力的关键六个月的时期。 这可能重塑 AI 行业，决定开源模型是否能与主要实验室的专有系统竞争，从而影响可及性和创新。 这篇题为《6 个月后开源模型存活期》的文章发布在 interconnects.ai 上，作者是一位知名 AI 研究员，评分高达 8.0/10，表明分析深入有力。

rss · Interconnects · 7月12日 16:47

**背景**: 开源 AI 模型，如 Meta 和其他团体发布的模型，允许自由使用、修改和分发。它们在资金、计算资源和跟上专有系统快速进步方面面临挑战。

**标签**: `#open source`, `#AI`, `#viability`, `#models`, `#industry`

---

<a id="item-5"></a>
## [苹果起诉 OpenAI 窃取商业秘密](https://www.reddit.com/r/LocalLLaMA/comments/1uus189/apple_sues_openai_alleging_trade_secret_theft/) ⭐️ 8.0/10

苹果已对 OpenAI 提起诉讼，指控其在公司各个层面窃取商业秘密。 这起诉讼可能为 AI 公司保护商业秘密确立先例，影响整个科技行业。 案件的具体指控和细节尚未公开，该消息尚未得到证实。

reddit · r/LocalLLaMA · /u/fallingdowndizzyvr · 7月12日 21:25

**背景**: 商业秘密盗窃涉及未经授权获取或披露机密商业信息。在 AI 行业，公司将其专有算法、训练数据和模型架构作为商业秘密保护。

**标签**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secret`, `#AI`

---

<a id="item-6"></a>
## [将 J-lens 应用于 Qwen3-8B 监控静默推理](https://www.reddit.com/r/LocalLLaMA/comments/1uugulk/anthropic_found_claude_reasoning_in_silence/) ⭐️ 8.0/10

作者将 Anthropic 的 Jacobian lens (J-lens)应用于开源模型 Qwen3-8B，捕捉到模型在工具调用前从 JSON 格式漂移到自然语言散文的静默推理漂移。 这项工作展示了 Anthropic 的 J-space 研究在开源权重模型上的实际应用，实现了智能体监控和安全护栏，增强了基于 LLM 的系统的安全性和可靠性。 J-lens 被本地部署在 Qwen3-8B 上，用于检测工具调用前的散文漂移，并将恢复数据蒸馏为 LoRA 权重进行微调。

reddit · r/LocalLLaMA · /u/Murky-Sign37 · 7月12日 14:22

**背景**: Anthropic 的研究发现 Claude 中有一个隐藏的内部工作空间称为 J-space，其中发生静默推理，但不体现在可见文本中。Jacobian lens 是一种可解释性工具，通过计算内部激活对模型下一词元概率的线性化影响，使研究人员能够探测这个静默空间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/global-workspace">A global workspace in language models \ Anthropic</a></li>
<li><a href="https://github.com/anthropics/jacobian-lens">GitHub - anthropics/jacobian-lens: Companion code for the global workspace interpretability paper · GitHub</a></li>
<li><a href="https://explainx.ai/blog/anthropic-j-space-global-workspace-claude-interpretability-2026">Anthropic's J-Space: A Global Workspace Inside Claude — Silent ...</a></li>

</ul>
</details>

**标签**: `#LLM interpretability`, `#J-space`, `#Qwen3`, `#AI safety`, `#agent monitoring`

---

<a id="item-7"></a>
## [小米悄然在 Hugging Face 发布 MiMo-V2.5-DFlash](https://www.reddit.com/r/LocalLLaMA/comments/1uu8d1v/xiaomi_quietly_uploaded_mimov25dflash_official/) ⭐️ 8.0/10

此次发布带来了一款大型开源 LLM，并采用了创新的 DFlash 优化技术，能够在消费级硬件上可能将推理速度提升一倍，从而使其更易于本地部署和研究。 该模型包含一个专门的 dflash 目录和独立的 MTP（多令牌预测）头，不过 MTP 头尚未兼容 llama.cpp，而 DFlash 可能立即可用。

reddit · r/LocalLLaMA · /u/nasone32 · 7月12日 07:11

**背景**: DFlash 是一种用于推测解码的块扩散方法，它并行生成整个令牌块，在某些 GPU 上可实现高达 6 倍的加速。GGUF 格式用于高效的量化和本地推理。多令牌预测（MTP）是另一种同时预测多个未来令牌的技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/boost-inference-performance-up-to-15x-on-nvidia-blackwell-using-dflash-speculative-decoding/">Boost Inference Performance up to 15x on NVIDIA Blackwell Using DFlash Speculative Decoding | NVIDIA Technical Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/GGUF">GGUF - Wikipedia</a></li>
<li><a href="https://sebastianraschka.com/llm-architecture-gallery/mtp/">Multi-Token Prediction (MTP) | Sebastian Raschka, PhD</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区对 DFlash 可能带来的速度翻倍感到兴奋，用户们正在讨论 GGUF 转换以及独立的 MTP 头。一些人指出 MTP 在 llama.cpp 中尚无法使用，但推测 DFlash 可以正常工作。

**标签**: `#LLM`, `#open-source`, `#Hugging Face`, `#inference optimization`, `#Xiaomi`

---

<a id="item-8"></a>
## [三行代码修复 llama.cpp 中 Tesla P100 的 fp16 精度问题](https://www.reddit.com/r/LocalLLaMA/comments/1uu6p9o/your_80_tesla_p100_has_been_doing_silently_noisy/) ⭐️ 8.0/10

llama.cpp 中的一个三行补丁修正了 CUDA 标志，该标志错误地在 Tesla P100（sm_60）GPU 上启用了快速 fp16 运算，导致无声的精度损失。该修复将现有的 sm_61 豁免扩大到 sm_60，恢复了计算精度。 此修复显著提高了 Tesla P100 用户的推理精度和性能，使这些售价 80 美元的 GPU 在大模型推理中更具竞争力。同时，它也凸显了在开源项目中验证硬件特定标志的重要性。 应用补丁后，中位 KL 散度从 0.0023 降至 0.000001（提升了 2300 倍），最高 token 一致率从 96.5% 升至 99.9%。解码性能反而提升了约 1.4%，且预填速度不受影响。

reddit · r/LocalLLaMA · /u/apollo_mg · 7月12日 05:41

**背景**: llama.cpp 是一个开源库，用于在各种硬件上本地运行大型语言模型。Tesla P100 是一款采用 Pascal 架构的 GPU，具有快速的 fp16 硬件，但之前被错误地与其他 Pascal 显卡（如 GTX 1080 和 P40）区别对待。该修复已合并到 turboquant 分支，并向 llama.cpp 主仓库提交了拉取请求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>
<li><a href="https://www.techpowerup.com/gpu-specs/tesla-p100-pcie-16-gb.c2888">NVIDIA Tesla P100 PCIe 16 GB Specs | TechPowerUp GPU Database</a></li>
<li><a href="https://images.nvidia.com/content/tesla/pdf/nvidia-tesla-p100-PCIe-datasheet.pdf">Data Sheet: Tesla P100 - Nvidia</a></li>

</ul>
</details>

**社区讨论**: Reddit 上的讨论技术性很强且反响积极，社区成员验证了修复方案并赞赏详细的基准测试。作者提到，该 bug 是通过运行 Fable 5 的智能体循环发现的。

**标签**: `#llama.cpp`, `#GPU optimization`, `#Tesla P100`, `#fp16`, `#LLM inference`

---

<a id="item-9"></a>
## [Voodoo Quant 声称比 Unsloth Dynamic 2.0 KLD 提升 95%](https://www.reddit.com/r/LocalLLaMA/comments/1uua3jd/voodoo_quant_beats_unsloth_dynamic_20_kld_by_95/) ⭐️ 8.0/10

一种名为 Voodoo Quant 的新型量化技术发布，声称在 Qwen3.5 0.8B 和 2B 模型上，比 Unsloth Dynamic 2.0 的 Kullback-Leibler 散度（KLD）提升了 95%。 这可能创下量化效率的新标杆，使更大模型能在更小硬件上运行而无显著精度损失，有利于大语言模型的部署和可及性。 Voodoo Quant 对每个张量单独优化，而非像 Unsloth Dynamic 那样按块优化，且在“2 bit”等激进量化级别上特别有效。该技术在 Torch 和 Llama.cpp 中均表现出众，而 Unsloth 则过拟合于 Llama.cpp，在 Torch 中表现较差。

reddit · r/LocalLLaMA · /u/1ncehost · 7月12日 08:52

**背景**: 量化通过降低模型精度（例如从 16 位降至 4 位）来缩小体积并加快推理速度。Kullback-Leibler 散度（KLD）衡量量化导致的信息损失，越低越好。Qwen3.5 是阿里巴巴推出的一系列开源大语言模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://voodooquant.com/">Voodoo Quant</a></li>
<li><a href="https://unsloth.ai/docs/basics/unsloth-dynamic-2.0-ggufs">Unsloth Dynamic 2.0 GGUFs | Unsloth Documentation</a></li>

</ul>
</details>

**标签**: `#quantization`, `#model optimization`, `#Qwen`, `#efficiency`, `#mixed precision`

---

<a id="item-10"></a>
## [消息称 DeepSeek 正研发自有 AI 芯片](https://www.reddit.com/r/LocalLLaMA/comments/1uu15mz/chinas_deepseek_developing_its_own_ai_chip/) ⭐️ 8.0/10

据消息人士透露，中国人工智能公司 DeepSeek 正在开发自有 AI 芯片。此举有望减少对外国供应商（如英伟达）的依赖。 如果成功，DeepSeek 自研芯片可能颠覆 AI 硬件市场，挑战英伟达的主导地位，并符合中国半导体自主化的战略方向。该芯片还可能进一步降低 DeepSeek 本就高效模型的成本。 该芯片仍处于早期开发阶段，尚未公布发布时间表。此前由于出口限制，DeepSeek 使用性能较弱的 AI 芯片训练了其 R1 模型，从而高效利用了受限制的硬件。

reddit · r/LocalLLaMA · /u/TheRealMasonMac · 7月12日 01:04

**背景**: DeepSeek 是一家成立于 2023 年的中国人工智能公司，以其低成本、开源权重的大语言模型（如 DeepSeek-R1）而闻名。由于美国出口管制，DeepSeek 使用更少且性能较低的芯片进行模型训练。开发自有芯片将使 DeepSeek 进一步优化软硬件协同设计，并减少对英伟达高端 GPU 的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://www.bbc.com/news/articles/c5yv5976z9po">What is DeepSeek - and why is everyone talking about it?</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AI chips`, `#China`, `#semiconductors`, `#hardware`

---

<a id="item-11"></a>
## [RedHook 恶意软件滥用无线 ADB 获取 Shell 访问权限](https://www.bleepingcomputer.com/news/security/redhook-android-malware-now-uses-wireless-adb-for-shell-access/) ⭐️ 7.0/10

RedHook 安卓恶意软件现在利用安卓无线调试（Wireless ADB）功能，无需电脑或 USB 连接即可获取 Shell 级权限。 这种对合法开发者工具的新颖滥用，使恶意软件能够静默获取更高权限，增加检测难度，并扩展其在定向攻击中的能力。 该恶意软件通过无线 ADB 自主获取 UID 2000 的 Shell 访问权限，无需配对的电脑，并已在针对越南和印尼的攻击活动中被观察到。

rss · BleepingComputer · 7月12日 14:27

**背景**: 无线 ADB 是 Android 11 引入的开发者功能，允许通过 Wi-Fi 进行调试而无需 USB 线。RedHook 是一种于 2025 年 7 月首次被识别的银行木马，其最新变种滥用该功能获取系统级权限，用于窃取凭证和远程控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.androidpolice.com/use-wireless-adb-android-phone/">How to use wireless ADB on your Android phone A Complete Guide to Android ADB Wireless Debugging How to Enable and Use Wireless ADB on Your Android Phone How to Enable and Use Wireless ADB on Your Android Phone Android Debug Bridge (adb) | Android Studio | Android Developers Complete guide to wireless ADB on Android 11 or higher How to Set Up ADB Over Wireless Without USB Cable at All for ...</a></li>
<li><a href="https://www.group-ib.com/blog/redhook-android-rat-upgraded/">RedHook Returns with a Dangerous Upgrade | Group-IB Blog</a></li>

</ul>
</details>

**标签**: `#Android`, `#Security`, `#Malware`, `#Wireless ADB`

---