# Table of Contents
- [Image Restoration](#image-restoration)
- [Image Dehazing](#image-dehazing)
- [Image Debluring](#image-debluring)
- [Reflection Removal](#reflection-removal)
- [Image Inpainting](#image-inpainting)
- [De-raining (Archived)](#de-raining)
- [Image Demoireing (Archived)](#image-demoireing)



# Image Restoration
#### Dual Pixel Exploration
**[Paper]** (CVPR 2021 Oral) Dual Pixel Exploration: Simultaneous Depth Estimation and Image Restoration  <Br>
**[Author]**  Liyuan Pan, Shah Chowdhury, [Richard Hartley](http://users.cecs.anu.edu.au/~hartley/), [Miaomiao Liu](http://users.cecs.anu.edu.au/~mliu/), [Hongguang Zhang](https://hongguangzhang.github.io/), [Hongdong Li](https://cecs.anu.edu.au/~hongdong) <Br>
**[[Code](https://github.com/panpanfei/Dual-Pixel-Exploration-Simultaneous-Depth-Estimation-and-Image-Restoration)]** <Br>

#### DISCNet ★★
**[Paper]** (CVPR 2021) Removing Diffraction Image Artifacts in Under-Display Camera via Dynamic Skip Connection Networks  <Br>
**[Author]** [Ruicheng Feng](https://jnjaby.github.io/), [Chongyi Li](https://li-chongyi.github.io/), [Huaijin Chen](https://hc25.web.rice.edu), Shuai Li, [Chen Change Loy](https://personal.ie.cuhk.edu.hk/~ccloy/), [Jinwei Gu](https://www.gujinwei.org/) <Br>
**[[Project](https://jnjaby.github.io/projects/UDC/)]** **[[Pytorch-Code](https://github.com/jnjaby/DISCNet)]** <Br>
(**UDC图像修复**) 使用中兴UDC相机, 模拟Point Spread Function(PSF), 并生成数据集. 网络使用动态卷积, 并加入PSF kernel, 为模型提供先验信息. 

#### Image Restoration for UDC
**[Paper]** (CVPR 2021) Image Restoration for Under-Display Camera   <Br>
**[Author]** [Yuqian Zhou](https://yzhouas.github.io/), David Ren, [Neil Emerton](https://www.microsoft.com/applied-sciences/people/neil-emerton), [Sehoon Lim](https://www.microsoft.com/applied-sciences/people/sehoon-lim), [Timothy Large](https://www.microsoft.com/applied-sciences/people/tim-large) <Br>
**[[Project](https://yzhouas.github.io/projects/UDC/udc.html)]** <Br>

#### MPRNet ★
**[Paper]** (CVPR 2021) Multi-Stage Progressive Image Restoration <Br>
**[Author]** [Syed Waqas Zamir](https://scholar.google.es/citations?user=WNGPkVQAAAAJ&hl=en), [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Munawar Hayat](https://scholar.google.com/citations?user=Mx8MbWYAAAAJ&hl=en), [Fahad Shahbaz Khan](https://scholar.google.es/citations?user=zvaeYnUAAAAJ&hl=en), [Ming-Hsuan Yang](https://scholar.google.com/citations?user=p9-ohHsAAAAJ&hl=en), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en) <Br>
**[[Pytorch-Code](https://github.com/swz30/MPRNet)]** <Br>
多阶段结构, 用了attention等一些trick

#### PANet 
**[Paper]** (arXiv 2004) Pyramid Attention Networks for Image Restoration <Br>
**[Author]** [Yiqun Mei](https://yiqunmei.net/), [Yuchen Fan](https://ychfan.github.io/), [Yulun Zhang](http://yulunzhang.com/), [Jiahui Yu](https://jiahuiyu.com/), [Yuqian Zhou](https://yzhouas.github.io/), Ding Liu, Yun Fu, [Thomas S. Huang](http://ifp-uiuc.github.io/), [Humphrey Shi](https://www.humphreyshi.com/) <Br>
**[[Pytorch-Code](https://github.com/SHI-Labs/Pyramid-Attention-Networks)]** <Br>
	
#### NSR
**[Paper]** (NeurIPS 2020) Neural Sparse Representation for Image Restoration <Br>
**[Author]** [Yuchen Fan](https://ychfan.github.io/), [Jiahui Yu](https://jiahuiyu.com/), [Yiqun Mei](https://yiqunmei.net/), [Yulun Zhang](http://yulunzhang.com/), Yun Fu, Ding Liu, [Thomas S. Huang](http://ifp-uiuc.github.io/) <Br>
**[[Code](https://github.com/ychfan/nsr)]** <Br>

#### SCN
**[Paper]** (AAAI 2020) Scale-wise Convolution for Image Restoration <Br>
**[Author]** [Yuchen Fan](https://ychfan.github.io/), [Jiahui Yu](https://jiahuiyu.com/), Ding Liu, [Thomas S. Huang](http://ifp-uiuc.github.io/) <Br>
**[[Pytorch-Code](https://github.com/ychfan/scn)]** <Br>
	
#### DGP ★★
**[Paper]** (ECCV 2020 Oral) Exploiting Deep Generative Prior for Versatile Image Restoration and Manipulation <Br>
**[Author]** [Xingang Pan](https://xingangpan.github.io/), [Xiaohang Zhan](https://xiaohangzhan.github.io/), [Bo Dai](http://daibo.info/), [Dahua Lin](http://dahua.site/), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/), [Ping Luo](http://luoping.me/) <Br>
**[[Pytorch-Code](https://github.com/XingangPan/deep-generative-prior)]** <Br>
提出用预训练的GAN作为先验, 无需在特定任务上finetune, 即可实现超分, 上色等图像恢复任务和图像变形，类别转换等图像编辑功能. 论文主要是在一般GAN inversion的基础上, 提出同时优化隐向量z和生成网络参数, 达到了更好更自然的效果.

#### Stacking Networks Dynamically for Image Restoration
**[Paper]** (ECCV 2020) Stacking Networks Dynamically for Image Restoration Based on the Plug-and-Play Framework <Br>
**[Author]** Haixin Wang, Tianhao Zhang, Muzhi Yu, Jinan Sun, Wei Ye, Chen Wang, Shikun Zhang <Br>	

#### SNSC ★
**[Paper]** (ECCV 2020) Blind Image Restoration without Prior Knowledge <Br>
**[Author]** Noam Elron, Shahar S. Yuval, [Dmitry Rudoy](https://dmitryrudoy.wixsite.com/dmitryrudoy), Noam Lev <Br>	
提出了一个Self-Normalization Side-Chain模块, 用来提取全局信息

#### LIRA
**[Paper]** (ECCV 2020) LIRA: Lifelong Image Restoration from Unknown Blended Distortions <Br>
**[Author]** Jianzhao Liu, [Jianxin Lin](http://home.ustc.edu.cn/~linjx/), Xin Li, Wei Zhou, Sen Liu, [Zhibo Chen](http://staff.ustc.edu.cn/~chenzhibo/) <Br>	

#### CResMD ★
**[Paper]** (ECCV 2020) Interactive Multi-Dimension Modulation with Dynamic Controllable Residual Learning for Image Restoration <Br>
**[Author]** Jingwen He, Chao Dong, [Yu Qiao](http://mmlab.siat.ac.cn/yuqiao/) <Br>
**[[Pytorch-Code](https://github.com/hejingwenhejingwen/CResMD)]** <Br>
**(控制restoration level)**	 将控制参数由一个扩展为多个, 处理不同种类不同程度的退化, 输入的参数由若干FC层处理为权值vector, 作为残差块中的卷积分支的scale. 提出了一些trick训练不同退化的数据. 虽然论文表示可以处理多种退化情形, 但是用户手动调节两个甚至更多参数还是挺麻烦的.

#### DeepWienerRestoration
**[Paper]** (ECCV 2020) Microscopy Image Restoration with Deep Wiener-Kolmogorov filters <Br>
**[Author]** [Valeriya Pronina](https://vpronina.github.io/), [Filippos Kokkinos](https://fkokkinos.github.io/), Dmitry V. Dylov, Stamatios Lefkimmiatis <Br>
**[[Project](https://vpronina.github.io/resources/project.htm)]** **[[Pytorch-Code](https://github.com/vpronina/DeepWienerRestoration/)]** <Br>
	
#### GroupSC
**[Paper]** (ECCV 2020) Fully Trainable and Interpretable Non-Local Sparse Models for Image Restoration <Br>
**[Author]** Bruno Lecouat, [Jean Ponce](https://www.di.ens.fr/~ponce/), [Julien Mairal](http://thoth.inrialpes.fr/people/mairal/) <Br>
**[[Pytorch-Code](https://github.com/bruno-31/groupsc)]** <Br>

#### Learning Disentangled Feature Representation ★
**[Paper]** (ECCV 2020) Learning Disentangled Feature Representation for Hybrid-distorted Image Restoration <Br>
**[Author]** Xin Li, Xin Jin, [Jianxin Lin](http://home.ustc.edu.cn/~linjx/), Tao Yu, Sen Liu, Yaojun Wu, Wei Zhou, [Zhibo Chen](http://staff.ustc.edu.cn/~chenzhibo/)  <Br>
**(处理多种退化)** 大致浏览, 通过gain-control-based normalization学习解耦特征, 并据此设计了几个模块, 处理多种退化混合问题. 文中使用了spectral value dierence orthogonality regularization作为一个loss, 促使feature map直接学到不相关的信息.

#### MIRNet ★
**[Paper]** (ECCV 2020)  Learning Enriched Features for Real Image Restoration and Enhancement<Br>
**[Author]**  [Syed Waqas Zamir](https://scholar.google.es/citations?user=WNGPkVQAAAAJ&hl=en), [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Munawar Hayat](https://scholar.google.com/citations?user=Mx8MbWYAAAAJ&hl=en), [Fahad Shahbaz Khan](https://scholar.google.es/citations?user=zvaeYnUAAAAJ&hl=en), [Ming-Hsuan Yang](https://scholar.google.com/citations?user=p9-ohHsAAAAJ&hl=en), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en)  <Br>
**[[Pytorch-Code](https://github.com/swz30/MIRNet)]**  <Br>
提出了一个就多尺度特征融合的网络用于去噪, 超分, 增强等任务. 使用attention的思想设计了很多模块, 性能不错, 在各种任务上适用性看起来较强
	
#### *Bringing Old Photos Back to Life* ★★☆
**[Paper]** (CVPR 2020 Oral) Bringing Old Photos Back to Life <Br>
**[Author]** [Ziyu Wan](http://raywzy.com/), [Bo Zhang](https://www.microsoft.com/en-us/research/people/zhanbo/), [Dongdong Chen](http://www.dongdongchen.bid/), [Pan Zhang](https://panzhang0212.github.io/), [Dong Chen](https://www.microsoft.com/en-us/research/people/doch/), [Jing Liao](https://liaojing.github.io/html/), [Fang Wen](https://www.microsoft.com/en-us/research/people/fangwen/)  <Br>
**[[Project](http://raywzy.com/Old_Photo/)]** <Br>**(无监督, domain transfer)**  无监督老照片恢复, 用生成的老照片训练, 在真实老照片上取得好效果. 使用一个VAE将真实和生成的照片映射到相近的空间, 第二个VAE负责恢复无损照片, 中间还有一些映射等操作. 

#### DualCNN ★
**[Paper]**  (CVPR 2018) Learning Dual Convolutional Neural Networks for Low-Level Vision  <Br>
**[Author]** [Jinshan Pan](https://sites.google.com/site/jspanhomepage/), [Sifei Liu](https://www.sifeiliu.net/), Deqing Sun, [Jiawei Zhang](https://sites.google.com/site/zhjw1988), Yang Liu, [Jimmy Ren](http://www.jimmyren.com/), Zechao Li, Jinhui Tang, [Huchuan Lu](http://ice.dlut.edu.cn/lu/), Yu-Wing Tai, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/)  <Br>
**[[Project](https://sites.google.com/site/jspanhomepage/dualcnn)]** **[[Unofficial-TF-Code](https://github.com/galad-loth/DualCNN-TF)]**  <Br>
  粗读, 设计了一双分支网络, 一个学习detail, 一个学习structure, 针对任务对两个分支也分别进行监督训练 <Br>

#### Deep Image Prior ★★
**[Paper]** (CVPR 2018) Deep Image Prior <Br>
**[Author]** [Dmitry Ulyanov](https://dmitryulyanov.github.io/about), [Andrea Vedald](https://www.robots.ox.ac.uk/~vedaldi/), [Victor Lempitsky](http://sites.skoltech.ru/compvision/members/vilem/)<Br>
**[[Project](https://dmitryulyanov.github.io/deep_image_prior)]**  <Br>
**(zero-shot)**	
1) 一篇有趣的论文, 提出深度卷积网络在图像生成和恢复任务中表现好的原因, 可能并不是因为其从大量图像中学习到了某种先验, 其实随机初始化的网络足以从输入中抓取大量的low-level图像先验信息. 在通过迭代的方式从图像中学习先验的过程中, 那些自然的, 有规律的内容较容易提取,会先被学习出来, 因此就达到了去噪或其它restoration的目的. <Br>
2) 粗读, 实用性有待验证, 有时间可以好好研究一下. <Br>

#### DuRN ★☆
**[Paper]** (CVPR 2019) Dual Residual Networks Leveraging the Potential of Paired Operations for Image Restoration<Br>
**[Author]** Xing Liu, [Masanori Suganuma](https://sites.google.com/site/suganumamasanori/eng), Zhun Sun, Takayuki Okatani<Br>
**[[Code](https://github.com/liu-vis/DualResidualNetworks)]**  <Br>
1) 文章提出, 许多图像复原任务都由一些成对的模块组成, 比如去噪里的大kernel和小kernel, 超分里的下采样和上采样. 本文在residual connection的基础上, 进一步给每个模块内部的操作直接加入residual connection, 增加了组合数. <Br>
2) 在去噪, 去模糊, 去雾等任务中都取得了不错的效果. <Br>
	
#### OperationAttention ★☆
**[Paper]** (CVPR 2019) Attention-based Adaptive Selection of Operations for Image Restoration in the Presence of Unknown Combined Distortions<Br>
**[Author]** [Masanori Suganuma](https://sites.google.com/site/suganumamasanori/eng), Xing Liu, Takayuki Okatani<Br>
**[[Code](https://github.com/sg-nm/Operation-wise-attention-network)]** <Br>
**(处理多种退化)**	 提出用一个基于attention的操作加权网络, 用来处理不同种类的degradation. 性能一般, 不太容易收敛, 思路值得借鉴. <Br>

#### AdaFM ★☆
**[Paper]** (CVPR 2019) Modulating Image Restoration with Continual Levels via Adaptive Feature Modification Layers<Br>
**[Author]** Jingwen He, Chao Dong, [Yu Qiao](http://mmlab.siat.ac.cn/yuqiao/)  <Br>
**[[Pytorch-Code](https://github.com/hejingwenhejingwen/AdaFM)]**   <Br>
**(控制restoration level)**	提出了一个AdaFM模块, 用于控制网络对图像的修复程度. AdaFM模块实际上就是一个dw conv层, 通过手动控制该层的权重, 达到控制修复程度的目的. 论文这么做是基于两个发现: 1) 对于不同restoration level, 网络提取的visual patterns是相似的, 只是weights不同; 2)调整网络内部参数对输出的影响是连续的.
	

#### CFSNet ★
**[Paper]** (ICCV 2019) CFSNet: Toward a Controllable Feature Space for Image Restoration<Br>
**[Author]** Wei Wang, Ruiming Guo, [Yapeng Tian](http://yapengtian.org/), Wenming Yang<Br>
**[[Pytorch-Code](https://github.com/qibao77/CFSNet)]** <Br>
**(控制restoration level)**	 粗读, 用一个手动输入的参数控制两个分支的权重, 一个分支负责low distortion修复, 另一个分支负责high visual quality. 两个分支通过使用不同loss (L1, L2 v.s. vgg, GAN loss) 训练来得到. 文章的效果和实用性有待检验, 思路可借鉴. <Br>
	
#### GCANet ★
**[Paper]** (WACV 2019) Gated Context Aggregation Network for Image Dehazing and Deraining <Br>
**[Author]** [Dongdong Chen](http://www.dongdongchen.bid/), Mingming He, [Qingnan Fan](https://fqnchina.github.io/)  <Br>
**[[Code](https://github.com/cddlyf/GCANet)]**  <Br>	
在dilation卷积前加入可分离卷积, 消除grid effect. 除去雾去雨外应该也适合其它任务.






# Image Dehazing
#### Dehazing via Multi-Guided Bilateral Learning
**[Paper]** (CVPR 2021) Ultra-High-Definition Image Dehazing via Multi-Guided Bilateral Learning <Br>
**[Author]** Zhuoran Zheng, [Wenqi Ren](https://sites.google.com/site/renwenqi888/home), [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en), Xiaobin Hu, Tao Wang, Fenglong Song, Xiuyi Jia <Br>

#### AECR-Net
**[Paper]** (CVPR 2021) Contrastive Learning for Compact Single Image Dehazing  <Br>
**[Author]** Haiyan Wu, [Yanyun Qu](https://quyanyun.xmu.edu.cn/), [Shaohui Lin](https://sites.google.com/site/shaohuilin007/home) <Br>
**[[Pytorch-Code](https://github.com/GlassyWu/AECR-Net)]**  <Br>

#### Physics-based Feature Dehazing
**[Paper]**  (ECCV 2020)  Physics-based Feature Dehazing Networks  <Br>
**[Author]**  Jiangxin Dong, [Jinshan Pan](https://jspan.github.io/) <Br>
**[[Project](https://jspan.github.io/)]**  <Br>

#### MSBDN-DFF ★☆
**[Paper]**  (CVPR 2020) Multi-Scale Boosted Dehazing Network with Dense Feature Fusion <Br>
**[Author]**  [Hang Dong](https://sites.google.com/view/hdong/%E9%A6%96%E9%A1%B5), [Jinshan Pan](https://jspan.github.io/), [Zhe Hu](https://zjuela.github.io/), Xiang Lei, [Xinyi Zhang](http://xinyizhang.tech/), Fei Wang, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Pytorch-Code](https://github.com/BookerDeWitt/MSBDN-DFF)]**  <Br>
粗读, Unet结合超分中的Deep Back-Projection, 有时间可以研究一下反投影的原理和代码


#### DA_dahazing ★☆
**[Paper]**  (CVPR 2020) Domain Adaptation for Image Dehazing <Br>
**[Author]**  Yuanjie Shao, [Lerenhan Li](https://sites.google.com/view/lerenhanli/homepage), [Wenqi Ren](https://sites.google.com/site/renwenqi888/), [Changxin Gao](https://sites.google.com/site/changxingao), Nong Sang<Br>
**[[Pytorch-Code](https://github.com/HUSTSYJ/DA_dahazing)]**  <Br>
粗读, 提出了一个生成数据集训练的网络迁移到真实图像去雾中的框架, 使用两个变换网络和GAN完成Syn和Real数据间的相互迁移.
	
#### FFA=Net
**[Paper]**  (AAAI 2020) FFA-Net: Feature Fusion Attention Network for Single Image Dehazing <Br>
**[Author]**  Xu Qin, Zhilin Wang, Yuanchao Bai, Xiaodong Xie, Huizhu Jia <Br>
**[[Pytorch-Code](https://github.com/zhilin007/FFA-Net)]**  <Br>
								     
#### DCPDN ★
**[Paper]**  (CVPR 2018) Densely Connected Pyramid Dehazing Network<Br>
**[Author]** [He Zhang](https://sites.google.com/site/hezhangsprinter), [Vishal M. Patel](https://engineering.jhu.edu/vpatel36/sciencex_teams/vishalpatel/) <Br>
**[[Pytorch-Code](https://github.com/hezhangsprinter/DCPDN)]**<Br>
两分支网络, transmission map通过类似dense-net的网络预测, 大气光照假设是一全局常量并通过一UNet预测, 两分支结果经大气散射模型公式的计算, 恢复清晰RGB. 使用了L2, VGG loss, gradient loss和GAN loss.
	
#### Multi-scale-CNN-Dehazing ☆
**[Paper]**  (CVPR 2018) Single Image Dehazing via Multi-Scale Convolutional Neural Networks <Br>
**[Author]** [Wenqi Ren](https://sites.google.com/site/renwenqi888/), [Si Liu](http://www.colalab.org/people), Hua Zhang, [Jinshan Pan](https://sites.google.com/site/jspanhomepage/), [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Project](https://sites.google.com/site/renwenqi888/research/dehazing/mscnndehazing)]** **[[Matlab-Code](https://github.com/rwenqi/Multi-scale-CNN-Dehazing)]**  **[[Unofficial-TF-Code](https://github.com/dishank-b/MSCNN-Dehazing-Tensorflow)]**<Br>
大致浏览, 一个多尺度去雾网络, coarse尺度预测transmission map, fine尺度预测去雾图像, 用深度图生成transmmision map训练 <Br>

#### GFN
**[Paper]**  (CVPR 2018) Gated Fusion Network for Single Image Dehazing <Br>
**[Author]** [Wenqi Ren](https://sites.google.com/site/renwenqi888/), [Lin Ma](http://forestlinma.com/), [Jiawei Zhang](https://sites.google.com/site/zhjw1988), [Jinshan Pan](https://sites.google.com/site/jspanhomepage/), [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en),  Wei Liu, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Project](https://sites.google.com/site/renwenqi888/research/dehazing/gfn)]** **[[MatCaffe-Code](https://github.com/rwenqi/GFN-dehazing)]**  <Br>

#### AOD-NET ★
**[Paper]**  (ICCV 2017) AOD-NET：An All-in-One Network for Dehazing and Beyond<Br>
**[Author]** [Boyi Li](https://sites.google.com/site/boyilics/home), Xiulian Peng, [Zhangyang Wang](https://www.atlaswang.com/), Jizheng Xu, Dan Feng <Br>
**[[Project](https://sites.google.com/site/boyilics/website-builder/project-page)]**  **[[Pytorch&Caffe-Code](https://github.com/Boyiliee/AOD-Net)]** <Br>
轻量级去雾网络, 通过预测一个变量, 直接输出清晰的RGB图像

#### DehazeNet ☆
**[Paper]**  (TIP 2016) DehazeNet: An End-to-End System for Single Image Haze Removal <Br>
**[Author]** [Bolun Cai](https://caibolun.github.io/), Xiangmin Xu, Kui Jia, Chunmei Qing, Dacheng Tao, Lingke Zeng <Br>
**[[Project](http://caibolun.github.io/DehazeNet/)]** **[[Matlab-Code](https://github.com/caibolun/DehazeNet)]**<Br>
端到端预测透射率map







# Image Debluring	
#### blur-kernel-space-exploring
**[Paper]** (CVPR 2021) Explore Image Deblurring via Encoded Blur Kernel Space <Br>
**[Author]** P.Tran, A.Tran, Q.Phung, [M. Hoai](https://www3.cs.stonybrook.edu/~minhhoai/)    <Br>
**[[Pytorch-Code](https://github.com/VinAIResearch/blur-kernel-space-exploring)]** 

#### RSCD 
**[Paper]** (CVPR 2021) Towards Rolling Shutter Correction and Deblurring in Dynamic Scenes <Br>
**[Author]** Zhihang Zhong, Yinqiang Zheng, [Imari Sato](http://research.nii.ac.jp/~imarik/)   <Br>
**[[Pytorch-Code](https://github.com/zzh-tech/RSCD)]** 

#### DeFMO
**[Paper]** (CVPR 2021) DeFMO: Deblurring and Shape Recovery of Fast Moving Objects <Br>
**[Author]** [Denys Rozumnyi](http://people.inf.ethz.ch/denysr/), [Martin R. Oswald](http://people.inf.ethz.ch/moswald/), [Vittorio Ferrari](https://sites.google.com/view/vittoferrari), [Jiri Matas](https://cmp.felk.cvut.cz/~matas/), [Marc Pollefeys](https://people.inf.ethz.ch/pomarc/)   <Br>
**[[Pytorch-Code](https://github.com/rozumden/DeFMO)]** 

#### Non-blind Deblurring
**[Paper]** (CVPR 2021) Learning a Non-blind Deblurring Network for Night Blurry Images <Br>
**[Author]** Liang Chen, [Jiawei Zhang](https://sites.google.com/site/zhjw1988), [Jinshan Pan](https://jspan.github.io/), Songnan Lin, Faming Fang, [Jimmy Ren](http://www.jimmyren.com/)    <Br>
	
#### Deblurring by Realistic Blurring
**[Paper]** (CVPR 2020) Deblurring by Realistic Blurring <Br>
**[Author]** [Kaihao Zhang](https://sites.google.com/view/kaihaozhang), [Wenhan Luo](https://sites.google.com/site/whluoimperial/), Yiran Zhong, [Lin Ma](http://forestlinma.com/), Bjorn Stenger, Wei Liu, [Hongdong Li](http://users.cecs.anu.edu.au/~hongdong/)<Br>

#### Event-Based Motion Deblurring
**[Paper]** (CVPR 2020) Learning Event-Based Motion Deblurring <Br>
**[Author]** Zhe Jiang, [Yu Zhang](https://zhangyulb.github.io/), Dongqing Zou, [Jimmy Ren](http://www.jimmyren.com/), Jiancheng Lv, Yebin Liu<Br>

#### Deblurring Using Spatially Variant Deconvolution
**[Paper]** (CVPR 2020) Efficient Dynamic Scene Deblurring Using Spatially Variant Deconvolution Network With Optical Flow Guided Training <Br>
**[Author]** Yuan Yuan, Wei Su, Dandan Ma<Br>

#### Adaptive Motion Deblurring
**[Paper]** (CVPR 2020) Spatially-Attentive Patch-Hierarchical Network for Adaptive Motion Deblurring <Br>
**[Author]** Maitreya Suin, Kuldeep Purohit, A. N. Rajagopalan<Br>
	
#### Variational-EM-Based Deblurring
**[Paper]** (CVPR 2020) Variational-EM-Based Deep Learning for Noise-Blind Image Deblurring <Br>
**[Author]** Yuesong Nan, Yuhui Quan, Hui Ji<Br>
	
#### Deblurring Using Analysis-Synthesis Networks Pair
**[Paper]** (CVPR 2020) Deblurring Using Analysis-Synthesis Networks Pair<Br>
**[Author]** Adam Kaufman, Raanan Fattal<Br>

#### Handling Kernel/model Uncertainty in Image Deconvolution
**[Paper]** (CVPR 2020) Deep Learning for Handling Kernel/model Uncertainty in Image Deconvolution<Br>
**[Author]** Yuesong Nan, Hui Ji<Br>
	
#### *Bad Weather Removal using Architectural Search*
**[Paper]** (CVPR 2020) All in One Bad Weather Removal using Architectural Search<Br>
**[Author]** Ruoteng Li, Robby T. Tan, Loong-Fah Cheong<Br>

#### DeblurGAN-v2 ★☆
**[Paper]** (ICCV 2019) DeblurGAN-v2: Deblurring (Orders-of-Magnitude) Faster and Better <Br>
**[Author]** Orest Kupyn, Tetiana Martyniuk, Junru Wu, Zhangyang Wang<Br>
**[[Pytorch-Code](https://github.com/TAMU-VITA/DeblurGANv2)]**  <Br>
DeblurGAN基础上的改进, 把生成网络换成了FPN, 设计了新的loss, 效果更快更好了

#### DeepGyro ★
**[Paper]** (WACV 2019) Gyroscope-Aided Motion Deblurring with Deep Network <Br>
**[Author]** Janne Mustaniemi, Juho Kannala, Simo Särkkä, Jiri Matas, Janne Heikkilä<Br>
结合陀螺仪作为先验deblur. 从陀螺仪和图像拍摄信息生成训练集的方法可以参考. <Br>
	
#### Dr-Net ★☆
**[Paper]** (CVPR 2019) Douglas-Rachford Networks: Learning Both the Image Prior and Data Fidelity Terms for Blind Image Deconvolution <Br>
**[Author]** Raied Aljadaany, [Dipan K. Pal](https://dkpal.github.io/), [Marios Savvides](https://www.cmu-biometrics.org/)<Br>
1) 基于Douglas-Rachford迭代优化求解blind deconvolution的思路(不懂), 提出了一个由简单conv和连接操作组成的Dr Block, 将其嵌入普通卷积网络中, 用L2和GAN loss训练, 取得了不错的效果. <Br>
2) 网络细节没看, 可以借鉴其模块设计
	
#### DMPHN ☆
**[Paper]** (CVPR 2019) Deep Stacked Multi-patch Hierarchical Network for Image Deblurring <Br>
**[Author]** [Hongguang Zhang](https://hongguangzhang.github.io/), [Yuchao Dai](http://users.cecs.anu.edu.au/~yuchao/), [Hongdong Li](http://users.cecs.anu.edu.au/~hongdong/), [Piotr Koniusz](http://users.cecs.anu.edu.au/~koniusz/)<Br>
**[[Pytorch-Code](https://github.com/HongguangZhang/DMPHN-cvpr19-master)]** <Br>
从spatial pyramid matching的角度出发, 提出了一个分patch的逐层融合处理的网络, 参数少速度快. 但个人仍不理解这种分patch的做法对CNN来说到底有什么意义. 

#### HA-Deblur ★☆
**[Paper]** (ICCV 2019) Human-Aware Motion Deblurring <Br>
**[Author]** [Ziyi Shen](https://sites.google.com/site/ziyishenmi/), [Wenguan Wang](https://sites.google.com/view/wenguanwang/), [Xiankai Lu](https://sites.google.com/site/xiankailu111/), Jianbin Shen, [Haibin Ling](https://www3.cs.stonybrook.edu/~hling/), Tingfa Xu, [Ling Shao](http://www.inceptioniai.org/)<Br>
**[[Project](https://sites.google.com/site/ziyishenmi/ha_deblur)]**  **[[HIDE Dataset](https://github.com/joanshen0508/HA_deblur)]** <Br>
1. 提出了HIDE数据集, 主要关注对人体的deblur <Br>
2. 提出了一个多分支deblur网络, 根据human-aware子网络预测前背景生成weight map, 将多分枝信息融合处理后输出 <Br>	
	
#### ED-DSRN ☆
**[Paper]** (ICASSP 2018) A Deep Encoder-Decoder Network For Joint Deblurring and Super-Resolution <Br>
**[Author]** Xinyi Zhang, Fei Wang, Hang Dong, Yu Guo  <Br>
**[[Project](http://xinyizhang.tech/icassp2018/)]**  <Br>
大致浏览, 一个端到端的同时deblur和超分网络 <Br>
	
#### GFN ★☆
**[Paper]** (BMVC 2018) Gated Fusion Network for Joint Image Deblurring and Super-Resolution <Br>
**[Author]** Xinyi Zhang, Hang Dong, [Zhe Hu](https://zjuela.github.io/), [Wei-Sheng Lai](http://graduatestudents.ucmerced.edu/wlai24/), Fei Wang, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/_)<Br>
**[[Project](http://xinyizhang.tech/bmvc2018/)]** **[[Pytorch-Code](https://github.com/jacquelinelala/GFN)]** <Br>
1) 提出了一个同时做deblur和超分的网络. 网络有两个分支, 一个encoder-decoder结构做deblur, 一个不降分辨率做SR, 用一个几层卷积组成的gate模块选择特征. <Br>
2) 思路简单, 可以尝试.<Br>
	
#### DeblurGAN ★★
**[Paper]** (CVPR 2018) DeblurGAN: Blind Motion Deblurring Using Conditional Adversarial Networks <Br>
**[Author]** Orest Kupyn, Volodymyr Budzan, Mykola Mykhailych, Dmytro Mishkin, Jiří Matas<Br>
**[[Pytorch-Code](https://github.com/KupynOrest/DeblurGAN)]** **[[Unofficial-TF-Code1](https://github.com/LeeDoYup/DeblurGAN-tf)]** **[[Unofficial-TF-Code2](https://github.com/dongheehand/DeblurGAN-tf)]**<Br>
1) 用GAN做deblur的一篇典型文章, 效果不错.<Br>
2) 生成网络结构简单, 采用残差形式. <Br>
3) 提出了生成blur数据的方法, 可以参考一下. <Br>
	
#### Deep Multi-scale Deblur ★☆
**[Paper]** (CVPR 2017 Spotlight) Deep Multi-scale Convolutional Neural Network for Dynamic Scene Deblurring <Br>
**[Author]** [Seungjun Nah](https://seungjunnah.github.io/), [Tae Hyun Kim](https://sites.google.com/site/lliger9/), [Kyoung Mu Lee](https://cv.snu.ac.kr/index.php/~kmlee/)  <Br>
**[[Code](https://github.com/SeungjunNah/DeepDeblur_release)]**  <Br>
1) 提出了GOPRO单张图像deblur数据集 <Br>
2) 提出了一个多尺度输入的去噪网络	








# Reflection Removal
#### Panoramic image reflection removal
**[Paper]** (CVPR 2021) Panoramic image reflection removal  <Br>
**[Author]** [Yuchen Hong](http://vcc.szu.edu.cn/index-2.html), [Qian Zheng](https://q-zh.github.io/), Lingran Zhao, [Xudong Jiang](https://personal.ntu.edu.sg/exdjiang/), Alex C. Kot, [Boxin Shi](http://ci.idm.pku.edu.cn/)  <Br>

#### reflection removal with absorption effect
**[Paper]** (CVPR 2021) Single image reflection removal with absorption effect  <Br>
**[Author]** [Qian Zheng](https://q-zh.github.io/), [Boxin Shi](http://ci.idm.pku.edu.cn/), Jinnan Chen, [Xudong Jiang](https://personal.ntu.edu.sg/exdjiang/), Ling-Yu Duan, Alex C. Kot  <Br>
**[[Pytorch-Code](https://github.com/q-zh/absorption)]** <Br>

#### Reflection Removal with Reflection-free Flash-only Cues
**[Paper]** (CVPR 2021) Robust Reflection Removal with Reflection-free Flash-only Cues  <Br>
**[Author]** [Chenyang Lei](https://chenyanglei.github.io/), [Qifeng Chen](https://cqf.io/)  <Br>
**[[Project](https://chenyanglei.github.io/flashrr_rfc/index.html)]** **[[TF-Code](https://github.com/ChenyangLEI/flash-reflection-removal)]**<Br>

#### Reflection scene separation from a single image
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

#### Polarized Reflection Removal
**[Paper]** (CVPR 2020) Polarized Reflection Removal with Perfect Alignment in the Wild  <Br>
**[Author]** [Chenyang Lei](https://chenyanglei.github.io/), Xuhua Huang, Mengdi Zhang, Qiong Yan, Wenxiu Sun, [Qifeng Chen](https://cqf.io/)  <Br>
**[[Project](https://chenyanglei.github.io/polar_rr/index.html)]**, **[[TF-Code](https://github.com/ChenyangLEI/polarization-reflection-removal)]**<Br>

#### Reflection removal rendering
**[Paper]** (CVPR 2020 Oral) Single Image Reflection Removal with Physically-Based Training Images <Br>
**[Author]** [Soomin Kim](https://sgvr.kaist.ac.kr/~smkim/), [Yuchi Huo](https://sgvr.kaist.ac.kr/~ychuo/), [Sung-Eui Yoon](https://sgvr.kaist.ac.kr/~sungeui/)  <Br>
**[[Project](https://sgvr.kaist.ac.kr/~smkim/Reflection_removal_rendering/)]**, **[[TF-Code](https://github.com/sookim813/Reflection_removal_rendering)]**<Br>

#### Single Image Reflection Removal Beyond Linearity
**[Paper]** (CVPR 2019) Single Image Reflection Removal Beyond Linearity <Br>
**[Author]** Qiang Wen, Yinjie Tan, Jing Qin, Wenxi Liu, Guoqiang Han, and Shengfeng He <Br>
**[[Pytorch-Code](https://github.com/csqiangwen/Single-Image-Reflection-Removal-Beyond-Linearity)]**<Br>

#### Learning to jointly generate and separate reflections
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
#### ICT
**[Paper]** (ICCV 2021) High-Fidelity Pluralistic Image Completion with Transformers <Br>
**[Author]** [Ziyu Wan](http://raywzy.com/), Jingbo Zhang, [Dongdong Chen](http://www.dongdongchen.bid/), [Jing Liao](https://liaojing.github.io/html/index.html) <Br>
**[[Project](https://zengxianyu.github.io/iic/)]**  **[[Pytorch-Code](https://github.com/raywzy/ICT)]**  <Br>
	
#### EII
**[Paper]** (CVPR 2021) Generating Diverse Structure for Image Inpainting with Hierarchical VQ-VAE <Br>
**[Author]** Tengfei Wang, Hao Ouyang, [Qifeng Chen](https://cqf.io/) <Br>
**[[Project](https://tengfei-wang.github.io/EII/index.html/)]** **[[Pytorch-Code](https://github.com/Tengfei-Wang/external-internal-inpainting)]**  <Br>

#### Diverse-Structure-Inpainting
**[Paper]** (CVPR 2021) Generating Diverse Structure for Image Inpainting with Hierarchical VQ-VAE <Br>
**[Author]** Jialun Peng, [Dong Liu](http://staff.ustc.edu.cn/~dongeliu/), [Songcen Xu](http://www.xusongcen.com/), [Houqiang Li](http://staff.ustc.edu.cn/~lihq/) <Br>
**[[Pytorch-Code](https://github.com/USTC-JialunPeng/Diverse-Structure-Inpainting)]**  <Br>
	
#### TransFill
**[Paper]** (CVPR 2021) TransFill: Reference-guided Image Inpainting by Merging Multiple Color and Spatial Transformations <Br>
**[Author]** [Yuqian Zhou](https://yzhouas.github.io/), [Connelly Barnes](http://www.connellybarnes.com/work/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/), Sohrab Amirghodsi <Br>
**[[Project](https://yzhouas.github.io/projects/TransFill/index.html)]** **[[Pytorch-Code](https://github.com/yzhouas/TransFill-Reference-Inpainting)]**  <Br>
		
#### PD-GAN
**[Paper]** (CVPR 2021) PD-GAN:Probabilistic Diverse GAN for Image Inpainting <Br>
**[Author]** Hongyu Liu, [Ziyu Wan](http://raywzy.com/), Wei Huang, [Yibing Song](https://ybsong00.github.io/), Xintong Han, [Jing Liao](https://liaojing.github.io/html/index.html) <Br>
**[[Pytorch-Code](https://github.com/KumapowerLIU/PD-GAN)]**  <Br>
	
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
	
#### Guidance and Evaluation
**[Paper]** (ECCV 2020) Guidance and Evaluation: Semantic-Aware Image Inpainting for Mixed Scenes <Br>
**[Author]** Liang Liao, Jing Xiao, [Zheng Wang](https://wangzwhu.github.io/home/), [Chia-Wen Lin](https://www.ee.nthu.edu.tw/cwlin/), [Shin'ichi Satoh](http://research.nii.ac.jp/~satoh/) <Br>

#### Prior Guided GAN Based Semantic Inpainting ★☆
**[Paper]** (CVPR 2020) Prior Guided GAN Based Semantic Inpainting <Br>
**[Author]** Avisek Lahiri, Arnav Kumar Jain, Sanskar Agrawal, Pabitra Mitra, Prabir Kumar Biswas <Br>
大致浏览. 分为两个阶段, 第一阶段训练从noise prior生成图像的generator, 第二阶段固定generator, 训练从待修复图像生成噪声先验的网络. 使用了人脸关键点作为额外的prior控制生成结果.






# De-raining
#### JRGR
**[Paper]** (CVPR 2021) Closing the Loop: Joint Rain Generation and Removal via Disentangled Image Translation <Br>
**[Author]** [Yuntong Ye](https://owuchangyuo.github.io/), Yi Chang, Hanyu Zhou, Luxin Yan <Br>
**[[Pytorch-Code](https://github.com/guyii54/JRGR)]**<Br>
	
#### CCN 
**[Paper]** (CVPR 2021) Removing Raindrops and Rain Streaks in One Go <Br>
**[Author]** Ruijie Quan, [Xin Yu](https://sites.google.com/view/xinyus-homepage/Home), Yuanzhi Liang, [Yi Yang](http://reler.net/) <Br>

#### VRGNet
**[Paper]** (CVPR 2021) From Rain Generation to Rain Removal <Br>
**[Author]** [Hong Wang](https://hongwang01.github.io/), [Zongsheng Yue](https://github.com/zsyOAOA), Qi Xie, Qian Zhao, [Yefeng Zheng](https://sites.google.com/site/yefengzheng), [Deyu Meng](http://gr.xjtu.edu.cn/web/dymeng)  <Br>
**[[Pytorch-Code](https://github.com/hongwang01/VRGNet)]**<Br>
	
#### Syn2Real ★★
**[Paper]** (CVPR 2020) Syn2Real Transfer Learning for Image Deraining using Gaussian Processes<Br>
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

#### Wavelet-Based Dual-Branch Networkfor Image Demoireing
**[Paper]** (ECCV 2020) Wavelet-Based Dual-Branch Networkfor Image Demoireing  <Br>
**[Author]**[Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), Jianzhuang Liu, [Shanxin Yuan](https://shanxinyuan.github.io/), [Gregory Slabaugh](http://www.gregslabaugh.net/), [Ales Leonardis](https://www.cs.bham.ac.uk/~leonarda/), Wengang Zhou, Qi Tian <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>
	
#### FHDe²Net
**[Paper]** (ECCV 2020) FHDe²Net: Full High Definition Demoireing Network <Br>
**[Author]** Bin He, Ce Wang, [Boxin Shi](http://ci.idm.pku.edu.cn/), Ling-Yu Duan <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>
	
#### Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs
**[Paper]** (NeurIPS 2020) Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs  <Br>
**[Author]** [Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), [Shanxin Yuan](https://shanxinyuan.github.io/), Jianzhuang Liu, Liping Bao, Gregory Slabaugh, Qi Tian <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>
