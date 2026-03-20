# Awesome Humanoid WBC

Companion repository for the review paper **Learning-Based Whole-Body Control for Humanoid Robots: An Implementation-Centric Review**.

This repository curates papers, datasets, simulators, and open-source systems for learning-based whole-body control of humanoid robots. The list is organized for review writing and implementation reuse rather than for broad hype coverage: we emphasize locomotion, whole-body tracking, teleoperation, loco-manipulation, language-conditioned control, retargeting, and the infrastructure that makes those systems reproducible.

> Code links are included only when an official repository or project page is easy to verify.
>
> Year grouping follows the citation year in the seed bibliography.

Last updated: 2026-03-20

## Table of Contents

- [Recommended Starting Points](#recommended-starting-points)
- [2026](#2026)
- [2025](#2025)
- [2024](#2024)
- [2023](#2023)
- [2022 and Earlier](#2022-and-earlier)
- [Open-Source Frameworks](#open-source-frameworks)
- [Citation](#citation)

## Recommended Starting Points

- Real-World Humanoid Locomotion with Reinforcement Learning. Radosavovic et al. Science Robotics, 2024. [Paper](https://arxiv.org/abs/2303.03381) [Project](https://learning-humanoid-locomotion.github.io/)
- Learning Humanoid Locomotion with Perceptive Internal Model. Long et al. ICRA, 2025. [Paper](https://junfeng-long.github.io/PIM/)
- HOVER: Versatile Neural Whole-Body Controller for Humanoid Robots. He et al. ICRA, 2025. [Paper](https://arxiv.org/abs/2410.21229) [Project](https://hover-versatile-humanoid.github.io/)
- ExBody2: Advanced Expressive Humanoid Whole-Body Control. Ji et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2412.13196)
- OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning. He et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2406.08858) [Project](https://omni.human2humanoid.com/)
- BeyondMimic: From Motion Tracking to Versatile Humanoid Control via Guided Diffusion. Liao et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2508.08241)
- LangWBC: Language-directed Humanoid Whole-Body Control via End-to-end Learning. Shao et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2504.21738)
- HumanoidVerse: A Multi-Simulator Framework for Humanoid Robot Sim-to-Real Learning. CMU LeCAR Lab. GitHub repository, 2025. [Project](https://github.com/LeCAR-Lab/HumanoidVerse) [Code](https://github.com/LeCAR-Lab/HumanoidVerse)

## 2026

### Language-Conditioned and Foundation Models

- FRoM-W1: Towards General Humanoid Whole-Body Control with Language Instructions. Li et al. arXiv, 2026. [Paper](https://arxiv.org/abs/2601.12799)
- HumanX: Toward Agile and Generalizable Humanoid Interaction Skills from Human Videos. Wang et al. arXiv, 2026. [Paper](https://arxiv.org/abs/2602.02473)

### Locomotion and Whole-Body Control

- CLF-RL: Control Lyapunov Function Guided Reinforcement Learning. Li et al. RA-L, 2026. [Paper](https://www.zacholkin.com/research/clf_rl/)
- OmniXtreme: Breaking the Generality Barrier in High-Dynamic Humanoid Control. Wang et al. arXiv, 2026. [Paper](https://arxiv.org/abs/2602.23843)

## 2025

### Locomotion

- BeamDojo: Learning Agile Humanoid Locomotion on Sparse Footholds. Wang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.10363)
- Learning Humanoid Locomotion with Perceptive Internal Model. Long et al. ICRA, 2025. [Paper](https://junfeng-long.github.io/PIM/)
- Chasing Stability: Humanoid Running via Control Lyapunov Function Guided Reinforcement Learning. Olkin et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.19573)
- A Unified and General Humanoid Whole-Body Controller for Versatile Locomotion. Xue et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.03206)
- Gait-Conditioned Reinforcement Learning with Multi-Phase Curriculum for Humanoid Locomotion. Peng et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2505.20619)
- Contrastive Representation Learning for Robust Sim-to-Real Transfer of Adaptive Humanoid Locomotion. Lu et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.12858)
- Humanoid Whole-Body Locomotion on Narrow Terrain via Dynamic Balance and Reinforcement Learning. Xie et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.17219)
- ULC: A Unified and Fine-Grained Controller for Humanoid Loco-Manipulation. Sun et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2507.06905)
- HiFAR: Multi-stage Curriculum Learning for High-Dynamics Humanoid Fall Recovery. Chen et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.20061)
- Reduced-Order Model Guided Contact-Implicit Model Predictive Control for Humanoid Locomotion. Esteban et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.15630)
- RL-augmented Adaptive Model Predictive Control for Bipedal Locomotion over Challenging Terrain. Kamohara et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.18466)
- HuMam: Humanoid Motion Control via End-to-End Deep Reinforcement Learning with Mamba. Wang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.18046)
- Traversing Narrow Paths: A Two-Stage Reinforcement Learning Framework for Robust and Safe Humanoid Walking. Huang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2508.20661)
- RuN: Residual Policy for Natural Humanoid Locomotion. Li et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.20696)
- Learning Humanoid Standing-up Control Across Diverse Postures. Huang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.08378)
- Learning Getting-up Policies for Real-World Humanoid Robots. He et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.12152)
- FRASA: An End-to-End Reinforcement Learning Agent for Fall Recovery and Stand Up of Humanoid Robots. Gaspard et al. ICRA, 2025. [Paper](https://jglobal.jst.go.jp/en/public/202502215189879077) [Code](https://github.com/Rhoban/frasa)
- HWC-Loco: A Hierarchical Whole-Body Control Approach to Robust Humanoid Locomotion. Lin et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2503.00923)
- HuB: Learning Extreme Humanoid Balance. Zhang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2505.07294)
- Hold My Beer: Learning Gentle Humanoid Locomotion and End-Effector Stabilization Control. Li et al. CoRL, 2025. [Paper](https://proceedings.mlr.press/v305/li25i.html) [Project](https://lecar-lab.github.io/SoFTA/)

### Whole-Body Control and Motion Tracking

- GMT: General Motion Tracking for Humanoid Whole-Body Control. Chen et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2506.14770)
- UniTracker: Learning Universal Whole-Body Motion Tracker for Humanoid Robots. Yin et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2507.07356)
- Track Any Motions Under Any Disturbances. Zhang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.13833)
- Behavior Foundation Model for Humanoid Robots. Zeng et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.13780)
- SMAP: Self-supervised Motion Adaptation for Physically Plausible Humanoid Whole-body Control. Zhao et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2505.19463)
- KungfuBot: Physics-Based Humanoid Whole-Body Control for Learning Highly-Dynamic Skills. Xie et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2506.12851)
- KungfuBot2: Learning Versatile Motion Skills for Humanoid Whole-Body Control. Han et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.16638)
- BeyondMimic: From Motion Tracking to Versatile Humanoid Control via Guided Diffusion. Liao et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2508.08241)
- SoftMimic: Learning Compliant Whole-Body Control from Examples. Margolis et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2510.17792)
- ASAP: Aligning Simulation and Real-World Physics for Learning Agile Humanoid Whole-Body Skills. He et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.01143)
- Visual Imitation Enables Contextual Humanoid Control. Allshire et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2505.03729) [Project](https://videomimic.github.io/)
- HDMI: Learning Interactive Humanoid Whole-Body Control from Human Videos. Weng et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.16757)
- Towards Adaptable Humanoid Control via Adaptive Motion Tracking. Huang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2510.14454)
- Adversarial Locomotion and Motion Imitation for Humanoid Policy Learning. Shi et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2504.14305)
- Embrace Collisions: Humanoid Shadowing for Deployable Contact-Agnostic Motions. Zhuang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.01465)
- HOVER: Versatile Neural Whole-Body Controller for Humanoid Robots. He et al. ICRA, 2025. [Paper](https://arxiv.org/abs/2410.21229) [Project](https://hover-versatile-humanoid.github.io/)
- JAEGER: Dual-Level Humanoid Whole-Body Controller. Ding et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2505.06584)
- AMO: Adaptive Motion Optimization for Hyper-Dexterous Humanoid Whole-Body Control. Li et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2505.03738)
- Agility Meets Stability: Versatile Humanoid Control with Heterogeneous Data. Pan et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2511.17373)
- SONIC: Supersizing Motion Tracking for Natural Humanoid Whole-Body Control. Luo et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2511.07820)

