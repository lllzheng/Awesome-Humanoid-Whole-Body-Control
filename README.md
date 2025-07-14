# Awesome-Humanoid-Whole-Body-Control
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)

**Foreword**
This compilation provides a rigorously curated survey of state-of-the-art literature, toolkits, and datasets in the domain of humanoid robot learning. It is maintained as a living document and we welcome community-driven enhancements via pull requests. The markdown document primarily includes papers, titles, project websites, code and datasets, abstract summaries, algorithmic system frameworks, and the author's affiliation (only displaying the first author's affiliation).

---

## Loco-Manipulation and Whole-Body-Control


|   arXiv   |   Title   |   Website |   Code & Dataset    |   Summarize   |   Overview   | Organization |
| --------- | --------- | --------- | --------- | ------------- | --------- | --------- |
| [arXiv 2025.07](https://arxiv.org/abs/2507.07356) | UniTracker: Learning Universal Whole-Body Motion Tracker for Humanoid Robots             | [UniTracker](https://yinkangning0124.github.io/Humanoid-UniTracker/) | - | UniTracker提出在师生框架中引入条件变分自编码器（CVAE），以显式建模并保留教师策略的丰富动作多样性，相比仅用 MLP-DAgger 蒸馏的传统方法，单一学生策略即可泛化跟踪更多样、更未见过的全身参考动作，仿真与实物实验显示其在多样运动类型与未知动作上均显著优于现有基线。 | ![UniTracker](./Assets/images/UniTracker.png) | Shanghai Jiao Tong University |
| [arXiv 2025.07](https://arxiv.org/abs/2507.06905) | ULC: A Unified and Fine-Grained Controller for Humanoid Loco-Manipulation | [ULC](https://ulc-humanoid.github.io) | Coming Soon| ULC提出统一人形机器人移动-操作控制器 ULC，用单一端到端策略同时跟踪根速度/高度、躯干姿态与双臂关节，通过序列技能递增、残差动作建模、指令多项式插值、随机延迟释放、负载随机化与质心跟踪六大技术实现高精度、大工作空间与鲁棒性，Unitree G1 实测较分层基线显著提升跟踪精度并能在负重扰动下完成复杂全身协调任务。 | ![ULC](./Assets/images/ULC.png) | Harbin Institute of Technology |
| [arXiv 2025.06](https://arxiv.org/abs/2506.12851) | KungfuBot: Physics-Based Humanoid Whole-Body
Control for Learning Highly-Dynamic Skills | [KungfuBot](https://kungfu-bot.github.io/) | [🖥️](https://github.com/TeleHuman/PBHC)| KungfuBot提出“多步运动处理+自适应跟踪容忍度的双层优化”框架，用非对称演员-评论家策略在物理约束内高效模仿高动态功夫/舞蹈动作。在运动处理方面，设计了一个流程来提取、过滤、校正和重新定位运动，同时最大程度地确保符合物理约束；在运动模仿方面，构建了一个双层优化问题，根据当前跟踪误差动态调整跟踪精度容差，从而创建了一种自适应课程机制。相较现有方法显著降低跟踪误差并成功部署于Unitree G1，实现稳定且富表现力的全身控制。 | ![KungfuBot](./Assets/images/KungfuBot.png) | 中国电信人工智能研究院(TeleAI) |
| [arXiv 2025.06](https://arxiv.org/abs/2506.13751) | LeVERB: Humanoid Whole-Body Control with Latent Vision-Language Instruction | [LeVERB](https://ember-lab-berkeley.github.io/LeVERB-Website/)   | Coming Soon & [🤗](https://huggingface.co/datasets/ember-lab-berkeley/LeVERB-Bench-Dataset) | LeVERB 首次提出“高层视觉-语言策略自训潜在动作词汇 + 底层 RL-WBC 策略解码”的分层框架，打破以往依赖手工低层动作词汇的局限，在首创的 150 项人形全身控制基准中实现 58.5% 零样本成功率，较朴素 VLA 提升 7.8 倍，并支持动态奔跑等敏捷行为。 | ![LeVERB](./Assets/images/LeVERB.png) | University of California Berkeley | 
| [arXiv 2025.05](https://arxiv.org/abs/2505.06776) | FALCON: Learning Force-Adaptive Humanoid Loco-Manipulation | [FALCON](https://lecar-lab.github.io/falcon-humanoid/) | [🖥️](https://github.com/LeCAR-Lab/FALCON/) | FALCON 用“下肢稳态行走 + 上肢隐式力补偿”双智能体强化学习框架，在渐进式外力课程中联合训练，无需针对机器人结构调参即可在多台人形机器人上零样本部署，实现搬运 0–20 N、推车 0–100 N、开门 0–40 N 等真实任务，关节跟踪精度较基线提升 2 倍并保持鲁棒行走。 | ![FALCON](./Assets/images/FALCON.png) | Carnegie Mellon University |
