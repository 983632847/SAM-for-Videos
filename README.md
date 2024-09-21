[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

# Segment Anything for Videos: A Systematic Survey

> **The first survey for : Segment Anything for Videos: A Systematic Survey.** Chunhui Zhang, Yawen Cui, Weilin Lin, Guanjie Huang, Yan Rong, Li Liu, Shiguang Shan. [[ArXiv]](https://arxiv.org/abs/2408.08315)[[ChinaXiv]](https://chinaxiv.org/abs/202408.00019)[[ResearchGate]](https://www.researchgate.net/publication/382737497_Segment_Anything_for_Videos_A_Systematic_Survey)[[Project]](https://github.com/983632847/SAM-for-Videos)[[中文解读]](https://zhuanlan.zhihu.com/p/712807912)

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
- [Video Segmentation](#video-segmentation)
  - [Video Semantic Segmentation](#video-semantic-segmentation)
  - [Video Instance Segmentation](#video-instance-segmentation)
  - [Video Panoptic Segmentation](#video-panoptic-segmentation)
  - [3D Video Segmentation](#3d-video-segmentation)
  - [Audio-Visual Segmentation](#audio-visual-segmentation)
  - [Referring Video Object Segmentation](#referring-video-object-segmentation)
  - [Universal Segmentation](#universal-segmentation)
  
- [Video Detection and Recognition](#video-detection-and-recognition)
  - [Video Object Detection](#video-object-detection)
  - [Video Shadow Detection](#video-shadow-detection)
  - [Video Camouflaged Object Detection](#video-camouflaged-object-detection)
  - [Deepfake Detection](#deepfake-detection)
  - [Video Anomaly Detection](#video-anomaly-detection)
  - [Video Salient Object Detection](#video-salient-object-detection)
  - [Event Detection](#event-detection)
  - [Action Recognition](#action-recognition)
  - [Video Activity and Scene Classification](#video-activity-and-scene-classification) 

- [Video Tracking](#video-tracking)
  - [General Object Tracking](#general-object-tracking)
  - [Open-Vocabulary Tracking](#open-vocabulary-tracking)
  - [Point Tracking](#point-tracking)
  - [Instruction Tracking](#instruction-tracking)
  - [Interactive Tracking and Localization](#interactive-tracking-and-localization)
  - [Domain Specifc Tracking](#domain-specifc-tracking)

- [Video Editing and Generation](#video-editing-and-generation)
  - [Video Editing](#video-editing)
    - [Text Guided Video Editing](#text-guided-video-editing)
    - [Other Modality-guided Video Editing](#other-modality-guided-video-editing)
    - [Domain Spacific Editing](#domain-spacific-editing)
  - [Video Frame Interpolation](#video-frame-interpolation)
  - [3D Video Reconstruction](#3d-video-reconstruction)
  - [Video Dataset Annotation Generation](#video-dataset-annotation-generation)
  - [Video Super-Resolution](#video-super-resolution)
  - [Text-to-Video Generation](#text-to-video-generation)
  - [Video Generation with Other Modalities](#video-generation-with-other-modalities)

- [Video Understanding and Analysis](#video-understanding-and-analysis)
  - [Video Captioning](#video-captioning)
  - [Video Dialog](#video-dialog)
  - [Video Grounding](#video-grounding)
  - [Optical Flow Estimation](#optical-flow-estimation)
  - [Pose Estimation](#pose-estimation)
  - [Video ReID](#video-reid)

- [Medical Video Processing](#medical-video-processing)

- [Other Video Tasks](#other-video-tasks)
  - [Video Compression](#video-compression)
  - [Robotics](#robotics)
  - [Video Game](#video-game)
  - [Video Style Transfer Attack](#video-style-transfer-attack)
  - [Semantic Communication](#semantic-communication)
  - [Tool Software](#tool-software)

## Video Segmentation
### Video Semantic Segmentation
- **PerSAM:** Renrui Zhang, Zhengkai Jiang, Ziyu Guo, Shilin Yan, Junting Pan, Hao Dong, Peng Gao, Hongsheng Li.<br />
  "Personalize Segment Anything Model with One Shot." ArXiv (2023).
  [[paper]( https://arxiv.org/abs/2305.03048)] 
  [[code]( https://github.com/ZrrSkywalker/Personalize-SAM)]
  [2023.05]

 - **UVOSAM:** Zhenghao Zhang, Zhichao Wei, Shengfan Zhang, Zuozhuo Dai, Siyu Zhu.<br />
  "UVOSAM: A Mask-free Paradigm for Unsupervised Video Object Segmentation via Segment Anything Model." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2305.12659)] 
  [2023.05]
 
- **DSEC-MOS:** Zhuyun Zhou, Zongwei Wu, Rémi Boutteau, Fan Yang, Dominique Ginhac.<br />
  "DSEC-MOS: Segment Any Moving Object with Moving Ego Vehicle." ArXiv (2023).
  [[paper]( https://arxiv.org/abs/2305.00126)] 
  [[code]( https://github.com/ZZY-Zhou/DSEC-MOS)]
  [2023.05]

- **Matcher:** Yang Liu, Muzhi Zhu, Hengtao Li, Hao Chen, Xinlong Wang, Chunhua Shen.<br />
  "Matcher: Segment Anything with One Shot Using All-Purpose Feature Matching." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2305.13310)] 
  [[code](https://github.com/aim-uofa/Matcher)]
  [2023.05]
  
-  Shijie Chang, Zeqi Hao, Ben Kang, Xiaoqi Zhao, Jiawen Zhu, Zhenyu Chen, Lihe Zhang, Lu Zhang, Huchuan Lu.<br />
  " 3rd Place Solution for PVUW2023 VSS Track: A Large Model for Semantic Segmentation on VSPW." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2306.02291)] 
  [2023.06]

- **SEGIC:** Lingchen Meng, Shiyi Lan, Hengduo Li, Jose M. Alvarez, Zuxuan Wu, Yu-Gang Jiang.<br />
  "SEGIC: Unleashing the Emergent Correspondence for In-Context Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.14671)] 
  [[code](https://github.com/MengLcool/SEGIC)]
  [2023.11]
  
- **MVS:** Mykhailo Shvets, Dongxu Zhao, Marc Niethammer, Roni Sengupta, Alexander C. Berg.<br />
  "Joint Depth Prediction and Semantic Segmentation with Multi-View SAM." WACV (2024).
  [[paper](https://arxiv.org/abs/2311.00134)] 
  [2023.11]

- **ABR:** Junyu Xie, Weidi Xie, Andrew Zisserman.<br />
  "Appearance-based Refinement for Object-Centric Motion Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.11463)] 
  [2023.12]

- **FoodMem:** Ahmad AlMughrabi, Adrián Galán, Ricardo Marques, Petia Radeva.<br />
  "FoodMem: Near Real-time and Precise Food Video Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2407.12121)] 
  [2024.07]

- **MVP-TIME:** Feiyu Pan, Hao Fang, Runmin Cong, Wei Zhang, Xiankai Lu.<br />
  "Video Object Segmentation via SAM 2: The 4th Solution for LSVOS Challenge VOS Track." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.10125)] 
  [2024.08]

- Xinyu Liu, Jing Zhang, Kexin Zhang, Xu Liu, Lingling Li.<br />
  "LSVOS Challenge 3rd Place Report: SAM2 and Cutie based VOS." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.10469)] 
  [2024.08]
  
  
### Video Instance Segmentation
### Video Panoptic Segmentation
### 3D Video Segmentation
### Audio-Visual Segmentation
### Referring Video Object Segmentation
### Universal Segmentation

## Video Detection and Recognition
### Video Object Detection
### Video Shadow Detection
### Video Camouflaged Object Detection
### Deepfake Detection
### Video Anomaly Detection
### Video Salient Object Detection
### Event Detection
### Action Recognition
### Video Activity and Scene Classification

## Video Tracking
### General Object Tracking
### Open-Vocabulary Tracking
### Point Tracking
### Instruction Tracking
### Interactive Tracking and Localization
### Domain Specifc Tracking

## Video Editing and Generation
### Video Editing
#### Text Guided Video Editing
#### Other Modality-guided Video Editing
#### Domain Spacific Editing
### Video Frame Interpolation
### 3D Video Reconstruction
### Video Dataset Annotation Generation
### Video Super-Resolution
### Text-to-Video Generation
### Video Generation with Other Modalities

## Video Understanding and Analysis
### Video Captioning
### Video Dialog
### Video Grounding
### Optical Flow Estimation
### Pose Estimation
### Video ReID

## Medical Video Processing

## Other Video Tasks
### Video Compression
### Robotics
### Video Game
### Video Style Transfer Attack
### Semantic Communication
### Tool Software

## License
This project is released under the MIT license. Please see the [LICENSE](LICENSE) file for more information.