### Teleoperation, Imitation, and Retargeting

- TWIST: Teleoperated Whole-Body Imitation System. Ze et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2505.02833)
- Mobile-TeleVision: Predictive Motion Priors for Humanoid Whole-Body Control. Lu et al. ICRA, 2025. [Paper](https://arxiv.org/abs/2412.07773) [Project](https://mobile-tv.github.io/)
- CLONE: Closed-Loop Whole-Body Humanoid Teleoperation for Long-Horizon Tasks. Li et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2506.08931)
- Homie: Humanoid Loco-Manipulation with Isomorphic Exoskeleton Cockpit. Ben et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2502.13013)
- Retargeting Matters: General Motion Retargeting for Humanoid Motion Tracking. Araujo et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2510.02252)
- OmniRetarget: Interaction-preserving Data Generation for Humanoid Whole-Body Loco-Manipulation and Scene Interaction. Yang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.26633)
- Implicit Kinodynamic Motion Retargeting for Human-to-Humanoid Imitation Learning. Chen et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.15443)

### Loco-Manipulation and Scene Interaction

- Falcon: Learning Force-Adaptive Humanoid Loco-Manipulation. Zhang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2505.06776)
- Unleashing Humanoid Reaching Potential via Real-world-Ready Skill Space. Zhang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2505.10918)
- ResMimic: From General Motion Tracking to Humanoid Whole-Body Loco-Manipulation via Residual Learning. Zhao et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2510.05070)
- Learning Human-Humanoid Coordination for Collaborative Object Carrying. Du et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2510.14293)
- TrajBooster: Boosting Humanoid Whole-Body Manipulation via Trajectory-Centric Learning. Liu et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.11839)
- VisualMimic: Visual Humanoid Loco-Manipulation via Motion Tracking and Generation. Yin et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.20322)
- Embracing Bulky Objects with Humanoid Robots: Whole-Body Manipulation with Reinforcement Learning. Zheng et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.13534)
- Opt2Skill: Imitating Dynamically-feasible Whole-Body Trajectories for Versatile Humanoid Loco-Manipulation. Liu et al. RA-L, 2025. [Paper](https://arxiv.org/abs/2409.20514) [Project](https://opt2skill.github.io/)
- DreamControl: Human-inspired Whole-Body Humanoid Control for Scene Interaction via Guided Diffusion. Kalaria et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.14353)
- StageACT: Stage-Conditioned Imitation for Robust Humanoid Door Opening. Lee et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.13200)
- PhySHSI: Towards a Real-World Generalizable and Natural Humanoid-Scene Interaction System. Wang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2510.11072)
- Hand-Eye Autonomous Delivery: Learning Humanoid Navigation, Locomotion and Reaching. Chen et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2508.03068)
- Hitter: A Humanoid Table Tennis Robot via Hierarchical Planning and Learning. Su et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2508.21043)
- SEEC: Stable End-Effector Control with Model-Enhanced Residual Learning for Humanoid Loco-Manipulation. Jang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2509.21231) [Project](https://seec-humanoid.github.io/)
- DemoHLM: From One Demonstration to Generalizable Humanoid Loco-Manipulation. Fu et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2510.11258)
- Opening the Sim-to-Real Door for Humanoid Pixel-to-Action Policy Transfer. Xue et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2512.01061)

