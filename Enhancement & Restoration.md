# Table of Contents
- [Image Enhancement](#image-enhancement)
- [Image Restoration](#image-restoration)
- [Restoration and Enhancement](#restoration-and-enhancement)
- [Image Inpainting](#image-inpainting)
- [Video Restoration and Enhancement)](#video-restoration-and-enhancement)
- [Video Inpainting](#video-inpainting)
- [Traditional Restoration](#traditional-restoration)



# Image Enhancement

### DPED ★★
**[Paper]** (ICCV 2017) DSLR-Quality Photos on Mobile Devices with Deep Convolutional Networks <Br>
**[Author]** Andrey Ignatov, Nikolay Kobyshev, Kenneth Vanhoey, Radu Timofte , Luc Van Gool  <Br>
**[[Code](http://people.ee.ethz.ch/~ihnatova/index.html)]**   <Br>
1) 从变换的角度出发, 学习一个从低质量图像到高质量图片的变换函数 
2) 变换部分采用残差快结构的CNN，定义了4个loss (color, texture, content, variance). color loss是图像进行高斯模糊后的均方差, texture loss是adversarial loss, content loss是perceptual loss, variance loss是图像梯度的模.
3) 提出了用于图像质量增强的数据集DPED, 包括iPhone, BlackBerry和Sony三种手机与Canon单反相机的图相对.
	
### HDRNet ★★
**[Paper]** (Siggraph 2017) Deep Bilateral Learning for Real-Time Image Enhancement <Br>
**[Author]** 	Michaël Gharbi, [Jiawen Chen](http://people.csail.mit.edu/jiawen/), [Jonathan T. Barron](https://jonbarron.info/),  [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Frédo Durand](http://people.csail.mit.edu/fredo/)  <Br>
**[[Project](https://groups.csail.mit.edu/graphics/hdrnet/)]**<Br>
1) 提出了一个实时图像增强网络, 速度快, 效果好. <Br>
2) 网络分为两个分支, 低分辨率分支提取特征, 学习每个像素的色彩映射参数; 高分辨率分支负责提取和保留细节信息. low res分支学到的映射参数通过类似于双线性差值的过程上采样到high res, 最后对high res图像做色彩映射并输出. <Br>
3) 学习映射参数部分, 采用bilateral grid的思路. 第三个维度被解释成8*12的网格, 意思是对8个灰度level做不同的色彩映射. 处理时选择哪个level的参数, 由high res分支生成的引导图决定. <Br> 
 
### EnhanceGAN ★ 
**[Paper]** (MM 2018) Aesthetic-Driven Image Enhancement by Adversarial Learning <Br>
**[Author]** 	Yubin Deng, [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/index.html),	[Xiaoou Tang](https://www.ie.cuhk.edu.hk/people/xotang.shtml)  <Br>
**[[Project](http://personal.ie.cuhk.edu.hk/~dy015/ImageAesthetics/EnhanceGAN.html)]** **[[Torch-Code](https://github.com/dannysdeng/EnhanceGAN)]**<Br>
1) weakly supervised方法, 学习crop和色彩变换参数, 增强aesthetic quality

### PPCN ☆
**[Paper]** (ECCVW 2018) Perception-Preserving Convolutional Networks for Image Enhancement on Smartphones <Br>
**[Author]** Zheng Hui, Xiumei Wang, Lirui Deng, [Xinbo Gao](http://see.xidian.edu.cn/faculty/xbgao/) <Br>
**[[TF-Code](https://github.com/Zheng222/PPCN)]**   <Br>
ECCV PIRM(Perceptual Image Restoration and Manipulation ) 2018竞赛, 一个快速图像增强方案

### FEQE ☆
**[Paper]** (ECCVW 2018)  Fast and Efficient Image Quality Enhancement via Desubpixel Convolutional Neural Networks <Br>
**[Author]** [Thang Vu](https://thangvubk.github.io/), Cao V. Nguyen, Trung X. Pham, Tung M. Luu, and Chang D. Yoo  <Br>
**[[TF-Code](https://github.com/thangvubk/FEQE)]**   <Br>
使用pixel shuffle的实时图像增强网络

### WESPE ★
**[Paper]** (CVPRW 2018) WESPE: Weakly Supervised Photo Enhancer for Digital Cameras <Br>
**[Author]** Andrey Ignatov, Nikolay Kobyshev, Radu Timofte , Kenneth Vanhoey, Luc Van Gool  <Br>
**[[Project](http://people.ee.ethz.ch/~ihnatova/index.html)]**   <Br>
	
### RSGUNet ★
**[Paper]** (ECCVW 2018) Range Scaling Global U-Net for Perceptual Image Enhancement on Mobile Devices <Br>
**[Author]** Jie Huang, Pengfei Zhu, Mingrui Geng, Jiewen Ran, Xingguang Zhou, Chen Xing, Pengfei Wan, Xiangyang Ji  <Br>
**[[TF-Code](https://github.com/MTlab/rsgunet_image_enhance)]**   <Br>
UNet + Global Pooling feature + 输入输出feature间的elementwise scaling
	
### CURL ★
**[Paper]** (ICLR 2020) CURL: Neural Curve Layers for Global Image Enhancement <Br>
**[Author]** [Sean Moran](http://www.seanjmoran.com/), [Steven McDonagh](https://biomedia.doc.ic.ac.uk/person/steven-mcdonagh/), [Gregory Slabaugh](http://www.gregslabaugh.net/)  <Br>
**[[Pytorch-Code](https://github.com/sjmoran/neural_curve_layers)]**  <Br>
在LAB, RGB, HSV三个空间预测curve

### FUnIE-GAN ★
**[Paper]** (RAL 2020) Fast Underwater Image Enhancement for Improved Visual Perception <Br>
**[Author]** [Md Jahidul Islam](https://xahidbuffon.github.io/), [Youya Xia](https://www.xiayouya.com/), [Junaed Sattar](https://junaedsattar.cs.umn.edu/)  <Br>
**[[Code](https://github.com/xahidbuffon/FUnIE-GAN)]**   <Br>
encoder-decoder结构, 使用了几个目标函数从各方面增强图像视觉质量. 提出了一个水下图像数据集.

### *Content-preserving Tone Adjustment* ★☆
**[Paper]** (CVPRW 2019) Content-preserving Tone Adjustment for Image Enhancement <Br>
**[Author]** [Simone Bianco](http://www.ivl.disco.unimib.it/people/simone-bianco/), [Claudio Cusano](http://www.ivl.disco.unimib.it/people/claudio-cusano/), [Flavio Piccoli](http://www.ivl.disco.unimib.it/people/flavio-piccoli/), [Raimondo Schettini](http://www.ivl.disco.unimib.it/people/raimondo-schettini/)  <Br>
**[[PyTorch-Code](https://github.com/dros1986/content-preserving-tone-adjustment-for-image-enhancement)]**   <Br>
有点类似HRDNet, 在小分辨率预测输入值的分段映射系数, 在原图上增强. 速度快, 应该有较强的实用性.

### DeepLPF ★☆
**[Paper]** (CVPR 2020) DeepLPF: Deep Local Parametric Filters for Image Enhancement <Br>
**[Author]** [Sean Moran](http://www.seanjmoran.com/), Pierre Marza, Steven McDonagh, Sarah Parisot, [Gregory Slabaugh](http://gregslabaugh.net/)  <Br>
**[[PyTorch-Code](https://github.com/huawei-noah/noah-research/tree/071a49fb8f0975192dcc919a18f9a082093122e6/DeepLPF)]**   <Br>
1) 华为欧洲实验室的文章, 把lightroom等修图软件中的brugh, graduated filters, radial filters工具用CNN模拟出来. 分为三个分支, 一个分支预测pixelwise的增强, 两个分支分别预测两种fiter的参数. 
2) 个人觉得预测的filter仍然不太够local. 不过论文的思路挺有意思.
	

### Image-Adaptive-3DLUT ★★
**[Paper]** (TPAMI 2020) Learning Image-adaptive 3D Lookup Tables for High Performance Photo Enhancement in Real-time <Br>
**[Author]** Hui Zeng, [Jianrui Cai](https://csjcai.github.io/), Lida Li, Zisheng Cao, [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
**[[Code](https://github.com/HuiZeng/Image-Adaptive-3DLUT)]**   <Br>
预测若干个3D LUT, 并用一个轻量级CNN预测每个LUT的权重. LUT和CNN同时训练, 采用了平滑和单调两种正则方式消除伪影等问题. 非常适合处理大图, 实际应用价值大, 值得一试.

### GLeNet ★★
**[Paper]** (ECCV 2020) Global and Local Enhancement Networks for Paired and Unpaired Image Enhancement <Br>
**[Author]** Han-Ul Kim, Young Jun Koh, Chang-Su Kim <Br>
**[[Project](http://mcl.korea.ac.kr/research/hukim-eccv2020-glenet/)]**   **[[Pytorch-Code](https://github.com/dongkwonjin/GleNet)]** <Br>
全局预测曲线(3*256) + 局部增强. 无监督训练部分采用类似cycle gan的策略. 更具有实用性的曲线预测策略已经开始获得关注, 相关论文越来越多了.

### PieNet ★★
**[Paper]** (ECCV 2020) PieNet: Personalized Image Enhancement Network <Br>
**[Author]** Han-Ul Kim, Young Jun Koh, Chang-Su Kim <Br>
**[[Project](http://mcl.korea.ac.kr/research/hukim-eccv2020-pienet/)]**   **[[TF-Code](https://github.com/hukim1124/PieNet)]** <Br>
使用度量学习的方法, 学习一个网络, 从用户选择的若干图像中提取偏好特征向量, 该特征向量作用在增强网络上, 产生符合用户喜好的增强结果.

### CSRNet
**[Paper]** (ECCV 2020) Conditional Sequential Modulation for Efficient Global Image Retouching <Br>
**[Author]** Jingwen He, Yihao Liu, [Yu Qiao](http://mmlab.siat.ac.cn/yuqiao/), Chao Dong <Br>
**[[Pytorch-Code](https://github.com/hejingwenhejingwen/CSRNet)]**<Br>

### Early Exit or Not
**[Paper]** (ECCV 2020) Early Exit or Not: Resource-Efficient Blind Quality Enhancement for Compressed Images <Br>
**[Author]** [Qunliang Xing](https://ryanxingql.github.io/), Mai Xu, Tianyi Li, Zhenyu Guan <Br>
**[[Pytorch-Code](https://github.com/RyanXingQL/RBQE)]**<Br>
	
### URIE
**[Paper]** (ECCV 2020) URIE: Universal Image Enhancement for Visual Recognition in the Wild <Br>
**[Author]** Taeyoung Son, Juwon Kang, Namyup Kim, [Sunghyun Cho](https://www.scho.pe.kr/), [Suha Kwak](http://cvlab.postech.ac.kr/~suhakwak/) <Br>
**[[Project](http://cvlab.postech.ac.kr/research/URIE/)]** **[[Pytorch-Code](https://github.com/taeyoungson/urie)]**<Br>
	
	
	
# Image Restoration
	
### DualCNN ★
**[Paper]**  (CVPR 2018) Learning Dual Convolutional Neural Networks for Low-Level Vision  <Br>
**[Author]** [Jinshan Pan](https://sites.google.com/site/jspanhomepage/), [Sifei Liu](https://www.sifeiliu.net/), Deqing Sun, [Jiawei Zhang](https://sites.google.com/site/zhjw1988), Yang Liu, [Jimmy Ren](http://www.jimmyren.com/), Zechao Li, Jinhui Tang, [Huchuan Lu](http://ice.dlut.edu.cn/lu/), Yu-Wing Tai, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/)  <Br>
**[[Project](https://sites.google.com/site/jspanhomepage/dualcnn)]** **[[Unofficial-TF-Code](https://github.com/galad-loth/DualCNN-TF)]**  <Br>
  粗读, 设计了一双分支网络, 一个学习detail, 一个学习structure, 针对任务对两个分支也分别进行监督训练 <Br>

### Deep Image Prior ★★
**[Paper]** (CVPR 2018) Deep Image Prior <Br>
**[Author]** [Dmitry Ulyanov](https://dmitryulyanov.github.io/about), [Andrea Vedald](https://www.robots.ox.ac.uk/~vedaldi/), [Victor Lempitsky](http://sites.skoltech.ru/compvision/members/vilem/)<Br>
**[[Project](https://dmitryulyanov.github.io/deep_image_prior)]**  <Br>
1) 一篇有趣的论文, 提出深度卷积网络在图像生成和恢复任务中表现好的原因, 可能并不是因为其从大量图像中学习到了某种先验, 其实随机初始化的网络足以从输入中抓取大量的low-level图像先验信息. 在通过迭代的方式从图像中学习先验的过程中, 那些自然的, 有规律的内容较容易提取,会先被学习出来, 因此就达到了去噪或其它restoration的目的. <Br>
2) 粗读, 实用性有待验证, 有时间可以好好研究一下. <Br>
	
### DuRN ★☆
**[Paper]** (CVPR 2019) Dual Residual Networks Leveraging the Potential of Paired Operations for Image Restoration<Br>
**[Author]** Xing Liu, [Masanori Suganuma](https://sites.google.com/site/suganumamasanori/eng), Zhun Sun, Takayuki Okatani<Br>
**[[Code](https://github.com/liu-vis/DualResidualNetworks)]**  <Br>
1) 文章提出, 许多图像复原任务都由一些成对的模块组成, 比如去噪里的大kernel和小kernel, 超分里的下采样和上采样. 本文在residual connection的基础上, 进一步给每个模块内部的操作直接加入residual connection, 增加了组合数. <Br>
2) 在去噪, 去模糊, 去雾等任务中都取得了不错的效果. <Br>
	
### OperationAttention ★☆
**[Paper]** (CVPR 2019) Attention-based Adaptive Selection of Operations for Image Restoration in the Presence of Unknown Combined Distortions<Br>
**[Author]** [Masanori Suganuma](https://sites.google.com/site/suganumamasanori/eng), Xing Liu, Takayuki Okatani<Br>
**[[Code](https://github.com/sg-nm/Operation-wise-attention-network)]** <Br>
1) 提出用一个基于attention的操作加权网络, 用来处理不同种类的degradation. <Br>
2) 性能一般, 不太容易收敛, 思路值得借鉴. <Br>

### CFSNet ★
**[Paper]** (ICCV 2019) CFSNet: Toward a Controllable Feature Space for Image Restoration<Br>
**[Author]** Wei Wang, Ruiming Guo, [Yapeng Tian](http://yapengtian.org/), Wenming Yang<Br>
**[[Pytorch-Code](https://github.com/qibao77/CFSNet)]** <Br>
粗读, 用一个手动输入的参数控制两个分支的权重, 一个分支负责low distortion修复, 另一个分支负责high visual quality. 两个分支通过使用不同loss (L1, L2 v.s. vgg, GAN loss) 训练来得到. 文章的效果和实用性有待检验, 思路可借鉴. <Br>
	
### GCANet
**[Paper]** (WACV 2019) Gated Context Aggregation Network for Image Dehazing and Deraining <Br>
**[Author]** [Dongdong Chen](http://www.dongdongchen.bid/), Mingming He, [Qingnan Fan](https://fqnchina.github.io/)  <Br>
**[[Code](https://github.com/cddlyf/GCANet)]**  <Br>	

### DGP
**[Paper]** (ECCV 2020 Oral) Exploiting Deep Generative Prior for Versatile Image Restoration and Manipulation <Br>
**[Author]** [Xingang Pan](https://xingangpan.github.io/), [Xiaohang Zhan](https://xiaohangzhan.github.io/), [Bo Dai](http://daibo.info/), [Dahua Lin](http://dahua.site/), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/), [Ping Luo](http://luoping.me/) <Br>
**[[Pytorch-Code](https://github.com/XingangPan/deep-generative-prior)]** <Br>
	
### *Stacking Networks Dynamically for Image Restoration Based on the Plug-and-Play Framework*
**[Paper]** (ECCV 2020) Stacking Networks Dynamically for Image Restoration Based on the Plug-and-Play Framework <Br>
**[Author]** Haixin Wang, Tianhao Zhang, Muzhi Yu, Jinan Sun, Wei Ye, Chen Wang, Shikun Zhang <Br>	

### LIRA
**[Paper]** (ECCV 2020) LIRA: Lifelong Image Restoration from Unknown Blended Distortions <Br>
**[Author]** Jianzhao Liu, [Jianxin Lin](http://home.ustc.edu.cn/~linjx/), Xin Li, Wei Zhou, Sen Liu, [Zhibo Chen](http://staff.ustc.edu.cn/~chenzhibo/) <Br>	

### CResMD
**[Paper]** (ECCV 2020) Interactive Multi-Dimension Modulation with Dynamic Controllable Residual Learning for Image Restoration <Br>
**[Author]** Jingwen He, Chao Dong, [Yu Qiao](http://mmlab.siat.ac.cn/yuqiao/) <Br>
**[[Pytorch-Code](https://github.com/hejingwenhejingwen/CResMD)]** <Br>

### DeepWienerRestoration
**[Paper]** (ECCV 2020) Microscopy Image Restoration with Deep Wiener-Kolmogorov filters <Br>
**[Author]** [Valeriya Pronina](https://vpronina.github.io/), [Filippos Kokkinos](https://fkokkinos.github.io/), Dmitry V. Dylov, Stamatios Lefkimmiatis <Br>
**[[Project]https://vpronina.github.io/resources/project.htm)]** **[[Pytorch-Code](https://github.com/vpronina/DeepWienerRestoration/)]** <Br>
	
### GroupSC
**[Paper]** (ECCV 2020) Fully Trainable and Interpretable Non-Local Sparse Models for Image Restoration <Br>
**[Author]** Bruno Lecouat, [Jean Ponce](https://www.di.ens.fr/~ponce/), [Julien Mairal](http://thoth.inrialpes.fr/people/mairal/) <Br>
**[[Pytorch-Code](https://github.com/bruno-31/groupsc)]** <Br>
	
### *Learning Disentangled Feature Representation for Hybrid-distorted Image Restoration*
**[Paper]** (ECCV 2020) Learning Disentangled Feature Representation for Hybrid-distorted Image Restoration <Br>
**[Author]** Xin Li, Xin Jin, [Jianxin Lin](http://home.ustc.edu.cn/~linjx/), Tao Yu, Sen Liu, Yaojun Wu, Wei Zhou, [Zhibo Chen](http://staff.ustc.edu.cn/~chenzhibo/)  <Br>
**[[Pytorch-Code](https://github.com/bruno-31/groupsc)]** <Br>
	
		

# Restoration and Enhancement
### MIRNet ★
**[Paper]** (ECCV 2020)  Learning Enriched Features for Real Image Restoration and Enhancement<Br>
**[Author]**  [Syed Waqas Zamir](https://scholar.google.es/citations?user=WNGPkVQAAAAJ&hl=en), [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Munawar Hayat](https://scholar.google.com/citations?user=Mx8MbWYAAAAJ&hl=en), [Fahad Shahbaz Khan](https://scholar.google.es/citations?user=zvaeYnUAAAAJ&hl=en), [Ming-Hsuan Yang](https://scholar.google.com/citations?user=p9-ohHsAAAAJ&hl=en), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en)  <Br>
**[[Pytorch-Code](https://github.com/swz30/MIRNet)]**  <Br>
提出了一个就多尺度特征融合的网络用于去噪, 超分, 增强等任务. 使用attention的思想设计了很多模块, 性能不错, 在各种任务上适用性看起来较强



# Image Inpainting
### Rethinking-Inpainting-MEDFE
**[Paper]** (ECCV 2020 Oral) Rethinking Image Inpainting via a Mutual Encoder-Decoder with Feature Equalizations<Br>
**[Author]** Hongyu Liu, Bin Jiang, [Yibing Song](https://ybsong00.github.io/), Wei Huang, Chao Yang <Br>
**[[Pytorch-Code](https://github.com/KumapowerLIU/Rethinking-Inpainting-MEDFE)]**  <Br>

### ProFill
**[Paper]** (ECCV 2020) High-Resolution Image Inpainting with Iterative Confidence Feedback and Guided Upsampling <Br>
**[Author]** [Yu Zeng](https://zengxianyu.github.io/), [Zhe Lin](https://sites.google.com/site/zhelin625/), [Jimei Yang](https://eng.ucmerced.edu/people/jyang44), [Jianming Zhang](https://jimmie33.github.io/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/), [Huchuan Lu](https://ice.dlut.edu.cn/lu/) <Br>
**[[Project](https://zengxianyu.github.io/iic/)]** 	

### VCNet
**[Paper]** (ECCV 2020) VCNet: A Robust Approach to Blind Image Inpainting <Br>
**[Author]** [Yi Wang](https://shepnerd.github.io/), [Ying-Cong Chen](https://yingcong.github.io/), Xin Tao, [Jiaya Jia](http://jiaya.me/) <Br>
**[[Code]](https://github.com/shepnerd/blindinpainting_vcnet)]** 
	
### *Guidance and Evaluation: Semantic-Aware Image Inpainting for Mixed Scenes*
**[Paper]** (ECCV 2020) Guidance and Evaluation: Semantic-Aware Image Inpainting for Mixed Scenes <Br>
**[Author]** Liang Liao, Jing Xiao, [Zheng Wang](https://wangzwhu.github.io/home/), [Chia-Wen Lin](https://www.ee.nthu.edu.tw/cwlin/), [Shin'ichi Satoh](http://research.nii.ac.jp/~satoh/) <Br>
	
	
	

# Video Restoration and Enhancement
### ST-SR
**[Paper]**  (CVPR 2020) Space-Time-Aware Multi-Resolution Video Enhancement<Br>
**[Author]** [Muhammad Haris](https://alterzero.github.io/), [Greg Shakhnarovich](https://ttic.uchicago.edu/~gregory/), [Norimichi Ukita](https://www.toyota-ti.ac.jp/Lab/Denshi/iim/ukita/) <Br>
**[[Project](https://alterzero.github.io/projects/STAR.html)]** **[[Pytorch-Code](https://github.com/alterzero/STARnet)]**<Br>


# Video Inpainting
### *Short-Term and Long-Term Context Aggregation Network for Video Inpainting*
**[Paper]** (ECCV 2020) Short-Term and Long-Term Context Aggregation Network for Video Inpainting <Br>
**[Author]** [Ang Li](https://angliunimelb.github.io/), [Shanshan Zhao](https://sshan-zhao.github.io/), [Xingjun Ma](http://xingjunma.com/), [Mingming Gong](https://mingming-gong.github.io/), [Jianzhong Qi](https://people.eng.unimelb.edu.au/jianzhongq/), [Rui Zhang](http://www.ruizhang.info/), [Dacheng Tao](https://www.sydney.edu.au/engineering/about/our-people/academic-staff/dacheng-tao.html), [Ramamohanarao Kotagirig](http://www.cloudbus.org/rao/) <Br>

### STTN
**[Paper]** (ECCV 2020) Learning Joint Spatial-Temporal Transformations for Video Inpainting  <Br>
**[Author]** [Yanhong Zeng](https://sites.google.com/view/1900zyh), [Jianlong Fu](https://jianlong-fu.github.io/), Hongyang Chao <Br>
**[[Pytorch-Code]](https://github.com/researchmm/STTN)]** 

### DVI
**[Paper]** (ECCV 2020) DVI: Depth Guided Video Inpainting for Autonomous Driving <Br>
**[Author]** Miao Liao, Feixiang Lu, Dingfu Zhou, [Sibo Zhang](https://sites.google.com/view/sibozhang/home), Wei Li, [Ruigang Yang](http://www.vis.uky.edu/~ryang/) <Br>
**[[Project]](https://sites.google.com/view/sibozhang/dvi)]** **[[Code]](https://github.com/sibozhang/Depth-Guided-Inpainting)]** 

### Depth-Guided-Inpainting
**[Paper]** (ECCV 2020) Learning Joint Spatial-Temporal Transformations for Video Inpainting <Br>
**[Author]** Miao Liao, Feixiang Lu, Dingfu Zhou, [Sibo Zhang](https://sites.google.com/view/sibozhang/home), Wei Li, [Ruigang Yang](http://www.vis.uky.edu/~ryang/) <Br>
**[[Project]](https://sites.google.com/view/sibozhang/dvi)]** **[[Code]](https://github.com/sibozhang/Depth-Guided-Inpainting)]** 
	
	
	
# Traditional Restoration

### Reproduction Angular Error ★
**[Paper]** (BMVC 2014)  Reproduction Angular Error: An Improved Performance Metric for Illuminant Estimation <Br>
**[Author]**   Graham Finlayson, Roshanak Zakizadeh  <Br>
1) 提出了一个用于评估illuminant estimation性能的准则, 该准则与光源的色温无关. 大致浏览, 一些原理没看懂. <Br>
2) 后面Google在此基础上做了改进, 作为loss去训练低光照时AWB模型. <Br>

### Discriminative Prior ☆
**[Paper]**  (CVPR 2018) Learnign a Discriminative Prior for Blind Image Deblurring  <Br>
**[Author]** [Lerenhan Li](https://sites.google.com/view/lerenhanli/homepage), [Jinshan Pan](https://sites.google.com/site/jspanhomepage/), [Wei-Sheng Lai](http://graduatestudents.ucmerced.edu/wlai24/), [Changxin Gao](https://sites.google.com/site/changxingao/home), Nong Sang     [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Project](https://sites.google.com/view/lerenhanli/homepage/learn_prior_deblur)]** <Br>
用CNN学习一个deblur用的prior, 用来提供输入图像是否模糊的先验知识, 把该prior加入目标函数, 之后用迭代的方法求解优化函数 <Br>
	


