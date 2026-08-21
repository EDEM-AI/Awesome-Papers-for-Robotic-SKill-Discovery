# Awesome Papers for Robotic Skill Discovery

Papers that autonomously determine what robot skills or tasks should be learned, extract reusable skills from experience, or build data engines that generate validated data for newly discovered skills.

## What Counts as Robotic Skill Discovery?

A **skill demonstration** is one execution represented as a trajectory of state–action pairs, $\tau = (s_0,a_0,\ldots,s_T)$. A **skill** is a collection or distribution of trajectories that realize the same reusable capability, intent, or effect. Skill data may optionally be paired with a learned policy, controller, or executable program.

| Concept | Meaning | Output |
|---|---|---|
| **Skill discovery or acquisition** | Identifying a new capability and obtaining data that demonstrates it | A new skill dataset or skill repertoire |
| **Skill data engine** | Automatically proposing, generating, validating, and organizing skill trajectories | Validated datasets for newly discovered skills |
| **Task discovery or generation** | Proposing tasks or goals that require new capabilities | Tasks, goals, or training objectives |
| **Skill extraction or segmentation** | Finding reusable skills and their boundaries in recorded experience | Skill segments, prototypes, or hierarchies |
| **Skill data scaling** | Producing more trajectories for an already known skill | A larger and more diverse skill dataset |
| **Skill composition and planning** | Combining existing skills to solve longer tasks | Skill sequences, hierarchies, or plans |
| **Skill transfer and deployment** | Adapting existing skills to new settings | Skills transferred across objects, environments, or robots |

In this survey, a central application of skill discovery is an autonomous **skill data engine**: a system that identifies capabilities worth acquiring and produces validated state–action trajectories for learning them. This differs from data scaling, which increases the amount or diversity of data for skills that are already specified.

Paper entry format:

```markdown
- [YYYY.MM] PAPER TITLE [[paper](link)] [[project](link)] [[code](link)]
```

## 1. Surveys and Foundations of Robotic Skill Discovery

Surveys and foundational works that frame robotic skill discovery and its connections to generative AI, foundation models, and general robot learning.