### Language-Conditioned and Foundation Models

- LangWBC: Language-directed Humanoid Whole-Body Control via End-to-end Learning. Shao et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2504.21738)
- LeverB: Humanoid Whole-Body Control with Latent Vision-Language Instruction. Xue et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2506.13751)
- From Language to Locomotion: Retargeting-free Humanoid Control via Motion Latent Guidance. Li et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2510.14952)
- Sentinel: A Fully End-to-End Language-Action Model for Humanoid Whole Body Control. Wang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2511.19236)
- Commanding Humanoid by Free-form Language: A Large Language Action Model with Unified Motion Vocabulary. Liu et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2511.22963)
- BFM-Zero: A Promptable Behavioral Foundation Model for Humanoid Control using Unsupervised Reinforcement Learning. Li et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2511.04131)
- UniAct: Unified Motion Generation and Action Streaming for Humanoid Robots. Jiang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2512.24321)

### Simulators, Datasets, Surveys, and Background

- Humanoid Locomotion and Manipulation: Current Progress and Challenges in Control, Planning, and Learning. Gu et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2501.02116)
- Learning-based Legged Locomotion: State of the Art and Future Perspectives. Ha et al. IJRR, 2025. [Paper](https://doi.org/10.1177/02783649241312698)
- Deep Reinforcement Learning for Robotics: A Survey of Real-World Successes. Tang et al. AAAI, 2025. [Paper](https://doi.org/10.1609/aaai.v39i27.35095)
- Isaac Lab: A GPU-accelerated Simulation Framework for Multi-Modal Robot Learning. Mittal et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2511.04831) [Code](https://github.com/isaac-sim/IsaacLab)
- PHUMA: Physically-grounded Humanoid Locomotion Dataset. Lee et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2510.26236)
- Motion-X++: A Large-Scale Multimodal 3D Whole-body Human Motion Dataset. Zhang et al. arXiv, 2025. [Paper](https://arxiv.org/abs/2501.05098)
- Go to Zero: Towards Zero-shot Motion Generation with Million-scale Data. Fan et al. ICCV, 2025. [Paper](https://arxiv.org/abs/2507.07095)
- InterMimic: Towards Universal Whole-Body Control for Physics-Based Human-Object Interactions. Xu et al. CVPR, 2025. [Paper](https://arxiv.org/abs/2502.20390) [Project](https://sirui-xu.github.io/InterMimic/)
- ModSkill: Physical Character Skill Modularization. Huang et al. ICCV, 2025. [Paper](https://openaccess.thecvf.com/content/ICCV2025/html/Huang_ModSkill_Physical_Character_Skill_Modularization_ICCV_2025_paper.html)
- Diffusion Policy: Visuomotor Policy Learning via Action Diffusion. Chi et al. IJRR, 2025. [Paper](https://arxiv.org/abs/2303.04137)
- Learning Multi-Modal Whole-Body Control for Real-World Humanoid Robots. Dugar et al. AAAI Symposium, 2025. [Paper](https://arxiv.org/abs/2408.07295) [Project](https://masked-humanoid.github.io/mhc/)

## 2024

### Locomotion

- Advancing Humanoid Locomotion: Mastering Challenging Terrains with Denoising World Model Learning. Gu et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2408.14472)
- Revisiting Reward Design and Evaluation for Robust Humanoid Standing and Walking. van Marum et al. IROS, 2024. [Paper](https://doi.org/10.1109/IROS58592.2024.10802680)
- Real-World Humanoid Locomotion with Reinforcement Learning. Radosavovic et al. Science Robotics, 2024. [Paper](https://arxiv.org/abs/2303.03381) [Project](https://learning-humanoid-locomotion.github.io/)
- Learn to Teach: Sample-Efficient Privileged Learning for Humanoid Locomotion over Diverse Terrains. Wu et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2402.06783)
- Learning Humanoid Locomotion over Challenging Terrain. Radosavovic et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2410.03654)
- Whole-Body Humanoid Robot Locomotion with Human Reference. Zhang et al. IROS, 2024. [Paper](https://arxiv.org/abs/2402.18294)
- HumanMimic: Learning Natural Locomotion and Transitions for Humanoid Robot via Wasserstein Adversarial Imitation. Tang et al. ICRA, 2024. [Paper](https://arxiv.org/abs/2309.14225)
- Humanoid Parkour Learning. Zhuang et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2406.10759)

### Whole-Body Control and Motion Priors

- Expressive Whole-Body Control for Humanoid Robots. Cheng et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2402.16796)
- ExBody2: Advanced Expressive Humanoid Whole-Body Control. Ji et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2412.13196)
- FLD: Fourier Latent Dynamics for Structured Motion Representation and Learning. Li et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2402.13820)
- HumanPlus: Humanoid Shadowing and Imitation from Humans. Fu et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2406.10454)
- I-CTRL: Imitation to Control Humanoid Robots through Constrained Reinforcement Learning. Yan et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2405.08726)
- Learning from Massive Human Videos for Universal Humanoid Pose Control. Mao et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2412.14172)
- Wococo: Learning Whole-Body Humanoid Control with Sequential Contacts. Zhang et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2406.06005)

