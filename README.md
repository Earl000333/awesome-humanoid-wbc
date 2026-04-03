# A Survey on Learning-Based Whole-Body Control for Humanoid Robots

[![Survey](https://img.shields.io/badge/Type-Survey%20Companion-1f6feb?style=flat-square)](https://github.com/Earl000333/awesome-humanoid-wbc)
[![Topic](https://img.shields.io/badge/Topic-Humanoid%20WBC-0f766e?style=flat-square)](https://github.com/Earl000333/awesome-humanoid-wbc)
[![Focus](https://img.shields.io/badge/Focus-Implementation--Centric-b45309?style=flat-square)](https://github.com/Earl000333/awesome-humanoid-wbc)
[![Status](https://img.shields.io/badge/Status-Active%20Curation-7c3aed?style=flat-square)](https://github.com/Earl000333/awesome-humanoid-wbc)

Project page and curated reference repository for the survey paper *A Survey on Learning-Based Whole-Body Control for Humanoid Robots*.

This repository organizes the literature of humanoid whole-body control from an implementation-oriented perspective, following the pipeline from **data acquisition**, **policy learning**, and **simulation transfer** to **real-robot deployment**. The main papers are grouped into four paradigms: **command-based control**, **motion tracking-based control**, **interaction-based control**, and **multimodal learning-based control**.

> The goal of this repository is readability and implementation value: representative papers, key datasets, simulators, and official code resources are placed in one survey-aligned index.
>
> Code links are included when an official repository or project page is clearly available.

Last updated: 2026-03-20

## Table of Contents

- [Latest Works Recommended](#latest-works-recommended)
- [Survey View](#survey-view)
- [Task Taxonomy](#task-taxonomy)
- [Implementation Pipeline](#implementation-pipeline)
- [Command-based Control](#command-based-control)
- [Motion Tracking-based Control](#motion-tracking-based-control)
- [Interaction-based Control](#interaction-based-control)
- [Multimodal Learning-based Control](#multimodal-learning-based-control)
- [Motion Data, Retargeting, and Perception Assets](#motion-data-retargeting-and-perception-assets)
- [Simulators and Open-Source Frameworks](#simulators-and-open-source-frameworks)
- [Surveys and Background](#surveys-and-background)
- [Citation](#citation)

## Latest Works Recommended

| Title | Why it matters | Venue | Links |
| --- | --- | --- | --- |
| Real-World Humanoid Locomotion with Reinforcement Learning | Landmark real-robot RL locomotion baseline for modern humanoid control | Science Robotics 2024 | [Paper](https://arxiv.org/abs/2303.03381) / [Project](https://learning-humanoid-locomotion.github.io/) |
| Learning Humanoid Locomotion with Perceptive Internal Model | Strong terrain-aware command-based locomotion pipeline | ICRA 2025 | [Paper](https://junfeng-long.github.io/PIM/) |
| ExBody2: Advanced Expressive Humanoid Whole-Body Control | Representative large-scale motion tracking and expressive imitation system | arXiv 2024 | [Paper](https://arxiv.org/abs/2412.13196) |
| HOVER: Versatile Neural Whole-Body Controller for Humanoid Robots | Unified whole-body control across multiple behavior modes | ICRA 2025 | [Paper](https://arxiv.org/abs/2410.21229) / [Project](https://hover-versatile-humanoid.github.io/) |
| OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning | Strong teleoperation and human-to-humanoid data pipeline | arXiv 2024 | [Paper](https://arxiv.org/abs/2406.08858) / [Project](https://omni.human2humanoid.com/) |
| BeyondMimic: From Motion Tracking to Versatile Humanoid Control via Guided Diffusion | Representative diffusion-based whole-body control work | arXiv 2025 | [Paper](https://arxiv.org/abs/2508.08241) |
| LangWBC: Language-directed Humanoid Whole-Body Control via End-to-end Learning | Clear entry point for language-conditioned humanoid control | arXiv 2025 | [Paper](https://arxiv.org/abs/2504.21738) |
| HumanoidVerse: A Multi-Simulator Framework for Humanoid Robot Sim-to-Real Learning | Practical open-source stack for experimentation and sim-to-real studies | GitHub 2025 | [Repo](https://github.com/LeCAR-Lab/HumanoidVerse) |

## Survey View

This repository is designed to mirror the structure of the survey:

1. **Task understanding**: what control objective is being solved.
2. **Data pipeline**: where motion, perception, and interaction priors come from.
3. **Learning paradigm**: RL, imitation, teacher-student distillation, latent modeling, diffusion, or foundation models.
4. **Deployment stack**: simulator choice, sim-to-real method, and real-robot engineering constraints.

If you are reading the survey while building a system, the tables below are intended to let you jump quickly from a paragraph in the paper to representative references and codebases.

## Task Taxonomy

| Paradigm | Typical input | Typical output | Core challenge | Representative examples |
| --- | --- | --- | --- | --- |
| Command-based control | Velocity, heading, gait command, terrain cues | Whole-body locomotion actions | Stability, robustness, terrain adaptation, curriculum design | Real-World RL, PIM, BeamDojo, HugWBC |
| Motion tracking-based control | MoCap, video, teleoperation, reference trajectory | High-fidelity whole-body tracking | Physical plausibility, tracking fidelity, deployable sensing | ExBody2, GMT, UniTracker, HOVER |
| Interaction-based control | Object/task goals, contact objectives, sparse rewards | Contact-rich loco-manipulation policy | Sparse-reward exploration, long-horizon planning, contact robustness | AMO, Falcon, StageACT, Opt2Skill |
| Multimodal learning-based control | Vision, language, proprioception, semantics | Perception-to-action or semantic-to-action policy | Cross-modal alignment, feasibility, real-time inference | LangWBC, LeVERB, Sentinel, FRoM-W1 |

## Implementation Pipeline

| Stage | Main questions in the survey | Representative resources |
| --- | --- | --- |
| Data acquisition and construction | Where do motion priors come from, and how are they retargeted, filtered, and augmented? | AMASS, PHUMA, Motion-X++, WHAM, OmniRetarget |
| Policy learning and architecture design | Which training paradigm best fits the task: RL, imitation, hierarchical control, diffusion, latent modeling, or BFMs? | Real-World RL, ExBody2, HOVER, BeyondMimic, BFM-Zero |
| Simulation transfer and deployment | Which simulator, transfer strategy, and hardware adaptation stack support real deployment? | Isaac Gym, Isaac Lab, MuJoCo, Genesis, HumanoidVerse |

## Command-based Control

| Title | Venue | Year | Focus | Links |
| --- | --- | --- | --- | --- |
| Learning Natural Locomotion Behaviors for Humanoid Robots using Human Bias | RA-L | 2020 | Early learning-based natural locomotion prior | [Paper](https://www.research.ed.ac.uk/en/publications/learning-natural-locomotion-behaviors-for-humanoid-robots-using-h) |
| Real-World Humanoid Locomotion with Reinforcement Learning | Science Robotics | 2024 | Real-robot locomotion with RL | [Paper](https://arxiv.org/abs/2303.03381) / [Project](https://learning-humanoid-locomotion.github.io/) |
| Advancing Humanoid Locomotion: Mastering Challenging Terrains with Denoising World Model Learning | arXiv | 2024 | Challenging terrain locomotion with latent world-model guidance | [Paper](https://arxiv.org/abs/2408.14472) |
| Learn to Teach: Sample-Efficient Privileged Learning for Humanoid Locomotion over Diverse Terrains | arXiv | 2024 | Privileged teacher-student terrain learning | [Paper](https://arxiv.org/abs/2402.06783) |
| Revisiting Reward Design and Evaluation for Robust Humanoid Standing and Walking | IROS | 2024 | Reward-design analysis for standing and walking | [Paper](https://doi.org/10.1109/IROS58592.2024.10802680) |
| Learning Humanoid Locomotion over Challenging Terrain | arXiv | 2024 | Terrain locomotion benchmark-style formulation | [Paper](https://arxiv.org/abs/2410.03654) |
| Learning Humanoid Locomotion with Perceptive Internal Model | ICRA | 2025 | Terrain-aware locomotion with internal perceptive model | [Paper](https://junfeng-long.github.io/PIM/) |
| BeamDojo: Learning Agile Humanoid Locomotion on Sparse Footholds | arXiv | 2025 | Sparse foothold locomotion | [Paper](https://arxiv.org/abs/2502.10363) |
| A Unified and General Humanoid Whole-Body Controller for Versatile Locomotion | arXiv | 2025 | Unified locomotion controller | [Paper](https://arxiv.org/abs/2502.03206) |
| Gait-Conditioned Reinforcement Learning with Multi-Phase Curriculum for Humanoid Locomotion | arXiv | 2025 | Gait-conditioned curriculum design | [Paper](https://arxiv.org/abs/2505.20619) |
| Humanoid Whole-Body Locomotion on Narrow Terrain via Dynamic Balance and Reinforcement Learning | arXiv | 2025 | Dynamic balance on narrow terrain | [Paper](https://arxiv.org/abs/2502.17219) |
| Traversing Narrow Paths: A Two-Stage Reinforcement Learning Framework for Robust and Safe Humanoid Walking | arXiv | 2025 | Safe narrow-path walking | [Paper](https://arxiv.org/abs/2508.20661) |
| HWC-Loco: A Hierarchical Whole-Body Control Approach to Robust Humanoid Locomotion | arXiv | 2025 | Hierarchical locomotion control | [Paper](https://arxiv.org/abs/2503.00923) |
| Chasing Stability: Humanoid Running via Control Lyapunov Function Guided Reinforcement Learning | arXiv | 2025 | CLF-guided running | [Paper](https://arxiv.org/abs/2509.19573) |
| HuB: Learning Extreme Humanoid Balance | arXiv | 2025 | Extreme balance and recovery | [Paper](https://arxiv.org/abs/2505.07294) |
| Learning Humanoid Standing-up Control Across Diverse Postures | arXiv | 2025 | Stand-up control from diverse initial states | [Paper](https://arxiv.org/abs/2502.08378) |
| Learning Getting-up Policies for Real-World Humanoid Robots | arXiv | 2025 | Real-world getting-up deployment | [Paper](https://arxiv.org/abs/2502.12152) |
| FRASA: An End-to-End Reinforcement Learning Agent for Fall Recovery and Stand Up of Humanoid Robots | ICRA | 2025 | Fall recovery and stand-up | [Paper](https://jglobal.jst.go.jp/en/public/202502215189879077) / [Code](https://github.com/Rhoban/frasa) |
| Hold My Beer: Learning Gentle Humanoid Locomotion and End-Effector Stabilization Control | CoRL | 2025 | Locomotion with stabilized upper body | [Paper](https://proceedings.mlr.press/v305/li25i.html) / [Project](https://lecar-lab.github.io/SoFTA/) |
| CLF-RL: Control Lyapunov Function Guided Reinforcement Learning | RA-L | 2026 | Formal-stability-guided RL | [Paper](https://www.zacholkin.com/research/clf_rl/) |
| OmniXtreme: Breaking the Generality Barrier in High-Dynamic Humanoid Control | arXiv | 2026 | Highly dynamic general-purpose control | [Paper](https://arxiv.org/abs/2602.23843) |

## Motion Tracking-based Control

| Title | Venue | Year | Focus | Links |
| --- | --- | --- | --- | --- |
| Whole-Body Humanoid Robot Locomotion with Human Reference | IROS | 2024 | Human-reference locomotion tracking | [Paper](https://arxiv.org/abs/2402.18294) |
| Expressive Whole-Body Control for Humanoid Robots | arXiv | 2024 | Expressive motion imitation baseline | [Paper](https://arxiv.org/abs/2402.16796) |
| ExBody2: Advanced Expressive Humanoid Whole-Body Control | arXiv | 2024 | Large-scale expressive tracking | [Paper](https://arxiv.org/abs/2412.13196) |
| HumanMimic: Learning Natural Locomotion and Transitions for Humanoid Robot via Wasserstein Adversarial Imitation | ICRA | 2024 | Adversarial imitation for natural locomotion | [Paper](https://arxiv.org/abs/2309.14225) |
| Learning Human-to-Humanoid Real-Time Whole-Body Teleoperation | IROS | 2024 | Real-time teleoperation pipeline | [Paper](https://arxiv.org/abs/2403.04436) / [Project](https://human2humanoid.com/) |
| OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning | arXiv | 2024 | Unified teleoperation and learning system | [Paper](https://arxiv.org/abs/2406.08858) / [Project](https://omni.human2humanoid.com/) |
| HumanPlus: Humanoid Shadowing and Imitation from Humans | arXiv | 2024 | Human shadowing and imitation | [Paper](https://arxiv.org/abs/2406.10454) |
| Learning from Massive Human Videos for Universal Humanoid Pose Control | arXiv | 2024 | Large-scale video-derived motion prior | [Paper](https://arxiv.org/abs/2412.14172) |
| GMT: General Motion Tracking for Humanoid Whole-Body Control | arXiv | 2025 | Multi-motion tracking and robustness | [Paper](https://arxiv.org/abs/2506.14770) |
| UniTracker: Learning Universal Whole-Body Motion Tracker for Humanoid Robots | arXiv | 2025 | Universal motion tracker | [Paper](https://arxiv.org/abs/2507.07356) |
| Track Any Motions Under Any Disturbances | arXiv | 2025 | Disturbance-robust tracking | [Paper](https://arxiv.org/abs/2509.13833) |
| HOVER: Versatile Neural Whole-Body Controller for Humanoid Robots | ICRA | 2025 | Unified whole-body controller | [Paper](https://arxiv.org/abs/2410.21229) / [Project](https://hover-versatile-humanoid.github.io/) |
| SMAP: Self-supervised Motion Adaptation for Physically Plausible Humanoid Whole-body Control | arXiv | 2025 | Motion adaptation across embodiment gap | [Paper](https://arxiv.org/abs/2505.19463) |
| KungfuBot: Physics-Based Humanoid Whole-Body Control for Learning Highly-Dynamic Skills | arXiv | 2025 | High-dynamic skill tracking | [Paper](https://arxiv.org/abs/2506.12851) |
| KungfuBot2: Learning Versatile Motion Skills for Humanoid Whole-Body Control | arXiv | 2025 | Versatile high-dynamic motion skills | [Paper](https://arxiv.org/abs/2509.16638) |
| BeyondMimic: From Motion Tracking to Versatile Humanoid Control via Guided Diffusion | arXiv | 2025 | Diffusion-based motion tracking | [Paper](https://arxiv.org/abs/2508.08241) |
| ASAP: Aligning Simulation and Real-World Physics for Learning Agile Humanoid Whole-Body Skills | arXiv | 2025 | Sim-to-real alignment for imitation-style skills | [Paper](https://arxiv.org/abs/2502.01143) |
| HDMI: Learning Interactive Humanoid Whole-Body Control from Human Videos | arXiv | 2025 | Video-driven whole-body control | [Paper](https://arxiv.org/abs/2509.16757) |
| Mobile-TeleVision: Predictive Motion Priors for Humanoid Whole-Body Control | ICRA | 2025 | Motion priors for teleoperation | [Paper](https://arxiv.org/abs/2412.07773) / [Project](https://mobile-tv.github.io/) |
| TWIST: Teleoperated Whole-Body Imitation System | arXiv | 2025 | Teleoperated imitation and deployment | [Paper](https://arxiv.org/abs/2505.02833) |
| CLONE: Closed-Loop Whole-Body Humanoid Teleoperation for Long-Horizon Tasks | arXiv | 2025 | Closed-loop long-horizon teleoperation | [Paper](https://arxiv.org/abs/2506.08931) |
| Homie: Humanoid Loco-Manipulation with Isomorphic Exoskeleton Cockpit | arXiv | 2025 | Exoskeleton-based teleoperation | [Paper](https://arxiv.org/abs/2502.13013) |
| Retargeting Matters: General Motion Retargeting for Humanoid Motion Tracking | arXiv | 2025 | General-purpose retargeting pipeline | [Paper](https://arxiv.org/abs/2510.02252) |
| Towards Adaptable Humanoid Control via Adaptive Motion Tracking | arXiv | 2025 | Motion-tracking-driven adaptation | [Paper](https://arxiv.org/abs/2510.14454) |
| SONIC: Supersizing Motion Tracking for Natural Humanoid Whole-Body Control | arXiv | 2025 | Scaling motion tracking with more data and model capacity | [Paper](https://arxiv.org/abs/2511.07820) |

## Interaction-based Control

| Title | Venue | Year | Focus | Links |
| --- | --- | --- | --- | --- |
| Wococo: Learning Whole-Body Humanoid Control with Sequential Contacts | arXiv | 2024 | Sequential-contact whole-body control | [Paper](https://arxiv.org/abs/2406.06005) |
| CooHOI: Learning Cooperative Human-Object Interaction with Manipulated Object Dynamics | NeurIPS | 2024 | Human-object interaction prior | [Paper](https://papers.nips.cc/paper_files/paper/2024/hash/8ff154c486ef2f73894f7d0ee7ee8f54-Abstract-Conference.html) |
| Sim-to-Real Learning for Humanoid Box Loco-Manipulation | ICRA | 2024 | Box carrying and loco-manipulation | [Paper](https://ieeexplore.ieee.org/document/10611502) |
| OKAMI: Teaching Humanoid Robots Manipulation Skills through Single Video Imitation | arXiv | 2024 | Single-video manipulation imitation | [Paper](https://arxiv.org/abs/2410.11792) / [Project](https://ut-austin-rpl.github.io/OKAMI/) |
| ULC: A Unified and Fine-Grained Controller for Humanoid Loco-Manipulation | arXiv | 2025 | Unified locomotion and manipulation | [Paper](https://arxiv.org/abs/2507.06905) |
| AMO: Adaptive Motion Optimization for Hyper-Dexterous Humanoid Whole-Body Control | arXiv | 2025 | Optimization-guided whole-body manipulation | [Paper](https://arxiv.org/abs/2505.03738) |
| Falcon: Learning Force-Adaptive Humanoid Loco-Manipulation | arXiv | 2025 | Force-adaptive interaction | [Paper](https://arxiv.org/abs/2505.06776) |
| Unleashing Humanoid Reaching Potential via Real-world-Ready Skill Space | arXiv | 2025 | Reaching skill space for deployment | [Paper](https://arxiv.org/abs/2505.10918) |
| ResMimic: From General Motion Tracking to Humanoid Whole-Body Loco-Manipulation via Residual Learning | arXiv | 2025 | Residual learning for loco-manipulation | [Paper](https://arxiv.org/abs/2510.05070) |
| Learning Human-Humanoid Coordination for Collaborative Object Carrying | arXiv | 2025 | Human-robot collaborative carrying | [Paper](https://arxiv.org/abs/2510.14293) |
| TrajBooster: Boosting Humanoid Whole-Body Manipulation via Trajectory-Centric Learning | arXiv | 2025 | Trajectory-centric manipulation learning | [Paper](https://arxiv.org/abs/2509.11839) |
| VisualMimic: Visual Humanoid Loco-Manipulation via Motion Tracking and Generation | arXiv | 2025 | Visual loco-manipulation | [Paper](https://arxiv.org/abs/2509.20322) |
| Embracing Bulky Objects with Humanoid Robots: Whole-Body Manipulation with Reinforcement Learning | arXiv | 2025 | Bulky-object manipulation | [Paper](https://arxiv.org/abs/2509.13534) |
| Opt2Skill: Imitating Dynamically-feasible Whole-Body Trajectories for Versatile Humanoid Loco-Manipulation | RA-L | 2025 | Dynamically feasible trajectory imitation | [Paper](https://arxiv.org/abs/2409.20514) / [Project](https://opt2skill.github.io/) |
| DreamControl: Human-inspired Whole-Body Humanoid Control for Scene Interaction via Guided Diffusion | arXiv | 2025 | Scene interaction with guided diffusion | [Paper](https://arxiv.org/abs/2509.14353) |
| StageACT: Stage-Conditioned Imitation for Robust Humanoid Door Opening | arXiv | 2025 | Long-horizon door-opening interaction | [Paper](https://arxiv.org/abs/2509.13200) |
| PhySHSI: Towards a Real-World Generalizable and Natural Humanoid-Scene Interaction System | arXiv | 2025 | Scene interaction system | [Paper](https://arxiv.org/abs/2510.11072) |
| Hand-Eye Autonomous Delivery: Learning Humanoid Navigation, Locomotion and Reaching | arXiv | 2025 | Navigation + reaching in one policy stack | [Paper](https://arxiv.org/abs/2508.03068) |
| Hitter: A Humanoid Table Tennis Robot via Hierarchical Planning and Learning | arXiv | 2025 | Skill hierarchy for sports interaction | [Paper](https://arxiv.org/abs/2508.21043) |
| SEEC: Stable End-Effector Control with Model-Enhanced Residual Learning for Humanoid Loco-Manipulation | arXiv | 2025 | Stable end-effector control | [Paper](https://arxiv.org/abs/2509.21231) / [Project](https://seec-humanoid.github.io/) |
| DemoHLM: From One Demonstration to Generalizable Humanoid Loco-Manipulation | arXiv | 2025 | One-shot demonstration to generalization | [Paper](https://arxiv.org/abs/2510.11258) |

## Multimodal Learning-based Control

| Title | Venue | Year | Modality | Links |
| --- | --- | --- | --- | --- |
| Humanoid Parkour Learning | arXiv | 2024 | Vision-to-action locomotion | [Paper](https://arxiv.org/abs/2406.10759) |
| Generalizable Humanoid Manipulation with Improved 3D Diffusion Policies | arXiv | 2024 | 3D visual diffusion policy | [Paper](https://arxiv.org/abs/2410.10803) |
| Harmon: Whole-Body Motion Generation of Humanoid Robots from Language Descriptions | arXiv | 2024 | Language-to-motion generation | [Paper](https://arxiv.org/abs/2410.12773) / [Project](https://ut-austin-rpl.github.io/Harmon/) |
| Visual Imitation Enables Contextual Humanoid Control | arXiv | 2025 | Video-conditioned contextual control | [Paper](https://arxiv.org/abs/2505.03729) / [Project](https://videomimic.github.io/) |
| LangWBC: Language-directed Humanoid Whole-Body Control via End-to-end Learning | arXiv | 2025 | Language-conditioned whole-body control | [Paper](https://arxiv.org/abs/2504.21738) |
| LeverB: Humanoid Whole-Body Control with Latent Vision-Language Instruction | arXiv | 2025 | Vision-language latent control | [Paper](https://arxiv.org/abs/2506.13751) |
| From Language to Locomotion: Retargeting-free Humanoid Control via Motion Latent Guidance | arXiv | 2025 | Language-to-locomotion with latent guidance | [Paper](https://arxiv.org/abs/2510.14952) |
| Sentinel: A Fully End-to-End Language-Action Model for Humanoid Whole Body Control | arXiv | 2025 | End-to-end language-action model | [Paper](https://arxiv.org/abs/2511.19236) |
| Commanding Humanoid by Free-form Language: A Large Language Action Model with Unified Motion Vocabulary | arXiv | 2025 | Free-form language control | [Paper](https://arxiv.org/abs/2511.22963) |
| BFM-Zero: A Promptable Behavioral Foundation Model for Humanoid Control using Unsupervised Reinforcement Learning | arXiv | 2025 | Promptable behavior foundation model | [Paper](https://arxiv.org/abs/2511.04131) |
| UniAct: Unified Motion Generation and Action Streaming for Humanoid Robots | arXiv | 2025 | Unified generation and action streaming | [Paper](https://arxiv.org/abs/2512.24321) |
| Opening the Sim-to-Real Door for Humanoid Pixel-to-Action Policy Transfer | arXiv | 2025 | Vision-based pixel-to-action transfer | [Paper](https://arxiv.org/abs/2512.01061) |
| FRoM-W1: Towards General Humanoid Whole-Body Control with Language Instructions | arXiv | 2026 | Language-conditioned general WBC | [Paper](https://arxiv.org/abs/2601.12799) |
| HumanX: Toward Agile and Generalizable Humanoid Interaction Skills from Human Videos | arXiv | 2026 | Large-scale human-video-driven interaction skill learning | [Paper](https://arxiv.org/abs/2602.02473) |

## Motion Data, Retargeting, and Perception Assets

| Resource | Type | Why it matters | Links |
| --- | --- | --- | --- |
| AMASS | Dataset | Canonical large-scale MoCap corpus for motion priors | [Project](https://amass.is.tue.mpg.de/) |
| HumanML3D | Dataset | Motion-language alignment for language-conditioned control | [Paper](https://arxiv.org/abs/2206.10659) |
| OMOMO | Dataset | Human-object interaction data for interaction-rich tasks | [Paper](https://arxiv.org/abs/2301.07553) |
| PHUMA | Dataset | Robot-oriented physically grounded humanoid locomotion dataset | [Paper](https://arxiv.org/abs/2510.26236) |
| Motion-X++ | Dataset | Large-scale multimodal whole-body human motion data | [Paper](https://arxiv.org/abs/2501.05098) |
| Go to Zero / MotionMillion | Dataset | Million-scale motion generation data source | [Paper](https://arxiv.org/abs/2507.07095) |
| NTU RGB+D / NTU RGB+D 120 | Dataset | Human activity understanding benchmark useful for multimodal pretraining | [NTU RGB+D](https://rose1.ntu.edu.sg/dataset/actionRecognition/) / [NTU 120](https://arxiv.org/abs/1905.04757) |
| WHAM | Human motion recovery | Widely used video-to-motion reconstruction system | [Project](https://wham.is.tue.mpg.de/) |
| GVHMR | Human motion recovery | World-grounded motion recovery from video | [Paper](https://arxiv.org/abs/2409.06661) |
| TRAM | Human trajectory recovery | Global trajectory reconstruction for video-derived motion | [Paper](https://arxiv.org/abs/2403.17346) |
| HybrIK | Human pose estimation | Real-time pose estimation pipeline used in teleoperation and imitation | [Paper](https://arxiv.org/abs/2011.14672) / [Code](https://github.com/jeffffffli/HybrIK) |
| Retargeting Matters (GMR) | Retargeting | General motion retargeting reference for humanoids | [Paper](https://arxiv.org/abs/2510.02252) |
| OmniRetarget | Retargeting | Interaction-preserving retargeting and data generation | [Paper](https://arxiv.org/abs/2509.26633) |
| Implicit Kinodynamic Motion Retargeting | Retargeting | Learned implicit retargeting with dynamics awareness | [Paper](https://arxiv.org/abs/2509.15443) |
| FLD | Motion representation | Latent motion representation useful for structured control | [Paper](https://arxiv.org/abs/2402.13820) |
| Diffusion Policy | Action-generation background | Core action diffusion reference for downstream humanoid work | [Paper](https://arxiv.org/abs/2303.04137) |

## Simulators and Open-Source Frameworks

| Resource | Type | Use case | Links |
| --- | --- | --- | --- |
| Isaac Gym | Simulator | High-throughput GPU RL training | [Paper](https://arxiv.org/abs/2108.10470) |
| Isaac Lab | Simulator / framework | Modern Isaac-based multi-modal robot learning stack | [Paper](https://arxiv.org/abs/2511.04831) / [Code](https://github.com/isaac-sim/IsaacLab) |
| MuJoCo | Simulator | High-fidelity contact dynamics and control benchmarking | [Paper](https://ieeexplore.ieee.org/document/6386109) |
| Genesis | Simulator | Emerging unified high-performance simulator | [Paper](https://arxiv.org/abs/2401.01454) |
| HumanoidVerse | Framework | Multi-simulator training and sim-to-real experiments | [Repo](https://github.com/LeCAR-Lab/HumanoidVerse) |
| ProtoMotions3 | Framework | Open-source humanoid simulation and control stack | [Repo](https://github.com/NVLabs/ProtoMotions/) |
| MuJoCo Playground | Framework | Lightweight GPU-accelerated robot learning framework | [Repo](https://github.com/google-deepmind/mujoco_playground) |
| Motion-X | Dataset / code | Practical data and code release for motion learning | [Repo](https://github.com/IDEA-Research/Motion-X) |

## Surveys and Background

| Title | Venue | Year | Role | Links |
| --- | --- | --- | --- | --- |
| Humanoid Locomotion and Manipulation: Current Progress and Challenges in Control, Planning, and Learning | arXiv | 2025 | Broad humanoid survey with control/planning emphasis | [Paper](https://arxiv.org/abs/2501.02116) |
| Learning-based Legged Locomotion: State of the Art and Future Perspectives | IJRR | 2025 | Broader legged-locomotion context | [Paper](https://doi.org/10.1177/02783649241312698) |
| Deep Reinforcement Learning for Robotics: A Survey of Real-World Successes | AAAI | 2025 | Real-world RL context | [Paper](https://doi.org/10.1609/aaai.v39i27.35095) |
| Advancements in Humanoid Robots: A Comprehensive Review and Future Prospects | JAS | 2024 | General humanoid systems overview | [Paper](https://doi.org/10.1109/JAS.2024.124237) |
| Universal Humanoid Motion Representations for Physics-Based Control | arXiv | 2023 | Motion representation background for WBC | [Paper](https://arxiv.org/abs/2310.04582) |
| Perpetual Humanoid Control for Real-time Simulated Avatars | ICCV | 2023 | Physics-based avatar control precursor | [Paper](https://openaccess.thecvf.com/content/ICCV2023/html/Luo_Perpetual_Humanoid_Control_for_Real-time_Simulated_Avatars_ICCV_2023_paper.html) |
| Learning to Walk in Minutes Using Massively Parallel Deep Reinforcement Learning | arXiv | 2022 | Foundational massively parallel RL recipe | [Paper](https://arxiv.org/abs/2109.11978) |
| Learning Transferable Visual Models from Natural Language Supervision | ICML | 2021 | Common multimodal pretraining background | [Paper](https://arxiv.org/abs/2103.00020) |

## Citation

If this repository is useful in your review or implementation work, please cite the accompanying survey:

```text
Xiaoyu Yan, Zhiyu Chen, Yuxuan Fang, Xin Li, Ronghui Li, Zhe Li, Feifei Wu, Zhirui Fang, and Xiu Li*.
A Survey on Learning-Based Whole-Body Control for Humanoid Robots.
```

Pull requests for missing papers, broken links, wrong categorization, or official code releases are welcome.
