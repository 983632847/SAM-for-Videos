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
- 2024.11.22: The latest update of this project.
- 2024.07.31: The first survey on SAM for videos was online.
- 2024.07.29: The SAM 2 was released.
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
  - [Video Object Segmentation](#video-object-segmentation)
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

- [Video Object Tracking](#video-object-tracking)
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
### Video Object Segmentation
- **SAM2-VCOS:** Yuli Zhou, Guolei Sun, Yawei Li, Luca Benini, Ender Konukoglu.<br />
  "When SAM2 Meets Video Camouflaged Object Segmentation: A Comprehensive Evaluation and Adaptation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.18653)] 
  [[code](https://github.com/zhoustan/SAM2-VCOS)]
  [2024.09]

- **VideoSAM:** Pinxue Guo, Zixu Zhao, Jianxiong Gao, Chongruo Wu, Tong He, Zheng Zhang, Tianjun Xiao, Wenqiang Zhang.<br />
  "VideoSAM: Open-World Video Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2410.08781)] 
  [2024.10]

- **SAM2Long:** Shuangrui Ding, Rui Qian, Xiaoyi Dong, Pan Zhang, Yuhang Zang, Yuhang Cao, Yuwei Guo, Dahua Lin, Jiaqi Wang.<br />
  "SAM2Long: Enhancing SAM 2 for Long Video Segmentation with a Training-Free Memory Tree." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2410.16268)] 
  [[code](https://github.com/Mark12Ding/SAM2Long)]
  [2024.10]

- **VideoSAM:** Chika Maduabuchi, Ericmoore Jossou, Matteo Bucci.<br />
"VideoSAM: A Large Vision Foundation Model for High-Speed Video Segmentation." ArXiv (2024).
[[paper](https://arxiv.org/abs/2410.21304)]
[[code](https://github.com/chikap421/videosam)]
[2024.10]
  
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

- **S-AModal:** Jasmin Breitenstein, Franz Jünger, Andreas Bär, Tim Fingscheidt.<br />
  "Foundation Models for Amodal Video Instance Segmentation in Automated Driving." ECCV VCAD Workshop (2024).
  [[paper](https://arxiv.org/abs/2409.14095)] 
  [[code](https://github.com/ifnspaml/S-AModal)]
  [2024.09]

- **MWVOS:** Zhenghao Zhang and Shengfan Zhang and Zuozhuo Dai and Zilong Dong and Siyu Zhu.<br />
"MWVOS: Mask-Free Weakly Supervised Video Object Segmentation via promptable foundation model." Pattern Recognition(2024).
[[paper](https://www.sciencedirect.com/science/article/pii/S0031320324008513)]
[2024.10]

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

- **Sim Anything:** Haoyu Zhao, Hao Wang, Xingyue Zhao, Hongqiu Wang, Zhiyu Wu, Chengjiang Long, Hua Zou.<br />
"Automated 3D Physical Simulation of Open-world Scene with Gaussian Splatting." ArXiv (2024).
[[paper](https://arxiv.org/abs/2411.12789)]
[[code](https://sim-gs.github.io/)]
[2024.11]
  
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

- **AL-Ref-SAM2:** Shaofei Huang, Rui Ling, Hongyu Li, Tianrui Hui, Zongheng Tang, Xiaoming Wei, Jizhong Han, Si Liu.<br />
  "Unleashing the Temporal-Spatial Reasoning Capacity of GPT for Training-Free Audio and Language Referenced Video Object Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.15876)] 
  [[code](https://github.com/appletea233/AL-Ref-SAM2)]
  [2024.08]

- **SAM-SPB:** Zhao, Quan and Wu, Siying and Zhang, Yueyi and Sun, Xiaoyan.<br />
"Semantic-Enhanced Point-Box Joint Prompting for Video Object Segmentation" ICIP (2024).
[paper](https://ieeexplore.ieee.org/abstract/document/10648107?casa_token=CDER8G2ujekAAAAA:q3xlO94oqrLBoVsyHZeAd85YXtRtffZLpLoQiw8nHF8N4zif9UxGlNQEUnbiaZlhxS0kQ34eVa1b)] 
  [2024.09]

- **SAMWISE:** Claudia Cuttano, Gabriele Trivigno, Gabriele Rosi, Carlo Masone, Giuseppe Averta.<br />
"SAMWISE: Infusing wisdom in SAM2 for Text-Driven Video Segmentation." ArXiv (2024).
[[paper](https://arxiv.org/abs/2411.17646)]
[[code](https://github.com/ClaudiaCuttano/SAMWISE)]
[2024.11]


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

- **VideoLISA:** Zechen Bai, Tong He, Haiyang Mei, Pichao Wang, Ziteng Gao, Joya Chen, Lei Liu, Zheng Zhang, Mike Zheng Shou.<br />
  "One Token to Seg Them All: Language Instructed Reasoning Segmentation in Videos." NeurIPS (2024).
  [[paper](https://arxiv.org/abs/2409.19603)] 
  [[code](https://github.com/showlab/VideoLISA)]
  [2024.09]
  
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
  "Region-Based Representations Revisited." CVPR (2024).
  [[paper](https://arxiv.org/abs/2402.02352)]
  [[website](https://regionreps.web.illinois.edu/)]
  [[code](https://github.com/michalsr/regions)]
  [2024.02]

## Video Object Tracking
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

- **SAMURAI:** Cheng-Yen Yang, Hsiang-Wei Huang, Wenhao Chai, Zhongyu Jiang, Jenq-Neng Hwang.<br />
"SAMURAI: Adapting Segment Anything Model for Zero-Shot Visual Tracking with Motion-Aware Memory." ArXiv (2024).
[[paper](https://arxiv.org/abs/2411.11922)]
[[code](https://github.com/yangchris11/samurai)]
[2024.11]

- **GCR:** Kuiran Wang, Xuehui Yu, Wenwen Yu, Guorong Li, Xiangyuan Lan, Qixiang Ye, Jianbin Jiao, Zhenjun Han.<br />
"Click; Single Object Tracking; Video Object Segmentation; Real-time Interaction." ArXiv (2024).
[[paper](https://arxiv.org/abs/2411.13183)]
[2024.11]

- **DAM4SAM:** Jovana Videnovic, Alan Lukezic, Matej Kristan.<br />
"A Distractor-Aware Memory for Visual Object Tracking with SAM2." ArXiv (2024).
[[paper](https://arxiv.org/abs/2411.17576)]
[[code](https://github.com/jovanavidenovic/DAM4SAM)]
[2024.11]

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
  
- **MobileSAM-Track:** Liu, Yehui, Yuliang Zhao, Xinyue Zhang, Xiaoai Wang, Chao Lian, Jian Li, Peng Shan, Changzeng Fu, Xiaoyong Lyu, Lianjiang Li, and et al.<br />
  "MobileSAM-Track: Lightweight One-Shot Tracking and Segmentation of Small Objects on Edge Devices." Remote Sensing (2023).
  [[paper](https://www.mdpi.com/2072-4292/15/24/5665)] 
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

- **UW-COT:** Chunhui Zhang, Li Liu, Guanjie Huang, Hao Wen, Xi Zhou, Yanfeng Wang.<br />
  "Towards Underwater Camouflaged Object Tracking: An Experimental Evaluation of SAM and SAM 2." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.16902)] 
  [[project](https://github.com/983632847/Awesome-Multimodal-Object-Tracking)]

- **TAP:** Jia Syuen Lim, Yadan Luo, Zhi Chen, Tianqi Wei, Scott Chapman, Zi Huang.<br />
"Track Any Peppers: Weakly Supervised Sweet Pepper Tracking Using VLMs." ArXiv (2024).
[[paper](https://arxiv.org/abs/2411.06702)]
[2024.11]


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
  "Gaussian Grouping: Segment and Edit Anything in 3D Scenes." ECCV (2024).
  [[paper](https://arxiv.org/abs/2312.00732)] 
  [[code](https://github.com/lkeab/gaussian-grouping)]
  [2023.12]
  
- **Gaussian Grouping:** Mingqiao Ye, Martin Danelljan, Fisher Yu, Lei Ke.<br />
  "Gaussian Grouping: Segment and Edit Anything in 3D Scenes —– Supplementary Material —." ECCV (2024).
  [[paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/04195-supp.pdf)] 
  [2024.09]
  
- **Diffusion Handles:** Karran Pandey, Paul Guerrero, Matheus Gadelha, Yannick Hold-Geoffroy, Karan Singh, Niloy Mitra.<br />
  "Diffusion Handles: Enabling 3D Edits for Diffusion Models by Lifting Activations to 3D." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.02190)] 
  [[code](https://diffusionhandles.github.io/)]
  [2023.12]

  
### Video Frame Interpolation
- **InterpAny-Clearer:** Zhihang Zhong, Gurunandan Krishnan, Xiao Sun, Yu Qiao, Sizhuo Ma, Jian Wang.<br />
  "Clearer Frames, Anytime: Resolving Velocity Ambiguity in Video Frame Interpolation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.08007)] 
  [[homepage](https://zzh-tech.github.io/InterpAny-Clearer/)]
  [[code](https://github.com/zzh-tech/InterpAny-Clearer)]
  [2023.11]

- **HRFFM:** Yan Han, Xiaogang Xu, Yingqi Lin, Jiafei Wu, Zhe Liu.<br />
  "Video Frame Interpolation with Region-Distinguishable Priors from SAM." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.15868)] 
  [2023.12]

  
### 3D Video Reconstruction
- **SAM3D:** Yunhan Yang, Xiaoyang Wu, Tong He, Hengshuang Zhao, Xihui Liu.<br />
  "SAM3D: Segment Anything in 3D Scenes." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2306.03908)] 
  [[code](https://github.com/Pointcept/SegmentAnything3D)]
  [2023.06]
  
- **OSTRA :** Jiexiong Xu, Weikun Zhao, Zhiyan Tang, Xiangchao Gan.<br />
  "A One Stop 3D Target Reconstruction and multilevel Segmentation Method." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2308.06974)] 
  [[code](https://github.com/ganlab/OSTRA)]
  [2023.08]
  
- **ControlRoom3D:** Jonas Schult, Sam Tsai, Lukas Höllein, Bichen Wu, Jialiang Wang, Chih-Yao Ma, Kunpeng Li, Xiaofang Wang, Felix Wimbauer, Zijian He, Peizhao Zhang, Bastian Leibe, Peter Vajda, Ji Hou.<br />
  "ControlRoom3D: Room Generation using Semantic Proxy Rooms." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.05208)] 
  [[code](https://jonasschult.github.io/ControlRoom3D/)]
  [2023.12]

- **HOLD:** Zicong Fan, Maria Parelli, Maria Eleni Kadoglou, Muhammed Kocabas, Xu Chen, Michael J. Black, Otmar Hilliges.<br />
  "HOLD: Category-agnostic 3D Reconstruction of Interacting Hands and Objects from Video." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.18448)] 
  [[code](https://github.com/zc-alexfan/hold)]
  [2023.12]

- **NPGs:** Devikalyan Das, Christopher Wewer, Raza Yunus, Eddy Ilg, Jan Eric Lenssen.<br />
  "Neural Parametric Gaussians for Monocular Non-Rigid Object Reconstruction." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.01196)] 
  [2023.12]

- **Efficient4D:** Zijie Pan, Zeyu Yang, Xiatian Zhu, Li Zhang.<br />
  "Fast Dynamic 3D Object Generation from a Single-view Video." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2401.08742)] 
  [[code](https://fudan-zvg.github.io/Efficient4D)]
  [2024.01]

- **GVA:** Xinqi Liu, Chenming Wu, Jialun Liu, Xing Liu, Jinbo Wu, Chen Zhao, Haocheng Feng, Errui Ding, Jingdong Wang.<br />
  "GVA: Reconstructing Vivid 3D Gaussian Avatars from Monocular Videos." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2402.16607)] 
  [[code](https://3d-aigc.github.io/GVA/)]
  [2024.02]

- **Uni3DR^2:** Tao Chu, Pan Zhang, Xiaoyi Dong, Yuhang Zang, Qiong Liu, Jiaqi Wang.<br />
  "Unified Scene Representation and Reconstruction for 3D Large Language Models." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.13044)] 
  [[code](https://chtsy.github.io/uni3drr-page/)]
  [2024.04]
  
- **X-Ray:** Tao Hu, Wenhang Ge, Yuyang Zhao, Gim Hee Lee.<br />
  "X-Ray: A Sequential 3D Representation for Generation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.14329)] 
  [2024.04]
    
### Video Dataset Annotation Generation
- **SLP:** David Balaban, Justin Medich, Pranay Gosar, Justin Hart.<br />
  "Propagating Semantic Labels in Video Data." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2310.00783)] 
  [[homepage](https://dataverse.tdl.org/dataverse/robotics)]
  [2023.10]
  
- **AVIS :** Ruohao Guo, Yaru Chen, Yanyu Qi, Wenzhen Yue, Dantong Niu, Xianghua Ying.<br />
  "Audio-Visual Instance Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2310.18709)] 
  [2023.10]
  
- **CoralVOS:** Zheng Ziqiang, Xie Yaofeng, Liang Haixin, Yu Zhibin, Sai-Kit Yeung.<br />
  "CoralVOS: Dataset and Benchmark for Coral Video Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2310.01946)] 
  [2023.10]

- **EVA-VOS:** Thanos Delatolas, Vicky Kalogeiton, Dim P. Papadopoulos.<br />
  "Learning the What and How of Annotation in Video Object Segmentation." WACV  (2023).
  [[paper](https://arxiv.org/abs/2311.04414)] 
  [[code](https://eva-vos.compute.dtu.dk/)]
  [2023.11]
  
- **Emu2:** Quan Sun, Yufeng Cui, Xiaosong Zhang, Fan Zhang, Qiying Yu, Zhengxiong Luo, Yueze Wang, Yongming Rao, Jingjing Liu, Tiejun Huang, Xinlong Wang.<br />
  "Generative Multimodal Models are In-Context Learners." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.13286)] 
  [[homepage](https://baaivision.github.io/emu2)]
  [[code](https://github.com/baaivision/Emu)] 
  [2023.12]

- **MANUS:** Chandradeep Pokhariya, Ishaan N Shah, Angela Xing, Zekun Li, Kefan Chen, Avinash Sharma, Srinath Sridhar.<br />
  "MANUS: Markerless Hand-Object Grasp Capture using Articulated 3D Gaussians." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.02137)] 
  [[code](https://ivl.cs.brown.edu/research/manus.html)]
  [2023.12]

- **Wild2Avatar:** Tiange Xiang, Adam Sun, Scott Delp, Kazuki Kozuka, Li Fei-Fei, Ehsan Adeli.<br />
  "Wild2Avatar: Rendering Humans Behind Occlusions." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2401.00431)] 
  [[code](https://cs.stanford.edu/~xtiange/projects/wild2avatar/)]
   [2023.12]

- **GSC:** Luis Bolanos, Shih-Yang Su, Helge Rhodin.<br />
  "Gaussian Shadow Casting for Neural Characters." ArXiv (2024).  
   [[paper](https://arxiv.org/abs/2401.06116)] 
  [2024.01]
  
- **WildRGB-D:** Hongchi Xia, Yang Fu, Sifei Liu, Xiaolong Wang.<br />
  "RGBD Objects in the Wild: Scaling Real-World 3D Object Learning from RGB-D Videos." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2401.12592)] 
  [[code](https://wildrgbd.github.io/)]
  [2024.01]
  
- **SBSM:** Zizhang Li, Dor Litvak, Ruining Li, Yunzhi Zhang, Tomas Jakab, Christian Rupprecht, Shangzhe Wu, Andrea Vedaldi, Jiajun Wu.<br />
  "Learning the 3D Fauna of the Web." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2401.02400)] 
  [[code](https://kyleleey.github.io/3DFauna/)]
  [2024.01]

- **DiffuMatting:** Xiaobin Hu, Xu Peng, Donghao Luo, Xiaozhong Ji, Jinlong Peng, Zhengkai Jiang, Jiangning Zhang, Taisong Jin, Chengjie Wang, Rongrong Ji.<br />
  "DiffuMatting: Synthesizing Arbitrary Objects with Matting-level Annotation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.06168)] 
  [2024.03]

- Meyer, A., Mazellier, JP., Dana, J. et al.<br />
  "On-the-fly point annotation for fast medical video labeling." Int J CARS (2024).
  [[paper](https://link.springer.com/article/10.1007/s11548-024-03098-y)] 
  [2024.04]
    
- **DTLLM-VLT:** Xuchen Li, Xiaokun Feng, Shiyu Hu, Meiqi Wu, Dailing Zhang, Jing Zhang, Kaiqi Huang.<br />
  "DTLLM-VLT: Diverse Text Generation for Visual Language Tracking Based on LLM." CVPRW (2024).
  [[paper](https://arxiv.org/abs/2405.12139)] 
  [2024.05]

- **SAMText:** Haibin He, Jing Zhang, Mengyang Xu, Juhua Liu, Bo Du, Dacheng Tao.<br />
  "Scalable Mask Annotation for Video Text Spotting." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2305.01443)] 
  [[code](https://github.com/ViTAE-Transformer/SAMText)]
  [2023.05]
  
- **SeaDronesSee-3D and BOArienT:** Benjamin Kiefer, Timon Höfer, Andreas Zell.<br />
  "Stable Yaw Estimation of Boats from the Viewpoint of UAVs and USVs." ECMR  (2023).
  [[paper](https://arxiv.org/abs/2306.14056)] 
  [2023.06]
      
- **LU-AVS:** Chen Liu, Peike Patrick Li, Qingtao Yu, Hongwei Sheng, Dadong Wang, Lincheng Li, Xin Yu.<br />
  "Benchmarking Audio Visual Segmentation for Long-Untrimmed Videos." CVPR (2024).
  [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Liu_Benchmarking_Audio_Visual_Segmentation_for_Long-Untrimmed_Videos_CVPR_2024_paper.html)] 
  [[code](https://yenanliu.github.io/LU-AVS/)]
  [2024.06]
  
- Yunho Kim, Jeong Hyun Lee, Choongin Lee, Juhyeok Mun, Donghoon Youm, Jeongsoo Park, Jemin Hwangbo.<br />
  "Learning Semantic Traversability with Egocentric Video and Automated Annotation Strategy." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2406.02989)] 
  [2024.06]
  
- **SegmentWithSAM:** Zafer Yildiz, Yuwen Chen, Maciej A. Mazurowski.<br />
  "SAM & SAM 2 in 3D Slicer: SegmentWithSAM Extension for Annotating Medical Images." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.15224)] 
  [[code](https://github.com/mazurowski-lab/SlicerSegmentWithSAM)]
  [2024.08]
    
### Video Super-Resolution
- **SEEM:** Zhihe Lu, Zeyu Xiao, Jiawang Bai, Zhiwei Xiong, Xinchao Wang.<br />
  "Can SAM Boost Video Super-Resolution?" ArXiv (2023).
  [[paper]( https://arxiv.org/abs/2305.06524)] 
  [2023.05]
  
### Text-to-Video Generation
- **Dancing Avatar:** Bosheng Qin, Wentao Ye, Qifan Yu, Siliang Tang, Yueting Zhuang.<br />
  "Dancing Avatar: Pose and Text-Guided Human Motion Videos Synthesis with Image Diffusion Model." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2308.07749)] 
  [2023.08]

- **MotionZero:** Sitong Su, Litao Guo, Lianli Gao, Hengtao Shen, Jingkuan Song.<br />
  "MotionZero:Exploiting Motion Priors for Zero-shot Text-to-Video Generation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.16635)] 
  [2023.11]

- **WonderJourney:** Hong-Xing Yu, Haoyi Duan, Junhwa Hur, Kyle Sargent, Michael Rubinstein, William T. Freeman, Forrester Cole, Deqing Sun, Noah Snavely, Jiajun Wu, Charles Herrmann.<br />
  "WonderJourney: Going from Anywhere to Everywhere." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.03884)] 
  [[code](https://kovenyu.com/WonderJourney/)]
  [2023.12]
      
- **CoCoCo:** Bojia Zi, Shihao Zhao, Xianbiao Qi, Jianan Wang, Yukai Shi, Qianyu Chen, Bin Liang, Kam-Fai Wong, Lei Zhang.<br />
  "CoCoCo: Improving Text-Guided Video Inpainting for Better Consistency, Controllability and Compatibility." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.12035)] 
  [[project](http://cococozibojia.github.io/)]
  [[code](https://github.com/zibojia/COCOCO)]
  [2024.03]

- Chaoyi Wang, Yaozhe Song, Yafeng Zhang, Jun Pei, Lijie Xia, Jianpo Liu.<br />
  "Video Generation with Consistency Tuning." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.06356)] 
  [2024.03]

- **AvatarGO:** Yukang Cao, Liang Pan, Kai Han, Kwan-Yee K. Wong, Ziwei Liu.<br />
  "AvatarGO: Zero-shot 4D Human-Object Interaction Generation and Animation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2410.07164)] 
  [[code](https://yukangcao.github.io/AvatarGO/)]
  [2024.10]

### Video Generation with Other Modalities
- **DisCo:** Tan Wang, Linjie Li, Kevin Lin, Yuanhao Zhai, Chung-Ching Lin, Zhengyuan Yang, Hanwang Zhang, Zicheng Liu, Lijuan Wang.<br />
  "DisCo: Disentangled Control for Realistic Human Dance Generation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2307.00040)] 
  [[code](https://disco-dance.github.io/)]
  [2023.07]
  
- **VideoBooth:** Yuming Jiang, Tianxing Wu, Shuai Yang, Chenyang Si, Dahua Lin, Yu Qiao, Chen Change Loy, Ziwei Liu.<br />
  "VideoBooth: Diffusion-based Video Generation with Image Prompts." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.00777)] 
  [[code](https://vchitect.github.io/VideoBooth-project/)]
  [2023.12]
  
- Yao-Chih Lee, Zhoutong Zhang, Kevin Blackburn-Matzen, Simon Niklaus, Jianming Zhang, Jia-Bin Huang, Feng Liu.<br />
  "Fast View Synthesis of Casual Videos with Soup-of-Planes." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.02135)] 
  [[code](https://casual-fvs.github.io/)]
  [2023.12]
    
- **CoDeF:** Hao Ouyang, Qiuyu Wang, Yuxi Xiao, Qingyan Bai, Juntao Zhang, Kecheng Zheng, Xiaowei Zhou, Qifeng Chen, Yujun Shen.<br />
  "CoDeF: Content Deformation Fields for Temporally Consistent Video Processing." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2308.07926)] 
  [[code](https://qiuyu96.github.io/CoDeF/)]
  [2023.08] 

- **CPAB:** Hexiang Wang, Fengqi Liu, Qianyu Zhou, Ran Yi, Xin Tan, Lizhuang Ma.<br />
  "Continuous Piecewise-Affine Based Motion Model for Image Animation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2401.09146)] 
  [[code](https://github.com/DevilPG/AAAI2024-CPABMM)]
  [2024.01]
  
- **MultiDance-Zero:** Zhe Xu, Kun Wei, Xu Yang, Cheng Deng.<br />
  "Do You Guys Want to Dance: Zero-Shot Compositional Human Dance Generation with Multiple Persons." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2401.13363)] 
  [2024.01]
  
- **Lester:** Ruben Tous.<br />
  "Lester: rotoscope animation through video object segmentation and tracking." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2402.09883)] 
  [2024.02]
  
- **DragAnything:** Weijia Wu, Zhuang Li, Yuchao Gu, Rui Zhao, Yefei He, David Junhao Zhang, Mike Zheng Shou, Yan Li, Tingting Gao, Di Zhang.<br />
  "DragAnything: Motion Control for Anything using Entity Representation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.07420)] 
  [[code](https://github.com/showlab/DragAnything)]
  [[homepage](https://weijiawu.github.io/draganything_page/)]
  [2024.03]

- Chaoyi Wang, Yaozhe Song, Yafeng Zhang, Jun Pei, Lijie Xia, Jianpo Liu.<br />
  "Video Generation with Consistency Tuning." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.06356)] 
  [2024.03]
  
- **UnSAMFlow:** Shuai Yuan, Lei Luo, Zhuo Hui, Can Pu, Xiaoyu Xiang, Rakesh Ranjan, Denis Demandolx.<br />
  "UnSAMFlow: Unsupervised Optical Flow Guided by Segment Anything Model." CVPR (2024).
  [[paper](https://arxiv.org/abs/2405.02608)] 
  [[code](https://github.com/facebookresearch/UnSAMFlow)]
  [2024.05]  

### Others
- **VTA:** Yuchen Hu, Yu Gu, Chenxing Li, Rilin Chen, Dong Yu.<br />
  "Video-to-Audio Generation with Fine-grained Temporal Semantics." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.14709)] 
  [[code](https://sounddemos.github.io/vta-sam/)]
  [2024.09]

  
## Video Understanding and Analysis
### Video Captioning
- **Exo2EgoDVC:** Takehiko Ohkawa, Takuma Yagi, Taichi Nishimura, Ryosuke Furuta, Atsushi Hashimoto, Yoshitaka Ushiku, Yoichi Sato.<br />
  "Exo2EgoDVC: Dense Video Captioning of Egocentric Procedural Activities Using Web Instructional Videos." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.16444)] 
  [2023.11]
  
- **u-LLaVA:** Jinjin Xu, Liwu Xu, Yuzhe Yang, Xiang Li, Yanchun Xie, Yi-Jie Huang, Yaqian Li.<br />
  "u-LLaVA: Unifying Multi-Modal Tasks via Large Language Model." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.05348)] 
  [2023.11]

- **OW-VISCap:** Anwesa Choudhuri, Girish Chowdhary, Alexander G. Schwing.<br />
  "OW-VISCap: Open-World Video Instance Segmentation and Captioning." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.03657)] 
  [[code](https://anwesachoudhuri.github.io/OpenWorldVISCap/)]
  [2024.04]

- **BACON:** Zhantao Yang, Ruili Feng, Keyu Yan, Huangji Wang, Zhicai Wang, Shangwen Zhu, Han Zhang, Jie Xiao, Pingyu Wu, Kai Zhu, Jixuan Chen, Chen-Wei Xie, Chaojie Mao, Yue Yang, Hongyang Zhang, Yu Liu, Fan Cheng.<br />
  "BACON: Supercharge Your VLM with Bag-of-Concept Graph to Mitigate Hallucinations." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2407.03314)] 
  [[code](https://ztyang23.github.io/bacon-page)]
  [2024.07]

### Video Dialog
- **MST_MIXER:** Adnen Abdessaied, Lei Shi, Andreas Bulling.<br />
  "Multi-Modal Video Dialog State Tracking in the Wild." ECCV (2024).
  [[paper](https://arxiv.org/abs/2407.02218)] 
  [[code](https://perceptualui.org/publications/abdessaied24_eccv)]
 [2024.07]

### Video Grounding
- **PG-Video-LLaVA:** Shehan Munasinghe, Rusiru Thushara, Muhammad Maaz, Hanoona Abdul Rasheed, Salman Khan, Mubarak Shah, Fahad Khan.<br />
  "PG-Video-LLaVA: Pixel Grounding Large Video-Language Models." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.13435)] 
  [[code](https://github.com/mbzuai-oryx/Video-LLaVA)]
  [2023.11]

### Optical Flow Estimation
- **SAMFlow:** Shili Zhou, Ruian He, Weimin Tan, Bo Yan.<br />
  "SAMFlow: Eliminating Any Fragmentation in Optical Flow with Segment Anything Model." AAAI (2024).
  [[paper](https://arxiv.org/abs/2307.16586)] 
  [2023.07]
  
### Pose Estimation
- **Mask as Supervision:** Yuchen Yang, Yu Qiao, Xiao Sun.<br />
  "Mask as Supervision: Leveraging Unified Mask Information for Unsupervised 3D Pose Estimation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.07051)] 
  [[code](https://github.com/Charrrrrlie/Mask-as-Supervision)]
  [2023.12]
  
### Video ReID
- **SemReID:** Siyuan Huang, Yifan Zhou, Ram Prabhakar Kathirvel, Rama Chellappa, Chun Pong Lau.<br />
  "Self-Supervised Learning of Whole and Component-Based Semantic Representations for Person Re-Identification." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2311.17074)] 
  [2023.11]
  

### Others
- **SAMEdge:** Rui Lu, Siping Shi, Yanting Liu, Dan Wang.<br />
  "SAMEdge: An Edge-cloud Video Analytics Architecture for the Segment Anything Model." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.14784)] 
  [2024.09]

- **MORA:** Andong Deng, Tongjia Chen, Shoubin Yu, Taojiannan Yang, Lincoln Spencer, Yapeng Tian, Ajmal Saeed Mian, Mohit Bansal, Chen Chen.<br />
"Motion-Grounded Video Reasoning: Understanding and Perceiving Motion at Pixel Level." ArXiv (2024).
[[paper](https://arxiv.org/abs/2411.09921)]
[[code](https://groundmore.github.io/)]
[2024.11]
  
## Medical Video Processing
- **SurgicalSAM:** An Wang, Mobarakol Islam, Mengya Xu, Yang Zhang, Hongliang Ren.<br />
  "SAM Meets Robotic Surgery: An Empirical Study on Generalization, Robustness and Adaptation." MICCAI MedAGI Workshop (2023).
  [[paper](https://arxiv.org/abs/2308.07156)] 
  [2023.08]
  
- **SAMSNeRF:** Ange Lou, Yamin Li, Xing Yao, Yike Zhang, Jack Noble.<br />
  "SAMSNeRF: Segment Anything Model (SAM) Guides Dynamic Surgical Scene Reconstruction by Neural Radiance Field (NeRF)." Image-Guided Procedures, Robotic Interventions, and Modeling (2024).
  [[paper](https://arxiv.org/abs/2308.11774)] 
  [[code](https://github.com/AngeLouCN/SAMSNeRF)]
  [2023.08]
  
- **SurgicalSAM:** Wenxi Yue, Jing Zhang, Kun Hu, Yong Xia, Jiebo Luo, Zhiyong Wang.<br />
  "SurgicalSAM: Efficient Class Promptable Surgical Instrument Segmentation." AAAI (2024).
  [[paper](https://arxiv.org/abs/2308.08746)] 
  [[code](https://github.com/wenxi-yue/SurgicalSAM)]
  [2023.08]
    
- Leo Fillioux, Emilie Gontran, Jérôme Cartry, Jacques RR Mathieu, Sabrina Bedja, Alice Boilève, Paul-Henry Cournède, Fanny Jaulin, Stergios Christodoulidis, Maria Vakalopoulou.<br />
  "Spatio-Temporal Analysis of Patient-Derived Organoid Videos Using Deep Learning for the Prediction of Drug Efficacy." ICCV Workshop (2023).
  [[paper](https://arxiv.org/abs/2308.14461)] 
  [2023.08]
  
- **SuPerPM:** Shan Lin, Albert J. Miao, Ali Alabiad, Fei Liu, Kaiyuan Wang, Jingpei Lu, Florian Richter, Michael C. Yip.<br />
  "SuPerPM: A Large Deformation-Robust Surgical Perception Framework Based on Deep Point Matching Learned from Physical Constrained Simulation Data" ArXiv (2023).
  [[paper](https://arxiv.org/abs/2309.13863)] 
  [2023.09]
  
- **SP-SAM:** Wenxi Yue, Jing Zhang, Kun Hu, Qiuxia Wu, Zongyuan Ge, Yong Xia, Jiebo Luo, Zhiyong Wang.<br />
  "SurgicalPart-SAM: Part to Whole Collaborative Prompting for Surgical Instrument Segmentation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.14481)] 
  [[code](https://github.com/wenxi-yue/SurgicalPart-SAM)]
  [2023.12]

- **Surgment:** Jingying Wang, Haoran Tang, Taylor Kantor, Tandis Soltani, Vitaliy Popov, Xu Wang.<br />
  "Surgment: Segmentation-enabled Semantic Search and Creation of Visual Question and Feedback to Support Video-Based Surgery Learning." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2402.17903)] 
  [2024.02]
    
- Aviad Dahan, Tal Shaharabany, Raja Giryes, Lior Wolf.<br />
  "Video Polyp Segmentation using Implicit Networks." ArXiv (2024).
  [[paper](https://openreview.net/forum?id=7gFODPjwOe)] 
  [2024.02]

- **P^2SAM:** Chenhui Zhao, Liyue Shen.<br />
  "Part-aware Personalized Segment Anything Model for Patient-Specific Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.05433)] 
  [2024.03]
    
- **WeakSurg:** Qiyuan Wang, Yanzhe Liu, Shang Zhao, Rong Liu, S. Kevin Zhou.<br />
  "WeakSurg: Weakly supervised surgical instrument segmentation using temporal equivariance and semantic continuity." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.09551)] 
  [2024.03]
              
- **CCSpO2Net:** Sun, Xiantao and Wen, Tao and Chen, Weihai and Huang, Bin.<br />
  "CCSpO2Net: Camera-Based Contactless Oxygen Saturation Measurement Foundation Model in Clinical Settings." TIM (2024).
  [[paper](https://ieeexplore.ieee.org/abstract/document/10464344)] 
  [2024.03]
  
- Zijian Wu, Adam Schmidt, Peter Kazanzides, Septimiu E. Salcudean.<br />
  "Augmenting Efficient Real-time Surgical Instrument Segmentation in Video with Point Tracking and Segment Anything." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.08003)] 
  [2024.03]
  
- Seda Camalan, Muhammad Khalid Khan Niazi, Charles Elmaraghy, Aaron C. Moberly, Metin N. Gurcan.<br />
  "Tympanic membrane segmentation of video frames to create composite images using SAM." SPIE (2024).
  [[paper](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/12927/1292736/Tympanic-membrane-segmentation-of-video-frames-to-create-composite-images/10.1117/12.3006926.short#_=_)] 
  [2024.04]
   
- **ESD:** Jieming Yu, Long Bai, Guankun Wang, An Wang, Xiaoxiao Yang, Huxin Gao, Hongliang Ren.<br />
  "Adapting SAM for Surgical Instrument Tracking and Segmentation in Endoscopic Submucosal Dissection Videos." IEEE ICRA C4SR+ Workshop (2024).
  [[paper](https://arxiv.org/abs/2404.10640)] 
  [2024.04]
  
- **Surgical-DeSAM:** Yuyang Sheng, Sophia Bano, Matthew J. Clarkson, Mobarakol Islam.<br />
  "Surgical-DeSAM: Decoupling SAM for Instrument Segmentation in Robotic Surgery." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.14040)] 
  [2024.04]
  
- **UroSAM:** Leng, Jixuan and Liu, Junfei and Cheng, Galen and Wang, Haohan and Quarrier, Scott Orzech and Luo, Jiebo and Jain, Rajat.<br />
  "Development of UroSAM: a machine learning model to automatically identify kidney stone composition from endoscopic video." Journal of Endourology (2024).
  [[paper](https://www.liebertpub.com/doi/abs/10.1089/end.2023.0740?casa_token=w2fwDmE_-swAAAAA%3AvQ_F2iaHPYMxOOlhV4z2iaK3X5nE9V0gsUBoD93FqbW5DJa3XkaB2d5X9lmZSeRBtjJRtqkzttM4Amx8)] 
  [2024.05]
    
- **MemSAM:** Xiaolong Deng, Huisi Wu, Runhao Zeng, Jing Qin.<br />
  "MemSAM: Taming Segment Anything Model for Echocardiography Video Segmentation." CVPR (2024).
  [[paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Deng_MemSAM_Taming_Segment_Anything_Model_for_Echocardiography_Video_Segmentation_CVPR_2024_paper.pdf)] 
  [[code](https://github.com/dengxl0520/MemSAM)]
  [2024.05]
  
- **WSPoly-SAM:** Tingting Cai and Hongping Yan and Kun Ding and Yan Zhang and Yueyue Zhou.<br />
  "WSPoly-SAM: Weakly-Supervised and Self-Guided Fine-Tuning of SAM for Colonoscopy Polyp Segmentation." ArXiv (2024).
  [[paper](https://www.preprints.org/manuscript/202405.0389/v1)] 
  [2024.05]
    
- **D2GPLan:** Jialun Pei, Ruize Cui, Yaoqian Li, Weixin Si, Jing Qin, Pheng-Ann Heng.<br />
  "Depth-Driven Geometric Prompt Learning for Laparoscopic Liver Landmark Detection." MICCAI (2024).
  [[paper](https://arxiv.org/abs/2406.17858)] 
  [[code](https://github.com/PJLallen/D2GPLand)]
  [2024.06]
    
- **ASI-Seg:** Zhen Chen, Zongming Zhang, Wenwu Guo, Xingjian Luo, Long Bai, Jinlin Wu, Hongliang Ren, Hongbin Liu.<br />
  "ASI-Seg: Audio-Driven Surgical Instrument Segmentation with Surgeon Intention Understanding." IROS  (2024).
  [[paper](https://arxiv.org/abs/2407.19435)] 
  [[code](https://github.com/Zonmgin-Zhang/ASI-Seg)]
  [2024.07]
  
- **VDST-Net:** Guiqiu Liao, Matjaz Jogan, Sai Koushik, Eric Eaton, Daniel A. Hashimoto.<br />
  "Disentangling spatio-temporal knowledge for weakly supervised object detection and segmentation in surgical video." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2407.15794)] 
  [2024.07]
  
- Ange Lou, Yamin Li, Yike Zhang, Robert F. Labadie, Jack Noble.<br />
  "Zero-Shot Surgical Tool Segmentation in Monocular Video Using Segment Anything Model 2." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.01648)] 
  [[project](https://github.com/AngeLouCN/SAM-2_Surgical_Video)]
  [2024.08]
    
- Yosuke Yamagishi, Shouhei Hanaoka, Tomohiro Kikuchi, Takahiro Nakao, Yuta Nakamura, Yukihiro Nomura, Soichiro Miki, Takeharu Yoshikawa, Osamu Abe.<br />
  "Zero-shot 3D Segmentation of Abdominal Organs in CT Scans Using Segment Anything Model 2: Adapting Video Tracking Capabilities for 3D Medical Imaging." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.06170)] 
  [2024.08]
    
- **MedSAM:** Jun Ma, Sumin Kim, Feifei Li, Mohammed Baharoon, Reza Asakereh, Hongwei Lyu, Bo Wang.<br />
  "Segment Anything in Medical Images and Videos: Benchmark and Deployment." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.03322)] 
  [[code](https://github.com/bowang-lab/MedSAM)]
  [2024.08]
    
- Andrew Seohwan Yu, Mohsen Hariri, Xuecen Zhang, Mingrui Yang, Vipin Chaudhary, Xiaojuan Li.<br />
  "Novel adaptation of video segmentation to 3D MRI: efficient zero-shot knee segmentation with SAM2." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.04762)] 
  [2024.08]
  
- Jieming Yu, An Wang, Wenzhen Dong, Mengya Xu, Mobarakol Islam, Jie Wang, Long Bai, Hongliang Ren.<br />
  "SAM 2 in Robotic Surgery: An Empirical Evaluation for Robustness and Generalization in Surgical Video Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.04593)] 
  [2024.08]
  
- Haoyu Dong, Hanxue Gu, Yaqian Chen, Jichen Yang, Maciej A. Mazurowski.<br />
  "Segment anything model 2: an application to 2D and 3D medical images." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.00756)] 
  [2024.08]
      
- Lin Zhao, Xiao Chen, Eric Z. Chen, Yikang Liu, Terrence Chen, Shanhui Sun.<br />
  "Retrieval-augmented Few-shot Medical Image Segmentation with Foundation Models." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.08813)] 
  [2024.08]
      
- **BioSAM 2:** Zhiling Yan, Weixiang Sun, Rong Zhou, Zhengqing Yuan, Kai Zhang, Yiwei Li, Tianming Liu, Quanzheng Li, Xiang Li, Lifang He, Lichao Sun.<br />
  "Biomedical SAM 2: Segment Anything in Biomedical Images and Videos." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.03286)] 
  [2024.08]

- **SAM_2_Medical_3D:** Chuyun Shen, Wenhao Li, Yuhang Shi, Xiangfeng Wang.<br />
  "Interactive 3D Medical Image Segmentation with SAM 2." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.02635)] 
  [[code](https://github.com/Chuyun-Shen/SAM_2_Medical_3D)]
  [2024.08]
  
- Sourya Sengupta, Satrajit Chakrabarty, Ravi Soni.<br />
  "Is SAM 2 Better than SAM in Medical Image Segmentation?." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.04212)] 
  [2024.08]
  
- **Surgical SAM 2:** Haofeng Liu, Erli Zhang, Junde Wu, Mingxuan Hong, Yueming Jin.<br />
  "Surgical SAM 2: Real-time Segment Anything in Surgical Video by Efficient Frame Pruning." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.07931)] 
  [[code](https://github.com/jinlab-imvr/Surgical-SAM-2)]
  [2024.08]
    
- Yiqing Shen, Hao Ding, Xinyuan Shao, Mathias Unberath.<br />
  "Performance and Non-adversarial Robustness of the Segment Anything Model 2 in Surgical Video Segmentation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.04098)] 
  [2024.08]
    
- **MedSAM-2:** Jiayuan Zhu, Yunli Qi, Junde Wu.<br />
  "Medical SAM 2: Segment medical images as video via Segment Anything Model 2." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.00874)] 
  [[code](https://github.com/MedicineToken/Medical-SAM2)]
  [2024.08]
  
- **Polyp SAM 2:** Mobina Mansoori, Sajjad Shahabodini, Jamshid Abouei, Konstantinos N. Plataniotis, Arash Mohammadi.<br />
  "Polyp SAM 2: Advancing Zero shot Polyp Segmentation in Colorectal Cancer Detection." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2408.05892)] 
  [[code](https://github.com/sajjad-sh33/Polyp-SAM-2)]
  [2024.08]
          
- **FS-MedSAM2:** Yunhao Bai, Qinji Yu, Boxiang Yun, Dakai Jin, Yingda Xia, Yan Wang.<br />
  "FS-MedSAM2: Exploring the Potential of SAM2 for Few-Shot Medical Image Segmentation without Fine-tuning." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.04298)] 
  [[code](https://github.com/DeepMed-Lab-ECNU/FS_MedSAM2)]
  [2024.09]
  
- **YOLO-SAM 2:** Mobina Mansoori, Sajjad Shahabodini, Jamshid Abouei, Konstantinos N. Plataniotis, Arash Mohammadi.<br />
  "Self-Prompting Polyp Segmentation in Colonoscopy using Hybrid Yolo-SAM 2 Model." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.09484)] 
  [[code](https://github.com/sajjad-sh33/YOLO_SAM2)]
  [2024.09]
  
- **MediViSTA-SAM:** Sekeun Kim, Kyungsang Kim, Jiang Hu, Cheng Chen, Zhiliang Lyu, Ren Hui, Sunghwan Kim, Zhengliang Liu, Aoxiao Zhong, Xiang Li, Tianming Liu, Quanzheng Li.<br />
  "MediViSTA-SAM: Zero-shot Medical Video Analysis with Spatio-temporal SAM Adaptation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2309.13539)] 
  [[code](https://github.com/kimsekeun/MediViSTA-SAM)]
  [2023.09]
  
- **SAM-OCTA2:** Xinrun Chen, Chengliang Wang, Haojian Ning, Mengzhan Zhang, Mei Shen, Shiying Li.<br />
  "SAM-OCTA2: Layer Sequence OCTA Segmentation with Fine-tuned Segment Anything Model 2." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.09286)] 
  [[code](https://github.com/ShellRedia/SAM-OCTA2)]
  [2024.09]

- **VP-SAM:** Zhixue Fang, Yuzhi Liu, Huisi Wu , and Jin Qin.<br />
  "VP-SAM: Taming Segment Anything Model for Video Polyp Segmentation via Disentanglement and Spatio-temporal Side Network." ECCV (2024).
  [[paper](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/03403.pdf)] 
  [[code](https://github.com/zhixue-fang/VPSAM)]
  [2024.09]
  
## Other Video Tasks
### Video Compression
- **SA-ICM:** Takahiro Shindo, Kein Yamada, Taiju Watanabe, Hiroshi Watanabe.<br />
  "Image Coding for Machines with Edge Information Learning Using Segment Anything." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.04173)] 
  [2024.03]
  
### Robotics
- **MMPM:** Jiange Yang, Wenhui Tan, Chuhao Jin, Bei Liu, Jianlong Fu, Ruihua Song, Limin Wang.<br />
  "Pave the Way to Grasp Anything: Transferring Foundation Models for Universal Pick-Place Robots." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2306.05716)] 
  [[YouTube](https://www.youtube.com/watch?v=1m9wNzfp_4E)]
  [[Bilibili](https://www.bilibili.com/video/BV178411Z7H2/)]
  [2023.06]
  
- **DEFT:** Aditya Kannan.<br />
  "Learning from Human Videos for Robotic Manipulation." ArXiv (2023).
  [[paper](http://reports-archive.adm.cs.cmu.edu/anon/anon/usr/ftp/2023/CMU-CS-23-124.pdf)] 
  [[code](https://github.com/adityak77/masters-thesis)]
  [2023.07]
  
- **ROSGPT_Vision:** Bilel Benjdira, Anis Koubaa, Anas M. Ali.<br />
  "ROSGPT_Vision: Commanding Robots Using Only Language Models' Prompts." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2308.11236)] 
  [[code](https://github.com/bilel-bj/ROSGPT_Vision)]
  [2023.08]
    
- Mayara E. Bonani, Max Schwarz, Sven Behnke.<br />
  "Learning from SAM: Harnessing a Segmentation Foundation Model for Sim2Real Domain Adaptation through Regularization." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2309.15562)] 
  [2023.09]
    
- **SAM-G:** Ziyu Wang, Yanjie Ze, Yifei Sun, Zhecheng Yuan, Huazhe Xu.<br />
  "Generalizable Visual Reinforcement Learning with Segment Anything Model." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.17116)] 
  [[code](https://yanjieze.com/SAM-G/)]
  [2023.12]

- Kangcheng Liu, Xinhu Zheng, Chaoqun Wang, Hesheng Wang, Ming Liu, Kai Tang.<br />
  "Online Robot Navigation and and Manipulation with Distilled Vision-Language Models." ICRA  (2024).
  [[paper](https://arxiv.org/abs/2401.17083)] 
  [2024.01]
    
- **ScaleFlow:** Chengbo Yuan, Chuan Wen, Tong Zhang, Yang Gao.<br />
  "General Flow as Foundation Affordance for Scalable Robot Learning." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2401.11439)] 
  [[code](https://general-flow.github.io/)]
  [2024.01]
  
- **GEMO:** Yinuo Zhao, Kun Wu, Tianjiao Yi, Zhiyuan Xu, Xiaozhu Ju, Zhengping Che, Qinru Qiu, Chi Harold Liu, Jian Tang.<br />
  "An Efficient Generalizable Framework for Visuomotor Policies via Control-aware Augmentation and Privilege-guided Distillation." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2401.09258)] 
  [2024.01]

- **CTL:** Anas Gouda, Max Schwarz, Christopher Reining, Sven Behnke, Alice Kirchheim.<br />
  "Learning Embeddings with Centroid Triplet Loss for Object Identification in Robotic Grasping." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2404.06277)] 
  [[code](https://github.com/AnasIbrahim/ctl_classification)]
  [2024.04]
  
- **RoVi-Aug:** Lawrence Yunliang Chen, Chenfeng Xu, Karthik Dharmarajan, Zubair Irshad, Richard Cheng, Kurt Keutzer, Masayoshi Tomizuka, Quan Vuong, Ken Goldberg.<br />
  "RoVi-Aug: Robot and Viewpoint Augmentation for Cross-Embodiment Robot Learning." CoRL (2024).
  [[paper](https://arxiv.org/abs/2409.03403)] 
  [2024.09]

- Xi Wang, Tianxing Chen, Qiaojun Yu, Tianling Xu, Zanxin Chen, Yiting Fu, Cewu Lu, Yao Mu, Ping Luo.<br />
  "Articulated Object Manipulation using Online Axis Estimation with SAM2-Based Tracking." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.16287)] 
  [[code](https://hytidel.github.io/video-tracking-for-axis-estimation/)]
  [2024.09]
  
- **Robotic-CLIP:** Nghia Nguyen, Minh Nhat Vu, Tung D. Ta, Baoru Huang, Thieu Vo, Ngan Le, Anh Nguyen.<br />
  "Robotic-CLIP: Fine-tuning CLIP on Action Data for Robotic Applications." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2409.17727)] 
  [2024.09]   
  
### Video Game
- Christian A. Schiller.<br />
  "Virtual Augmented Reality for Atari Reinforcement Learning." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2310.08683)]
  [2023.10]
  
### Video Style Transfer Attack
- **LocalStyleFool:** Yuxin Cao, Jinghao Li, Xi Xiao, Derui Wang, Minhui Xue, Hao Ge, Wei Liu, Guangwu Hu.<br />
  "LocalStyleFool: Regional Video Style Transfer Attack Using Segment Anything Model." SPW (2024).
  [[paper](https://arxiv.org/abs/2403.11656)] 
  [2024.03]
  
### Semantic Communication
- **SemCom:** Avi Deb Raha, Md. Shirajum Munir, Apurba Adhikary, Yu Qiao, Choong Seon Hong.<br />
  "Generative AI-driven Semantic Communication Framework for NextG Wireless Network." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2310.09021)] 
  [2023.10]
  
### Tool Software
- Cheng-Yu Hsieh, Si-An Chen, Chun-Liang Li, Yasuhisa Fujii, Alexander Ratner, Chen-Yu Lee, Ranjay Krishna, Tomas Pfister.<br />
  "Tool Documentation Enables Zero-Shot Tool-Usage with Large Language Models." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2308.00675)] 
  [2023.08]
  
- **ASSISTGUI:** Difei Gao, Lei Ji, Zechen Bai, Mingyu Ouyang, Peiran Li, Dongxing Mao, Qinchen Wu, Weichen Zhang, Peiyi Wang, Xiangwu Guo, Hengxu Wang, Luowei Zhou, Mike Zheng Shou.<br />
  "ASSISTGUI: Task-Oriented Desktop Graphical User Interface Automation." ArXiv (2023).
  [[paper](https://arxiv.org/abs/2312.13108)] 
  [2023.12]
  
- **Annolid:** Chen Yang, Thomas A. Cleland.<br />
  "Annolid: Annotate, Segment, and Track Anything You Need." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2403.18690)] 
  [2024.03]
  
- Aditya Gunturu, Yi Wen, Jarin Thundathil, Nandi Zhang, Rubaiat Habib Kazi, Ryo Suzuki.<br />
  "Augmented Physics: A Machine Learning-Powered Tool for Creating Interactive Physics Simulations from Static Diagrams." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2405.18614)] 
  [2024.05]

- Kevin Charles Bierlich, Sagar Karki, Clara N. Bird, Alan Fern, Leigh G. Torres.<br />
  "Automated body length and body condition measurements of whales from drone videos for rapid assessment of population health." Marine Mammal Science (2024).
  [[paper](https://onlinelibrary.wiley.com/doi/full/10.1111/mms.13137)] 
  [2024.05]

- **DisFormer:** Sanket Gandhi, Atul, Samanyu Mahajan, Vishal Sharma, Rushil Gupta, Arnab Kumar Mondal, Parag Singla.<br />
  "Learning Disentangled Representation in Object-Centric Models for Visual Dynamics Prediction via Transformers." ArXiv (2024).
  [[paper](https://arxiv.org/abs/2407.03216)] 
 [2024.07]  
  
## License
This project is released under the MIT license. Please see the [LICENSE](LICENSE) file for more information.
