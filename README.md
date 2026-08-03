# Awesome Papers for Robotic Skill Discovery

Papers that autonomously determine what robot skills or tasks should be learned, or automatically extract reusable robot skills from experience.

Paper entry format:

```markdown
- [YYYY.MM] PAPER TITLE [[paper](link)] [[project](link)] [[code](link)]
```

## 1. Surveys and Foundations of Robotic Skill Discovery

Surveys and foundational works that frame robotic skill discovery and its connections to generative AI, foundation models, and general robot learning.

- [2025.03] Generative Artificial Intelligence in Robotic Manipulation: A Survey [[paper](https://arxiv.org/abs/2503.03464)]
- [2024.04] What Foundation Models Can Bring for Robot Learning in Manipulation: A Survey [[paper](https://journals.sagepub.com/doi/abs/10.1177/02783649251390579)]

## 2. Unsupervised Robotic Skill Discovery

Methods that autonomously learn diverse behavioral repertoires without task-specific rewards, demonstrations, or manually defined skills.

- [2025.08] Unsupervised Skill Discovery as Exploration for Learning Agile Locomotion [[paper](https://arxiv.org/abs/2508.08982)]
- [2022.09] Unsupervised Skill Discovery via Recurrent Skill Training [[paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/ff6b031d5bdc552b795175a0f3b35a50-Abstract-Conference.html)]
- [2019.05] Autonomous Skill Discovery with Quality-Diversity and Unsupervised Descriptors [[paper](https://dl.acm.org/doi/abs/10.1145/3321707.3321804)]

## 3. Guided and Agentic Robotic Skill Discovery

Methods that use language models, semantic guidance, or autonomous agents to propose, learn, and expand meaningful robot skills.

- [2024.06] Language Guided Skill Discovery [[paper](https://proceedings.iclr.cc/paper_files/paper/2025/hash/dae30ba63ca043588cdf804bbba295ed-Abstract-Conference.html)]
- [2024.05] Agentic Skill Discovery [[paper](https://www.sciencedirect.com/science/article/pii/S0921889025003458)] [[project](https://agentic-skill-discovery.github.io/)] [[code](https://github.com/xf-zhao/Agentic-Skill-Discovery)]

## 4. Robotic Skill Discovery from Demonstrations and Trajectories

Methods that identify reusable skills, skill boundaries, or shared representations from unlabeled demonstrations and interaction trajectories.

- [2023.07] XSkill: Cross Embodiment Skill Discovery [[paper](https://proceedings.mlr.press/v229/xu23a.html)]
- [2021.03] SkiD RAW: Skill Discovery from Raw Trajectories [[paper](https://ieeexplore.ieee.org/abstract/document/9387162)]

## 5. Automatic Task Generation for Open-Ended Robotic Skill Acquisition

Methods that automatically propose tasks, goals, simulation programs, or training objectives, then acquire the robot skills needed to solve them. Unlike unsupervised skill discovery, these methods are task-first and use generated supervision.

- [2024.10] GenSim2: Scaling Robot Data Generation with Multi-Modal and Reasoning LLMs [[paper](https://arxiv.org/abs/2410.03645)] [[project](https://gensim2.github.io/)] [[code](https://github.com/GenSim2/GenSim2)]
- [2023.11] RoboGen: Towards Unleashing Infinite Data for Automated Robot Learning via Generative Simulation [[paper](https://arxiv.org/abs/2311.01455)]
- [2023.10] GenSim: Generating Robotic Simulation Tasks via Large Language Models [[paper](https://arxiv.org/abs/2310.01361)] [[project](https://gen-sim.github.io/)] [[code](https://github.com/liruiw/GenSim)]

## 6. Extraction, Composition, and Deployment of Discovered Robotic Skills

Methods that turn discovered or segmented behaviors into reusable skills that can be adapted, composed, and deployed on downstream tasks.

- [2025.05] DexScale: Automating Data Scaling for Sim2Real Generalizable Robot Control [[paper](https://proceedings.mlr.press/v267/liu25k.html)] [[project](https://edem-ai.github.io/dexscale.github.io/)]
- [2024.10] SkillMimicGen: Automated Demonstration Generation for Efficient Skill Learning and Deployment [[paper](https://arxiv.org/abs/2410.18907)] [[project](https://skillgen.github.io/)]
