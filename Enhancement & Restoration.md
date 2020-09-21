# Table of Contents
- [Image Enhancement](#image-enhancement)
- [Image Restoration](#image-restoration)
- [Restoration&Enhancementn](#restoration-&-enhancement)
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
**[Author]**Zheng Hui, Xiumei Wang, Lirui Deng, [Xinbo Gao](http://see.xidian.edu.cn/faculty/xbgao/) <Br>
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
	
### *Low-Light Image Enhancement via a Deep Hybrid Network*
**[Paper]** (TIP 2019) Low-Light Image Enhancement via a Deep Hybrid Network <Br>
**[Author]** [Wenqi Ren](https://sites.google.com/site/renwenqi888/home), [Sifei Liu](https://www.sifeiliu.net/), [Lin Ma](http://forestlinma.com/), [Qianqian Xu](https://qianqianxu010.github.io/), [Xiangyu Xu](https://sites.google.com/view/xiangyuxu), [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en), Junping Du, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/)  <Br>
**[[Code](https://sites.google.com/site/renwenqi888/home)]**   <Br>	

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
**[Author]** [Sean Moran](http://www.seanjmoran.com/), Pierre Marza, [Steven McDonagh], Sarah Parisot, [Gregory Slabaugh](http://gregslabaugh.net/)  <Br>
**[[PyTorch-Code](https://github.com/huawei-noah/noah-research/tree/071a49fb8f0975192dcc919a18f9a082093122e6/DeepLPF)]**   <Br>
1) 华为欧洲实验室的文章, 把lightroom等修图软件中的brugh, graduated filters, radial filters工具用CNN模拟出来. 分为三个分支, 一个分支预测pixelwise的增强, 两个分支分别预测两种fiter的参数. 
2) 个人觉得预测的filter仍然不太够local. 不过论文的思路挺有意思.
	



	
	
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
	



# Restoration & Enhancement
### MIRNet
**[Paper]** (ECCV 2030)  Learning Enriched Features for Real Image Restoration and Enhancement<Br>
**[Author]**  [Syed Waqas Zamir](https://scholar.google.es/citations?user=WNGPkVQAAAAJ&hl=en), [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Munawar Hayat](https://scholar.google.com/citations?user=Mx8MbWYAAAAJ&hl=en), [Fahad Shahbaz Khan](https://scholar.google.es/citations?user=zvaeYnUAAAAJ&hl=en), [Ming-Hsuan Yang](https://scholar.google.com/citations?user=p9-ohHsAAAAJ&hl=en), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en)  <Br>
**[[Pytorch-Code](https://github.com/swz30/MIRNet)]**  <Br>


	
	
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
	


