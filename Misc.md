# Table of Contents
- [Reflection Removal](#reflection-removal)
- [Image Inpainting](#image-inpainting)
- [De-raining (Archived)](#de-raining)
- [Image Demoireing (Archived)](#image-demoireing)
- [Style Transfer (Archived)](#style-transfer)
- [Image Fusion (Archived)](#image-fusion)

# Reflection Removal
#### *Panoramic image reflection removal*
**[Paper]** (CVPR 2021) Panoramic image reflection removal  <Br>
**[Author]** [Yuchen Hong](http://vcc.szu.edu.cn/index-2.html), [Qian Zheng](https://q-zh.github.io/), Lingran Zhao, [Xudong Jiang](https://personal.ntu.edu.sg/exdjiang/), Alex C. Kot, [Boxin Shi](http://ci.idm.pku.edu.cn/)  <Br>

#### *Single image reflection removal with absorption effect*
**[Paper]** (CVPR 2021) Single image reflection removal with absorption effect  <Br>
**[Author]** [Qian Zheng](https://q-zh.github.io/), [Boxin Shi](http://ci.idm.pku.edu.cn/), Jinnan Chen, [Xudong Jiang](https://personal.ntu.edu.sg/exdjiang/), Ling-Yu Duan, Alex C. Kot  <Br>
**[[Pytorch-Code](https://github.com/q-zh/absorption)]** <Br>

#### *Robust Reflection Removal with Reflection-free Flash-only Cues*
**[Paper]** (CVPR 2021) Robust Reflection Removal with Reflection-free Flash-only Cues  <Br>
**[Author]** [Chenyang Lei](https://chenyanglei.github.io/), [Qifeng Chen](https://cqf.io/)  <Br>
**[[Project](https://chenyanglei.github.io/flashrr_rfc/index.html)]** **[[TF-Code](https://github.com/ChenyangLEI/flash-reflection-removal)]**<Br>

#### *Reflection scene separation from a single image*
**[Paper]** (CVPR 2020) Reflection scene separation from a single image  <Br>
**[Author]** [Renjie Wan](https://wanrenjie.github.io/), [Boxin Shi](http://ci.idm.pku.edu.cn/), [Haoliang Li](https://hlli1991.github.io/), Ling-Yu Duan, Alex C. Kot  <Br>

#### ObstructionRemoval ★★
**[Paper]** (CVPR 2020) Learning to See Through Obstructions  <Br>
**[Author]** [Yu-Lun Liu](http://www.cmlab.csie.ntu.edu.tw/~yulunliu/), [Wei-Sheng Lai](https://www.wslai.net/), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/)  <Br>
**[[Project](https://alex04072000.github.io/ObstructionRemoval/)]** **[[TF-Code](https://github.com/alex04072000/ObstructionRemoval)]**<Br>
使用多帧和光流的思想去反射. 用多帧处理去反射问题与单帧相比更可靠一些, 本文的网络设计值得学习.

#### IBCLN
**[Paper]** (CVPR 2020) Single Image Reflection Removal through Cascaded Refinement  <Br>
**[Author]** Chao Li, Yixiao Yang, Kun He, Stephen Lin, John E. Hopcroft  <Br>
**[[Pytorch-Code](https://github.com/JHL-HUST/IBCLN)]** <Br>

#### *Polarized Reflection Removal*
**[Paper]** (CVPR 2020) Polarized Reflection Removal with Perfect Alignment in the Wild  <Br>
**[Author]** [Chenyang Lei](https://chenyanglei.github.io/), Xuhua Huang, Mengdi Zhang, Qiong Yan, Wenxiu Sun, [Qifeng Chen](https://cqf.io/)  <Br>
**[[Project](https://chenyanglei.github.io/polar_rr/index.html)]**, **[[TF-Code](https://github.com/ChenyangLEI/polarization-reflection-removal)]**<Br>

#### Reflection removal rendering
**[Paper]** (CVPR 2020 Oral) Single Image Reflection Removal with Physically-Based Training Images <Br>
**[Author]** [Soomin Kim](https://sgvr.kaist.ac.kr/~smkim/), [Yuchi Huo](https://sgvr.kaist.ac.kr/~ychuo/), [Sung-Eui Yoon](https://sgvr.kaist.ac.kr/~sungeui/)  <Br>
**[[Project](https://sgvr.kaist.ac.kr/~smkim/Reflection_removal_rendering/)]**, **[[TF-Code](https://github.com/sookim813/Reflection_removal_rendering)]**<Br>

#### *Single Image Reflection Removal Beyond Linearity*
**[Paper]** (CVPR 2019) Single Image Reflection Removal Beyond Linearity <Br>
**[Author]** Qiang Wen, Yinjie Tan, Jing Qin, Wenxi Liu, Guoqiang Han, and Shengfeng He <Br>
**[[Pytorch-Code](https://github.com/csqiangwen/Single-Image-Reflection-Removal-Beyond-Linearity)]**<Br>

#### *Learning to jointly generate and separate reflections*
**[Paper]** (ICCV 2019) Learning to jointly generate and separate reflections  <Br>
**[Author]** [Daiqian Ma](https://madaiqian.github.io/), [Renjie Wan](https://wanrenjie.github.io/, [Boxin Shi](http://ci.idm.pku.edu.cn/), [Haoliang Li](https://hlli1991.github.io/), Ling-Yu Duan  <Br>

#### perceptual-reflection-removal ★☆
**[Paper]** (CVPR 2018) Single Image Reflection Removal with Perceptual Losses <Br>
**[Author]** [Xuaner Zhang](https://people.eecs.berkeley.edu/~cecilia77/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html), [Qifeng Chen](https://cqf.io/) <Br>
**[[Project](https://people.eecs.berkeley.edu/~cecilia77/project-pages/reflection.html)]** **[[TF-Code](https://github.com/ceciliavision/perceptual-reflection-removal)]**<Br>
VGG19的多层特征作为hypercolumn与图像串联作为输入, 一个网络同时预测transmission和reflection, 使用pixel, VGG和GAN loss, 另外提出了一个gradient exclusion loss. 

#### ReflectNet
**[Paper]** (ECCV 2018) ReflectNet: Separating Reflection and Transmission Images in the Wild <Br>
**[Author]** [Patrick Wieschollek](http://patwie.com/), [Orazio Gallo](https://oraziogallo.github.io/), [Jinwei Gu](http://www.gujinwei.org/), [Jan Kautz](https://jankautz.com/)  <Br>
**[[Project](https://research.nvidia.com/publication/2018-09_Separating-Reflection-and)]** **[[TF-Code](https://github.com/NVlabs/ReflectNet)]**<Br>

#### BDN
**[Paper]** (ECCV 2018) Deep Bidirectional Estimation for Single Image Reflection Removal <Br>
**[Author]** [Jie Yang](https://github.com/yangj1e), [Dong Gong](https://donggong1.github.io)\, [Lingqiao Liu](https://sites.google.com/site/lingqiaoliu83/), [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/index.html) <Br>
**[[Pytorch-Code](https://github.com/yangj1e/bdn-refremv)]** <Br>



# Image Inpainting
#### Rethinking-Inpainting-MEDFE
**[Paper]** (ECCV 2020 Oral) Rethinking Image Inpainting via a Mutual Encoder-Decoder with Feature Equalizations<Br>
**[Author]** Hongyu Liu, Bin Jiang, [Yibing Song](https://ybsong00.github.io/), Wei Huang, Chao Yang <Br>
**[[Pytorch-Code](https://github.com/KumapowerLIU/Rethinking-Inpainting-MEDFE)]**  <Br>

#### ProFill
**[Paper]** (ECCV 2020) High-Resolution Image Inpainting with Iterative Confidence Feedback and Guided Upsampling <Br>
**[Author]** [Yu Zeng](https://zengxianyu.github.io/), [Zhe Lin](https://sites.google.com/site/zhelin625/), [Jimei Yang](https://eng.ucmerced.edu/people/jyang44), [Jianming Zhang](https://jimmie33.github.io/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/), [Huchuan Lu](https://ice.dlut.edu.cn/lu/) <Br>
**[[Project](https://zengxianyu.github.io/iic/)]** 	

#### VCNet
**[Paper]** (ECCV 2020) VCNet: A Robust Approach to Blind Image Inpainting <Br>
**[Author]** [Yi Wang](https://shepnerd.github.io/), [Ying-Cong Chen](https://yingcong.github.io/), Xin Tao, [Jiaya Jia](http://jiaya.me/) <Br>
**[[Code]](https://github.com/shepnerd/blindinpainting_vcnet)]** 
	

#### *Guidance and Evaluation: Semantic-Aware Image Inpainting for Mixed Scenes*
**[Paper]** (ECCV 2020) Guidance and Evaluation: Semantic-Aware Image Inpainting for Mixed Scenes <Br>
**[Author]** Liang Liao, Jing Xiao, [Zheng Wang](https://wangzwhu.github.io/home/), [Chia-Wen Lin](https://www.ee.nthu.edu.tw/cwlin/), [Shin'ichi Satoh](http://research.nii.ac.jp/~satoh/) <Br>
	

#### *Prior Guided GAN Based Semantic Inpainting* ★☆
**[Paper]** (CVPR 2020) Prior Guided GAN Based Semantic Inpainting <Br>
**[Author]** Avisek Lahiri, Arnav Kumar Jain, Sanskar Agrawal, Pabitra Mitra, Prabir Kumar Biswas <Br>
大致浏览. 分为两个阶段, 第一阶段训练从noise prior生成图像的generator, 第二阶段固定generator, 训练从待修复图像生成噪声先验的网络. 使用了人脸关键点作为额外的prior控制生成结果.
		
	

	

# De-raining
#### Syn2Real ★★
**[Paper]**  (CVPR 2020) Syn2Real Transfer Learning for Image Deraining using Gaussian Processes<Br>
**[Author]** [Rajeev Yasarla](https://sites.google.com/view/rajeevyasarla/home), [Vishwanath A. Sindagi](https://www.vishwanathsindagi.com/), [Vishal M. Patel](https://engineering.jhu.edu/ece/faculty/vishal-m-patel/) <Br>
**[[Pytorch-Code](https://github.com/rajeevyasarla/Syn2Real)]**<Br>
使用高斯过程计算无标签真实数据的unsupervised loss. 从paper的实验效果来看有不错的效果, 值得一试

#### MSPFN
**[Paper]**  (CVPR 2020) Multi-Scale Progressive Fusion Network for Single Image Deraining <Br>
**[Author]** [Kui Jiang](https://github.com/kuihua/kuijiang.github.io/blob/master/home.md), Zhongyuan Wang, Peng Yi, [Chen Chen](https://webpages.uncc.edu/cchen62/), Baojin Huang, Yimin Luo, [Jiayi Ma](https://sites.google.com/site/jiayima2013/), [Junjun Jiang](https://jiangjunjun.wordpress.com/) <Br>
**[[TF-Code](https://github.com/kuihua/MSPFN)]**<Br>
	
#### DRD-Net
**[Paper]**  (CVPR 2020) Detail-recovery Image Deraining via Context Aggregation Networks <Br>
**[Author]** Sen Deng, Mingqiang Wei, Jun Wang, Yidan Feng, Luming Liang, Haoran Xie, Fu Lee Wang, Meng Wang <Br>
**[[TF-Code](hhttps://github.com/Dengsgithub/DRD-Net)]**<Br>

#### DID-MDN ★☆
**[Paper]**  (CVPR 2018) Density-aware Single Image De-raining using a Multi-stream Dense Network<Br>
**[Author]** [He Zhang](https://sites.google.com/site/hezhangsprinter), [Vishal M. Patel](https://engineering.jhu.edu/vpatel36/sciencex_teams/vishalpatel/) <Br>
**[[Pytorch-Code](https://github.com/hezhangsprinter/DID-MDN)]**<Br>
基于dense connection的双分支去雨网络, 一个分支预测一个雨稠密程度的类别标签(大中小), 一个采用残差预测结构, 并结合稠密程度label, 预测去雨图像, 经过一个refinement网络输出. 加入一个预测程度的分支的策略, 在图像增强恢复任务中还是比较值得尝试的.

	
  

# Image Demoireing
#### Learnbale_Bandpass_Filter ★
**[Paper]**  (CVPR 2020) Image Demoireing with Learnable Bandpass Filters  <Br>
**[Author]** Bolun Zheng, [Shanxin Yuan](https://sites.google.com/site/shanxinyuan/), [Gregory Slabaugh](http://www.gregslabaugh.net/), [Ales Leonardis](https://www.cs.bham.ac.uk/~leonarda/) <Br>
**[[TF-Code](https://github.com/zhenngbolun/Learnbale_Bandpass_Filter)]** <Br>
在DCT变换后的频谱域做摩尔纹提取, 分为3个scale提取不同尺度的摩尔纹. 对带通去取摩尔纹的推导部分没看懂. <Br>

#### JDD
**[Paper]**  (CVPR 2020) Joint Demosaicing and Denoising With Self Guidance  <Br>
**[Author]** [Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), [Xu Jia](https://stephenjia.github.io/), Jianzhuang Liu, Qi Tian <Br>

#### *Wavelet-Based Dual-Branch Networkfor Image Demoireing*
**[Paper]** (ECCV 2020) Wavelet-Based Dual-Branch Networkfor Image Demoireing  <Br>
**[Author]**[Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), Jianzhuang Liu, [Shanxin Yuan](https://shanxinyuan.github.io/), [Gregory Slabaugh](http://www.gregslabaugh.net/), [Ales Leonardis](https://www.cs.bham.ac.uk/~leonarda/), Wengang Zhou, Qi Tian <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>
	
#### FHDe²Net
**[Paper]** (ECCV 2020) FHDe²Net: Full High Definition Demoireing Network <Br>
**[Author]** Bin He, Ce Wang, [Boxin Shi](http://ci.idm.pku.edu.cn/), Ling-Yu Duan <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>
	
#### *Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs*
**[Paper]** (NeurIPS 2020) Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs  <Br>
**[Author]** [Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), [Shanxin Yuan](https://shanxinyuan.github.io/), Jianzhuang Liu, Liping Bao, Gregory Slabaugh, Qi Tian <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>



# Style Transfer
#### *Bilateral Style Transfer* ★★
**[Paper]**  (ECCV 2020) Joint Bilateral Learning for Real-time Universal Photorealistic Style Transfer  <Br>
**[Author]** [Xide Xia](https://xidexia.github.io/), Meng Zhang, [Tianfan Xue](http://people.csail.mit.edu/tfxue/), Zheng Sun, Hui Fang, [Brian Kulis](http://people.bu.edu/bkulis/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/) <Br>
基于HDRNet的实时风格迁移, 创新点尽管不是很多, 但是工作很有价值

  

# Image Fusion
#### Deep Convolutional Network for Colorization in Monochrome-Color Dual-Lens System ★
**[Paper]** (AAAI 2019) Learning a Deep Convolutional Network for Colorization in Monochrome-Color Dual-Lens System <Br>
**[Author]**  Xuan Dong, Weixin Li, Xiaojie Wang, Yunhong Wang <Br>
1) 提出了一个Mono和Color图像融合的网络, 将融合看做对Mono图像的上色问题. 未开源, 非轻量级. <Br>
2) 分为rough和fine两部分, 首先将color图像在x方向加权求和作为rough result, 其中权值是使用3D卷积预测的weight volume; 接下来再用rough result和mono图像作为输入进行refine. <Br>

#### Stereoscopic Dark Flash ★
**[Paper]** (Siggraph 2017) Stereoscopic Dark Flash for Low-light Photography <Br>
**[Author]** [Jian Wang](https://jianwang-cmu.github.io/), [Tianfan Xue](http://people.csail.mit.edu/tfxue/), [Jonathan T. Barron](https://jonbarron.info/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/)<Br>
1) 大致浏览, 提出了一个RGB和NIR-NUV双相机成像方案, 以增强低光照条件下的图像质量. <Br>
2) 分为registration, 基于scalemap的融合, 基于HDRNet的tone correction三部分. <Br>

#### *BJND* ★☆
**[Paper]** (Optics express 2017) Enhancement of low light level images using color-plus-mono dual camera <Br>
**[Author]**   [Yong Ju Jung](https://sites.google.com/site/coolyjjung/)<Br>
1) 提出了一个融合Mono和Color图像的流程, 包括直方图匹配, 配准, Color+Color和Color+Mono的引导滤波, BJND-aware merge和detail trainsfer几个步骤. <Br>
2) 大致流程与 Digital Photography with Flash and No-Flash Image Pairs 这篇paper类似, 创新点是提出用BJND引导detail transfer. BJND即binocular just-noticeable-difference, 是根据人眼视觉系统的特性提出的. 具体方法中有很多参数和细节. <Br>
	
#### *Stereo Matching with Color and Monochrome Cameras in Low-light Conditions* ★
**[Paper]** (CVPR 2016) Stereo Matching with Color and Monochrome Cameras in Low-light Conditions <Br>
**[Author]**   [Hae-Gon Jeon](https://sites.google.com/site/hgjeoncv/), [Joon-Young Lee](https://joonyoung-cv.github.io/), [Sunghoon Im](https://sunghoonim.github.io/), [Hyowon Ha](https://sites.google.com/site/hyowoncv/), [In So Kweon](https://scholar.google.com/citations?user=XA8EOlEAAAAJ&hl=zh-CN&oi=ao) <Br>

#### Exposure Fusion ★★
**[Paper]** (Pacific Graphics 2007) Exposure Fusion <Br>
**[Author]** [Tom Mertens](http://www.mericam.net/)，[Jan Kautz](http://jankautz.com/)，Frank Van Reeth <Br>
**[[Code](https://github.com/Mericam/exposure-fusion)]**   <Br>
1) 提出了一个融合exposure bracketing图像的经典方案, 可以直接融合图像序列而无需现将其转换为HDR图像再tone mapping. <Br>
2) 使用三个指标确定每张图像的权重图, 三个指标为对比度, 饱和度和well-exposureness, 最后的权重为三个指标相乘.<Br>
3) 为消除直接逐像素融合产生的seam, 将图像和权重图分别计算分解为拉普拉斯和高斯金字塔, 在每个level做融合.

#### Digital Photography with Flash and No-Flash Image Pairs ★★
**[Paper]** (SIGGRAPH 2004) Digital Photography with Flash and No-Flash Image Pairs<Br>
**[Author]** Georg Petschnigg, [Maneesh Agrawala](http://vis.berkeley.edu/~maneesh/), [Hugues Hoppe](http://hhoppe.com/), [Richard Szeliski](http://szeliski.org/RichardSzeliski.htm), Michael Cohen, Kentaro Toyama <Br>
**[[Project](http://hhoppe.com/proj/flash/)]** **[[Code](https://github.com/pranaygupta36/DIP_PROJECT_REPO)]**<Br>
提出了一个融合Flash和Non-Flash照片的流程, 包括双边滤波, 联合双边滤波, detail提取和detail transfer. 可用于去躁, 白平衡, 去红眼, 调整flash强度等多种图像增强应用中. <Br>
	
