## 2026年2月11日

- **Chain of Mindset: Reasoning with Adaptive Cognitive Modes** `[无需训练]` — [2602.10063](https://arxiv.org/abs/2602.10063) | [GitHub](https://github.com/QuantaAlpha/chain-of-mindset)
  > Chain of Mindset (CoM) 提出步级自适应认知模式编排框架，将推理分解为四种思维模式（空间、收敛、发散、算法），由 Meta-Agent 根据推理状态动态选择最优模式，双向上下文门控模块维护跨模块信息流。无需训练，直接在推理时组合多种思维模式。在数学、代码生成、科学 QA 和空间推理六个基准上，在 Qwen3-VL-32B-Instruct 和 Gemini-2.0-Flash 上分别比最强基线提升 4.96% 和 4.72%。

---

## 2026年2月13日

- **Composition-RL: Compose Your Verifiable Prompts for Reinforcement Learning of Large Language Models** `[RL]` — [2602.12036](https://arxiv.org/abs/2602.12036) | [GitHub](https://github.com/XinXU-USTC/Composition-RL)
  > 通过将多个可验证问题自动组合为单一更难但仍可验证的复合提示来对抗"pass rate=1"的过易样本。结合逐步增加组合深度的课程学习策略，在 4B~30B 规模模型上一致提升推理性能，并在跨域 RL（数学+物理）中超越简单混合或顺序训练的效果。

- **DeepGen 1.0: A Lightweight Unified Multimodal Model for Advancing Image Generation and Editing** `[VLM]` `[微调]` `[RL]` — [2602.12205](https://arxiv.org/abs/2602.12205) | [GitHub](https://github.com/DeepGenTeam/DeepGen)
  > 仅 5B 参数（3B VLM + 2B DiT）的轻量统一多模态模型，集成图像生成、编辑、推理生成等五大能力。通过 SCB 架构和三阶段训练策略（预训练→SFT→MR-GRPO 强化学习），以 3~16 倍更小参数量达到与大模型竞争的性能。

- **Think Longer to Explore Deeper: Learn to Explore In-Context via Length-Incentivized Reinforcement Learning** `[RL]` — [2602.11748](https://arxiv.org/abs/2602.11748) | [GitHub](https://github.com/LINs-lab/LIE)
  > LIE 通过长度奖励鼓励模型延伸推理过程，通过冗余惩罚抑制重复 token。在 Qwen3 和 Llama 上相较 GRPO/GSPO 实现 +4.4% 域内、+2.7% OOD 提升，展现出更好的推理计算扩展曲线，有效避免标准 RL 模型的饱和退化。

- **dVoting: Fast Voting for dLLMs** `[无需训练]` — [2602.12153](https://arxiv.org/abs/2602.12153) | [GitHub](https://github.com/fscdc/dVoting)
  > 针对扩散大语言模型提出快速投票方法，利用其并行解码特性实现高效集成推理。在 GSM8K、MATH500、GPQA 等基准上对 LLaDA-8B-Instruct 和 Dream-v0 等模型验证了在保持精度同时大幅提升投票速度的效果。

- **Unveiling Implicit Advantage Symmetry: Why GRPO Struggles with Exploration and Difficulty Adaptation** `[RL]` — [2602.05548](https://arxiv.org/abs/2602.05548) | [GitHub](https://github.com/HKU-HealthAI/A-GRAE)
  > 揭示 GRPO 中存在的隐式优势对称性问题，导致探索不足和对样本难度的错误估计。提出 A-GRAE（Asymmetric GRAE），通过打破对称性改善探索效率和训练动态，在 RLVR 数学推理任务上展现出更好的探索多样性和整体推理性能。

- **Dreaming in Code for Curriculum Learning in Open-Ended Worlds** `[RL]` — [2602.08194](https://arxiv.org/abs/2602.08194) | [GitHub](https://github.com/konstantinosmitsides/dreaming-in-code)
  > DiCode 使用基础模型生成可执行 Python 代码作为训练环境，为 RL 智能体创建自适应课程。在 Dream-Evaluate-Refine 闭环中运行，在开放世界游戏 Craftax 上比最强基线高出 16% 平均回报，并在基线完全失败（0%成功率）的深层任务上实现非零突破。

- **Sci-CoE: Co-evolving Scientific Reasoning LLMs via Geometric Consensus with Sparse Supervision** `[RL]` `[微调]` — [2602.12164](https://arxiv.org/abs/2602.12164) | [GitHub](https://github.com/InternScience/Sci-CoE)
  > 解决科学推理中无显式答案情景下的 RL 训练难题。提出两阶段共进化框架：第一阶段用少量标注数据建立验证锚点；第二阶段引入几何奖励机制，联合建模共识性、可靠性和多样性，在无标注数据上实现稳定可扩展的自迭代，无需依赖外部评判器。

- **P-GenRM: Personalized Generative Reward Model with Test-time User-based Scaling** `[RL]` `[无需训练]` — [2602.12116](https://arxiv.org/abs/2602.12116) | [GitHub](https://github.com/Tongyi-ConvAI/Qwen-Character)
  > 将用户偏好信号转化为结构化评估链，通过构建用户原型支持测试时用户级扩展。在个性化奖励模型基准上达到 SOTA，被 ICLR 2026 接收为 Oral（Top 1%）。

---

## 2026年2月17日

- **Experiential Reinforcement Learning** `[RL]` — [2602.13949](https://arxiv.org/abs/2602.13949) | [GitHub](https://github.com/microsoft/experiential_rl)
  > 在 RL 训练过程中嵌入"经验-反思-巩固"显式循环。模型先生成初始尝试，接收反馈后产生反思并指导第二次更优尝试，成功结果被强化内化为基础策略。在稀疏奖励控制环境和智能体推理任务上比强 RL 基线最多提升 81%。

- **STATe-of-Thoughts: Structured Action Templates for Tree-of-Thoughts** `[无需训练]` — [2602.14265](https://arxiv.org/abs/2602.14265) | [GitHub](https://github.com/zbambergerNLP/state-of-thoughts)
  > 通过搜索高层次推理模式替代随机温度采样的推理时计算方法，包含控制器-生成器-评估器三组件框架。动作引导干预比温度采样产生更高输出多样性，动作序列对输出质量高度可预测。

- **Learning to Configure Agentic AI Systems** `[RL]` — [2602.11574](https://arxiv.org/abs/2602.11574) | [GitHub](https://github.com/somsagar07/Context_Optimization)
  > ARC 将 LLM 智能体系统配置形式化为逐查询决策问题，使用 RL 训练轻量级层次策略动态裁剪配置。在推理和工具增强问答等多个任务上，学习策略比手工设计基线任务准确率提升最多 25%，同时降低 Token 消耗和运行时间。

- **Embed-RL: Reinforcement Learning for Reasoning-Driven Multimodal Embeddings** `[RL]` `[VLM]` — [2602.13823](https://arxiv.org/abs/2602.13823) | [GitHub](https://github.com/ZoengHN/Embed-RL)
  > 引入嵌入器引导强化学习（EG-RL）优化推理器生成可追溯的 CoT（T-CoT）。EG-RL 让 Embedder 为 Reasoner 提供显式监督，T-CoT 提取多模态关键线索聚焦检索相关元素。在 MMEB-V2 和 UVRB 基准上以有限计算资源超越现有嵌入模型。

- **Conversational Image Segmentation: Grounding Abstract Concepts with Scalable Supervision** `[VLM]` — [2602.13195](https://arxiv.org/abs/2602.13195) | [GitHub](https://github.com/AadSah/ConverSeg)
  > 提出会话式图像分割任务，将功能、意图、安全等抽象概念接地到像素级掩码。构建 ConverSeg 基准涵盖多类型查询，设计无需人工标注的 AI 数据引擎自动生成提示-掩码对，在 ConverSeg 上取得显著提升。

- **A Critical Look at Targeted Instruction Selection** `[微调]` — [2602.14696](https://arxiv.org/abs/2602.14696) | [GitHub](https://github.com/dcml-lab/targeted-instruction-selection)
  > 系统分析 LLM 指令微调中目标数据选择方法的核心要素。发现仅基于梯度的数据表示在跨数据集和模型时能一致预测性能；低预算下梯度表示配合贪婪轮询选择算法表现最佳。将多种选择算法统一为近似距离最小化框架。

- **Found-RL: foundation model-enhanced reinforcement learning for autonomous driving** `[RL]` `[VLM]` — [2602.10458](https://arxiv.org/abs/2602.10458) | [GitHub](https://github.com/ys-qu/found-rl)
  > 通过基础模型增强自动驾驶强化学习。异步批量推理框架将 VLM 推理与仿真循环解耦；引入 Value-Margin 正则化和优势加权动作引导将 VLM 专家建议蒸馏入 RL 策略。轻量级 RL 模型实现近 VLM 性能（约 500 FPS 实时推理）。

---

## 2026年2月18日

- **TAROT: Test-driven and Capability-adaptive Curriculum Reinforcement Fine-tuning for Code Generation** `[RL]` `[微调]` — [2602.15449](https://arxiv.org/abs/2602.15449) | [GitHub](https://github.com/deep-diver/TAROT)
  > 测试驱动的能力自适应课程强化微调方法用于代码生成。为每道题构建四级测试套件，课程进度与原始奖励分数解耦。发现能力较弱的模型通过由易到难获益更多，能力较强的模型在先难后易下表现更好。

- **Understanding vs. Generation: Navigating Optimization Dilemma in Multimodal Models** `[VLM]` — [2602.15772](https://arxiv.org/abs/2602.15772) | [GitHub](https://github.com/sen-ye/R3)
  > 提出 Reason-Reflect-Refine（R3）框架，将单步生成任务重构为"生成-理解-再生成"的多步过程，显式利用模型理解能力指导生成。在不牺牲理解性能的前提下实现了更强的生成结果。

- **The Vision Wormhole: Latent-Space Communication in Heterogeneous Multi-Agent Systems** `[VLM]` — [2602.15382](https://arxiv.org/abs/2602.15382) | [GitHub](https://github.com/xz-liu/heterogeneous-latent-mas)
  > 复用 VLM 的视觉接口实现异构多智能体间免文本的潜空间通信。Universal Visual Codec 将异构推理轨迹映射到共享潜空间，采用轮毂-辐射拓扑将配对复杂度从 O(N²) 降至 O(N)。

- **ClinAlign: Scaling Healthcare Alignment from Clinician Preference** `[微调]` — [2602.09653](https://arxiv.org/abs/2602.09653) | [GitHub](https://github.com/AQ-MedAI/ClinAlign)
  > 两阶段医疗对齐框架：构建 HealthRubrics 数据集（7034个医师验证的偏好样本），蒸馏为 119 条 HealthPrinciples 支持离线对齐和推理时自我修正。30B 参数（激活 3B）模型在 HealthBench-Hard 上超过 DeepSeek-R1 和 o3。

---

## 2026年2月19日

- **CADEvolve: Creating Realistic CAD via Program Evolution** `[VLM]` `[微调]` — [2602.16317](https://arxiv.org/abs/2602.16317) | [GitHub](https://github.com/zhemdi/CADEvolve)
  > 进化驱动的 CAD 程序生成框架，通过 VLM 引导的编辑和验证迭代生成工业级复杂 CAD 程序。生成 130 万脚本数据集，在此上微调的 VLM 在 DeepCAD、Fusion 360 和 MCB 数据集的 Image2CAD 任务上达到最新 SOTA。

---

## 2026年2月24日

- **Mobile-O: Unified Multimodal Understanding and Generation on Mobile Device** `[VLM]` `[微调]` — [2602.20161](https://arxiv.org/abs/2602.20161) | [GitHub](https://github.com/Amshaker/Mobile-O)
  > 面向移动端的紧凑型视觉-语言-扩散统一模型，基于 Qwen2-0.5B + FastViT + SANA DiT，总内存不足 2GB，可在 iPhone 15 Pro 以上设备实时运行。通过 LoRA 微调联合优化理解与生成能力。

- **AAVGen: Precision Engineering of Adeno-associated Viral Capsids for Renal Selective Targeting** `[RL]` `[微调]` — [2602.18915](https://arxiv.org/abs/2602.18915) | [GitHub](https://github.com/mohammad-gh009/AAVGen)
  > 用于从头设计 AAV 病毒衣壳的生成式 AI 框架，将蛋白质语言模型（ProtGPT2）与 SFT 和 GSPO（基于 PPO 的 RL）结合。生成 500,000 条序列中 99.7% 在生产适应性方面达到最优，AlphaFold3 结构分析确认折叠保守性。

---

## 2026年2月25日

- **PyVision-RL: Forging Open Agentic Vision Models via RL** `[RL]` `[VLM]` — [2602.20739](https://arxiv.org/abs/2602.20739) | [GitHub](https://github.com/agents-x-project/PyVision-RL)
  > 针对多模态智能体 RL 训练中的交互崩塌问题，通过过采样-过滤-排序 rollout 策略与累积工具奖励防止崩塌并鼓励多轮工具使用。PyVision-Video 采用按需上下文构建，选择性采样任务相关帧显著减少视觉 token 消耗。

---

## 2026年2月26日

- **ARLArena: A Unified Framework for Stable Agentic Reinforcement Learning** `[RL]` — [2602.21534](https://arxiv.org/abs/2602.21534) | [GitHub](https://github.com/WillDreamer/ARL-Arena)
  > 针对智能体 RL 训练不稳定性的系统分析框架，将策略梯度分解为四个核心设计维度。基于此提出 SAMPO——稳定的智能体策略优化方法，在网页浏览和工具使用等智能体任务上显著优于不稳定基线。

- **GUI-Libra: Training Native GUI Agents to Reason and Act with Action-aware Supervision and Partially Verifiable RL** `[RL]` `[微调]` — [2602.22190](https://arxiv.org/abs/2602.22190) | [GitHub](https://github.com/GUI-Libra/GUI-Libra)
  > 结合动作感知监督和部分可验证强化学习训练原生 GUI 智能体。SFT 阶段建立动作感知监督，PVRL 阶段利用可验证奖励精炼策略。在 AndroidWorld、WebArena 等基准上取得 SOTA。

- **NoLan: Mitigating Object Hallucinations in Large Vision-Language Models via Dynamic Suppression of Language Priors** `[VLM]` `[无需训练]` — [2602.22144](https://arxiv.org/abs/2602.22144) | [GitHub](https://github.com/lingfengren/NoLan)
  > 动态语言先验抑制方法，在解码时识别并降低与当前图像不一致的语言先验对输出的影响，无需额外训练即可减少幻觉。可直接应用于现有 VLM，在多个幻觉评测基准上验证有效性。

---

## 2026年2月27日

- **From Blind Spots to Gains: Diagnostic-Driven Iterative Training for Large Multimodal Models** `[RL]` `[VLM]` — [2602.22859](https://arxiv.org/abs/2602.22859) | [GitHub](https://github.com/hongruijia/DPE)
  > DPE 是 LMM 自进化训练框架，多智能体协同标注无标注多模态数据并将失败案例归因到特定弱点，动态调整数据配比生成针对性强化数据。在 Qwen3-VL-8B 和 Qwen2.5-VL-7B 上跨 11 个基准稳定持续提升。

- **Imagination Helps Visual Reasoning, But Not Yet in Latent Space** `[VLM]` — [2602.22766](https://arxiv.org/abs/2602.22766) | [GitHub](https://github.com/AI9Stars/CapImagine)
  > 通过因果中介分析揭示多模态 LLM 中潜在视觉推理的两个关键断层，提出 CapImagine 替代方案，训练模型使用文本显式表达想象过程。在以视觉为中心的基准上显著优于复杂潜在空间基线。

- **Exploratory Memory-Augmented LLM Agent via Hybrid On- and Off-Policy Optimization** `[RL]` — [2602.23008](https://arxiv.org/abs/2602.23008) | [GitHub](https://github.com/beanie00/EMPO)
  > EMPO² 提出混合在策略+离策略优化框架，利用记忆增强探索。在 ScienceWorld 和 WebShop 上分别比 GRPO 提升 128.6% 和 11.3%；在分布外测试中对新任务的适应能力优于基线。

---

## 2026年3月2日

- **dLLM: Simple Diffusion Language Modeling** — [2602.22661](https://arxiv.org/abs/2602.22661) | [GitHub](https://github.com/ZHZisZZ/dllm)
  > 简洁的扩散语言模型实现，通过离散扩散过程替换自回归解码，统一了掩码扩散（MDM）和吸收扩散（ADM）等主流变体。提供标准化训练和评估基础设施，深入分析并行解码带来的测试时计算扩展潜力。

- **Ref-Adv: Exploring MLLM Visual Reasoning in Referring Expression Tasks** `[VLM]` `[微调]` — [2602.23898](https://arxiv.org/abs/2602.23898) | [GitHub](https://github.com/dddraxxx/Ref-Adv)
  > 针对指称表达任务提出对抗性干扰评估框架，在目标对象周围引入高度相似的干扰对象测试精细视觉区分能力。发现通过构造对抗训练数据进行 SFT 可显著提升模型鲁棒性。

- **DUET-VLM: Dual stage Unified Efficient Token reduction for VLM Training and Inference** `[VLM]` — [2602.18846](https://arxiv.org/abs/2602.18846) | [GitHub](https://github.com/AMD-AGI/DUET-VLM)
  > 两阶段统一视觉 token 压缩框架，同时优化 VLM 的训练和推理效率。训练阶段通过结构化剪枝减少计算开销；推理阶段通过动态 token 合并压缩序列长度。在 LLaVA 等主流 VLM 上训练速度提升约 1.5×。

---

## 2026年3月3日

- **CHIMERA: Compact Synthetic Data for Generalizable LLM Reasoning** `[微调]` — [2603.00889](https://arxiv.org/abs/2603.00889)
  > CHIMERA 针对 LLM 推理能力复现的三大数据瓶颈（冷启动缺乏详细 CoT 轨迹、领域覆盖局限于数学、标注成本高）提出 9K 样本跨领域合成推理数据集。涵盖 8 个科学领域和 1K+ 细粒度话题，使用最强推理模型合成长 CoT 轨迹并交叉验证答案正确性。用 CHIMERA 后训练 Qwen3-4B 后，在 GPQA-Diamond、AIME 24/25/26、HMMT 25 和 Humanity's Last Exam 上接近甚至超过 DeepSeek-R1 和 Qwen3-235B（Apple 出品）。

- **Spectral Condition for μP under Width-Depth Scaling** — [2603.00541](https://arxiv.org/abs/2603.00541) | [GitHub](https://github.com/ML-GSAI/Width-Depth-muP)
  > 针对最大更新参数化（μP）在宽度-深度联合 scaling 中的失效问题，提出谱条件，给出 μP 在宽度和深度同时扩展时的理论充要条件，推导出联合宽度-深度 scaling 的新初始化方案和学习率调度建议。

- **When Does RL Help Medical VLMs? Disentangling Vision, SFT, and RL Gains** `[RL]` `[VLM]` `[微调]` — [2603.01301](https://arxiv.org/abs/2603.01301) | [GitHub](https://github.com/armenjeddi/medbridgerl)
  > 系统分析 RL 在医疗 VLM 中的作用：视觉编码器质量影响最大；SFT 提供任务适应基础；RL 在 SFT 已充分情况下带来额外增益。基于此提出 MedBridgeRL，在多个医疗影像推理基准上达到 SOTA。

- **SEKA: Spectral Attention Steering for Prompt Highlighting** `[无需训练]` — [2603.01281](https://arxiv.org/abs/2603.01281) | [GitHub](https://github.com/waylonli/SEKA)
  > 基于谱分析的注意力引导方法，通过在推理时对注意力矩阵的谱分解结果进行干预，放大关键 token 的注意力权重而无需重新训练模型。在长文本理解和指令遵循任务上显著优于提示工程基线。

- **Reasoning Core: A Scalable Procedural Data Generation Suite for Symbolic Pre-training and Post-Training** `[RL]` `[微调]` — [2603.02208](https://arxiv.org/abs/2603.02208) | [GitHub](https://github.com/sileod/reasoning_core)
  > 可扩展的程序化推理数据生成套件，支持符号预训练和后训练。通过程序化方式生成覆盖算术、逻辑、图论等多种符号推理类型的大规模训练数据，所有样本均带有可验证答案，支持 RLVR 训练。

- **RAISE: Requirement-Adaptive Evolutionary Refinement for Training-Free Text-to-Image Alignment** `[无需训练]` — [2603.00483](https://arxiv.org/abs/2603.00483) | [GitHub](https://github.com/LiyaoJiang1998/RAISE)
  > 无需训练的 T2I 对齐优化框架，由多模态 LLM 评估生成图像与需求的不足并生成针对性修订提示，引导扩散模型在潜空间中进行自适应精炼。支持对属性绑定、计数、空间关系等复杂语义需求的对齐优化。

- **Tool Verification for Test-Time Reinforcement Learning** `[RL]` `[无需训练]` — [2603.02203](https://arxiv.org/abs/2603.02203)
  > T³RL 针对测试时强化学习（TTRL）中多数投票引发虚假奖励共识、导致错误模式坍塌的问题，在奖励估计中引入测试时工具验证机制。使用外部工具（如代码执行）的返回结果作为证据，对多数投票的奖励信号进行校正，过滤不可靠共识并引导模型向经验证的正确方向演化。实验表明在数学和代码推理任务上显著优于仅依赖多数投票的 TTRL 基线，有效避免了模式坍塌。

---

## 2026年3月4日

- **Beyond Language Modeling: An Exploration of Multimodal Pretraining** `[VLM]` — [2603.03276](https://arxiv.org/abs/2603.03276)
  > Meta 通过受控从头预训练实验（Transfusion 框架）系统性地探索多模态预训练设计空间，得出四个关键洞察：RAE 是最优统一视觉表示；视觉与语言数据互补产生协同增益；统一多模态预训练自然涌现世界建模能力；MoE 可高效扩展多模态模型并诱导模态专业化。IsoFLOP 分析揭示了视觉-语言 scaling 不对称性（视觉更数据饥渴），MoE 正好弥合这一不对称性。

- **Pushing the Frontier of Deep Think via Process Reward Model-Guided Inference** `[无需训练]` — [2603.02479](https://arxiv.org/abs/2603.02479)
  > PRISM 针对 DeepThink 系统中缺乏可靠正确性信号导致"更深思考放大错误"的瓶颈，引入 PRM 指导的推理算法。通过步级验证对候选解的推理轨迹进行在线评估，动态剪枝低质量路径、保留高价值轨迹，在候选解群体中实现精准正确性引导。实验表明在复杂数学和科学推理任务上显著优于无 PRM 引导的 DeepThink 基线，且随着计算预算增加持续受益。

---

## 2026年3月5日

- **Heterogeneous Agent Collaborative Reinforcement Learning** `[RL]` — [2603.02604](https://arxiv.org/abs/2603.02604)
  > HACRL 提出异构智能体协作 RL 范式，允许异构智能体在训练时共享经过验证的 rollout 相互提升，推理时保持独立运行。HACPO 算法通过有原则的 rollout 共享最大化样本利用率和跨智能体知识转移，引入四种机制保证无偏优势估计。在各类异构模型组合上平均优于 GSPO 3.3%，仅使用其一半 rollout 成本。

- **MemSifter: Offloading LLM Memory Retrieval via Outcome-Driven Proxy Reasoning** `[RL]` `[长文本]` — [2603.03379](https://arxiv.org/abs/2603.03379) | [GitHub](https://github.com/plageon/MemSifter)
  > MemSifter 将 LLM 长期记忆检索任务卸载至小型代理模型，系统采用三阶段流水线：会话嵌入粗筛、MemSifter 生成式精排、下游 LLM 生成答案。引入基于任务结果的 RL 训练范式，以主工作 LLM 的实际任务完成质量作为奖励信号，结合课程学习和模型融合。在八个 LLM 记忆基准（含 Deep Research）上达到或超越现有最优方法。

- **Memex(RL): Scaling Long-Horizon LLM Agents via Indexed Experience Memory** `[RL]` `[长文本]` — [2603.04257](https://arxiv.org/abs/2603.04257)
  > Memex 针对 LLM 智能体在长时域任务中受限于有限上下文窗口的瓶颈，提出带索引的经验记忆机制。维护紧凑的工作上下文（结构化摘要+稳定索引）并将完整轨迹存入持久化记忆库，实现无损上下文压缩。结合 RL 训练使智能体学习高效利用索引记忆，在超长任务中保持对远端证据的完整访问能力。

- **V_1: Unifying Generation and Self-Verification for Parallel Reasoners** `[RL]` `[无需训练]` — [2603.04304](https://arxiv.org/abs/2603.04304) | [GitHub](https://github.com/HarmanDotpy/pairwise-self-verification)
  > V₁ 统一了生成与自我验证，利用模型在成对比较上显著强于逐点打分的洞察，提出基于锦标赛排名的推理时扩展框架。V₁-Infer 通过不确定性引导的瑞士循环赛动态分配验证算力；V₁-PairRL 同时训练生成器和成对验证器。在代码生成和数学推理任务上，相比逐点验证提升 Pass@1 最高 10%，相比标准 RL 提升 8.7%。

- **Specificity-aware reinforcement learning for fine-grained open-world classification** `[RL]` `[VLM]` — [2603.03197](https://arxiv.org/abs/2603.03197)
  > SpeciaRL 针对开放世界细粒度视觉分类中大型多模态模型预测过于笼统的问题，设计特异性感知奖励函数：既奖励正确的细粒度预测，又惩罚在正确预测上的过度泛化。实验证明能有效引导推理型 LMM 在开放世界场景下给出既准确又具体的细粒度分类结果。

- **BeamPERL: Parameter-Efficient RL with Verifiable Rewards Specializes Compact LLMs for Structured Beam Mechanics Reasoning** `[RL]` `[微调]` — [2603.04124](https://arxiv.org/abs/2603.04124) | [GitHub](https://github.com/lamm-mit/BeamPERL)
  > 使用 1.5B 参数推理模型，通过 LoRA 适配器进行 RLVR 训练，奖励信号来自符号求解器的二进制正确性判断，无需教师推理轨迹。最优检查点在 Pass@1 上相比基础模型提升 66.7%。发现学习到的能力具有各向异性：模型可组合泛化，但在拓扑变化下失败，表明精确可验证奖励可能诱导程序化模板而非真正的方程内化。

---

## 2026年3月6日

- **MOOSE-Star: Unlocking Tractable Training for Scientific Discovery by Breaking the Complexity Barrier** `[微调]` — [2603.03756](https://arxiv.org/abs/2603.03756) | [GitHub](https://github.com/ZonglinY/MOOSE-Star)
  > MOOSE-Star 解决了科学发现假设生成训练中 O(N^k) 指数级复杂度瓶颈。通过三步将复杂度降至 O(log N)：分解假设组合为逐步单灵感序列任务、训练独立灵感检索模型、在聚类树上进行层次化搜索。数据集 TOMATO-Star 包含 108,717 篇分解论文（耗费 38,400 GPU 小时）。基于 DeepSeek-R1-Distill-Qwen-7B 并用 32B 教师模型进行拒绝采样训练，在测试时展现出持续的计算扩展性。

---

## 2026年3月8日

- **Reasoning Models Struggle to Control their Chains of Thought** `[RL]` — [2603.05706](https://arxiv.org/abs/2603.05706)
  > 提出 CoT 可控性（CoT Controllability）概念与评测套件 CoT-Control，衡量推理模型在遵循 CoT 约束指令时的能力。发现推理模型的 CoT 可控性远低于输出可控性——Claude Sonnet 4.5 控制 CoT 仅成功 2.7%，控制输出达 61.9%。CoT 可控性随模型规模增大而提升，但随 RL 训练量增加、测试时计算增多及问题难度提升而下降。对抗性提示优化或激励机制均难以显著提升 CoT 可控性，这对 CoT 监控性安全研究具有积极意义。
- **FlashPrefill: Instantaneous Pattern Discovery and Thresholding for Ultra-Fast Long-Context Prefilling** `[长文本]` `[无需训练]` — [2603.06199](https://arxiv.org/abs/2603.06199) | [GitHub](https://github.com/qhfan/FlashPrefill)
  > FlashPrefill 是针对 LLM 长上下文 prefilling 阶段的高效稀疏注意力框架。通过快速块搜索技术同时定位垂直、斜线和块稀疏注意力模式，并引入动态阈值机制，无需排序或累加注意力分数即可消除长尾分布、提升稀疏度。在 256K 序列上实现 27.78 倍加速，在 4K 上下文长度下仍维持 1.71 倍加速，已集成至 vLLM。

---

## 2026年3月9日

- **BandPO: Bridging Trust Regions and Ratio Clipping via Probability-Aware Bounds for LLM Reinforcement Learning** `[RL]` — [2603.04918](https://arxiv.org/abs/2603.04918) | [GitHub](https://github.com/OpenMOSS/BandPO)
  > 针对 LLM 强化学习中固定 PPO 裁剪边界压缩低概率动作探索空间、诱发熵崩塌的问题，提出 Band 算子作为统一理论替代方案。Band 将 f-散度定义的信任域映射为动态概率感知裁剪区间，对低概率高优势的 tail token 自适应扩展上行探索幅度，同时满足概率单纯形约束。在 Qwen2.5、Llama3 等模型和多个数学推理数据集上持续优于 GRPO 和 Clip-Higher，同时稳健抑制熵崩塌。
- **Progressive Residual Warmup for Language Model Pretraining** — [2603.05369](https://arxiv.org/abs/2603.05369) | [GitHub](https://github.com/dandingsky/ProRes)
  > ProRes 针对 Transformer LLM 预训练稳定性问题，提出渐进式残差预热策略：对每层残差连接乘以从 0 到 1 线性预热的标量，越深的层预热步数越长，实现"早层先学，深层后学"。在 Pre-LN、Sandwich-LN、Post-LN 等多种归一化方案和 130M~7B 参数规模的预训练实验中，ProRes 均能稳定训练、加快收敛、提升泛化能力和下游性能。
- **Nabla-Reasoner: LLM Reasoning via Test-Time Gradient Descent in Latent Space** `[无需训练]` — [2603.04948](https://arxiv.org/abs/2603.04948) | [GitHub](https://github.com/VITA-Group/Nabla-Reasoner)
  > ∇-Reasoner（ICLR 2026）在解码循环中引入可微优化（DTO），利用 LLM 似然和奖励模型的梯度信号在 token logit 空间对策略进行实时精炼，无需离线训练即可提升推理质量。理论上证明推理时梯度下降以最大化奖励等价于 KL 正则 RL 对齐。在数学推理基准上超过基线 20% 以上精度，同时减少模型调用次数。
- **Censored LLMs as a Natural Testbed for Secret Knowledge Elicitation** `[微调]` — [2603.05494](https://arxiv.org/abs/2603.05494) | [GitHub](https://github.com/cywinski/chinese_auditing)
  > 将中文开源 LLM（如 Qwen3）对政治敏感话题的审查行为作为诚实性引出方法的自然测试床。研究发现去掉 chat template 采样、few-shot 提示、在通用诚实数据上微调效果最佳；让被审查模型自我分类其回答的谎言检测效果接近无审查版本。提供了比人工构造说谎模型更贴近真实不诚实行为的评测场景。

---

## 2026年3月10日

- **How Far Can Unsupervised RLVR Scale LLM Training?** `[RL]` — [2603.08660](https://arxiv.org/abs/2603.08660)
  > 对无监督可验证奖励强化学习（URLVR）进行系统性分析，将其分为内在奖励和外部奖励两类，建立统一理论框架证明所有内在奖励方法本质上是对模型初始分布的"尖锐化"。该机制在置信度与正确性对齐时有效，但二者错位时会灾难性崩溃，导致内在奖励普遍呈现"先涨后塌"的模式。论文提出"模型崩塌步"（Model Collapse Step）作为衡量 RL 可训练性的实用指标，并展示外部奖励方法突破置信度-正确性上限的初步证据。
- **Believe Your Model: Distribution-Guided Confidence Calibration** `[无需训练]` — [2603.03872](https://arxiv.org/abs/2603.03872)
  > DistriVoting 利用置信度分布先验改进大型推理模型的测试时投票策略。用高斯混合模型将混合置信度分布分解为正负两类并进行 reject filter，同时提出 SelfStepConf 在推理中动态调整步骤级置信度以加大两分布间距，从根本上减少重叠。在 16 个模型和 5 个基准上显著优于最先进的测试时扩展投票方法，无需额外训练。

---

## 2026年3月11日

- **Thinking to Recall: How Reasoning Unlocks Parametric Knowledge in LLMs** `[无需训练]` — [2603.09906](https://arxiv.org/abs/2603.09906)
  > 研究推理对 LLM 参数化知识召回的影响。发现对于单跳事实性问题，启用推理链仍能显著扩展模型知识边界，识别出两种关键机制：(1) 计算缓冲效应——推理 token 提供潜在计算空间；(2) 事实启动效应——生成相关事实充当语义桥梁促进正确答案检索。同时警告推理中的幻觉中间事实会提升最终答案幻觉概率，并展示优先选择无幻觉推理轨迹可直接提升模型准确率。
- **Omni-Diffusion: Unified Multimodal Understanding and Generation with Masked Discrete Diffusion** `[VLM]` — [2603.06577](https://arxiv.org/abs/2603.06577) | [GitHub](https://github.com/VITA-MLLM/Omni-Diffusion)
  > Omni-Diffusion 是首个完全基于掩码离散扩散模型的任意到任意多模态语言模型，统一了文本、语音和图像的理解与生成。不同于主流自回归架构，使用单一掩码离散扩散模型直接建模多模态离散 token 的联合分布，支持双模态及多模态复杂场景。在多样化基准上与现有多模态系统相比性能持平或超越，证明扩散模型作为多模态基础模型骨干的巨大潜力。
- **MM-Zero: Self-Evolving Multi-Model Vision Language Models From Zero Data** `[RL]` `[VLM]` — [2603.09206](https://arxiv.org/abs/2603.09206) | [GitHub](https://github.com/zli12321/MM-Zero)
  > MM-Zero 是首个无需任何训练数据即可实现 VLM 自进化的 RL 框架。采用三角色协同框架：Proposer 生成视觉概念和问题，Coder 将概念转为可执行代码（Python/SVG）渲染图像，Solver 对生成内容进行多模态推理。三个角色均以 GRPO 强化学习训练，通过代码执行结果作为可验证奖励，无需任何标注数据即可自举多模态能力。在多个 VLM 基准上优于同规模有监督方法。

---

## 2026年3月12日

- **Bootstrapping Exploration with Group-Level Natural Language Feedback in Reinforcement Learning** `[RL]` — [2603.04597](https://arxiv.org/abs/2603.04597) | [GitHub](https://github.com/LuckyyySTA/GOLF)
  > GOLF 利用组级自然语言反馈引导 LLM 强化学习探索。聚合两类互补反馈：外部批评指出错误或修复建议，组内尝试提供多样化失败模式。这些组级反馈被聚合为高质量精炼意见，以离策略脚手架形式注入稀疏奖励区域，同时在统一 RL 循环中联合优化生成和精炼能力。实验在可验证与不可验证任务上均优于基线，相比纯标量奖励方法实现 2.2 倍样本效率提升。
- **V_{0.5}: Generalist Value Model as a Prior for Sparse RL Rollouts** `[RL]` — [2603.10848](https://arxiv.org/abs/2603.10848)
  > 在 RLVR 框架下提出自适应基线融合方法，将通用价值模型（V_0）的先验预测与稀疏 rollout 的经验均值动态结合，构建低方差且计算高效的优势基线。核心机制是实时统计检验与动态预算分配：通过假设检验评估价值先验可靠性，在需要时动态追加 rollout 配额，最小化基线估计均方误差。即使在 group size=4 的极端稀疏采样下也能保持稳定。在六个数学推理基准上显著优于 GRPO 和 DAPO，收敛更快且性能提升超过 10%。
- **Just-in-Time: Training-Free Spatial Acceleration for Diffusion Transformers** `[无需训练]` — [2603.10744](https://arxiv.org/abs/2603.10744)
  > JiT 提出无需训练的 Diffusion Transformer 空间加速框架。建立空间近似生成 ODE，仅用动态选择的稀疏锚点 token 子集驱动完整潜在状态演化，并引入确定性微流方法保持结构连贯性和统计正确性。在 FLUX.1-dev 模型上最高可达 7 倍加速，性能几乎无损，显著优于现有加速方法。
- **CLIPO: Contrastive Learning in Policy Optimization Generalizes RLVR** `[RL]` — [2603.10101](https://arxiv.org/abs/2603.10101) | [GitHub](https://github.com/Qwen-Applications/CLIPO)
  > 将对比学习机制引入 RLVR 策略优化流程，以解决现有方法仅依赖最终答案奖励、忽略中间推理步骤正确性的问题。通过在成功 rollout 上优化对比损失，引导 LLM 捕捉多条正确推理路径共享的不变结构，提供跨轨迹正则化，有效抑制推理不一致和幻觉。引入轻量级对比头从正确 rollout 中提取不变推理结构并生成密集对比奖励。在多个 RLVR 基线上持续提升泛化能力和鲁棒性。
- **LLM2Vec-Gen: Generative Embeddings from Large Language Models** `[微调]` — [2603.10913](https://arxiv.org/abs/2603.10913) | [GitHub](https://github.com/McGill-NLP/llm2vec-gen)
  > 提出自监督文本嵌入训练范式：不直接编码输入，而是学习表示模型对输入的潜在回答。在 LLM 词汇表中添加可训练特殊 token，将其附加于输入并优化为固定长度响应表示。训练由 LLM 自身生成的回答补全和无监督嵌入教师的蒸馏目标共同引导，LLM 主干参数保持冻结。在 MTEB 上比最优无监督教师提升 9.3%，有害内容检索降低 43.2%，推理能力提升 29.3%，嵌入还可解码还原为文本。
- **RbtAct: Rebuttal as Supervision for Actionable Review Feedback Generation** `[微调]` — [2603.09723](https://arxiv.org/abs/2603.09723) | [GitHub](https://github.com/formula12/RbtAct)
  > 针对 AI 生成学术审稿意见可操作性不足的问题，提出以同行评审 rebuttal 作为隐式监督信号直接优化反馈生成器。引入 RMR-75K 大型数据集（将审稿片段映射到对应 rebuttal 片段，含视角标签和影响类别），基于此用 SFT 训练 Llama-3.1-8B-Instruct 并以 rebuttal 衍生对进行 DPO 偏好优化。人工专家和 LLM-as-judge 评测显示，在保持准确性的同时，可操作性和具体性显著优于强基线。

