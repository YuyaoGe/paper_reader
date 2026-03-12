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
