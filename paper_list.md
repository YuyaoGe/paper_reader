## 2026年2月19日

- **CADEvolve: Creating Realistic CAD via Program Evolution** `[微调]` `[VLM]` — [2602.16317](https://arxiv.org/abs/2602.16317) | [GitHub](https://github.com/zhemdi/CADEvolve)
  > CADEvolve 提出了一种基于演化的流水线，用于生成工业级复杂 CAD 程序。现有公开 CAD 数据集以简单草图拉伸序列为主，缺乏复杂操作与设计意图，严重限制了模型微调效果。本文从简单基元出发，借助 VLM 引导的编辑与几何验证，迭代演化出约 8000 个复杂 CadQuery 参数化生成器；经过多阶段后处理与增强，最终构建出含 130 万条脚本的统一数据集，并配以多视角渲染图像。在此数据集上微调的 VLM 在 Image2CAD 任务上的 DeepCAD、Fusion 360 和 MCB 三个评测集上均取得最优结果。代码、数据集与模型检查点均已开源。

- **Reinforced Fast Weights with Next-Sequence Prediction** `[RL]` `[长文本]` — [2602.16704](https://arxiv.org/abs/2602.16704) | [GitHub](https://github.com/princetonvisualai/ReFINE)
  > 快速权重架构（如 LaCT、DeltaNet）在长上下文建模中具有恒定内存优势，但受限于下一词预测（NTP）训练范式——NTP 仅优化单词预测，忽视多词语义连贯性，导致快速权重模型难以捕获长程依赖。本文提出 ReFINE，通过强化学习在下一序列预测（NSP）目标下训练快速权重模型：基于预测熵选取信息量大的 token 位置，生成多 token 展开，分配自监督序列级奖励，并用 GRPO 进行优化。ReFINE 适用于预训练模型的中期训练、后训练和测试时训练三个阶段。在 LaCT-760M 和 DeltaNet-1.3B 上的实验表明，ReFINE 在 NIAH 检索、长上下文问答及 LongBench 多项任务上均持续超过监督微调基线。

- **MMA: Multimodal Memory Agent** `[VLM]` `[MeM]` `[无需训练]` — [2602.16493](https://arxiv.org/abs/2602.16493) | [GitHub](https://github.com/AIGeeksGroup/MMA)
  > 长时多模态智能体依赖外部记忆，但基于相似度的检索常召回过时、低可信度或冲突条目，导致过度自信错误。本文提出 MMA（多模态记忆智能体），为每条检索到的记忆动态计算可信度分数，综合来源可信度、时间衰减与冲突感知网络共识，据此重新加权证据并在支持不足时主动弃权。同时引入 MMA-Bench，通过可编程方式生成含受控可信度与视觉-文本矛盾的信念动态评测集，并揭示了「视觉安慰剂效应」。实验表明，在 FEVER 上 MMA 保持准确率同时降低方差 35.2%；在 MMA-Bench 视觉模式下达到 41.18% Type-B 准确率，而基线崩溃至 0%。

- **Visual Memory Injection Attacks for Multi-Turn Conversations** `[VLM]` `[长文本]` — [2602.15927](https://arxiv.org/abs/2602.15927) | [GitHub](https://github.com/chs20/visual-memory-injection)
  > 本文研究大视觉语言模型（LVLM）在长上下文多轮对话中的安全漏洞。攻击者将篡改图像上传至网络，用户下载后输入 LVLM。所提出的视觉记忆注入（VMI）攻击具有隐蔽性：在普通 prompt 下模型正常作答，但一旦用户给出触发性 prompt，模型将输出预设目标消息（如广告植入或政治诱导）。与以往单轮攻击不同，VMI 在经过漫长多轮对话后仍然有效。实验在多个开源权重 LVLM 上验证了攻击的高成功率，并提供了不同上下文长度下的定量分析，表明基于扰动图像的大规模用户操纵是可行的，呼吁提升 LVLM 对此类攻击的鲁棒性。

- **Efficient Text-Guided Convolutional Adapter for the Diffusion Model** `[微调]` `[无需训练]` — [2602.14514](https://arxiv.org/abs/2602.14514) | [GitHub](https://github.com/arya-domain/Nexus-Adapters)
  > 本文提出 Nexus Adapters，用于扩散模型框架的文本引导高效适配器，旨在解决结构保持条件生成（SPCG）中现有方法参数量大、对输入 prompt 不感知的问题。Nexus 包含两种变体：Nexus Prime 和 Nexus Slim。每个 Nexus Block 引入交叉注意力机制实现丰富的多模态条件融合，使适配器同时理解文本 prompt 与结构输入（如草图、深度图）。Nexus Prime 仅增加 800 万参数即显著提升生成质量，Nexus Slim 参数比 T2I-Adapter 少 1800 万却仍达到最优水平。论文在 WACV 2026 上发表，代码已开源。

- **Uncertainty-Aware Vision-Language Segmentation for Medical Imaging** `[VLM]` `[微调]` — [2602.14498](https://arxiv.org/abs/2602.14498) | [GitHub](https://github.com/arya-domain/UA-VLS)
  > 本文提出了一种不确定性感知的多模态分割框架，融合放射影像与临床文本进行精准医学诊断。核心贡献包括：（1）模态解码注意力块（MoDAB）结合轻量级状态空间混合器（SSMix），实现高效跨模态融合与长程依赖建模；（2）谱熵不确定性损失（SEU Loss），在统一目标中同时捕获空间重叠、频谱一致性和预测不确定性。在 QATA-COVID19、MosMed++ 和 Kvasir-SEG 三个公开医学数据集上的大量实验表明，该方法在实现优越分割性能的同时计算效率显著高于现有最优方案，论文发表于 WACV 2026。


## 2026年2月20日

- **2Mamba2Furious: Linear in Complexity, Competitive in Accuracy** `[长文本]` — [2602.17363](https://arxiv.org/abs/2602.17363) | [GitHub](https://github.com/gmongaras/2Mamba2Furious)
  > 本文针对线性注意力与 softmax 注意力之间的精度差距问题，对 Mamba-2 进行深入分析与改造。作者首先将 Mamba-2 简化至最核心组件，得到 Mamba-2S，随后通过改进 A-mask 并提升隐状态阶数，提出 2Mamba 方法。实验表明，2Mamba 在精度上接近 softmax 注意力，同时在长上下文场景下保持显著更低的显存占用。此外，作者还探索了可使线性注意力超越 softmax 精度的额外设计要素，并在 NIAH 等长文本记忆任务上取得了与 softmax 相当的表现。

- **Mobile-Agent-v3.5: Multi-platform Fundamental GUI Agents** `[VLM]` `[微调]` — [2602.16855](https://arxiv.org/abs/2602.16855) | [GitHub](https://github.com/X-PLUG/MobileAgent)
  > 本文介绍 GUI-Owl-1.5，一套覆盖桌面、移动、浏览器等多平台的原生 GUI 智能体模型系列，提供 2B/4B/8B/32B/235B 多尺寸的 instruct 与 thinking 变体，支持云边协同与实时交互。GUI-Owl-1.5 在 20+ GUI 基准测试中达到开源模型最优：OSWorld 56.5、AndroidWorld 71.6、WebArena 48.4；在 grounding 任务上同样领先。通过 Mobile-Agent-v3.5 框架与 GUI-Owl-1.5 模型的结合，系统实现了跨平台基础 GUI 自动化能力。

- **Calibrate-Then-Act: Cost-Aware Exploration in LLM Agents** `[RL]` — [2602.16699](https://arxiv.org/abs/2602.16699) | [GitHub](https://github.com/Wenwen-D/env-explorer)
  > 本文研究 LLM 智能体在序列决策场景中如何平衡探索代价与不确定性。作者将信息检索和编程等任务形式化为带先验的不确定性下序列决策问题，提出 Calibrate-Then-Act（CTA）框架，通过显式地向 LLM 传递代价-不确定性上下文，引导其做出更优的探索决策。实验在信息寻求 QA 和简化编程任务上验证了 CTA 的有效性，且该改进在 RL 训练后仍然保持。结果表明，显式的代价收益权衡能帮助智能体发现更优的决策策略。

- **On the Mechanism and Dynamics of Modular Addition: Fourier Features, Lottery Ticket, and Grokking** — [2602.16849](https://arxiv.org/abs/2602.16849) | [GitHub](https://github.com/Y-Agent/modular-addition-feature-learning)
  > 本文对两层神经网络学习模块化加法任务的机制和训练动态进行全面分析，提供完整的机制解释与理论推导。研究发现：每个神经元独立学习单频余弦 Fourier 特征（Fourier Feature Learning）；初始化中相位对齐最优的频率通过赢者通吃竞争获胜（Lottery Ticket Dynamics）；在部分数据加权衰减训练下，网络经历「记忆→稀疏化→清理」三阶段后突然泛化（Grokking）。作者还给出了多样化条件的形式化证明，解释了单频特征如何组合为全局解。

- **ArXiv-to-Model: A Practical Study of Scientific LM Training** `[微调]` — [2602.17288](https://arxiv.org/abs/2602.17288) | [GitHub](https://github.com/kitefishai/KiteFish-A1-1.5B-Math)
  > 本文详细记录了从原始 arXiv LaTeX 源码从零训练 1.36B 参数科学语言模型（Minnow-Math-1.5B）的完整流程，覆盖元数据过滤、.tar.gz 压缩包解析、多文件 LaTeX 解析、去重、领域自适应分词器训练（102k 词表）及模型训练全链路。训练使用 2×A100 80GB GPU，处理 200GB 语料，总计 52.18B 预训练 token。模型在持留科学语料上验证困惑度约 4.2，展现出对科学写作风格与 LaTeX 结构的强烈建模能力，为受限算力下领域专用语言模型训练提供了实践参考。

- **Modeling Distinct Human Interaction in Web Agents** — [2602.17588](https://arxiv.org/abs/2602.17588) | [GitHub](https://github.com/oaishi/PlowPilot)
  > 本文研究自主 Web 智能体执行任务过程中人类干预行为的建模问题。作者收集了 CowCorpus 数据集，记录真实用户在 Web 任务执行中的干预时机与类型，并将干预建模为独立任务——预测何时以及为何需要人类介入。基于此，提出 PlowPilot 浏览器扩展系统，结合决策模型与动作执行模型协作完成 Web 任务。实验表明，融入人类干预建模后，智能体在关键决策节点的行为更准确，不必要的确认请求大幅减少，协作效率显著提升。

- **References Improve LLM Alignment in Non-Verifiable Domains** `[RL]` `[微调]` — [2602.16802](https://arxiv.org/abs/2602.16802) | [GitHub](https://github.com/yale-nlp/RLRR)
  > 本文针对 RLVR 无法直接应用于无法验证的领域（如 LLM 对齐）这一问题，探究参考输出引导的 LLM 评估器是否能充当「软验证器」。研究表明，使用前沿模型参考输出可大幅提升弱模型评估器的准确性；高质量人类参考输出也能增强强模型评估器。基于改进后的评估器，作者提出参考引导自我改进方法，通过 DPO 训练实现对齐。在 AlpacaEval/Arena-Hard 上，Llama-3-8B 达到 73.1%/58.7%，Qwen2.5-7B 达到 70.0%/74.1%，分别比 SFT 蒸馏平均提升 +20.2/+17.1 分，比无参考自我改进提升 +5.3/+3.6 分。

- **CrispEdit: Low-Curvature Projections for Scalable Non-Destructive LLM Editing** `[无需训练]` — [2602.15823](https://arxiv.org/abs/2602.15823) | [GitHub](https://github.com/zarifikram/CrispEdit)
  > 本文提出 CrispEdit，一种可扩展的二阶 LLM 知识编辑算法，将能力保留明确建模为约束条件。核心思想是将编辑方向投影至能力损失曲率最低的子空间，从而在更新目标知识的同时避免对通用能力的破坏。CrispEdit 统一并推广了多种现有编辑方法，支持千级别的连续知识编辑。实验表明，在 WILD 自回归评估中，CrispEdit 在目标编辑精度上表现突出，同时保持原有能力，相比 AlphaEdit 和 MEMIT 实现超过 100 倍的速度提升。


## 2026年2月23日

- **VESPO: Variational Sequence-Level Soft Policy Optimization for Stable Off-Policy LLM Training** `[RL]` — [2602.10693](https://arxiv.org/abs/2602.10693) | [GitHub](https://github.com/FloyedShen/VESPO)
  > VESPO 针对 LLM 强化学习训练中普遍存在的 off-policy 问题——策略滞后（staleness）、异步训练以及训练/推理引擎不匹配——提出了基于变分公式的方差缩减方案。核心贡献是推导出一个作用于序列级重要性权重的闭合式重塑核（reshaping kernel），无需 token 级截断或长度归一化。实验表明，VESPO 在滞后倍率高达 64× 及完全异步训练下仍保持稳定，在数学推理基准上对稠密模型和 MoE 模型均取得一致性提升，支持在 Qwen3-30B-A3B-Base 上进行 fully async 训练而不发散。

- **Spanning the Visual Analogy Space with a Weight Basis of LoRAs** `[微调]` `[无需训练]` — [2602.15727](https://arxiv.org/abs/2602.15727) | [GitHub](https://github.com/NVlabs/LoRWeB)
  > LoRWeB（LoRA Weight Basis）解决视觉类比学习问题：给定图像三元组 {a, a', b}，生成 b' 使得 a:a'::b:b'。现有方法用单个 LoRA 模块捕捉视觉变换空间，泛化能力有限。本文提出由一组可学习 LoRA 模块构成的「变换基」，以及一个轻量编码器，在推理时根据类比输入动态组合这些基，即在「LoRA 空间」中选择一个点。方法在推理时特化、无需对每个新任务重新训练，在未见变换上的泛化能力显著优于现有 SOTA，代码和数据均已开源。

- **DeepVision-103K: A Visually Diverse, Broad-Coverage, and Verifiable Mathematical Dataset for Multimodal Reasoning** `[RL]` `[VLM]` — [2602.16742](https://arxiv.org/abs/2602.16742) | [GitHub](https://github.com/SKYLENAGE-AI/DeepVision-103K)
  > DeepVision-103K 是一个面向多模态推理 RLVR（强化学习可验证奖励）训练的大规模数学数据集，涵盖平面几何、立体几何、解析图、数据图表、示意图等丰富视觉元素，以及代数、概率统计等 K12 数学主题。每条样本含可验证唯一答案，支持规则奖励。经三阶段流水线（有效性过滤、难度过滤、Gemini-3-Flash 正确性验证）构建。在 DeepVision 上训练的 Qwen3-VL-8B 在多模态数学及通用推理基准上超越基线，平均准确率从 66.50% 提升至 70.15%，且推理 token 消耗更高效。

- **Sink-Aware Pruning for Diffusion Language Models** `[无需训练]` — [2602.17664](https://arxiv.org/abs/2602.17664) | [GitHub](https://github.com/VILA-Lab/Sink-Aware-Pruning)
  > 扩散语言模型（DLMs）的注意力 sink 与自回归模型不同：位置不固定、跨去噪时间步高度不稳定，因此直接沿用「保留 sink」的 AR 剪枝启发式会导致次优结果。本文提出 Sink-Aware Pruning，通过测量 sink token 在完整去噪轨迹上的位置方差来识别不稳定 sink，并将其剪掉以减少冗余全局注意力。在 LLaDA、Dream 7B 等模型上，于 50% 稀疏度下一致超越 Wanda 和 SparseGPT 基线，在 8 个基准上平均准确率提升明显，压缩比越高收益越显著。

- **Adam Improves Muon: Adaptive Moment Estimation with Orthogonalized Momentum** `[微调]` — [2602.17080](https://arxiv.org/abs/2602.17080) | [GitHub](https://github.com/minxin-zhg/namo)
  > NAMO（NAMO/NAMO-D）将 Muon 优化器的正交化动量机制与 Adam 的自适应学习率结合：对一阶动量进行 Nesterov 正交化处理后，再应用逐元素自适应二阶矩缩放。这在理论上弥合了 Muon 缺乏自适应性的局限。实验在 nanoGPT 及多种语言模型预训练任务上验证，NAMO 收敛速度和最终困惑度均优于 Muon 和 Adam，尤其在大批量和高学习率场景下稳定性更优。

- **Avey-B** `[长文本]` — [2602.15814](https://arxiv.org/abs/2602.15814) | [GitHub](https://github.com/rimads/avey-b)
  > Avey-B 将 Avey（一种无注意力自回归架构）重构为 encoder-only 双向编码器，面向工业级紧凑 NLP 应用。核心创新包括：解耦静态与动态参数化、面向稳定性的归一化设计、以及神经压缩技术。与四种主流 Transformer 编码器（BERT 系列）对比，在 token 分类和信息检索基准上持续胜出，同时对长上下文的扩展效率更高。论文完整提供了 MLM 预训练代码、评测框架及检查点，已在 ICLR 2026 发表。

- **Rubrics as an Attack Surface: Stealthy Preference Drift in LLM Judges** `[RL]` — [2602.13576](https://arxiv.org/abs/2602.13576) | [GitHub](https://github.com/ZDCSlab/Rubrics-as-an-Attack-Surface)
  > 本文研究 LLM-as-Judge 评估流程中的「评分标准诱导偏好漂移」（RIPD）：攻击者通过微小修改评分 rubric，在基准域上保持验证通过，同时在目标部署域上引发系统性方向偏差，且难以用标准指标检测。实验利用基于种群的进化搜索寻找满足约束的 rubric 变体，并证明该偏差可通过下游后训练传播，导致持久性策略错对齐。涵盖 UltraFeedback、ChatbotArena、PKU-SafeRLHF 等五个人类偏好数据集，代码和数据集已开源。

- **Whom to Query for What: Adaptive Group Elicitation via Multi-Turn LLM Interactions** — [2602.14279](https://arxiv.org/abs/2602.14279) | [GitHub](https://github.com/ZDCSlab/Group-Adaptive-Elicitation)
  > 自适应群体意见收集框架 GAE，在有限查询和参与预算下，同时自适应选择「问哪个问题」和「问哪个被试」。方法结合：①基于 LLM 期望信息增益（EIG）的问题评分；②异构图神经网络（HGNN）聚合已有回答与被试属性，对缺失回答进行插补并指导被试选择。在 CES、OpinionQA、Twin-2k 三个真实调查数据集上，相比固定被试池方法显著提升群体级响应预测，在 10% 预算下 CES 相对增益超 12%。


## 2026年2月24日

- **Learning Cross-View Object Correspondence via Cycle-Consistent Mask Prediction** `[无需训练]` — [2602.18996](https://arxiv.org/abs/2602.18996) | [GitHub](https://github.com/shannany0606/CCMP)
  > 研究跨视角目标级视觉对应任务，专注于以自我为中心（egocentric）与以外部为中心（exocentric）视角间的相互转换场景。提出基于条件二值分割的简洁框架：将目标查询掩膜编码为隐变量表示，引导在目标视频中定位对应目标。为学习鲁棒的视角无关表示，引入循环一致性训练目标——将目标视角预测掩膜投影回源视角以重建原始查询掩膜，无需真值标注即可提供强自监督信号，并支持推理阶段的测试时训练（TTT）。在Ego-Exo4D和HANDAL-X基准上达到SOTA性能，CVPR 2026高分接收（评分554）。方法简洁高效，展示了简单设计在困难任务上的强大泛化能力。

- **Mobile-O: Unified Multimodal Understanding and Generation on Mobile Device** `[VLM]` `[微调]` — [2602.20161](https://arxiv.org/abs/2602.20161) | [GitHub](https://github.com/Amshaker/Mobile-O)
  > 提出Mobile-O，一个紧凑高效的视觉-语言-扩散统一模型，可完全在移动设备本地运行，同时支持多模态理解（VQA、OCR、推理）和图像生成与编辑。核心架构包含三部分：基于FastVLM的轻量视觉语言模型骨干、基于SANA的轻量DiT扩散解码器，以及创新性的Mobile Conditioning Projector（MCP，仅约2.4M参数）将两者桥接。通过预训练（9M图文对）、SFT（105K对）和统一后训练（105K四元组）三阶段训练优化至移动端实用水平。在iPhone 15/16/17 Pro上实测：图像生成约3-4秒、视觉理解约0.4秒、内存占用小于2GB。已完整开源训练评测代码、推理脚本及iOS应用。

- **Large Causal Models for Temporal Causal Discovery** `[无需训练]` — [2602.18662](https://arxiv.org/abs/2602.18662) | [GitHub](https://github.com/kougioulis/LCM-paper)
  > 提出大型因果模型（LCMs）框架用于时序因果发现，颠覆传统「每数据集单独拟合一个模型」范式。核心贡献在于将多样合成生成器与真实时序数据集结合进行大规模多域预训练，使单一模型具备强跨域迁移能力。在合成、半合成及真实基准上的广泛实验表明，LCMs可有效扩展至更多变量数和更深架构，在分布外（OOD）场景相比经典和神经基线取得有竞争力或更优准确率，并支持单次前向推理（无需为新数据集重新训练）。提供2.5M至24M参数规模的预训练模型，代码、Jupyter实验笔记本及预训练检查点完整开源。

## 2026年2月25日

- **PyVision-RL: Forging Open Agentic Vision Models via RL** `[RL]` `[VLM]` — [2602.20739](https://arxiv.org/abs/2602.20739) | [GitHub](https://github.com/agents-x-project/PyVision-RL)
  > PyVision-RL 提出了一个开放权重多模态模型的强化学习训练框架，解决了代理型多模态模型中的「交互坍塌」问题——模型在 RL 微调后倾向于减少工具调用和多轮推理。核心方法包括过采样-过滤-排序（oversampling-filtering-ranking）rollout 策略与累积工具奖励机制，从而防止崩塌并激励多轮工具使用。基于统一训练管线，分别开发了 PyVision-Image（图像理解）和 PyVision-Video（视频推理），后者采用按需上下文构建，在推理时选择性采样任务相关帧，大幅降低视觉 token 消耗。实验表明，在多模态推理、视觉搜索和代理推理任务上均取得领先性能，验证了持续交互和按需视觉处理对可扩展多模态代理的关键作用。

- **Multi-Vector Index Compression in Any Modality** `[无需训练]` — [2602.21202](https://arxiv.org/abs/2602.21202) | [GitHub](https://github.com/hanxiangqin/omni-col-press)
  > 本文研究跨模态的多向量检索效率问题。Late interaction（延迟交互）在文本、图像、视觉文档和视频检索中已成主流范式，但其计算和存储开销随文档长度线性增长，在富媒体语料库中代价高昂。本文提出四种 query-agnostic 的多向量文档表示压缩方法：序列缩放、记忆 token、层次池化以及新颖的注意力引导聚类（AGC）。AGC 通过注意力机制识别文档中语义最突出的区域作为聚类中心，加权聚合 token 表示。在 BEIR（文本）、ViDoRe（视觉文档）和 MSR-VTT/MultiVENT 2.0（视频）等检索任务上，AGC 始终优于其他参数化压缩方法，并在不同 index 大小配置下超越或持平未压缩全量索引。

- **TAPE: Tool-Guided Adaptive Planning and Constrained Execution in Language Model Agents** `[无需训练]` — [2602.19633](https://arxiv.org/abs/2602.19633) | [GitHub](https://github.com/UW-Madison-Lee-Lab/TAPE)
  > TAPE（工具引导自适应规划与约束执行）旨在解决 LM 智能体在严格可行性约束下单次错误导致不可恢复失败的问题。系统性分析发现，不完善规划与随机执行是主要失败原因。TAPE 通过将多个规划方案聚合为图并利用外部求解器寻找可行路径来增强规划能力；执行阶段采用约束解码降低采样噪声，当环境反馈偏离预期时自适应重新规划。在 Sokoban、ALFWorld、MuSiQue 和 GSM8K-Hard 上的实验表明，TAPE 一致优于现有框架：在困难设置下平均提升成功率 21.0 个百分点，对弱基础模型平均提升 20.0 个百分点，充分验证了图规划与约束执行的有效组合。

- **PETS: A Principled Framework Towards Optimal Trajectory Allocation for Efficient Test-Time Self-Consistency** `[无需训练]` — [2602.16745](https://arxiv.org/abs/2602.16745) | [GitHub](https://github.com/ZDCSlab/PETS)
  > PETS（原则化高效测试时自一致性）针对有限预算下的样本高效测试时推理问题，通过优化框架系统研究轨迹分配策略。核心贡献是引入「自一致率」——与无限预算多数投票的一致程度——作为新衡量指标，使样本高效分配具有理论依据。离线设置中将轨迹分配类比为众包问题，借助成熟众包理论推导理论保证和高效多数投票分配算法；在线流式设置中设计自适应算法，根据问题难度动态调整预算。在 GPQA 上，PETS 在离线设置下将采样预算降低高达 75%、在线设置下降低 55%，同时维持完美自一致率，验证了框架的实用性与理论严谨性。

- **One-step Language Modeling via Continuous Denoising** `[微调]` — [2602.16813](https://arxiv.org/abs/2602.16813) | [GitHub](https://github.com/david3684/flm)
  > 本文挑战「离散扩散是离散模态生成建模必要条件」这一广泛假设，提出基于流匹配连续去噪的语言模型 FLM。FLM 在 one-hot token 编码上执行欧几里得去噪，通过交叉熵目标预测干净数据进行训练，并引入简单的时间重参数化大幅提升训练稳定性和生成质量。通过将 FLM 蒸馏为关联流图，得到 FMLM，实现高质量少步生成。在 LM1B 和 OWT 语料上，FLM 达到与最先进离散扩散模型相当的生成质量；FMLM 单步生成质量超越同类模型 8 步的表现，全面优于近期少步语言模型，为加速流式语言建模铺平道路。

- **Communication-Inspired Tokenization for Structured Image Representations** `[无需训练]` `[VLM]` — [2602.20731](https://arxiv.org/abs/2602.20731) | [GitHub](https://github.com/Araachie/comit)
  > COMiT（通信启发式 Tokenization）受人类交流渐进式组合性质启发，提出学习结构化离散视觉 token 序列的框架。在固定 token 预算内，模型迭代观察局部图像块并循环更新离散表示，每步整合新视觉信息并精炼重组现有 token 序列，最终利用流匹配解码器重建完整图像，编解码均在单一 Transformer 中端到端训练。实验证明，语义对齐提供基础锚定，而注意力驱动的序列 Tokenization 是实现可解释对象中心 token 结构的关键，相较先前方法在组合泛化和关系推理上有显著提升。

- **TextPecker: Rewarding Structural Anomaly Quantification for Enhancing Visual Text Rendering** `[RL]` `[VLM]` — [2602.20903](https://arxiv.org/abs/2602.20903) | [GitHub](https://github.com/CIawevy/TextPecker)
  > 视觉文本渲染（VTR）是文本到图像生成的核心挑战，现有先进模型仍频繁出现扭曲、模糊、错位等结构性异常。本文发现主流 MLLM 和专业 OCR 模型对这些结构异常的感知能力严重不足，成为 VTR 评估和 RL 优化的关键瓶颈。TextPecker 提出即插即用的结构异常感知 RL 策略，构建了字符级结构异常标注识别数据集并开发笔划编辑合成引擎扩展结构错误覆盖范围，可与任意文本到图像生成器配合使用。CVPR 2026 录用；实验表明在充分优化的 Qwen-Image 上，中文文本渲染结构保真度平均提升 4%，语义对齐提升 8.7%，达到新 SOTA。

- **FlowPrefill: Decoupling Preemption from Prefill Scheduling Granularity to Mitigate Head-of-Line Blocking in LLM Serving** `[无需训练]` — [2602.16603](https://arxiv.org/abs/2602.16603) | [GitHub](https://github.com/HSIEHCHIACHI/FlowPrefill)
  > FlowPrefill 针对 LLM 推理服务中预填充（prefill）阶段的队头阻塞（HoL blocking）问题，提出将抢占粒度与调度频率解耦的 TTFT 吞吐量优化系统。核心创新包括：①算子级抢占（Operator-Level Preemption），利用算子边界实现细粒度执行中断，避免固定小分块带来的效率损失；②事件驱动调度（Event-Driven Scheduling），仅在请求到达或完成事件时触发调度决策，最小化控制平面开销。在真实生产负载（QwenTrace）上的评估表明，相比现有最先进系统，在满足异构 SLO 约束的同时，FlowPrefill 将最大有效吞吐量（goodput）提升高达 5.6 倍。


## 2026年2月26日

- **ARLArena: A Unified Framework for Stable Agentic Reinforcement Learning** `[RL]` — [2602.21534](https://arxiv.org/abs/2602.21534) | [GitHub](https://github.com/WillDreamer/ARL-Arena)
  > 智能体强化学习（ARL）在训练多步骤交互任务方面展现出潜力，但训练不稳定导致的崩溃问题制约了其扩展性。本文提出ARLArena，一个稳定的训练方案与系统性分析框架，在可控可复现的环境中研究训练稳定性。ARLArena构建了标准化测试平台，将策略梯度分解为四个核心设计维度并逐一评估。基于细粒度分析，论文提炼出统一视角并提出SAMPO——一种稳定的智能体策略优化方法，旨在消除ARL中的主要不稳定来源。在多样化智能体任务上，SAMPO实现了持续稳定的训练和强劲性能，为构建可扩展的智能体RL系统提供了重要基础。

- **GUI-Libra: Training Native GUI Agents to Reason and Act with Action-aware Supervision and Partially Verifiable RL** `[RL]` `[VLM]` `[微调]` — [2602.22190](https://arxiv.org/abs/2602.22190) | [GitHub](https://github.com/GUI-Libra/GUI-Libra)
  > 本文针对原生GUI智能体后训练的两大瓶颈：高质量动作对齐推理数据匮乏，以及忽视GUI交互独特约束的通用后训练流程。GUI-Libra提出GUI专属配方：81K精选推理数据集、通过token重加权平衡推理与直接动作监督的动作感知SFT，以及结合KL正则化与成功自适应负梯度缩放的保守RL。在AndroidWorld、Online-Mind2Web和WebArena-Lite-v2等线上离线基准上，GUI-Libra-4B和GUI-Libra-8B持续超越强基线原生GUI智能体，在多个设置下甚至超过专有系统，验证了专门化后训练流程的有效性。

- **From Statics to Dynamics: Physics-Aware Image Editing with Latent Transition Priors** `[VLM]` `[微调]` — [2602.21778](https://arxiv.org/abs/2602.21778) | [GitHub](https://github.com/liangbingzhao/PhysicEdit)
  > 基于指令的图像编辑在语义对齐上取得显著成功，但涉及折射、材料形变等复杂因果动力学时，现有模型难以生成物理合理的结果。作者将物理感知编辑重新表述为预测性物理状态转换，构建了大规模视频数据集PhysicTran38K（五大物理领域38K转换轨迹），并提出端到端框架PhysicEdit。该框架配备文本-视觉双重思考机制，将冻结的Qwen2.5-VL用于物理推理，结合可学习的转换查询为扩散主干提供时步自适应视觉引导。实验表明，PhysicEdit在物理真实性上比Qwen-Image-Edit提升5.9%，知识引导编辑提升10.1%，达到开源方法最优，且与领先闭源模型竞争。

- **VecGlypher: Unified Vector Glyph Generation with Language Models** `[微调]` — [2602.21461](https://arxiv.org/abs/2602.21461) | [GitHub](https://github.com/xk-huang/VecGlypher)
  > 矢量字形是数字排版的基本单元，但现有学习方法依赖精心策划的样例集和光栅转矢量后处理，限制了可访问性与可编辑性。VecGlypher提出单一多模态语言模型，可直接从文本描述或图像样例生成高保真矢量字形。给定风格提示、可选参考字形图像和目标字符，模型自回归地输出SVG路径token，无需光栅中间件，一次生成可编辑轮廓。训练方案包含：在39K Envato字体上的大规模续训以掌握SVG语法，以及在2.5K Google Fonts上的专家标注后训练以对齐语言与几何。实验显示VecGlypher在字形保真度和风格对齐上显著优于现有基线。

- **Revisiting Text Ranking in Deep Research** `[无需训练]` — [2602.21456](https://arxiv.org/abs/2602.21456) | [GitHub](https://github.com/ChuanMeng/text-ranking-in-deep-research)
  > 深度研究是通过大规模开放网络探索回答复杂查询的重要任务。现有工作使用黑箱搜索API，使得对搜索组件的系统分析受限。本文系统复现了IR文本排序方法在深度研究场景的表现，从检索单元（文档vs.段落）、流水线配置（检索器、重排序器及深度）和查询特征（智能体查询与训练查询的不匹配）三个维度评估。在固定语料库的BrowseComp-Plus数据集上，对2个开源智能体、5个检索器和3个重排序器进行实验。发现智能体查询倾向于网页搜索风格，偏好词汇、稀疏和多向量检索器；段落级检索更高效；重排序效果显著；将智能体查询转换为自然语言问题能有效弥合查询不匹配。

- **SeaCache: Spectral-Evolution-Aware Cache for Accelerating Diffusion Models** `[无需训练]` — [2602.18993](https://arxiv.org/abs/2602.18993) | [GitHub](https://github.com/jiwoogit/SeaCache)
  > 扩散模型的序列去噪过程导致推理速度缓慢。现有缓存加速方法基于相邻时间步的特征距离决定是否复用，但忽视了低频结构先出现、高频细节后精化的频谱演化规律。本文提出SeaCache，一种无需训练的基于频谱对齐表示的缓存调度方法。通过理论与实证分析，推导出频谱演化感知（SEA）滤波器，保留内容相关成分并抑制噪声。使用SEA滤波特征估计冗余，动态调度兼顾内容自适应与扩散模型内在频谱先验。在多种视觉生成模型上，SeaCache达到最先进的延迟-质量权衡，已被CVPR 2026接受。

- **NoLan: Mitigating Object Hallucinations in Large Vision-Language Models via Dynamic Suppression of Language Priors** `[VLM]` `[无需训练]` — [2602.22144](https://arxiv.org/abs/2602.22144) | [GitHub](https://github.com/lingfengren/NoLan)
  > 大型视觉语言模型（LVLM）的目标幻觉问题（输出图像中不存在的对象）是关键挑战。作者通过系统实验分析视觉编码器与语言解码器在幻觉生成中的作用，发现目标幻觉主要源于语言解码器的强先验。基于此，提出无需训练的框架NoLan（No-Language-Hallucination Decoding），通过对比多模态输入与纯文本输入的输出分布差异，动态抑制语言先验来精化输出分布。实验表明，NoLan在多种LVLM的不同任务上有效减少目标幻觉，例如在POPE上将LLaVA-1.5 7B和Qwen-VL 7B的准确率分别提升6.45和7.21。

- **Small Language Models for Privacy-Preserving Clinical Information Extraction in Low-Resource Languages** `[无需训练]` — [2602.21374](https://arxiv.org/abs/2602.21374) | [GitHub](https://github.com/mohammad-gh009/Small-language-models-on-clinical-data-extraction)
  > 本文在低资源语言（波斯语）临床信息提取任务上，对五款开源小语言模型（SLM，1B-8B参数）进行评测。采用两阶段流水线从1221份匿名波斯语姑息治疗转录本中提取13个二元临床特征，无需微调。Qwen2.5-7B-Instruct取得最佳综合表现（宏F1: 0.899，MCC: 0.797）。实验还发现，使用Aya-expanse-8B将波斯语翻译为英语后再提取，可提升召回率与完整性，但略微降低特异性。研究为资源匮乏语言中的隐私保护临床NLP提供了实用方案。

- **The Truthfulness Spectrum Hypothesis** — [2602.20273](https://arxiv.org/abs/2602.20273) | [GitHub](https://github.com/zfying/truth_spec)
  > 本文提出「真实性谱系假说」：不同泛化程度的真实方向在语言模型中共存，探针几何结构预测泛化性，后训练会重塑探针空间。研究构建了FLEED数据集（定义性、经验性、逻辑性、虚构性、伦理性真实）及奉承性说谎等新数据集；发现现有探针与奉承性说谎正交，甚至与反预期说谎负相关；提出Mahalanobis余弦相似度（R²=0.98）完美预测OOD泛化；后训练将奉承性说谎方向与其他说谎方向分离，解释了为何聊天模型比基础模型更容易奉承；提出Stratified INLP方法迭代提取高度领域通用与特异方向，域特异方向比通用方向更适合因果干预。

- **Functional Continuous Decomposition** — [2602.20857](https://arxiv.org/abs/2602.20857) | [GitHub](https://github.com/Tima-a/fcd)
  > 非平稳时序数据的分析需要对局部和全局模式的物理可解释洞察。传统平滑算法（B样条、Savitzky-Golay滤波、经验模式分解EMD）缺乏带连续性保证的参数优化能力。本文提出FCD（Functional Continuous Decomposition），一个基于JAX加速的参数化连续优化框架，支持对多种数学函数族进行优化，利用Levenberg-Marquardt优化实现C¹连续拟合，将原始时序分解为M个模式，捕获从短期到长期的不同时间尺度规律。FCD可应用于物理、医学、金融和机器学习领域，全分解1000点速度0.47秒，SRMSE均值0.735。以FCD特征增强CNN可使收敛速度提升16.8%，准确率提升2.5%。


## 2026年2月27日

- **From Blind Spots to Gains: Diagnostic-Driven Iterative Training for Large Multimodal Models** `[VLM]` `[微调]` `[RL]` — [2602.22859](https://arxiv.org/abs/2602.22859) | [GitHub](https://github.com/hongruijia/DPE)
  > 本文提出 DPE（诊断驱动渐进式进化），一种针对大型多模态模型（LMM）的螺旋式迭代训练范式。现有训练依赖静态数据和固定流程，难以诊断能力盲区或进行动态针对性强化。DPE 包含两个核心组件：（1）多智能体协同标注和质量控制大量未标注多模态数据，利用网络搜索和图像编辑工具生成多样化样本；（2）将失败归因于特定弱点，动态调整数据混合比例，并引导智能体生成针对弱点的训练数据。每轮迭代完成后重新诊断更新后的模型，驱动下一轮针对性改进。在 Qwen3-VL-8B 和 Qwen2.5-VL-7B 上的实验显示，DPE 在 11 个基准上取得持续稳定提升，验证了其作为开放任务分布下 LMM 持续训练可扩展范式的有效性。

- **OmniGAIA: Towards Native Omni-Modal AI Agents** `[VLM]` `[微调]` `[RL]` — [2602.22897](https://arxiv.org/abs/2602.22897) | [GitHub](https://github.com/RUC-NLPIR/OmniGAIA)
  > 本文提出 OmniGAIA——一个面向全模态智能体的综合评测框架，以及 OmniAtlas——一个原生全模态基础智能体。OmniGAIA 通过新颖的「全模态事件图」方法构建跨视觉、音频和语言的复杂多跳推理任务。OmniAtlas 在工具集成推理范式下，结合基于后见之明的树搜索策略和 OmniDPO 细粒度误差校正进行训练，有效提升了现有开源模型的工具使用能力。实验证明 OmniAtlas 在跨模态推理和多轮工具执行任务上达到先进水平，是迈向下一代原生全模态 AI 助手的重要一步。

- **Exploratory Memory-Augmented LLM Agent via Hybrid On- and Off-Policy Optimization** `[RL]` `[MeM]` — [2602.23008](https://arxiv.org/abs/2602.23008) | [GitHub](https://github.com/microsoft/agent-lightning)
  > 本文提出 EMPO²（探索性记忆增强混合策略优化），一种用于大语言模型智能体的混合强化学习框架。现有方法依赖预训练知识，在需要发现新状态的环境中表现不足。EMPO² 利用记忆机制支持探索，并将在线策略与离线策略更新相结合，使 LLM 在配备记忆时性能优越、同时在无记忆时保持鲁棒性。在 ScienceWorld 和 WebShop 上，相比 GRPO 分别取得 128.6% 和 11.3% 的提升。在分布外测试中，EMPO² 仅需少量带记忆的试验即可适应新任务，无需参数更新。

- **AgentDropoutV2: Optimizing Information Flow in Multi-Agent Systems via Test-Time Rectify-or-Reject Pruning** `[无需训练]` — [2602.23258](https://arxiv.org/abs/2602.23258) | [GitHub](https://github.com/TonySY2/AgentDropoutV2)
  > 本文提出 AgentDropoutV2，一种面向多智能体系统（MAS）的测试时「修正或拒绝」剪枝框架，无需重新训练即可动态优化信息流。该框架充当主动防火墙，拦截智能体输出并使用基于检索增强的修正器，通过失败驱动的指标池迭代纠错。无法修复的输出将被剪枝以阻止错误传播，同时通过回退策略维持系统完整性。在大量数学基准测试上，AgentDropoutV2 平均准确率提升 6.3 个百分点，并展现出强大的泛化能力，可根据任务难度动态调整修正力度。

- **MediX-R1: Open Ended Medical Reinforcement Learning** `[RL]` `[VLM]` `[微调]` — [2602.23363](https://arxiv.org/abs/2602.23363) | [GitHub](https://github.com/mbzuai-oryx/MediX-R1)
  > 本文提出 MediX-R1，一个面向医疗多模态大语言模型的开放式强化学习框架，支持自由文本形式的临床答案生成，突破了传统多选题格式限制。MediX-R1 采用基于组的强化学习（Group-Based RL）和复合奖励信号：基于 LLM 的语义准确性奖励、医疗嵌入语义奖励，以及格式和模态奖励。仅使用约 51K 条指令样本，MediX-R1 在文本和图文医疗基准上均优于强开源基线，在开放式临床任务上取得特别显著的提升，验证了开放式 RL 结合 LLM 评估在医疗推理中的实用价值。

- **General Agent Evaluation** `[无需训练]` — [2602.22953](https://arxiv.org/abs/2602.22953) | [GitHub](https://github.com/Exgentic/exgentic)
  > 本文将通用智能体评估确立为首要研究目标。现有智能体多为领域专用，且现有基准将任务信息以妨碍公平评估的方式编码，无法对通用智能体进行系统评测。本文提出通用智能体评估的概念原则、统一协议（Unified Protocol）以及实用框架 Exgentic。在六个环境中对五种主流智能体实现进行测评，建立了首个「开放通用智能体排行榜」。实验显示，通用智能体无需任何环境特定调整即可实现与专用智能体相当的性能，证明通用智能体跨环境泛化能力的可行性。

- **Accelerating Diffusion via Hybrid Data-Pipeline Parallelism Based on Conditional Guidance Scheduling** `[无需训练]` — [2602.21760](https://arxiv.org/abs/2602.21760) | [GitHub](https://github.com/kaist-dmlab/Hybridiff)
  > 本文提出一种混合并行框架，结合新颖的数据并行策略（条件分区）与最优流水线调度方法（自适应并行切换），以加速条件扩散模型推理。核心思路是将条件与无条件去噪路径作为新的数据分区视角，并根据两路径去噪差异自适应启用最优流水线并行。使用两块 NVIDIA RTX 3090 GPU，在 SDXL 和 SD3 上分别实现 2.31× 和 2.07× 的延迟降低，同时保持图像质量，验证了方法对 U-Net 和 DiT 架构的通用性，在高分辨率合成场景下优于现有方法。

- **MedCLIPSeg: Probabilistic Vision-Language Adaptation for Data-Efficient and Generalizable Medical Image Segmentation** `[VLM]` `[微调]` — [2602.20423](https://arxiv.org/abs/2602.20423) | [GitHub](https://github.com/HealthX-Lab/MedCLIPSeg)
  > 本文提出 MedCLIPSeg，一个将 CLIP 适配至医学图像分割的新框架，解决标注稀缺、解剖特征模糊和域偏移等挑战。该方法通过概率性跨模态注意力利用 patch 级 CLIP 嵌入，实现图像与文本 token 的双向交互并显式建模预测不确定性，配合软 patch 级对比损失提升语义学习。在跨 5 种成像模态、6 个器官的 16 个数据集上的实验表明，MedCLIPSeg 在准确性、效率和鲁棒性方面均优于先前方法，并提供可解释的不确定性图。

- **DLT-Corpus: A Large-Scale Text Collection for the Distributed Ledger Technology Domain** `[微调]` — [2602.22045](https://arxiv.org/abs/2602.22045) | [GitHub](https://github.com/dlt-science/DLT-Corpus)
  > 本文介绍 DLT-Corpus，迄今最大的分布式账本技术（DLT）领域专用文本集合，包含来自科学文献（37,440 篇论文）、美国专利（49,023 份）和社交媒体（2200 万条帖子）共 29.8 亿 token。通过分析技术涌现模式和市场-创新相关性，发现技术通常先出现于科学文献，再扩散至专利和社交媒体，印证了传统技术转移规律。此外，论文还发布了领域适配模型 LedgerBERT，在 DLT 专属命名实体识别任务上比 BERT-base 提升 23%。


## 2026年3月2日

- **dLLM: Simple Diffusion Language Modeling** `[微调]` — [2602.22661](https://arxiv.org/abs/2602.22661) | [GitHub](https://github.com/ZHZisZZ/dllm)
  > dLLM 是一个开源统一框架，旨在标准化扩散语言模型（DLM）的核心组件，包括训练、推理与评估流程。现有扩散语言模型（如 LLaDA、Dream）的实现分散于各自代码库，缺乏统一规范，导致复现和扩展困难。dLLM 通过标准化流水线使用户能够复现、微调、部署和评估开源大型扩散语言模型，同时提供从 BERT 编码器或自回归语言模型转化为 DLM 的最小可复现配方，并公开了多个小型 DLM 的检查点，降低了扩散语言模型研究的门槛，加速未来相关工作的开展。

- **Compositional Generalization Requires Linear, Orthogonal Representations in Vision Embedding Models** `[无需训练]` — [2602.24264](https://arxiv.org/abs/2602.24264) | [GitHub](https://github.com/oshapio/necessary-compositionality)
  > 本文从理论上形式化了组合泛化所需的表示几何结构，证明若要在标准训练下实现对新组合的泛化，模型的表示必须满足三个条件：可分性、可迁移性和稳定性，由此推导出必要几何约束——表示须线性分解为各概念的正交分量。这为广泛观察到的「线性表示假说」提供了理论支撑：神经网络表示中的线性结构是组合泛化的必然结果。作者在 CLIP、SigLIP、DINO 等现代视觉模型上验证了这一预测，发现这些模型的表示确实呈现出部分线性因子化与低秩正交结构，且该结构程度与组合泛化性能正相关。

- **How to Take a Memorable Picture? Empowering Users with Actionable Feedback** `[VLM]` `[无需训练]` — [2602.21877](https://arxiv.org/abs/2602.21877) | [GitHub](https://github.com/laitifranz/MemCoach)
  > 本文提出 MemFeed 任务与 MemCoach 方法，旨在为用户拍摄时提供可操作的图像记忆性改善建议（如「强调面部表情」「将主体推至前景」）。MemCoach 基于多模态大语言模型（MLLM），无需训练，采用教师-学生引导策略，通过将模型内部激活对齐至教师模型从低记忆性到高记忆性样本学到的更具记忆性的模式来实现引导。论文还构建了 MemBench 数据集，包含序列对齐的连拍照片及记忆性评分标注。实验表明，MemCoach 相比多个零样本基线均有持续提升，证明记忆性不仅可以被预测，还可以被教导与指令化。

- **Accelerating Masked Image Generation by Learning Latent Controlled Dynamics** `[无需训练]` — [2602.23996](https://arxiv.org/abs/2602.23996) | [GitHub](https://github.com/Kaiwen-Zhu/MIGM-Shortcut)
  > 掩码图像生成模型（MIGM）因双向注意力的多步推理而效率受限。现有特征缓存方法在高加速比下存在较大近似误差。本文提出 MIGM-Shortcut，学习一个轻量化模型，综合利用历史特征与采样 token 来回归特征演化的平均速度场，从而更准确地预测未来特征。该方法被应用于两种代表性 MIGM 架构；在最先进的 Lumina-DiMOO 上，MIGM-Shortcut 实现了超过 4 倍的文本到图像生成加速，同时保持生成质量，显著推进了掩码图像生成的帕累托前沿。

- **Ref-Adv: Exploring MLLM Visual Reasoning in Referring Expression Tasks** `[VLM]` — [2602.23898](https://arxiv.org/abs/2602.23898) | [GitHub](https://github.com/dddraxxx/Ref-Adv)
  > 本文介绍 Ref-Adv，一个旨在抑制快捷路径的指代表达理解（REC）数据集，通过将语言上非平凡的表达与仅包含唯一标识目标所需信息的难干扰项配对构建而成，并标注了包含否定在内的推理类型。实验通过词序扰动和描述词删除充分性消融验证了求解 Ref-Adv 需要真正的推理能力。对大量多模态 LLM 的评估表明，尽管模型在 RefCOCO 系列上表现强劲，在 Ref-Adv 上却显著下降，揭示了当前 MLLM 在视觉推理与定位方面依赖快捷路径的局限。

- **DUET-VLM: Dual stage Unified Efficient Token reduction for VLM Training and Inference** `[VLM]` `[微调]` — [2602.18846](https://arxiv.org/abs/2602.18846) | [GitHub](https://github.com/AMD-AGI/DUET-VLM)
  > DUET-VLM 是一个即插即用的双阶段视觉 token 压缩框架，用于提升视觉语言模型（VLM）的训练和推理效率。第一阶段在视觉编码器输出上进行冗余感知压缩，生成信息保留的 token；第二阶段在语言主干中逐层进行文本引导的显著性 token 丢弃，渐进剪除信息量低的 token。在 LLaVA-1.5-7B 上，DUET-VLM 以减少 67% token 的代价保持超过 99% 的基线精度，在极端 89% 减少设置下仍保留 97% 精度，在多个评测任务上超越已有 SoTA token 压缩方法；集成到 Video-LLaVA-7B 后更以 53.1% token 减少超越原始基线。


## 2026年3月3日

- **OmniLottie: Generating Vector Animations via Parameterized Lottie Tokens** `[VLM]` `[无需训练]` — [2603.02138](https://arxiv.org/abs/2603.02138) | [GitHub](https://github.com/OpenVGLab/OmniLottie)
  > OmniLottie 是一个通用向量动画生成框架，支持从多模态指令生成高质量矢量动画。核心贡献在于设计了 Lottie Tokenizer，将 JSON 格式的 Lottie 动画文件转换为形状、动画函数和控制参数的结构化命令序列，消除了原始 JSON 中大量不变结构元数据的冗余，使预训练视觉语言模型能够高效处理向量动画生成任务。框架在预训练 VLM 基础上构建，支持多模态交互式指令输入，能够生成语义对齐的矢量动画。为推动该领域研究，作者同步发布了 MMLottie-2M 大规模数据集，包含专业设计的矢量动画及其文本和视觉标注。实验验证 OmniLottie 可生成符合多模态人类指令、视觉生动且语义准确的向量动画。

- **OpenAutoNLU: Open Source AutoML Library for NLU** `[微调]` — [2603.01824](https://arxiv.org/abs/2603.01824) | [GitHub](https://github.com/mts-ai/OpenAutoNLU)
  > OpenAutoNLU 是一个面向自然语言理解（NLU）任务的开源自动化机器学习库，覆盖文本分类和命名实体识别（NER）。其核心创新是「数据感知训练模式选择」机制，无需用户手动配置即可根据数据特性自动选择最优训练方案，有别于现有 AutoML 解决方案。库内还集成了数据质量诊断模块、可配置的分布外（OOD）检测功能，以及基于 LLM 的特性支持，整体通过极简低代码 API 提供。该库提供了完整的 Docker 部署方案，并有在线 Demo 可直接访问。作者在多个 NLU 任务上验证了其自动化流程的有效性，展示了无需专业配置也能获得竞争力结果的实用价值。

- **MMR-Life: Piecing Together Real-life Scenes for Multimodal Multi-image Reasoning** `[VLM]` — [2603.02024](https://arxiv.org/abs/2603.02024) | [GitHub](https://github.com/BugMakerzzz/MMR-Life)
  > MMR-Life 是一个面向真实场景的多模态多图推理评测集，旨在全面评估多模态大语言模型（MLLM）在真实生活场景中的推理能力。数据集包含 2,646 道多选题，基于 19,108 张真实场景图像构建，覆盖 7 种推理类型：溯因、类比、因果、演绎、归纳、空间和时间推理。与现有推理评测集不同，MMR-Life 不依赖特定领域专业知识，而是要求模型跨多图整合信息并运用多元推理能力。对 37 个先进模型的评测表明，该数据集极具挑战性，即使是 GPT-5 也仅达到 58% 准确率，且在不同推理类型间表现差异显著。研究还分析了思维长度、推理方法和推理类型等因素对 MLLM 性能的影响，为下一代多模态推理系统的评估与改进提供了基础。


## 2026年3月4日

- **Utonia: Toward One Encoder for All Point Clouds** `[VLM]` — [2603.03283](https://arxiv.org/abs/2603.03283) | [GitHub](https://github.com/Pointcept/Utonia)
  > Utonia 提出了一个统一的自监督点云 Transformer 编码器，能够跨越遥感、户外 LiDAR、室内 RGB-D 序列、物体级 CAD 模型和从 RGB 视频提取的点云等多个领域进行联合预训练。尽管各域的传感器几何、密度和先验差异显著，Utonia 仍能学习到一致的表征空间并跨域迁移。联合训练不仅提升了感知能力，还产生了单域训练中未出现的涌现行为。此外，Utonia 表征可以用于视觉-语言-动作策略和视觉-语言模型，分别在空间推理任务上取得了增益，迈向稀疏三维数据的基础模型。

- **BeyondSWE: Can Current Code Agent Survive Beyond Single-Repo Bug Fixing?** — [2603.03194](https://arxiv.org/abs/2603.03194) | [GitHub](https://github.com/AweAI-Team/BeyondSWE)
  > BeyondSWE 扩展了代码智能体的评估维度，沿「解决范围」和「知识范围」两个轴设计了包含 500 个真实实例的综合评估框架，涵盖跨仓库推理、领域专业化问题修复、依赖驱动迁移和完整仓库生成四类任务。实验表明，即使是前沿模型在整体成功率上也低于 45%，且没有单一模型能在所有任务类型上保持一致优势。论文还提出 SearchSWE 框架，将深度搜索与编码能力结合，探索外部知识对代码智能体的影响，发现搜索增强的收益并不稳定，有时甚至降低性能。

- **PRISM: Pushing the Frontier of Deep Think via Process Reward Model-Guided Inference** `[RL]` `[无需训练]` — [2603.02479](https://arxiv.org/abs/2603.02479) | [GitHub](https://github.com/Rituraj003/PRISM)
  > PRISM 针对「深度思考」方法中缺乏可靠正确性信号的瓶颈问题，引入了一个以过程奖励模型（PRM）为核心的功能性推理框架。通过在推理过程中利用 PRM 对中间步骤进行评估，PRISM 有效避免了群体增强时错误被放大、正确少数解被抑制的问题，从而实现更深层次的思考并提升计算效率。在复杂数学和科学推理任务上，PRISM 相比现有深度思考方法取得了显著提升，展示了过程监督信号在推理时扩展中的关键作用。

- **Code2Math: Can Your Code Agent Effectively Evolve Math Problems Through Exploration?** — [2603.03202](https://arxiv.org/abs/2603.03202) | [GitHub](https://github.com/TarferSoul/Code2Math)
  > Code2Math 研究代码智能体能否自主将已有数学问题演化为更复杂的变体，以缓解高质量难题稀缺的瓶颈。论文提出一个多智能体框架，在演化问题的同时验证可解性和难度提升。实验表明，给予足够的测试时探索，代码智能体能够合成结构上有别于原题且更具挑战性的可解新题，为高难度数学推理数据的自动化生成提供了可行路径。所有演化数据、示例和提示模板已开源。

- **Humans and LLMs Diverge on Probabilistic Inferences** — [2602.23546](https://arxiv.org/abs/2602.23546) | [GitHub](https://github.com/McGill-NLP/probabilistic-reasoning)
  > 本文提出 ProbCOPA，一个包含 210 道手工构造的概率推理题的数据集，评估模型在开放式、非确定性推断任务上的表现。研究发现，推理型 LLM 在这类任务上与人类判断存在系统性分歧：模型倾向于将非必然推断处理为确定性结论，而人类则更倾向于概率化推断。实验涵盖多个推理模型，通过与人类基准的比对揭示了当前 LLM 在概率推理上的本质局限，并分析了不同提示策略和思维链推理对结果的影响。

- **Surgical Post-Training: Cutting Errors, Keeping Knowledge** `[微调]` `[RL]` — [2603.01683](https://arxiv.org/abs/2603.01683) | [GitHub](https://github.com/Visual-AI/SPoT)
  > Surgical Post-Training（SPoT）旨在解决 LLM 后训练中效率与灾难性遗忘之间的权衡难题。论文从理论和实验两方面揭示了 DPO 奖励估计中的隐式正则化机制，并基于此设计了手术式后训练方法：通过精准识别并仅微调导致错误的参数子集，在显著减少计算开销的同时保留已有知识。在多个推理基准上，SPoT 相比全量后训练方法在遗忘和效率方面均取得了更优的平衡，验证了局部参数更新策略的有效性。

- **Spilled Energy in Large Language Models** `[无需训练]` — [2602.18671](https://arxiv.org/abs/2602.18671) | [GitHub](https://github.com/OmnAI-Lab/spilled-energy)
  > 本文将 LLM 最终层的 softmax 分类器重新解释为基于能量的模型（EBM），将序列到序列的概率链分解为多个相互作用的 EBM。通过在解码过程中追踪「能量溢出」现象，实证研究表明能量溢出与事实性错误、偏差和推理失败之间存在高度相关性。该方法能精准定位答案 token 并进行幻觉检测，无需额外训练，优于依赖语义不一致性检测的方法。实验在多个 LLM 和事实性问答任务上验证了能量溢出作为可靠幻觉预测器的有效性。

- **InfoPO: Information-Driven Policy Optimization for User-Centric Agents** `[RL]` — [2603.00656](https://arxiv.org/abs/2603.00656) | [GitHub](https://github.com/kfq20/InfoPO)
  > InfoPO 针对 LLM 智能体处理欠规格用户请求时的多轮交互优化问题，解决了基于轨迹级奖励的 GRPO 方法存在的信用分配问题和组内优势信号不足的缺陷。通过在细粒度层面识别高价值交互轮次，InfoPO 引入信息驱动的策略优化框架，能够针对性地学习何时主动获取信息、何时直接执行任务。在多个以用户为中心的智能体任务上，InfoPO 显著优于基线方法，在减少不必要澄清的同时提升了下游任务成功率。

- **CFG-Ctrl: Control-Based Classifier-Free Diffusion Guidance** `[无需训练]` — [2603.03281](https://arxiv.org/abs/2603.03281) | [GitHub](https://github.com/hanyang-21/CFG-Ctrl)
  > CFG-Ctrl 将分类器自由引导（CFG）统一重新诠释为施加在一阶连续时间生成流上的控制，以条件-无条件差异作为误差信号调整速度场。从这一视角出发，标准 CFG 等价于增益固定的比例控制器（P-控制），而 CFG-Ctrl 进一步引入积分和微分项（PI/PD/PID 控制），动态调节引导强度。在 text-to-image 生成任务中，该方法在不改变模型结构的前提下提升了语义对齐质量和生成多样性，展示了控制论视角对扩散模型引导机制的统一解释力。

- **SciDER: Scientific Data-centric End-to-end Researcher** — [2603.01421](https://arxiv.org/abs/2603.01421) | [GitHub](https://github.com/leonardodalinky/SciDER)
  > SciDER 是一个以数据为中心的端到端自动化科研系统，旨在解决现有 LLM 科研智能体无法自主处理真实实验原始数据的瓶颈。系统通过多个专业化智能体协作解析和分析原始科学数据，结合具体数据生成假说和实验设计，并迭代执行实验以验证假说。与传统框架相比，SciDER 将数据处理、假说生成和实验执行整合进统一闭环，在多个科学发现任务上展示了更高的自动化程度和研究质量，推动了 LLM 辅助科学发现的前沿。

- **Towards Simulating Social Media Users with LLMs: Evaluating the Operational Validity of Conditioned Comment Prediction** — [2602.22752](https://arxiv.org/abs/2602.22752) | [GitHub](https://github.com/nsschw/Conditioned-Comment-Prediction)
  > 本文提出条件评论预测（CCP）任务，通过将模型生成输出与真实数字轨迹对比，严格评估 LLM 作为社交媒体用户模拟器的操作有效性。研究引入多维框架，系统分析当前 LLM 在模拟用户评论行为方面的能力与局限，揭示了模型输出与真实用户行为之间的显著差距。实验覆盖多个主流 LLM，结果表明现有模型仍难以可靠地捕捉真实用户的多样性和个体特征，为社会科学中的「硅基受试者」研究提供了基础验证框架。

- **DREAM: Where Visual Understanding Meets Text-to-Image Generation** `[VLM]` `[微调]` — [2603.02667](https://arxiv.org/abs/2603.02667) | [GitHub](https://github.com/chaoli-charlie/dream)
  > DREAM 在单一模型中统一优化判别式视觉表征学习和生成式 text-to-image 目标。其核心技术包括：训练阶段的「掩码预热」（从低掩码率渐进提升以建立对比对齐基础），以及「双流注意力」（将图像 token 路由至独立的理解和生成流）。这种设计使模型同时在表征质量和生成质量上达到强基线水平，打破了判别目标和生成目标之间的传统冲突，为多模态统一模型提供了新的技术路径。

- **ParEVO: Synthesizing Code for Irregular Data: High-Performance Parallelism through Agentic Evolution** — [2603.02510](https://arxiv.org/abs/2603.02510) | [GitHub](https://github.com/WildAlg/ParEVO)
  > ParEVO 针对不规则数据结构（稀疏图、非平衡树、非均匀网格）的高性能并行代码生成难题，提出了一种智能体进化框架。当前 LLM 在此类任务上往往生成存在竞争条件和死锁的错误代码，ParEVO 通过多智能体协作演化和验证机制迭代改进代码正确性与并行效率。实验表明，在充分探索后，ParEVO 能合成结构正确、高性能的并行代码，相比直接生成方法显著降低了错误率并提升了加速比，为不规则计算场景提供了可扩展的自动并行化路径。

- **LFPO: Likelihood-Free Policy Optimization for Masked Diffusion Models** `[RL]` `[微调]` — [2603.01563](https://arxiv.org/abs/2603.01563) | [GitHub](https://github.com/kithib/LFPO)
  > LFPO 解决了将强化学习与可验证奖励（RLVR）范式应用于扩散大语言模型（dLLM）时精确似然难以计算的根本性障碍。现有方法不得不依赖高方差近似，LFPO 提出无需似然计算的策略优化方法，直接基于可验证奖励信号优化掩码扩散模型。在数学推理和代码生成任务上，LFPO 相比现有 dLLM 强化学习方法取得了显著提升，验证了无似然策略优化在离散扩散模型后训练中的可行性，为将 RLVR 的成功从自回归模型扩展到扩散模型提供了桥梁。

- **Conditioned Activation Transport for T2I Safety Steering** `[无需训练]` — [2603.03163](https://arxiv.org/abs/2603.03163) | [GitHub](https://github.com/NASK-AISafety/conditional-activation-transport)
  > 针对 text-to-image 模型生成不安全内容的问题，本文首先构建了 SafeSteerDataset——包含 2300 对高余弦相似度安全/不安全提示对的对比数据集，发现线性激活引导在良性提示下会显著降低图像质量。为此，提出条件激活传输（CAT）方法，通过最优传输将不安全激活条件映射到安全激活空间，实现精准的推理时安全干预。实验表明 CAT 在有效阻止不安全生成的同时，对良性提示的图像质量损伤极小，在安全性和生成质量的权衡上优于现有激活引导方法。

- **HateMirage: An Explainable Multi-Dimensional Dataset for Decoding Faux Hate and Subtle Online Abuse** — [2603.02684](https://arxiv.org/abs/2603.02684) | [GitHub](https://github.com/Sai-Kartheek-Reddy/HateMirage)
  > HateMirage 是一个新颖的「伪仇恨」评论数据集，专注于从虚假信息中涌现的隐性仇恨言论，填补了现有数据集主要覆盖显性毒性内容的空白。数据集提供多维度标注，包括仇恨类型、推理链和可解释性标签，旨在推进针对微妙在线虐待和伪装式仇恨的推理与可解释性研究。实验评估了多种 LLM 在检测此类细微仇恨言论上的能力，揭示了当前模型在理解隐性有害意图方面的局限，为更鲁棒的在线安全系统提供了数据基础。

- **Fast Matrix Multiplication in Small Formats: Discovering New Schemes with an Open-Source Flip Graph Framework** — [2603.02398](https://arxiv.org/abs/2603.02398) | [GitHub](https://github.com/dronperminov/ternary_flip_graph)
  > 本文开源了一个用于发现快速矩阵乘法方案的 C++ 框架，基于翻转图（flip graph）方法，支持二进制（Z₂）、模三元（Z₃）和整数三元（Z_T = {-1,0,1}）多种系数环，并实现了固定维度和元维度搜索算子。通过位级编码和 OpenMP 并行化，框架可在普通硬件上进行大规模探索，覆盖 680 种小格式矩阵乘法方案。实验发现了多个具有改进乘法复杂度的新方案，证明了翻转图方法结合高效工程实现在矩阵乘法算法发现中的实用价值。

- **Words & Weights: Streamlining Multi-Turn Interactions via Co-Adaptation** `[微调]` — [2603.01375](https://arxiv.org/abs/2603.01375) | [GitHub](https://github.com/kithib/ROSA2)
  > ROSA2 提出「测试时策略适应」（T2PAM）框架，同时优化提示（文字）和权重两个维度来适配多轮交互中的动态用户需求。现有方法要么仅优化提示工程，要么仅进行测试时训练，而 ROSA2 指出交互失败源于歧义和能力不足的耦合，需要双轴协同优化。通过在推理时动态协调指令精化和权重调整，ROSA2 在多轮对话适应任务上显著优于单轴基线，验证了提示-权重协同适应在处理多轮动态用户需求中的有效性。

- **GroupGPT: A Token-efficient and Privacy-preserving Agentic Framework for Multi-User Chat Assistant** `[微调]` — [2603.01059](https://arxiv.org/abs/2603.01059) | [GitHub](https://github.com/Eliot-Shen/GroupGPT)
  > GroupGPT 针对多用户群聊场景，提出一个兼顾 token 效率和隐私保护的智能体框架。现有系统通常将 LLM 同时用于推理和生成，导致 token 消耗高、可扩展性差且存在隐私风险。GroupGPT 设计了专用的轻量推理模块判断何时介入，配合隐私保护机制避免泄露用户个人信息，并通过训练任务使模型能主动、准确地在复杂演化的多用户语境中插话。实验表明，GroupGPT 相比现有多用户对话系统在介入准确性和 token 效率上均取得了显著提升。

- **SGDC: Structurally-Guided Dynamic Convolution for Medical Image Segmentation** — [2602.23496](https://arxiv.org/abs/2602.23496) | [GitHub](https://github.com/solstice0621/SGDC)
  > SGDC 针对医学图像分割中主流动态卷积通过平均池化生成核权重导致高频空间细节丢失、预测过平滑的问题，提出结构引导的动态卷积方法。通过引入结构敏感的核生成机制，保留局部高频细节，在生成动态卷积核时保持对细粒度临床结构的感知能力。在多个医学图像分割数据集上，SGDC 相比标准动态卷积基线显著提升了精细结构的分割保真度，验证了结构引导机制在空间自适应卷积中的重要性。

- **Transform-Invariant Generative Ray Path Sampling for Efficient Radio Propagation Modeling** — [2603.01655](https://arxiv.org/abs/2603.01655) | [GitHub](https://github.com/jeertmans/sampling-paths)
  > 本文针对射线追踪在无线传播建模中指数级计算复杂度的瓶颈，提出变换不变生成式射线路径采样方法。传统方法候选路径数随物体数量指数增长，而本方法通过生成模型直接采样高概率传播路径，并利用变换不变性降低所需路径候选数量。实验表明，相比传统射线追踪工具，该方法在保持精度的同时大幅降低计算开销，为大规模或实时无线传播仿真提供了可行的深度学习路径。

- **Multi-Domain Riemannian Graph Gluing for Building Graph Foundation Models** — [2603.00618](https://arxiv.org/abs/2603.00618) | [GitHub](https://github.com/RiemannGraph/GraphGlue)
  > 本文提出黎曼图粘合（Graph Gluing）框架，解决多域图预训练中知识跨域整合与迁移的理论问题。现有图基础模型预训练方法缺乏对跨域知识如何整合的清晰解释，本文通过重新审视预训练与域适应之间的一致性和可迁移性，在黎曼几何空间中构建统一的理论框架，实现多域图知识的「粘合」。在多个图学习任务和域上，GraphGlue 相比现有多域图预训练方法取得了更优的迁移学习性能，为构建通用图基础模型提供了有理论保证的技术路径。

## 2026年3月5日

- **MemSifter: Offloading LLM Memory Retrieval via Outcome-Driven Proxy Reasoning** `[RL]` `[MeM]` — [2603.03379](https://arxiv.org/abs/2603.03379) | [GitHub](https://github.com/plageon/MemSifter)
  > MemSifter 提出了一种将记忆检索任务卸载到小型代理模型的新框架，解决大语言模型在长期任务中记忆管理的效率与准确性权衡难题。核心创新是为代理模型引入记忆专用强化学习训练范式：基于工作LLM的实际任务完成情况设计任务结果导向奖励函数，通过多次交互衡量检索记忆的真实贡献，并采用阶梯递减贡献区分检索排名。同时结合课程学习和模型合并技术提升性能。在包括Deep Research在内的8个LLM记忆基准测试上，MemSifter达到或超越现有最优方法的检索精度和任务完成率，并已开源模型权重、代码和训练数据。

- **V_1: Unifying Generation and Self-Verification for Parallel Reasoners** `[RL]` `[无需训练]` — [2603.04304](https://arxiv.org/abs/2603.04304) | [GitHub](https://github.com/HarmanDotpy/pairwise-self-verification)
  > V_1 是将生成与自我验证统一于并行推理器的框架，针对测试时扩展中验证瓶颈问题提出解法。核心洞察是模型在两两对比验证上远强于标量评分，引入基于锦标赛排名的不确定性引导算法V_1-Infer，动态为最不确定的候选对分配验证算力；V_1-PairRL通过强化学习联合训练单一模型同时作为生成器和成对自我验证器。在代码生成（LiveCodeBench、SWE-Bench）和数学推理（AIME、HMMT）上，V_1-Infer相比逐点验证提升Pass@1最高10%；V_1-PairRL相比标准RL实现7-9%测试时扩展增益，基础Pass@1提升最高8.7%。

- **AgilePruner: An Empirical Study of Attention and Diversity for Adaptive Visual Token Pruning in Large Vision-Language Models** `[VLM]` `[无需训练]` — [2603.01236](https://arxiv.org/abs/2603.01236) | [GitHub](https://github.com/cvsp-lab/AgilePruner)
  > AgilePruner 针对大型视觉语言模型的视觉token剪枝策略进行深度实证分析。通过有效秩（erank）衡量特征多样性、注意力分数熵衡量注意力机制，揭示两大关键洞见：多样性导向剪枝实际保留的特征多样性远低于预期，且CHAIR评估表明其保留多样性与更高幻觉频率相关；注意力方法在视觉证据集中的简单图像上更有效，多样性方法则更擅长特征分散的复杂图像。基于此提出将图像感知调整融入混合剪枝策略，设计的自适应剪枝机制在标准评测和幻觉评估上均表现出稳健的性能提升。

- **BeamPERL: Parameter-Efficient RL with Verifiable Rewards Specializes Compact LLMs for Structured Beam Mechanics Reasoning** `[RL]` — [2603.04124](https://arxiv.org/abs/2603.04124) | [GitHub](https://github.com/lamm-mit/BeamPERL)
  > BeamPERL 研究参数高效RLVR能否教会小型语言模型进行物理推理。以梁静力学工程问题为场景，对1.5B参数模型使用来自符号求解器的二元可验证奖励训练，无需教师推理轨迹。最优检查点Pass@1相比基础模型提升66.7%。然而习得的能力呈各向异性：可泛化到组合变化（更多载荷），但在需要相同平衡方程的拓扑变化（移动支撑）下失败。研究揭示结果级对齐的关键局限：精确物理奖励信号仅诱导程序性解题模板而非真正内化控制方程，提示需结合结构化推理脚手架才能超越模板匹配。

- **HDINO: A Concise and Efficient Open-Vocabulary Detector** `[VLM]` — [2603.02924](https://arxiv.org/abs/2603.02924) | [GitHub](https://github.com/HaoZ416/HDINO)
  > HDINO 提出简洁高效的开放词汇目标检测方法，消除对人工标注细粒度训练数据和逐层跨模态特征提取的依赖。基于DINO模型的两阶段训练策略：第一阶段通过一对多语义对齐机制（O2M）将噪声样本视为额外正例，配合难样本加权分类损失促进视觉-语言对齐；第二阶段用轻量特征融合模块增强对语言语义的敏感性。HDINO-T仅用220万图片在COCO达49.2 mAP，超越使用540万图片训练的Grounding DINO-T（+0.8 mAP）；微调后HDINO-T和HDINO-L分别达56.4和59.2 mAP。

## 2026年3月6日

- **MOOSE-Star: Unlocking Tractable Training for Scientific Discovery by Breaking the Complexity Barrier** `[无需训练]` — [2603.03756](https://arxiv.org/abs/2603.03756) | [GitHub](https://github.com/ZonglinY/MOOSE-Star)
  > MOOSE-Star 针对科学发现中直接训练假设生成过程P(h|b)在数学上不可行（组合复杂度O(N^k)）的问题，提出将复杂度从指数降至对数O(log N)的统一框架。核心方法包含：基于发现概率方程分解子任务进行训练；动机引导层次化搜索实现对数级检索并剪枝无关子空间；有界组合增强对检索噪声的鲁棒性。同时发布包含108,717篇分解论文的TOMATO-Star训练数据集（耗费38,400 GPU小时）。实验表明暴力采样遭遇「复杂度墙」，而MOOSE-Star展现持续的测试时扩展能力，为LLM驱动的科学发现提供可行训练路径。

- **SkillNet: Create, Evaluate, and Connect AI Skills** `[MeM]` — [2603.04448](https://arxiv.org/abs/2603.04448) | [GitHub](https://github.com/zjunlp/SkillNet)
  > SkillNet 是一个面向AI Agent技能系统性积累与迁移的开放基础设施，解决Agent因缺乏技能统一沉淀机制而「重复造轮子」的问题。基于统一本体论组织技能，支持从异构来源创建技能、建立丰富关联关系，并从安全性、完整性、可执行性、可维护性和成本意识五个维度进行多维评估。平台集成超过20万技能仓库、交互平台和Python工具包。在ALFWorld、WebShop和ScienceWorld上的评估显示，SkillNet将Agent平均奖励提升40%，执行步骤减少30%。

- **DARE: Aligning LLM Agents with the R Statistical Ecosystem via Distribution-Aware Retrieval** — [2603.04743](https://arxiv.org/abs/2603.04743) | [GitHub](https://github.com/AMA-CMFAI/DARE)
  > DARE（分布感知检索嵌入）提出将数据分布信息融入函数表示的轻量化即插即用检索模型，解决LLM Agent在R包检索中忽略数据分布导致匹配次优的问题。主要贡献包括：RPKB——从8,191个高质量CRAN包构建的R包知识库；DARE——融合分布特征与函数元数据的嵌入模型；RCodingAgent——面向R统计生态的LLM代码生成Agent。实验中DARE在包检索NDCG@10达93.47%，比最优开源嵌入模型高出最多17%，参数量显著更少，集成DARE的RCodingAgent在下游统计分析任务中取得显著提升。

- **AgentVista: Evaluating Multimodal Agents in Ultra-Challenging Realistic Visual Scenarios** `[VLM]` — [2602.23166](https://arxiv.org/abs/2602.23166) | [GitHub](https://github.com/hkust-nlp/AgentVista)
  > AgentVista 为通用多模态Agent构建了一个覆盖7类25个子领域的高难度评估集，将真实细节丰富的视觉场景与自然混合工具使用配对。任务要求跨模态长时程工具交互，包括网页搜索、图像搜索、页面导航及图像处理和通用编程的代码操作。对最先进模型的综合评估揭示了其在长时程多模态工具使用上的显著差距——表现最好的Gemini-3-Pro with tools整体准确率仅27.3%，难题可能需要超过25轮工具调用。

- **Large Multimodal Models as General In-Context Classifiers** `[VLM]` `[无需训练]` — [2602.23229](https://arxiv.org/abs/2602.23229) | [GitHub](https://github.com/marco-garosi/CIRCLE)
  > 本文重新审视大型多模态模型（LMM）在分类任务中的潜力，提出LMM凭借上下文学习能力可媲美甚至超越CLIP类对比VLM。研究发现：LMM零样本分类性能低于CLIP，但提供少量上下文示例后，LMM可匹配或超越带缓存适配器的对比VLM。针对开放世界分类中不完美上下文信息导致LMM表现退化的问题，提出CIRCLE——一种无需训练的方法，通过为上下文示例分配伪标签并迭代精炼来克服这一局限。广泛实验证明CIRCLE在开放世界分类上建立了稳健基线，凸显LMM作为统一分类器的潜力。

- **Towards Multimodal Lifelong Understanding: A Dataset and Agentic Baseline** `[VLM]` `[MeM]` — [2603.05484](https://arxiv.org/abs/2603.05484) | [GitHub](https://github.com/cg1177/Recursive-Multimodal-Agent)
  > 本文引入MM-Lifelong数据集，专为多模态终身理解设计，包含181.1小时真实日常生活影像，按Day、Week、Month三个时间尺度组织，捕捉不同时间密度的内容。评估揭示现有方法两大关键失败模式：端到端多模态LLM因上下文饱和遭遇工作记忆瓶颈，代理基线则在稀疏月级时间线中发生全局定位崩溃。为此提出递归多模态Agent（ReMA），采用动态记忆管理迭代更新递归信念状态，显著优于现有方法。数据集还设计了隔离时间和领域偏差的划分方式，为未来研究提供严格基础。

- **Truncated Step-Level Sampling with Process Rewards for Retrieval-Augmented Reasoning** `[RL]` — [2602.23440](https://arxiv.org/abs/2602.23440) | [GitHub](https://github.com/algoprog/SLATE)
  > SLATE 框架针对RAG推理中强化学习训练的信用分配难题提出解决方案。现有方法仅在完整轨迹末提供稀疏结果奖励，无法归因个体推理和检索决策。SLATE基于两个互补思想：截断步级采样，生成共享公共前缀而仅在下一步不同的k条轨迹，理论证明相较完整轨迹采样可将优势估计方差降低最多T倍；LLM-as-judge密集奖励，取代启发式评分，对每个推理步、搜索查询和答案进行质量评估。在7个QA基准上的实验证实SLATE持续优于稀疏奖励和过程奖励基线，在更难的多跳任务和小模型上增益最大。

## 2026年3月8日

- **FlashPrefill: Instantaneous Pattern Discovery and Thresholding for Ultra-Fast Long-Context Prefilling** `[长文本]` `[无需训练]` — [2603.06199](https://arxiv.org/abs/2603.06199) | [GitHub](https://github.com/qhfan/FlashPrefill)
  > FlashPrefill 提出了一种超快速长上下文预填充框架，通过即时模式发现与动态阈值化机制解决注意力的二次复杂度瓶颈。核心方法包括：快速块搜索技术同时定位动态垂直、斜线及块稀疏注意力模式；动态阈值机制绕过排序或累积注意力分数的高昂开销，消除长尾分布以增强稀疏性。实验表明，FlashPrefill 在 256K 序列上实现了前所未有的 27.78 倍加速，即使在 4K 上下文长度下也保持 1.71 倍加速，展现出在不同序列规模下的强健性与实用价值，同时不损失任务性能。

## 2026年3月9日

- **Penguin-VL: Exploring the Efficiency Limits of VLM with LLM-based Vision Encoders** `[VLM]` `[微调]` — [2603.06569](https://arxiv.org/abs/2603.06569) | [GitHub](https://github.com/tencent-ailab/Penguin-VL)
  > Penguin-VL 挑战了主流 VLM 必须依赖 CLIP/SigLIP 等对比预训练视觉编码器的惯例，转而使用纯文本 LLM 初始化的视觉编码器。研究发现，对比学习优化的判别目标会强制施加粗粒度类别级别不变性，压制精细视觉线索。Penguin-Encoder 在多模态理解中解锁了更高的视觉保真度与数据效率。在紧凑型 2B/8B 参数规模下，Penguin-VL 在数学推理上媲美 Qwen3-VL，在文档理解、视觉知识和多视角视频理解上超越之。消融实验表明改善视觉表示而非扩大模型规模才是性能的主要驱动力。

- **BandPO: Bridging Trust Regions and Ratio Clipping via Probability-Aware Bounds for LLM Reinforcement Learning** `[RL]` — [2603.04918](https://arxiv.org/abs/2603.04918) | [GitHub](https://github.com/OpenMOSS/BandPO)
  > BandPO 针对大语言模型强化学习训练中 PPO 固定裁剪边界的关键瓶颈进行改进：固定边界严格限制低概率动作的上行更新余量，不成比例地压制高优势尾部策略并引发快速熵崩溃。BandPO 用 Band 算子替换标准裁剪，将 f-散度定义的信任域投影到动态的概率感知裁剪区间。理论分析证明 Band 有效解决了探索瓶颈，其映射被构造为凸优化问题并给出特定散度的闭式解。在多种模型和数据集上的大量实验表明，BandPO 持续优于标准裁剪和 Clip-Higher，同时稳健缓解熵崩溃。

- **Progressive Residual Warmup for Language Model Pretraining** — [2603.05369](https://arxiv.org/abs/2603.05369) | [GitHub](https://github.com/dandingsky/ProRes)
  > ProRes（渐进残差预热）为语言模型预训练提出了"早层先学"哲学：对每层的残差连接乘以标量，该标量从 0 逐渐预热至 1，深层比浅层需要更长的预热步数。这使得深层等待浅层进入更稳定的学习模式后再开始贡献学习。通过跨越不同模型规模、归一化方式和初始化方案的预训练实验验证，ProRes 不仅稳定了预训练过程，还引入了独特的优化轨迹，带来更快的收敛速度、更强的泛化能力和更好的下游任务性能。

## 2026年3月10日

- **Lost in Stories: Consistency Bugs in Long Story Generation by LLMs** `[长文本]` — [2603.05890](https://arxiv.org/abs/2603.05890) | [GitHub](https://github.com/Picrew/ConStory-Bench)
  > 本文研究了大语言模型在长篇故事生成中维护叙事一致性的能力。研究提出 ConStory-Bench，含 2000 个提示的评测集，覆盖四种任务场景，定义了 5 类误差、19 个细粒度子类型的分类体系。同时开发了 ConStory-Checker 自动化流水线，检测矛盾并在文本证据中定位每个判断。通过对多种 LLM 的五大研究问题评估发现：一致性错误在事实和时间维度最为常见，倾向出现在叙事中段，发生在 token 级熵更高的文本段落，为改进长篇叙事生成中的一致性提供了方向性指导。

- **LoGeR: Long-Context Geometric Reconstruction with Hybrid Memory** `[长文本]` `[无需训练]` — [2603.03269](https://arxiv.org/abs/2603.03269) | [GitHub](https://github.com/Junyi42/LoGeR)
  > LoGeR（长上下文几何重建）提出了一种将稠密重建扩展至超长序列的新架构，无需后优化。通过分块处理视频流并利用双向先验进行高保真块内推理，LoGeR 以混合记忆模块解决跨块边界的一致性挑战：参数化的测试时训练（TTT）记忆锚定全局坐标系防止尺度漂移，非参数化的滑动窗口注意力（SWA）保留未压缩上下文以实现高精度邻近对齐。训练于 128 帧序列，推理可泛化至数千帧。在含最长 19k 帧序列的数据集上，LoGeR 将 KITTI ATE 降低超过 74%，实现跨前所未有长度的全局一致重建。

- **CARE-Edit: Condition-Aware Routing of Experts for Contextual Image Editing** `[无需训练]` — [2603.08589](https://arxiv.org/abs/2603.08589) | [GitHub](https://github.com/CARE-Edit/Code)
  > CARE-Edit 提出了条件感知专家路由机制，解决统一扩散编辑器因使用固定共享主干导致的任务干扰和多条件冲突问题。核心设计是轻量级潜在注意力路由器，根据多模态条件和扩散时间步将编码扩散 token 动态分配给文本、掩码、参考和基础四类专家。稀疏 top-K 路由动态分配计算至最相关专家；潜在混合模块融合专家输出整合语义、空间和风格信息。在擦除、替换、文本驱动编辑和风格迁移等任务上验证了 CARE-Edit 的优越性能。

- **CoCo: Code as CoT for Text-to-Image Preview and Rare Concept Generation** `[VLM]` `[微调]` — [2603.08652](https://arxiv.org/abs/2603.08652) | [GitHub](https://github.com/micky-li-hd/CoCo)
  > CoCo（Code-as-CoT）提出以可执行代码作为链式思维（CoT）推理的载体，替代抽象自然语言规划，为文本到图像生成实现精确且可验证的中间规划。给定文本提示，CoCo 首先生成指定场景结构布局的可执行代码，在沙箱环境中渲染确定性草稿图像，随后通过精细图像编辑优化为最终高保真结果。构建了包含结构化草稿-最终图像对的 CoCo-10K 数据集支持训练。在 StructT2IBench、OneIG-Bench 和 LongText-Bench 上，CoCo 分别取得了 +68.83%、+54.8% 和 +41.23% 的提升。

## 2026年3月11日

- **MM-Zero: Self-Evolving Multi-Model Vision Language Models From Zero Data** `[RL]` `[VLM]` — [2603.09206](https://arxiv.org/abs/2603.09206) | [GitHub](https://github.com/zli12321/MM-Zero)
  > MM-Zero 提出了首个基于强化学习的零数据 VLM 自演化框架。与以往双角色（提问者+求解者）设置不同，MM-Zero 引入三角色训练框架：Proposer 生成抽象视觉概念并提问，Coder 将概念转为可执行代码渲染图像，Solver 对生成内容进行多模态推理。三个角色从同一基础模型初始化，使用 GRPO 训练，奖励机制融合了执行反馈、视觉验证和难度平衡。实验表明 MM-Zero 在多项多模态推理基准上显著提升性能，建立了可扩展的多模型自演化路径。

- **Omni-Diffusion: Unified Multimodal Understanding and Generation with Masked Discrete Diffusion** `[VLM]` — [2603.06577](https://arxiv.org/abs/2603.06577) | [GitHub](https://github.com/VITA-MLLM/Omni-Diffusion)
  > Omni-Diffusion 是首个完全基于掩码离散扩散模型构建的任意模态到任意模态多模态语言模型，统一了文本、语音和图像的理解与生成。该模型采用统一的掩码离散扩散架构直接建模多模态离散 token 的联合分布，支持双模态及更复杂的多模态任务。与主流自回归 MLLM 相比，Omni-Diffusion 探索了离散扩散作为多模态基础模型骨干的可行性，在多项多模态基准上达到同等甚至更优的性能。

- **InternVL-U: Democratizing Unified Multimodal Models for Understanding, Reasoning, Generation and Editing** `[VLM]` — [2603.09877](https://arxiv.org/abs/2603.09877) | [GitHub](https://github.com/OpenGVLab/InternVL-U)
  > InternVL-U 是一个轻量级 4B 参数统一多模态模型，融合了理解、推理、生成与编辑能力。模型遵循统一上下文建模和模态特定模块化设计原则，将先进 MLLM 与 MMDiT 视觉生成头结合。通过面向高语义密度任务（如文本渲染、科学推理）的数据合成流程，并以 Chain-of-Thought 为推理中心范式对齐用户意图与生成细节。实验表明，尽管仅有 4B 参数，InternVL-U 在生成和编辑任务上一致超越参数量超其 3 倍的统一模型（如 BAGEL-14B）。

- **Test-Driven AI Agent Definition (TDAD): Compiling Tool-Using Agents from Behavioral Specifications** — [2603.08806](https://arxiv.org/abs/2603.08806) | [GitHub](https://github.com/f-labs-io/tdad-paper-code)
  > TDAD（测试驱动 AI Agent 定义）将 Agent 提示视为可编译的制品：工程师提供行为规范，编码 Agent 将其转化为可执行测试，第二个编码 Agent 迭代优化提示直至测试通过。为防止规范博弈，TDAD 引入三机制：可见/隐藏测试分割、语义变异测试以及规范演化场景。在 SpecSuite-Core 基准上，TDAD 在 24 次独立试验中实现 92% 编译成功率，平均隐藏测试通过率 97%，变异得分 86-100%，具备 97% 回归安全性。

- **Decoupling Reasoning and Confidence: Resurrecting Calibration in Reinforcement Learning from Verifiable Rewards** `[RL]` — [2603.09117](https://arxiv.org/abs/2603.09117) | [GitHub](https://github.com/icip-cas/DCPO)
  > RLVR 在显著提升 LLM 推理能力的同时引发了严重的校准退化问题——模型对错误答案过度自信。现有方法将校准目标直接嵌入优化目标，但理论分析表明准确率最大化与校准误差最小化之间存在根本性梯度冲突。为此，本文提出 DCPO，通过系统解耦推理与置信度目标来解决这一矛盾。大量实验表明 DCPO 在保持与 GRPO 相当的准确率的同时，实现了最佳的校准性能，显著缓解了过度自信问题。

- **Reward Prediction with Factorized World States** `[无需训练]` — [2603.09400](https://arxiv.org/abs/2603.09400) | [GitHub](https://github.com/yijunshens/StateFactory)
  > 本文研究如何仅凭结构化世界状态表示实现跨域精确奖励预测。提出 StateFactory，一种将非结构化观测转化为层次对象-属性结构的因子化表示方法，利用语言模型构建层次对象描述，将当前状态与目标状态的语义相似度作为奖励估计。在 RewardPrediction 基准上，StateFactory 零样本结果超越 VLWM-critic 和 LLM-as-a-Judge，在 AlfWorld 和 ScienceWorld 上规划成功率分别提升 +21.64% 和 +12.40%。

- **ReflexiCoder: Teaching Large Language Models to Self-Reflect on Generated Code and Self-Correct It via Reinforcement Learning** `[RL]` — [2603.05863](https://arxiv.org/abs/2603.05863) | [GitHub](https://github.com/juyongjiang/ReflexiCoder)
  > ReflexiCoder 提出一种强化学习框架，将结构化推理轨迹（初始生成、错误感知反思、自我纠正）内化到模型权重中，使 LLM 在推理时无需外部 Oracle 即可自主反思和修正代码。采用 RL-zero 训练范式和细粒度奖励函数优化整个反思-纠正轨迹。ReflexiCoder-8B 在 HumanEval、MBPP、BigCodeBench、LiveCodeBench、CodeForces 等 7 个基准上达到 1.5B-14B 开源模型的 SOTA，单次尝试媲美 GPT-5.1，且推理计算开销减少约 40%。

- **Multi-Head Low-Rank Attention** `[长文本]` — [2603.02188](https://arxiv.org/abs/2603.02188) | [GitHub](https://github.com/SongtaoLiu0823/MLRA)
  > 多头低秩注意力（MLRA）针对 MLA（多头潜在注意力）在分布式解码中的 Tensor Parallelism 分片瓶颈问题，通过支持可分区的潜在状态来实现高效 4 路 TP 解码。MLA 的单一潜在头无法分片，导致每个设备需冗余加载完整 KV 缓存；MLRA 则引入可分区多头低秩状态解决这一问题。大量实验证明 MLRA 在困惑度和下游任务上达到最优，相比 MLA 实现 2.8 倍解码加速，有效提升长文本推理效率。

- **BiCLIP: Domain Canonicalization via Structured Geometric Transformation** `[无需训练]` `[VLM]` — [2603.08942](https://arxiv.org/abs/2603.08942) | [GitHub](https://github.com/QuantitativeImagingLaboratory/BilinearCLIP)
  > BiCLIP 提出一种基于结构化几何变换的领域规范化框架，用于将视觉语言模型适配到专业领域。基于独立训练的 VLM 之间存在规范变换的理论洞察，BiCLIP 假设不同领域的图像特征可通过少量锚点估计的规范化几何变换对齐。BiCLIP 对多模态特征施加有针对性的变换以增强跨模态对齐，参数极少。在 11 个标准基准（含 EuroSAT、DTD、FGVCAircraft）上，BiCLIP 持续达到最优的小样本分类结果，并通过分析所学变换的正交性验证了几何结构对齐是领域适应的关键。

- **Beyond Test-Time Training: Learning to Reason via Hardware-Efficient Optimal Control** `[无需训练]` — [2603.09221](https://arxiv.org/abs/2603.09221) | [GitHub](https://github.com/VITA-Group/TTC-Net)
  > TTC（测试时控制）将推理建模为最优控制问题，引入 Test-Time Control 层在推理时对潜在状态执行有限时域 LQR 规划，在预测前完成规划，并在神经架构内表示价值函数。通过辛分解推导硬件高效 LQR 求解器，以并行化实现最小开销。TTC 层作为适配器集成到预训练 LLM，在 MATH-500 上提升数学推理性能高达 +27.8%，在 AMC 和 AIME 上实现 2-3 倍 Pass@8 改善，展示了将最优控制嵌入架构作为推理机制的有效性与可扩展性。

- **TALON: Test-time Adaptive Learning for On-the-Fly Category Discovery** `[无需训练]` — [2603.08075](https://arxiv.org/abs/2603.08075) | [GitHub](https://github.com/ynanwu/TALON)
  > TALON 提出一种用于在线类别发现的测试时自适应学习框架，在识别已知类别同时从无标签在线流中发现新类别。与现有冻结特征提取器的哈希方法不同，TALON 包含语义感知原型更新（动态精化类原型）和稳定的测试时编码器更新（将新信息直接融入参数空间）两种互补策略，使模型能持续扩充知识库。离线阶段还引入 margin-aware logit 校准以扩大类间间隔、提升类内紧凑性。在标准 OCD 基准上，TALON 显著超越现有哈希方法，在新类准确率上取得显著提升。

## 2026年3月12日

- **OpenClaw-RL: Train Any Agent Simply by Talking** `[RL]` — [2603.10165](https://arxiv.org/abs/2603.10165) | [GitHub](https://github.com/Gen-Verse/OpenClaw-RL)
  > OpenClaw-RL 是一个通用 Agent RL 训练框架，核心观察是每次 Agent 交互产生的"下一状态信号"（用户回复、工具输出、终端/GUI 状态变化）是普适的在线学习来源。框架将下一状态信号分为评估信号（通过 PRM 裁判提取标量奖励）和指令信号（通过 Hindsight-Guided On-Policy Distillation 提取 token 级方向性监督），比纯标量奖励更丰富。异步设计使模型服务、PRM 评判和训练器更新并行进行，支持对话、终端、GUI、SWE 和工具调用等多类型交互的统一策略训练。

- **In-Context Reinforcement Learning for Tool Use in Large Language Models** `[RL]` — [2603.08068](https://arxiv.org/abs/2603.08068) | [GitHub](https://github.com/applese233/ICRL)
  > ICRL（上下文强化学习）提出纯 RL 框架，无需 SFT 冷启动即可训练 LLM 使用外部工具（Python 解释器、搜索引擎等）。核心方法：在 RL rollout 阶段引入 few-shot 上下文示例教导模型调用工具，随训练进行逐步减少示例数量，最终过渡到零样本工具调用。这一渐进式训练策略消除了大量有标注 SFT 数据的需求。在多个推理和工具使用基准上，ICRL 达到 SOTA 性能，证明其作为传统 SFT 流程可扩展、数据高效替代方案的有效性。

- **RetroAgent: From Solving to Evolving via Retrospective Dual Intrinsic Feedback** `[RL]` `[MeM]` — [2603.08561](https://arxiv.org/abs/2603.08561) | [GitHub](https://github.com/zhangxy-2019/RetroAgent)
  > RetroAgent 是一个在线 RL 框架，通过回溯自反思机制使 Agent 不仅能解题更能持续进化。框架产生双重内在反馈：数值内在反馈追踪相对先前尝试的子任务增量完成度；语言内在反馈将可复用的经验蒸馏为记忆缓冲区，通过 SimUtil-UCB 策略（平衡相关性、有效性、探索性）检索利用。在 ALFWorld、WebShop、Sokoban、MineSweeper 四类 Agent 任务上，分别超越 GRPO 训练 Agent +18.3%、+15.4%、+27.1%、+8.9%，展示了强泛化性与测试时自适应能力。

- **CodePercept: Code-Grounded Visual STEM Perception for MLLMs** `[微调]` `[VLM]` — [2603.10757](https://arxiv.org/abs/2603.10757) | [GitHub](https://github.com/TongkunGuan/Qwen-CodePercept)
  > CodePercept 通过系统性缩放分析发现：对于 MLLM 的 STEM 视觉推理，感知缩放的效益持续优于推理缩放，揭示感知才是限制当前能力的核心瓶颈。为此，将代码作为强大感知媒介，构建 ICC-1M 数据集（100 万图像-描述-代码三元组），通过代码基础字幕生成和 STEM 图像到代码翻译两种互补方法增强感知。同时引入 STEM2Code-Eval 新基准，要求模型通过生成图像重建代码进行全面视觉理解评估，提供确定性、可验证的评估。

- **Prism-Δ: Differential Subspace Steering for Prompt Highlighting in Large Language Models** `[无需训练]` — [2603.10705](https://arxiv.org/abs/2603.10705) | [GitHub](https://github.com/YuyaoGe/PRISM-DELTA)
  > PRISM-Δ 是一种提示高亮方法，使 LLM 在生成时优先关注用户指定的文本片段。核心思路是分解正负交叉协方差矩阵的差值以最大化判别能量、消除共享方向，每个注意力头获得连续 softplus 重要性权重（弱但有用的头以降低强度贡献），并扩展到 Value 表示以捕获内容通道信号。在 4 个基准、5 个模型上，PRISM-Δ 在 20 个配置中的 19 个匹配或超越最佳现有方法，相对增益最高 +10.6%，流畅度损失减半，长文本检索场景相对增益最高 +4.8%。

- **Bootstrapping Exploration with Group-Level Natural Language Feedback in Reinforcement Learning** `[RL]` — [2603.04597](https://arxiv.org/abs/2603.04597) | [GitHub](https://github.com/LuckyyySTA/GOLF)
  > GOLF 提出了一种利用组级自然语言反馈引导 LLM Agent 强化学习探索的框架。核心方法是在 rollout 阶段对同一问题的多条轨迹进行跨轨迹对比分析，用 LLM 生成描述成功与失败轨迹差异的自然语言反馈，将该反馈注入后续 rollout 以引导探索。这种组级反馈比逐条奖励信号提供了更丰富的探索指导，有效缓解稀疏奖励下的探索瓶颈。在多个 Agent 任务上，GOLF 显著提升了样本效率和最终性能，尤其在需要多步规划的复杂任务上增益明显。

- **LLM2Vec-Gen: Generative Large Language Models are Strong Text Encoders** `[微调]` — [2603.10913](https://arxiv.org/abs/2603.10913) | [GitHub](https://github.com/McGill-NLP/llm2vec-gen)
  > LLM2Vec-Gen 系统研究了将生成式 LLM 转化为强大文本编码器的方法，挑战了"生成模型不适合做编码器"的惯见。通过在预训练生成 LLM 上施加双向注意力掩码微调，结合对比学习目标，LLM2Vec-Gen 在 MTEB 文本嵌入基准上显著超越同规模的专用编码器模型。研究揭示生成预训练积累的丰富语义知识可被有效迁移至编码任务，为统一生成与理解能力的基础模型提供了实践路径。
