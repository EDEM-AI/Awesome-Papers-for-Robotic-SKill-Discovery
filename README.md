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
- [2025.08] Unsupervised Skill Discovery as Exploration for Learning Agile Locomotion [[paper](https://arxiv.org/abs/2508.08982)]
- [2023.10] METRA: Scalable Unsupervised RL with Metric-Aware Abstraction [[paper](https://arxiv.org/abs/2310.08887)] [[project](https://seohong.me/projects/metra/)]
- [2023.10] Learning to Discover Skills through Guidance (DISCO-DANCE) [[paper](https://arxiv.org/abs/2310.20178)] [[project](https://mynsng.github.io/discodance)]
- [2023.07] Variational Curriculum Reinforcement Learning for Unsupervised Discovery of Skills [[paper](https://arxiv.org/abs/2310.19424)]
- [2023.05] Safety-Aware Unsupervised Skill Discovery [[paper](https://safe-skill.github.io/static/pdfs/safe-skill.pdf)] [[project](https://safe-skill.github.io/)]
- [2023.05] Behavior Contrastive Learning for Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/2305.04477)]
- [2023.02] Controllability-Aware Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/2302.05103)] [[project](https://seohong.me/projects/csd/)]
- [2022.09] Unsupervised Skill Discovery via Recurrent Skill Training [[paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/ff6b031d5bdc552b795175a0f3b35a50-Abstract-Conference.html)]
- [2022.02] Lipschitz-Constrained Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/2202.00914)]
- [2022.02] CIC: Contrastive Intrinsic Control for Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/2202.00161)]
- [2021.10] Direct then Diffuse: Incremental Unsupervised Skill Discovery for State Covering and Goal Reaching [[paper](https://arxiv.org/abs/2110.14457)]
- [2021.08] APS: Active Pretraining with Successor Features [[paper](https://arxiv.org/abs/2108.13956)]
- [2021.06] Unsupervised Skill Discovery with Bottleneck Option Learning [[paper](https://arxiv.org/abs/2106.14305)]
- [2020.12] Relative Variational Intrinsic Control [[paper](https://arxiv.org/abs/2012.07827)]
- [2020.04] Emergent Real-World Robotic Skills via Unsupervised Off-Policy Reinforcement Learning [[paper](https://arxiv.org/abs/2004.12974)]
- [2020.02] Explore, Discover and Learn: Unsupervised Discovery of State-Covering Skills [[paper](https://arxiv.org/abs/2002.03647)]
- [2019.07] Dynamics-Aware Unsupervised Discovery of Skills [[paper](https://arxiv.org/abs/1907.01657)]
- [2019.07] Dynamical Distance Learning for Semi-Supervised and Unsupervised Skill Discovery [[paper](https://arxiv.org/abs/1907.08225)]
- [2019.05] Autonomous Skill Discovery with Quality-Diversity and Unsupervised Descriptors [[paper](https://dl.acm.org/doi/abs/10.1145/3321707.3321804)]
- [2018.07] Variational Option Discovery Algorithms [[paper](https://arxiv.org/abs/1807.10299)]
- [2018.02] Diversity Is All You Need: Learning Skills without a Reward Function [[paper](https://arxiv.org/abs/1802.06070)]
- [2017.10] Eigenoption Discovery through the Deep Successor Representation [[paper](https://arxiv.org/abs/1710.11089)]
- [2016.11] Variational Intrinsic Control [[paper](https://arxiv.org/abs/1611.07507)]

## 3. Guided and Agentic Robotic Skill Discovery

Methods that use language models, semantic guidance, or autonomous agents to propose, learn, and expand meaningful robot skills.

- [2026.06] ASPIRE: Agentic Skills Discovery for Robotics [[paper](https://arxiv.org/abs/2607.00272)]
- [2026.04] Leveraging Human Feedback for Semantically-Relevant Skill Discovery [[paper](https://arxiv.org/abs/2604.24127)]
- [2025.05] Real-Time Verification of Embodied Reasoning for Generative Skill Acquisition [[paper](https://arxiv.org/abs/2505.11175)]
- [2024.06] Language Guided Skill Discovery [[paper](https://proceedings.iclr.cc/paper_files/paper/2025/hash/dae30ba63ca043588cdf804bbba295ed-Abstract-Conference.html)]
- [2024.05] Agentic Skill Discovery [[paper](https://www.sciencedirect.com/science/article/pii/S0921889025003458)] [[project](https://agentic-skill-discovery.github.io/)] [[code](https://github.com/xf-zhao/Agentic-Skill-Discovery)]
- [2024.03] ARO: Large Language Model Supervised Robotics Text2Skill Autonomous Learning [[paper](https://arxiv.org/abs/2403.15834)]

## 4. Robotic Skill Discovery from Demonstrations and Trajectories

Methods that identify reusable skills, skill boundaries, or shared representations from unlabeled demonstrations and interaction trajectories.

- [2023.07] XSkill: Cross Embodiment Skill Discovery [[paper](https://proceedings.mlr.press/v229/xu23a.html)]
- [2022.02] Bayesian Nonparametrics for Offline Skill Discovery [[paper](https://arxiv.org/abs/2202.04675)] [[code](https://github.com/layer6ai-labs/BNPO)]
- [2021.09] Bottom-Up Skill Discovery from Unsegmented Demonstrations for Long-Horizon Robot Manipulation [[paper](https://arxiv.org/abs/2109.13841)]
- [2021.03] SkiD RAW: Skill Discovery from Raw Trajectories [[paper](https://ieeexplore.ieee.org/abstract/document/9387162)]
- [2019.03] Learning Latent Plans from Play [[paper](https://arxiv.org/abs/1903.01973)]
- [2018.12] CompILE: Compositional Imitation Learning and Execution [[paper](https://arxiv.org/abs/1812.01483)]

## 5. Automatic Task Generation for Open-Ended Robotic Skill Acquisition

Methods that automatically propose tasks, goals, simulation programs, or training objectives, then acquire the robot skills needed to solve them. Unlike unsupervised skill discovery, these methods are task-first and use generated supervision.

- [2026.07] AXIS: A Growable Community-Driven Data Engine for Scalable Robot Manipulation [[paper](https://arxiv.org/abs/2607.21588)] [[project](https://axisaiorg.github.io/AXIS-V1/)]
- [2026.03] FATE: Closed-Loop Feasibility-Aware Task Generation with Active Repair for Physically Grounded Robotic Curricula [[paper](https://arxiv.org/abs/2603.01505)]
- [2026.02] RoboGene: Boosting VLA Pre-training via Diversity-Driven Agentic Framework for Real-World Task Generation [[paper](https://arxiv.org/abs/2602.16444)] [[project](https://robogene-boost-vla.github.io/)]
- [2026.02] Affordance-Graphed Task Worlds: Self-Evolving Task Generation for Scalable Embodied Learning [[paper](https://arxiv.org/abs/2602.12065)]
- [2025.12] AnyTask: An Automated Task and Data Generation Framework for Advancing Sim-to-Real Policy Learning [[paper](https://arxiv.org/abs/2512.17853)] [[project](https://anytask.rai-inst.com/)]
- [2025.11] Human-Centric Open-Future Task Discovery: Formulation, Benchmark, and Scalable Tree-Based Search [[paper](https://arxiv.org/abs/2511.18929)]
- [2024.11] Eurekaverse: Environment Curriculum Generation via Large Language Models [[paper](https://arxiv.org/abs/2411.01775)]
- [2024.10] Unsupervised Skill Discovery for Robotic Manipulation through Automatic Task Generation [[paper](https://arxiv.org/abs/2410.04855)]
- [2024.10] GenSim2: Scaling Robot Data Generation with Multi-Modal and Reasoning LLMs [[paper](https://arxiv.org/abs/2410.03645)] [[project](https://gensim2.github.io/)] [[code](https://github.com/GenSim2/GenSim2)]
- [2024.10] GRS: Generating Robotic Simulation Tasks from Real-World Images [[paper](https://arxiv.org/abs/2410.15536)]
- [2024.09] CurricuLLM: Automatic Task Curricula Design for Learning Complex Robot Skills Using Large Language Models [[paper](https://arxiv.org/abs/2409.18382)] [[project](https://iconlab.negarmehr.com/CurricuLLM/)]
- [2023.11] RoboGen: Towards Unleashing Infinite Data for Automated Robot Learning via Generative Simulation [[paper](https://arxiv.org/abs/2311.01455)]
- [2023.10] GenSim: Generating Robotic Simulation Tasks via Large Language Models [[paper](https://arxiv.org/abs/2310.01361)] [[project](https://gen-sim.github.io/)] [[code](https://github.com/liruiw/GenSim)]

## 6. Extraction, Composition, and Deployment of Discovered Robotic Skills

Methods that turn discovered or segmented behaviors into reusable skills that can be adapted, composed, and deployed on downstream tasks.

- [2025.11] SkillWrapper: Generative Predicate Invention for Task-Level Robot Planning [[paper](https://arxiv.org/abs/2511.18203)]
- [2025.05] DexScale: Automating Data Scaling for Sim2Real Generalizable Robot Control [[paper](https://proceedings.mlr.press/v267/liu25k.html)] [[project](https://edem-ai.github.io/dexscale.github.io/)]
- [2024.10] SkillMimicGen: Automated Demonstration Generation for Efficient Skill Learning and Deployment [[paper](https://arxiv.org/abs/2410.18907)] [[project](https://skillgen.github.io/)]
