[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

# Segment Anything for Videos: A Systematic Survey

> **The first survey for : Segment Anything for Videos: A Systematic Survey.** Chunhui Zhang, Yawen Cui, Weilin Lin, Guanjie Huang, Yan Rong, Li Liu, Shiguang Shan. [[paper](https://github.com/983632847/SAM-for-Videos/blob/main/SAM_for_videos.pdf)] [[project](https://github.com/983632847/SAM-for-Videos)]

> **<p align="justify"> Abstract:** *The recent wave of foundation models has witnessed tremendous success in computer vision (CV) and beyond, with the segment anything model (SAM) having sparked a passion for exploring task-agnostic visual foundation models. Empowered by its remarkable zero-shot generalization, SAM is currently challenging numerous traditional paradigms in CV, delivering extraordinary performance not only in various image segmentation and multi-modal segmentation (e.g., text-to-mask) tasks, but also in the video domain. Additionally, the latest released SAM 2 is once again sparking research enthusiasm in the realm of promptable visual segmentation for both images and videos. However, existing surveys mainly focus on SAM in various image processing tasks, a comprehensive and in-depth review in the video domain is notably absent. To address this gap, this work conducts a systematic review on SAM for videos in the era of foundation models. As the first to review the progress of SAM for videos, this work focuses on its applications to various tasks by discussing its recent advances, and innovation opportunities of developing foundation models on broad applications. We begin with a brief introduction to the background of SAM and video-related research domains. Subsequently, we present a systematic taxonomy that categorizes existing methods into three key areas: video understanding, video generation, and video editing, analyzing and summarizing their advantages and limitations. Furthermore, comparative results of SAM-based and current state-of-the-art methods on representative benchmarks, as well as insightful analysis are offered. Finally, we discuss the challenges faced by current research and envision several future research directions in the field of SAM for video and beyond.* </p>

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
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

### Video Shadow Detection
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

### Deepfake
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

### Miscellaneous
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

#### Audio-Visual Segmentation
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

#### Referring Video Object Segmentation
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

### Domain Specific
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

#### Medical Videos
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |


#### Domain Adaptation
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |


#### Tool Software
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

#### More Directions
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |


## Video Generation
### Video Synthesis
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

### Video Super-Resolution
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

### 3D Reconstruction
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

### Video Dataset Annotation Generation
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |


## Video Editing
### Generic Video Editing
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

### Text Guided Video Editing
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |

### Object Removing
| Title | arXiv | Github | Pub. & Date |
|---|---|---|---|
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |
|[]() | [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)]() | [github]()  | arXiv-2023 |