### Teleoperation, Imitation, and Retargeting

- Learning Human-to-Humanoid Real-Time Whole-Body Teleoperation. He et al. IROS, 2024. [Paper](https://arxiv.org/abs/2403.04436) [Project](https://human2humanoid.com/)
- OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning. He et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2406.08858) [Project](https://omni.human2humanoid.com/)
- Open-TeleVision: Teleoperation with Immersive Active Visual Feedback. Cheng et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2407.01512)

### Manipulation, Scene Interaction, and Diffusion-based Control

- Generalizable Humanoid Manipulation with Improved 3D Diffusion Policies. Ze et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2410.10803)
- CooHOI: Learning Cooperative Human-Object Interaction with Manipulated Object Dynamics. Gao et al. NeurIPS, 2024. [Paper](https://papers.nips.cc/paper_files/paper/2024/hash/8ff154c486ef2f73894f7d0ee7ee8f54-Abstract-Conference.html)
- Sim-to-Real Learning for Humanoid Box Loco-Manipulation. Dao et al. ICRA, 2024. [Paper](https://ieeexplore.ieee.org/document/10611502)
- OKAMI: Teaching Humanoid Robots Manipulation Skills through Single Video Imitation. Li et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2410.11792) [Project](https://ut-austin-rpl.github.io/OKAMI/)
- Harmon: Whole-Body Motion Generation of Humanoid Robots from Language Descriptions. Jiang et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2410.12773) [Project](https://ut-austin-rpl.github.io/Harmon/)
- Adaptive-Frequency Model Learning and Predictive Control for Dynamic Maneuvers on Legged Robots. Nguyen et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2407.14749)

### Surveys, Human Motion, and Supporting Infrastructure

- Learning Robot Soccer from Egocentric Vision with Deep Reinforcement Learning. Tirumala et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2405.02425)
- Learning Agile Soccer Skills for a Bipedal Robot with Deep Reinforcement Learning. Haarnoja et al. Science Robotics, 2024. [Paper](https://arxiv.org/abs/2304.13653)
- Advancements in Humanoid Robots: A Comprehensive Review and Future Prospects. Tong et al. IEEE/CAA Journal of Automatica Sinica, 2024. [Paper](https://doi.org/10.1109/JAS.2024.124237)
- WHAM: Reconstructing World-grounded Humans with Accurate 3D Motion. Shin et al. CVPR, 2024. [Paper](https://wham.is.tue.mpg.de/)
- World-Grounded Human Motion Recovery via Gravity-View Coordinates. Shen et al. SIGGRAPH Asia, 2024. [Paper](https://arxiv.org/abs/2409.06661)
- TRAM: Global Trajectory and Motion of 3D Humans from In-the-Wild Videos. Wang et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2403.17346)
- Genesis: A Generative and Universal Physics Engine for Robotics and Beyond. Zhou et al. arXiv, 2024. [Paper](https://arxiv.org/abs/2401.01454)

## 2023

### Humanoid Control

- Learning Bipedal Walking for Humanoids with Current Feedback. Xie et al. IEEE Access, 2023. [Paper](https://ieeexplore.ieee.org/document/10245056)
- Perpetual Humanoid Control for Real-time Simulated Avatars. Luo et al. ICCV, 2023. [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.html)
- Universal Humanoid Motion Representations for Physics-Based Control. Luo et al. arXiv, 2023. [Paper](https://arxiv.org/abs/2310.04582)

### Human Motion Models and Retargeting Context

- Object Motion Guided Human Motion Synthesis. Li et al. TOG, 2023. [Paper](https://arxiv.org/abs/2309.16237)
- SMPL: A Skinned Multi-Person Linear Model. Loper et al. Seminal Graphics Papers, 2023. [Paper](https://smpl.is.tue.mpg.de/)
- Generating Human Motion from Textual Descriptions with Discrete Representations. Zhang et al. CVPR, 2023. [Paper](https://arxiv.org/abs/2301.06052)

## 2022 and Earlier

### Humanoid and Legged Learning

- Learning Natural Locomotion Behaviors for Humanoid Robots using Human Bias. Yang et al. RA-L, 2020. [Paper](https://www.research.ed.ac.uk/en/publications/learning-natural-locomotion-behaviors-for-humanoid-robots-using-h)
- Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning. Rudin et al. arXiv, 2022. [Paper](https://arxiv.org/abs/2109.11978)
- Isaac Gym: High Performance GPU-Based Physics Simulation for Robot Learning. Makoviychuk et al. arXiv, 2021. [Paper](https://arxiv.org/abs/2108.10470)
- MuJoCo: A Physics Engine for Model-Based Control. Todorov et al. IROS, 2012. [Paper](https://ieeexplore.ieee.org/document/6386109)

### Human Motion Datasets and Perception

- AMASS: Archive of Motion Capture as Surface Shapes. Mahmood et al. ICCV, 2019. [Paper](https://amass.is.tue.mpg.de/) [Project](https://is.mpg.de/ps/publications/amass-iccv-2019)
- Robust Motion In-betweening. Harvey et al. TOG, 2020. [Paper](https://arxiv.org/abs/2002.04900)
- Generating Diverse and Natural 3D Human Motions from Text. Guo et al. CVPR, 2022. [Paper](https://arxiv.org/abs/2206.10949)
- NTU RGB+D: A Large Scale Dataset for 3D Human Activity Analysis. Shahroudy et al. CVPR, 2016. [Paper](https://rose1.ntu.edu.sg/dataset/actionRecognition/)
- NTU RGB+D 120: A Large-Scale Benchmark for 3D Human Activity Understanding. Liu et al. TPAMI, 2020. [Paper](https://arxiv.org/abs/1905.04757)
- HybrIK: A Hybrid Analytical-Neural Inverse Kinematics Solution for 3D Human Pose and Shape Estimation. Li et al. CVPR, 2021. [Paper](https://arxiv.org/abs/2011.14672) [Code](https://github.com/jeffffffli/HybrIK)
- Human Motion Diffusion Model. Tevet et al. arXiv, 2022. [Paper](https://arxiv.org/abs/2209.14916)
- Learning Transferable Visual Models from Natural Language Supervision. Radford et al. ICML, 2021. [Paper](https://arxiv.org/abs/2103.00020)

### Surveys and General Background

- Community Detection in Graphs. Fortunato. Physics Reports, 2010. [Paper](https://doi.org/10.1016/j.physrep.2009.11.002)

## Open-Source Frameworks

- HumanoidVerse: A Multi-Simulator Framework for Humanoid Robot Sim-to-Real Learning. GitHub repository, 2025. [Project](https://github.com/LeCAR-Lab/HumanoidVerse) [Code](https://github.com/LeCAR-Lab/HumanoidVerse)
- ProtoMotions3: An Open-source Framework for Humanoid Simulation and Control. GitHub repository, 2025. [Project](https://github.com/NVLabs/ProtoMotions/) [Code](https://github.com/NVLabs/ProtoMotions/)
- MuJoCo Playground: An Open-source Framework for GPU-accelerated Robot Learning and Sim-to-Real Transfer. GitHub repository, 2025. [Project](https://github.com/google-deepmind/mujoco_playground) [Code](https://github.com/google-deepmind/mujoco_playground)
- Isaac Lab. Open-source repository. [Project](https://github.com/isaac-sim/IsaacLab) [Code](https://github.com/isaac-sim/IsaacLab)
- Motion-X. Official implementation and dataset release. [Project](https://github.com/IDEA-Research/Motion-X) [Code](https://github.com/IDEA-Research/Motion-X)

## Citation

If this repository is useful in your review or implementation work, please cite the accompanying survey once it is publicly available:

```text
Learning-Based Whole-Body Control for Humanoid Robots: An Implementation-Centric Review
```

Pull requests for missing links, wrong venue assignments, or new code releases are welcome.
