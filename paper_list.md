## 2026年1月19日

- **RubricHub: A Comprehensive and Highly Discriminative Rubric Dataset via Automated Coarse-to-Fine Generation** `[RL]` `[微调]` — [2601.08430](https://arxiv.org/abs/2601.08430) | [GitHub](https://github.com/teqkilla/RubricHub)
  > RubricHub 针对开放式文本生成缺乏真值标准的问题，提出一套自动化「由粗到细的 Rubric 生成框架」。该框架融合原则引导的合成、多模型聚合与难度演进三步骤，生成具有高判别力的精细化评分标准。基于此框架构建了包含约 11 万条跨领域样本的大规模数据集 RubricHub，并设计了两阶段后训练流程：基于 Rubric 的拒绝采样微调（RuFT）与强化学习（RuRL）。实验表明，以 Qwen3-14B 为骨干的后训练模型在 HealthBench 上取得 69.3 分的 SOTA 成绩，超越 GPT-5 等闭源前沿模型。数据合成代码已开源。

- **BAPO: Boundary-Aware Policy Optimization for Reliable Agentic Search** `[RL]` — [2601.11037](https://arxiv.org/abs/2601.11037) | [GitHub](https://github.com/Liushiyu-0709/BAPO-Reliable-Search)
  > 基于 RL 的智能体搜索系统在准确性上取得显著进展，但存在「可靠性盲区」：即使证据不足或推理触及边界，模型也很少表达「我不知道」（IDK）。本文提出 BAPO（边界感知策略优化），通过两个核心组件解决这一问题：(i) 基于分组的边界感知奖励，仅在推理真正触及上限时才激励 IDK 响应；(ii) 自适应奖励调节器，在早期探索阶段暂停该奖励，防止模型将 IDK 用作捷径。在四个基准上的实验表明，BAPO 在不损失准确率的前提下显著提升了智能体搜索的整体可靠性。

- **Entropy Sentinel: Continuous LLM Accuracy Monitoring from Decoding Entropy Traces in STEM** `[无需训练]` — [2601.09001](https://arxiv.org/abs/2601.09001) | [GitHub](https://github.com/pmemoli/Entropy-Sentinel)
  > 本文研究是否能用推理时信号估算 LLM 在不同领域的 slice 级准确率。对每个响应，从最终层 next-token 概率计算输出熵特征，并以多种统计量加以汇总；轻量分类器预测实例正确性，平均预测概率得出领域级准确率估计。在 10 个 STEM 推理基准上进行穷举 train/test 组合实验，横跨 9 个 LLM（6 个系列，3B–20B）。结果表明输出熵特征往往能追踪泛化准确率，多个模型呈现近单调领域排序，为可扩展的性能监控和目标数据采集提供了可访问的信号。

- **ProFit: Leveraging High-Value Signals in SFT via Probability-Guided Token Selection** `[微调]` — [2601.09195](https://arxiv.org/abs/2601.09195) | [GitHub](https://github.com/Utaotao/ProFit)
  > 传统 SFT 强制对齐单一参考答案，导致模型在非核心表达上过拟合。本文揭示 token 概率与语义重要性的内在联系：高概率 token 承载核心逻辑框架，低概率 token 多为可替换表达。基于此，提出 ProFit，选择性地屏蔽低概率 token 以防止表层过拟合。与耗费大量资源引入多参考答案不同，ProFit 以轻量方式从根本上缓解单一参考过拟合问题。在通用推理与数学基准上的大量实验确认，ProFit 相比传统 SFT 基线持续取得更好的效果。

- **Language of Thought Shapes Output Diversity in Large Language Models** `[无需训练]` — [2601.11227](https://arxiv.org/abs/2601.11227) | [GitHub](https://github.com/iNLP-Lab/Multilingual-LoT-Diversity)
  > 本文揭示控制模型「思维语言」（Language of Thought）是提升 LLM 输出多样性的新结构化来源。初步研究显示不同思维语言在模型思维空间中占据截然不同的区域。基于此，研究了多语言思维下的两种重复采样策略，并在输出统一为英语的条件下评估多样性。大量实验表明，将思维语言从英语切换为非英语语言可持续提高输出多样性，且思维空间中与英语距离越远的语言增益越大。跨语言聚合样本进一步带来组合效应，在多元文化对齐场景中拓宽了文化知识与价值取向的覆盖范围。

- **PersonalAlign: Hierarchical Implicit Intent Alignment for Personalized GUI Agent with Long-Term User-Centric Records** `[MeM]` `[VLM]` — [2601.09636](https://arxiv.org/abs/2601.09636) | [GitHub](https://github.com/JiuTian-VL/PersonalAlign)
  > 本文提出 PersonalAlign，一种面向个性化 GUI 智能体的层次化隐式意图对齐新任务，要求智能体利用长期用户记录作为持久上下文，解析模糊指令中被省略的偏好并主动预判用户意图。为此引入 AndroidIntent 基准（含 775 条偏好意图与 215 条常规意图），并设计 HIM-Agent（层次意图记忆智能体），该智能体维护持续更新的个人记忆并分层组织用户偏好与常规行为。对 GPT-5、Qwen3-VL、UI-TARS 等主流 GUI 智能体的评测表明，HIM-Agent 将执行性能与主动性能分别提升了 15.7% 和 7.3%。


## 2026年1月20日

- **Multiplex Thinking: Reasoning via Token-wise Branch-and-Merge** `[RL]` — [2601.08808](https://arxiv.org/abs/2601.08808) | [GitHub](https://github.com/GMLR-Penn/Multiplex-Thinking)
  > 本文提出 Multiplex Thinking，一种随机软推理机制，用于改进大型语言模型的链式思考（CoT）推理效率。核心方法是在每个推理步骤中采样 K 个候选 token，并将其嵌入聚合为单个连续的「多路 token」，从而在不增加序列长度的情况下表示多种可能的后续步骤。该机制兼容标准离散生成的词表嵌入先验和采样动态，并可直接使用 on-policy 强化学习进行优化。当模型置信度高时，多路 token 接近离散，与标准 CoT 一致；置信度低时则紧凑地表示多种可能路径。在多个数学推理基准上，Multiplex Thinking 在 Pass@1 至 Pass@1024 范围内均优于强基线，同时产生更短的序列。

- **NAACL: Noise-AwAre Verbal Confidence Calibration for LLMs in RAG Systems** `[微调]` — [2601.11004](https://arxiv.org/abs/2601.11004) | [GitHub](https://github.com/HKUST-KnowComp/NAACL)
  > 本文聚焦于检索增强生成（RAG）系统中大语言模型的置信度校准问题，指出噪声检索上下文会严重导致模型过度自信。作者系统研究了多个基准上的校准表现，提出「噪声感知置信度校准规则」（NAACL Rules），并设计了一套噪声感知监督微调框架（NAACL），利用有针对性的监督信号让模型内化对噪声的感知能力。实验结果表明，该方法在域内和域外场景下均能稳定降低期望校准误差（ECE），有效提升 RAG 系统中 LLM 输出的认知可靠性，增强实际部署中事实类应用的可信度。

- **Medical SAM3: A Foundation Model for Universal Prompt-Driven Medical Image Segmentation** `[微调]` `[VLM]` — [2601.10880](https://arxiv.org/abs/2601.10880) | [GitHub](https://github.com/AIM-Research-Lab/Medical-SAM3)
  > 本文提出 Medical SAM3，一个通用提示驱动的医学图像分割基础模型，通过对 SAM3 进行全参数微调得到。研究发现原版 SAM3 在医学数据上性能大幅退化，主要依赖真值边界框等强空间先验。为此，作者在涵盖 10 种影像模态的 33 个数据集上对 SAM3 进行完整微调，使模型获得鲁棒的领域特定表示，同时保留提示驱动的灵活性。仅使用文本提示（如「息肉」「肿瘤」）时，Medical SAM3 在 7 个未见外部数据集的零样本分割中将 Dice 分数从 11.9% 大幅提升至 73.9%，在器官、影像模态和维度方面均展示出显著性能提升。

- **The Assistant Axis: Situating and Stabilizing the Default Persona of Language Models** `[无需训练]` — [2601.10387](https://arxiv.org/abs/2601.10387) | [GitHub](https://github.com/safety-research/assistant-axis)
  > 本文研究大语言模型人格空间的结构，通过提取对应多种角色原型的激活方向，发现其主成分是一个「助手轴」（Assistant Axis），衡量模型在多大程度上处于默认助手模式。向助手方向激活引导可强化有益无害行为；反向引导则使模型倾向扮演其他身份，极端情况下会产生神秘、戏剧化的表达风格。该轴同样存在于预训练模型中。沿助手轴的偏差可预测「人格漂移」现象，即模型滑入有害或奇异行为。将激活限制在助手轴的固定区域可稳定模型行为，对抗对抗性人格越狱攻击同样有效。

- **YaPO: Learnable Sparse Activation Steering Vectors for Domain Adaptation** `[微调]` — [2601.08441](https://arxiv.org/abs/2601.08441) | [GitHub](https://github.com/MBZUAI-Paris/YaPO)
  > 本文提出 YaPO（Yet another Policy Optimization），一种无参考方法，在稀疏自编码器（SAE）的潜在空间中学习稀疏激活引导向量，用于大语言模型的精细化对齐。针对密集引导向量因神经元多义性导致的特征纠缠问题，YaPO 通过 DPO 风格优化稀疏编码来产生解耦、可解释且高效的引导方向。实验表明，YaPO 收敛更快、训练更稳定，在文化对齐、幻觉抑制、越狱防御等场景均优于密集基线，且在 MMLU 上无可测量的知识退化。YaPO 提供了一个通用配方，适用于 LLM 的高效、稳定、精细对齐。

- **Spurious Rewards Paradox: Mechanistically Understanding How RLVR Activates Memorization Shortcuts in LLMs** `[RL]` — [2601.11061](https://arxiv.org/abs/2601.11061) | [GitHub](https://github.com/idwts/How-RLVR-Activates-Memorization-Shortcuts)
  > 本文研究带可验证奖励的强化学习（RLVR）中的「虚假奖励悖论」：即使在虚假或错误奖励下，Qwen 2.5 等模型也能取得显著性能提升。通过分析发现「困惑度悖论」——虚假 RLVR 导致答案 token 困惑度下降而提示端连贯性退化，表明模型绕过推理转向记忆。借助路径修补、Logit Lens、JSD 分析和神经微分方程，作者揭示了隐藏的「锚适配器电路」：中间层（L18-20）的功能锚触发记忆检索，后层（L21+）的结构适配器完成表示转换。通过缩放特定 MLP 键，可双向因果控制数据污染驱动的性能，为识别和缓解 RLVR 微调模型中的数据污染提供了机械可解释路径。


## 2026年1月21日

- **Agentic-R: Learning to Retrieve for Agentic Search** `[微调]` `[MeM]` — [2601.11888](https://arxiv.org/abs/2601.11888) | [GitHub](https://github.com/8421BCD/Agentic-R)
  > 本文提出面向Agentic搜索的检索器训练框架Agentic-R。不同于传统单轮RAG检索器仅依赖局部查询-段落相关性，Agentic-R同时利用局部相关性和全局答案正确性来衡量段落价值。框架引入迭代训练策略，搜索智能体与检索器相互优化：智能体产生的高质量查询持续改进检索器，检索器反过来提升智能体的搜索能力。在七个单跳和多跳QA基准上的实验表明，Agentic-R在多个搜索智能体上均显著优于强基线，验证了专为多轮Agentic搜索设计的检索器的有效性。

- **UniX: Unifying Autoregression and Diffusion for Chest X-Ray Understanding and Generation** `[VLM]` `[微调]` — [2601.11522](https://arxiv.org/abs/2601.11522) | [GitHub](https://github.com/ZrH42/UniX)
  > UniX是一个面向胸部X光的统一医学基础模型，将视觉理解（自回归分支）与高保真生成（扩散分支）解耦，通过跨模态自注意力机制让生成过程受理解特征动态引导，实现两任务协同。结合严格数据清洗和多阶段训练策略，UniX在理解任务（Micro-F1）上提升46.1%，生成质量（FD-RadDino）提升24.2%，参数量仅为LLM-CXR的四分之一，性能接近任务专用模型，建立了医学图像理解与生成协同的可扩展范式。

- **DARC: Decoupled Asymmetric Reasoning Curriculum for LLM Evolution** `[微调]` `[RL]` — [2601.13761](https://arxiv.org/abs/2601.13761) | [GitHub](https://github.com/RUCBM/DARC)
  > DARC（解耦非对称推理课程）是一种稳定LLM自我进化的两阶段框架。第一阶段训练Questioner根据难度级别和外部语料生成难度校准的问题；第二阶段采用非对称自蒸馏机制，文档增强的教师模型生成高质量伪标签来监督无文档访问权限的学生Solver，消除自生成标签带来的bootstrapping误差。实验表明DARC与模型无关，在三个骨干模型和九个推理基准上平均提升10.9分，在无需人工标注的情况下接近全监督模型性能。

- **Which Reasoning Trajectories Teach Students to Reason Better? A Simple Metric of Informative Alignment** `[微调]` — [2601.14249](https://arxiv.org/abs/2601.14249) | [GitHub](https://github.com/UmeanNever/RankSurprisalRatio)
  > 本文提出Rank-Surprisal Ratio（RSR），一种衡量推理轨迹对学生模型适合性的简单指标，解决知识蒸馏中「更强教师并不总产生更好学生」的问题。RSR定义为轨迹平均token排名与平均负对数似然之比，同时捕捉对齐度（低绝对概率）和信息量（相对高排名token），在五个学生模型和11个教师的实验中与训练后性能高度相关（平均Spearman 0.86），优于现有指标，在轨迹选择和教师选择中均具实用价值。

- **InT: Self-Proposed Interventions Enable Credit Assignment in LLM Reasoning** `[RL]` `[微调]` — [2601.14209](https://arxiv.org/abs/2601.14209) | [GitHub](https://github.com/intervention-training/int)
  > 本文针对RL训练中仅对最终结果分配信用导致的步级错误归因问题，提出Intervention Training（InT）。模型通过识别推理轨迹中第一个错误步并提出单步干预来实现细粒度信用归因，利用参考解验证（验证比生成容易）构建SFT数据，将错误精准定位到特定步骤。InT得到的模型作为RL的更好初始化，在4B参数模型上于IMO-AnswerBench提升约14%，超越更大规模的开源模型如gpt-oss-20b。

- **FutureOmni: Evaluating Future Forecasting from Omni-Modal Context for Multimodal LLMs** `[VLM]` `[微调]` — [2601.13836](https://arxiv.org/abs/2601.13836) | [GitHub](https://github.com/OpenMOSS/FutureOmni)
  > FutureOmni是首个专门评估多模态LLM从视听环境预测未来事件能力的基准，包含919个视频和1034个多选QA对，覆盖8个主要领域。评估13个全模态和7个纯视频模型发现，当前系统在音视频未来预测上表现欠佳，最佳准确率64.8%（Gemini 3 Flash）。作者进一步提出全模态未来预测（OFF）训练策略，构建7K样本指令微调数据集，在FutureOmni及主流音视频/纯视频基准上均显著提升预测和泛化能力。

- **FantasyVLN: Unified Multimodal Chain-of-Thought Reasoning for Vision-Language Navigation** `[VLM]` `[微调]` — [2601.13976](https://arxiv.org/abs/2601.13976) | [GitHub](https://github.com/Fantasy-AMAP/fantasy-vln)
  > FantasyVLN提出统一隐式推理框架用于视语言导航（VLN），兼顾CoT推理优势而无需显式token开销。训练阶段利用预训练Visual AutoRegressor（VAR）将想象的视觉token编码到紧凑潜在空间，在统一多CoT策略下联合学习文本、视觉和多模态CoT模式。推理时模型直接映射指令到动作，同时享有推理感知表征。LH-VLN实验表明，与显式CoT方法相比，推理延迟降低一个数量级，同时提升成功率和效率。

- **On the Evidentiary Limits of Membership Inference for Copyright Auditing** `[微调]` — [2601.12937](https://arxiv.org/abs/2601.12937) | [GitHub](https://github.com/kiraz-ai/sage-sps-mia)
  > 本文研究成员推断攻击（MIA）作为版权审计证据的可靠性局限。作者提出SAGE（基于稀疏自编码器引导的改写框架），在保持语义内容的同时改变训练数据词法结构，用于模拟对抗性版权争议场景。实验表明，在SAGE生成的改写版本上微调的模型可使最先进MIA准确率显著下降，表明MIA信号对语义保持变换不鲁棒，在对抗设置下不足以独立作为LLM版权审计机制。

- **SciCoQA: Quality Assurance for Scientific Paper--Code Alignment** `[长文本]` — [2601.12910](https://arxiv.org/abs/2601.12910) | [GitHub](https://github.com/ukplab/scicoqa)
  > SciCoQA是用于检测科学论文与代码库间差异的数据集，包含611条论文-代码不一致样本（81条真实，530条合成），涵盖AI、物理、定量生物等领域。数据集结合GitHub issue和可重现性论文构建，并提出合成数据生成方法扩展规模。评估21个LLM的结果揭示该任务的高难度，尤其对涉及省略论文细节、长上下文输入的案例；最优模型GPT-5仅能检测45.7%的真实世界差异。


## 2026年1月22日

- **Paper2Rebuttal: A Multi-Agent Framework for Transparent Author Response Assistance** `[无需训练]` — [2601.14171](https://arxiv.org/abs/2601.14171) | [GitHub](https://github.com/AutoLab-SAI-SJTU/Paper2Rebuttal)
  > RebuttalAgent 是首个将学术评审回复生成重构为「以证据为中心的规划任务」的多智能体框架。系统将审稿人反馈分解为原子性关切点，动态构建混合上下文（摘要+高保真原文），并集成自主外部搜索模块以引用文献证据。生成前先构造可检查的响应计划，确保每个论点都锚定于内部或外部证据。在提出的 RebuttalBench 上，该方法在覆盖率、忠实度和策略一致性方面超越强基线，为同行评审流程提供透明可控的辅助工具。

- **GutenOCR: A Grounded Vision-Language Front-End for Documents** `[VLM]` `[微调]` — [2601.14490](https://arxiv.org/abs/2601.14490) | [GitHub](https://github.com/Roots-Automation/GutenOCR)
  > GutenOCR 是通过微调 Qwen2.5-VL-3B 和 Qwen2.5-VL-7B 获得的接地式 OCR 前端模型族，以统一的提示接口暴露阅读、检测和定位能力。训练数据涵盖商业文档、科学文章和合成定位数据，支持全页及局部阅读、行/段落级边界框以及「x 在哪里？」条件查询。GutenOCR-7B 在 10.5K 张保留页上将其 Qwen2.5-VL-7B 骨干的综合接地 OCR 分数从 0.40 提升至 0.82，在 Fox 和 OmniDocBench v1.5 上显著改善区域/行级 OCR 及文本检测召回率。

- **Behavior Knowledge Merge in Reinforced Agentic Models** `[RL]` `[微调]` — [2601.13572](https://arxiv.org/abs/2601.13572) | [GitHub](https://github.com/xiangchi-yuan/mrl)
  > 本文提出 Reinforced Agent Merging（RAM），一种专为 RL 训练的智能体模型设计的分布感知合并框架。现有 SFT 风格合并方法在 RL 模型上表现欠佳，根源在于 RL 产生的任务向量高度稀疏且异质，简单全局平均会稀释关键任务特定行为。RAM 将参数更新解耦为共享和任务特有成分，对共享部分取平均，对唯一成分选择性保留并重新缩放。跨多个智能体域和模型架构的实验表明，RAM 不仅超越合并基线，还能释放智能体间的协同潜力，使融合后的通用模型超越各自专用模型的性能。

- **Numina-Lean-Agent: An Open and General Agentic Reasoning System for Formal Mathematics** `[无需训练]` — [2601.14027](https://arxiv.org/abs/2601.14027) | [GitHub](https://github.com/project-numina/numina-lean-agent)
  > 本文提出直接将通用编码 Agent 用于形式化数学推理的范式，无需针对特定任务训练形式化证明器。Numina-Lean-Agent 结合 Claude Code 与 Numina-Lean-MCP，实现与 Lean 的自主交互、相关定理检索以及非形式化辅助推理。使用 Claude Opus 4.5 作为基础模型，在 Putnam 2025 上解决了全部 12 题（12/12），与最优闭源系统持平。还成功协助数学家形式化了 Brascamp-Lieb 定理，验证了该范式超越基准评测的通用性。

- **Render-of-Thought: Rendering Textual Chain-of-Thought as Images for Visual Latent Reasoning** `[VLM]` `[无需训练]` — [2601.14750](https://arxiv.org/abs/2601.14750) | [GitHub](https://github.com/TencentBAC/RoT)
  > Render-of-Thought（RoT）是首个将文本推理链渲染为图像以显式化潜在推理过程的框架。通过利用 VLM 的视觉编码器作为语义锚点，将视觉嵌入与文本空间对齐，实现即插即用无需额外预训练。在数学和逻辑推理任务上，RoT 实现了 3-4 倍的 token 压缩和显著的推理加速，同时保持与显式 CoT 相当的性能，验证了通过视觉潜在空间表示推理链这一新范式的可行性。

- **Typhoon OCR: Open Vision-Language Model For Thai Document Extraction** `[VLM]` `[微调]` — [2601.14722](https://arxiv.org/abs/2601.14722) | [GitHub](https://github.com/scb-10x/typhoon-ocr)
  > Typhoon OCR 是针对泰语和英语文档提取的开源视觉语言模型，通过多阶段数据构建流程（传统 OCR + VLM 重构 + 合成数据）微调自 VLM 骨干。模型以统一框架支持文本转录、版面重建和文档结构一致性。最新版 Typhoon OCR V1.5 设计紧凑高效，减少对元数据的依赖。在金融报告、政府表单、书籍、信息图表和手写文档等多样泰语文档上，性能可与更大型的前沿专有模型媲美，同时计算成本大幅降低。

- **Privacy Collapse: Benign Fine-Tuning Can Break Contextual Privacy in Language Models** `[微调]` `[MeM]` — [2601.15220](https://arxiv.org/abs/2601.15220) | [GitHub](https://github.com/parameterlab/privacy-collapse)
  > 本文发现语言模型中的一种新现象：对前沿模型进行良性微调可导致「隐私崩溃」。多种训练数据模式可降低模型对上下文隐私的遵守，包括针对帮助性的优化、用户信息暴露和调试代码等。微调后的模型失去对上下文隐私规范的推理能力，并跨上下文违反记忆边界。关键在于，这是「静默失败」——模型在标准安全基准上仍保持高性能，但存在严重隐私漏洞。实验跨越 6 个模型、5 个微调数据集和 2 类任务验证了该现象，机制分析表明隐私表征对微调尤为脆弱。

- **XR: Cross-Modal Agents for Composed Image Retrieval** `[VLM]` `[无需训练]` — [2601.14245](https://arxiv.org/abs/2601.14245) | [GitHub](https://github.com/01yzzyu/xr.github.io)
  > XR 是一个无需训练的多智能体框架，将组合图像检索重构为逐步协调的推理过程。三类专用 Agent 协同工作：想象 Agent 通过跨模态生成合成目标表示，相似性 Agent 通过混合匹配进行粗粒度过滤，问答 Agent 通过针对性推理进行细粒度事实一致性验证。在 FashionIQ、CIRR 和 CIRCO 上相较强基线最高提升 38%，消融实验验证了每类 Agent 的必要性，展示了超越传统相似度计算的多模态推理能力。

- **Implicit Neural Representation Facilitates Unified Universal Vision Encoding** `[微调]` — [2601.14256](https://arxiv.org/abs/2601.14256) | [GitHub](https://github.com/tiktok/huvr)
  > HUVR 是首个同时学习适用于识别和生成的图像表示的统一模型。通过将模型训练为隐式神经表示（INR）的超网络，学习将图像映射为模型权重以实现快速精准重建，并整合知识蒸馏提升泛化能力。模型学到前所未有的压缩嵌入空间，在各类视觉任务上表现出色。该方法在图像表示学习上达到最优结果，同时凭借高质量微型嵌入实现生成能力，打通识别与生成之间的隔阂。

- **AgentEHR: Advancing Autonomous Clinical Decision-Making via Retrospective Summarization** `[长文本]` `[MeM]` — [2601.13918](https://arxiv.org/abs/2601.13918) | [GitHub](https://github.com/BlueZeros/AgentEHR)
  > AgentEHR 挑战 Agent 在原始高噪声电子健康记录数据库中执行复杂临床决策任务（如诊断和治疗规划），需要长程交互推理。为解决现有摘要方法导致的关键信息丢失问题，提出 RetroSum：通过回顾性机制动态重新评估交互历史以防止长上下文信息丢失，并通过演化经验策略从记忆库中检索积累的经验以弥合领域差距。实验表明 RetroSum 比竞争基线性能提升最高 29.16%，同时将交互错误减少最高 92.3%。

- **CURE-Med: Curriculum-Informed Reinforcement Learning for Multilingual Medical Reasoning** `[RL]` `[微调]` — [2601.13262](https://arxiv.org/abs/2601.13262) | [GitHub](https://github.com/AikyamLab/cure-med)
  > 本文针对多语言医学推理提出 CURE-MED 框架，包含跨 13 种语言（含阿姆哈拉语、约鲁巴语、斯瓦希里语等低资源语言）的高质量开放式医学推理数据集 CUREMED-BENCH，以及结合代码切换感知监督微调和 Group Relative Policy Optimization 的课程强化学习框架，同时优化逻辑正确性和语言稳定性。7B 参数规模下语言一致性 85.21%、逻辑正确性 54.35%；32B 参数规模下分别达 94.96% 和 70.04%，为多语言医疗场景的 LLM 部署提供可靠支持。


## 2026年1月23日

- **Evolving Computer Use Agents via Learning from Scalable Synthetic Experience** `[RL]` — [2601.15876](https://arxiv.org/abs/2601.15876) | [GitHub](https://github.com/meituan/EvoCUA)
  > EvoCUA 是一个原生计算机操作智能体（CUA），通过将数据生成与策略优化整合为自持进化循环来突破静态数据扩展的瓶颈。核心贡献包括：(1) 可验证合成引擎，自动生成多样任务并附带可执行验证器以缓解数据稀缺；(2) 支持数万个异步沙盒 rollout 的可扩展基础设施；(3) 基于大规模轨迹的迭代优化方法。与纯被动模仿静态数据集不同，EvoCUA 通过内在因果动态学习长视野计算机任务，在多个计算机操作基准上显著超越现有方法。

- **LLM-in-Sandbox Elicits General Agentic Intelligence** `[RL]` `[长文本]` `[无需训练]` — [2601.16206](https://arxiv.org/abs/2601.16206) | [GitHub](https://github.com/llm-in-sandbox/llm-in-sandbox)
  > LLM-in-Sandbox 使 LLM 在代码沙盒（虚拟计算机）中探索，以激发其在非代码领域的通用智能。研究发现强力 LLM 无需额外训练即可利用沙盒解决非代码任务（如访问外部资源获取新知识、利用文件系统处理长上下文、执行脚本满足格式要求）。进一步提出 LLM-in-Sandbox-RL，仅使用非智能体数据训练模型用于沙盒探索。实验表明该方法在数学、物理、化学、生物医学、长文本理解和指令跟随等领域均展现出稳健泛化能力，并开源为 Python 包。

- **The Flexibility Trap: Why Arbitrary Order Limits Reasoning Potential in Diffusion Language Models** `[RL]` — [2601.15165](https://arxiv.org/abs/2601.15165) | [GitHub](https://github.com/LeapLabTHU/JustGRPO)
  > 本文揭示了扩散语言模型（dLLMs）中任意顺序生成的反直觉现象：灵活的生成顺序实际上收窄而非扩展了 dLLMs 的推理边界。研究发现 dLLMs 倾向于利用顺序灵活性绕过高不确定性 token，导致解空间过早坍缩。基于此，提出放弃任意顺序、改用标准 GRPO（JustGRPO）的方案，通过简单高效的强化学习直接提升 dLLMs 推理能力，在数学和代码任务上取得显著性能提升，同时大幅降低实现复杂度。

- **Scaling Text-to-Image Diffusion Transformers with Representation Autoencoders** — [2601.16208](https://arxiv.org/abs/2601.16208) | [GitHub](https://github.com/ZitengWangNYU/Scale-RAE)
  > 本文研究表示自编码器（RAE）框架在大规模文字生成图像任务中的可扩展性。通过在冻结表示编码器（SigLIP-2）上扩展 RAE 解码器，使用网络、合成及文字渲染数据训练，发现规模提升改善整体保真度，但特定领域需定向数据组合。对比实验表明，在 0.5B 到 9.8B 参数量的扩散 Transformer 上，RAE 始终优于最先进的 FLUX VAE，且微调时 VAE 模型在 64 epoch 后灾难性过拟合，而 RAE 模型在 256 epoch 保持稳定，收敛更快、生成质量更好，建立了 RAE 作为大规模文字生成图像更强基础的地位。

- **Learning to Discover at Test Time** `[RL]` — [2601.16175](https://arxiv.org/abs/2601.16175) | [GitHub](https://github.com/test-time-training/discover)
  > TTT-Discover 提出在测试时进行强化学习（而非仅用冻结 LLM 搜索），使模型针对特定测试问题持续训练，目标是产生一个极优解而非平均意义上的多个好解。学习目标和搜索子程序均设计为优先探索最有前景的方案。在数学（Erdős 最小重叠问题、自相关不等式）、GPU 核工程（速度提升 2×）、算法竞赛（AtCoder）及单细胞生物学去噪问题上，TTT-Discover 几乎在所有尝试问题上都达到了新的最优水平，结果经专家或竞赛主办方审核确认。

- **SAMTok: Representing Any Mask with Two Words** `[VLM]` `[RL]` `[微调]` — [2601.16093](https://arxiv.org/abs/2601.16093) | [GitHub](https://github.com/bytedance/Sa2VA)
  > SAMTok 是一个离散掩码分词器，将任意区域掩码压缩为两个特殊 token，并以高保真度重建掩码。通过将掩码视为新的语言 token，SAMTok 使基础多模态 LLM（如 QwenVL 系列）无需修改架构和专用损失设计，即可通过标准下一 token 预测和简单强化学习学习像素级能力。SAMTok 基于 SAM2，在 2.09 亿个多样掩码上训练，使用掩码编码器和残差向量量化生成离散紧凑信息丰富的 token，在 500 万 SAMTok 格式的掩码数据上微调后，多个像素级理解任务取得 SOTA 性能。

- **CGPT: Cluster-Guided Partial Tables with LLM-Generated Supervision for Table Retrieval** `[微调]` — [2601.15849](https://arxiv.org/abs/2601.15849) | [GitHub](https://github.com/yumeow0122/CGPT)
  > CGPT 提出一种通过 LLM 生成监督信号增强表格检索的训练框架。核心方法：使用 K-means 聚类表格实例，跨聚类采样构建语义多样的部分表格，LLM 为这些部分表格生成合成查询，再用于硬负例对比微调嵌入模型。在四个公开基准（MimoTable、OTTQA、FetaQA、E2E-WTQ）上，CGPT 平均 R@1 提升 16.54%，并在跨域评估中展示出强泛化能力，即使使用较小 LLM 生成查询也依然有效，证明了语义引导的部分表格构建结合对比训练的有效性。

## 2026年1月26日

- **SWE-Pruner: Self-Adaptive Context Pruning for Coding Agents** `[微调]` `[长文本]` — [2601.16746](https://arxiv.org/abs/2601.16746) | [GitHub](https://github.com/Ayanami1314/swe-pruner)
  > SWE-Pruner 是一个专为代码 Agent 设计的自适应上下文剪枝框架。现有的上下文压缩方法（如 LongLLMLingua）依赖固定指标（如 PPL），忽略代码理解的任务特异性，容易破坏语法与逻辑结构。本文受人类程序员「选择性浏览」代码的启发，提出任务感知自适应剪枝：给定当前任务，Agent 先明确目标（如「关注错误处理」），再用轻量神经 Skimmer（0.6B 参数）动态筛选上下文中的相关行。在四个 benchmark 和多个模型上的评估表明，SWE-Pruner 在 SWE-Bench Verified 等代理任务上实现 23-54% 的 Token 压缩，在 LongCodeQA 单轮任务上实现最高 14.84x 压缩，且性能几乎不受影响。

- **Inference-Time Scaling of Verification: Self-Evolving Deep Research Agents via Test-Time Rubric-Guided Verification** `[无需训练]` `[微调]` — [2601.15808](https://arxiv.org/abs/2601.15808) | [GitHub](https://github.com/yxwan123/DeepVerifier)
  > 本文提出一种新范式：通过推理时验证的自我迭代来提升 Deep Research Agent（DRA）的能力，而非依赖昂贵的后训练。作者基于自动构建的 DRA 失败分类体系（5 大类、13 子类），提出 DeepVerifier——一个基于评分细则的结果奖励验证器，在 meta-evaluation F1 上比 agent-as-judge 和 LLM judge 基线高出 12%-48%。DeepVerifier 以即插即用模块形式嵌入推理流程，产生细粒度反馈供 Agent 迭代改进，无需额外训练。在强大闭源 LLM 驱动下，GAIA 和 XBench-DeepResearch 难题子集上准确率提升 8%-11%。此外还发布 DeepVerifier-4K，包含 4646 条高质量 SFT 数据，专注 DRA 验证能力训练。

- **Endless Terminals: Scaling RL Environments for Terminal Agents** `[RL]` — [2601.16443](https://arxiv.org/abs/2601.16443) | [GitHub](https://github.com/kanishkg/endless-terminals)
  > 现有 terminal 任务集为评估而非训练而设计，无法满足 RL 所需的可扩展流程。本文提出 Endless Terminals，一个全自动的终端任务生成 pipeline，包括任务描述生成、容器化环境构建与验证、完成测试生成、可解性过滤四个阶段，共产生 3255 个涵盖文件操作、日志管理、数据处理、脚本编写和数据库操作的任务。使用 vanilla PPO 训练（二元 episode 奖励，无检索/多 Agent/专用工具），多个模型取得显著提升：Qwen2.5-7B 从 10.7% 提升至 53.3%，在 TerminalBench 2.0 上优于更复杂的 Agent 架构，验证了「简单 RL + 可扩展环境」的可行性。

- **Dancing in Chains: Strategic Persuasion in Academic Rebuttal via Theory of Mind** `[RL]` `[微调]` — [2601.15715](https://arxiv.org/abs/2601.15715) | [GitHub](https://github.com/Zhitao-He/RebuttalAgent)
  > 本文提出 RebuttalAgent，首个将心智理论（Theory of Mind）应用于学术 rebuttal 的框架。现有方法仅模仿表面语言，缺乏视角采纳能力。本文通过 ToM-Strategy-Response（TSR）流程建模审稿人心理状态、制定说服策略并生成有证据支撑的回复。训练分两阶段：第一阶段 SFT 赋予模型 ToM 分析与策略规划能力；第二阶段 RL 利用自奖励机制实现可扩展自我提升。还开发了 Rebuttal-RM 评估器（100K+ 样本训练），一致性超越 GPT-4.1。实验显示 RebuttalAgent 在自动化指标上平均超越基础模型 18.3%，且在人类评估中优于前沿专有模型。已被 ICLR 2026 接收。

- **DSGym: A Holistic Framework for Evaluating and Training Data Science Agents** `[微调]` `[RL]` — [2601.16344](https://arxiv.org/abs/2601.16344) | [GitHub](https://github.com/fannie1208/DSGym)
  > 现有数据科学 benchmark 存在评估接口碎片化、任务覆盖窄以及大量任务无需使用实际数据即可作答等问题。本文提出 DSGym，一个在隔离执行环境中评估和训练数据科学 Agent 的标准化框架，提供模块化架构，便于扩展任务、Agent 脚手架和工具。DSGym-Tasks 通过质量过滤和可快捷性筛选标准化现有 benchmark，并新增 DSBio（生物信息学任务）和 DSPredict（跨域预测任务）。在训练侧，通过执行验证数据合成 pipeline 生成 2000 条训练数据，训练的 4B 模型在标准化分析 benchmark 上超越 GPT-4o。

- **ChartVerse: Scaling Chart Reasoning via Reliable Programmatic Synthesis from Scratch** `[VLM]` `[微调]` `[RL]` — [2601.13606](https://arxiv.org/abs/2601.13606) | [GitHub](https://github.com/starriver030515/ChartVerse)
  > 图表推理是 VLM 的关键能力，但高质量训练数据匮乏制约了开源模型发展。本文提出 ChartVerse，一个从零合成复杂图表与可靠推理数据的可扩展框架。（1）引入 Rollout Posterior Entropy（RPE）量化图表复杂度，并据此开发复杂度感知图表生成器；（2）采用「答案优先」的真值锚定逆向 QA 合成，保证推理严谨性。基于此构建 SFT-1.8M 和 RL-40K 数据集，ChartVerse-8B 在 6 个 benchmark 上平均得分 64.1%，超越教师模型 Qwen3-VL-30B-Thinking（62.9%），在 HuggingFace 数据集趋势榜排名第一。

- **MeepleLM: A Virtual Playtester Simulating Diverse Subjective Experiences** `[微调]` — [2601.07251](https://arxiv.org/abs/2601.07251) | [GitHub](https://github.com/leroy9472/MeepleLM)
  > 桌游中缺乏能基于涌现用户体验提供建设性批评的 AI 系统。本文整理包含 1727 份结构校正规则书和 150K 条评论的数据集，通过质量评分和面向感知的采样进行筛选，并引入 MDA（机制-动态-美学）推理来弥合规则与玩家体验之间的因果鸿沟。进一步提炼玩家角色并训练 MeepleLM——一个专为不同玩家原型内化角色特定推理模式的模型，能精准模拟多样化主观反馈。实验表明 MeepleLM 在社区认可度和评论质量上显著优于 GPT-5.1、Gemini3-Pro 等商业模型，在用户研究中偏好率达 70%。

- **VisGym: Diverse, Customizable, Scalable Environments for Multimodal Agents** `[VLM]` `[微调]` — [2601.16973](https://arxiv.org/abs/2601.16973) | [GitHub](https://github.com/visgym/VIsGym)
  > 现有 VLM 在多步视觉交互设置中的能力刻画不足，尤其是长时序感知、记忆与行动整合。本文提出 VisGym，包含 17 个可视化交互环境的综合训练和评估套件，跨越符号谜题、真实图像理解、导航和操作，提供难度、输入表示、规划时域和反馈的灵活控制，并配备生成结构化 demonstration 的多步求解器以支持 SFT。评估表明所有前沿模型在交互环境中表现不佳（简单配置成功率 46.6%，困难配置 26.0%），并揭示了上下文利用、视觉渲染等关键失败模式及改进路径。

- **VISTA-PATH: An interactive foundation model for pathology image segmentation and quantitative analysis in computational pathology** `[VLM]` `[微调]` — [2601.16451](https://arxiv.org/abs/2601.16451) | [GitHub](https://github.com/zhihuanglab/VISTA-PATH)
  > VISTA-PATH 是一个面向病理图像分割的交互式基础模型，联合以视觉上下文、语义组织描述和可选专家空间提示为条件，实现跨异质病理图像的精确多类别分割。构建了包含 160 万图像-掩码-文本三元组（覆盖 9 个器官、93 种组织类别）的 VISTA-PATH Data 语料库进行预训练。模型支持动态人在环路细化，将稀疏块级边界框反馈传播为全切片像素级分割。在多个 held-out 和外部 benchmark 上持续优于现有分割基础模型，并通过提出肿瘤相互作用评分（TIS）展示了与患者生存预后的强相关性。


## 2026年1月27日

- **Elastic Attention: Test-time Adaptive Sparsity Ratios for Efficient Transformers** `[无需训练]` `[长文本]` — [2601.17367](https://arxiv.org/abs/2601.17367) | [GitHub](https://github.com/LCM-Lab/Elastic-Attention)
  > 标准注意力机制的平方复杂度是大语言模型长上下文推理的性能瓶颈。现有混合稀疏-全注意力策略通常采用静态比例，无法根据输入动态调整。本文提出 Elastic Attention，通过在预训练模型中加入轻量级 Attention Router，在推理时动态地为每个注意力头分配全注意力或稀疏注意力模式，实现自适应稀疏率。训练仅需 8 张 A800 GPU 运行 12 小时，在三个长上下文基准测试上验证了其相对于现有方法的优越性，同时兼顾了强大的性能和高效的推理能力。

- **iFSQ: Improving FSQ for Image Generation with 1 Line of Code** `[微调]` — [2601.17124](https://arxiv.org/abs/2601.17124) | [GitHub](https://github.com/Tencent-Hunyuan/iFSQ)
  > 图像生成领域长期被自回归模型（离散 token）和扩散模型（连续隐变量）两条技术路线割裂。有限标量量化（FSQ）理论上可作为两者的桥梁，但原始 FSQ 的等间隔量化会导致激活崩塌。本文提出 iFSQ，仅需将激活函数替换为分布匹配映射以实施均匀先验，即可解决该问题。研究发现：(1) 自回归在效率上领先，扩散有更高质量上限；(2) 表示的最优比特约为 4 bits；(3) REPA 对齐的最优深度始终为总层数的 1/3。iFSQ 为统一 AR 与 Diffusion 建模提供了简洁有效的 tokenizer 基础。

- **Masked Depth Modeling for Spatial Perception** `[微调]` — [2601.17895](https://arxiv.org/abs/2601.17895) | [GitHub](https://github.com/Robbyant/lingbot-depth)
  > 空间视觉感知对自动驾驶、具身交互等物理世界应用至关重要，而 RGB-D 摄像头在镜面或无纹理表面等条件下深度获取不稳定。本文将深度传感器的不准确性建模为「带掩码」的信号，提出 LingBot-Depth 深度补全模型，通过视觉上下文结合掩码深度建模对深度图进行精化，并引入自动数据策略管道以扩展训练规模。该方法能在真实场景挑战条件下可靠地恢复准确的空间深度信息。

- **AR-Omni: A Unified Autoregressive Model for Any-to-Any Generation** `[微调]` `[VLM]` — [2601.17761](https://arxiv.org/abs/2601.17761) | [GitHub](https://github.com/ModalityDance/AR-Omni)
  > 现有全模态大语言模型（Omni MLLM）通常依赖额外专家组件实现多模态生成，破坏了统一训练与推理的简洁性。本文提出 AR-Omni，基于自回归范式构建统一的任意到任意生成模型，在单一 Transformer 解码器下同时支持文本、图像和流式语音生成，无需专家解码器。针对模态不平衡问题引入任务感知损失重加权，采用轻量级 token 级感知对齐损失提升视觉质量，并通过有限状态解码机制平衡稳定性与创造性。实验表明 AR-Omni 在三种模态下均达到较强质量，语音生成实时因子达 0.88。

- **CGPT: Cluster-Guided Partial Tables with LLM-Generated Supervision for Table Retrieval** `[微调]` — [2601.15849](https://arxiv.org/abs/2601.15849) | [GitHub](https://github.com/yumeow0122/CGPT)
  > 通用嵌入模型在表格检索中表现欠佳，原因在于高度结构化内容导致语义压缩与查询-表格不匹配。本文提出 CGPT 训练框架，利用 K-means 对表格实例聚类并跨簇采样，构建语义多样的部分表格，再由 LLM 为这些部分表格生成合成查询，通过难负样本对比微调嵌入模型。在 MimoTable、OTTQA、FetaQA 和 E2E-WTQ 四个公开基准上，CGPT 相比 QGpT 平均 R@1 提升 16.54%，在统一多领域语料库设置中展示了强跨域泛化能力。已被 WWW 2026 收录。

- **DRPG (Decompose, Retrieve, Plan, Generate): An Agentic Framework for Academic Rebuttal** `[无需训练]` `[长文本]` — [2601.18081](https://arxiv.org/abs/2601.18081) | [GitHub](https://github.com/ulab-uiuc/DRPG-RebuttalAgent)
  > 学术审稿回复是学术交流的关键环节，但现有方法多依赖现成 LLM 或简单流程，在长上下文理解和生成针对性回复方面表现不足。本文提出 DRPG 智能体框架，分四步自动生成学术回复：将审稿意见分解为原子级关切、从论文中检索相关证据、规划回复策略、生成对应回复。DRPG 的规划器识别最优回复方向的准确率超 98%，使用 8B 模型即超越人类平均水平，在顶级会议数据上显著优于现有方法，并支持多轮回复场景。

- **One Adapts to Any: Meta Reward Modeling for Personalized LLM Alignment** `[RL]` `[微调]` — [2601.18731](https://arxiv.org/abs/2601.18731) | [GitHub](https://github.com/ModalityDance/MRM)
  > 个性化 LLM 对齐依赖能捕获用户特定偏好的个性化奖励模型，面临两大挑战：个人反馈数据匮乏和对未见用户的高效适应。本文提出元奖励建模（MRM），将个性化奖励建模重构为元学习问题：将每位用户的奖励模型表示为基础奖励函数的加权组合，采用 MAML 风格框架优化权重初始化，支持少量反馈下的快速适应；引入鲁棒个性化目标（RPO）在元优化时重点关注难以学习的用户。在个性化偏好数据集上的实验表明 MRM 显著提升了少样本个性化能力并改善了用户鲁棒性。

- **Fast KVzip: Efficient and Accurate LLM Inference with Gated KV Eviction** `[无需训练]` `[长文本]` — [2601.17668](https://arxiv.org/abs/2601.17668) | [GitHub](https://github.com/Janghyun1230/FastKVzip)
  > KV 缓存管理对大语言模型的实际部署至关重要，但现有压缩方法往往在性能损失和计算开销之间存在权衡。本文提出基于门控的 KV 缓存淘汰方法，为冻结权重的 LLM 引入轻量级 sink-attention 门控模块以识别并保留关键 KV 对，无缝集成到 prefill 和 decoding 阶段，训练仅依赖前向传播，规避了昂贵的反向传播。在 Qwen2.5-1M、Qwen3 和 Gemma3 等模型上，淘汰 70% KV 缓存后仍保持近无损性能，涵盖长上下文理解、代码理解和数学推理等任务。

- **The Side Effects of Being Smart: Safety Risks in MLLMs' Multi-Image Reasoning** `[VLM]` — [2601.14127](https://arxiv.org/abs/2601.14127) | [GitHub](https://github.com/thu-coai/MIR-SafetyBench)
  > 随着多模态大语言模型（MLLM）处理复杂多图像指令的推理能力增强，新的安全风险随之出现。本文提出 MIR-SafetyBench，首个聚焦多图像推理安全的基准，涵盖 9 种多图像关系共 2676 个实例。对 19 个 MLLM 的评测揭示了一个令人警惕的趋势：多图像推理能力越强的模型在 MIR-SafetyBench 上往往越脆弱。研究还发现不安全生成在注意力熵上低于安全生成，暗示模型可能过度聚焦于任务求解而忽视安全约束。代码和数据均已开源。

- **TensorLens: End-to-End Transformer Analysis via High-Order Attention Tensors** `[无需训练]` — [2601.17958](https://arxiv.org/abs/2601.17958) | [GitHub](https://github.com/idoatad/TensorLens)
  > 注意力矩阵分析是 Transformer 可解释性研究的基础，但现有方法多聚焦单个注意力头或层，难以反映模型全局行为。本文提出 TensorLens，将整个 Transformer 建模为单一输入相关线性算子，通过高阶注意力交互张量统一编码注意力、FFN、激活函数、归一化层和残差连接。该张量提供了理论一致且表达丰富的模型计算线性表示，实验验证其产生的表示比已有注意力聚合方法更丰富，可作为可解释性和模型理解工具开发的有力基础。

- **HalluGuard: Demystifying Data-Driven and Reasoning-Driven Hallucinations in LLMs** `[无需训练]` — [2601.18753](https://arxiv.org/abs/2601.18753) | [GitHub](https://github.com/Susan571/HalluGuard-ICLR2026)
  > LLM 的幻觉问题严重影响其在医疗、法律、科学发现等高风险领域的可靠性，通常源于数据驱动幻觉和推理驱动幻觉两类。现有方法通常只针对一类且依赖特定任务的启发式，泛化能力有限。本文提出幻觉风险界（Hallucination Risk Bound）统一理论框架，将幻觉风险正式分解为训练时不匹配（数据驱动）和推理时不稳定（推理驱动）两个分量；在此基础上提出基于 NTK 的评分方法 HalluGuard，利用 NTK 诱导的几何结构和捕获表示联合识别两类幻觉。在 10 个数据集、11 个基线、9 个主流 LLM 上持续实现最优性能，已被 ICLR 2026 收录。


## 2026年1月28日

- **AgentDoG: A Diagnostic Guardrail Framework for AI Agent Safety and Security** `[微调]` — [2601.18491](https://arxiv.org/abs/2601.18491) | [GitHub](https://github.com/AI45Lab/AgentDoG)
  > 随着AI智能体的兴起，自主工具调用和环境交互带来复杂安全挑战，现有护栏模型缺乏智能体风险感知和诊断透明度。本文提出统一三维分类体系，从来源（where）、失效模式（how）、后果（what）三个正交维度对智能体风险建模，并据此构建细粒度安全基准ATBench和诊断护栏框架AgentDoG。AgentDoG可跨轨迹进行上下文感知监控，并能诊断不安全行为及「看似安全但不合理」行为的根因，超越二元标签提供溯源和透明度。框架提供4B/7B/8B三种规格，覆盖Qwen和Llama模型家族，在多种复杂交互场景下达到最优安全审核性能，所有模型和数据集均开源。

- **AdaReasoner: Dynamic Tool Orchestration for Iterative Visual Reasoning** `[RL]` `[VLM]` — [2601.18631](https://arxiv.org/abs/2601.18631) | [GitHub](https://github.com/ssmisya/AdaReasoner)
  > 本文提出AdaReasoner，使多模态大模型将工具使用作为通用推理技能而非特定任务行为来学习。核心贡献包括三点：（1）可扩展数据整理流程，构建长程多步骤工具交互训练数据；（2）Tool-GRPO强化学习算法，基于最终任务成功优化工具选择与排序；（3）自适应学习机制，动态调节工具使用频率。实验表明AdaReasoner能自主采纳有益工具、抑制无关工具，7B基模型在多个基准上平均提升24.9%，在VSP和Jigsaw等任务上超越GPT-5等强大闭源系统。

- **Youtu-VL: Unleashing Visual Potential via Unified Vision-Language Supervision** `[VLM]` `[微调]` — [2601.19798](https://arxiv.org/abs/2601.19798) | [GitHub](https://github.com/TencentCloudADP/youtu-vl)
  > 现有视觉语言模型（VLM）存在文本主导优化偏差，将视觉信号仅视为被动条件输入，导致细粒度视觉信息丢失。本文提出Youtu-VL，引入视觉语言统一自回归监督（VLUAS）范式，将优化目标从「视觉为输入」转变为「视觉为目标」——将视觉token直接纳入预测流，对视觉细节和语言内容施加统一自回归监督。进一步将该范式扩展至视觉中心任务，使标准VLM无需任务特定添加即可完成视觉中心任务。大量实验表明Youtu-VL在通用多模态任务和视觉中心任务上均取得有竞争力的性能。

- **World Craft: Agentic Framework to Create Visualizable Worlds via Text** — [2601.09150](https://arxiv.org/abs/2601.09150) | [GitHub](https://github.com/HerzogFL/World-Craft)
  > 本文提出World Craft，一个通过用户文本描述创建可执行可视化AI Town的智能体框架，面向无编程能力的非专家用户。框架由两个核心模块构成：World Scaffold是基于Godot引擎的结构化简洁标准化方案，为LLM高效定制交互式游戏场景提供脚手架；World Guild是多智能体框架，通过渐进式分析用户意图自动生成游戏资产和角色。该框架支持大型语言模型自动理解用户需求、生成场景代码，并最终创建可直观运行的虚拟世界环境。

- **Revisiting Parameter Server in LLM Post-Training** `[RL]` `[微调]` — [2601.19362](https://arxiv.org/abs/2601.19362) | [GitHub](https://github.com/sail-sg/odc)
  > 现代数据并行训练偏好集合通信方式，但LLM后训练中序列长度高度不均衡，导致集合通信产生同步屏障，短序列设备大量空闲。本文重新审视参数服务器（PS）范式，提出按需通信（ODC），将PS融入全分片数据并行（FSDP），以点对点通信替代all-gather和reduce-scatter集合操作。ODC可在不平衡工作负载下减少同步开销，理论上支持异步更新。实验表明在序列长度高度不均衡的RLHF等场景中，ODC相比FSDP显著提升训练效率和设备利用率。

- **Selective Steering: Norm-Preserving Control Through Discriminative Layer Selection** `[无需训练]` — [2601.19375](https://arxiv.org/abs/2601.19375) | [GitHub](https://github.com/knoveleng/steering)
  > 激活引导（activation steering）是一种推理时对齐干预方法，但现有方法存在系数调优敏感或违反范数保持的问题。本文提出Selective Steering，通过两个核心创新解决上述局限：（1）判别性层选择机制，识别对目标行为最具影响力的层并仅在这些层进行干预；（2）范数保持旋转操作，在2D子空间内实现连续控制同时保持激活分布不变，避免分布偏移和生成崩塌问题。该方法在小参数量（7B以下）模型上尤为有效，在多个对齐和安全控制任务上超越现有激活引导基线。

- **EvolVE: Evolutionary Search for LLM-based Verilog Generation and Optimization** — [2601.18067](https://arxiv.org/abs/2601.18067) | [GitHub](https://github.com/weiber2002/ICRTL)
  > Verilog设计周期劳动密集且需要大量领域专业知识，LLM虽提供自动化途径但受限于训练数据不足和顺序推理。本文提出EvolVE，首个系统分析多种进化策略在芯片设计任务上效果的框架：蒙特卡洛树搜索（MCTS）在功能正确性上最优，思路引导精化（IGR）在优化任务上更优，并利用结构化测试台生成（STG）加速进化过程。同时引入工业级基准IC-RTL，源自全国集成电路设计大赛。实验表明EvolVE在VerilogEval v2上达98.1%、RTLLM v2上达92%，并在IC-RTL上超越参赛者参考实现，Huffman编码任务PPA乘积降低66%。


## 2026年1月29日

- **Harder Is Better: Boosting Mathematical Reasoning via Difficulty-Aware GRPO and Multi-Aspect Question Reformulation** `[RL]` `[微调]` — [2601.20614](https://arxiv.org/abs/2601.20614) | [GitHub](https://github.com/AMAP-ML/MathForge)
  > 本文提出 MathForge 框架，针对现有 RLVR 方法在算法和数据层面对难题关注不足的问题进行改进。算法层面，作者提出难度感知 GRPO（DGPO），通过难度平衡的组优势估计修正 GRPO 的隐式不平衡，并引入问题级别的难度加权。数据层面，提出多角度问题重构（MQR）策略，从多维度改写题目以提升固有难度，同时保持原有标准答案不变。MathForge 形成协同循环：MQR 扩展数据边界，DGPO 从增强数据中高效学习。实验表明，MathForge 在多个数学推理任务上显著超越现有方法。

- **Innovator-VL: A Multimodal Large Language Model for Scientific Discovery** `[VLM]` `[微调]` `[RL]` — [2601.19325](https://arxiv.org/abs/2601.19325) | [GitHub](https://github.com/InnovatorLM/Innovator-VL)
  > Innovator-VL 是一个面向科学发现的多模态大语言模型，展示了在大幅减少数据量的前提下实现强科学推理能力的可能性。核心贡献包括：（1）完全透明的端到端可复现训练流程，涵盖数据采集、清洗、SFT、RL 和评估；（2）仅使用不足 500 万精选样本、无需大规模预训练即可在多种科学任务上达到有竞争力的性能，体现出极高数据效率；（3）在通用视觉、多模态推理和科学基准测试上均表现出强泛化能力。实验结果表明，基于原则性数据选择而非无差别扩展，即可实现高效的科学对齐。

- **DeepSeek-OCR 2: Visual Causal Flow** `[VLM]` — [2601.20552](https://arxiv.org/abs/2601.20552) | [GitHub](https://github.com/deepseek-ai/DeepSeek-OCR-2)
  > DeepSeek-OCR 2 提出了全新编码器 DeepEncoder V2，能够根据图像语义动态重排视觉 token 顺序。传统视觉语言模型对视觉 token 采用固定的光栅扫描顺序，这与人类视觉感知的灵活语义扫描模式相悖。DeepEncoder V2 受人类因果信息处理机制启发，在输入 LLM 前通过因果推理能力智能重排 token。本文探索了一种新范式：2D 图像理解是否可通过两级级联的 1D 因果推理结构有效实现，为真正的 2D 推理提供新的架构思路。

- **SERA: Soft-Verified Efficient Repository Agents** `[微调]` — [2601.20789](https://arxiv.org/abs/2601.20789) | [GitHub](https://github.com/allenai/SERA)
  > SERA（Soft-Verified Efficient Repository Agents）提出了一种高效训练方法，使开源代码智能体能够以极低成本快速专化到私有代码库。仅使用监督微调（SFT），SERA 在全开源模型中达到最先进水平，并与 Devstral-Small-2 等前沿开权重模型性能相当。相较于强化学习训练方法，SERA 成本降低 26 倍，相较于其他高质量 SFT 管道降低 57 倍。核心创新在于「软验证」机制，通过轻量级语义等价检查而非昂贵的执行验证来筛选训练数据质量，使专化代码智能体的快速创建变得实用可行。

- **Training Reasoning Models on Saturated Problems via Failure-Prefix Conditioning** `[RL]` — [2601.20829](https://arxiv.org/abs/2601.20829) | [GitHub](https://github.com/minwukim/training-on-saturated-problems)
  > 本文针对 RLVR 训练中问题饱和导致学习停滞的问题，提出「失败前缀条件化」（Failure-Prefix Conditioning）方法。核心思路是：不从原始问题开始 rollout，而是从少见的错误推理轨迹中提取前缀作为条件，将探索重定向到容易失败的状态，从而暴露更多有效学习信号。实验表明，该方法在饱和问题上取得的性能提升与在更大规模数据集上训练相当，同时不影响模型在未饱和问题上的泛化能力，为 RLVR 训练突破饱和瓶颈提供了简单有效的解决方案。

- **UPLiFT: Efficient Pixel-Dense Feature Upsampling with Local Attenders** `[无需训练]` — [2601.17950](https://arxiv.org/abs/2601.17950) | [GitHub](https://github.com/mwalmer-umd/UPLiFT)
  > UPLiFT 研究任务无关的特征上采样问题，旨在以极低成本从预训练视觉骨干网络生成更密集特征。现有基于交叉注意力的上采样方法面临与骨干网络相同的效率扩展问题，而本文证明迭代上采样方法仍具有竞争力。UPLiFT 架构（Universal Pixel-Level Feature Transformer）采用局部注意力机制，在保持低推理开销的同时达到最先进性能。实验涵盖分割、深度估计等多个密集预测任务，UPLiFT 以更低计算成本超越或匹配基于交叉注意力的方法，为高效密集特征提取提供了新的技术路线。

- **Persona Prompting as a Lens on LLM Social Reasoning** `[无需训练]` — [2601.20757](https://arxiv.org/abs/2601.20757) | [GitHub](https://github.com/jingyng/PP-social-reasoning)
  > 本文研究角色提示（Persona Prompting）对大语言模型社会推理能力的影响，聚焦于仇恨检测等社会敏感任务中模型解释质量的变化。通过在带有词级标注的数据集上测量 LLM 生成理由与不同人口群体人工标注的一致性，评估角色提示对模型偏差和人类对齐的影响。在三个 LLM 上的实验揭示三个关键发现：（1）角色提示在最主观任务（仇恨检测）上提升分类性能，但在更客观任务上会降低性能；（2）角色提示能改变模型理由以更好对齐特定群体视角；（3）不同模型对角色提示的响应存在显著差异。研究为角色提示作为社会推理「透镜」提供了系统性评估框架。

- **SE-DiCoW: Self-Enrolled Diarization-Conditioned Whisper** `[微调]` — [2601.19194](https://arxiv.org/abs/2601.19194) | [GitHub](https://github.com/BUTSpeechFIT/TS-ASR-Whisper)
  > SE-DiCoW 针对多说话人环境下目标说话人 ASR 的关键局限——说话人完全重叠时 STNO 掩码的歧义性问题——提出改进方案。通过自注册机制，利用对话中目标说话人最活跃的片段作为固定条件，经由每个编码器层的交叉注意力注入。同时改进了数据分割、模型初始化和数据增强策略。综合改进使 SE-DiCoW 在 EMMA MT-ASR 基准测试上相较原始 DiCoW 将宏平均 tcpWER 降低 52.4%（相对值），在领域外数据集上展现出优异的泛化性能。


## 2026年1月30日

- **Idea2Story: An Automated Pipeline for Transforming Research Concepts into Complete Scientific Narratives** `[无需训练]` `[MeM]` — [2601.20833](https://arxiv.org/abs/2601.20833) | [GitHub](https://github.com/AgentAlphaAGI/Idea2Paper)
  > Idea2Story 提出了一种预计算驱动的自主科学发现框架，将文献理解从在线推理转移到离线知识构建。系统持续收集同行评审论文及其评审反馈，提取核心方法单元，构建可复用的研究模式，并组织为结构化方法论知识图谱。运行时，将模糊的用户研究意图对齐到已有研究范式，实现高质量研究模式的高效检索与复用，避免开放性生成和试错。该方法缓解了大模型的上下文窗口瓶颈，显著减少了运行时的文献重复推理。实验表明，Idea2Story 能生成连贯、方法扎实且具有新颖性的研究方案，证明离线知识构建可作为可靠自主科研的实用可扩展基础。

- **MMFineReason: Closing the Multimodal Reasoning Gap via Open Data-Centric Methods** `[VLM]` `[微调]` — [2601.21821](https://arxiv.org/abs/2601.21821) | [GitHub](https://github.com/LHL3341/MMFineReason)
  > MMFineReason 构建了一个大规模多模态推理数据集，包含 180 万样本和 51 亿解题 token，通过系统化三阶段流程（数据收集与标准化、CoT 推理生成、质量与难度感知筛选）生成高质量推理标注（从 Qwen3-VL-235B-A22B-Thinking 蒸馏）。数据集涵盖 STEM 问题、视觉谜题和复杂图表，每个样本均附有视觉扎根的推理链。基于此微调的 MMFineReason-4B 超越了 Qwen3-VL-8B-Thinking，MMFineReason-8B 甚至媲美 Qwen3-VL-32B-Thinking，展现了卓越的参数效率。研究还发现「少即是多」现象：仅 7% 的子集（12.3 万样本）即可达到与完整数据集相当的性能。

- **ConceptMoE: Adaptive Token-to-Concept Compression for Implicit Compute Allocation** `[无需训练]` `[长文本]` — [2601.21420](https://arxiv.org/abs/2601.21420) | [GitHub](https://github.com/ZihaoHuang-notabot/ConceptMoE)
  > ConceptMoE 针对大语言模型对所有 token 分配均匀计算这一低效问题，提出了动态 token 到概念压缩方法，实现隐式 token 级计算分配。可学习的分块模块通过测量 token 间相似度识别最优边界，按目标压缩比 R 压缩序列，再输入计算密集的概念块转换器。不同于离散专家路由，ConceptMoE 通过连续语义聚合隐式分配计算。实验在语言建模和下游任务上验证了方法有效性，实现了灵活的精度-效率权衡，可即插即用于标准 Transformer 架构。

- **Shaping capabilities with token-level data filtering** `[微调]` — [2601.21571](https://arxiv.org/abs/2601.21571) | [GitHub](https://github.com/neilrathi/token-filtering)
  > 当前去除语言模型不良能力的方法大多是事后干预，容易被绕过。本文提出在预训练阶段直接通过数据过滤来塑造模型能力。以去除医学能力为代理任务，研究表明对预训练数据进行 token 级过滤（而非文档级过滤）简单有效、鲁棒且在规模上廉价。受数据归因研究启发，token 级过滤比文档级过滤效果更好。该方法可精确控制模型在特定领域的能力，为预训练阶段的能力塑造提供了一种实用的新范式，无需事后对齐即可减少潜在的有害知识。

- **Exploring Reasoning Reward Model for Agents** `[RL]` — [2601.22154](https://arxiv.org/abs/2601.22154) | [GitHub](https://github.com/kxfan2002/Reagent)
  > Agentic RL 在复杂推理和工具调用方面取得了显著成功，但大多数方法仍依赖稀疏的结果奖励，无法区分中间推理质量。本文提出 Agent Reasoning Reward Model（Agent-RRM），一种多维度奖励模型，为智能体轨迹提供结构化反馈，包括：步骤级推理质量评估、工具调用合理性判断和整体轨迹一致性评分。Agent-RRM 通过强化学习训练智能体追求更高质量的推理过程，实验结果表明在多个 agentic 基准上显著优于仅使用结果奖励的基线方法。

- **Language-based Trial and Error Falls Behind in the Era of Experience** `[RL]` — [2601.21754](https://arxiv.org/abs/2601.21754) | [GitHub](https://github.com/Harry-mic/SCOUT)
  > 尽管大语言模型在基于语言的任务中表现出色，但在符号或空间等非语言环境中的适应能力仍然有限。本文证明主要瓶颈不是预训练分布不匹配，而是探索的高昂代价：掌握这类任务需要大量试错，计算上不可持续。为此提出 SCOUT 框架，将强化学习引入智能体的经验学习中，通过直接环境交互积累经验而非依赖语言试错。实验表明，SCOUT 在多种非语言任务上显著超越基于语言的 ReAct 等方法，体现了「经验时代」中基于 RL 的智能体学习范式的优越性。

- **Latent Adversarial Regularization for Offline Preference Optimization** `[RL]` `[微调]` — [2601.22083](https://arxiv.org/abs/2601.22083) | [GitHub](https://github.com/enyijiang/GANPO)
  > 偏好优化中传统 token 级正则化存在局限性，因为 token 空间的相似性不等价于语义或行为相似性。本文提出 GANPO，通过潜在空间正则化解决这一挑战：引入对抗性惩罚机制，约束策略在连续潜在空间中与参考模型的分布偏差，从而保留语义一致性。GANPO 无需显式训练判别器，通过最小化潜在空间中的对抗损失实现隐式正则化。在多个偏好优化基准上，GANPO 相比 DPO、IPO 等基线方法显著提升了对齐质量，尤其在分布外泛化方面表现突出。

- **Typhoon-S: Minimal Open Post-Training for Sovereign Large Language Models** `[微调]` `[RL]` — [2601.18129](https://arxiv.org/abs/2601.18129) | [GitHub](https://github.com/scb-10x/typhoon-s)
  > Typhoon-S 探索了在主权/区域场景下以最小代价进行 LLM 后训练的方法，使区域机构能够在可控预算内掌控模型权重、训练数据和部署决策。研究在资源有限的东南亚语言（泰语等）上，系统评估了监督微调（SFT）和强化学习后训练（RLHF/GRPO）的最优组合策略，包括数据配比、训练顺序和超参数选择。实验表明，通过精心设计的最小后训练流程，可以在保持英语能力的同时大幅提升低资源语言性能，为主权 LLM 建设提供了开源参考基线。

- **MAD: Modality-Adaptive Decoding for Mitigating Cross-Modal Hallucinations in Multimodal Large Language Models** `[VLM]` `[无需训练]` — [2601.21181](https://arxiv.org/abs/2601.21181) | [GitHub](https://github.com/top-yun/MAD)
  > 多模态大语言模型存在跨模态幻觉问题，即一种模态不当影响另一种模态的生成，导致虚构输出。本文提出 MAD（Modality-Adaptive Decoding），一种无需训练的方法，根据任务需求自适应地加权模态特定解码分支。MAD 利用模型内在的自评估能力来判断各模态的相关性，在推理时动态调整视觉和语言分支的权重。在多个 VLM 幻觉基准上的实验证明，MAD 能有效减少跨模态幻觉，且无需额外训练或参数，可即插即用于现有多模态模型。

- **VTC-R1: Vision-Text Compression for Efficient Long-Context Reasoning** `[VLM]` `[长文本]` `[无需训练]` — [2601.22069](https://arxiv.org/abs/2601.22069) | [GitHub](https://github.com/w-yibo/VTC-R1)
  > 长上下文推理赋予 LLM 处理复杂任务的能力，但引入了严重的计算效率瓶颈。现有高效方法通常需要复杂的额外训练或外部模型，限制了可扩展性。VTC-R1 提出一种新的高效推理范式，将视觉-文本压缩集成到推理过程中：通过识别并压缩推理步骤中的冗余视觉 token 和文本 token，在保持推理质量的同时大幅降低计算开销。在视觉语言推理任务上的实验表明，VTC-R1 相比基线方法在显著压缩上下文长度的同时，维持了具有竞争力的推理准确率。

- **KromHC: Manifold-Constrained Hyper-Connections with Kronecker-Product Residual Matrices** `[微调]` — [2601.21579](https://arxiv.org/abs/2601.21579) | [GitHub](https://github.com/wz1119/KromHC)
  > Hyper-Connections（HC）在神经网络中取得了成功，但存在训练不稳定和扩展性受限的问题。流形约束 Hyper-Connections（mHC）通过将残差连接空间投影到 Birkhoff 多面体来缓解这些挑战，但面临两个问题：Sinkhorn-Knopp 算法无法总是产生精确双随机矩阵；以及 O(n³C) 的参数复杂度过高。本文提出 KromHC，利用 Kronecker 积分解残差矩阵，将参数复杂度降至 O(nC)，同时保证严格的流形约束。实验表明 KromHC 在多个语言模型任务上实现了更好的训练稳定性和参数效率。

- **MetricAnything: Scaling Metric Depth Pretraining with Noisy Heterogeneous Sources** `[无需训练]` — [2601.22054](https://arxiv.org/abs/2601.22054) | [GitHub](https://github.com/metric-anything/metric-anything)
  > 将缩放范式扩展到度量深度估计面临异构传感器噪声、相机依赖偏差和跨源 3D 数据中的度量歧义等挑战。MetricAnything 提出了一种简单可扩展的预训练框架，无需手工设计提示、相机特定建模或任务特定架构，即可从噪声多样 3D 来源中学习度量深度。核心方法通过自适应噪声建模和跨源对齐将异构数据统一处理。大规模实验表明，该框架在多个度量深度估计基准上取得了领先性能，证明了噪声异构数据扩展预训练的可行性。

- **BMAM: Brain-inspired Multi-Agent Memory Framework** `[MeM]` — [2601.20465](https://arxiv.org/abs/2601.20465) | [GitHub](https://github.com/innovation64/BMAM)
  > 基于语言模型的智能体在长时交互中面临时序信息保留和跨会话行为一致性的挑战（即「灵魂侵蚀」问题）。BMAM（脑启发多智能体记忆）提出了一种通用记忆架构，将智能体记忆建模为功能专化子系统集合而非单一非结构化存储。受认知记忆系统启发，BMAM 将记忆分解为感知记忆、情景记忆、语义记忆和程序记忆等模块，并通过多智能体协作管理和检索。实验表明 BMAM 显著改善了长期交互中的记忆保留和行为一致性，减少了信息遗忘和「灵魂侵蚀」现象。

- **FROST: Filtering Reasoning Outliers with Attention for Efficient Reasoning** `[无需训练]` `[长文本]` — [2601.19001](https://arxiv.org/abs/2601.19001) | [GitHub](https://github.com/robinzixuan/FROST)
  > FROST 提出了一种基于注意力的高效推理方法，利用注意力权重剪除非关键推理路径，生成更短且更可靠的推理轨迹。方法引入推理离群点的概念，设计了注意力驱动机制在句子级别识别并去除这些低质量推理步骤。理论分析证明 FROST 在消除离群点的同时保留并增强了模型的推理能力。在多个推理基准上的实验验证表明，FROST 在显著压缩推理长度的同时维持了准确率，适用于需要实时响应的推理场景。

- **Flow-based Extremal Mathematical Structure Discovery** `[RL]` — [2601.18005](https://arxiv.org/abs/2601.18005) | [GitHub](https://github.com/berczig/FlowBoost)
  > 数学中极值结构的发现需要在分析方法几乎无指引、暴力搜索又不可行的广阔非凸空间中导航。FlowBoost 提出了一种闭环生成框架，结合三个组件：（i）几何感知的条件 flow-matching 模型，学习采样高质量配置；（ii）奖励引导的策略优化，配合动作空间约束；（iii）课程化难度递进学习。框架在图论和组合优化中的极值结构发现任务上进行了验证，展示了基于生成模型的数学结构探索能力，为数学自动化发现提供了新思路。

- **Beyond Imitation: Reinforcement Learning for Active Latent Planning** `[RL]` `[微调]` — [2601.21598](https://arxiv.org/abs/2601.21598) | [GitHub](https://github.com/zz1358m/ATP-Latent-master)
  > 潜在推理方法通过让 LLM 用连续潜在 token 替代离散语言 token 来实现高效密集的思维链推理，但现有方法对语言标签的被动模仿导致次优的潜在 token 表示和推理策略。ATP-Latent（主动潜在规划）将潜在 token 的监督过程建模为条件变分自编码器（VAE），获得更平滑的潜在空间，并通过 RL 和辅助一致性奖励（基于 VAE 解码内容的一致性）引导最优潜在推理策略。在 LLaMA-1B 上的实验显示，与先进基线相比准确率提升 +4.1%，token 消耗降低 -3.3%。


## 2026年2月2日

- **PaperBanana: Automating Academic Illustration for AI Scientists** `[VLM]` `[无需训练]` — [2601.23265](https://arxiv.org/abs/2601.23265) | [GitHub](https://github.com/dwzhu-pku/PaperBanana)
  > PaperBanana 是一个用于自动生成学术论文配图的智能体框架，旨在解放科研人员在制作出版级示意图时的人工负担。系统以最先进的 VLM 和图像生成模型为驱动，协调多个专职智能体完成参考检索、内容与风格规划、图像渲染以及自我批判的迭代精炼。为系统评估框架能力，作者构建了 PaperBananaBench 基准，包含 292 个从 NeurIPS 2025 论文中采集的方法论示意图测试案例，覆盖多样研究领域与配图风格。实验表明 PaperBanana 在忠实度、简洁性、可读性和美观性四个维度上均优于主流基线，并进一步验证了对统计图表生成的迁移能力。

- **ASTRA: Automated Synthesis of agentic Trajectories and Reinforcement Arenas** `[RL]` `[微调]` — [2601.21558](https://arxiv.org/abs/2601.21558) | [GitHub](https://github.com/LianjiaTech/astra)
  > ASTRA 是一个全自动端到端框架，用于通过可扩展数据合成与可验证强化学习来训练工具增强型语言模型智能体。框架包含两个互补模块：一是利用工具调用图静态拓扑合成多样且结构化的高质量轨迹，赋予模型广泛可迁移的工具使用能力；二是将分解后的问答追踪转化为独立可执行、规则可验证的环境，支持确定性多轮 RL 训练。作者将 SFT 与在线 RL 结合为统一训练方法，使用轨迹级奖励平衡任务完成与交互效率。在多个工具使用基准上，ASTRA 训练的模型以同等规模达到最优性能，接近闭源系统水平，同时保留核心推理能力。

- **Quartet II: Accurate LLM Pre-Training in NVFP4 by Improved Unbiased Gradient Estimation** `[微调]` — [2601.22813](https://arxiv.org/abs/2601.22813) | [GitHub](https://github.com/IST-DASLab/Quartet-II)
  > Quartet II 针对 NVIDIA Blackwell GPU 支持的 NVFP4 低精度格式，提出了一种更准确的无偏量化方案，旨在实现大规模 LLM 的全精度端到端预训练。核心贡献是新型微尺度格式无偏量化例程 MS-EDEN，其量化误差比随机舍入（SR）降低 2 倍以上。将 MS-EDEN 集成为完整的全 NVFP4 线性层量化方案 Quartet II 后，前向和反向传播中所有关键矩阵乘法的梯度估计质量均得到提升。作者在 1.9B 参数、38B token 的端到端 LLM 训练中验证了方案效果，并提供了在 Blackwell GPU 上相比 BF16 快 4.2× 的内核实现。

- **THINKSAFE: Self-Generated Safety Alignment for Reasoning Models** `[RL]` `[微调]` — [2601.23143](https://arxiv.org/abs/2601.23143) | [GitHub](https://github.com/seanie12/ThinkSafe)
  > 大型推理模型（LRM）通过强化学习驱动的长链思维获得强大推理能力，但过度优化合规性会使模型对有害提示产生漏洞。现有安全对齐方法依赖外部教师蒸馏，会引入分布偏差并损害原生推理能力。ThinkSafe 提出了一种无需外部教师的自生成对齐框架：关键洞察是模型虽然顺从性增强，但仍保留识别有害内容的潜在知识。框架通过轻量级拒绝引导让模型自行生成分布内的安全推理链，再在这些自生成响应上微调，实现安全对齐的同时最小化分布偏移。在 DeepSeek-R1-Distill 和 Qwen3 上的实验表明，ThinkSafe 显著提升安全性并保留推理水平，计算成本远低于 GRPO。

- **ReGuLaR: Variational Latent Reasoning Guided by Rendered Chain-of-Thought** `[微调]` `[VLM]` — [2601.23184](https://arxiv.org/abs/2601.23184) | [GitHub](https://github.com/FanmengWang/ReGuLaR)
  > 链式思维（CoT）大幅提升 LLM 推理性能，但显式推理链引入大量计算冗余；现有潜在推理方法又因缺乏合适的压缩引导而性能严重下降。ReGuLaR 在变分自编码（VAE）框架下形式化潜在推理：当前潜在推理状态从以历史状态为条件的后验分布中采样。训练时将显式推理链渲染为图像，提取稠密视觉语义表示来正则化后验分布，实现信息损失最小的高效压缩。大量实验表明，ReGuLaR 在计算效率和推理效果上均大幅超越现有潜在推理方法，甚至通过多模态推理超越了标准 CoT，为潜在推理提供了新颖且有洞察力的解决方案。

- **TTCS: Test-Time Curriculum Synthesis for Self-Evolving** `[RL]` — [2601.22628](https://arxiv.org/abs/2601.22628) | [GitHub](https://github.com/XMUDeepLIT/TTCS)
  > 测试时训练（TTT）可通过仅利用测试问题来提升 LLM 推理能力，但测试问题往往过难、测试集规模有限，导致伪标签质量不稳定。TTCS 提出了一种协同进化测试时训练框架，由同一预训练模型初始化问题合成器和推理求解器两个策略，通过迭代优化共同进化：合成器根据测试问题生成渐进困难的课程变体，求解器则利用多样本自一致性奖励进行在线自进化，两者形成闭环反馈。实验证明 TTCS 在挑战性数学基准上持续提升不同 LLM 骨干的推理能力，并可迁移至通用任务，是一条通过动态测试时课程实现自进化的可扩展路径。

- **Do Reasoning Models Enhance Embedding Models?** `[RL]` `[微调]` — [2601.21192](https://arxiv.org/abs/2601.21192) | [GitHub](https://github.com/HKUST-KnowComp/Reasoning-Embedding)
  > 当前最先进的嵌入模型越来越多地从仅解码器 LLM 主干通过对比学习适配而来。随着 RLVR 推理模型的兴起，一个自然问题是：以推理模型为嵌入初始化是否能产生更优的语义表示？出乎预料，作者在 MTEB 和 BRIGHT 上的评估揭示了「零效果」：以 RLVR 调优主干初始化的嵌入模型，在相同训练配方下相比基础模型无一致性能提升。为解析这一悖论，作者引入层级表示相似性分析框架（HRSA），分析发现 RLVR 导致局部几何重组（不可逆）和坐标基漂移（可逆），但保留全局流形几何与线性读出，随后对比学习驱动两者强对齐，形成「流形重对齐」现象。

- **MemOCR: Layout-Aware Visual Memory for Efficient Long-Horizon Reasoning** `[RL]` `[VLM]` `[长文本]` — [2601.21468](https://arxiv.org/abs/2601.21468) | [GitHub](https://github.com/meituan/MemOCR)
  > 长时域智能体推理需要将不断增长的交互历史有效压缩到有限上下文窗口内，而现有记忆系统将历史序列化为文本导致 token 成本线性增长。MemOCR 是一个多模态记忆智能体，通过视觉布局实现自适应信息密度的记忆空间分配：维护结构化富文本记忆（含标题、高亮等），将其渲染为图像供智能体检索，以视觉方式突出关键证据同时激进压缩辅助细节。为确保在不同记忆预算下的鲁棒性，使用强化学习在预算感知目标下训练 MemOCR，使智能体适应多样压缩级别。在长上下文多跳和单跳问答基准上，MemOCR 超越强大的文本基线，在极端预算下实现更有效的上下文利用。

- **FourierSampler: Unlocking Non-Autoregressive Potential in Diffusion Language Models via Frequency-Guided Generation** `[无需训练]` — [2601.23182](https://arxiv.org/abs/2601.23182) | [GitHub](https://github.com/ShirleYoung/FourierSampler)
  > 扩散语言模型（dLLMs）具有非自回归生成潜力，但现有解码策略存在位置偏差，未能充分发挥任意顺序生成的优势。本文首次对 dLLMs 进行频域分析，发现隐状态中低频分量主要编码全局结构信息和长程依赖，高频分量负责局部细节。基于此，提出 FourierSampler：利用频域滑动窗口机制动态引导模型实现「结构→细节」的渐进式生成。在 LLaDA 和 SDAR 上，FourierSampler 超越其他推理增强策略，在 LLaDA1.5-8B 上实现 20.4% 的相对提升，在 LLaDA-8B-Instruct 上提升 16.0%，明显超过同规模自回归模型 Llama3.1-8B-Instruct。

- **NativeTok: Native Visual Tokenization for Improved Image Generation** `[微调]` `[VLM]` — [2601.22837](https://arxiv.org/abs/2601.22837) | [GitHub](https://github.com/wangbei1/Nativetok)
  > VQ 图像生成通常采用两阶段流程：分词器编码离散 token，生成模型学习其依赖关系。然而现有方法不约束 token 依赖关系，导致生成模型面临无序分布，产生偏差与弱一致性。本文提出「原生视觉分词化」，在分词阶段即强制因果依赖关系。NativeTok 框架包含：元图像 Transformer（MIT）用于潜变量图像建模；混合因果专家 Transformer（MoCET），每个轻量级专家块基于历史 token 和潜变量特征生成单个 token；层级原生训练策略仅更新新专家块，确保训练效率。大量实验验证了 NativeTok 的有效性。

- **Scaling Multiagent Systems with Process Rewards** `[RL]` `[微调]` — [2601.23228](https://arxiv.org/abs/2601.23228) | [GitHub](https://github.com/ltjed/multiagent-coaching)
  > 多智能体系统虽在复杂任务上展现出分工协作的潜力，但同时微调多个智能体面临信用分配和昂贵多智能体 rollout 样本效率两大挑战。本文提出 MAPPA（来自 AI 反馈的每动作过程奖励微调多智能体系统），通过对每个智能体动作单独分配信用而非仅在任务完成时给予奖励，在无需真实标签的前提下实现细粒度监督并最大化每次 rollout 的训练信号。在竞赛数学题上，MAPPA 在 AIME 和 AMC 分别提升 5.0-17.5pp 和 7.8-17.2pp；在数据分析任务上成功率提升 12.5pp，质量指标改善高达 30%。

- **TAM-Eval: Evaluating LLMs for Automated Unit Test Maintenance** `[微调]` — [2601.18241](https://arxiv.org/abs/2601.18241) | [GitHub](https://github.com/trndcenter/TAM-Eval)
  > 现有 LLM 在软件测试领域的应用主要局限于孤立的测试生成或预言预测，忽视了测试套件维护这一更广泛挑战。TAM-Eval 提出一个评估框架与基准，涵盖测试套件的创建、修复和更新三个核心维护场景，在测试文件级别（而非函数级别）运作，同时支持访问完整仓库上下文以贴近真实工作流。基准包含从 Python、Java 和 Go 项目中自动抽取并验证的 1,539 个场景，采用基于测试套件通过率、代码覆盖率和变异测试的无参考评估协议。实验表明当前最先进 LLM 在现实测试维护流程中能力有限，测试有效性提升边际。

- **LMK > CLS: Landmark Pooling for Dense Embeddings** `[微调]` `[长文本]` — [2601.21525](https://arxiv.org/abs/2601.21525) | [GitHub](https://github.com/meetdoshi90/LMK-Pooling)
  > 表示学习对搜索、聚类、分类和重排序等下游任务至关重要。现有序列编码器通常使用 [CLS] token 或均值池化将变长序列压缩为单向量：[CLS] 倾向于向序列头部集中信息导致证据表示不均衡，均值池化会稀释显著的局部信号。本文提出 Landmark（LMK）池化：将序列分割为若干块，在块间插入 landmark token，最后对 landmark token 嵌入取均值作为最终表示。该简单机制在不牺牲局部显著特征的前提下改善了长上下文外推，仅增加少量特殊 token。实验表明 LMK 池化在短上下文检索任务上持平现有方法，并在长上下文任务上取得大幅提升。

- **Why Attention Patterns Exist: A Unifying Temporal Perspective Analysis** `[无需训练]` `[MeM]` — [2601.21709](https://arxiv.org/abs/2601.21709) | [GitHub](https://github.com/MIRALab-USTC/LLM-TAPPA)
  > 注意力模式（检索头、sink 头、对角迹等）对 LLM 训练与推理至关重要，但现有观察零散且缺乏统一解释。本文提出时序注意力模式可预测性分析（TAPPA）框架，从时域连续视角分析各注意力模式的数学形式，将其分为具有清晰规律的「可预测模式」和近似随机的「不可预测模式」，并证明此区别可用 query 在时序维度的自相似度（q-similarity）来量化。对可预测模式的详细数学分析揭示了 query、key 及旋转位置编码（RoPE）的联合作用机制。将 TAPPA 的洞察应用于 KV 缓存压缩和 LLM 剪枝，以 q-similarity 为信号的简单指标一致超越基线方法，在 Qwen2.5 KV 压缩上相比 EA 提升最高 11.34 分。

- **KAPSO: A Knowledge-grounded framework for Autonomous Program Synthesis and Optimization** `[无需训练]` — [2601.21526](https://arxiv.org/abs/2601.21526) | [GitHub](https://github.com/Leeroo-AI/kapso)
  > KAPSO 是一个用于自主程序合成与优化的模块化框架：给定自然语言目标和评估方法，在长时域优化循环中迭代执行构思、代码合成与编辑、执行、评估和学习。框架以合成为算子、以评估者结果定义进展，通过三个紧耦合组件攻克编码智能体的常见长时域失败：git 原生实验引擎将每次尝试隔离为分支以保证可复现性；知识系统将仓库、内部手册和外部资源组织为支持工作流与实现检索的结构化表示；认知记忆层维护从实验追踪中提炼的可复用经验，降低重复错误并加速收敛。在 MLE-Bench 和 ALE-Bench 上评估均取得最先进性能。

- **Machine Learning for Energy-Performance-aware Scheduling** — [2601.23134](https://arxiv.org/abs/2601.23134) | [GitHub](https://github.com/PeterHUistyping/ml-cpu-sched)
  > 后 Dennard 时代嵌入式系统优化需要在能效和延迟之间权衡，传统启发式调优在高维非平滑搜索空间中效率低下。本文提出基于高斯过程的贝叶斯优化框架，自动化搜索异构多核架构的最优调度配置，并通过帕累托前沿显式建模能耗与时间的多目标权衡。通过引入灵敏度分析（fANOVA）并比较不同协方差核（Matérn vs. RBF），为黑盒模型提供物理可解释性，揭示驱动系统性能的主导硬件参数。

## 2026年2月3日

- **Closing the Loop: Universal Repository Representation with RPG-Encoder** `[无需训练]` — [2602.02084](https://arxiv.org/abs/2602.02084) | [GitHub](https://github.com/microsoft/RPG-ZeroRepo)
  > RPG-Encoder 是一个代码仓库理解框架，将仓库「生成」与「理解」视为统一循环中的互逆过程。框架通过三个机制闭合推理环路：(1) 将原始代码编码为融合语义特征与依赖关系的 Repository Planning Graph（RPG）；(2) 增量拓扑更新，将维护成本降低 95.7%；(3) 提供结构感知的统一导航接口。评估表明，RPG-Encoder 在 SWE-bench Verified 上以 93.7% Acc@5 达到最优仓库理解性能，在 SWE-bench Live Lite 上超越最优基线 10% 以上，并在 RepoCraft 上实现 98.5% 重建覆盖率，验证了 RPG 对代码库的高保真镜像能力。

- **FS-Researcher: Test-Time Scaling for Long-Horizon Research Tasks with File-System-Based Agents** `[长文本]` — [2602.01566](https://arxiv.org/abs/2602.01566) | [GitHub](https://github.com/Ignoramus0817/FS-Researcher)
  > FS-Researcher 是一个基于文件系统的双智能体框架，用于突破上下文窗口限制的深度研究任务。Context Builder 智能体充当「图书馆员」，浏览互联网、写结构化笔记、将原始资料归档至层次化知识库；Report Writer 智能体逐节撰写报告，将知识库作为事实来源。文件系统作为持久外部记忆和跨智能体协调媒介，支持超越上下文窗口的迭代精炼。在 DeepResearch Bench 和 DeepConsult 两个基准上，FS-Researcher 在不同骨干模型下均达到最优报告质量，且最终质量与 Context Builder 计算量正相关，验证了文件系统范式下的有效测试时扩展。

- **PixelGen: Pixel Diffusion Beats Latent Diffusion with Perceptual Loss** `[无需训练]` — [2602.02493](https://arxiv.org/abs/2602.02493) | [GitHub](https://github.com/Zehong-Ma/PixelGen)
  > PixelGen 提出了一个带感知监督的像素扩散框架，直接在像素空间端到端生成图像，避免了两阶段潜在扩散中 VAE 引入的伪影和瓶颈。框架引入两种互补感知损失：LPIPS 损失促进更好的局部模式学习，DINO 感知损失强化全局语义。实验表明，PixelGen 仅训练 80 个 epoch 即在 ImageNet-256 上取得 FID 5.11（无 CFG），在大规模文本到图像生成上 GenEval 评分为 0.79，超越强潜在扩散基线。无需 VAE、无潜在表示、无辅助阶段，提供更简洁且更强的生成范式。

- **Thinking with Comics: Enhancing Multimodal Reasoning through Structured Visual Storytelling** `[VLM]` `[长文本]` — [2602.02453](https://arxiv.org/abs/2602.02453) | [GitHub](https://github.com/andongBlue/Think-with-Comics)
  > 本文提出「Thinking with Comics」视觉推理范式，将漫画作为介于图像与视频之间的高信息密度媒介。漫画保留时序结构、嵌入文本和叙事连贯性，同时推理成本远低于视频。研究系统探讨了两种基于漫画的推理路径，并在多种推理任务和长上下文理解任务上进行评估。实验结果表明，Thinking with Comics 在多步时序与因果推理任务上优于 Thinking with Images，且效率大幅高于 Thinking with Video。进一步分析揭示不同漫画叙事结构和风格对各任务性能有一致性影响，证明漫画是提升多模态推理的有效中间视觉表示。

- **RLAnything: Forge Environment, Policy, and Reward Model in Completely Dynamic RL System** `[RL]` — [2602.02488](https://arxiv.org/abs/2602.02488) | [GitHub](https://github.com/Gen-Verse/Open-AgentRL)
  > RLAnything 是一个动态强化学习框架，通过闭环优化同时锻造环境、策略和奖励模型，适用于任意 LLM 或 Agent 场景。策略通过步骤级和结果级反馈联合训练；奖励模型通过一致性反馈联合优化，进而改善策略训练；理论驱动的自动环境适应则利用来自奖励和策略两侧的评论反馈改进训练。实验表明，各组件逐步提升整体系统性能，Qwen3-VL-8B-Thinking 在 OSWorld 上提升 9.1%，Qwen2.5-7B-Instruct 在 AlfWorld 和 LiveBench 上分别提升 18.7% 和 11.9%。

- **Wiki Live Challenge: Challenging Deep Research Agents with Expert-Level Wikipedia Articles** — [2602.01590](https://arxiv.org/abs/2602.01590) | [GitHub](https://github.com/WangShao2000/Wiki_Live_Challenge)
  > Wiki Live Challenge（WLC）是一个以最新维基百科「优质文章」（Good Articles）为专家级参考的实时基准，用于评估深度研究智能体。现有评估框架依赖 LLM 生成的参考内容，缺乏可靠性和细粒度评估。WLC 整合了 100 篇近期优质文章数据集，并提出 Wiki Eval 评估框架，包含 39 项写作质量标准和严格的事实可核查性指标。在多个深度研究智能体系统上的广泛实验表明，当前系统与人类专家水平的维基百科文章之间仍存在显著差距。

- **SLIME: Stabilized Likelihood Implicit Margin Enforcement for Preference Optimization** `[微调]` `[RL]` — [2602.02383](https://arxiv.org/abs/2602.02383) | [GitHub](https://github.com/fpsigma/trl-slime)
  > SLIME 是一种无参考对齐目标，旨在解耦偏好学习与生成质量。现有直接偏好优化方法存在「目标错配」问题：优化相对边际并不保证保留偏好响应的绝对概率，导致「遗忘」高质量输出和「格式崩溃」。SLIME 采用三重目标：(1) 锚定项最大化偏好响应概率；(2) 稳定惩罚防止被拒绝 token 概率塌零；(3) 软硬双边际机制实现精确边界整形。实验结果表明，SLIME 在保持更高生成稳定性的同时，性能优于最先进基线。

- **Mind-Brush: Integrating Agentic Cognitive Search and Reasoning into Image Generation** `[VLM]` `[无需训练]` — [2602.01756](https://arxiv.org/abs/2602.01756) | [GitHub](https://github.com/PicoTrex/Mind-Brush)
  > Mind-Brush 是一个将「思考-检索-创作」范式融入图像生成的统一 Agent 框架，弥补现有模型在分布外概念和复杂知识推理上的不足。框架通过主动检索多模态证据锚定陌生概念，并使用推理工具解决隐式视觉约束。为严格评估相关能力，提出 Mind-Bench 基准，含 500 个涉及实时新闻、新兴概念、数学与地理推理的样本。实验表明，Mind-Brush 显著提升统一模型能力，在 Mind-Bench 上将 Qwen-Image 基线从零分大幅提升，并在 WISE 和 RISE 等基准上取得领先结果。

- **RE-TRAC: REcursive TRAjectory Compression for Deep Search Agents** `[长文本]` `[微调]` — [2602.02486](https://arxiv.org/abs/2602.02486) | [GitHub](https://github.com/microsoft/InfoAgent)
  > RE-TRAC 是一个通过跨轨迹探索改进深度研究 Agent 的框架，针对 ReAct 线性设计在长上下文下的局部最优、冗余探索和低效搜索问题。框架在每条轨迹结束后生成结构化状态表示，总结证据、不确定性、失败原因和未来规划，并以此引导后续轨迹，将研究重构为渐进式过程。实验表明，Re-TRAC 在 BrowseComp 上以前沿 LLM 持续超越 ReAct 15-20%；针对小模型引入 Re-TRAC 感知监督微调，在同等规模下达到最先进性能，且工具调用和 token 用量随轮次单调递减。

- **CUA-Skill: Develop Skills for Computer Using Agent** `[MeM]` — [2601.21123](https://arxiv.org/abs/2601.21123) | [GitHub](https://github.com/microsoft/cua_skill)
  > CUA-Skill 是一个面向计算机操作 Agent 的大规模技能库，将人类计算机操作知识编码为带参数化执行和组合图的技能，覆盖常见 Windows 应用。基于此技能库构建的 CUA-Skill Agent 支持动态技能检索、参数实例化和记忆感知故障恢复。实验表明，CUA-Skill 显著提升端到端 Agent 基准上的执行成功率与鲁棒性；在 WindowsAgentArena 上，CUA-Skill Agent 以 57.5%（best of three）成功率达到最先进水平，同时效率显著优于现有方案。

- **LoopViT: Scaling Visual ARC with Looped Transformers** `[无需训练]` — [2602.02156](https://arxiv.org/abs/2602.02156) | [GitHub](https://github.com/WenjieShu/LoopViT)
  > LoopViT 提出了一种递归架构，通过权重共享循环将推理深度与模型参数量解耦，以实现视觉归纳推理。模型迭代执行一个结合局部卷积和全局注意力的权重共享混合块，形成隐式「思维链」。关键创新是基于预测熵的无参数 Dynamic Exit 机制：当内部状态「结晶」为低不确定性吸引子时停止推理。在 ARC-AGI-1 基准上，仅 18M 参数的 LoopViT 达到 65.8% 准确率，超越 73M 参数集成模型，表明自适应迭代计算是视觉推理更高效的扩展轴。

- **Training LLMs for Divide-and-Conquer Reasoning Elevates Test-Time Scalability** `[RL]` — [2602.02477](https://arxiv.org/abs/2602.02477) | [GitHub](https://github.com/MasterVito/DAC-RL)
  > 本文提出一个端到端强化学习框架，训练 LLM 进行分治（DAC）式推理，弥补通用后训练与 DAC 推理之间的根本性错位。框架在每步中将问题分解为子问题并顺序求解，分解和求解均纳入 RL 训练。相比 CoT，DAC 风格框架赋予模型更高性能上限和更强测试时扩展性，在竞赛级基准上 Pass@1 提升 8.6%、Pass@32 提升 6.3%。分析揭示了通用后训练与 DAC 推理之间的根本性错位，并证明 RL 训练是解锁 DAC 潜力的有效途径。

- **Show, Don't Tell: Morphing Latent Reasoning into Image Generation** `[RL]` `[VLM]` — [2602.02227](https://arxiv.org/abs/2602.02227) | [GitHub](https://github.com/EnVision-Research/LatentMorph)
  > LatentMorph 将隐式潜在推理无缝整合到文本到图像生成过程中，避免了显式推理范式中文本解码与图像反复编解码的低效和信息损失。核心组件包括：将中间生成状态压缩为紧凑视觉记忆的 condenser、将潜在思维转为可操作引导的 translator、动态引导下一 token 预测的 shaper，以及 RL 训练的 invoker 自适应决定何时触发推理。实验表明，LatentMorph 在 GenEval 上提升基础模型 Janus-Pro 16%，在抽象推理任务上超越显式范式 11-15%，同时推理时间减少 44%、token 消耗减少 51%。

- **PromptRL: Prompt Matters in RL for Flow-Based Image Generation** `[RL]` `[微调]` — [2602.01382](https://arxiv.org/abs/2602.01382) | [GitHub](https://github.com/G-U-N/UniRL)
  > PromptRL 发现当前流匹配模型 RL 后训练管线存在两个被忽视的问题：生成多样性不足导致的样本低效，以及提示过拟合（prompt overfitting）。框架将语言模型作为可训练提示精炼 Agent 直接嵌入 RL 优化循环，在开发复杂提示改写能力的同时形成协同训练机制，重塑优化动态。PromptRL 在 GenEval 上评分 0.97，OCR 准确率 0.98，PickScore 24.05，达到最先进水平；在图像编辑模型上验证有效性，以仅 0.06M rollout 将 FLUX.1-Kontext 的 EditReward 从 1.19 提升至 1.43，超越 Gemini 2.5 Flash Image。

- **CoDiQ: Test-Time Scaling for Controllable Difficult Question Generation** `[微调]` — [2602.01660](https://arxiv.org/abs/2602.01660) | [GitHub](https://github.com/ALEX-nlp/CoDiQ)
  > CoDiQ 是一个通过测试时扩展实现可控难题生成的框架，解决现有自动化题目合成方法缺乏精确难度控制、计算成本高、难以规模化生成竞赛级题目的问题。框架识别测试时扩展规律（更多推理 token 提升难度但降低可解性）和模型生成有效高难度题目的内在上限，并开发 CoDiQ-Generator（基于 Qwen3-8B）。基于此构建 CoDiQ-Corpus（44K 竞赛级题目序列），人工评估显示题目难度显著超越 LiveCodeBench/AIME，可解性超 82%。在 CoDiQ-Corpus 上训练 LRM 显著提升推理性能。

- **Hunt Instead of Wait: Evaluating Deep Data Research on Large Language Models** — [2602.02039](https://arxiv.org/abs/2602.02039) | [GitHub](https://github.com/thinkwee/DDR_Bench)
  > 本文提出「深度数据研究」（DDR）任务，要求 LLM 从原始数据库中自主提取关键洞察，区分「调查型智能」（主动设目标、决定探索方向）与「执行型智能」（完成指定任务）。DDR-Bench 是一个基于核查清单的大规模可验证评估基准。实验结果显示，前沿模型表现出初步的自主性，但长视野探索仍具挑战。分析表明，有效的调查型智能不仅取决于 Agent 脚手架或规模扩展，还依赖于 Agent 模型的内在策略。

- **Rethinking LLM-as-a-Judge: Representation-as-a-Judge with Small Language Models via Semantic Capacity Asymmetry** `[无需训练]` — [2601.22588](https://arxiv.org/abs/2601.22588) | [GitHub](https://github.com/zhuochunli/Representation-as-a-judge)
  > 本文提出「Representation-as-a-Judge」范式，探索用小语言模型的内部表示替代大模型作为评估器。研究发现一致性经验规律：小 LM 尽管生成能力弱，但其隐藏状态编码了丰富的评估信号。由此提出「语义容量不对称假说」：评估所需语义容量远小于生成，可基于中间表示完成。基于此范式实例化 INSPECTOR，一个从小模型表示预测方面级评分的探针框架。在 GSM8K、MATH、GPQA 推理基准上，INSPECTOR 大幅优于基于提示的小 LM，接近完整 LLM 评判，同时更高效、可靠、可解释。

- **On the Limits of Layer Pruning for Generative Reasoning in LLMs** `[微调]` — [2602.01997](https://arxiv.org/abs/2602.01997) | [GitHub](https://github.com/safal312/on-the-limits-of-layer-pruning)
  > 本文系统研究层剪枝对 LLM 生成推理任务的影响。研究发现，尽管层剪枝在分类基准上表现良好，但多步推理任务对深度缩减极为敏感，导致算术计算和代码合成等关键算法能力退化。在现实后训练约束下，评估了基于自生成响应监督微调的缓解策略：该方案在分类任务上恢复高达 90% 基线性能，在生成基准上提升 20-30 个百分点，但生成推理恢复仍根本受限于分类任务，且仅在较低剪枝比例下可行，为实际应用提供了重要边界指导。


## 2026年2月4日

- **CodeOCR: A Transformer-Based Code Understanding via Optical Character Recognition** `[VLM]` — [2602.01785](https://arxiv.org/abs/2602.01785) | [GitHub](https://github.com/YerbaPage/CodeOCR)
  > 大型语言模型在代码理解上表现出色，但随着软件系统规模增长，基于文本的线性token处理方式导致上下文长度线性增加，计算效率成为瓶颈。本文提出CodeOCR，将源代码理解转化为视觉识别任务，通过OCR-based视觉编码方式处理代码，从而大幅降低token数量。实验表明，CodeOCR在多个代码理解基准上与传统文本模型相当，同时显著减少计算开销，为VLM处理大规模代码提供了新范式。

- **AOrchestra: A Unified Framework-Agnostic Agent Abstraction for Multi-Agent Systems** — [2602.03786](https://arxiv.org/abs/2602.03786) | [GitHub](https://github.com/FoundationAgents/AOrchestra)
  > 语言智能体在任务自动化上展现出强大潜力，但面向复杂长时任务时，现有的「sub-agent即工具」范式缺乏对子智能体的动态抽象能力，影响灵活性。AOrchestra提出了一种统一的、框架无关的智能体抽象方案，将子智能体视为可组合的动态模块，支持跨框架多智能体协作与调度。实验表明，该框架在长时任务上显著提升了任务成功率，且无需修改底层框架即可集成。

- **There Is No Global Plan in Chain-of-Thought: Studying the Dynamics of LLM Reasoning with Telescope Lens** — [2602.02103](https://arxiv.org/abs/2602.02103) | [GitHub](https://github.com/lxucs/tele-lens)
  > 本文深入研究链式思维（CoT）的动态机制，发现LLM在CoT生成前已有潜在规划，但该规划并不等同于「全局计划」。通过「Telescope Lens」方法分析LLM内部状态与外部推理步骤的关系，揭示CoT对多步推理至关重要，但不存在固定的全局预规划结构。研究结果对理解LLM推理机制及优化CoT训练方法具有重要意义，为设计更高效的推理模型提供了理论依据。

- **daVinci Agency: Synthesizing Long-Horizon Agentic Data via Cross-Stage Dependency** `[微调]` — [2602.02619](https://arxiv.org/abs/2602.02619) | [GitHub](https://github.com/GAIR-NLP/daVinci-Agency)
  > LLM在短任务上表现出色，但扩展到长时智能体工作流仍面临训练数据稀缺的挑战。daVinci Agency提出了一种合成方法，通过捕获跨阶段依赖结构来生成具有真实长依赖特性的训练数据，突破了现有方法局限于单特征场景或成本过高的瓶颈。实验表明，使用该合成数据训练的智能体在长时任务上实现了显著提升，有效弥合了短任务表现与长时任务能力之间的差距。

- **SWE-World: Building Software Engineering Agents in Docker-Free Environments** `[RL]` — [2602.03419](https://arxiv.org/abs/2602.03419) | [GitHub](https://github.com/RUCAIBox/SWE-World)
  > 现有软件工程智能体大多依赖容器化环境提供执行反馈，资源密集且维护困难。SWE-World提出在无Docker环境下构建软件工程智能体的方法，通过轻量级的代码静态分析与模拟执行替代真实容器，降低了部署门槛。实验表明，在SWE-Bench等标准评测上，该方法与依赖Docker的方法性能相当，同时大幅降低了资源消耗和环境配置难度，使SE智能体部署更加普及。

- **SWE-Master: Unleashing the Potential of Software Engineering Agents via Post-Training** `[微调]` `[RL]` — [2602.03411](https://arxiv.org/abs/2602.03411) | [GitHub](https://github.com/RUCAIBox/SWE-Master)
  > SWE-Master是一个开源可复现的软件工程智能体后训练框架，系统探索了完整的智能体开发流程，包括教师轨迹合成与数据整理、长时SFT、基于真实执行反馈的RL以及推理框架设计。从开源基础模型出发，SWE-Master在SWE-Bench Verified上取得了有竞争力的成绩，充分展示了后训练方法在提升软件工程智能体能力上的潜力，并提供了完整的可复现代码和数据。

- **Parallel-Probe: Towards Efficient Parallel Thinking via 2D Probing** `[无需训练]` — [2602.03845](https://arxiv.org/abs/2602.03845) | [GitHub](https://github.com/zhengkid/Parallel-Probe)
  > 并行思维作为一种推理范式具有潜力，但计算开销巨大。现有效率方法主要依赖局部的单轨迹信号，缺乏利用全局并行分支动态的机制。本文提出2D Probing接口，通过周期性探测暴露并行思维的宽度-深度动态，使系统能够在全局视角下自适应分配计算资源。实验表明，Parallel-Probe在保持推理质量的同时，相比基线方法显著降低了并行推理的计算成本。

- **Bridging Online and Offline RL: Contextual Bandit Learning for Multi-Turn Code Generation** `[RL]` — [2602.03806](https://arxiv.org/abs/2602.03806) | [GitHub](https://github.com/OSU-NLP-Group/cobalt)
  > 在线RL训练效果更优但成本高且不稳定，离线RL成本低但效果受限。本文观察到多轮代码生成可建模为单步可恢复马尔可夫决策过程，提出Cobalt方法——利用参考LLM收集轨迹后将其分割为上下文提示，再通过单步在线bandit学习完成轨迹。Cobalt超越了基于GRPO和VeRPO的多轮在线RL基线，在LiveCodeBench上将R1-Distill 8B和Qwen3 8B的Pass@1分别提升9.0和6.2个绝对值，同时分析了上下文奖励攻击问题并提出缓解方案。

- **Glance and Focus Reinforcement for Pan-cancer Screening** `[RL]` — [2601.19103](https://arxiv.org/abs/2601.19103) | [GitHub](https://github.com/Luffy03/GF-Screen)
  > 大规模CT扫描中的泛癌症筛查面临极端前后景不平衡的挑战，现有AI方法难以定位多种类型的微小病变。本文提出「扫视与聚焦」强化学习框架，先粗粒度扫描定位候选区域，再精细聚焦分析，有效解决了大体积CT中病灶检测的效率与精度问题。在多癌症类型的大规模CT数据集上，该方法显著优于现有方法，展示了RL在医学图像分析中的应用潜力。

- **Contextualized Visual Personalization in Vision-Language Models** `[RL]` `[VLM]` — [2602.03454](https://arxiv.org/abs/2602.03454) | [GitHub](https://github.com/oyt9306/CoViP)
  > 现有VLM方法难以基于用户特定视觉经验生成个性化回复，缺乏将视觉输入与用户积累视觉-文本上下文关联的能力。本文将此挑战正式化为「上下文化视觉个性化」问题，提出CoViP统一框架，包含新颖的个性化图像描述基准、基于RL的后训练方案和下游个性化诊断任务。实验表明，CoViP在个性化视觉理解和生成任务上显著优于基线，为VLM个性化能力的评估和提升建立了系统性方法。

- **SimpleGPT: Improving GPT via A Simple Normalization Strategy** `[微调]` — [2602.01212](https://arxiv.org/abs/2602.01212) | [GitHub](https://github.com/Ocram7/SimpleGPT)
  > 本文从二阶几何视角重新审视Transformer优化，建立了架构设计、激活尺度、Hessian矩阵与最大可容忍学习率之间的直接联系。提出SimpleNorm归一化策略，通过构造稳定中间激活尺度来提升训练稳定性。在大规模GPT预训练实验中，SimpleGPT在多个语言建模基准上取得改进，同时简化了架构设计，无需复杂调参即可获得更稳定的训练动态和更优的模型性能。

- **MedSAM-Agent: Empowering Interactive Medical Image Segmentation with Multi-turn Agentic Reinforcement Learning** `[RL]` — [2602.03320](https://arxiv.org/abs/2602.03320) | [GitHub](https://github.com/CUHK-AIM-Group/MedSAM-Agent)
  > 医学图像分割正从任务特定模型向通用框架演进。本文提出MedSAM-Agent，基于多模态大语言模型作为自主智能体，采用可验证奖励的强化学习（RLVR）协调SAM等专业工具，支持多轮交互式分割。与现有依赖单轮、固定交互策略的方法不同，MedSAM-Agent能自适应地进行多步推理和工具调用，在多种医学图像分割任务上达到先进水平，展示了RLVR在医疗AI中的应用潜力。

- **LRAgent: Efficient KV Cache Sharing for Multi-LoRA LLM Agents** `[无需训练]` — [2602.01053](https://arxiv.org/abs/2602.01053) | [GitHub](https://github.com/hjeon2k/LRAgent)
  > 多LLM智能体系统中，角色专化通常通过多LoRA实现，但各智能体对相同的长工具轨迹独立构建KV缓存，导致内存和计算开销巨大。LRAgent提出高效KV缓存共享框架，将预训练权重产生的高度相似基础缓存进行共享，同时保留LoRA适配器产生的轻量低秩缓存。实验表明，LRAgent在多LoRA多智能体系统中显著降低了内存占用和延迟，同时保持了各智能体的专有推理能力。

- **Privasis: Synthesizing the Largest "Public" Private Dataset from Scratch** `[微调]` — [2602.03183](https://arxiv.org/abs/2602.03183) | [GitHub](https://github.com/skywalker023/privasis)
  > 隐私敏感数据研究长期受数据稀缺制约，与其他受益于数据规模化的领域形成对比。随着现代AI智能体获得对敏感个人信息的持久访问权，该问题愈发紧迫。Privasis从头合成迄今最大规模的「公开」隐私数据集，通过生成既遵循真实隐私模式又不含真实个人信息的合成数据，为隐私保护研究提供数据基础。实验验证了合成数据在训练和评估隐私感知AI系统方面的有效性。

- **FullStack-Agent: Enhancing Agentic Full-Stack Web Coding via Development-Oriented Testing and Repository Back-Translation** `[微调]` — [2602.03798](https://arxiv.org/abs/2602.03798) | [GitHub](https://github.com/mnluzimu/FullStack-Agent)
  > 帮助非专业用户开发复杂交互式网站是LLM驱动代码智能体的热门任务，但现有方法倾向于仅生成前端页面，掩盖了对真实全栈数据处理和存储的缺失。FullStack-Agent提出统一系统，结合多智能体开发框架（FullStack-Dev）、通过仓库增强和回翻译的自我改进方法（FullStack-Learn），以及全栈开发基准（FullStack-Bench）。以Qwen3-Coder-480B为骨干，在前后端和数据库测试上分别达64.7%/77.8%/77.9%，超越SOTA 8.7/38.2/15.9个点。

- **Decouple Searching from Training: Scaling Data Mixing via Model Merging for Large Language Model Pre-training** `[微调]` — [2602.00747](https://arxiv.org/abs/2602.00747) | [GitHub](https://github.com/Lucius-lsr/DeMix)
  > 确定有效的数据混合比例是LLM预训练的关键因素，但现有方法或依赖不可靠的小规模代理实验，或需要昂贵的大规模搜索。DeMix将搜索与训练解耦：先训练多个数据集各自的小型模型，再通过模型合并探索数据混合空间，无需对整体模型重复训练。实验表明，DeMix能以低成本找到接近最优的数据混合比例，在多个下游任务上提升了LLM预训练质量，显著降低了数据配方搜索的计算成本。

- **LycheeDecode: Accelerating Long-Context LLM Inference via Hybrid-Head Sparse Decoding** `[长文本]` `[无需训练]` — [2602.04541](https://arxiv.org/abs/2602.04541) | [GitHub](https://github.com/HITsz-TMG/TMGNLP)
  > 长上下文LLM推理面临KV缓存访问带宽瓶颈。LycheeDecode提出混合头稀疏解码方法，通过区分不同注意力头的稀疏性需求——部分头使用完整注意力，其余头使用稀疏近似——实现了高效的长上下文推理。实验证明，LycheeDecode在多种长上下文任务上保持了接近全注意力的准确率，同时将解码延迟降低了显著幅度，为长上下文LLM部署提供了实用加速方案。

- **Balancing Understanding and Generation in Discrete Diffusion Models** `[微调]` — [2602.01362](https://arxiv.org/abs/2602.01362) | [GitHub](https://github.com/MzeroMiko/XDLM)
  > 在离散生成建模中，Masked扩散语言模型（MDLM）擅长语义理解和零样本泛化，而均匀噪声扩散语言模型（UDLM）在少步生成质量上更强，但两者均无法在两个维度上均衡表现。本文提出XDLM，桥接两种范式，在同一模型中平衡理解与生成能力。通过设计新颖的混合噪声调度和联合训练目标，XDLM在文本理解和生成基准上均显著优于各自的单一模型基线。

- **ObjEmbed: Towards Universal Multimodal Object Embeddings** `[VLM]` `[无需训练]` — [2602.01753](https://arxiv.org/abs/2602.01753) | [GitHub](https://github.com/WeChatCV/ObjEmbed)
  > 本文提出ObjEmbed，迈向通用多模态对象嵌入表示，使视觉-语言模型能够在统一的嵌入空间中理解和检索任意物体。ObjEmbed通过大规模多模态对比学习，将图像区域和文本描述映射到对齐的嵌入空间，支持跨模态的细粒度对象检索和理解。在多个视觉定位和检索基准上，ObjEmbed相比现有方法取得了显著提升，展示了通用对象嵌入在多模态任务中的广泛应用潜力。

- **SafeGround: Know When to Trust GUI Grounding Models via Uncertainty Calibration** `[VLM]` — [2602.02419](https://arxiv.org/abs/2602.02419) | [GitHub](https://github.com/eric-ai-lab/SAFEGROUND)
  > GUI定位旨在将自然语言指令翻译为可执行的屏幕坐标，但错误定位可能导致难以逆转的高代价操作（如错误付款）。本文提出SafeGround，一种不确定性感知的GUI定位框架，通过不确定性校准判断何时信任定位模型的预测。当不确定性高时，框架选择放弃操作或请求人工确认，从而在保持高成功率的同时显著减少危险错误操作，提升了GUI智能体在真实应用中的可靠性。

- **MEG-XL: Data-Efficient Brain-to-Text via Long-Context Pre-Training** `[长文本]` `[微调]` — [2602.02494](https://arxiv.org/abs/2602.02494) | [GitHub](https://github.com/neural-processing-lab/MEG-XL)
  > 临床脑-文本接口为瘫痪患者设计，但受限于训练数据稀缺。现有预训练方法仅使用数秒的神经上下文，无法捕获语音展开的长时统计规律。MEG-XL提出基于长上下文预训练的脑文本基础模型，每个训练样本使用2.5分钟的MEG上下文，有效学习跨时间尺度的神经统计先验。实验表明，MEG-XL在数据高效场景下的词解码性能显著优于现有方法，为数据稀缺的临床脑机接口应用提供了实用解决方案。

- **You Need an Encoder for Native Position-Independent Caching** `[长文本]` — [2602.01519](https://arxiv.org/abs/2602.01519) | [GitHub](https://github.com/shijuzhao/Comb)
  > LLM的KV缓存基于前缀结构，对无序检索的上下文处理效率极低。位置无关缓存（PIC）旨在实现无位置约束的KV复用，但现有方法往往存在显著的精度退化。本文提出通过引入编码器组件来实现原生PIC，无需改变解码器推理过程即可获得位置无关的KV表示。实验表明，该方法在多种上下文检索场景中，显著优于现有PIC方法，在准确率和推理效率之间取得了更好的平衡。

- **Position: Agentic Evolution is the Path to Evolving LLMs** `[RL]` `[微调]` — [2602.00359](https://arxiv.org/abs/2602.00359) | [GitHub](https://github.com/ventr1c/agentic-evoluiton)
  > 本文提出「智能体进化」作为持续改进LLM的关键路径，通过智能体在开放环境中自主执行任务、收集经验并利用这些经验进行自我优化。文章系统阐述了智能体进化的核心要素：经验收集、质量筛选和迭代训练，并展示了该范式如何解决单纯依赖人工数据标注的可扩展性瓶颈。实验验证了智能体进化在多个任务域中有效提升LLM能力的潜力，为构建持续自我改进的AI系统提供了框架。


## 2026年2月5日

- **FASA: Frequency-aware Sparse Attention** `[长文本]` — [2602.03152](https://arxiv.org/abs/2602.03152) | [GitHub](https://github.com/AMAP-ML/FASA-ICLR2026)
  > FASA 提出了一种频率感知稀疏注意力框架，解决大语言模型处理长文本时 KV 缓存显存开销过大的问题。现有方法要么静态剪枝导致信息不可恢复丢失，要么动态启发式策略无法充分捕捉查询相关的 token 重要性。FASA 通过频率域分析实现查询感知的 token 驱逐，在保持模型性能的同时大幅降低显存占用。实验在多个长文本任务上验证了方法的有效性，该工作已被 ICLR 2026 接收。

- **WideSeek-R1: Exploring Width Scaling for Broad Information Seeking via Multi-Agent Reinforcement Learning** `[RL]` — [2602.04634](https://arxiv.org/abs/2602.04634) | [GitHub](https://github.com/RLinf/RLinf)
  > WideSeek-R1 探索了多智能体系统的「宽度扩展」维度，与现有以单智能体深度推理为主的路线互补。针对广泛信息检索任务，提出通过多智能体强化学习协调并行工作流，取代人工设计的工作流和轮流交互模式。实验表明，在宽广信息检索场景下，宽度扩展比单智能体深度扩展更能有效提升整体性能，为多智能体 RL 系统设计提供了新范式。

- **Training Data Efficiency in Multimodal Process Reward Models** `[VLM]` `[微调]` — [2602.04145](https://arxiv.org/abs/2602.04145) | [GitHub](https://github.com/JinYuanLi0012/Balanced-Info-MPRM)
  > 本文研究多模态过程奖励模型（MPRM）的训练数据效率问题。实验发现现有蒙特卡洛标注语料存在大量冗余，随机下采样快速饱和。作者提出「平衡信息分数（BIS）」，从标签混合度和标签可靠性两个维度对训练样本评分排序，仅用 10% 数据即可匹配全量训练效果，大幅降低 MPRM 训练成本。在多个视觉推理基准上验证了方法的有效性。

- **Rethinking the Trust Region in LLM Reinforcement Learning** `[RL]` `[微调]` — [2602.04879](https://arxiv.org/abs/2602.04879) | [GitHub](https://github.com/sail-sg/Stable-RL)
  > 本文指出 PPO 中的概率比值裁剪机制对大词表 LLM 存在结构性缺陷：低概率 token 的更新被过度惩罚，高概率 token 则惩罚不足，导致学习动态次优。作者提出 DPPO（Direct Policy Optimization with direct divergence），用全变差或 KL 散度直接近似策略分布变化，构建更有原则性的信任域。在 AIME24 等推理任务上，DPPO 显著优于 GRPO 基线，训练稳定性更强。

- **TIDE: Trajectory-based Diagnostic Evaluation of Test-Time Improvement in LLM Agents** `[MeM]` — [2602.02196](https://arxiv.org/abs/2602.02196) | [GitHub](https://github.com/yayayacc/TIDE)
  > TIDE 针对 LLM 智能体的「测试时自我改进（TTI）」能力提出轨迹级诊断评估框架。现有评估指标无法捕捉任务优化效率、错误后行为适应及工作记忆利用率。TIDE 通过分析智能体与环境交互轨迹，提供与智能体架构和环境无关的细粒度诊断。在 ALFWorld、WebShop 等多个环境上的实验揭示了不同 TTI 策略的内在工作机制与失败模式。

- **Residual Context Diffusion Language Models** `[无需训练]` — [2601.22954](https://arxiv.org/abs/2601.22954) | [GitHub](https://github.com/yuezhouhu/residual-context-diffusion)
  > 扩散大语言模型（dLLM）可并行解码多个 token，但现有重掩码机制只保留高置信度 token，丢弃的 token 中仍包含有用的上下文信息。本文提出残差上下文扩散（RCD），将被丢弃 token 的分布转化为上下文残差注入下一去噪步骤，通过两阶段训练避免反向传播的内存开销。在 AIME24/25 等难题基准上，RCD 相比序列去噪（SeqD）一致提升推理准确率，并行度提升 4 倍同时维持峰值精度。

- **Self-Hinting Language Models Enhance Reinforcement Learning** `[RL]` `[微调]` — [2602.03143](https://arxiv.org/abs/2602.03143) | [GitHub](https://github.com/BaohaoLiao/SAGE)
  > SAGE（自提示 GRPO 优化框架）解决 GRPO 在稀疏奖励下因组内优势坍塌导致更新消失的问题。对于模型无法采样到正确轨迹的困难 prompt，SAGE 让模型从参考答案中自生成提示（hint），将该 hint 与原始 prompt 共同作为输入，确保困难样本的正确轨迹被采样用于策略更新。实验表明 SAGE 将困难 prompt 利用率提高约 10%，在多数学推理基准上持续优于 GRPO 基线，且维持相似熵量级。

- **Semantic Routing: Exploring Multi-Layer LLM Feature Weighting for Diffusion Transformers** `[无需训练]` — [2602.03510](https://arxiv.org/abs/2602.03510) | [GitHub](https://github.com/zooblastlbz/SemanticRouting)
  > 语义路由研究如何将 LLM 多层隐状态动态融合用于 DiT 文本到图像模型的文本条件，解决传统单层静态文本条件无法适应 LLM 的语义层次结构与扩散模型非平稳去噪动态的问题。本文提出统一归一化凸融合框架，配备轻量门控机制，系统探索时间维度、深度维度和联合融合策略。实验发现「深度维度语义路由」效果最优，显著提升文本-图像对齐和组合生成能力。

- **AutoFigure: Generating and Refining Publication-Ready Scientific Illustrations** — [2602.03828](https://arxiv.org/abs/2602.03828) | [GitHub](https://github.com/ResearAI/AutoFigure)
  > AutoFigure 是首个从科学文本自动生成出版级别科学插图的智能体框架，配套提出 FigureBench——首个大规模科学插图生成基准，包含 3300 个高质量文本-图像对，覆盖论文、综述、博客和教材等多种来源。AutoFigure 通过迭代精炼机制将 LLM 的长文本理解与代码生成能力结合，输出结构化、可编辑的矢量科学图表。实验表明 AutoFigure 在自动评估和人工评估上均显著超越现有基线。

- **A-RAG: Scaling Agentic Retrieval-Augmented Generation via Hierarchical Retrieval Interfaces** `[无需训练]` — [2602.03442](https://arxiv.org/abs/2602.03442) | [GitHub](https://github.com/Ayanami0730/arag)
  > A-RAG 提出了一种智能体式 RAG 框架，通过分层检索接口（关键词检索、语义检索、片段阅读）让模型参与检索决策，而非依赖单次检索或预定义工作流。前沿语言模型的强推理和长程工具调用能力在现有 RAG 范式中被严重低估。A-RAG 允许模型根据任务需求自主选择检索粒度，在多跳问答任务上达到最优性能，并随模型能力提升实现高效扩展。

- **PaperSearchQA: Learning to Search and Reason over Scientific Papers with RLVR** `[RL]` — [2601.18207](https://arxiv.org/abs/2601.18207) | [GitHub](https://github.com/jmhb0/PaperSearchQA)
  > PaperSearchQA 提出了用于训练科学文献搜索智能体的强化学习环境，专注于生物医学领域的技术问答。系统包含从科学摘要自动生成 QA 数据的流水线（约 60K 样本）和检索语料库，用 RLVR 仅监督最终答案准确率来训练搜索智能体。实验表明训练后的智能体能泛化到未见过的 BioASQ 基准，展现了 RLVR 在专业领域文献搜索推理上的潜力。

- **Horizon-LM: A RAM-Centric Architecture for LLM Training** `[微调]` — [2602.04816](https://arxiv.org/abs/2602.04816) | [GitHub](https://github.com/DLYuanGod/Horizon-LM)
  > Horizon-LM 提出了以 RAM 为核心的 LLM 训练架构，打破训练规模与多 GPU 集群的强耦合。核心思路是将 FP32 主权重存于 CPU 内存，GPU 仅保留 BF16 工作副本，通过 CPU-GPU 协同执行实现单卡训练 120B+ 参数模型。相比 GPU 中心式范式，显著降低了显存需求和分布式运行时复杂度，同时支持 YAML 配置和自动 CUDA 扩展构建，已验证 Qwen2/2.5 全系列模型的训练。

- **MEnvAgent: Scalable Polyglot Environment Construction for Verifiable Software Engineering** — [2601.22859](https://arxiv.org/abs/2601.22859) | [GitHub](https://github.com/ernie-research/MEnvAgent)
  > MEnvAgent 提出了跨编程语言的可执行环境自动构建框架，解决可验证软件工程数据集稀缺的瓶颈。采用多智能体规划-执行-验证架构，自主解决环境构建失败并通过环境复用机制提升效率，支持 Python、Java、TypeScript 等 10 种主流编程语言。已发布 MEnvData-SWE（3005 个任务实例，942 个代码仓库）和 MEnvBench（1000 个评估任务），是目前最大的开源多语言可验证软件工程数据集。

- **Agent-Omit: Training Efficient LLM Agents for Adaptive Thought and Observation Omission via Agentic Reinforcement Learning** `[RL]` `[微调]` — [2602.04284](https://arxiv.org/abs/2602.04284) | [GitHub](https://github.com/usail-hkust/Agent-Omit)
  > Agent-Omit 提出了通过智能体强化学习训练 LLM 智能体自适应省略冗余思维和观察的统一框架。现有方法对交互轨迹中所有步骤一视同仁，忽略了不同轮次中思维必要性和观察有效性的差异。Agent-Omit 量化分析思维和观察对智能体效率的影响，训练模型自主判断何时省略，在保持任务性能的同时大幅降低 token 消耗，在多个智能体基准上取得显著效率提升。

- **D-CORE: Incentivizing Task Decomposition in Large Reasoning Models for Complex Tool Use** `[RL]` `[微调]` — [2602.02160](https://arxiv.org/abs/2602.02160) | [GitHub](https://github.com/alibaba/EfficientAI)
  > D-CORE 提出两阶段训练框架解决大型推理模型（LRM）在复杂工具调用场景下的「惰性推理」问题：首先通过自蒸馏激励子任务分解推理能力，再用多样性感知强化学习恢复模型的反思推理能力。在 BFCLv3 基准上，D-CORE-8B 达到 77.7% 准确率（超越最优 8B 模型 5.7%），D-CORE-14B 以 79.3% 超越所有 70B 以下模型，建立了新的最优性能。

- **MeKi: Memory-based Expert Knowledge Injection for Efficient LLM Scaling** `[MeM]` — [2602.03359](https://arxiv.org/abs/2602.03359) | [GitHub](https://github.com/ningding-o/MeKi)
  > MeKi（基于内存的专家知识注入）提出通过存储空间而非算力来扩展边缘设备 LLM 性能的新范式。针对手机等边缘设备 RAM 和 NPU 资源受限、无法通过增加参数或测试时计算扩展的挑战，MeKi 为每个 Transformer 层配备 token 级内存专家，利用快闪存储存储大量知识块并在推理时按需调取。实验表明 MeKi 在保持实时推理速度的同时，以更小的参数规模达到更强模型的性能。

- **AgentArk: Distilling Multi-Agent Intelligence into a Single LLM Agent** `[微调]` — [2602.03955](https://arxiv.org/abs/2602.03955) | [GitHub](https://github.com/AIFrontierLab/AgentArk)
  > AgentArk 提出将多智能体系统的集体动态内化为单个模型权重的蒸馏框架，将显式测试时交互转化为隐式模型能力。研究三种层次化蒸馏策略：推理增强微调、轨迹增强和群体迭代推理蒸馏。单智能体系统在保持多智能体级别推理性能的同时，大幅降低计算成本和错误传播风险。在数学推理、代码生成等多任务场景下验证了方法的通用性和扩展性。

- **Proxy Compression for Language Modeling** `[微调]` — [2602.04289](https://arxiv.org/abs/2602.04289) | [GitHub](https://github.com/LZhengisme/proxy-compression)
  > 代理压缩提出一种新型语言模型训练方案，在保留压缩输入效率优势的同时提供端到端的原始字节推理接口，解除模型对固定分词器的依赖。训练时语言模型同时在原始字节序列和外部压缩器生成的压缩视图上联合训练（支持 gzip、神经压缩等），推理时模型可直接处理原始字节。实验在代码生成和语言建模任务上验证了代理压缩的效果，为构建通用字节级语言模型提供新思路。

- **Self-Rewarding Sequential Monte Carlo for Masked Diffusion Language Models** `[无需训练]` — [2602.01849](https://arxiv.org/abs/2602.01849) | [GitHub](https://github.com/Algolzw/self-rewarding-smc)
  > 本文提出自奖励序列蒙特卡洛（SR-SMC），一种针对掩码扩散语言模型（MDLM）的推理时扩展算法。现有 MDLM 依赖基于置信度的贪婪解码，导致生成多样性坍塌。SR-SMC 通过并行运行多个相互作用的扩散过程，以扩散模型自身的轨迹级置信度作为重要性权重引导采样，无需任何奖励模型即可提升生成质量。在 MDLM、BD3-LMs、LLaDA-1.5 和 Dream-7B 上均实现一致的性能提升。

- **Context Learning for Multi-Agent Discussion** `[微调]` — [2602.02350](https://arxiv.org/abs/2602.02350) | [GitHub](https://github.com/HansenHua/M2CL-ICLR26)
  > M2CL 针对多智能体讨论（MAD）中因各智能体上下文对齐不足导致的「讨论不一致」问题，提出多 LLM 上下文学习方法。为每个智能体学习独立的上下文生成器，能够在每轮讨论中动态生成个性化上下文指令，通过自动信息组织和精炼来维护一致的协作推理过程。在数学推理、常识推理等多任务上验证了 M2CL 显著改善讨论一致性并提升整体问题解决性能，已被 ICLR 2026 接收。

- **EntRGi: Entropy Aware Reward Guidance for Diffusion Language Models** `[无需训练]` — [2602.05000](https://arxiv.org/abs/2602.05000) | [GitHub](https://github.com/atutej/entrgi)
  > EntRGi 研究离散扩散语言模型的推理时奖励引导问题。由于离散 token 无法直接对奖励模型求梯度，现有方法要么用连续松弛替代（损害梯度质量），要么用直通估计器（梯度信号失真）。EntRGi 提出根据模型预测熵动态在软嵌入和硬 token 之间插值：高熵（低置信度）时偏向软嵌入保证梯度质量，低熵时偏向硬 token 保证奖励模型可靠性。无需微调即可应用于任意预训练扩散 LLM。

- **SAFE: Stable Alignment Finetuning with Entropy-Aware Predictive Control for RLHF** `[RL]` `[微调]` — [2602.04651](https://arxiv.org/abs/2602.04651) | [GitHub](https://github.com/ryyzn9/SAFE)
  > SAFE 提出了针对 LM-RLHF 场景的纯在线策略 Actor-Critic 强化学习方法，解决 PPO 在对齐微调中存在的奖励震荡、熵坍塌、价值函数漂移和策略突然发散等问题。核心创新是熵感知预测控制器，通过自适应 KL 阈值动态调整 KL 惩罚，配合双软最小评论家网络和层归一化设计，在无需频繁重启和大量超参数调整的情况下保持训练稳定性。实验在多个 LLM 家族（Qwen3、Llama3、Gemma3）上验证了效果。

- **OmniRad: A Radiological Foundation Model for Multi-Task Medical Image Analysis** `[VLM]` `[微调]` — [2602.04547](https://arxiv.org/abs/2602.04547) | [GitHub](https://github.com/unica-visual-intelligence-lab/OmniRad)
  > OmniRad 是基于 120 万张医学影像自监督预训练的放射学基础模型，强调表示复用和跨任务迁移能力。模型在分类、分割和放射学报告生成三类任务上统一评估，支持轻量 LoRA 适配器（冻结主干）和全量端到端微调两种下游适配模式。通过 STA（空间 token 聚合）从多 ViT 层提取多尺度特征，结合 DEIMv2 风格的 HybridEncoder 实现密集预测。在多个放射学下游任务上取得领先性能。


## 2026年2月6日

- **Spider-Sense: Intrinsic Risk Sensing for Efficient Agent Defense with Hierarchical Adaptive Screening** `[无需训练]` — [2602.05386](https://arxiv.org/abs/2602.05386) | [GitHub](https://github.com/aifinlab/Spider-Sense)
  > 现有 Agent 安全机制依赖强制检查范式，在固定阶段触发安全验证，导致开销大且不灵活。本文提出 Spider-Sense 框架，基于「内生风险感知」(IRS) 的事件驱动防御机制，使 Agent 保持潜在警觉，仅在感知到风险时触发防御。框架分层自适应筛查，兼顾效率与安全性，在多类攻击场景下显著降低 Token 消耗，同时维持强防御性能。

- **MemSkill: Learning and Evolving Memory Skills for Self-Evolving Agents** `[微调]` `[MeM]` — [2602.02474](https://arxiv.org/abs/2602.02474) | [GitHub](https://github.com/ViktorAxelsen/MemSkill)
  > 现有 LLM Agent 记忆系统依赖静态手工设计的操作，难以适应多样交互模式。MemSkill 将记忆操作重构为可学习、可进化的「记忆技能」，结构化地提取、整合和剪枝交互历史。通过 Controller 动态选择相关技能，配合 Learner 在线更新技能，MemSkill 在长轨迹任务上超越现有记忆基线，记忆质量与效率显著提升。

- **Length-Unbiased Sequence Policy Optimization: Revealing and Controlling Response Length Variation in RLVR** `[RL]` — [2602.05261](https://arxiv.org/abs/2602.05261) | [GitHub](https://github.com/murphy4122/LUSPO)
  > RLVR 训练中，响应长度变化被视为推理能力增长的关键因素，但不同算法的长度变化规律差异显著。本文深入分析主流 RLVR 算法组件，从理论上揭示长度偏差的根源，提出「长度无偏序列策略优化」(LUSPO)，通过对序列级奖励进行长度归一化消除偏差，在保持推理准确率的同时有效控制响应长度，实验验证了理论分析的有效性。

- **DFlash: Block Diffusion for Flash Speculative Decoding** `[无需训练]` — [2602.06036](https://arxiv.org/abs/2602.06036) | [GitHub](https://github.com/z-lab/dflash)
  > 自回归 LLM 解码本质上是串行的，导致高推理延迟和低 GPU 利用率。投机解码依赖草稿模型并行验证，但现有方法草稿阶段仍是自回归的。DFlash 提出用轻量级块扩散模型作为草稿模型，实现真正并行草稿生成。DFlash 在多个主流模型（Qwen3、LLaMA 等）上相比标准解码实现 2-3× 加速，同时保持输出质量不变。

- **Multi-Task GRPO: Reliable LLM Reasoning Across Tasks** `[RL]` `[微调]` — [2602.05547](https://arxiv.org/abs/2602.05547) | [GitHub](https://github.com/rsshyam/MT-GRPO)
  > 基于 GRPO 的 RL 后训练广泛用于提升 LLM 单任务推理，但多任务场景下直接扩展会导致部分任务优化主导、其他任务停滞。本文提出 MT-GRPO，动态调整任务权重以明确优化最差任务性能，并引入零优势感知的梯度校正处理任务贡献不均问题。在数学、代码、逻辑等多任务评测中，MT-GRPO 显著提升最差任务指标，整体推理可靠性更强。

- **DASH: Faster Shampoo via Batched Block Preconditioning and Efficient Inverse-Root Solvers** `[微调]` — [2602.02016](https://arxiv.org/abs/2602.02016) | [GitHub](https://github.com/IST-DASLab/DASH)
  > Shampoo 是领先的近似二阶优化器，但内部运算（特别是矩阵逆根计算）代价高昂，导致训练速度大幅降低。DASH（分布式加速 Shampoo）通过两项核心技术解决此问题：一是将预条件块堆叠为 3D 张量批量处理以提升 GPU 利用率，二是提出高效逆根求解器。在 LLM 预训练实验中，DASH 相比标准 Shampoo 达到接近 AdamW 的计算开销，同时保留二阶优化的收敛优势。

- **SwimBird: Eliciting Switchable Reasoning Mode in Hybrid Autoregressive MLLMs** `[VLM]` `[微调]` — [2602.06040](https://arxiv.org/abs/2602.06040) | [GitHub](https://github.com/Accio-Lab/SwimBird)
  > 现有多模态 LLM 主要依赖文本 CoT 推理，对视觉密集型任务效果有限；注入固定数量连续隐状态作为「视觉思维」会损害文本逻辑推理。本文提出 SwimBird，通过可切换推理模式的混合自回归 MLLM，使模型能根据不同查询自适应选择文本或视觉推理路径。在视觉问答、多步推理等任务上，SwimBird 相比纯文本推理基线取得显著提升，同时维持文本推理能力。

- **V-Retrver: Evidence-Driven Agentic Reasoning for Universal Multimodal Retrieval** `[VLM]` `[无需训练]` — [2602.06034](https://arxiv.org/abs/2602.06034) | [GitHub](https://github.com/chendy25/V-Retrver)
  > 现有多模态检索方法依赖静态视觉编码和语言驱动推理，在视觉模糊案例中易产生推测性错误。V-Retrver 将多模态检索重构为基于视觉检查的 Agent 推理过程，通过外部视觉工具主动获取细粒度视觉证据。V-Retrver 在多个通用多模态检索基准上达到最优性能，相比依赖 CoT 重排序的方法大幅提升在模糊图像检索场景下的准确率。

- **CoPE: Clipped RoPE as A Scalable Free Lunch for Long Context LLMs** `[长文本]` `[无需训练]` — [2602.05258](https://arxiv.org/abs/2602.05258) | [GitHub](https://github.com/hrlics/CoPE)
  > RoPE 是 LLM 上下文扩展的关键组件，现有扩展方法分为 OOD 缓解（缩放频率）和语义建模（优先关注语义相似 Token）两类。本文提出 CoPE，通过对 RoPE 低频分量进行软裁剪，统一上述两个看似矛盾的目标：消除 OOD 异常值的同时优化语义建模。CoPE 是免训练的「即插即用」方案，在多个长文本任务上持续提升性能，几乎零额外计算开销。

- **Approximation of Log-Partition Function in Policy Mirror Descent Induces Implicit Regularization for LLM Post-Training** `[RL]` `[微调]` — [2602.05933](https://arxiv.org/abs/2602.05933) | [GitHub](https://github.com/horizon-rl/OpenKimi)
  > 策略镜像下降（PMD）为 RL 后训练提供了原则性框架，Kimi K1.5/K2 等先进 LLM 均采用此方法。然而理想的 PMD 闭合解依赖配分函数的精确估计，在 LLM 庞大动作空间中极具挑战。本文研究实用算法 PMD-mean，用采样策略下的均值奖励近似对数配分项，并在对数策略空间进行回归。理论分析表明此近似带来隐式正则化效果，有助于防止过拟合，实验结果验证了算法有效性。

- **Breaking the Static Graph: Context-Aware Traversal for Robust Retrieval-Augmented Generation** `[无需训练]` — [2602.01965](https://arxiv.org/abs/2602.01965) | [GitHub](https://github.com/kwunhang/CatRAG)
  > 现有基于知识图谱的 RAG 方法（如 HippoRAG）依赖索引时固定的转移概率，导致随机游走易被「枢纽」高度节点偏转，丢失关键证据链。本文提出「打破静态图」框架 CatRAG，通过上下文感知遍历动态调整边的相关性权重，使随机游走更关注与查询语义相关的路径。在多跳 QA 基准上，CatRAG 显著提升完整证据链召回率，减少幻觉。

- **Failing to Explore: Language Models on Interactive Tasks** — [2601.22345](https://arxiv.org/abs/2601.22345) | [GitHub](https://github.com/mahdi-jfri/explore-exploit-bench)
  > 本文评估语言模型在有限交互预算下探索交互环境的能力，提出三类难度可控的参数化任务，覆盖连续和离散环境。实验发现当前 SOTA 模型系统性地探索不足，性能常显著劣于简单探索-利用启发式基线，且随预算增加扩展性弱。研究了两种轻量级干预：将固定预算拆分为并行执行（意外地提升了性能）以及周期性总结交互历史，为改进 LLM 探索能力提供实证依据。

- **Assessing Domain-Level Susceptibility to Emergent Misalignment from Narrow Finetuning** `[微调]` — [2602.00298](https://arxiv.org/abs/2602.00298) | [GitHub](https://github.com/abhishek9909/assessing-domain-emergent-misalignment)
  > 涌现性错误对齐（Emergent Misalignment）对 AI 安全构成风险。本文对 11 个不同领域的不安全数据集微调的 LLM 群体（基于 Qwen2.5-Coder-7B 和 GPT-4o-mini）进行系统评测，发现：(i) 后门触发器在 77.8% 的领域中加剧错误对齐；(ii) 域级漏洞差异显著，成员推断指标可作为预测广泛错误对齐程度的先验。本文首次提供了按领域分级的涌现错误对齐分类排名，为 AI 安全和后训练研究提供参考。

## 2026年2月9日

- **Baichuan-M3: Modeling Clinical Inquiry for Reliable Medical Decision-Making** `[微调]` `[长文本]` — [2602.06570](https://arxiv.org/abs/2602.06570) | [GitHub](https://github.com/baichuan-inc/Baichuan-M3-235B)
  > 本文提出 Baichuan-M3，一个医疗增强型大语言模型，旨在将临床决策支持从被动问答转变为主动式、临床级别的诊断辅助。核心能力包括：(1) 主动信息获取以消除歧义；(2) 长程推理将零散证据整合为连贯诊断；(3) 自适应幻觉抑制确保事实可靠性。模型通过专门的训练流程模拟医生系统化工作流程。在 HealthBench、HealthBench-Hallu 和 ScanBench 上均取得最优结果，在临床问询、咨询与安全方面显著超越 GPT-5.2。模型权重已公开。

- **On the Entropy Dynamics in Reinforcement Fine-Tuning of Large Language Models** `[RL]` `[微调]` — [2602.03392](https://arxiv.org/abs/2602.03392) | [GitHub](https://github.com/agentscope-ai/Trinity-RFT)
  > 本文对大语言模型强化微调（RFT）过程中的熵动态建立了理论框架。以单次 logit 更新下熵变化的判别表达式为起点，推导出熵变一阶表达式，并将其推广至 GRPO 的更新公式。理论分析揭示了各类基于熵的方法的统一视角，并启发了熵判别器裁剪方法的设计。实验验证了主要结论，并展示了熵控制方法在优化 LLM 微调中探索与利用平衡方面的有效性。结果表明，该方法在 RFT 训练中显著改善了熵崩塌问题。

- **Self-Improving Multilingual Long Reasoning via Translation-Reasoning Integrated Training** `[RL]` `[微调]` `[长文本]` — [2602.05940](https://arxiv.org/abs/2602.05940) | [GitHub](https://github.com/NJUNLP/TRIT)
  > 长推理模型在多语言场景中常出现「英语推理偏向」问题，即面对非英语问题时倾向于用英语推理，而强制使用问题语言推理则准确率大幅下降。本文提出 TRIT（Translation-Reasoning Integrated Training），一个无需外部反馈或额外多语言数据的自改进框架，将翻译训练整合进多语言推理训练中，同步提升多语言问题理解与回答生成能力。在 MMATH 上，该方法平均超越多个基线 7 个百分点，跨语言问题对齐提升超 10 个百分点，翻译质量在 FLORES-200 上提升最高 8.4 COMET 分。

- **POINTS-GUI-G: GUI-Grounding Journey** `[RL]` `[微调]` `[VLM]` — [2602.06391](https://arxiv.org/abs/2602.06391) | [GitHub](https://github.com/Tencent/POINTS-GUI)
  > 本文研究从基础能力弱的 VLM 出发，构建高性能 GUI 定位模型的完整技术路径。提出 POINTS-GUI-G-8B，在 ScreenSpot-Pro（59.9）、OSWorld-G（66.0）、ScreenSpot-v2（95.7）和 UI-Vision（49.9）上达到最优。成功的三大关键因素为：(1) 精细数据工程，包括多源数据格式统一、增广过滤与难度分级；(2) 改进训练策略，含视觉编码器持续微调与训练推理分辨率一致性；(3) 基于可验证奖励的强化学习——RL 不仅提升推理能力，在感知密集型 GUI 定位任务中同样显著改善精度。

- **Outcome Accuracy is Not Enough: Aligning the Reasoning Process of Reward Models** `[RL]` `[微调]` — [2602.04649](https://arxiv.org/abs/2602.04649) | [GitHub](https://github.com/QwenLM/RationaleRM)
  > 生成式奖励模型（GenRM）和 LLM-as-a-Judge 存在「欺骗性对齐」问题：模型以错误理由给出正确判断，过度依赖结果准确性导致 RLHF 泛化失效。本文提出「理由一致性」指标，量化模型推理过程与人类判断的对齐程度。在此基础上设计混合训练信号，将理由一致性与结果准确性结合。方法在 RM-Bench（87.1%）和 JudgeBench（82%）上达到最优，超越仅结果训练基线平均 5%；在 RLHF 阶段，创意写作任务上提升 7%；理由一致性分析确认该方法成功规避了欺骗性对齐陷阱。

- **OmniMoE: An Efficient MoE by Orchestrating Atomic Experts at Scale** `[微调]` — [2602.05711](https://arxiv.org/abs/2602.05711) | [GitHub](https://github.com/flash-algo/omni-moe)
  > 本文提出 OmniMoE，一个系统-算法协同设计的 MoE 框架，将专家粒度推向极致——引入向量级「原子专家」并结合共享密集 MLP 分支。针对路由复杂度和内存访问挑战，设计了笛卡尔积路由器（将复杂度从 O(N) 降至 O(√N)）和专家中心调度（将分散内存访问转为高效矩阵运算）。在七个基准上，OmniMoE（1.7B 激活参数）零样本准确率 50.9%，超越 DeepSeekMoE 和 PEER 等基线；推理延迟从 73ms 降至 6.7ms（10.9倍加速）。证明了大规模细粒度 MoE 可以同时快速且准确。

- **compar:IA: The French Government's LLM arena to collect French-language human prompts and preference data** `[微调]` — [2602.06669](https://arxiv.org/abs/2602.06669) | [GitHub](https://github.com/betagouv/ComparIA)
  > 非英语语言的 LLM 人类偏好数据严重匮乏。本文介绍 compar:IA，法国政府开发的开源平台，通过盲式成对比较界面大规模收集以法语为主的真实用户提示和偏好投票。截至 2026-02-07，已收集超 60 万条自由形式提示和 25 万条偏好投票，约 89% 为法语数据。发布对话、投票和反应三个互补数据集，并提供法语模型排行榜和用户交互分析。该平台正向国际化数字公共品演进，提供可复用的多语言偏好数据收集基础设施。

- **Uncovering Cross-Objective Interference in Multi-Objective Alignment** `[RL]` `[微调]` — [2602.06869](https://arxiv.org/abs/2602.06869) | [GitHub](https://github.com/yining610/ctwa)
  > 本文研究大语言模型多目标对齐中的「跨目标干扰」现象：训练提升部分目标性能的同时导致其他目标退化。通过对经典标量化算法的系统性研究，证明干扰现象普遍且具有强烈的模型依赖性。理论推导了局部协方差定律，并将其推广至带裁剪的代理目标。基于此提出 CTWA（协方差目标权重自适应），一种即插即用方法，通过维持目标奖励与训练信号的正协方差来缓解跨目标干扰。同时提供 PL 条件下的全局收敛分析，揭示跨目标干扰对模型几何特性的依赖。

- **SEMA: Simple yet Effective Learning for Multi-Turn Jailbreak Attacks** `[RL]` `[微调]` — [2602.06854](https://arxiv.org/abs/2602.06854) | [GitHub](https://github.com/fmmarkmq/SEMA)
  > 多轮越狱攻击是安全对齐聊天机器人的真实威胁模型。本文提出 SEMA，一个无需依赖现有策略或外部数据的多轮攻击者训练框架。SEMA 分两阶段：(1) 预填充自调优，通过在自生成的结构化非拒绝对话上微调来稳定后续学习；(2) 意图漂移感知奖励的强化学习，结合意图对齐、合规风险和细节程度三维度奖励训练攻击者。该框架统一了单轮和多轮场景，降低探索复杂度。在 AdvBench 上平均 ASR@1 达 80.1%，超过最优基线 33.9%，为 LLM 安全红队测试提供更强现实压力测试。

- **PlanViz: Evaluating Planning-Oriented Image Generation and Editing for Computer-Use Tasks** `[VLM]` `[无需训练]` — [2602.06663](https://arxiv.org/abs/2602.06663) | [GitHub](https://github.com/lijunxian111/PlanViz)
  > 本文提出 PlanViz，一个专门评估计算机使用任务中规划导向图像生成与编辑能力的基准。统一多模态模型（UMM）虽在自然图像生成和多模态推理上表现出色，但其在计算机使用规划任务中的潜力尚未被充分探索。PlanViz 聚焦三个日常子任务：路线规划、工作流程图和网页/UI 展示，采用人工标注问题和参考图像，并提出任务自适应评分指标 PlanScore，综合评估生成正确性、视觉质量和效率。实验揭示了当前模型的关键局限性，为未来研究指明方向。

- **Vision Transformer Finetuning Benefits from Non-Smooth Components** `[微调]` — [2602.06883](https://arxiv.org/abs/2602.06883) | [GitHub](https://github.com/ambroiseodt/vit-plasticity)
  > 本文分析视觉 Transformer 组件在迁移学习中的「可塑性」（plasticity），定义为输出对输入变化的平均变化率，高可塑性意味着低平滑性。通过理论分析和全面实验，证明注意力模块和前馈层的高可塑性持续带来更好的微调性能。关键发现挑战了平滑性有益的主流假设：在微调场景中，非平滑组件反而更具优势。本研究为迁移学习中 Transformer 组件优先级选择提供了原则性指导，揭示了 Transformer 函数特性的新视角。

- **AtlasPatch: An Efficient and Scalable Tool for Whole Slide Image Preprocessing in Computational Pathology** `[微调]` `[无需训练]` — [2602.03998](https://arxiv.org/abs/2602.03998) | [GitHub](https://github.com/AtlasAnalyticsLab/AtlasPatch)
  > 全切片图像（WSI）预处理是计算病理学 AI 工作流的基础，包括组织检测和补丁提取，但现有工具存在精度低或计算复杂度高的问题。本文提出 AtlasPatch，一个高效可扩展的幻灯片预处理框架。组织检测模块在约 3 万张 WSI 缩略图上通过高效微调 Segment-Anything 模型训练而成，从缩略图推断全分辨率切片的组织掩码，支持多种放大倍数下的补丁坐标提取，可直接流式传输到图像编码器或存储补丁图像，且 CPU/GPU 并行化。在分割精度、计算复杂度和下游多实例学习上均匹配最优性能，同时计算开销仅为其几分之一。

- **SEAD: Self-Evolving Agent for Multi-Turn Service Dialogue** `[RL]` `[微调]` — [2602.03548](https://arxiv.org/abs/2602.03548) | [GitHub](https://github.com/Da1yuqin/SEAD)
  > 当前服务对话系统依赖嘈杂低质量的人工对话数据，性能受限。本文提出 SEAD（自进化服务对话智能体），无需大规模人工标注即可学习有效策略。SEAD 将用户建模解耦为两个组件：Profile Controller（生成多样化用户状态管理训练课程）和 User Role-play Model（专注真实角色扮演），确保训练环境提供自适应场景而非不公平对手。实验表明，SEAD 显著超越开源基础模型和闭源商业模型，任务完成率提升 17.6%，对话效率提升 11.1%。

- **Learning a Generative Meta-Model of LLM Activations** `[无需训练]` `[MeM]` — [2602.06964](https://arxiv.org/abs/2602.06964) | [GitHub](https://github.com/g-luo/generative_latent_prior)
  > 现有神经网络激活分析方法（如 PCA、稀疏自编码器）依赖强结构假设。本文探索生成模型作为替代方案：在十亿个残差流激活上训练扩散模型，构建「元模型」学习网络内部状态分布。发现扩散损失随计算量平滑下降，并可靠预测下游效用：将元模型学习到的先验应用于引导干预可提升文本流畅性，随损失降低增益增大；元模型神经元在概念隔离方面表现提升，稀疏探测分数随损失降低而增加。结果表明，生成元模型为无强结构假设的可解释性研究提供了可扩展路径。

- **Table-as-Search: Formulate Long-Horizon Agentic Information Seeking as Table Completion** `[无需训练]` `[长文本]` — [2602.06724](https://arxiv.org/abs/2602.06724) | [GitHub](https://github.com/AIDC-AI/Marco-DeepResearch)
  > 当前信息检索智能体在长程探索中难以维持焦点和连贯性。本文提出 TaS（Table-as-Search），将信息检索任务重新表述为表格补全任务：将每个查询映射到外部数据库中的结构化表格模式，行表示搜索候选，列表示约束或所需信息，已填格严格记录历史和搜索结果，空白格作为明确搜索计划。TaS 统一了深度搜索、广度搜索和深度广度搜索三类任务。大量实验表明，TaS 在三类基准上显著超越多个最优基线，展现出优越的长程鲁棒性、效率、可扩展性和灵活性。

- **Seg-ReSearch: Segmentation with Interleaved Reasoning and External Search** `[RL]` `[微调]` `[VLM]` — [2602.04454](https://arxiv.org/abs/2602.04454) | [GitHub](https://github.com/iSEE-Laboratory/Seg-ReSearch)
  > 现有基于语言的分割系统受限于 MLLM 的冻结内部知识，难以处理需要最新信息或领域特定概念的真实场景。本文提出 Seg-ReSearch，通过交替推理与外部检索打破知识瓶颈，使分割系统能够处理超出模型冻结知识的动态开放世界查询。为有效训练此能力，设计了层次化奖励，平衡稀疏结果信号与刚性逐步监督之间的困境。同时构建 OK-VOS 基准，专门评估需要外部知识的视频目标分割。在 OK-VOS 及两个现有推理分割基准上显著超越最优方法。

- **Uncertainty Drives Social Bias Changes in Quantized Large Language Models** — [2602.06181](https://arxiv.org/abs/2602.06181) | [GitHub](https://github.com/stan-hua/PostTrainingBiasBenchmark)
  > 训练后量化降低 LLM 计算成本，但会以聚合指标难以捕获的方式改变社会偏见。本文在统一基准 PostTrainingBiasBench（13 个偏见数据集）上对 50 个量化模型进行首次大规模研究。发现「量化诱导的掩蔽偏见翻转」现象：量化后高达 21% 的回答在偏见与无偏间翻转，但聚合分数无变化。翻转由模型不确定性驱动，高不确定性回答翻转概率比低不确定性高 3-11 倍；4 位量化模型行为变化是 8 位模型的 4-6 倍，且偏见变化对不同人口群体产生非对称影响。


## 2026年2月10日

- **Weak-Driven Learning: How Weak Agents make Strong Agents Stronger** `[微调]` `[RL]` — [2602.08222](https://arxiv.org/abs/2602.08222) | [GitHub](https://github.com/chenzehao82/Weak-Driven-Learning)
  > 提出 WMSS（弱智能体能使强智能体更强），一种通过历史弱检查点（weak checkpoints）来引导持续优化的后训练范式。通过熵动态识别可恢复的学习缺口，并通过补偿学习加以强化，使强模型能够突破传统后训练的饱和瓶颈。方法无需昂贵的强教师模型，仅利用模型自身历史弱版本。在数学推理和代码生成任务上实验表明，该方法在零额外推理成本下实现了有效性能提升。

- **TermiGen: High-Fidelity Environment and Robust Trajectory Synthesis for Terminal Agents** `[微调]` — [2602.07274](https://arxiv.org/abs/2602.07274) | [GitHub](https://github.com/ucsb-mlsec/terminal-bench-env)
  > 提出 TermiGen，一个端到端管道，用于合成可验证的终端任务环境和具有鲁棒性的专家轨迹。首先通过多智能体迭代精炼循环生成合法任务和 Docker 容器；然后采用 Generator-Critic 协议在轨迹收集中主动注入错误，合成富含错误纠正循环的数据。基于此数据微调的 TermiGen-Qwen2.5-Coder-32B 在 TerminalBench 上取得 31.3% 通过率，超越已有开源模型及 o4-mini 等闭源模型，建立新的开源最优水平。

- **QuantaAlpha: An Evolutionary Framework for LLM-Driven Alpha Mining** — [2602.07085](https://arxiv.org/abs/2602.07085) | [GitHub](https://github.com/QuantaAlpha/QuantaAlpha)
  > 提出 QuantaAlpha，一个将每次端到端挖掘运行视为轨迹的进化型 Alpha 因子挖掘框架，通过轨迹级变异和交叉操作来改进因子。框架在因子生成时强制执行假设、因子表达式和可执行代码的语义一致性，并约束复杂度以减少过度拥挤。在 CSI 300 上的大量实验显示，使用 GPT-5.2 时 IC 达 0.1501，年化超额收益 27.75%，最大回撤 7.98%，且因子能有效迁移到 CSI 500 和 S&P 500。

- **Modality Gap-Driven Subspace Alignment Training Paradigm For Multimodal Large Language Models** `[VLM]` `[无需训练]` `[微调]` — [2602.07026](https://arxiv.org/abs/2602.07026) | [GitHub](https://github.com/Yu-xm/ReVision)
  > 针对多模态对比学习中持续存在的「模态鸿沟」问题，提出 Fixed-frame Modality Gap 理论，将模态鸿沟分解为稳定偏差和各向异性残差。在此基础上提出 ReAlign——一种无需训练的模态对齐策略，利用大规模未配对数据的统计信息，通过 Anchor、Trace、Centroid 对齐三步将文本表示映射到图像分布。进一步提出 ReVision 训练范式，在预训练阶段集成 ReAlign，使模型在无需大量图文配对数据的情况下完成高效扩展。

- **InternAgent-1.5: A Unified Agentic Framework for Long-Horizon Autonomous Scientific Discovery** `[MeM]` — [2602.08990](https://arxiv.org/abs/2602.08990) | [GitHub](https://github.com/InternScience/InternAgent)
  > 提出 InternAgent-1.5，一个用于端到端科学发现的统一系统，包含生成、验证、进化三个协调子系统，支持深度研究、解决方案优化和长视野记忆等能力。在 GAIA、HLE、GPQA、FrontierScience 等科学推理基准上取得领先性能。在算法发现任务中能自主设计机器学习方法，在实证发现任务中可执行完整计算或湿实验。该框架具备通用性和可扩展性，适用于广泛的自主科学发现场景。

- **LLaDA2.1: Speeding Up Text Diffusion via Token Editing** `[RL]` `[微调]` — [2602.08676](https://arxiv.org/abs/2602.08676) | [GitHub](https://github.com/inclusionAI/LLaDA2.X)
  > 提出 LLaDA2.1，通过将 Token-to-Token（T2T）编辑融入传统 Mask-to-Token（M2T）方案，引入联合可配置阈值解码策略，分 Speedy Mode 和 Quality Mode。此外，首次为扩散语言模型（dLLMs）构建了大规模 RL 训练框架，使用专门的梯度估计技术提升推理精度和指令遵循能力。发布 LLaDA2.1-Mini（16B）和 LLaDA2.1-Flash（100B），在 33 项基准上表现优异，HumanEval+ 上达到 892 TPS 的推理速度。

- **Alleviating Sparse Rewards by Modeling Step-Wise and Long-Term Sampling Effects in Flow-Based GRPO** `[RL]` — [2602.06422](https://arxiv.org/abs/2602.06422) | [GitHub](https://github.com/YunzeTong/TurningPoint-GRPO)
  > 提出 TurningPoint-GRPO（TP-GRPO），解决 Flow Matching 模型上应用 GRPO 时的步骤级奖励稀疏问题。核心创新：（1）用步骤级增量奖励替代基于结果的奖励，提供密集的逐步学习信号；（2）识别「转折点」——翻转局部奖励趋势且使后续奖励演化与整体轨迹趋势一致的步骤，并赋予聚合长期奖励以捕捉其延迟影响。转折点仅通过增量奖励的符号变化检测，无超参数。实验表明 TP-GRPO 更有效地利用奖励信号并持续提升生成质量。

- **Learning Query-Aware Budget-Tier Routing for Runtime Agent Memory** `[RL]` `[MeM]` `[长文本]` — [2602.06025](https://arxiv.org/abs/2602.06025) | [GitHub](https://github.com/ViktorAxelsen/BudgetMem)
  > 提出 BudgetMem，一个支持显式查询感知性能-成本控制的运行时智能体记忆框架。将记忆处理结构化为多个模块，每个模块提供低/中/高三个预算档位，并用轻量级路由器（RL 训练的紧凑神经策略）进行预算档路由。研究了实现（方法复杂度）、推理（行为）和容量（模型规模）三种档位实现策略。在 LoCoMo、LongMemEval 和 HotpotQA 上，BudgetMem 在高预算下超越强基线，并在紧约束下提供更优的精度-成本前沿。

- **Theory of Space: Can Foundation Models Construct Spatial Beliefs through Active Exploration?** `[VLM]` — [2602.07055](https://arxiv.org/abs/2602.07055) | [GitHub](https://github.com/mll-lab-nu/Theory-of-Space)
  > 定义「空间理论」能力：智能体在主动自导探索中获取信息，并从序列局部观测中构建、修订和利用空间信念。通过基准测试评估当前模型，发现三个瓶颈：主动-被动差距（主动探索时性能显著下降）、高度低效的探索策略、以及「信念惰性」（智能体无法用新证据更新过时先验，视觉模型尤为严重）。研究揭示当前基础模型在主动探索下难以维持连贯可修订的空间信念。

- **LatentChem: From Textual CoT to Latent Thinking in Chemical Reasoning** `[无需训练]` — [2602.07075](https://arxiv.org/abs/2602.07075) | [GitHub](https://github.com/xinwuye/LatentChem)
  > 提出 LatentChem，一个将化学计算从文本生成中解耦的潜在推理接口，使模型能在连续潜在空间中直接执行多步推理，仅在最终输出时生成语言。实验发现，模型在仅优化任务成功的情况下会自发将推理内化，逐渐放弃冗长的文本推导而转向隐式潜在计算。在多个化学推理基准上，LatentChem 对强 CoT 基线的非平局胜率达 59.88%，同时实现平均 10.84 倍推理加速。

- **Fundamental Reasoning Paradigms Induce Out-of-Domain Generalization in Language Models** `[微调]` — [2602.08658](https://arxiv.org/abs/2602.08658) | [GitHub](https://github.com/voalmciaf/FR-OOD)
  > 研究演绎、归纳、溯因三种基本推理范式如何促进 LLM 的域外泛化。从符号任务收集推理轨迹数据集，每个任务专注于三种范式之一，以抽象化具体世界知识。通过简单微调、增加模型深度、将稠密模型转为混合专家等多种方法将这些技能注入 LLM。在完全用自然语言表述且含真实世界知识的域外任务上评估，结果显示该方法在现实任务上带来显著的泛化增益（最高 14.60 分）。

- **RelayGen: Intra-Generation Model Switching for Efficient Reasoning** `[无需训练]` — [2602.06454](https://arxiv.org/abs/2602.06454) | [GitHub](https://github.com/jiwonsong-dev/RelayGen)
  > 提出 RelayGen，一个无需训练的段级运行时模型切换框架，利用长推理链中的难度变化。通过离线分析 token 概率边际的生成不确定性，识别模型特定切换线索（信号困难段向容易段的转变），动态将低难度段委托给小模型，将高难度推理保留在大模型上。无需额外训练或学习路由组件。结合推测解码，RelayGen 实现最高 2.2 倍端到端加速，精度损失小于 2%。

- **How2Everything: Mining the Web for How-To Procedures to Evaluate and Improve LLMs** `[RL]` `[微调]` — [2602.08808](https://arxiv.org/abs/2602.08808) | [GitHub](https://github.com/lilakk/how2everything)
  > 提出 How2Everything，一个评估和改进目标条件程序生成的可扩展框架。包含 How2Mine（从 98 万个网页挖掘 35.1 万个步骤化程序）、How2Bench（7K 样本评估集）、以及 How2Score（用 LLM 评判检测关键失败的评估协议）。将前沿模型蒸馏为 8B 开放模型，与人工标注者达到 80.5% 一致性。使用 How2Score 作为 RL 奖励，三个模型上 How2Bench 性能提升 10 分以上，且在标准基准上无系统性退步。

- **Data Science and Technology Towards AGI Part I: Tiered Data Management** `[微调]` — [2602.09003](https://arxiv.org/abs/2602.09003) | [GitHub](https://github.com/UltraData-OpenBMB/UltraData-Math)
  > 提出分层数据管理框架，支持 LLM 训练全生命周期中的异构学习目标和成本约束。引入 L0-L4 五层数据管理体系，从原始未整理资源到有组织的可验证知识。LLM 被充分用于数据管理过程（质量评分和内容编辑）以精炼各层数据，每层具有不同数据属性、管理策略和训练角色。实验表明，层次感知的数据利用显著提升训练效率和模型性能，并开源了分层数据集和处理工具。

- **CodeCircuit: Toward Inferring LLM-Generated Code Correctness via Attribution Graphs** — [2602.07080](https://arxiv.org/abs/2602.07080) | [GitHub](https://github.com/bruno686/CodeCircuit)
  > 探索能否仅从 LLM 内部计算结构评估生成代码的功能正确性，无需外部执行测试或辅助模型裁判。受机械可解释性启发，将代码验证视为机械诊断任务，将模型的算法轨迹映射为行级归因图。通过分解复杂残差流识别区分正确推理与逻辑失败的结构特征。在 Python、C++、Java 上的分析确认内在正确性信号跨语法具有鲁棒性，拓扑特征比表面启发式更可靠地预测正确性。

- **SoulX-Singer: Towards High-Quality Zero-Shot Singing Voice Synthesis** — [2602.07803](https://arxiv.org/abs/2602.07803) | [GitHub](https://github.com/Soul-AILab/SoulX-Singer)
  > 提出 SoulX-Singer，一个面向工业部署的高质量开源零样本歌唱语音合成系统。支持基于乐谱（MIDI）或旋律表示的可控歌唱生成，在超过 4.2 万小时人声数据上训练，覆盖普通话、英语和粤语。在多种音乐条件下跨语言达到最新最优合成质量。构建了 SoulX-Singer-Eval 评估集，具有严格的训练-测试隔离，支持零样本场景的系统评估。

- **MotionCrafter: Dense Geometry and Motion Reconstruction with a 4D VAE** — [2602.08961](https://arxiv.org/abs/2602.08961) | [GitHub](https://github.com/TencentARC/MotionCrafter)
  > 提出 MotionCrafter，一个基于视频扩散的框架，从单目视频中联合重建 4D 几何结构并估计密集运动。核心是密集 3D 点图和 3D 场景流的联合表示，以及用于有效学习该表示的新型 4D VAE。与强制 3D 值和潜变量与 RGB VAE 潜变量严格对齐的先前工作不同，提出了新的数据归一化和 VAE 训练策略，无需任何后优化即可在几何重建和密集场景流估计上分别取得 38.64% 和 25.0% 的性能提升。

- **Towards Bridging the Gap between Large-Scale Pretraining and Efficient Finetuning for Humanoid Control** `[RL]` `[微调]` — [2601.21363](https://arxiv.org/abs/2601.21363) | [GitHub](https://github.com/bigai-ai/LIFT-humanoid)
  > 提出 LIFT 框架，弥合仿人机器人控制中大规模预训练与高效微调之间的差距。使用大批量更新和高 UTD 比率的离策略 SAC 进行大规模预训练，实现零样本部署到真实机器人。微调阶段采用基于模型的 RL，在新环境中执行确定性策略同时将随机探索限制在物理感知世界模型中，降低随机探索风险。在仿人运动任务上验证了该框架的有效性，兼顾预训练的时钟效率和微调的样本效率。

- **WildReward: Learning Reward Models from In-the-Wild Human Interactions** `[RL]` `[微调]` — [2602.08829](https://arxiv.org/abs/2602.08829) | [GitHub](https://github.com/THU-KEG/WildReward)
  > 探索直接从真实用户与 LLM 的交互中构建奖励模型的可能性。采用 WildChat 作为交互来源，提出提取可靠人类反馈的管道，生成 18.6 万高质量实例，通过序数回归直接在用户反馈上训练 WildReward。大量实验表明 WildReward 相比传统奖励模型具有可比甚至更优的性能，标定和跨样本一致性更好。用户多样性越高，奖励模型越强。将 WildReward 用于在线 DPO 训练，跨任务取得显著改进。

- **Optimal Turkish Subword Strategies at Scale: Systematic Evaluation of Data, Vocabulary, Morphology Interplay** — [2602.06942](https://arxiv.org/abs/2602.06942) | [GitHub](https://github.com/turkish-nlp-suite/Turkish-subwords-research)
  > 首个对土耳其语子词分词进行系统全面研究的工作，联合调整词汇量和分词器训练语料大小，比较 WordPiece、形态级和字符基线等多个分词器家族，并在语义（NLI、STS、情感分析、NER）、句法（POS、依存分析）和形态敏感探针上进行评估。引入形态感知诊断工具包，包括边界级微/宏 F1、词素原子性等细粒度指标。结果揭示最优词汇量因推理密集型和知识密集型任务差异显著，为形态丰富语言建立了可复现的分词优化基础。

- **ECO: Energy-Constrained Optimization with Reinforcement Learning for Humanoid Walking** `[RL]` — [2602.06445](https://arxiv.org/abs/2602.06445) | [GitHub](https://github.com/bigai-ai/ECO-humanoid)
  > 提出 ECO（Energy-Constrained Optimization），一个将能量相关指标从奖励中分离出来、重新表述为显式不等式约束的约束 RL 框架。通过拉格朗日方法执行能耗和参考运动约束，实现稳定、对称且节能的仿人机器人行走。与 MPC、标准奖励塑形 RL 及四种最先进约束 RL 方法的对比实验（含仿真到仿真和仿真到真实迁移）表明，ECO 在保持鲁棒行走性能的同时显著降低了能耗。

- **Echoes as Anchors: Probabilistic Costs and Attention Refocusing in LLM Reasoning** `[微调]` `[无需训练]` — [2602.06600](https://arxiv.org/abs/2602.06600) | [GitHub](https://github.com/hhh2210/echoes-as-anchors)
  > 分析并利用 LLM 推理中重述问题的「提示回声」（EOP）现象作为前置计算塑形机制。形式化其概率代价，将回声移除建模为基于拒绝的条件化，定义 Echo Likelihood Gap ΔL 作为可计算代理指标。提出 Echo-Distilled SFT（ED-SFT）通过监督微调注入「先回声再推理」模式，以及 Echoic Prompting（EP）在推理中重新锚定模型。注意力分析表明 EOP 在中间层增加了答案到答案前缀的注意力。在 GSM8K、MathQA、AIME24、MATH-500 上取得一致提升。

- **CauScale: Neural Causal Discovery at Scale** — [2602.08629](https://arxiv.org/abs/2602.08629) | [GitHub](https://github.com/OpenCausaLab/CauScale)
  > 提出 CauScale，一个将因果发现推理扩展到 1000 节点图的神经架构。通过压缩数据嵌入的缩减单元提升时间效率，通过绑定注意力权重（避免维护轴特定注意力图）提升空间效率。采用双流设计：数据流从高维观测提取关系证据，图流整合统计图先验。在训练时成功扩展到 500 节点图（先前方法因空间限制失败），在分布内数据上取得 99.6% mAP，比先前方法快 4-13000 倍。

- **Cost-Efficient RAG for Entity Matching with LLMs: A Blocking-based Exploration** `[无需训练]` — [2602.05708](https://arxiv.org/abs/2602.05708) | [GitHub](https://github.com/machuangtao/CE-RAG4EM)
  > 提出 CE-RAG4EM，一个通过基于阻塞的批量检索和生成来降低大规模实体匹配计算开销的高效 RAG 架构。提出用于分析和评估实体匹配 RAG 系统的统一框架，聚焦于阻塞感知优化和检索粒度。大量实验表明 CE-RAG4EM 能在与强基线相当甚至更优的匹配质量下显著降低端到端运行时间，并揭示关键配置参数在性能与开销之间的内在权衡，为高效可扩展的 RAG 系统设计提供实践指导。


## 2026年2月11日

- **Chain of Mindset: Reasoning with Adaptive Cognitive Modes** `[无需训练]` `[VLM]` — [2602.10063](https://arxiv.org/abs/2602.10063) | [GitHub](https://github.com/QuantaAlpha/chain-of-mindset)
  > 提出 Chain of Mindset（CoM），一个无需训练的智能体框架，实现步骤级别的自适应思维编排。CoM 将推理分解为四种异质思维模式：空间、收敛、发散和算法。Meta-Agent 根据推理状态动态选择最优思维，双向 Context Gate 过滤模块间信息流以保持效率。在数学、代码生成、科学问答、空间推理等六个基准上，使用 Qwen3-VL-32B-Instruct 和 Gemini-2.0-Flash 分别超越最强基线 4.96% 和 4.72%，同时平衡推理效率。

- **SkillRL: Evolving Agents via Recursive Skill-Augmented Reinforcement Learning** `[RL]` `[MeM]` — [2602.08234](https://arxiv.org/abs/2602.08234) | [GitHub](https://github.com/aiming-lab/SkillRL)
  > 提出 SkillRL，通过自动技能发现和递归演化桥接原始经验与策略改进。引入基于经验的蒸馏机制构建层级技能库 SkillBank，自适应检索策略支持通用和任务特定启发式，递归演化机制使技能库与智能体策略在强化学习过程中协同演化。显著减少 token 占用同时提升推理效能。在 ALFWorld、WebShop 及七项搜索增强任务上超越基线 15.3%，一个 7B 模型实现对 GPT-4o 的超越。

- **Large-Scale Terminal Agentic Trajectory Generation from Dockerized Environments** `[微调]` — [2602.01244](https://arxiv.org/abs/2602.01244) | [GitHub](https://github.com/Wusiwei0410/TerminalTraj)
  > 提出 TerminalTraj，一个可扩展流水线，解决终端智能体训练数据构建中的可执行性和可验证性挑战。该流水线过滤高质量代码库以构建 Docker 化执行环境，生成 Docker 对齐的任务实例，并合成具有可执行验证代码的智能体轨迹。使用 TerminalTraj 构建了 3.2 万 Docker 镜像，生成跨八个领域的 50,733 条验证轨迹。基于 Qwen2.5-Coder 的模型在 TerminalBench 上提升高达 20%，TerminalTraj-32B 达到 100B 参数以下最强性能。

- **Agent Banana: High-Fidelity Image Editing with Agentic Thinking and Tooling** `[MeM]` — [2602.09084](https://arxiv.org/abs/2602.09084) | [GitHub](https://github.com/taco-group/agent-banana)
  > 提出 Agent Banana，一个用于高保真、对象感知图像编辑的层级智能体规划-执行框架，解决专业工作流中过度编辑、单轮限制和超高清分辨率评测三大挑战。引入两项核心机制：Context Folding（将长交互历史压缩为结构化记忆以实现稳定长程控制）和 Image Layer Decomposition（执行局部层级编辑以保留非目标区域并支持原生分辨率输出）。构建 HDD-Bench 高清对话评测集，含 4K 分辨率图像。Agent Banana 在多轮一致性和背景保真度上达到最优（IC 0.871，SSIM-OM 0.84）。

- **Secure Code Generation via Online Reinforcement Learning with Vulnerability Reward Model** `[RL]` `[微调]` — [2602.07422](https://arxiv.org/abs/2602.07422) | [GitHub](https://github.com/AndrewWTY/SecCoderX)
  > 提出 SecCoderX，一个在线强化学习框架，用于保留功能性的安全代码生成。通过重新利用漏洞检测资源两种方式：（1）合成多样化的漏洞诱发编码任务用于在线 RL 推出，（2）训练基于推理的漏洞奖励模型提供可扩展安全监督。两者统一到在线 RL 循环中对齐代码 LLM。实验表明 SecCoderX 达到最优性能，Effective Safety Rate（ESR）相比未对齐模型提升约 10%，而先前方法常导致 ESR 下降 14-54%。

- **DLLM-Searcher: Adapting Diffusion Large Language Model for Search Agents** `[微调]` — [2602.07035](https://arxiv.org/abs/2602.07035) | [GitHub](https://github.com/bubble65/DLLM-Searcher)
  > 提出 DLLM-Searcher，将扩散大语言模型（dLLM）适配为高效搜索智能体。核心贡献包括：并行推理与行动（P-ReAct），利用扩散模型的非自回归生成特性实现并行推理和工具执行，显著降低推理延迟；以及两阶段智能体后训练流水线（Agentic SFT + Agentic VRPO），改善推理结构、工具调用和搜索可靠性。在多跳检索任务上与强自回归搜索智能体相当，端到端推理速度提升约 15%，验证了 dLLM 作为实用搜索智能体的可行性。


## 2026年2月12日

- **GENIUS: Generative Fluid Intelligence Evaluation Suite** `[VLM]` `[无需训练]` — [2602.11144](https://arxiv.org/abs/2602.11144) | [GitHub](https://github.com/arctanxarc/GENIUS)
  > 现有多模态生成模型基准主要评估「晶体智能」（依赖已学习的模式和知识），而忽视了「流体生成智能」（GFI）——即在新情境下进行模式归纳、约束推理和动态适应的能力。本文提出 GENIUS 评估套件，涵盖三类任务：隐式模式归纳、临时约束执行和情境知识适应，采用混合度量（规则符合度、视觉约束符合度、美学质量）和 LMM-as-a-Judge 框架进行评测。实验表明，即便是最先进的专有模型（如 Nano Banana Pro）整体得分也仅约 57 分，远未达到及格线；模型普遍表现出「认知惯性」，无法抑制预训练先验以适应新情境；且「视觉美观」与「逻辑合规」之间存在严重鸿沟，指出当前 UMM 架构在注意力分布和上下文传播上的结构性缺陷。

- **How Do Decoder-Only LLMs Perceive Users? Rethinking Attention Masking for User Representation Learning** `[微调]` — [2602.10622](https://arxiv.org/abs/2602.10622) | [GitHub](https://github.com/JhCircle/Deepfind-GGSM)
  > 解码器架构的大语言模型在用户行为建模中的注意力掩码设计尚未得到系统研究。本文在统一对比学习框架下，基于支付宝大规模真实用户行为数据，系统比较了因果注意力、混合注意力和双向注意力掩码对用户表示质量的影响。为改善向双向注意力过渡时的训练动态，提出「渐进式掩码转换」策略，并通过门控自注意力稀疏化（GGSM）优化 KV Cache 效率。实验表明，所提方法在工业级用户理解任务上显著优于因果掩码基线，验证了注意力掩码设计对 LLM 用户表示学习的根本重要性。

- **G-LNS: Generative Large Neighborhood Search for LLM-Based Automatic Heuristic Design** `[无需训练]` — [2602.08253](https://arxiv.org/abs/2602.08253) | [GitHub](https://github.com/ZBoyn/G-LNS)
  > 现有基于 LLM 的自动启发式设计（AHD）方法通常局限于优先规则或参数化局部搜索的固定形式，难以突破深层局部最优。本文提出 G-LNS，一种生成式进化框架，利用 LLM 协同进化「销毁算子」和「修复算子」对，通过协同评估矩阵（Synergy Matrix）显式建模两类算子的交互关系，并维护双种群结构实现自适应选择与联合交叉。在 TSP 和 CVRP 等组合优化挑战上，G-LNS 显著超越先前的 LLM-AHD 方法及经典求解器，且在跨分布实例上展现出强泛化能力。

- **DataChef: Cooking Up Optimal Data Recipes for LLM Adaptation via Reinforcement Learning** `[RL]` `[微调]` — [2602.11089](https://arxiv.org/abs/2602.11089) | [GitHub](https://github.com/yichengchen24/DataChef)
  > 大语言模型的适配性能在很大程度上取决于数据配方（Data Recipe）的质量，但现有设计方式高度依赖人工经验。本文提出 DataChef，一个用于自动生成最优数据配方的 LLM 系统，输入目标任务和原始数据源，输出包含可执行处理流水线和训练数据集的完整方案。DataChef 通过强化学习训练，将下游任务性能作为奖励信号，迭代优化数据规划（Planner）和代码生成（Coder）模块。实验表明，DataChef 在多个下游 LLM 适配任务上优于人工设计的数据配方，且模型权重和在线演示已公开发布。

- **ROCKET: Rapid Optimization via Calibration-guided Knapsack Enhanced Truncation for Efficient Model Compression** `[无需训练]` — [2602.11008](https://arxiv.org/abs/2602.11008) | [GitHub](https://github.com/mts-ai/ROCKET)
  > 本文提出 ROCKET，一种无需训练的模型压缩方法，在分解、结构化稀疏化和动态压缩基线上达到最新最优水平。ROCKET 的核心创新有二：（1）将逐层压缩分配形式化为多选背包问题（Multi-Choice Knapsack），在全局压缩预算约束下最小化总重建误差；（2）引入基于校准的快速敏感度评估，避免逐层 SVD 搜索开销。在主流语言模型上，ROCKET 以更低的精度损失实现与当前最佳方法相当甚至更好的压缩率，且无需任何微调。

- **Online Causal Kalman Filtering for Stable and Effective Policy Optimization** `[RL]` — [2602.10609](https://arxiv.org/abs/2602.10609) | [GitHub](https://github.com/shuohe1995/verl-kpo)
  > LLM 强化学习中基于重要性采样（IS）的策略优化因 token 级 IS 比例高方差而面临训练不稳定问题。现有方法要么使用序列级固定比例，要么独立调整每个 token，均忽略了序列内跨 token 的时序离策略偏差。本文提出 KPO（Kalman Policy Optimization），利用一维因果卡尔曼滤波器平滑 token 级对数比率，获得更稳定的重要性权重估计。KPO 作为即插即用模块集成到 verl 框架（PPO/GRPO 流水线），在数学推理等 RLHF 工作负载上实现更稳定、更高效的策略优化。

- **LoopFormer: Elastic-Depth Looped Transformers for Latent Reasoning via Shortcut Modulation** `[无需训练]` — [2602.11451](https://arxiv.org/abs/2602.11451) | [GitHub](https://github.com/armenjeddi/loopformer)
  > 循环 Transformer 在语言推理任务上表现出色，但现有方法在训练和推理阶段固定循环次数，限制了计算深度的灵活性。本文提出 LoopFormer，通过弹性深度循环架构与快捷调制（Shortcut Modulation）目标，使模型在可变长度轨迹上训练，支持时间步长和步长大小条件化，从而实现无需重新训练的预算条件式语言建模与潜在推理。LoopFormer 基于 NanoGPT 实现，在多个语言推理任务上以更少参数达到与固定深度模型相当的性能，并支持测试时动态调整计算量。

- **Data Repetition Beats Data Scaling in Long-CoT Supervised Fine-Tuning** `[微调]` — [2602.11149](https://arxiv.org/abs/2602.11149) | [GitHub](https://github.com/dkopi/data-repetition)
  > 在固定更新预算下，长链思维（Long-CoT）监督微调中数据重复（即在小数据集上多轮训练）优于单轮大数据集训练——这一发现反直觉地挑战了「更多独特样本带来更好泛化」的传统认知。本文在 AIME'24/25 和 GPQA 等推理基准上验证：Olmo3-7B 在 128 轮训练少量数据的条件下，优于单轮训练 128 倍更多数据的设置。作者还发布了 45 个 checkpoint 及全套训练/评估脚本，为长推理链 SFT 的数据效率研究提供了系统性基础设施。

- **The Pensieve Paradigm: Stateful Language Models Mastering Their Own Context** `[RL]` `[长文本]` `[MeM]` — [2602.12108](https://arxiv.org/abs/2602.12108) | [GitHub](https://github.com/xyliu-cs/StateLM)
  > 现有语言模型缺乏对自身上下文的主动管理能力，被动接受人工工程化的上下文输入。本文提出 StateLM，一类新型基础模型，具备内生的有状态推理能力，可自主控制上下文：构建索引、迭代检索、记录笔记、剪枝冗余信息。StateLM 在长文本问答（如 HELMET、LongBench）和深度研究任务上超越现有长上下文方法，且无需外部工具编排。其 RL 训练基于 verl v0.6.0，模型（StateLM-8B）和完整代码已开源。

- **Latent Thoughts Tuning: Bridging Context and Reasoning with Fused Information in Latent Tokens** `[微调]` — [2602.10229](https://arxiv.org/abs/2602.10229) | [GitHub](https://github.com/NeosKnight233/Latent-Thoughts-Tuning)
  > 显式链式推理（CoT）将中间步骤局限于离散词汇空间，而现有连续潜在推理方案常受特征坍缩之苦。本文提出 LT-Tuning，一种无需外部辅助模型的后训练框架，通过「置信度驱动动态切换」自适应决定何时插入潜在 <thinking> token，并通过「上下文预测融合」将上下文隐状态与词表嵌入空间的预测语义融合，缓解特征坍缩。三阶段课程学习从显式 CoT 渐进过渡到潜在推理。在 GSM8K-NL、ASDiv、MultiArith、SVAMP 等数学推理基准上，LT-Tuning 优于现有潜在推理方法。

- **Free(): Learning to Forget in Malloc-Only Reasoning Models** `[微调]` `[长文本]` — [2602.08030](https://arxiv.org/abs/2602.08030) | [GitHub](https://github.com/TemporaryLoRA/FreeLM)
  > 推理模型通过扩展测试时计算提升问题求解能力，但过多思考 token 反而会导致性能下降。本文将其归因于标准 LLM「只申请不释放」（malloc-only）的架构缺陷，提出 Free()LM：通过即插即用的 Free-Module（LoRA 适配器）引入内生自遗忘能力，在推理和清理模式间迭代切换，动态识别并剪除无用上下文块。在 8B 至 685B 多个模型规模上，Free()LM 平均提升 3.3%；在 Qwen3-235B 完全崩溃（0% 准确率）的长 horizon 任务上，Free()LM 将性能恢复至约 50%，并在 IMOanswerBench 上创造新 SOTA。

- **AgenticPay: A Multi-Agent LLM Negotiation System for Buyer-Seller Transactions** `[无需训练]` — [2602.06008](https://arxiv.org/abs/2602.06008) | [GitHub](https://github.com/SafeRL-Lab/AgenticPay)
  > 现有基准缺乏评估多智能体语言经济交互的规范化设置。本文提出 AgenticPay，一个基于 LLM 的多智能体买卖双方谈判仿真框架与基准，建模买方和卖方持有私有约束和商品估值并用自然语言进行多轮谈判的市场场景。框架支持单品/多品谈判、并行/顺序谈判模式及用户画像系统，采用类 Gym 接口设计，兼容 OpenAI/vLLM/SGLang 多种 LLM 后端。实验揭示了主流 LLM 在复杂经济谈判中的策略局限性。

- **When Actions Go Off-Task: Detecting and Correcting Misaligned Actions in Computer-Use Agents** `[无需训练]` — [2602.08995](https://arxiv.org/abs/2602.08995) | [GitHub](https://github.com/OSU-NLP-Group/Misaligned-Action-Detection)
  > 计算机使用智能体（CUA）频繁产生偏离用户原始意图的「失准动作」，可能来自外部攻击（如间接提示注入）或内部推理错误，严重影响安全性和可靠性。本文首次系统定义并研究 CUA 的失准动作检测问题，构建了 MisActBench 基准数据集，并提出 DeAction 检测框架：通过「叙事摘要 + 系统分析 + 快速检查」三级流水线识别失准动作并给出纠错建议。实验表明，DeAction 在 MisActBench 上大幅超越单纯依赖 LLM 判断的基线方法。

- **Large Language Lobotomy: Jailbreaking Mixture-of-Experts via Expert Silencing** `[无需训练]` — [2602.08741](https://arxiv.org/abs/2602.08741) | [GitHub](https://github.com/jonatelintelo/LargeLanguageLobotomy)
  > 混合专家（MoE）架构的大语言模型通过路由结构引入了新的安全攻击面。本文发现 MoE LLM 中的安全关键行为（如拒绝有害请求）集中于少数专家，而非均匀分布。基于此，本文提出 Large Language Lobotomy（LLL）：通过识别并静默负责安全行为的专家组合，绕过模型的安全拒绝机制。实验在 Mixtral 和其他 MoE 模型上验证了该攻击的有效性，揭示了现有 MoE 安全对齐机制的根本脆弱性。

- **FedPS: Federated data Preprocessing via aggregated Statistics** `[无需训练]` — [2602.10870](https://arxiv.org/abs/2602.10870) | [GitHub](https://github.com/xuefeng-xu/fedps)
  > 联邦学习中，数据预处理（缺失值填补、格式统一、特征缩放）对模型性能至关重要，但在隐私约束下无法集中原始数据。本文提出 FedPS，一个用于联邦数据预处理的统一框架，通过聚合统计量（而非原始数据）实现隐私保护的分布式预处理。FedPS 兼容水平和垂直联邦场景，支持离散化、编码、缩放等多类预处理算子，提供类 sklearn 的 API 接口，在模拟通信场景下验证了与集中式预处理相当的效果且通信开销可接受。

- **Graph-Enhanced Deep Reinforcement Learning for Multi-Objective Unrelated Parallel Machine Scheduling** `[RL]` — [2602.08052](https://arxiv.org/abs/2602.08052) | [GitHub](https://github.com/bulentsoykan/GNN-DRL4UPMSP)
  > 异构并行机器调度问题（UPMSP）在同时最小化加权总延迟（TWT）和总换机时间（TST）时面临显著挑战。本文提出结合近端策略优化（PPO）与异构图神经网络（GNN）的深度强化学习框架：GNN 将作业、机器和换机类型构建为异构图，捕获复杂约束关系；PPO 通过动作掩码保证可行调度。实验表明，该框架在真实约束场景（释放日期、机器适用性、序列相关换机时间）下显著优于传统启发式和元启发式方法，推理速度也满足动态环境需求。

- **From Features to Actions: Explainability in Traditional and Agentic AI Systems** `[无需训练]` — [2602.06841](https://arxiv.org/abs/2602.06841) | [GitHub](https://github.com/VectorInstitute/unified-xai-evaluation-framework)
  > 传统可解释 AI（XAI）聚焦于单次预测的特征归因，而智能体 AI 系统的行为展开于多步轨迹之上。本文在统一框架下系统比较静态预测与智能体系统的可解释性需求，实验横跨传统 ML 文本分类（SHAP、LIME、显著性方法）和基于 LLM 的工具调用智能体（TAU-bench、AssistantBench）两类范式。研究表明，针对静态模型的归因方法无法可靠诊断智能体故障，提出面向智能体的轨迹级诊断方案（基于执行日志和行为评估 Rubric），并发布可复现的端到端实验流水线。

- **StealthRL: Reinforcement Learning Paraphrase Attacks for Multi-Detector Evasion of AI-Text Detectors** `[RL]` `[微调]` — [2602.08934](https://arxiv.org/abs/2602.08934) | [GitHub](https://github.com/suraj-ranganath/StealthRL)
  > AI 文本检测器面临对抗性改写攻击的鲁棒性挑战。本文提出 StealthRL，一个基于强化学习的框架，训练改写策略以在保持语义忠实度的同时逃避多检测器集成的检测。StealthRL 使用 GRPO（带 LoRA 适配器）在 Qwen3-4B 上微调改写模型，奖励函数综合考量检测逃避率、语义相似度和流畅性。在 MAGE 基准上，StealthRL 在严格低误报操作点下显著降低检测率，同时保持高语义相似度，超越简单改写和检测器引导基线，为 AI 文本检测系统的红队测试提供了系统性工具。

## 2026年2月13日

- **Composition-RL: Compose Your Verifiable Prompts for Reinforcement Learning of Large Language Models** `[RL]` — [2602.12036](https://arxiv.org/abs/2602.12036) | [GitHub](https://github.com/XinXU-USTC/Composition-RL)
  > 大规模可验证提示是RLVR成功的基础，但现有训练集中包含大量无信息样本且难以扩展。已有工作聚焦于优先使用pass rate为0的困难问题，而本文关注pass rate为1的简单问题在训练中逐渐增多的问题。提出Composition-RL：自动将多个问题组合成新的可验证复合问题，用于RL训练。在4B到30B模型上实验表明，Composition-RL持续提升推理能力，课程式变体通过逐步增加组合深度可进一步增益。此外该方法还支持跨领域RL，通过组合不同领域的提示实现更有效的迁移。

- **DeepGen 1.0: A Lightweight Unified Multimodal Model for Advancing Image Generation and Editing** `[VLM]` `[RL]` `[微调]` — [2602.12205](https://arxiv.org/abs/2602.12205) | [GitHub](https://github.com/DeepGenTeam/DeepGen)
  > 当前统一多模态图像生成与编辑模型通常依赖超过10B的大规模参数。本文提出DeepGen 1.0，一个轻量级5B统一模型，性能与更大模型相当甚至超越。核心创新是层叠通道桥接（SCB）深度对齐框架，从多个VLM层提取层次化特征并通过可学习「think token」融合，为生成骨干提供结构化推理引导。训练策略包括三个阶段：对齐预训练、联合监督微调、使用MR-GRPO强化学习。仅在约5000万样本上训练，DeepGen 1.0在多项基准上达到领先性能，在WISE上超越80B HunyuanImage达28%，开源训练代码、权重与数据集。

- **LawThinker: A Deep Research Legal Agent in Dynamic Environments** `[无需训练]` — [2602.12056](https://arxiv.org/abs/2602.12056) | [GitHub](https://github.com/yxy-919/LawThinker-agent)
  > 法律推理不仅要求结论正确，还要求程序合规。现有方法缺乏验证中间推理步骤的机制，导致如不适用法条引用等错误无声传播。本文提出LawThinker，一个采用「探索-验证-记忆」策略的自主法律研究智能体，核心在于将验证作为每次知识探索之后的原子操作。DeepVerifier模块从知识准确性、事实-法律相关性、程序合规性三个维度审查每次检索结果，并通过记忆模块支持长链任务中的跨轮知识复用。在动态基准J1-EVAL上，LawThinker相比直接推理提升24%，相比工作流方法提升11%，在过程导向指标上表现尤为突出。

- **Stroke of Surprise: Progressive Semantic Illusions in Vector Sketching** `[无需训练]` — [2602.12280](https://arxiv.org/abs/2602.12280) | [GitHub](https://github.com/stroke-of-surprise/Stroke-Of-Surprise)
  > 视觉错觉传统上依赖空间操纵，本文引入渐进式语义错觉任务：一幅矢量草图通过依次添加笔触发生戏剧性语义变换。提出Stroke of Surprise生成框架，优化矢量笔触使其在不同绘制阶段满足不同语义解释。核心挑战是「双约束」：前缀笔触须构成连贯对象（如鸭子），同时作为添加增量笔触后第二概念（如绵羊）的结构基础。提出序列感知联合优化框架，驱动机制为双分支Score Distillation Sampling，动态调整前缀笔触探索两者共同结构子空间。引入Overlay Loss强制空间互补性，实验表明方法在可识别性和错觉强度上显著超越基线。

- **LIE: Think Longer to Explore Deeper: Learn to Explore In-Context via Length-Incentivized Reinforcement Learning** `[RL]` `[长文本]` — [2602.11748](https://arxiv.org/abs/2602.11748) | [GitHub](https://github.com/LINs-lab/LIE)
  > 有效的测试时扩展需要模型具备上下文内探索能力——在单一连续上下文中生成、验证和精炼多个推理假设。基于状态覆盖理论，本文识别出关键瓶颈：更广的状态覆盖需要更长的推理轨迹，但自回归生成中采样此类序列的概率指数衰减（称为「浅层探索陷阱」）。提出Length-Incentivized Exploration（LIE），通过基于长度的奖励加冗余惩罚显式鼓励模型深入探索，从而两步最大化状态覆盖。在Qwen3、Llama等模型上实验表明，LIE在域内任务平均提升4.4%，域外基准提升2.7%。

- **dVoting: Fast Voting for dLLMs** `[无需训练]` — [2602.12153](https://arxiv.org/abs/2602.12153) | [GitHub](https://github.com/fscdc/dVoting)
  > 扩散大语言模型（dLLMs）是超越自回归建模的新范式，天然支持灵活的解码过程，具有并行测试时扩展的巨大潜力。本文提出dVoting，一种无需训练即可提升推理能力的快速投票技术，额外计算开销可接受。dVoting观察到：对同一提示的多次采样中，大多数token预测高度一致，而性能由少量跨样本变化的token决定。利用dLLMs任意位置生成能力，dVoting通过采样、一致性分析识别不确定token、重新投票生成、迭代收敛来精炼输出。实验表明在GSM8K提升6.22%-7.66%，MATH500提升4.40%-7.20%，ARC-C提升3.16%-14.84%。

- **DeepSight: An All-in-One LM Safety Toolkit** — [2602.12092](https://arxiv.org/abs/2602.12092) | [GitHub](https://github.com/AI45Lab/DeepSafe)
  > 大模型安全工作流中，评估、诊断和对齐通常由独立工具处理，安全评估只能定位外部行为风险而无法找到内部根因。本文提出开源项目DeepSight，实践「安全评估-诊断一体化」新范式。DeepSight低成本、可复现、高效且高度可扩展，包含评估工具DeepSafe和诊断工具DeepScan。通过统一任务和数据协议，将两阶段串联，将安全评估从黑盒转变为白盒洞察。DeepSight是首个支持前沿AI风险评估和联合安全评估与诊断的开源工具集。

- **Unveiling Implicit Advantage Symmetry: Why GRPO Struggles with Exploration and Difficulty Adaptation** `[RL]` — [2602.05548](https://arxiv.org/abs/2602.05548) | [GitHub](https://github.com/HKU-HealthAI/A-GRAE)
  > RLVR特别是GRPO已成为激发LLM推理的标准方法，但其在探索和难度适应方面的效率仍是开放挑战。本文指出这些瓶颈源于GRAE内隐含的优势对称性，导致两个关键限制：(i)群体级别，正确与错误轨迹的权重严格对称，阻碍新颖正确解的探索；(ii)样本级别，算法隐式偏向中等难度样本。提出Asymmetric GRAE（A-GRAE），动态调节探索激励和样本难度关注，通过不对称抑制正确轨迹优势来鼓励探索，并采用课程式由易到难的转换。七个基准上的实验证明A-GRAE持续提升GRPO及其变体在LLM和MLLM上的表现。

- **Dreaming in Code for Curriculum Learning in Open-Ended Worlds** `[RL]` — [2602.08194](https://arxiv.org/abs/2602.08194) | [GitHub](https://github.com/konstantinosmitsides/dreaming-in-code)
  > 开放式学习中，大组合空间使智能体难以发现持续可学习的经验序列。本文提出Dreaming in Code（DiCode），利用基础模型合成可执行环境代码来支撑学习向更高能力进阶。「做梦」表现为在代码层面对世界进行物化变体。在Craftax开放式基准上实例化DiCode，实验表明智能体能习得长时域技能，平均回报比最强基线提升16%，在先前方法完全失败的后期战斗任务上首次取得非零成功率。结果表明代码级环境设计为课程控制提供了实用机制。

- **SPES: Pretraining A Large Language Model using Distributed GPUs: A Memory-Efficient Decentralized Paradigm** — [2602.11543](https://arxiv.org/abs/2602.11543) | [GitHub](https://github.com/zjr2000/SPES)
  > LLM预训练通常需要集中式集群和数千块高显存GPU。现有去中心化训练方法虽减少了通信开销，但仍需在每个节点上训练完整模型。本文提出SPES（稀疏专家同步），一种用于预训练MoE LLM的内存高效去中心化框架，每个节点仅训练专家子集，显著降低显存占用，并通过定期同步消除全参数传输。引入专家合并热身策略加速收敛。实验表明使用16块48GB GPU通过互联网连接训练2B参数MoE LLM，性能与集中训练相当。进一步验证了7B从头训练和9B从稠密checkpoint升级的可扩展性。

- **Sci-CoE: Co-evolving Scientific Reasoning LLMs via Geometric Consensus with Sparse Supervision** `[RL]` `[微调]` — [2602.12164](https://arxiv.org/abs/2602.12164) | [GitHub](https://github.com/InternScience/Sci-CoE)
  > LLM在科学推理任务上因不可靠的解题评估和有限的验证策略多样性而仍较脆弱。本文提出Sci-CoE，一个两阶段科学协同进化框架，使模型同时作为求解器和验证器进行自我进化，从稀疏监督过渡到无监督学习。第一阶段使用少量标注数据建立基础正确性判断锚点；第二阶段引入几何奖励机制，联合考虑共识性、可靠性和多样性，驱动在未标注数据上的大规模自迭代。在多个通用科学基准上的实验表明Sci-CoE增强了复杂推理能力并表现出强扩展性。

- **P-GenRM: Personalized Generative Reward Model with Test-time User-based Scaling** `[RL]` `[微调]` — [2602.12116](https://arxiv.org/abs/2602.12116) | [GitHub](https://github.com/Tongyi-ConvAI/Qwen-Character)
  > 个性化LLM对齐旨在通过强化学习将回复适应个人用户偏好。现有个性化奖励模型存在两个持续限制：将多样偏好过度简化为少量固定评估原则，以及在新用户少量反馈下泛化困难。本文提出P-GenRM，首个具有测试时用户级缩放的个性化生成奖励模型。P-GenRM将偏好信号转化为结构化评估链，推导自适应角色和评分标准，并将用户聚类为用户原型，引入双粒度缩放机制。实验表明P-GenRM在个性化奖励模型基准上达到最优，平均提升2.31%，测试时用户级缩放额外提供3%增益。被ICLR 2026接收为Oral。

- **MuRGAt: Multimodal Fact-Level Attribution for Verifiable Reasoning** `[VLM]` — [2602.11509](https://arxiv.org/abs/2602.11509) | [GitHub](https://github.com/meetdavidwan/murgat)
  > 现有多模态接地基准聚焦于简化的观察型场景或有限模态，无法评估复杂多模态推理中的归因能力。本文引入MuRGAt（带接地归因的多模态推理），一个评估需要超越直接观察进行推理的事实级多模态归因基准。给定跨视频、音频等模态的输入，MuRGAt要求模型生成带明确推理和精确引用的答案，每个引用须指定模态和时间段。引入与人类判断高度相关的自动评估框架。基准测试揭示即使强大的MLLM也会在推理正确的情况下频繁幻构引用，且更深推理或强制结构化接地往往降低准确性，暴露了内部推理与可验证归因之间的显著差距。

- **MetaphorStar: Image Metaphor Understanding and Reasoning with End-to-End Visual Reinforcement Learning** `[RL]` `[VLM]` — [2602.10575](https://arxiv.org/abs/2602.10575) | [GitHub](https://github.com/MING-ZCH/MetaphorStar)
  > 图像隐喻理解对现有AI系统仍是关键挑战，需要复杂多跳推理、文化背景和心智理论能力。本文提出MetaphorStar，首个针对图像含义任务的端到端视觉强化学习框架，包含三个核心组件：细粒度数据集TFQ-Data、视觉RL方法TFQ-GRPO和结构化基准TFQ-Bench。使用TFQ-GRPO在TFQ-Data上训练的MetaphorStar系列模型，在图像含义基准上平均提升82.6%。MetaphorStar-32B在多项指标上达到最优，在真假题上显著超越顶级闭源模型Gemini-3.0-pro。实验还揭示图像含义任务的学习提升了通用视觉推理能力。

- **Detecting RLVR Training Data via Structural Convergence of Reasoning** `[RL]` — [2602.11792](https://arxiv.org/abs/2602.11792) | [GitHub](https://github.com/StevenZHB/Detect_RLVR_Data)
  > RLVR是训练现代推理模型的核心方法，但未公开的训练数据引发了基准污染担忧。与预训练不同，RLVR基于自生成轨迹的奖励反馈进行微调，使基于似然的传统检测方法失效。本文发现RLVR诱导了独特的行为特征：训练时遇到的提示产生更僵化和相似的输出，而未见提示保留更大多样性。提出Min-kNN Distance，一种简单黑盒检测器，通过对给定提示采样多个补全并计算k个最小近邻编辑距离的平均值来量化这种收敛性。该方法无需访问参考模型或token概率，实验表明其可靠区分RL训练样本与未见样本，超越现有基线。

- **ScalSelect: Scalable Training-Free Multimodal Data Selection for Efficient Visual Instruction Tuning** `[无需训练]` `[VLM]` — [2602.11636](https://arxiv.org/abs/2602.11636) | [GitHub](https://github.com/ChangtiWu/ScalSelect)
  > 大规模视觉指令微调（VIT）是提升视觉语言模型性能的关键范式，但大规模数据训练计算开销大。现有数据选择方法要么需要昂贵训练或梯度计算，要么依赖代理模型且扩展性有限。本文提出ScalSelect，一种具有线性时间复杂度的可扩展无需训练多模态数据选择方法，无需外部模型或辅助数据集。ScalSelect通过提取目标VLM中指令token最关注的视觉特征构建样本表示，识别最能近似全数据集表示主子空间的样本。实验表明ScalSelect仅用16%的数据可实现全数据训练97.5%以上的性能，部分设置下甚至超越全数据训练。

- **Neural Additive Experts: Context-Gated Experts for Controllable Model Additivity** — [2602.10585](https://arxiv.org/abs/2602.10585) | [GitHub](https://github.com/Teddy-XiongGZ/NAE)
  > 可解释性与准确性之间的权衡是机器学习的核心挑战。标准广义加性模型（GAM）提供清晰的特征归因，但严格的加性性质限制了预测性能，而引入特征交互虽提升准确性却可能掩盖个体特征贡献。本文提出神经加性专家（NAE），一种无缝平衡可解释性与准确性的新框架。NAE采用混合专家框架，为每个特征学习多个专用网络，通过动态门控机制整合跨特征信息，从而放宽严格加性约束。提出有针对性的正则化技术降低专家预测方差，促进从纯加性模型到捕获复杂特征交互的平滑过渡。在合成数据和真实数据集上的实验证实了NAE在预测准确性和可解释性间的最优平衡。接收于AISTATS 2026。


## 2026年2月16日

- **Less is Enough: Synthesizing Diverse Data in Feature Space of LLMs** `[微调]` — [2602.10388](https://arxiv.org/abs/2602.10388) | [GitHub](https://github.com/Zhongzhi660/FAC-Synthesis)
  > 本文提出 Feature Activation Coverage（FAC），一种在可解释特征空间中度量数据多样性的指标，用于解决现有后训练数据构建方法依赖文本指标、无法捕捉任务相关特征的问题。基于 FAC，作者进一步提出 FAC Synthesis 框架：先用稀疏自编码器（SAE）识别种子数据集中缺失的特征，再合成明确反映这些特征的样本。实验表明，该方法在指令跟随、毒性检测、奖励建模和行为引导等任务上持续提升数据多样性和下游性能。论文还发现 LLaMA、Mistral、Qwen 等模型族共享可解释特征空间，支持跨模型知识迁移，为 LLM 的数据中心优化提供了扎实的方法论基础。

- **OneVision-Encoder: Codec-Aligned Sparsity as a Foundational Principle for Multimodal Intelligence** `[VLM]` `[无需训练]` — [2602.08683](https://arxiv.org/abs/2602.08683) | [GitHub](https://github.com/EvolvingLMMs-Lab/OneVision-Encoder)
  > 本文提出 OneVision-Encoder（OV-Encoder），一种以 Codec 对齐稀疏性为基础原则的视觉编码器。核心假设：AGI 本质上是压缩问题，有效压缩要求架构与数据的基本结构共振。OV-Encoder 采用 Codec Patchification，放弃均匀计算，仅专注于信号熵丰富的 3.1%–25% 区域；采用共享 3D RoPE 统一空间与时序推理，并在百万语义概念上以聚类判别目标训练。在 16 个图像、视频和文档理解 benchmark 上，OV-Encoder 以更少的视觉 token 和预训练数据持续优于 Qwen3-ViT 和 SigLIP2，视频理解任务平均提升 4.1%，验证了效率与精度正相关的核心假设。

- **GeoAgent: Learning to Geolocate Everywhere with Reinforced Geographic Characteristics** `[RL]` `[VLM]` — [2602.12617](https://arxiv.org/abs/2602.12617) | [GitHub](https://github.com/HVision-NKU/GeoAgent)
  > 本文提出 GeoAgent，一个能像人类专家那样推理并得出精细地址结论的地理定位模型。针对已有 RL 方法依赖 AI 生成思维链数据、与地理特性冲突的问题，作者构建了由地理专家和专业选手标注的 CoT 数据集 GeoSeek，并设计了地理相似性奖励和一致性奖励（由一致性智能体评估），引导模型从地理视角收敛到正确答案，同时保证推理过程的完整性与一致性。实验结果显示，GeoAgent 在多粒度定位任务上优于现有方法和多个通用 VLLM，且生成的推理过程与人类判断高度一致。

- **What does RL improve for Visual Reasoning? A Frankenstein-Style Analysis** `[RL]` `[VLM]` — [2602.12395](https://arxiv.org/abs/2602.12395) | [GitHub](https://github.com/tianyi-lab/Frankenstein)
  > 本文提出 Frankenstein 风格分析框架，深入剖析强化学习（RL）相对于监督微调（SFT）冷启动在视觉推理中究竟提升了什么能力。框架包含三个维度：（i）因果探针定位功能区域；（ii）参数比对刻画更新特征；（iii）模型合并测试可迁移性。分析发现，RL 在推理时主要在中后层产生一致性迁移，该迁移既可通过合并迁移，也对 RL 增益不可或缺。总体而言，RL 在视觉推理中的可靠贡献不是均匀增强视觉感知，而是系统性精化中后层 Transformer 计算，改善视觉到推理的对齐，揭示了单靠 benchmark 评估的局限性。

- **Favia: Forensic Agent for Vulnerability-fix Identification and Analysis** `[无需训练]` — [2602.12500](https://arxiv.org/abs/2602.12500) | [GitHub](https://github.com/andstor/agentic-security-patch-classification-replication-package)
  > 本文提出 Favia，一个面向漏洞修复提交识别的取证 Agent 框架，结合可扩展候选排名与深度迭代语义推理。Favia 首先通过高效排名阶段缩小提交搜索空间，再用基于 ReAct 的 LLM Agent 对每个提交进行严格评估：Agent 以修复前仓库为环境，借助专业工具定位漏洞组件、遍历代码库，并建立代码变更与漏洞根因之间的因果对齐。在自建大规模数据集 CVEVC（含 3708 个真实仓库、超 800 万提交）上，Favia 在精召权衡和 F1 分数上一致优于传统及 LLM 基线，尤其擅长识别间接、多文件的非平凡修复。

- **scPilot: Large Language Model Reasoning Toward Automated Single-Cell Analysis and Discovery** `[无需训练]` — [2602.11609](https://arxiv.org/abs/2602.11609) | [GitHub](https://github.com/maitrix-org/scPilot)
  > 本文提出 scPilot，首个系统实践「组学原生推理」（omics-native reasoning）的框架：LLM 以自然语言对话的同时直接检查单细胞 RNA-seq 数据和按需生物信息工具。scPilot 将细胞类型注释、发育轨迹重建和转录因子靶向等核心单细胞分析任务转化为逐步推理问题。配套发布评测套件 scBench（9 个专家策划数据集）。实验显示，迭代组学原生推理将细胞类型注释平均准确率提升 11%，Gemini-2.5-Pro 在轨迹图编辑距离上比 one-shot 提示降低 30%，并生成透明的推理轨迹。论文已被 NeurIPS 2025 主会接收。

- **Steer2Edit: From Activation Steering to Component-Level Editing** `[无需训练]` — [2602.09870](https://arxiv.org/abs/2602.09870) | [GitHub](https://github.com/Trustworthy-ML-Lab/Steer2Edit)
  > 本文提出 Steer2Edit，一个理论严格、无需训练的框架，将推理时激活操控（activation steering）向量转化为诊断信号，用于组件级 rank-1 权重编辑。不同于均匀注入 steering 方向的推理时干预，Steer2Edit 将行为影响选择性地分配到各注意力头和 MLP 神经元，生成可解释的编辑，同时保持标准前向传播并与优化并行推理兼容。在安全对齐、幻觉缓解和推理效率三类任务上，Steer2Edit 在相同下游性能下将安全性提升最高 17.2%、真实性提升 9.8%、推理长度平均缩短 12.2%，为表示操控与权重编辑提供了原则性桥梁。

- **Code2Worlds: Empowering Coding LLMs for 4D World Generation** `[VLM]` — [2602.11757](https://arxiv.org/abs/2602.11757) | [GitHub](https://github.com/AIGeeksGroup/Code2Worlds)
  > 本文提出 Code2Worlds，将 4D 动态场景生成表述为语言到仿真代码生成任务。针对现有方法在多尺度上下文纠缠和语义-物理执行鸿沟两大挑战，作者设计了双流架构：检索增强对象生成流与层级环境编排流相互解耦；并建立物理感知闭环机制，由 PostProcess Agent 脚本化动态行为，配合 VLM-Motion Critic 进行自我反思迭代精炼仿真代码。在 Code4D benchmark 上，Code2Worlds 相比 baseline SGS 增益 41%、Richness 提升 49%，并能唯一生成先前静态方法所缺失的物理感知动态效果。


## 2026年2月17日

- **Experiential Reinforcement Learning** `[RL]` `[微调]` — [2602.13949](https://arxiv.org/abs/2602.13949) | [GitHub](https://github.com/microsoft/experiential_rl)
  > 本文提出「经验强化学习」（ERL），一种将经验-反思-巩固循环嵌入RL训练流程的新范式。面对稀疏延迟奖励问题，ERL让模型先生成初始尝试、获取环境反馈，再产生结构化反思引导第二次尝试，成功的改进通过自蒸馏内化进基础策略，推理期无额外成本。实验跨越稀疏奖励控制环境和Agent推理基准，ERL在所有6个评测中均优于RLVR基线：Sokoban环境最高提升81%，HotpotQA等工具使用任务提升11%。结果表明，将显式自我反思融入策略训练可将反馈转化为持久行为改进。

- **BitDance: Scaling Autoregressive Generative Models with Binary Tokens** `[微调]` `[VLM]` — [2602.14041](https://arxiv.org/abs/2602.14041) | [GitHub](https://github.com/shallowdream204/BitDance)
  > 本文提出BitDance，一种基于二值化Token的自回归图像生成框架。通过将视觉特征量化为二进制Token，BitDance大幅降低了词表规模与序列复杂度，在保持生成质量的同时显著提升了训练与推理效率。文章设计了高效的二值化编码器和解码器，利用二值Token的稀疏性实现更快速的序列建模，并在主流图像生成基准上验证了方法的有效性，展示了二值化Token在大规模自回归生成模型中的可扩展性潜力。

- **STATe-of-Thoughts: Structured Action Templates for Tree-of-Thoughts** `[无需训练]` — [2602.14265](https://arxiv.org/abs/2602.14265) | [GitHub](https://github.com/zbambergerNLP/state-of-thoughts)
  > 本文提出STATe-of-Thoughts（STAToT），通过引入「结构化行动模板」（SAT）改进Tree-of-Thoughts（ToT）推理框架。现有ToT方法对中间推理步骤缺乏约束，导致搜索效率低下。STAToT预定义与任务匹配的行动模板，将推理树的每个节点限定在有意义的动作空间内，无需额外训练即可在多步推理任务上提升搜索效率和准确率。实验在数学推理、逻辑谜题等任务上验证了模板化推理相比标准ToT的优势。

- **CellMaster: Collaborative Cell Type Annotation in Single-Cell Analysis** `[无需训练]` `[VLM]` — [2602.13346](https://arxiv.org/abs/2602.13346) | [GitHub](https://github.com/AnonymousGym/CellMaster)
  > CellMaster是一个AI Agent框架，利用LLM（如GPT-4o）的编码知识实现单细胞RNA测序数据的零样本细胞类型注释。与现有自动化工具不同，CellMaster无需预训练或固定marker数据库，通过即时推理生成可解释的注释依据，并支持Human-in-the-loop精细化。在覆盖8种组织的9个数据集上，自动模式下准确率比最佳基线（CellTypist和scTab）提升7.1%；加入人工反馈后提升18.6%，亚型群体提升22.1%，在罕见及新颖细胞状态识别上表现尤为突出。

- **LM-Lexicon: Improving Definition Modeling via Harmonizing Semantic Experts** `[微调]` — [2602.14060](https://arxiv.org/abs/2602.14060) | [GitHub](https://github.com/jacklanda/LMLexicon)
  > LM-Lexicon是一种新颖的词义定义建模方法，整合了数据聚类、语义专家学习和稀疏混合专家（MoE）架构的模型合并技术。通过将定义建模任务分解为多个语义领域，并训练小型语言模型作为各领域专家，LM-Lexicon在五个广泛使用的基准上相比最先进方法提升了7% BLEU分数。聚类策略带来近10%的定义质量提升；语义感知的领域级路由机制比词级路由高1%；测试时计算扩展和语义专家缩放可进一步提升性能。

- **DHPLT: large-scale multilingual diachronic corpora and word representations for semantic change modelling** `[微调]` — [2602.11968](https://arxiv.org/abs/2602.11968) | [GitHub](https://github.com/ltgoslo/scdisc_hplt)
  > 本文发布DHPLT，一个基于网络爬取HPLT数据集的41种语言开放二历时语料集合，覆盖2011-2015、2020-2021和2024至今三个时间段，每种语言每期100万文档。作者额外提供了预计算的词类型/词元嵌入及词汇替换，以支持语义变化建模研究。DHPLT旨在填补当前超出十余种高资源语言外多语言二历时语料的空白，为语义变化研究提供多样化实验设置基础。所有资源公开可访问，代码通过src目录和.slurm脚本提供可复现的实验流程。


## 2026年2月18日

- **GLM-5: from Vibe Coding to Agentic Engineering** `[RL]` — [2602.15763](https://arxiv.org/abs/2602.15763) | [GitHub](https://github.com/zai-org/GLM-5)
  > 本文介绍 GLM-5，一个为「智能工程」范式设计的下一代基础模型。GLM-5 在前代 ARC（代理、推理、编码）能力基础上，采用 DSA（DeepSeek Sparse Attention）大幅降低训练与推理成本，同时维持长上下文保真度。参数规模从 355B（32B active）扩展至 744B（40B active），预训练数据从 23T 增至 28.5T tokens。为提升后训练效率，作者开发了 slime 异步强化学习基础设施，实现训练吞吐量的显著提升。GLM-5 在推理、编码和智能体任务上达到所有开源模型中最优水平，在 CC-Bench-V2 和 Vending Bench 2 上显著超越 GLM-4.7。

- **Does Socialization Emerge in AI Agent Society? A Case Study of Moltbook** — [2602.14299](https://arxiv.org/abs/2602.14299) | [GitHub](https://github.com/tianyi-lab/Moltbook_Socialization)
  > 随着 LLM 智能体越来越多地进入网络化环境，一个根本问题出现了：AI 智能体社会是否会经历类似人类社会的收敛动态？本文对 Moltbook AI 智能体社会进行首次大规模系统性诊断，引入量化诊断框架，从语义稳定化、词汇更替、个体惯性、影响力持久性和集体共识等维度进行测量。研究发现：仅靠规模和交互密度不足以诱发社会化现象，提供了下一代 AI 智能体社会的设计与分析原则。

- **ResearchGym: Evaluating Language Model Agents on Real-World AI Research** — [2602.15112](https://arxiv.org/abs/2602.15112) | [GitHub](https://github.com/Anikethh/ResearchGym)
  > 本文提出 ResearchGym，一个用于评估 AI 智能体端到端科研能力的基准与执行环境。作者从 ICML、ICLR、ACL 的 5 篇 oral/spotlight 论文仓库中保留数据集、评估框架和基线实现，但隐去论文提出的方法，形成 5 个容器化任务环境，共 39 个子任务。智能体须提出新颖假设、实现并验证，从而推动科研进展。实验评估了多种前沿 LLM 智能体，分析其在现实 AI 研究任务中的能力边界。

- **Revisiting the Platonic Representation Hypothesis: An Aristotelian View** `[无需训练]` — [2602.14486](https://arxiv.org/abs/2602.14486) | [GitHub](https://github.com/mlbio-epfl/aristotelian)
  > 「柏拉图表示假说」认为神经网络的表示正在收敛到现实的共同统计模型。本文发现，现有衡量表示相似性的指标受网络规模混淆：增加模型深度或宽度会系统性地虚高相似性分数。为此，作者引入基于置换的空值校准框架，将任意表示相似性度量转化为规模不变的检验统计量。经校正后，表示收敛现象大幅减弱甚至消失，提示「柏拉图假说」的结论需重新审视。

- **TAROT: Test-driven and Capability-adaptive Curriculum Reinforcement Fine-tuning for Code Generation with Large Language Models** `[RL]` `[微调]` — [2602.15449](https://arxiv.org/abs/2602.15449) | [GitHub](https://github.com/deep-diver/TAROT)
  > TAROT 提出一种测试驱动、能力自适应的课程式强化微调框架，用于提升 LLM 代码生成能力。现有方法忽视测试用例的异构难度，导致奖励信号失衡。TAROT 通过两阶段设计：首先利用测试覆盖率和边界条件构建能力感知的课程，动态分配难度；然后通过强化微调优化通过率和鲁棒性。在多个代码生成基准上，TAROT 相较于直接 RFT 方法取得显著提升，在复杂算法题上尤为突出。

- **Understanding vs. Generation: Navigating Optimization Dilemma in Multimodal Models** `[VLM]` `[微调]` — [2602.15772](https://arxiv.org/abs/2602.15772) | [GitHub](https://github.com/sen-ye/R3)
  > 当前多模态模型研究面临一个核心挑战：提升生成能力往往以牺牲理解能力为代价，反之亦然。本文分析了这一权衡，认为根本原因在于生成与理解目标之间存在潜在冲突，形成模型内部的竞争动态。为此提出 Reason-Reflect-Refine（R3）框架，将单步生成任务重构为多步推理过程：先推理、再反思、后精炼。在多个多模态理解与生成基准上，R3 同时提升了两方面性能，有效缓解了优化困境。

- **Panini: Continual Learning in Token Space via Structured Memory** `[MeM]` `[长文本]` `[无需训练]` — [2602.15156](https://arxiv.org/abs/2602.15156) | [GitHub](https://github.com/roychowdhuryresearch/gsw-memory)
  > Panini 提出一种类人的非参数持续学习框架，基础模型保持固定，通过将每次新经验整合到外部语义记忆状态中实现持续学习。核心是「生成式语义工作空间（GSW）」——以实体和事件感知的问答对网络表示文档，支持 LLM 通过推理链重建情境并挖掘潜在知识。查询时仅遍历持续更新的 GSW 而非原始文档，检索最可能的推理链。在六个 QA 基准上，Panini 平均性能较竞争基线高出 5-7%，同时使用的答案上下文 token 减少 2-30 倍。

- **Prescriptive Scaling Reveals the Evolution of Language Model Capabilities** — [2602.15327](https://arxiv.org/abs/2602.15327) | [GitHub](https://github.com/hlzhang109/prescriptive-scaling)
  > 本文研究「处方式扩展律」：给定预训练算力预算，当代后训练实践能达到什么下游精度，以及该映射随时间演进的稳定性。作者使用 5k 观测和 2k 新采样的模型性能数据，通过带单调饱和 sigmoid 参数化的平滑分位数回归估计能力边界。验证表明，各任务的能力边界基本稳定，但数学推理能力边界持续推进。同时发布 Proteus 2k 数据集，并提供高效算法，仅用约 20% 评估预算即可恢复接近完整的数据前沿。

- **The Vision Wormhole: Latent-Space Communication in Heterogeneous Multi-Agent Systems** `[VLM]` `[无需训练]` — [2602.15382](https://arxiv.org/abs/2602.15382) | [GitHub](https://github.com/xz-liu/heterogeneous-latent-mas)
  > 多智能体系统（MAS）依赖离散文本通信存在显著开销和信息量化损失，而现有潜在状态传输方案要么假设同构架构，要么依赖成对学习的翻译器，限制了可扩展性。本文提出「视觉虫洞」框架，通过共享潜在空间实现异构多智能体间的高带宽视觉信息传递。作者设计了架构无关的编解码机制，支持不同 VLM 架构间的潜在表示对齐与传输，显著降低通信开销并减少信息损失，在多智能体协作推理任务上取得性能提升。

- **ClinAlign: Scaling Healthcare Alignment from Clinician Preference** `[微调]` — [2602.09653](https://arxiv.org/abs/2602.09653) | [GitHub](https://github.com/AQ-MedAI/ClinAlign)
  > ClinAlign 提出一个两阶段框架，将 LLM 输出与临床医生的细粒度偏好对齐。第一阶段构建 HealthRubrics 数据集：包含 7,034 个医生验证的偏好样本，临床医生基于专业指南优化 LLM 起草的评分标准，涵盖准确性、安全性和可操作性等多个维度。第二阶段利用该数据通过偏好优化方法对医疗 LLM 进行微调。实验显示，ClinAlign 在医疗问答和临床摘要任务上显著优于现有对齐基线，在医生评估中尤为突出。

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
