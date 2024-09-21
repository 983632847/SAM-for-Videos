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
- **HQ-SAM:** Lei Ke, Mingqiao Ye, Martin Danelljan, Yifan Liu, Yu-Wing Tai, Chi-Keung Tang, Fisher Yu.<br />
  "Segment Anything in High Quality." NeurIPS (2023).
  [[paper](https://arxiv.org/abs/2306.01567)] 
  [[code](https://github.com/SysCV/SAM-HQ)]
  [2023.06]
  
- **RepViT-SAM:** Ao Wang, Hui Chen, Zijia Lin, Jungong Han, Guiguang Ding.<br />
  "RepViT-SAM: Towards Real-Time Segmenting Anything." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.05760)] 
  [[code](https://github.com/THU-MIG/RepViT)]
  [2023.12]
  
- **SAM-PD:** Tao Zhou, Wenhan Luo, Qi Ye, Zhiguo Shi, Jiming Chen.<br />
  "SAM-PD: How Far Can SAM Take Us in Tracking and Segmenting Anything in Videos by Prompt Denoising." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.04194)] 
  [[code](https://github.com/infZhou/SAM-PD)]
  [2024.03]
    
- **ClickVOS:** Pinxue Guo, Lingyi Hong, Xinyu Zhou, Shuyong Gao, Wanyun Li, Jinglun Li, Zhaoyu Chen, Xiaoqiang Li, Wei Zhang, Wenqiang Zhang.<br />
  "ClickVOS: Click Video Object Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.06130)] 
  [[code](https://github.com/PinxueGuo/ClickVOS)]
  [2024.03]

- **PM-VIS:** Zhangjing Yang, Dun Liu, Wensheng Cheng, Jinqiao Wang, Yi Wu.<br />
  "PM-VIS: High-Performance Box-Supervised Video Instance Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.13863)] 
  [2024.04]
    
- **OW-VISCap:** Anwesa Choudhuri, Girish Chowdhary, Alexander G. Schwing.<br />
  "OW-VISCap: Open-World Video Instance Segmentation and Captioning." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.03657)] 
  [[code](https://anwesachoudhuri.github.io/OpenWorldVISCap/)]
  [2024.04]
  
- **FlowSAM:** Junyu Xie, Charig Yang, Weidi Xie, Andrew Zisserman.<br />
  "Moving Object Segmentation: All You Need Is SAM (and Flow)." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.12389)] 
  [[code](https://www.robots.ox.ac.uk/~vgg/research/flowsam/)]
  [2024.04]
  
- **ASDeM:** Liu, Xiaohu and Luo, Yichuang and Sun, Wei.<br />
  "ASDeM: Augmenting SAM With Decoupled Memory for Video Object Segmentation." ACCESS (2024).
  [[paper](https://ieeexplore.ieee.org/abstract/document/10537204)] 
  [2024.06]

- **MouseSIS:** Friedhelm Hamann, Hanxiong Li, Paul Mieske, Lars Lewejohann, Guillermo Gallego.<br />
  "MouseSIS: A Frames-and-Events Dataset for Space-Time Instance Segmentation of Mice." ECCVW (2024).
  [[paper](https://arxiv.org/abs/2409.03358)] 
  [[code](https://github.com/tub-rip/MouseSIS)]
  [2024.09]
  
### Video Panoptic Segmentation
- **DEVA:** Ho Kei Cheng, Seoung Wug Oh, Brian Price, Alexander Schwing, Joon-Young Lee.<br />
  "Tracking Anything with Decoupled Video Segmentation." ICCV (2023).
  [[paper](https://arxiv.org/abs/2309.03903)] 
  [[project page](https://hkchengrex.com/Tracking-Anything-with-DEVA/)]
  [[code](https://github.com/hkchengrex/Tracking-Anything-with-DEVA)]
  [2023.09] 

- **CRSTM:** Xiaoli Wei, Zhaoqing Wang, Yandong Guo, Chunxia Zhang, Tongliang Liu, Mingming Gong.<br />
  "Training-Free Robust Interactive Video Object Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2406.05485)] 
  [2024.06]

  
### 3D Video Segmentation
- **CSF:** Shichao Dong, Fayao Liu, Guosheng Lin.<br />
  "Leveraging Large-Scale Pretrained Vision Foundation Models for Label-Efficient 3D Point Cloud Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.01989)] 
  [2023.11]

- **SAMPro3D:** Mutian Xu, Xingyilang Yin, Lingteng Qiu, Yang Liu, Xin Tong, Xiaoguang Han.<br />
  "SAMPro3D: Locating SAM Prompts in 3D for Zero-Shot Scene Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.17707)] 
  [[code](https://mutianxu.github.io/sampro3d/)]
  [2023.11]

- **SANeRF-HQ:** Yichen Liu, Benran Hu, Chi-Keung Tang, Yu-Wing Tai.<br />
  "SANeRF-HQ: Segment Anything for NeRF in High Quality." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.01531)] 
  [[code](https://lyclyc52.github.io/SANeRF-HQ/)]
  [2023.12]

- **Open3DIS:** Phuc D.A. Nguyen, Tuan Duc Ngo, Chuang Gan, Evangelos Kalogerakis, Anh Tran, Cuong Pham, Khoi Nguyen.<br />
  "Open3DIS: Open-vocabulary 3D Instance Segmentation with 2D Mask Guidance." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.10671)] 
  [[code](https://open3dis.github.io/)]
  [2023.12]

- **EgoLifter:** Qiao Gu, Zhaoyang Lv, Duncan Frost, Simon Green, Julian Straub, Chris Sweeney.<br />
  "EgoLifter: Open-world 3D Segmentation for Egocentric Perception." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.18118)] 
  [[code](https://egolifter.github.io/)]
  [2024.03]
      
- **3DSAM:** Shangjie Wang; Yan Zhang.<br />
  "3DSAM: Segment Anything in NeRF." ICASSP (2024).
  [[paper](https://ieeexplore.ieee.org/abstract/document/10445897)] 
  [2024.04]

- **SAM2Point:** Ziyu Guo, Renrui Zhang, Xiangyang Zhu, Chengzhuo Tong, Peng Gao, Chunyuan Li, Pheng-Ann Heng.<br />
  "SAM2Point: Segment Any 3D as Videos in Zero-shot and Promptable Manners." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.16768)] 
  [[code](https://github.com/ZiyuGuo99/SAM2Point)]
  [2024.08]
  
### Audio-Visual Segmentation
- **AV-SAM:** Shentong Mo, Yapeng Tian.<br />
  "AV-SAM: Segment Anything Model Meets Audio-Visual Localization and Segmentation." ArXiv (2023).
  [[paper]( https://arxiv.org/abs/2305.01836)]
  [2023.05]
  
- **CMSF:** Swapnil Bhosale, Haosen Yang, Diptesh Kanojia, Xiatian Zhu.<br />
  "Leveraging Foundation models for Unsupervised Audio-Visual Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2309.06728)] 
  [2023.09]
  
- **GAVS:** Yaoting Wang, Weisong Liu, Guangyao Li, Jian Ding, Di Hu, Xi Li.<br />
  "Prompting Segmentation with Sound is Generalizable Audio-Visual Source Localizer." AAAI (2024).
  [[paper](https://arxiv.org/abs/2309.07929)] 
  [2023.09]
    
- **COMBO:** Qi Yang, Xing Nie, Tong Li, Pengfei Gao, Ying Guo, Cheng Zhen, Pengfei Yan, Shiming Xiang.<br />
  "Cooperation Does Matter: Exploring Multi-Order Bilateral Relations for Audio-Visual Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.06462)] 
  [[code](https://combo-avs.github.io/)]
  [2023.12]
  
- **MoCA:** Swapnil Bhosale, Haosen Yang, Diptesh Kanojia, Jiangkang Deng, Xiatian Zhu.<br />
  "Unsupervised Audio-Visual Segmentation with Modality Alignment." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.14203)] 
  [2024.03]
  
- **ST-BAVA:** Juhyeong Seon, Woobin Im, Sebin Lee, Jumin Lee, Sung-Eui Yoon.<br />
  "Extending Segment Anything Model into Auditory and Temporal Dimensions for Audio-Visual Segmentation." ICIP  (2024).
  [[paper](https://arxiv.org/abs/2406.06163)] 
  [2024.06]

- **SAVE:** Khanh-Binh Nguyen, Chae Jung Park.<br />
  "SAVE: Segment Audio-Visual Easy way using Segment Anything Model." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2407.02004)] 
  [2024.07]

    
### Referring Video Object Segmentation
- **RefSAM:** Yonglin Li, Jing Zhang, Xiao Teng, Long Lan, Xinwang Liu.<br />
  "RefSAM: Efficiently Adapting Segmenting Anything Model for Referring Video Object Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2307.00997)] 
  [[code](https://github.com/LancasterLi/RefSAM)]
  [2023.07]

- **UniRef++:** Jiannan Wu, Yi Jiang, Bin Yan, Huchuan Lu, Zehuan Yuan, Ping Luo.<br />
  "UniRef++: Segment Every Reference Object in Spatial and Temporal Spaces." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.15715)] 
  [[code](https://github.com/FoundationVision/UniRef)]
  [2023.12]
  
- **PDM:** Dvir Samuel, Rami Ben-Ari, Matan Levy, Nir Darshan, Gal Chechik.<br />
  "Unveiling the Power of Diffusion Features For Personalized Segmentation and Retrieval." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2405.18025)] 
  [2024.06]
      
- **ROSA:** Yuhan Shen, Huiyu Wang, Xitong Yang, Matt Feiszli, Ehsan Elhamifar, Lorenzo Torresani, Effrosyni Mavroudi.<br />
  "Learning to Segment Referred Objects from Narrated Egocentric Videos." CVPR (2024).
  [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Shen_Learning_to_Segment_Referred_Objects_from_Narrated_Egocentric_Videos_CVPR_2024_paper.html)] 
  [2024.06]
  
- **MUTR:** Bin Cao, Yisi Zhang, Xuanxu Lin, Xingjian He, Bo Zhao, Jing Liu.<br />
  "2nd Place Solution for MeViS Track in CVPR 2024 PVUW Workshop: Motion Expression guided Video Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2406.13939)] 
  [2024.06]

- **TeSO:** Yaoting Wang, Peiwen Sun, Yuanchao Li, Honggang Zhang, Di Hu.<br />
  "Can Textual Semantics Mitigate Sounding Object Segmentation Preference?." ECCV (2024).
  [[paper](https://arxiv.org/abs/2407.10947)] 
  [[code](https://github.com/GeWu-Lab/Sounding-Object-Segmentation-Preference)]
  [2024.07]
  
- **VISA:** Cilin Yan, Haochen Wang, Shilin Yan, Xiaolong Jiang, Yao Hu, Guoliang Kang, Weidi Xie, Efstratios Gavves.<br />
  "VISA: Reasoning Video Object Segmentation via Large Language Models." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2407.11325)] 
  [[code](https://github.com/cilinyan/VISA)]
  [2024.07]
  
- Tuyen Tran.<br />
  "The 2nd Solution for LSVOS Challenge RVOS Track: Spatial-temporal Refinement for Consistent Semantic Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.12447)] 
  [2024.08]

- Bin Cao, Yisi Zhang, Hanyi Wang, Xingjian He, Jing Liu.<br />
  "The Instance-centric Transformer for the RVOS Track of LSVOS Challenge: 3rd Place Solution." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.10541)] 
  [2024.08]
  
### Universal Segmentation
- **UniLSeg:** Yong Liu, Cairong Zhang, Yitong Wang, Jiahao Wang, Yujiu Yang, Yansong Tang.<br />
  "Universal Segmentation at Arbitrary Granularity with Language Instruction." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.01623)] 
  [[code](https://github.com/workforai/UniLSeg)]
  [2023.12]
  
- **OMG-Seg:** Xiangtai Li, Haobo Yuan, Wei Li, Henghui Ding, Size Wu, Wenwei Zhang, Yining Li, Kai Chen, Chen Change Loy.<br />
  "OMG-Seg: Is One Model Good Enough For All Segmentation?." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2401.10229)] 
  [[code](https://github.com/lxtGH/OMG-Seg)]
  [2024.01]


  
## Video Detection and Recognition
### Video Object Detection
- Marian Longa, João F. Henriques.<br />
  "Unsupervised Object Detection with Theoretical Guarantees." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2406.07284)] 
  [2024.06]

### Video Shadow Detection
- **ShadowSAM:** Yonghui Wang, Wengang Zhou, Yunyao Mao, Houqiang Li.<br />
  "Detect Any Shadow: Segment Anything for Video Shadow Detection." TCSVT (2023).
  [[paper]( https://arxiv.org/abs/2305.16698)] 
  [[code](https://github.com/harrytea/Detect-AnyShadow)]
  [2023.05]

### Video Camouflaged Object Detection
  - **TSP-SAM:** Wenjun Hui, Zhenfeng Zhu, Shuai Zheng, Yao Zhao.<br />
  "Endow SAM with Keen Eyes: Temporal-spatial Prompt Learning for Video Camouflaged Object Detection." CVPR (2024).
  [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Hui_Endow_SAM_with_Keen_Eyes_Temporal-spatial_Prompt_Learning_for_Video_CVPR_2024_paper.html)] 
  [2024.06]

- **SAM-PM:** Muhammad Nawfal Meeran, Gokul Adethya T, Bhanu Pratyush Mantha.<br />
  "SAM-PM: Enhancing Video Camouflaged Object Detection using Spatio-Temporal Attention." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2406.05802)] 
  [[code](https://github.com/SpiderNitt/SAM-PM)]
  [2024.06]

### Deepfake Detection
- **DADF:** Yingxin Lai, Zhiming Luo, Zitong Yu.<br />
  "Detect Any Deepfakes: Segment Anything Meets Face Forgery Detection and Localization." Chinese Conference on Biometric Recognition (2023).
  [[paper](https://arxiv.org/abs/2306.17075)] 
  [[code](https://github.com/laiyingxin2/DADF)]
  [2023.06]

- **LandmarkBreaker:** Yuezun Li and Pu Sun and Honggang Qi and Siwei Lyu.<br />
  "LandmarkBreaker: A proactive method to obstruct DeepFakes via disrupting facial landmark extraction." CVIU (2024).
  [[paper](https://www.sciencedirect.com/science/article/pii/S107731422400016X)] 
  [2024.01]

### Video Anomaly Detection
- Hangbin Zheng, Shimin Liu, Hengjun Zhang, Jiayi Yu and Jinsong Bao.<br />
  "Visual-triggered contextual guidance for lithium battery disassembly: a multi-modal event knowledge graph approach." ArXiv (2024).
  [[paper](https://www.tandfonline.com/doi/pdf/10.1080/09544828.2024.2301876?casa_token=7COSjhYxn_8AAAAA:VPlW-3ISu60vumHZ-FaQsA5ToOmw-FPtL2nrBYZLhq0kdvPjeSNFnxIOYpgRcMBUEY7SMIxuIwQ1eIAu)] 
  [2024.01]
  
- **DecoAD:** Chenglizhao Chen, Xinyu Liu, Mengke Song, Luming Li, Xu Yu, Shanchen Pang.<br />
  "Unveiling Context-Related Anomalies: Knowledge Graph Empowered Decoupling of Scene and Action for Human-Related Video Anomaly Detection." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.03236)] 
  [[code](https://github.com/liuxy3366/DecoAD)]
  [2024.09]
  
### Video Salient Object Detection
- Xu, Binwei and Jiang, Qiuping and Zhao, Xing and Lu, Chenyang and Liang, Haoran and Liang, Ronghua.<br />
  "Multidimensional Exploration of Segment Anything Model for Weakly Supervised Video Salient Object Detection." TCSVT  (2024).
  [[paper](https://ieeexplore.ieee.org/document/10443051)] 
  [2024.02]

### Event Detection
- **SAM-GEBD:** Pranay Kashyap; Sourabh Vasant Gothe; Vibhav Agarwal; Jayesh Rajkumar Vachhani.<br />
  "SAM-GEBD: Zero-Cost Approach for Generic Event Boundary Detection." ICASSP (2024).
  [[paper](https://ieeexplore.ieee.org/abstract/document/10447789)] 
  [2024.04]
  
### Action Recognition
- **Annolid:** Chen Yang, Jeremy Forest, Matthew Einhorn, Thomas A. Cleland.<br />
  "Automated Behavioral Analysis Using Instance Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.07723)] 
  [[code](https://github.com/cplab/annolid)]
  [2023.12]
  
- **FBM:** Huang, Peng and Shu, Xiangbo and Yan, Rui and Tu, Zhewei and Tang, Jinhui.<br />
  "Appearance-Agnostic Representation Learning for Compositional Action Recognition." TCSVT (2024).
  [[paper](https://ieeexplore.ieee.org/abstract/document/10488474)] 
  [2024.04]

### Video Activity and Scene Classification
- Fengtian Lu, Yuzhi Li, Feng Tian.<br />
  "Exploring challenge and explainable shot type classification using SAM-guided approaches." SIVP (2024).
  [[paper](https://link.springer.com/article/10.1007/s11760-023-02928-x)] 
  [2024.01]

- **SAM+SLIC:** Michal Shlapentokh-Rothman, Ansel Blume, Yao Xiao, Yuqun Wu, Sethuraman T V, Heyi Tao, Jae Yong Lee, Wilfredo Torres, Yu-Xiong Wang, Derek Hoiem.<br />
  "Region-Based Representations Revisited." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2402.02352)] 
  [2024.02]

## Video Tracking
### General Object Tracking
- **MSDeAOT:** Yuanyou Xu, Jiahao Li, Zongxin Yang, Yi Yang, Yueting Zhuang.<br />
  "ZJU ReLER Submission for EPIC-KITCHEN Challenge 2023: TREK-150 Single Object Tracking." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2307.02508)] 
  [2023.07]
  
- **MASA:** Siyuan Li, Lei Ke, Martin Danelljan, Luigi Piccinelli, Mattia Segu, Luc Van Gool, Fisher Yu.<br />
  "Matching Anything by Segmenting Anything." CVPR (2024).
  [[paper](https://arxiv.org/abs/2406.04221)] 
  [[project](https://matchinganything.github.io/)]
  [[code](https://github.com/siyuanliii/masa)]
  [2024.06]
  
- **HQTrack:** Jiawen Zhu, Zhenyu Chen, Zeqi Hao, Shijie Chang, Lu Zhang, Dong Wang, Huchuan Lu, Bin Luo, Jun-Yan He, Jin-Peng Lan, Hanyuan Chen, Chenyang Li.<br />
  "Tracking Anything in High Quality." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2307.13974)] 
  [[code](https://github.com/jiawen-zhu/HQTrack)]
  [2023.07]

### Open-Vocabulary Tracking
- **OVTracktor:** Wen-Hsuan Chu, Adam W. Harley, Pavel Tokmakov, Achal Dave, Leonidas Guibas, Katerina Fragkiadaki.<br />
  "Zero-Shot Open-Vocabulary Tracking with Large Pre-Trained Models." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2310.06992)] 
  [[code](https://wenhsuanchu.github.io/ovtracktor/)]
  [2023.10]
  
### Point Tracking
- **SAM-PT:** Frano Rajič, Lei Ke, Yu-Wing Tai, Chi-Keung Tang, Martin Danelljan, Fisher Yu.<br />
  "Segment Anything Meets Point Tracking." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2307.01197)] 
  [[code](https://github.com/SysCV/sam-pt)]
  [2023.07]

### Instruction Tracking
- **TrackGPT:** Jiawen Zhu, Zhi-Qi Cheng, Jun-Yan He, Chenyang Li, Bin Luo, Huchuan Lu, Yifeng Geng, Xuansong Xie.<br />
  "Tracking with Human-Intent Reasoning." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.17448)] 
  [[code](https://github.com/jiawen-zhu/TrackGPT)]
   [2023.12]
  
### Interactive Tracking and Localization
- **TAM:** Jinyu Yang, Mingqi Gao, Zhe Li, Shang Gao, Fangjing Wang, Feng Zheng.<br />
  "Track Anything: Segment Anything Meets Videos." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2304.11968)] 
  [[code](https://github.com/gaomingqi/Track-Anything)]
  [2023.04]

- **SAM-Track:** Yangming Cheng, Liulei Li, Yuanyou Xu, Xiaodi Li, Zongxin Yang, Wenguan Wang, Yi Yang.<br />
  "Segment and Track Anything." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2305.06558)] 
  [[code](https://github.com/z-x-yang/Segment-and-Track-Anything)]
  [2023.05]

- **FIND:** Xueyan Zou, Linjie Li, Jianfeng Wang, Jianwei Yang, Mingyu Ding, Zhengyuan Yang, Feng Li, Hao Zhang, Shilong Liu, Arul Aravinthan, Yong Jae Lee, Lijuan Wang.<br />
  "Interfacing Foundation Models’ Embeddings." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.07532)] 
  [[code](https://github.com/UX-Decoder/FIND)]
  [2023.12]
  
### Domain Specifc Tracking
- Xiao Yang, Haixing Dai, Zihao Wu, Ramesh Bist, Sachin Subedi, Jin Sun, Guoyu Lu, Changying Li, Tianming Liu, Lilong Chai.<br />
  "SAM for Poultry Science." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2305.10254)] 
  [2023.05]
  
- **SAM-DA:** Liangliang Yao, Haobo Zuo, Guangze Zheng, Changhong Fu, Jia Pan.<br />
  "SAM-DA: UAV Tracks Anything at Night with SAM-Powered Domain Adaptation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2307.01024)] 
  [[code](https://github.com/vision4robotics/SAM-DA)]
  [2023.07]
  
- **FAn:** Alaa Maalouf, Ninad Jadhav, Krishna Murthy Jatavallabhula, Makram Chahine, Daniel M. Vogt, Robert J. Wood, Antonio Torralba, Daniela Rus.<br />
  "Follow Anything: Open-set detection, tracking, and following in real-time." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2308.05737)] 
  [[code](https://github.com/alaamaalouf/FollowAnything)]
  [[demo](https://www.youtube.com/watch?v=6Mgt3EPytrw)]
  [2023.08]

- **UniQuadric:** Linghao Yang, Yanmin Wu, Yu Deng, Rui Tian, Xinggang Hu, Tiefeng Ma.<br />
  "UniQuadric: A SLAM Backend for Unknown Rigid Object 3D Tracking and Light-Weight Modeling." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2309.17036)] 
  [2023.09]
  
- Alessandro Saviolo, Pratyaksh Rao, Vivek Radhakrishnan, Jiuhong Xiao, Giuseppe Loianno.<br />
  "Unifying Foundation Models with Quadrotor Control for Visual Tracking Beyond Object Categories." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2310.04781)] 
  [2023.10]

- Virmarie Maquiling, Sean Anthony Byrne, Diederick C. Niehorster, Marcus Nyström, Enkelejda Kasneci.<br />
  "Zero-Shot Segmentation of Eye Features Using the Segment Anything Model (SAM)." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.08077)] 
  [2023.11]

- **IT3DEgo:** Yunhan Zhao, Haoyu Ma, Shu Kong, Charless Fowlkes.<br />
  "Instance Tracking in 3D Scenes from Egocentric Videos." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.04117)] 
  [[code](https://github.com/IT3DEgo/IT3DEgo/)]
  [2023.12]

- **TrafficMOT:** Lihao Liu, Yanqi Cheng, Zhongying Deng, Shujun Wang, Dongdong Chen, Xiaowei Hu, Pietro Liò, Carola-Bibiane Schönlieb, Angelica Aviles-Rivero.<br />
  "TrafficMOT: A Challenging Dataset for Multi-Object Tracking in Complex Traffic Scenarios." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.18839)] 
  [2023.12]

- **HOIST-Former:** Supreeth Narasimhaswamy, Huy Anh Nguyen, Lihan Huang, Minh Hoai.<br />
  "HOIST-Former: Hand-held Objects Identification, Segmentation, and Tracking in the Wild." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.13819)] 
  [[code](https://supreethn.github.io/research/hoistformer/index.html)]
  [2024.04]

- **Offline-evt:** Fangwei Zhong, Kui Wu, Hai Ci, Churan Wang, Hao Chen.<br />
  "Empowering Embodied Visual Tracking with Visual Foundation Models and Offline RL." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.09857)] 
  [[code](https://sites.google.com/view/offline-evt)]
  [2024.04]

- **TAR:** Tharun V. Puthanveettil, Fnu Obaid ur Rahman.<br />
  "Track Anything Rapter(TAR)." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2405.11655)] 
  [[code](https://github.com/tvpian/Project-TAR)]
  [2024.05]

- **SAM-TAPIR:** Athena Psalta, Vasileios Tsironis, Andreas El Saer, Konstantinos Karantzalos.<br />
  "Addressing single object tracking in satellite imagery through prompt-engineered solutions." IGARSS (2024).
  [[paper](https://arxiv.org/abs/2407.05518)] 
  [2024.07]



## Video Editing and Generation
### Video Editing
#### Text Guided Video Editing
- **TGVE:** Jay Zhangjie Wu, Xiuyu Li, Difei Gao, Zhen Dong, Jinbin Bai, Aishani Singh, Xiaoyu Xiang, Youzeng Li, Zuwei Huang, Yuanxi Sun, Rui He, Feng Hu, Junhua Hu, Hai Huang, Hanyu Zhu, Xu Cheng, Jie Tang, Mike Zheng Shou, Kurt Keutzer, Forrest Iandola.<br />
  "CVPR 2023 Text Guided Video Editing Competition." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2310.16003)] 
  [[code](https://sites.google.com/view/loveucvpr23/track4)]
  [2023.10]

- **SAVE:** Yeji Song, Wonsik Shin, Junsoo Lee, Jeesoo Kim, Nojun Kwak.<br />
  "SAVE: Protagonist Diversification with Structure Agnostic Video Editing." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.02503)] 
  [[code](https://ldynx.github.io/SAVE/)]
  [2023.12]

- **ReimaginedAct:** Lan Wang, Vishnu Boddeti, Sernam Lim.<br />
  "Action Reimagined: Text-to-Pose Video Editing for Dynamic Human Actions." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.07198)] 
  [2024.03]

#### Other Modality-guided Video Editing
- **Make-A-Protagonist:** Yuyang Zhao, Enze Xie, Lanqing Hong, Zhenguo Li, Gim Hee Lee.<br />
  "Make-A-Protagonist: Generic Video Editing with An Ensemble of Experts." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2305.08850)] 
  [[code](https://make-a-protagonist.github.io/)]
  [2023.05]
  
- **OR-NeRF:** Youtan Yin, Zhoujie Fu, Fan Yang, Guosheng Lin.<br />
  "OR-NeRF: Object Removing from 3D Scenes Guided by Multiview Segmentation with Neural Radiance Fields." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2305.10503)] 
  [2023.05]
  
- **Drag-A-Video:** Yao Teng, Enze Xie, Yue Wu, Haoyu Han, Zhenguo Li, Xihui Liu.<br />
  "Drag-A-Video: Non-rigid Video Editing with Point-based Interaction." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.02936)] 
  [[code](https://drag-a-video.github.io/)]
  [2023.12]

- Zhan, Youyi and Wang, Tuanfeng Y. and Shao, Tianjia and Zhou, Kun.<br />
  "Pattern Guided UV Recovery for Realistic Video Garment Texturing." ArXiv (2024).
  [[paper](https://ieeexplore.ieee.org/abstract/document/10400917?casa_token=9UPxBTineFYAAAAA:WM3NcynIUd8rFkPE8GUzl5uh5ryqCkHgBsOR8wG3iPrClzFJ1E8hlPir_G0IQkw_I8A8BPq4Lo6X)] 
  [2024.01]


#### Domain Spacific Editing
- **OR-NeRF:** Youtan Yin, Zhoujie Fu, Fan Yang, Guosheng Lin.<br />
  "OR-NeRF: Object Removing from 3D Scenes Guided by Multiview Segmentation with Neural Radiance Fields." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2305.10503)] 
  [2023.05]
  
- **Gaussian Grouping:** Mingqiao Ye, Martin Danelljan, Fisher Yu, Lei Ke.<br />
  "Gaussian Grouping: Segment and Edit Anything in 3D Scenes." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.00732)] 
  [[code](https://github.com/lkeab/gaussian-grouping)]
  [2023.12]
  
- **Diffusion Handles:** Karran Pandey, Paul Guerrero, Matheus Gadelha, Yannick Hold-Geoffroy, Karan Singh, Niloy Mitra.<br />
  "Diffusion Handles: Enabling 3D Edits for Diffusion Models by Lifting Activations to 3D." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.02190)] 
  [[code](https://diffusionhandles.github.io/)]
  [2023.12]

  
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
