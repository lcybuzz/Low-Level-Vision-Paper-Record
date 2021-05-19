# Table of Contents
- [Reflection Removal](#reflection-removal)
- [De-raining (Archived)](#de-raining)
- [Image Demoireing (Archived)](#image-demoireing)
- [Style-Transfer (Archived)](#style-transfer)

# Reflection Removal
### *Panoramic image reflection removal*
**[Paper]** (CVPR 2021) Panoramic image reflection removal  <Br>
**[Author]** [Yuchen Hong](http://vcc.szu.edu.cn/index-2.html), [Qian Zheng](https://q-zh.github.io/), Lingran Zhao, [Xudong Jiang](https://personal.ntu.edu.sg/exdjiang/), Alex C. Kot, [Boxin Shi](http://ci.idm.pku.edu.cn/)  <Br>

### *Single image reflection removal with absorption effect*
**[Paper]** (CVPR 2021) Single image reflection removal with absorption effect  <Br>
**[Author]** [Qian Zheng](https://q-zh.github.io/), [Boxin Shi](http://ci.idm.pku.edu.cn/), Jinnan Chen, [Xudong Jiang](https://personal.ntu.edu.sg/exdjiang/), Ling-Yu Duan, Alex C. Kot  <Br>
**[[Pytorch-Code](https://github.com/q-zh/absorption)]** <Br>

### *Robust Reflection Removal with Reflection-free Flash-only Cues*
**[Paper]** (CVPR 2021) Robust Reflection Removal with Reflection-free Flash-only Cues  <Br>
**[Author]** [Chenyang Lei](https://chenyanglei.github.io/), [Qifeng Chen](https://cqf.io/)  <Br>
**[[Project](https://chenyanglei.github.io/flashrr_rfc/index.html)]** **[[TF-Code](https://github.com/ChenyangLEI/flash-reflection-removal)]**<Br>

### *Reflection scene separation from a single image*
**[Paper]** (CVPR 2020) Reflection scene separation from a single image  <Br>
**[Author]** [Renjie Wan](https://wanrenjie.github.io/, [Boxin Shi](http://ci.idm.pku.edu.cn/), [Haoliang Li](https://hlli1991.github.io/), Ling-Yu Duan, Alex C. Kot  <Br>

### ObstructionRemoval ★★
**[Paper]** (CVPR 2020) Learning to See Through Obstructions  <Br>
**[Author]** [Yu-Lun Liu](http://www.cmlab.csie.ntu.edu.tw/~yulunliu/), [Wei-Sheng Lai](https://www.wslai.net/), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/)  <Br>
**[[Project](https://alex04072000.github.io/ObstructionRemoval/)]** **[[TF-Code](https://github.com/alex04072000/ObstructionRemoval)]**<Br>
使用多帧和光流的思想去反射. 用多帧处理去反射问题与单帧相比更可靠一些, 本文的网络设计值得学习.

### IBCLN
**[Paper]** (CVPR 2020) Single Image Reflection Removal through Cascaded Refinement  <Br>
**[Author]** Chao Li, Yixiao Yang, Kun He, Stephen Lin, John E. Hopcroft  <Br>
**[[Pytorch-Code](https://github.com/JHL-HUST/IBCLN)]** <Br>

### *Polarized Reflection Removal*
**[Paper]** (CVPR 2020) Polarized Reflection Removal with Perfect Alignment in the Wild  <Br>
**[Author]** [Chenyang Lei](https://chenyanglei.github.io/), Xuhua Huang, Mengdi Zhang, Qiong Yan, Wenxiu Sun, [Qifeng Chen](https://cqf.io/)  <Br>
**[[Project](https://chenyanglei.github.io/polar_rr/index.html)]**, **[[TF-Code](https://github.com/ChenyangLEI/polarization-reflection-removal)]**<Br>

### Reflection removal rendering
**[Paper]** (CVPR 2020 Oral) Single Image Reflection Removal with Physically-Based Training Images <Br>
**[Author]** [Soomin Kim](https://sgvr.kaist.ac.kr/~smkim/), [Yuchi Huo](https://sgvr.kaist.ac.kr/~ychuo/), [Sung-Eui Yoon](https://sgvr.kaist.ac.kr/~sungeui/)  <Br>
**[[Project](https://sgvr.kaist.ac.kr/~smkim/Reflection_removal_rendering/)]**, **[[TF-Code](https://github.com/sookim813/Reflection_removal_rendering)]**<Br>

### *Single Image Reflection Removal Beyond Linearity*
**[Paper]** (CVPR 2019) Single Image Reflection Removal Beyond Linearity <Br>
**[Author]** Qiang Wen, Yinjie Tan, Jing Qin, Wenxi Liu, Guoqiang Han, and Shengfeng He <Br>
**[[Pytorch-Code](https://github.com/csqiangwen/Single-Image-Reflection-Removal-Beyond-Linearity)]**<Br>

### *Learning to jointly generate and separate reflections*
**[Paper]** (ICCV 2019) Learning to jointly generate and separate reflections  <Br>
**[Author]** [Daiqian Ma](https://madaiqian.github.io/), [Renjie Wan](https://wanrenjie.github.io/, [Boxin Shi](http://ci.idm.pku.edu.cn/), [Haoliang Li](https://hlli1991.github.io/), Ling-Yu Duan  <Br>

### perceptual-reflection-removal ★☆
**[Paper]** (CVPR 2018) Single Image Reflection Removal with Perceptual Losses <Br>
**[Author]** [Xuaner Zhang](https://people.eecs.berkeley.edu/~cecilia77/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html), [Qifeng Chen](https://cqf.io/) <Br>
**[[Project](https://people.eecs.berkeley.edu/~cecilia77/project-pages/reflection.html)]** **[[TF-Code](https://github.com/ceciliavision/perceptual-reflection-removal)]**<Br>
VGG19的多层特征作为hypercolumn与图像串联作为输入, 一个网络同时预测transmission和reflection, 使用pixel, VGG和GAN loss, 另外提出了一个gradient exclusion loss. 

### ReflectNet
**[Paper]** (ECCV 2018) ReflectNet: Separating Reflection and Transmission Images in the Wild <Br>
**[Author]** [Patrick Wieschollek](http://patwie.com/), [Orazio Gallo](https://oraziogallo.github.io/), [Jinwei Gu](http://www.gujinwei.org/), [Jan Kautz](https://jankautz.com/)  <Br>
**[[Project](https://research.nvidia.com/publication/2018-09_Separating-Reflection-and)]** **[[TF-Code](https://github.com/NVlabs/ReflectNet)]**<Br>

### BDN
**[Paper]** (ECCV 2018) Deep Bidirectional Estimation for Single Image Reflection Removal <Br>
**[Author]** [Jie Yang](https://github.com/yangj1e), [Dong Gong](https://donggong1.github.io)\, [Lingqiao Liu](https://sites.google.com/site/lingqiaoliu83/), [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/index.html) <Br>
*[[Pytorch-Code](https://github.com/yangj1e/bdn-refremv)]**<Br>


	

# De-raining
### Syn2Real ★★
**[Paper]**  (CVPR 2020) Syn2Real Transfer Learning for Image Deraining using Gaussian Processes<Br>
**[Author]** [Rajeev Yasarla](https://sites.google.com/view/rajeevyasarla/home), [Vishwanath A. Sindagi](https://www.vishwanathsindagi.com/), [Vishal M. Patel](https://engineering.jhu.edu/ece/faculty/vishal-m-patel/) <Br>
**[[Pytorch-Code](https://github.com/rajeevyasarla/Syn2Real)]**<Br>
使用高斯过程计算无标签真实数据的unsupervised loss. 从paper的实验效果来看有不错的效果, 值得一试

### MSPFN
**[Paper]**  (CVPR 2020) Multi-Scale Progressive Fusion Network for Single Image Deraining <Br>
**[Author]** [Kui Jiang](https://github.com/kuihua/kuijiang.github.io/blob/master/home.md), Zhongyuan Wang, Peng Yi, [Chen Chen](https://webpages.uncc.edu/cchen62/), Baojin Huang, Yimin Luo, [Jiayi Ma](https://sites.google.com/site/jiayima2013/), [Junjun Jiang](https://jiangjunjun.wordpress.com/) <Br>
**[[TF-Code](https://github.com/kuihua/MSPFN)]**<Br>
	
### DRD-Net
**[Paper]**  (CVPR 2020) Detail-recovery Image Deraining via Context Aggregation Networks <Br>
**[Author]** Sen Deng, Mingqiang Wei, Jun Wang, Yidan Feng, Luming Liang, Haoran Xie, Fu Lee Wang, Meng Wang <Br>
**[[TF-Code](hhttps://github.com/Dengsgithub/DRD-Net)]**<Br>

### DID-MDN ★☆
**[Paper]**  (CVPR 2018) Density-aware Single Image De-raining using a Multi-stream Dense Network<Br>
**[Author]** [He Zhang](https://sites.google.com/site/hezhangsprinter), [Vishal M. Patel](https://engineering.jhu.edu/vpatel36/sciencex_teams/vishalpatel/) <Br>
**[[Pytorch-Code](https://github.com/hezhangsprinter/DID-MDN)]**<Br>
基于dense connection的双分支去雨网络, 一个分支预测一个雨稠密程度的类别标签(大中小), 一个采用残差预测结构, 并结合稠密程度label, 预测去雨图像, 经过一个refinement网络输出. 加入一个预测程度的分支的策略, 在图像增强恢复任务中还是比较值得尝试的.

	
  

# Image Demoireing
### Learnbale_Bandpass_Filter ★
**[Paper]**  (CVPR 2020) Image Demoireing with Learnable Bandpass Filters  <Br>
**[Author]** Bolun Zheng, [Shanxin Yuan](https://sites.google.com/site/shanxinyuan/), [Gregory Slabaugh](http://www.gregslabaugh.net/), [Ales Leonardis](https://www.cs.bham.ac.uk/~leonarda/) <Br>
**[[TF-Code](https://github.com/zhenngbolun/Learnbale_Bandpass_Filter)]** <Br>
在DCT变换后的频谱域做摩尔纹提取, 分为3个scale提取不同尺度的摩尔纹. 对带通去取摩尔纹的推导部分没看懂. <Br>

### JDD
**[Paper]**  (CVPR 2020) Joint Demosaicing and Denoising With Self Guidance  <Br>
**[Author]** [Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), [Xu Jia](https://stephenjia.github.io/), Jianzhuang Liu, Qi Tian <Br>

### *Wavelet-Based Dual-Branch Networkfor Image Demoireing*
**[Paper]** (ECCV 2020) Wavelet-Based Dual-Branch Networkfor Image Demoireing  <Br>
**[Author]**[Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), Jianzhuang Liu, [Shanxin Yuan](https://shanxinyuan.github.io/), [Gregory Slabaugh](http://www.gregslabaugh.net/), [Ales Leonardis](https://www.cs.bham.ac.uk/~leonarda/), Wengang Zhou, Qi Tian <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>
	
### FHDe²Net
**[Paper]** (ECCV 2020) FHDe²Net: Full High Definition Demoireing Network <Br>
**[Author]** Bin He, Ce Wang, [Boxin Shi](http://ci.idm.pku.edu.cn/), Ling-Yu Duan <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>
	
### *Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs*
**[Paper]** (NeurIPS 2020) Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs  <Br>
**[Author]** [Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), [Shanxin Yuan](https://shanxinyuan.github.io/), Jianzhuang Liu, Liping Bao, Gregory Slabaugh, Qi Tian <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>



# Style-Transfer
### *Bilateral Style Transfer* ★★
**[Paper]**  (ECCV 2020) Joint Bilateral Learning for Real-time Universal Photorealistic Style Transfer  <Br>
**[Author]** [Xide Xia](https://xidexia.github.io/), Meng Zhang, [Tianfan Xue](http://people.csail.mit.edu/tfxue/), Zheng Sun, Hui Fang, [Brian Kulis](http://people.bu.edu/bkulis/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/) <Br>
基于HDRNet的实时风格迁移, 创新点尽管不是很多, 但是工作很有价值

  
  