- [2025.06] Discovering Temporal Structure: An Overview of Hierarchical Reinforcement Learning [[paper](https://arxiv.org/abs/2506.14045)]
- [2025.03] Generative Artificial Intelligence in Robotic Manipulation: A Survey [[paper](https://arxiv.org/abs/2503.03464)]
- [2024.04] What Foundation Models Can Bring for Robot Learning in Manipulation: A Survey [[paper](https://journals.sagepub.com/doi/abs/10.1177/02783649251390579)]

## 2. Unsupervised Robotic Skill Discovery

Methods that autonomously learn diverse behavioral repertoires without task-specific rewards, demonstrations, or manually defined skills.

- [2026.02] Diverse Skill Discovery for Quadruped Robots via Unsupervised Learning [[paper](https://arxiv.org/abs/2602.09767)]
- [2026.01] Group-Invariant Unsupervised Skill Discovery: Symmetry-aware Skill Representations for Generalizable Behavior [[paper](https://arxiv.org/abs/2601.14000)]
- [2025.11] Periodic Skill Discovery [[paper](https://arxiv.org/abs/2511.03187)] [[project](https://jonghaepark.github.io/psd/)]
- [2025.08] Divide, Discover, Deploy: Factorized Skill Learning with Symmetry and Style Priors [[paper](https://arxiv.org/abs/2508.19953)]
- [2025.08] From Tabula Rasa to Emergent Abilities: Discovering Robot Skills via Real-World Unsupervised Quality-Diversity [[paper](https://arxiv.org/abs/2508.19172)] [[project](https://adaptive-intelligent-robotics.github.io/URSA/)]
- [2025.08] Unsupervised Skill Discovery as Exploration for Learning Agile Locomotion [[paper](https://arxiv.org/abs/2508.08982)]
- [2025.06] SLAC: Safe and Efficient Real-Robot Reinforcement Learning via Unsupervised Simulation Pre-Training [[paper](https://arxiv.org/abs/2506.04147)] [[project](https://robo-rl.github.io/)]
- [2024.10] Constrained Skill Discovery: Quadruped Locomotion with Unsupervised Reinforcement Learning [[paper](https://arxiv.org/abs/2410.07877)]
- [2023.10] Learning to Discover Skills through Guidance (DISCO-DANCE) [[paper](https://arxiv.org/abs/2310.20178)] [[project](https://mynsng.github.io/discodance)]
- [2023.10] METRA: Scalable Unsupervised RL with Metric-Aware Abstraction [[paper](https://arxiv.org/abs/2310.08887)] [[project](https://seohong.me/projects/metra/)]
- [2023.09] Balancing State Exploration and Skill Diversity in Unsupervised Skill Discovery (ComSD) [[paper](https://arxiv.org/abs/2309.17203)]
- [2023.07] Variational Curriculum Reinforcement Learning for Unsupervised Discovery of Skills [[paper](https://arxiv.org/abs/2310.19424)]
- [2023.05] Behavior Contrastive Learning for Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/2305.04477)]
- [2023.05] Safety-Aware Unsupervised Skill Discovery [[paper](https://safe-skill.github.io/static/pdfs/safe-skill.pdf)] [[project](https://safe-skill.github.io/)]
- [2023.02] Controllability-Aware Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/2302.05103)] [[project](https://seohong.me/projects/csd/)]
- [2022.09] Unsupervised Skill Discovery via Recurrent Skill Training [[paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/ff6b031d5bdc552b795175a0f3b35a50-Abstract-Conference.html)]
- [2022.04] Unsupervised Reinforcement Learning for Transferable Manipulation Skill Discovery [[paper](https://arxiv.org/abs/2204.13906)]
- [2022.02] CIC: Contrastive Intrinsic Control for Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/2202.00161)]
- [2022.02] Lipschitz-Constrained Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/2202.00914)]
- [2021.10] Direct then Diffuse: Incremental Unsupervised Skill Discovery for State Covering and Goal Reaching [[paper](https://arxiv.org/abs/2110.14457)]
- [2021.08] APS: Active Pretraining with Successor Features [[paper](https://arxiv.org/abs/2108.13956)]
- [2021.07] Learning More Skills through Optimistic Exploration [[paper](https://arxiv.org/abs/2107.14226)]
- [2021.07] Skill Discovery for Exploration and Planning Using Deep Skill Graphs [[paper](https://proceedings.mlr.press/v139/bagaria21a.html)]
- [2021.06] Unsupervised Skill Discovery with Bottleneck Option Learning [[paper](https://arxiv.org/abs/2106.14305)]
- [2021.03] Mutual Information State Intrinsic Control [[paper](https://arxiv.org/abs/2103.08107)]
- [2020.12] Relative Variational Intrinsic Control [[paper](https://arxiv.org/abs/2012.07827)]
- [2020.06] ELSIM: End-to-End Learning of Reusable Skills through Intrinsic Motivation [[paper](https://arxiv.org/abs/2006.12903)]
- [2020.04] Emergent Real-World Robotic Skills via Unsupervised Off-Policy Reinforcement Learning [[paper](https://arxiv.org/abs/2004.12974)]
- [2020.02] Explore, Discover and Learn: Unsupervised Discovery of State-Covering Skills [[paper](https://arxiv.org/abs/2002.03647)]
- [2019.07] Dynamical Distance Learning for Semi-Supervised and Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/1907.08225)]
- [2019.07] Dynamics-Aware Unsupervised Discovery of Skills [[paper](https://arxiv.org/abs/1907.01657)]
- [2019.05] Autonomous Skill Discovery with Quality-Diversity and Unsupervised Descriptors [[paper](https://dl.acm.org/doi/abs/10.1145/3321707.3321804)]
- [2018.07] Variational Option Discovery Algorithms [[paper](https://arxiv.org/abs/1807.10299)]
- [2018.03] Unsupervised Learning of Goal Spaces for Intrinsically Motivated Goal Exploration [[paper](https://arxiv.org/abs/1803.00781)]
- [2018.02] Diversity Is All You Need: Learning Skills without a Reward Function [[paper](https://arxiv.org/abs/1802.06070)]
- [2017.10] Eigenoption Discovery through the Deep Successor Representation [[paper](https://arxiv.org/abs/1710.11089)]
- [2017.03] A Laplacian Framework for Option Discovery in Reinforcement Learning [[paper](https://arxiv.org/abs/1703.00956)]
- [2017.03] Multi-Level Discovery of Deep Options [[paper](https://arxiv.org/abs/1703.08294)]
- [2016.11] Variational Intrinsic Control [[paper](https://arxiv.org/abs/1611.07507)]

## 3. Guided and Agentic Robotic Skill Discovery

Methods that use language models, semantic guidance, or autonomous agents to propose, learn, and expand meaningful robot skills.

- [2026.08] RoboReact: Agentic Skill Distillation from Generated Egocentric Videos for Generalizable Whole-Body Manipulation [[paper](https://arxiv.org/abs/2608.03387)]
- [2026.06] ASPIRE: Agentic Skills Discovery for Robotics [[paper](https://arxiv.org/abs/2607.00272)]
- [2026.06] COLLIE: Guiding Skill Discovery in Semantically Coherent Latent Space [[paper](https://arxiv.org/abs/2606.00950)]
- [2026.06] Continual Quadruped Robots Coordination via Semantic Skill Discovery [[paper](https://arxiv.org/abs/2606.08102)] [[project](https://conquer-project.pages.dev/)]
- [2026.04] Leveraging Human Feedback for Semantically-Relevant Skill Discovery [[paper](https://arxiv.org/abs/2604.24127)]
- [2025.10] Guiding Skill Discovery with Foundation Models [[paper](https://arxiv.org/abs/2510.23167)]
- [2025.10] Reference Grounded Skill Discovery [[paper](https://arxiv.org/abs/2510.06203)]
- [2025.05] Real-Time Verification of Embodied Reasoning for Generative Skill Acquisition [[paper](https://arxiv.org/abs/2505.11175)]
- [2024.06] Do's and Don'ts: Learning Desirable Skills with Instruction Videos [[paper](https://arxiv.org/abs/2406.00324)]
- [2024.06] Language Guided Skill Discovery [[paper](https://proceedings.iclr.cc/paper_files/paper/2025/hash/dae30ba63ca043588cdf804bbba295ed-Abstract-Conference.html)]
- [2024.05] Agentic Skill Discovery [[paper](https://www.sciencedirect.com/science/article/pii/S0921889025003458)] [[project](https://agentic-skill-discovery.github.io/)] [[code](https://github.com/xf-zhao/Agentic-Skill-Discovery)]
- [2024.03] ARO: Large Language Model Supervised Robotics Text2Skill Autonomous Learning [[paper](https://arxiv.org/abs/2403.15834)]
- [2023.10] Bootstrap Your Own Skills: Learning to Solve New Tasks with Large Language Model Guidance [[paper](https://arxiv.org/abs/2310.10021)]
- [2023.07] Scaling Up and Distilling Down: Language-Guided Robot Skill Acquisition [[paper](https://arxiv.org/abs/2307.14535)]
- [2022.11] Robotic Skill Acquisition via Instruction Augmentation with Vision-Language Models [[paper](https://arxiv.org/abs/2211.11736)]
- [2019.12] Option Discovery Using Deep Skill Chaining [[paper](https://openreview.net/forum?id=B1gqipNYwH)] [[code](https://github.com/deep-skill-chaining/deep-skill-chaining)]
- [2011.08] Autonomous Skill Acquisition on a Mobile Manipulator [[paper](https://doi.org/10.1609/AAAI.V25I1.7982)]
- [2009.12] Skill Discovery in Continuous Reinforcement Learning Domains Using Skill Chaining [[paper](https://proceedings.neurips.cc/paper/2009/hash/e0cf1f47118daebc5b16269099ad7347-Abstract.html)]

## 4. Robotic Skill Discovery from Demonstrations and Trajectories

Methods that identify reusable skills, skill boundaries, or shared representations from unlabeled demonstrations and interaction trajectories.

- [2026.08] GORDON: Graph-based Object-centric Rewards for Decomposition of Long-Horizon Manipulation [[paper](https://arxiv.org/abs/2608.03753)]
- [2026.06] Learning Multi-Task Robot Trajectory Segmentation from Visual and Kinematic Streams (RoboSegNet) [[paper](https://openaccess.thecvf.com/content/CVPR2026F/papers/Chen_Learning_Multi-Task_Robot_Trajectory_Segmentation_from_Visual_and_Kinematic_Streams_CVPRF_2026_paper.pdf)] [[project](https://berkeleyautomation.github.io/RoboSegNet/)] [[code](https://github.com/KeplerC/RoboSegNet)]
- [2026.02] RoboSubtaskNet: Temporal Sub-task Segmentation for Human-to-Robot Skill Transfer in Real-World Environments [[paper](https://arxiv.org/abs/2602.10015)]
- [2025.10] Learning Parameterized Skills from Demonstrations (DEPS) [[paper](https://arxiv.org/abs/2510.24095)]
- [2025.10] RDD: Retrieval-Based Demonstration Decomposer for Planner Alignment in Long-Horizon Tasks [[paper](https://arxiv.org/abs/2510.14968)] [[project](https://rdd-neurips.github.io/)] [[code](https://github.com/tasl-lab/Retrieval-Demonstration-Decomposer)]
- [2025.10] SymSkill: Symbol and Skill Co-Invention for Data-Efficient and Reactive Long-Horizon Manipulation [[paper](https://arxiv.org/abs/2510.01661)] [[project](https://symskill.github.io/)]
- [2025.08] LodeStar: Long-horizon Dexterity via Synthetic Data Augmentation from Human Demonstrations [[paper](https://arxiv.org/abs/2508.17547)] [[project](https://lodestar-robot.github.io/)]
- [2025.05] UniSkill: Imitating Human Videos via Cross-Embodiment Skill Representations [[paper](https://arxiv.org/abs/2505.08787)] [[project](https://kimhanjung.github.io/UniSkill/)]
- [2025.04] Modality Selection and Skill Segmentation via Cross-Modality Attention [[paper](https://arxiv.org/abs/2504.14573)]
- [2025.02] Data Augmentation for Instruction Following Policies via Trajectory Segmentation [[paper](https://arxiv.org/abs/2503.01871)] [[project](https://nikehop.github.io/play_segmentation/)] [[code](https://github.com/NikeHop/PlaySegmentation-AAAI2025)]
- [2025.01] NBDI: A Simple and Effective Termination Condition for Skill Extraction from Task-Agnostic Demonstrations [[paper](https://arxiv.org/abs/2501.12668)]
- [2025.01] Robust Segmentation and Classification of Robot Skills from Demonstrations with Detection of Unknown Skills [[paper](https://doi.org/10.1016/j.procs.2025.01.215)]
- [2024.03] A Demonstration Trajectory Segmentation Approach for Wheelchair-Mounted Assistive Robots [[paper](https://doi.org/10.1049/cit2.12358)]
- [2023.11] LOTUS: Continual Imitation Learning for Robot Manipulation through Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/2311.02058)] [[project](https://ut-austin-rpl.github.io/Lotus/)]
- [2023.07] XSkill: Cross Embodiment Skill Discovery [[paper](https://proceedings.mlr.press/v229/xu23a.html)]
- [2022.02] Bayesian Nonparametrics for Offline Skill Discovery [[paper](https://arxiv.org/abs/2202.04675)] [[code](https://github.com/layer6ai-labs/BNPO)]
- [2021.09] Bottom-Up Skill Discovery from Unsegmented Demonstrations for Long-Horizon Robot Manipulation [[paper](https://arxiv.org/abs/2109.13841)]
- [2021.03] SkiD RAW: Skill Discovery from Raw Trajectories [[paper](https://ieeexplore.ieee.org/abstract/document/9387162)]
- [2019.03] Learning Latent Plans from Play [[paper](https://arxiv.org/abs/1903.01973)]
- [2018.12] CompILE: Compositional Imitation Learning and Execution [[paper](https://arxiv.org/abs/1812.01483)]
- [2017.11] Transition State Clustering: Unsupervised Surgical Trajectory Segmentation for Robot Learning [[paper](https://doi.org/10.1177/0278364917743319)]
- [2015.09] Nonparametric Bayesian Reward Segmentation for Skill Discovery Using Inverse Reinforcement Learning [[paper](https://doi.org/10.1109/IROS.2015.7353414)]
- [2010.12] Constructing Skill Trees for Reinforcement Learning Agents from Demonstration Trajectories [[paper](https://proceedings.neurips.cc/paper/2010/hash/27ed0fb950b856b06e1273989422e7d3-Abstract.html)]

## 5. Automatic Task Generation for Open-Ended Robotic Skill Acquisition

Methods that automatically propose tasks, goals, simulation programs, or training objectives, then acquire the robot skills needed to solve them. Unlike unsupervised skill discovery, these methods are task-first and use generated supervision.

- [2026.07] AXIS: A Growable Community-Driven Data Engine for Scalable Robot Manipulation [[paper](https://arxiv.org/abs/2607.21588)] [[project](https://axisaiorg.github.io/AXIS-V1/)]
- [2026.07] RoboSnap: One-Shot Real-to-Sim Scene Generation for Generalizable Robot Learning and Evaluation [[paper](https://arxiv.org/abs/2607.06699)] [[project](https://robosnap.github.io/)]
- [2026.06] SAGE: Scalable Agentic 3D Scene Generation for Embodied AI [[paper](https://arxiv.org/abs/2602.10116)] [[project](https://research.nvidia.com/labs/dir/sage/)]
- [2026.04] RoboLab: A High-Fidelity Simulation Benchmark for Analysis of Task Generalist Policies [[paper](https://arxiv.org/abs/2604.09860)] [[project](https://research.nvidia.com/labs/srl/projects/robolab/)] [[code](https://github.com/NVLabs/RoboLab)]
- [2026.03] FATE: Closed-Loop Feasibility-Aware Task Generation with Active Repair for Physically Grounded Robotic Curricula [[paper](https://arxiv.org/abs/2603.01505)]
- [2026.02] Affordance-Graphed Task Worlds: Self-Evolving Task Generation for Scalable Embodied Learning [[paper](https://arxiv.org/abs/2602.12065)]
- [2026.02] Automatic Cognitive Task Generation for In-Situ Evaluation of Embodied Agents [[paper](https://arxiv.org/abs/2602.05249)]
- [2026.02] RoboGene: Boosting VLA Pre-training via Diversity-Driven Agentic Framework for Real-World Task Generation [[paper](https://arxiv.org/abs/2602.16444)] [[project](https://robogene-boost-vla.github.io/)]
- [2025.12] AnyTask: An Automated Task and Data Generation Framework for Advancing Sim-to-Real Policy Learning [[paper](https://arxiv.org/abs/2512.17853)] [[project](https://anytask.rai-inst.com/)]
- [2025.11] ForeRobo: Unlocking Infinite Simulation Data for 3D Goal-driven Robotic Manipulation [[paper](https://arxiv.org/abs/2511.04381)]
- [2025.11] Human-Centric Open-Future Task Discovery: Formulation, Benchmark, and Scalable Tree-Based Search [[paper](https://arxiv.org/abs/2511.18929)]
- [2025.09] MesaTask: Towards Task-Driven Tabletop Scene Generation via 3D Spatial Reasoning [[paper](https://arxiv.org/abs/2509.22281)] [[project](https://mesatask.github.io/)]
- [2025.05] ManiTaskGen: A Comprehensive Task Generator for Benchmarking and Improving Vision-Language Agents on Embodied Decision-Making [[paper](https://arxiv.org/abs/2505.20726)] [[project](https://manitaskgen.github.io/)]
- [2025.05] Steerable Scene Generation with Post Training and Inference-Time Search [[paper](https://arxiv.org/abs/2505.04831)] [[project](https://steerable-scene-generation.github.io/)]
- [2025.02] Video2Policy: Scaling up Manipulation Tasks in Simulation through Internet Videos [[paper](https://arxiv.org/abs/2502.09886)]
- [2024.11] Eurekaverse: Environment Curriculum Generation via Large Language Models [[paper](https://arxiv.org/abs/2411.01775)]
- [2024.10] GenSim2: Scaling Robot Data Generation with Multi-Modal and Reasoning LLMs [[paper](https://arxiv.org/abs/2410.03645)] [[project](https://gensim2.github.io/)] [[code](https://github.com/GenSim2/GenSim2)]
- [2024.10] GRS: Generating Robotic Simulation Tasks from Real-World Images [[paper](https://arxiv.org/abs/2410.15536)]
- [2024.10] PARTNR: A Benchmark for Planning and Reasoning in Embodied Multi-Agent Tasks [[paper](https://arxiv.org/abs/2411.00081)] [[code](https://github.com/facebookresearch/partnr-planner)]
- [2024.10] Unsupervised Skill Discovery for Robotic Manipulation through Automatic Task Generation [[paper](https://arxiv.org/abs/2410.04855)]
- [2024.09] CurricuLLM: Automatic Task Curricula Design for Learning Complex Robot Skills Using Large Language Models [[paper](https://arxiv.org/abs/2409.18382)] [[project](https://iconlab.negarmehr.com/CurricuLLM/)]
- [2023.11] RoboGen: Towards Unleashing Infinite Data for Automated Robot Learning via Generative Simulation [[paper](https://arxiv.org/abs/2311.01455)]
- [2023.10] Gen2Sim: Scaling Up Robot Learning in Simulation with Generative Models [[paper](https://arxiv.org/abs/2310.18308)]
- [2023.10] GenSim: Generating Robotic Simulation Tasks via Large Language Models [[paper](https://arxiv.org/abs/2310.01361)] [[project](https://gen-sim.github.io/)] [[code](https://github.com/liruiw/GenSim)]
- [2022.11] Active Task Randomization: Learning Robust Skills via Unsupervised Generation of Diverse and Feasible Tasks [[paper](https://arxiv.org/abs/2211.06134)]
- [2021.06] Discovering Generalizable Skills via Automated Generation of Diverse Tasks [[paper](https://arxiv.org/abs/2106.13935)]

## 6. Deployment of Discovered Robotic Skills

Methods that convert discovered or segmented trajectories into executable skill units, scale their valid operating conditions, compose them into long-horizon behaviors, and verify their deployment across objects, scenes, embodiments, and physical environments.

- [2026.07] Robots Acquire Manipulation Skills in Seconds from a Single Human Video (HOST) [[paper](https://arxiv.org/abs/2607.20033)]
- [2026.06] An Embodied Simulation Platform, Benchmark, and Success-Verified Simulation Augmentation Framework for Wet-Lab Robotics (Pipette) [[paper](https://arxiv.org/abs/2606.12936)]
- [2026.06] VOLT: Vision and Language Trajectory Segmentation for Faster-than-Demonstration Policies [[paper](https://arxiv.org/abs/2606.06323)]
- [2026.05] From Reaction to Anticipation: Proactive Failure Recovery through Agentic Task Graph for Robotic Manipulation (AgentChord) [[paper](https://arxiv.org/abs/2605.11951)] [[project](https://shengxu.net/AgentChord/)] [[code](https://github.com/EDEM-AI/AgentChord)]
- [2026.04] AffordGen: Generating Diverse Demonstrations for Generalizable Object Manipulation with Affordance Correspondence [[paper](https://arxiv.org/abs/2604.10579)]
- [2026.04] AffordSim: A Scalable Data Generator and Benchmark for Affordance-Aware Robotic Manipulation [[paper](https://arxiv.org/abs/2604.11674)]
- [2026.03] MolmoB0T: Large-Scale Simulation Enables Zero-Shot Manipulation [[paper](https://arxiv.org/abs/2603.16861)] [[project](https://allenai.github.io/MolmoBot/)]
- [2025.12] IGen: Scalable Data Generation for Robot Learning from Open-World Images [[paper](https://arxiv.org/abs/2512.01773)]
- [2025.11] SkillWrapper: Generative Predicate Invention for Task-Level Robot Planning [[paper](https://arxiv.org/abs/2511.18203)]
- [2025.09] Annotation-Free One-Shot Imitation Learning for Multi-Step Manipulation Tasks [[paper](https://arxiv.org/abs/2509.24972)] [[code](https://github.com/vijja-w/AF-OSIL-MS)]
- [2025.09] VLBiMan: Vision-Language Anchored One-Shot Demonstration Enables Generalizable Bimanual Robotic Manipulation [[paper](https://arxiv.org/abs/2509.21723)] [[project](https://hnuzhy.github.io/projects/VLBiMan/)]
- [2025.09] TReF-6: Inferring Task-Relevant Frames from a Single Demonstration for One-Shot Skill Generalization [[paper](https://arxiv.org/abs/2509.00310)]
- [2025.06] RoboTwin 2.0: A Scalable Data Generator and Benchmark with Strong Domain Randomization for Robust Bimanual Robotic Manipulation [[paper](https://arxiv.org/abs/2506.18088)] [[project](https://robotwin-platform.github.io/doc/index.html)]
- [2025.06] DynScene: Scalable Generation of Dynamic Robotic Manipulation Scenes for Embodied AI [[paper](https://openaccess.thecvf.com/content/CVPR2025/html/Lee_DynScene_Scalable_Generation_of_Dynamic_Robotic_Manipulation_Scenes_for_Embodied_CVPR_2025_paper.html)]
- [2025.06] RoboCerebra: A Large-Scale Benchmark for Long-Horizon Robotic Manipulation Evaluation [[paper](https://arxiv.org/abs/2506.06677)] [[project](https://robocerebra.github.io/)]
- [2025.05] DexScale: Automating Data Scaling for Sim2Real Generalizable Robot Control [[paper](https://proceedings.mlr.press/v267/liu25k.html)] [[project](https://edem-ai.github.io/dexscale.github.io/)]
- [2025.05] DreamGen: Unlocking Generalization in Robot Learning through Video World Models [[paper](https://arxiv.org/abs/2505.12705)]
- [2025.02] DemoGen: Synthetic Demonstration Generation for Data-Efficient Visuomotor Policy Learning [[paper](https://arxiv.org/abs/2502.16932)] [[project](https://demo-generation.github.io/)]
- [2024.10] DexMimicGen: Automated Data Generation for Bimanual Dexterous Manipulation via Imitation Learning [[paper](https://arxiv.org/abs/2410.24185)]
- [2024.10] SDS: See It, Do It, Sorted: Quadruped Skill Synthesis from Single Video Demonstration [[paper](https://arxiv.org/abs/2410.11571)] [[project](https://rpl-cs-ucl.github.io/SDSweb)]
- [2024.10] SkillMimicGen: Automated Demonstration Generation for Efficient Skill Learning and Deployment [[paper](https://arxiv.org/abs/2410.18907)] [[project](https://skillgen.github.io/)]
- [2024.01] Generative Skill Chaining: Long-Horizon Skill Planning with Diffusion Models [[paper](https://arxiv.org/abs/2401.03360)] [[project](https://generative-skill-chaining.github.io/)]
- [2022.03] DiffSkill: Skill Abstraction from Differentiable Physics for Deformable Object Manipulations with Tools [[paper](https://arxiv.org/abs/2203.17275)]
- [2021.07] Hierarchical Few-Shot Imitation with Skill Transition Models [[paper](https://arxiv.org/abs/2107.08981)]
- [2021.06] The Option Keyboard: Combining Skills in Reinforcement Learning [[paper](https://arxiv.org/abs/2106.13105)]
- [2020.12] Reset-Free Lifelong Learning with Skill-Space Planning [[paper](https://arxiv.org/abs/2012.03548)]
- [2020.10] OPAL: Offline Primitive Discovery for Accelerating Offline Reinforcement Learning [[paper](https://arxiv.org/abs/2010.13611)]
- [2018.10] One-Shot Hierarchical Imitation Learning of Compound Visuomotor Tasks [[paper](https://arxiv.org/abs/1810.11043)]
