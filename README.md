[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

# Segment Anything for Videos: A Systematic Survey

> **The first survey for : Segment Anything for Videos: A Systematic Survey.** Chunhui Zhang, Yawen Cui, Weilin Lin, Guanjie Huang, Yan Rong, Li Liu, Shiguang Shan. [[Paper]](https://github.com/983632847/SAM-for-Videos/blob/main/SAM_for_videos.pdf)[[ResearchGate]](https://www.researchgate.net/publication/382737497_Segment_Anything_for_Videos_A_Systematic_Survey)[[Project]](https://github.com/983632847/SAM-for-Videos)[[ChinaXiv]](https://chinaxiv.org/abs/202408.00019)[[中文解读]](https://zhuanlan.zhihu.com/p/712807912)

> **<p align="justify"> Abstract:** *The recent wave of foundation models has witnessed tremendous success in computer vision (CV) and beyond, with the segment anything model (SAM) having sparked a passion for exploring task-agnostic visual foundation models. Empowered by its remarkable zero-shot generalization, SAM is currently challenging numerous traditional paradigms in CV, delivering extraordinary performance not only in various image segmentation and multi-modal segmentation (e.g., text-to-mask) tasks, but also in the video domain. Additionally, the latest released SAM 2 is once again sparking research enthusiasm in the realm of promptable visual segmentation for both images and videos. However, existing surveys mainly focus on SAM in various image processing tasks, a comprehensive and in-depth review in the video domain is notably absent. To address this gap, this work conducts a systematic review on SAM for videos in the era of foundation models. As the first to review the progress of SAM for videos, this work focuses on its applications to various tasks by discussing its recent advances, and innovation opportunities of developing foundation models on broad applications. We begin with a brief introduction to the background of SAM and video-related research domains. Subsequently, we present a systematic taxonomy that categorizes existing methods into three key areas: video understanding, video generation, and video editing, analyzing and summarizing their advantages and limitations. Furthermore, comparative results of SAM-based and current state-of-the-art methods on representative benchmarks, as well as insightful analysis are offered. Finally, we discuss the challenges faced by current research and envision several future research directions in the field of SAM for video and beyond.* </p>

> **This project will be continuously updated. We expect to include more state-of-the-arts on SAM for videos.**

> **We welcome authors of related works to submit pull requests and become a contributor to this project.**

> **The first comprehensive SAM survey: A Comprehensive Survey on Segment Anything Model for Vision and Beyond is at [[here]](https://github.com/liliu-avril/Awesome-Segment-Anything).**


## :fire: Highlights
```
- 2024.07.31: The first survey on SAM for videos was online.
- 2024.07.30: The SAM 2 was released.
```

## Citation

If you find our work useful in your research, please consider citing:
```
@article{chunhui2024samforvideos,
  title={Segment Anything for Videos: A Systematic Survey},
  author={Chunhui Zhang, Yawen Cui, Weilin Lin, Guanjie Huang, Yan Rong, Li Liu, Shiguang Shan},
  journal={arXiv},
  year={2024}
}
```

## Contents


- [Video Understanding](#video-understanding)
  - [Video Object Segmentation](#video-object-segmentation)
  - [Video Object Tracking](#video-object-tracking)
  - [Video Shadow Detection](#video-shadow-detection)
  - [Deepfake](#deepfake)
  - [Miscellaneous](#miscellaneous)
    - [Audio-Visual Segmentation](#audio-visual-segmentation)
    - [Referring Video Object Segmentation](#referring-video-object-segmentation)
  - [Domain Specific](#domain-specific)
    - [Medical Videos](#medical-videos)
    - [Domain Adaptation](#domain-adaptation)
    - [Tool Software](#tool-software)
    - [More Directions](#more-directions)

- [Video Generation](#video-generation)
  - [Video Synthesis](#video-synthesis)
  - [Video Super-Resolution](#video-super-resolution)
  - [3D Reconstruction](#3d-reconstruction)
  - [Video Dataset Annotation Generation](#video-dataset-annotation-generation)

- [Video Editing](#video-editing)
  - [Generic Video Editing](#generic-video-editing)
  - [Text Guided Video Editing](#text-guided-video-editing)
  - [Object Removing](#object-removing)


## Video Understanding
### Video Object Segmentation
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[SAM 2: Segment Anything in Images and Videos](https://ai.meta.com/sam2) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://ai.meta.com/research/publications/sam-2-segment-anything-in-images-and-videos/) | [github](https://github.com/facebookresearch/segment-anything-2)  | arXiv-2024 |
|[Segment Anything in High Quality](https://arxiv.org/abs/2306.01567) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.01567) | [github](https://github.com/SysCV/SAM-HQ)  | NeurIPS-2023 |
|[High-Quality Entity Segmentation](https://github.com/qqlu/Entity/tree/main/Entityv2) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://openaccess.thecvf.com/content/ICCV2023/html/Qi_High_Quality_Entity_Segmentation_ICCV_2023_paper.html) | [github](https://github.com/qqlu/Entity/blob/main/Entityv2/README.md)  | ICCV-2023 |
|[Tracking Anything with Decoupled Video Segmentation](https://hkchengrex.com/Tracking-Anything-with-DEVA/) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.03903) | [github](https://github.com/hkchengrex/Tracking-Anything-with-DEVA)  | ICCV-2023 |
|[DSEC-MOS: Segment Any Moving Object with Moving Ego Vehicle](https://arxiv.org/abs/2305.00126) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.00126) | [github](https://github.com/ZZY-Zhou/DSEC-MOS)  | arXiv-2023 |
|[Matcher: Segment Anything with One Shot Using All-Purpose Feature Matching](https://arxiv.org/abs/2305.13310) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.13310) | [github](https://github.com/aim-uofa/Matcher)  | arXiv-2023 |
|[Personalize Segment Anything Model with One Shot](https://arxiv.org/abs/2305.03048) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.03048) | [github](https://github.com/ZrrSkywalker/Personalize-SAM)  | arXiv-2023 |
|[UVOSAM: A Mask-free Paradigm for Unsupervised Video Object Segmentation via Segment Anything Model](https://arxiv.org/abs/2305.12659) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.12659) | - | arXiv-2023 |
|[3rd Place Solution for PVUW2023 VSS Track: A Large Model for Semantic Segmentation on VSPW](https://arxiv.org/abs/2306.02291) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.02291) | - | arXiv-2023 |

### Video Object Tracking
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
| [Matching Anything by Segmenting Anything](https://arxiv.org/abs/2406.04221) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2406.04221) | [github](https://github.com/siyuanliii/masa) | CVPR-2024
|[Tracking Anything in High Quality](https://arxiv.org/abs/2307.13974) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.13974) | [github](https://github.com/jiawen-zhu/HQTrack)  | arXiv-2023 |
|[Tracking Anything with Decoupled Video Segmentation](https://hkchengrex.com/Tracking-Anything-with-DEVA/) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.03903) | [github](https://github.com/hkchengrex/Tracking-Anything-with-DEVA)  | ICCV-2023 |
|[Segment and Track Anything](https://arxiv.org/abs/2305.06558) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.06558) | [github](https://github.com/z-x-yang/Segment-and-Track-Anything)  | arXiv-2023 |
|[Segment Anything Meets Point Tracking](https://arxiv.org/abs/2307.01197) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.01197) | [github](https://github.com/SysCV/sam-pt)  | arXiv-2023 |
|[Track Anything: Segment Anything Meets Videos](https://arxiv.org/abs/2304.11968) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2304.11968) | [github](https://github.com/gaomingqi/Track-Anything)  | arXiv-2023 |
|[SAM-DA: UAV Tracks Anything at Night with SAM-Powered Domain Adaptation](https://arxiv.org/abs/2307.01024) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.01024) | [github](https://github.com/vision4robotics/SAM-DA)  | arXiv-2023 |
|[Unifying Foundation Models with Quadrotor Control for Visual Tracking Beyond Object Categories](https://arxiv.org/abs/2310.04781) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.04781) |-  | arXiv-2023 |
|[UniQuadric: A SLAM Backend for Unknown Rigid Object 3D Tracking and Light-Weight Modeling](https://arxiv.org/abs/2309.17036) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.17036) |- | arXiv-2023 |
|[Zero-Shot Open-Vocabulary Tracking with Large Pre-Trained Models](https://arxiv.org/abs/2310.06992) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.06992) | [github](https://wenhsuanchu.github.io/ovtracktor/)  | arXiv-2023 |
|[Follow Anything: Open-set detection, tracking, and following in real-time](https://arxiv.org/abs/2308.05737) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.05737) | [github](https://github.com/alaamaalouf/FollowAnything)  | arXiv-2023 |
|[SAM for Poultry Science](https://arxiv.org/abs/2305.10254) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.10254) | -  | arXiv-2023 |
|[ZJU ReLER Submission for EPIC-KITCHEN Challenge 2023: TREK-150 Single Object Tracking](https://arxiv.org/abs/2307.02508) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.02508) | -  | arXiv-2023 |
|[CoDeF: Content Deformation Fields for Temporally Consistent Video Processing](https://arxiv.org/abs/2308.07926) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.07926) | [github](https://qiuyu96.github.io/CoDeF/)  | arXiv-2023 |


### Video Shadow Detection
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Detect Any Shadow: Segment Anything for Video Shadow Detection](https://arxiv.org/abs/2305.16698) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.16698) | [github](https://github.com/harrytea/Detect-AnyShadow)  | arXiv-2023 |


### Deepfake
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Detect Any Deepfakes: Segment Anything Meets Face Forgery Detection and Localization](https://arxiv.org/abs/2306.17075) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.17075) | [github](https://github.com/laiyingxin2/DADF)  | arXiv-2023 |


### Miscellaneous
#### Audio-Visual Segmentation
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[AV-SAM: Segment Anything Model Meets Audio-Visual Localization and Segmentation](https://arxiv.org/abs/2305.01836) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.01836) | -  | arXiv-2023 |
|[Leveraging Foundation models for Unsupervised Audio-Visual Segmentation](https://arxiv.org/abs/2309.06728) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.06728) |  - | arXiv-2023 |
|[Prompting Segmentation with Sound is Generalizable Audio-Visual Source LocalizerPrompting Segmentation with Sound is Generalizable Audio-Visual Source Localizer](https://arxiv.org/abs/2309.07929) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.07929) |   -  | arXiv-2023 |

#### Referring Video Object Segmentation
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[RefSAM: Efficiently Adapting Segmenting Anything Model for Referring Video Object Segmentation](https://arxiv.org/abs/2307.00997) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.00997) | [github](https://github.com/LancasterLi/RefSAM)  | arXiv-2023 |


### Domain Specific
#### Medical Videos
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Spatio-Temporal Analysis of Patient-Derived Organoid Videos Using Deep Learning for the Prediction of Drug Efficacy](https://arxiv.org/abs/2308.14461) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.14461) | - | ICCV Workshop-2023 |
|[SAM Meets Robotic Surgery: An Empirical Study on Generalization, Robustness and Adaptation](https://arxiv.org/abs/2308.07156) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.07156) | - | MICCAI MedAGI Workshop-2023 |
|[MediViSTA-SAM: Zero-shot Medical Video Analysis with Spatio-temporal SAM Adaptation](https://arxiv.org/abs/2309.13539) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.13539) | [github](https://github.com/kimsekeun/MediViSTA-SAM)  | arXiv-2023 |
|[SAMSNeRF: Segment Anything Model (SAM) Guides Dynamic Surgical Scene Reconstruction by Neural Radiance Field (NeRF)](https://arxiv.org/abs/2308.11774) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.11774) | [github](https://github.com/AngeLouCN/SAMSNeRF)  | arXiv-2023 |
|[SuPerPM: A Large Deformation-Robust Surgical Perception Framework Based on Deep Point Matching Learned from Physical Constrained Simulation Data](https://arxiv.org/abs/2309.13863) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.13863) | -   | arXiv-2023 |
|[SurgicalSAM: Efficient Class Promptable Surgical Instrument Segmentation](https://arxiv.org/abs/2308.08746) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.08746) | [github](https://github.com/wenxi-yue/SurgicalSAM)  | arXiv-2023 |

#### Domain Adaptation
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Learning from SAM: Harnessing a Segmentation Foundation Model for Sim2Real Domain Adaptation through Regularization](https://arxiv.org/abs/2309.15562) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2309.15562) | - | arXiv-2023 |
|[SAM-DA: UAV Tracks Anything at Night with SAM-Powered Domain Adaptation](https://arxiv.org/abs/2307.01024) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.01024) | [github](https://github.com/vision4robotics/SAM-DA)  | arXiv-2023 |


#### Tool Software
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Tool Documentation Enables Zero-Shot Tool-Usage with Large Language Models](https://arxiv.org/abs/2308.00675) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.00675) | -  | arXiv-2023 |


#### More Directions
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Generative AI-driven Semantic Communication Framework for NextG Wireless Network](https://arxiv.org/abs/2310.09021) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.09021) | -  | arXiv-2023 |
|[Learning from Human Videos for Robotic Manipulation](http://reports-archive.adm.cs.cmu.edu/anon/anon/usr/ftp/2023/CMU-CS-23-124.pdf) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](http://reports-archive.adm.cs.cmu.edu/anon/anon/usr/ftp/2023/CMU-CS-23-124.pdf) | [github](https://github.com/adityak77/masters-thesis)  | arXiv-2023 |
|[Leveraging Large-Scale Pretrained Vision Foundation Models for Label-Efficient 3D Point Cloud Segmentation](https://arxiv.org/abs/2311.01989) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.01989) |-  | arXiv-2023 |
|[Pave the Way to Grasp Anything: Transferring Foundation Models for Universal Pick-Place Robots](https://www.youtube.com/watch?v=1m9wNzfp_4E) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.05716) | [github]()  | arXiv-2023 |
|[ROSGPT_Vision: Commanding Robots Using Only Language Models' Prompts](https://arxiv.org/abs/2308.11236) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.11236) | [github](https://github.com/bilel-bj/ROSGPT_Vision)  | arXiv-2023 |
|[SAMFlow: Eliminating Any Fragmentation in Optical Flow with Segment Anything Model](https://arxiv.org/abs/2307.16586) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.16586) | - | arXiv-2023 |
|[Virtual Augmented Reality for Atari Reinforcement Learning](https://arxiv.org/abs/2310.08683) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.08683) | - | arXiv-2023 |


## Video Generation
### Video Synthesis
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Dancing Avatar: Pose and Text-Guided Human Motion Videos Synthesis with Image Diffusion Model](https://arxiv.org/abs/2308.07749) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.07749) | -  | arXiv-2023 |
|[DisCo: Disentangled Control for Realistic Human Dance Generation](https://arxiv.org/abs/2307.00040) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.00040) | [github](https://disco-dance.github.io/)  | arXiv-2023 |


### Video Super-Resolution
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Can SAM Boost Video Super-Resolution?](https://arxiv.org/abs/2305.06524) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.06524) |  | arXiv-2023 |


### 3D Reconstruction
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[SAM3D: Segment Anything in 3D Scenes](https://arxiv.org/abs/2306.03908) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.03908) | [github](https://github.com/Pointcept/SegmentAnything3D)  | arXiv-2023 |
|[A One Stop 3D Target Reconstruction and multilevel Segmentation Method](https://arxiv.org/abs/2308.06974) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2308.06974) | [github](https://github.com/ganlab/OSTRA)  | arXiv-2023 |


### Video Dataset Annotation Generation
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Scalable Mask Annotation for Video Text Spotting](https://arxiv.org/abs/2305.01443) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.01443) | [github](https://github.com/ViTAE-Transformer/SAMText)  | arXiv-2023 |
|[Audio-Visual Instance Segmentation](https://arxiv.org/abs/2310.18709) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.18709) | - | arXiv-2023 |
|[Learning the What and How of Annotation in Video Object Segmentation](https://arxiv.org/abs/2311.04414) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2311.04414) | [github](https://eva-vos.compute.dtu.dk/)  | WACV-2023 |
|[Propagating Semantic Labels in Video Data](https://dataverse.tdl.org/dataverse/robotics) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.00783) | [github](https://dataverse.tdl.org/dataverse/robotics)  | arXiv-2023 |
|[Stable Yaw Estimation of Boats from the Viewpoint of UAVs and USVs](https://arxiv.org/abs/2306.14056) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.14056) | - | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

## Video Editing
### Generic Video Editing
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[Make-A-Protagonist: Generic Video Editing with An Ensemble of Experts](https://arxiv.org/abs/2305.08850) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.08850) | [github](https://make-a-protagonist.github.io/)  | arXiv-2023 |


### Text Guided Video Editing
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[CVPR 2023 Text Guided Video Editing Competition](https://arxiv.org/abs/2310.16003) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2310.16003) | [github](https://sites.google.com/view/loveucvpr23/track4)  | arXiv-2023 |


### Object Removing
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[OR-NeRF: Object Removing from 3D Scenes Guided by Multiview Segmentation with Neural Radiance Fields](https://arxiv.org/abs/2305.10503) | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2305.10503) | -  | arXiv-2023 |

## License
This project is released under the MIT license. Please see the [LICENSE](LICENSE) file for more information.
