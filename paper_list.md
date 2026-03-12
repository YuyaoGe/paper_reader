## 2026年2月25日

- **PyVision-RL: Forging Open Agentic Vision Models via RL** `[RL]` `[VLM]` — [2602.20739](https://arxiv.org/abs/2602.20739) | [GitHub](https://github.com/agents-x-project/PyVision-RL)
  > 本文提出 PyVision-RL，一个针对开源多模态模型的强化学习训练框架，旨在解决交互折叠（interaction collapse）问题——即模型在RL训练中倾向于减少工具调用和多轮推理。核心贡献包括：（1）过采样-过滤-排序（oversampling-filtering-ranking）的 rollout 策略；（2）累积工具奖励（accumulative tool reward），两者协同防止交互折叠并鼓励多轮工具使用。统一训练流水线下，分别训练了 PyVision-Image 和 PyVision-Video 两个模型。对于视频推理，PyVision-Video 引入按需上下文构建机制，在推理时选择性采样任务相关帧，大幅减少视觉 token 用量。实验表明，该方法在多个图像和视频理解任务上实现了强性能与高效率，证明持续交互与按需视觉处理是可扩展多模态 Agent 的关键。

- **Multi-Vector Index Compression in Any Modality** — [2602.21202](https://arxiv.org/abs/2602.21202) | [GitHub](https://github.com/hanxiangqin/omni-col-press)
  > 本文研究跨模态后期交互（late interaction）的高效多向量检索压缩问题。后期交互是文本、图像、视觉文档等信息检索的主流范式，但其计算和存储开销随文档长度线性增长。本文探索了四种查询无关的文档多向量表示压缩方法：序列缩放、记忆 token、层次化池化，以及新提出的注意力引导聚类（AGC）。AGC 利用注意力机制识别文档最具语义价值的区域作为聚类中心，并加权聚合 token。在覆盖文本（BEIR）、视觉文档（ViDoRe）和视频（MSR-VTT、MultiVENT 2.0）的检索任务上，AGC 一致优于其他参数化压缩方法，同时比非参数化层次聚类更灵活，且性能与完整未压缩索引相当甚至更优。


## 2026年2月27日

- **From Blind Spots to Gains: Diagnostic-Driven Iterative Training for Large Multimodal Models** `[微调]` `[VLM]` `[RL]` — [2602.22859](https://arxiv.org/abs/2602.22859) | [GitHub](https://github.com/hongruijia/DPE)
  > 本文提出诊断驱动渐进演化（DPE），一种针对大型多模态模型（LMM）的持续训练范式，通过螺旋式迭代循环解决静态训练数据无法针对模型能力盲点的问题。DPE 由两个核心组件构成：首先，多个 Agent 对海量未标注多模态数据进行标注和质量控制，结合网络搜索和图像编辑工具生成多样化样本；其次，DPE 将训练失败归因到具体弱点，动态调整数据配比，并引导 Agent 生成针对性弱点数据。每轮迭代后重新诊断更新后的模型，驱动下一轮改进。在 Qwen3-VL-8B-Instruct 和 Qwen2.5-VL-7B-Instruct 上的实验表明，DPE 在 11 个任务上实现持续稳定提升，是一种可扩展的持续 LMM 训练范式。

- **OmniGAIA: Towards Native Omni-Modal AI Agents** `[VLM]` `[微调]` — [2602.22897](https://arxiv.org/abs/2602.22897) | [GitHub](https://github.com/RUC-NLPIR/OmniGAIA)
  > 本文提出 OmniGAIA，一个评估跨视觉、音频和图像模态的全模态 Agent 综合基准，并提出原生全模态基础 Agent OmniAtlas。OmniGAIA 通过全模态事件图方法，从真实世界数据中合成需要跨模态推理和外部工具集成的复杂多跳查询。OmniAtlas 采用工具集成推理范式，通过后见引导树探索策略合成训练轨迹，并利用 OmniDPO 进行细粒度错误纠正，有效增强开源模型的工具使用能力。该工作填补了当前多模态 LLM 主要局限于双模态交互（如视觉-语言）的空缺，迈向真正的全模态通用 AI 助手，在复杂推理和多轮工具执行任务上取得显著进展。

- **Imagination Helps Visual Reasoning, But Not Yet in Latent Space** `[VLM]` `[无需训练]` — [2602.22766](https://arxiv.org/abs/2602.22766) | [GitHub](https://github.com/AI9Stars/CapImagine)
  > 本文研究多模态大语言模型中潜在视觉推理（latent visual reasoning）的有效性，运用因果中介分析（Causal Mediation Analysis）揭示其两大关键断层：（1）输入-潜变量断层：对输入的剧烈扰动几乎不改变潜在 token，说明潜在 token 未能有效关注输入序列；（2）潜变量-答案断层：对潜在 token 的扰动对最终答案影响极小。进一步的探针分析发现潜在 token 编码的视觉信息有限且高度相似。基于此，提出简单替代方案 CapImagine，让模型通过文本形式显式想象。在多个视觉推理任务上，CapImagine 显著优于复杂的潜在空间基线，证明显式文字想象是更优的视觉推理路径。

- **AgentDropoutV2: Optimizing Information Flow in Multi-Agent Systems via Test-Time Rectify-or-Reject Pruning** `[无需训练]` — [2602.23258](https://arxiv.org/abs/2602.23258) | [GitHub](https://github.com/TonySY2/AgentDropoutV2)
  > 本文提出 AgentDropoutV2，一个测试时纠错-或-拒绝剪枝框架，无需重新训练即可动态优化多 Agent 系统（MAS）的信息流。该方法作为主动防火墙，拦截 Agent 输出并使用检索增强纠正器，基于失败驱动的指示池迭代纠正错误；无法修复的输出被剪枝以防止错误传播，后备策略保证系统完整性。在广泛数学任务上，AgentDropoutV2 平均准确率提升 6.3 个百分点，同时展现出鲁棒的泛化能力和自适应性：根据任务难度动态调节纠正力度，利用上下文感知指示器解决多样错误模式，有效降低 MAS 中错误级联传播的风险。


## 2026年3月2日

- **dLLM: Simple Diffusion Language Modeling** `[微调]` — [2602.22661](https://arxiv.org/abs/2602.22661) | [GitHub](https://github.com/ZHZisZZ/dllm)
  > 本文提出 dLLM，一个开源统一框架，旨在整合扩散语言模型（Diffusion LM）的核心组件——训练、推理与评估——并使其易于自定义扩展。当前大量扩散语言模型研究代码分散、缺乏透明实现，导致复现困难。dLLM 通过标准化流程支持用户复现、微调、部署和评估 LLaDA、Dream 等主流开源大型扩散语言模型，同时提供从零构建小型扩散语言模型的最小可复现方案，支持将任意 BERT 风格编码器或自回归 LM 转换为扩散语言模型。此外，作者还发布了相应的模型检查点，大幅降低了研究门槛，有助于加速扩散语言建模领域的后续研究进展。

- **Enhancing Spatial Understanding in Image Generation via Reward Modeling** `[RL]` — [2602.24233](https://arxiv.org/abs/2602.24233) | [GitHub](https://github.com/DAGroup-PKU/SpatialT2I)
  > 本文针对文本到图像生成中空间关系理解不足的问题，提出了一套基于奖励模型的在线强化学习方法。作者首先构建了包含超过 8 万个偏好对的 SpatialReward-Dataset，并在此基础上训练了空间关系奖励模型 SpatialScore，其评估精度超越了主流闭源模型。在此奖励信号的驱动下，通过在线强化学习对图像生成模型进行优化，使其在生成过程中更准确地遵循复杂的空间指令（如"左边/右边/前方/后方"等）。多组实验结果表明，SpatialScore 奖励模型能够带来显著且稳定的空间理解能力提升，验证了奖励建模与在线 RL 相结合在生成模型对齐中的有效性。

- **Compositional Generalization Requires Linear, Orthogonal Representations in Vision Embedding Models** — [2602.24264](https://arxiv.org/abs/2602.24264) | [GitHub](https://github.com/oshapio/necessary-compositionality)
  > 本文从理论层面深入分析了神经网络表征实现组合泛化所必须满足的几何条件。作者提出三项组合泛化的必要条件（可分性、可迁移性、稳定性），并证明这些条件共同决定了表征空间的几何结构：表征必须能对每个概念进行线性分解，且各概念的分量必须相互正交。这一结论为"线性表征假说"提供了严格的理论依据——线性结构并非偶然现象，而是组合泛化能力的必然结果。在实验上，作者在 CLIP、SigLIP、DINO 等视觉模型上进行了验证，发现这些模型的表征确实呈现出部分线性分解和近正交的每概念因子，且该结构的程度与模型的组合泛化能力高度相关。

- **How to Take a Memorable Picture? Empowering Users with Actionable Feedback** `[无需训练]` `[VLM]` — [2602.21877](https://arxiv.org/abs/2602.21877) | [GitHub](https://github.com/laitifranz/MemCoach)
  > 本文提出记忆度反馈（MemFeed）新任务：在用户拍照时，自动为其提供可操作的记忆度提升建议。作者设计了 MemCoach 系统，基于多模态大语言模型（MLLM），以训练无关（training-free）的方式生成自然语言拍摄指导（如"突出面部表情"、"将主体推到前景"等）。方法核心是教师-学生引导策略，通过将模型内部激活向从低记忆度到高记忆度样本中学到的模式对齐来实现改进。为系统评估此任务，作者还构建了 MemBench 评测集，包含按记忆度评分标注的序列化照片。实验结果表明，MemCoach 在多个零样本基线上均取得了一致性性能提升，证明记忆度不仅可以被预测，还可以被教授和指导。

- **InfoNCE Induces Gaussian Distribution** — [2602.24012](https://arxiv.org/abs/2602.24012) | [GitHub](https://github.com/rbetser/InfoNCE-induces-Gaussian-distribution)
  > 本文从理论角度分析了对比学习中 InfoNCE 损失函数对表征分布结构的影响，证明 InfoNCE 目标函数会诱导表征中出现高斯结构。作者在两种互补的理论框架下建立了这一结论：其一，在特定对齐与集中假设下，高维表征的投影在渐近意义上趋近多元高斯分布；其二，在较宽松的假设下，引入一个促进低范数和高熵的小型正则化项同样可以得到类似的渐近结果。基于合成数据集和 CIFAR-10，覆盖多种编码器架构的实验均验证了一致的高斯行为。这一理论视角为对比表征中普遍观测到的高斯性提供了原理性解释，也为后续基于高斯模型的表征分析奠定了基础。

- **Ref-Adv: Exploring MLLM Visual Reasoning in Referring Expression Tasks** `[VLM]` — [2602.23898](https://arxiv.org/abs/2602.23898) | [GitHub](https://github.com/dddraxxx/Ref-Adv)
  > 本文针对现有指代表达理解（REC）数据集存在的捷径问题（表达过短、干扰项不足、冗余描述符可绕过真正的视觉推理），构建了 Ref-Adv 评测集。该数据集专门压制捷径，要求模型仅凭语言上非平凡的表达和必要信息来唯一定位目标，并标注了包含否定等推理层面的类型。作者在词序扰动和描述符删除充分性等维度上进行了消融实验，证明解决 Ref-Adv 需要超越简单线索的真实推理能力。对主流多模态 LLM 的系统性评测显示，尽管这些模型在 RefCOCO 系列上表现出色，在 Ref-Adv 上均出现显著性能下降，揭示了 MLLM 在视觉推理与定位方面的不足，为未来研究指引方向。

- **Accelerating Masked Image Generation by Learning Latent Controlled Dynamics** `[无需训练]` — [2602.23996](https://arxiv.org/abs/2602.23996) | [GitHub](https://github.com/Kaiwen-Zhu/MIGM-Shortcut)
  > 本文针对掩码图像生成模型（MIGM）推理效率低下的问题，提出了 MIGM-Shortcut 加速方法。现有缓存方法试图通过近似未来特征来复用计算，但在激进加速比下存在较大近似误差，原因在于表达能力有限且未考虑采样信息。本文提出训练一个轻量级模型，同时利用历史特征和已采样的离散 token，回归特征演化的平均速度场，从而更准确地预测未来特征。方法应用于两种主流 MIGM 架构，在最先进的 Lumina-DiMOO 上实现了超过 4 倍的文本到图像生成加速，同时保持图像质量，显著推进了掩码图像生成的帕累托前沿。

- **SenCache: Accelerating Diffusion Model Inference via Sensitivity-Aware Caching** `[无需训练]` — [2602.24208](https://arxiv.org/abs/2602.24208) | [GitHub](https://github.com/vita-epfl/SenCache)
  > 本文提出了 SenCache，一个用于加速扩散模型推理的敏感性感知缓存框架。现有缓存方法依赖启发式准则选择缓存/复用时间步，需要大量调优。本文通过分析模型输出对去噪输入（含噪潜变量和时间步）扰动的敏感性，形式化建立了缓存误差的理论依据，并证明该敏感性是预测缓存误差的关键指标。在此基础上，提出动态、逐样本自适应选择缓存时间步的策略 SenCache，属于无需训练的推理加速方法。在 Wan 2.1、CogVideoX 和 LTX-Video 等模型上的实验表明，在相同计算预算下，SenCache 在视觉质量上优于现有缓存方法，为扩散推理加速提供了理论基础与实践指导。

- **DUET-VLM: Dual stage Unified Efficient Token reduction for VLM Training and Inference** `[VLM]` `[微调]` — [2602.18846](https://arxiv.org/abs/2602.18846) | [GitHub](https://github.com/AMD-AGI/DUET-VLM)
  > 本文提出 DUET-VLM，一个面向视觉语言模型（VLM）的即插即用双阶段压缩框架，用于同时降低训练和推理时的视觉 token 开销。框架分两步进行：第一步在视觉编码器输出端进行冗余感知压缩，保留信息丰富的 token；第二步在语言骨干网络中逐层进行文本引导的显著性 token 剪枝，渐进删除信息量低的视觉 token。在 LLaVA-1.5-7B 上，本方法在 67% token 减少下保持超过 99% 的基线精度，在极端 89% 压缩率下仍保持 97% 以上精度，大幅超越现有 SOTA 视觉 token 压缩方法，有效平衡了 VLM 的效率与性能。


## 2026年3月3日

- **OmniLottie: Generating Vector Animations via Parameterized Lottie Tokens** `[VLM]` — [2603.02138](https://arxiv.org/abs/2603.02138) | [GitHub](https://github.com/OpenVGLab/OmniLottie)
  > OmniLottie 是一个从多模态指令生成高质量矢量动画的统一框架。核心贡献在于设计了 Lottie 分词器，将原始 JSON 格式的 Lottie 文件转化为结构化的命令序列，涵盖形状、动画函数和控制参数，从而消除了大量冗余的结构元数据。在此基础上，框架利用预训练的视觉语言模型接受多模态交织指令并生成矢量动画。为推动研究，作者还构建了 MMLottie-2M，一个包含 200 万条专业矢量动画与文本/视觉注释配对的大规模数据集。实验验证了 OmniLottie 能够生成语义贴合、动作生动的矢量动画。

- **OpenAutoNLU: Open Source AutoML Library for NLU** — [2603.01824](https://arxiv.org/abs/2603.01824) | [GitHub](https://github.com/mts-ai/OpenAutoNLU)
  > OpenAutoNLU 是一个面向自然语言理解任务（文本分类和命名实体识别）的开源自动化机器学习库。核心创新是引入了数据感知的训练策略自动选择机制，无需用户手动配置即可根据数据特性选择最优训练方案。库中还集成了数据质量诊断、可配置的分布外检测（OOD Detection）以及大语言模型特性支持，提供极简的低代码 API 接口。该工具特别适合需要快速部署 NLU 系统的工程师和研究者，降低了 NLU 建模的使用门槛。

- **MMR-Life: Piecing Together Real-life Scenes for Multimodal Multi-image Reasoning** `[VLM]` — [2603.02024](https://arxiv.org/abs/2603.02024) | [GitHub](https://github.com/BugMakerzzz/MMR-Life)
  > MMR-Life 是一个评估多模态大模型在真实场景下多图推理能力的综合评测集，包含 2646 道基于 19108 张真实世界图片的多选题，覆盖溯因、类比、因果、演绎、归纳、空间和时间七种推理类型。与现有推理评测不同，MMR-Life 不依赖领域专业知识，而是要求模型综合多张图片进行多样化推理。对 37 个先进模型的评测揭示了显著的挑战性：GPT-5 最高仅达 58% 准确率，且不同推理类型间的表现差异显著。此外，论文还分析了思维长度、推理方式等因素对模型表现的影响。

- **LLaDA-o: An Effective and Length-Adaptive Omni Diffusion Model** `[VLM]` `[长文本]` — [2603.01068](https://arxiv.org/abs/2603.01068) | [GitHub](https://github.com/ML-GSAI/LLaDA-o)
  > LLaDA-o 是一个有效且长度自适应的全能扩散模型，支持多模态理解与生成。该模型基于混合扩散（MoD）框架，将文本理解的离散掩码扩散与视觉生成的连续扩散解耦，同时通过共享的高效注意力主干进行耦合，减少了对固定条件的冗余计算。在此基础上引入以数据为中心的长度自适应策略，无需修改模型架构即可支持多模态场景下的灵活长度解码。在多模态理解与生成基准上取得同类全能扩散模型的最优表现，在 DPG-Bench 文生图任务上达到 87.04 分。

- **Spectral Condition for μP under Width-Depth Scaling** — [2603.00541](https://arxiv.org/abs/2603.00541) | [GitHub](https://github.com/ML-GSAI/Width-Depth-muP)
  > 本文针对宽度与深度联合扩展的基础模型训练问题，提出了统一的谱框架以实现最大更新参数化（μP）。作者引入谱 μP 条件，精确刻画权重范数与每步更新量在宽度和深度上的扩展规律，将此前分散的各类 μP 表述统一为特例。基于该条件推导出覆盖广泛优化器的通用 μP 实现方案，不仅能恢复 SGD 和 AdamW 的现有公式，还自然扩展至更多优化器。GPT-2 语言模型实验验证了所提谱 μP 条件在宽深联合扩展下能保持稳定特征学习并实现超参数迁移。

- **Tool-R0: Self-Evolving LLM Agents for Tool-Learning from Zero Data** `[RL]` — [2602.21320](https://arxiv.org/abs/2602.21320) | [GitHub](https://github.com/emrecanacikgoz/Tool-R0)
  > Tool-R0 提出了一种在零数据假设下通过自博弈强化学习训练通用工具调用 Agent 的框架。从同一基础大模型出发，共同进化 Generator 和 Solver 两个角色，Generator 在 Solver 能力边界处提出有挑战性的任务，Solver 通过真实工具调用来解决这些任务，二者以互补奖励形成自我演化闭环，无需任何预先构建的任务或数据集。在多个工具使用评测集上，Tool-R0 相比基础模型取得了 92.5% 的相对提升，超越了同等设置下的全监督工具调用基线，并揭示了自博弈 LLM Agent 在协同进化、课程动态和扩展行为上的规律。

- **When Does RL Help Medical VLMs? Disentangling Vision, SFT, and RL Gains** `[RL]` `[微调]` `[VLM]` — [2603.01301](https://arxiv.org/abs/2603.01301) | [GitHub](https://github.com/armenjeddi/medbridgerl)
  > 本文通过受控实验系统解耦 RL 在医疗视觉语言模型后训练中的实际贡献，沿视觉、SFT 和 RL 三个维度分析其影响。在 MedMNIST 多模态测试床上，研究者对比了 VLM 视觉塔与纯视觉基线的表现，通过 Accuracy@1 与 Pass@K 量化推理支持度与采样效率，并考察 RL 何时能弥合支持度差距。核心发现：RL 在模型已具备一定正确候选支持（高 Pass@K）时最有效，主要作用是锐化输出分布；而 SFT 的作用是拓展支持度，为 RL 奠定基础。据此提出边界感知配方，在 PMC 医疗 VQA 子集上 RL 后训练后，在六个医疗 VQA 基准上取得强劲平均表现。

- **Spectral Attention Steering for Prompt Highlighting** `[无需训练]` — [2603.01281](https://arxiv.org/abs/2603.01281) | [GitHub](https://github.com/waylonli/SEKA)
  > 注意力引导是控制模型关注点的重要技术，但现有方法需显式存储完整注意力矩阵，与 FlashAttention 等内存高效实现不兼容。本文提出 SEKA（谱编辑键放大），一种免训练的引导方法，通过在注意力计算前直接编辑键嵌入来绕过该限制：利用谱分解将键嵌入引导至可放大特定 token 注意力分数的潜在方向。进一步提出自适应变体 AdaSEKA，通过免训练路由机制基于提示语义意图动态组合多个专家子空间。实验表明，两种方法在标准引导基准上显著优于强基线，同时引入极低的延迟和内存开销，并与优化注意力实现完全兼容。

- **Half-Truths Break Similarity-Based Retrieval** `[微调]` `[VLM]` — [2602.23906](https://arxiv.org/abs/2602.23906) | [GitHub](https://github.com/kargibora/CS-CLIP)
  > 本文揭示了 CLIP 类双编码器在图文相似度计算中存在"半真实"漏洞：在正确描述后附加错误细节，相似度分数不降反升。在 COCO 数据集上，CLIP 仅在 40.6% 的情况下偏好正确的较短描述，关系描述错误时降至 32.9%。作者将该问题归因于对比训练仅对齐整句而未显式约束实体和关系的粒度接地。为此提出 CS-CLIP，将标题分解为实体和关系单元，为每个单元构建最小化编辑的干扰样本，并微调模型使正确单元得分高于干扰样本。CS-CLIP 将半真实准确率提升至 69.3%，在组合理解基准上平均提升 5.7 分。

- **Reasoning Core: A Scalable Procedural Data Generation Suite for Symbolic Pre-training and Post-Training** `[RL]` `[微调]` — [2603.02208](https://arxiv.org/abs/2603.02208) | [GitHub](https://github.com/sileod/reasoning_core)
  > Reasoning Core 是一个可扩展的程序化符号推理数据生成套件，用于扩展语言模型的推理边界。与依赖固定谜题或模板的现有生成器不同，它覆盖了 PDDL 规划、一阶逻辑、上下文无关文法解析、因果推理（贝叶斯网络）和方程组五个核心形式推理域，每类任务均配合外部求解器进行严格验证，并支持连续难度控制以实现课程学习。生成样本可选地包含求解器推导的推理链，支持从预训练阶段即开始监督训练，同一接口也可提供 RL 可验证奖励函数。预训练混入 Reasoning Core 数据可提升下游推理表现同时不损害语言建模质量，且 GPT-5 等前沿模型在零样本评估上仍面临显著挑战。

- **RAISE: Requirement-Adaptive Evolutionary Refinement for Training-Free Text-to-Image Alignment** `[无需训练]` — [2603.00483](https://arxiv.org/abs/2603.00483) | [GitHub](https://github.com/LiyaoJiang1998/RAISE)
  > RAISE 是一个免训练的自适应进化框架，用于提升文生图扩散模型的提示对齐质量。它将图像生成建模为需求驱动的自适应扩展过程，在推理时对候选图像种群进行演化，支持提示重写、噪声重采样和指令编辑等多种精化动作，并通过结构化需求清单对结果进行验证，仅对未满足项分配额外计算资源。这实现了与语义复杂度匹配的自适应测试时扩展。在 GenEval 和 DrawBench 上，RAISE 实现最优对齐分数（GenEval 综合 0.94），同时将生成样本数减少 30-40%，VLM 调用次数减少 80%，展示了高效、可泛化的多轮自我改进能力。

- **CC-VQA: Conflict- and Correlation-Aware Method for Mitigating Knowledge Conflict in Knowledge-Based Visual Question Answering** `[无需训练]` `[VLM]` — [2602.23952](https://arxiv.org/abs/2602.23952) | [GitHub](https://github.com/cqu-student/CC-VQA)
  > CC-VQA 针对知识型视觉问答中检索信息与模型参数知识间冲突问题提出了一个免训练的冲突与相关性感知方法。现有方法忽视了视觉信息在冲突中的关键作用，且受冗余检索上下文干扰。CC-VQA 包含两个核心组件：（1）视觉中心的上下文冲突推理，对内部和外部知识上下文进行视觉语义冲突分析；（2）相关性引导的编码与解码，通过位置编码压缩低相关语句，并使用相关性加权冲突评分进行自适应解码。在 E-VQA、InfoSeek 和 OK-VQA 三个基准上，CC-VQA 相较现有方法实现了 3.3% 到 6.4% 的绝对准确率提升。

- **ProtegoFed: Backdoor-Free Federated Instruction Tuning with Interspersed Poisoned Data** `[微调]` — [2603.00516](https://arxiv.org/abs/2603.00516) | [GitHub](https://github.com/dongdongzhaoUP/ProtegoFed)
  > ProtegoFed 是首个能够处理分散在所有客户端中毒样本的无后门联邦指令微调框架。研究发现，当中毒样本分散于良性客户端时，现有防御方法均失效。为解决这一问题，论文发现频域梯度是区分中毒样本的鲁棒信号，并提出全局二次聚类机制以支持跨客户端协作识别中毒样本。ProtegoFed 在训练中准确检测、移除并净化分散的中毒数据。在四个联邦学习数据集上，中毒样本识别率达 92% 至 100%，攻击成功率降至接近零，同时保持主任务效用。

- **Planning from Observation and Interaction** `[RL]` — [2602.24121](https://arxiv.org/abs/2602.24121) | [GitHub](https://github.com/UWRobotLearning/mpail2)
  > 本文研究仅凭任务执行观察学习（无奖励、无示教者动作）的 Agent 训练问题，提出了一种基于规划的逆强化学习（IRL）算法，仅从观察与交互中构建世界模型。全程在真实世界中进行实验，在不到一小时内从零开始学习基于图像的操作任务，无需任何先验知识、预训练或额外数据。同时验证了学得的世界模型具备在线迁移学习能力。与 IRL、RL 及行为克隆等假设更严格的方法相比，该方法展示了显著更高的样本效率和成功率，为基于观察的在线世界建模与规划提供了实用路径。

- **Monocular Mesh Recovery and Body Measurement of Female Saanen Goats** — [2602.19896](https://arxiv.org/abs/2602.19896) | [GitHub](https://github.com/bojin-nwafu/Female-Saanen-Goats)
  > 本文针对萨能奶山羊体型测量问题提出了单目网格重建方法。首先构建了包含 55 只雌性萨能羊八视角 RGBD 视频的 FemaleSaanenGoat 数据集，利用多视角 DynamicFusion 将嘈杂非刚性点云融合为高保真 3D 扫描。在此基础上开发了 SaanenGoat 参数化 3D 体型模型，包含 41 个骨骼关节和增强的乳房表征，形状空间涵盖 48 只山羊的个体差异。借助该模型实现单视角 RGBD 输入的高精度三维重建，自动测量体长、体高、胸宽、胸围、臀宽、臀高六项关键体尺。实验表明该方法在 3D 重建和体尺测量上均超越基线，为精准畜牧业提供了新范式。


## 2026年3月4日

- **Utonia: Toward One Encoder for All Point Clouds** `[VLM]` — [2603.03283](https://arxiv.org/abs/2603.03283) | [GitHub](https://github.com/Pointcept/Utonia)
  > Utonia 是首个跨多域联合训练的自监督点云 Transformer 编码器，覆盖遥感、户外激光雷达、室内 RGB-D、物体级 CAD 模型以及 RGB-only 视频提升的点云等多个感知域。尽管各域在传感器几何、密度和先验知识上差异显著，Utonia 仍能学习出跨域一致的表征空间，且多域联合训练时涌现出单域训练中未出现的有趣行为。此外，Utonia 的表征也能提升多模态推理能力，在视觉语言模型中集成后在空间推理任务上取得收益。实验验证了该框架在 AR/VR、自动驾驶等下游应用中的广泛潜力。

- **BeyondSWE: Can Current Code Agent Survive Beyond Single-Repo Bug Fixing?** — [2603.03194](https://arxiv.org/abs/2603.03194) | [GitHub](https://github.com/AweAI-Team/BeyondSWE)
  > BeyondSWE 是一个超越单仓库 Bug 修复的代码 Agent 综合评测框架，从解决范围和知识范围两个维度扩展现有评测，包含 500 个真实世界实例，覆盖跨仓库推理、领域专业化问题解决、依赖驱动迁移和全仓库生成四类场景。实验揭示了显著的能力差距：即便是最先进的前沿模型成功率也低于 45%，且没有单一模型能在所有任务类型上保持一致表现。为系统研究外部知识的作用，作者还开发了 SearchSWE 框架，将深度检索与编码能力结合，结果表明检索增强的收益并不稳定，在部分情况下甚至会降低性能，揭示了模拟开发者工作流的固有挑战。

- **PRISM: Pushing the Frontier of Deep Think via Process Reward Model-Guided Inference** `[无需训练]` — [2603.02479](https://arxiv.org/abs/2603.02479) | [GitHub](https://github.com/Rituraj003/PRISM)
  > PRISM 是一种过程奖励模型（PRM）引导的推理时推断算法，用于改进 DEEPTHINK 系统中的种群增强瓶颈。现有框架在推断时缺乏可靠正确性信号，导致更深层推导放大错误并抑制正确少数解。PRISM 将候选解视为 PRM 定义能量景观中的粒子，通过分数引导的重采样和随机精化重塑种群，在保持多样性的同时将概率质量集中于高质量推理；聚合阶段同样由步级验证引导。在数学和科学基准上，PRISM 以 gpt-oss-20b 在 AIME25、HMMT25、GPQA Diamond 分别达到 90.0%、75.4%、71.4%，匹配或超越 gpt-oss-120b，且通常处于计算-精度帕累托前沿。

- **Humans and LLMs Diverge on Probabilistic Inferences** — [2602.23546](https://arxiv.org/abs/2602.23546) | [GitHub](https://github.com/McGill-NLP/probabilistic-reasoning)
  > 本文系统研究了人类与大语言模型在概率推断上的差异。研究者构建了 ProbCOPA 数据集，包含 210 条手工设计的概率推断样例，每条由 25-30 名人类参与者标注推断可能性，揭示了人类判断的连续性和差异性。对比八个前沿推理 LLM 的输出后发现，模型一致性地无法产生类人的概率分布。进一步分析 LLM 推理链，发现模型在评估此类推断时存在共同的推理模式缺陷。研究结果揭示了人类与 LLM 之间持续存在的认知差异，强调了在非确定性场景下评估推理能力的必要性。

- **Surgical Post-Training: Cutting Errors, Keeping Knowledge** `[微调]` `[RL]` — [2603.01683](https://arxiv.org/abs/2603.01683) | [GitHub](https://github.com/Visual-AI/SPoT)
  > SPoT（手术式后训练）是一种在提升 LLM 推理能力的同时防止灾难性遗忘的新范式。论文从理论和实验两方面揭示了 DPO 奖励估计中内在正则化机制的关键作用。SPoT 由两个核心组件组成：（1）数据修正流水线，利用 Oracle 通过最小化编辑外科式修正错误步骤，生成接近模型当前分布的数据；（2）基于奖励的二元交叉熵目标，将推理正确性建模为二分类问题，实施解耦监督信号。仅用 4K 条修正数学数据对，SPoT 在域内和 OOD 任务上平均提升 Qwen3-8B 准确率 6.2%，在 8×H800 GPU 上仅需 28 分钟训练。

- **Spilled Energy in Large Language Models** `[无需训练]` — [2602.18671](https://arxiv.org/abs/2602.18671) | [GitHub](https://github.com/OmnAI-Lab/spilled-energy)
  > 本文将 LLM 最终 softmax 分类器重新诠释为能量函数模型（EBM），将序列到序列的概率链分解为推断时多个交互 EBM。由此引入"能量溢出"概念，实验表明其与事实性错误、偏差和失败高度相关。与现有方法不同，作者无需训练探针分类器或激活消融，仅从输出 logits 推导出两个完全免训练的指标：溢出能量（捕捉理论上应匹配的连续生成步骤间的能量值差异）和边际化能量（单步可测量）。在九个基准上，对包括 LLaMA、Mistral、Gemma 等主流 LLM 的评测证明了该方法在幻觉检测上的鲁棒性和跨任务泛化能力。

- **InfoPO: Information-Driven Policy Optimization for User-Centric Agents** `[RL]` — [2603.00656](https://arxiv.org/abs/2603.00656) | [GitHub](https://github.com/kfq20/InfoPO)
  > InfoPO 针对现实中用户请求常存在信息不足的问题，提出了信息驱动的策略优化框架。现有多轮 GRPO 方法依赖轨迹级奖励，存在信用分配问题和 rollout 组内优势信号不足等缺陷。InfoPO 将多轮交互建模为主动降低不确定性的过程，计算信息增益奖励以信任那些可测量地改变 Agent 后续动作分布的交互轮次，再通过自适应方差门控融合与任务结果结合。在意图澄清、协作编程、工具增强决策等多类任务上，InfoPO 持续优于提示工程和多轮 RL 基线，同时在用户模拟器偏移和环境交互任务上也表现出良好的鲁棒性与泛化性。

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
