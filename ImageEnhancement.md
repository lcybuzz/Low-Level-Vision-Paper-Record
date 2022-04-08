# Table of Contents
- [Image Enhancement](#image-enhancement)
- [Low-light Image Enhancement](#low-light-image-enhancement)



# Image Enhancement
#### SSH
**[Paper]** (ICCV 2021) SSH: A Self-Supervised Framework for Image Harmonization <Br>
**[Author]** [Yifan Jiang](http://yifanjiang.net/), [He Zhang](https://sites.google.com/site/hezhangsprinter), [Jianming Zhang](https://jimmie33.github.io/), [Yilin Wang](http://yilinwang.org/), [Zhe Lin](https://sites.google.com/site/zhelin625/), [Kalyan Sunkavalli](http://www.kalyans.org/), Simon Chen, Sohrab Amirghodsi, Sarah Kong, Zhangyang Wang <Br>
**[[PyTorch-Code](https://github.com/VITA-Group/SSHarmonization)]**   <Br>

#### STAR
**[Paper]** (ICCV 2021) STAR: A Structure-Aware Lightweight Transformer for Real-time Image Enhancement <Br>
**[Author]**[ Zhaoyang Zhang](https://zzyfd.github.io/#/), Yitong Jiang, Jun Jiang, [Xiaogang Wang](http://www.ee.cuhk.edu.hk/~xgwang/), [Ping Luo](http://luoping.me/), [Jinwei Gu](https://www.gujinwei.org/) <Br>
	
#### G2R-ShadowNet
**[Paper]** (CVPR 2021) From Shadow Generation to Shadow Removal <Br>
**[Author]** Zhihao Liu, Hui Yin, Xinyi Wu, [Zhenyao Wu](http://zhenyaowu.com/), Yang Mi, [Song Wang](https://www.cse.sc.edu/~songwang/)<Br>
**[[PyTorch-Code](https://github.com/hhqweasd/G2R-ShadowNet)]**   <Br>

#### exposure fusion shadow removal
**[Paper]** (CVPR 2021) Auto-exposure fusion for single-image shadow removal <Br>
**[Author]** Lan Fu, Changqing Zhou, [Qing Guo](https://tsingqguo.github.io/), [Felix Juefei-Xu](http://xujuefei.com/), [Hongkai Yu](http://cis.csuohio.edu/~h.yu/), Wei Feng, [Yang Liu](https://personal.ntu.edu.sg/yangliu/), [Song Wang](https://www.cse.sc.edu/~songwang/) <Br>
**[[PyTorch-Code](https://github.com/tsingqguo/exposure-fusion-shadow-removal)]**   <Br>

#### Multi-Scale Photo Exposure Correction
**[Paper]** (CVPR 2021) Learning Multi-Scale Photo Exposure Correction<Br>
**[Author]** [Mahmoud Afifi](https://sites.google.com/view/mafifi), [Konstantinos G. Derpanis](https://www.cs.ryerson.ca/kosta/), [Björn Ommer](https://hci.iwr.uni-heidelberg.de/people/bommer), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
**[[PyTorch-Code](https://github.com/mahmoudnafifi/Exposure_Correction)]**   <Br>
coarse-to-fine增强的策略, 并在每个level加入相应的拉普拉斯金字塔层作为细节信息. 使用L1和GAN loss. 效果不错. <Br>
	
#### DeepLPF ★☆
**[Paper]** (CVPR 2020) DeepLPF: Deep Local Parametric Filters for Image Enhancement <Br>
**[Author]** [Sean Moran](http://www.seanjmoran.com/), Pierre Marza, Steven McDonagh, Sarah Parisot, [Gregory Slabaugh](http://gregslabaugh.net/)  <Br>
**[[PyTorch-Code](https://github.com/huawei-noah/noah-research/tree/071a49fb8f0975192dcc919a18f9a082093122e6/DeepLPF)]**   <Br>
1) 华为欧洲实验室的文章, 把lightroom等修图软件中的brugh, graduated filters, radial filters工具用CNN模拟出来. 分为三个分支, 一个分支预测pixelwise的增强, 两个分支分别预测两种fiter的参数. 
2) 个人觉得预测的filter仍然不太够local. 不过论文的思路挺有意思.
	
#### Image-Adaptive-3DLUT ★★
**[Paper]** (TPAMI 2020) Learning Image-adaptive 3D Lookup Tables for High Performance Photo Enhancement in Real-time <Br>
**[Author]** Hui Zeng, [Jianrui Cai](https://csjcai.github.io/), Lida Li, Zisheng Cao, [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
**[[Code](https://github.com/HuiZeng/Image-Adaptive-3DLUT)]**   <Br>
预测若干个3D LUT, 并用一个轻量级CNN预测每个LUT的权重. LUT和CNN同时训练, 采用了平滑和单调两种正则方式消除伪影等问题. 非常适合处理大图, 实际应用价值大, 值得一试.

#### GLeNet ★★
**[Paper]** (ECCV 2020) Global and Local Enhancement Networks for Paired and Unpaired Image Enhancement <Br>
**[Author]** Han-Ul Kim, Young Jun Koh, Chang-Su Kim <Br>
**[[Project](http://mcl.korea.ac.kr/research/hukim-eccv2020-glenet/)]**   **[[Pytorch-Code](https://github.com/dongkwonjin/GleNet)]** <Br>
**(曲线预测)**	全局预测曲线(3*256) + 局部增强. 无监督训练部分采用类似cycle gan的策略. 更具有实用性的曲线预测策略已经开始获得关注, 相关论文越来越多了.

#### PieNet ★★
**[Paper]** (ECCV 2020) PieNet: Personalized Image Enhancement Network <Br>
**[Author]** Han-Ul Kim, Young Jun Koh, Chang-Su Kim <Br>
**[[Project](http://mcl.korea.ac.kr/research/hukim-eccv2020-pienet/)]**   **[[TF-Code](https://github.com/hukim1124/PieNet)]** <Br>
**(个性化增强)**	使用度量学习的方法, 学习一个网络, 从用户选择的若干图像中提取偏好特征向量, 该特征向量作用在增强网络上, 产生符合用户喜好的增强结果.

#### CSRNet ★
**[Paper]** (ECCV 2020) Conditional Sequential Modulation for Efficient Global Image Retouching <Br>
**[Author]** Jingwen He, Yihao Liu, [Yu Qiao](http://mmlab.siat.ac.cn/yuqiao/), Chao Dong <Br>
**[[Pytorch-Code](https://github.com/hejingwenhejingwen/CSRNet)]**<Br>
**(控制restoration level)**	  本文聚焦于全局retouching, 认为很多操作都可以用MLP模拟, 据此设计了一个由若干1x1卷积组成的base网络, 另外又设计了一个condition网络提取全局信息对base网络各层进行调制.

#### RBQE ☆
**[Paper]** (ECCV 2020) Early Exit or Not: Resource-Efficient Blind Quality Enhancement for Compressed Images <Br>
**[Author]** [Qunliang Xing](https://ryanxingql.github.io/), Mai Xu, Tianyi Li, Zhenyu Guan <Br>
**[[Pytorch-Code](https://github.com/RyanXingQL/RBQE)]**<Br>
提出一个simple to hard的图像增强算法, 通过一个质量评估模块判断当前增强结果是否符合要求, 若符合要求, 就提前推出. 本文主要关注压缩图像, 不知是否可扩展到超分等任务中
	
#### URIE ★
**[Paper]** (ECCV 2020) URIE: Universal Image Enhancement for Visual Recognition in the Wild <Br>
**[Author]** Taeyoung Son, Juwon Kang, Namyup Kim, [Sunghyun Cho](https://www.scho.pe.kr/), [Suha Kwak](http://cvlab.postech.ac.kr/~suhakwak/) <Br>
**[[Project](http://cvlab.postech.ac.kr/research/URIE/)]** **[[Pytorch-Code](https://github.com/taeyoungson/urie)]**<Br>
提出了一个通用的质量增强模块, 可插入到检测分割等识别任务之前, 提升这些任务的性能.

#### CURL ★
**[Paper]** (ICLR 2020) CURL: Neural Curve Layers for Global Image Enhancement <Br>
**[Author]** [Sean Moran](http://www.seanjmoran.com/), [Steven McDonagh](https://biomedia.doc.ic.ac.uk/person/steven-mcdonagh/), [Gregory Slabaugh](http://www.gregslabaugh.net/)  <Br>
**[[Pytorch-Code](https://github.com/sjmoran/neural_curve_layers)]**  <Br>
在LAB, RGB, HSV三个空间预测curve

#### FUnIE-GAN ★
**[Paper]** (RAL 2020) Fast Underwater Image Enhancement for Improved Visual Perception <Br>
**[Author]** [Md Jahidul Islam](https://xahidbuffon.github.io/), [Youya Xia](https://www.xiayouya.com/), [Junaed Sattar](https://junaedsattar.cs.umn.edu/)  <Br>
**[[Code](https://github.com/xahidbuffon/FUnIE-GAN)]**   <Br>
encoder-decoder结构, 使用了几个目标函数从各方面增强图像视觉质量. 提出了一个水下图像数据集.

#### Content-preserving Tone Adjustment ★☆
**[Paper]** (CVPRW 2019) Content-preserving Tone Adjustment for Image Enhancement <Br>
**[Author]** [Simone Bianco](http://www.ivl.disco.unimib.it/people/simone-bianco/), [Claudio Cusano](http://www.ivl.disco.unimib.it/people/claudio-cusano/), [Flavio Piccoli](http://www.ivl.disco.unimib.it/people/flavio-piccoli/), [Raimondo Schettini](http://www.ivl.disco.unimib.it/people/raimondo-schettini/)  <Br>
**[[PyTorch-Code](https://github.com/dros1986/content-preserving-tone-adjustment-for-image-enhancement)]**   <Br>
有点类似HRDNet, 在小分辨率预测输入值的分段映射系数, 在原图上增强. 速度快, 应该有较强的实用性.

#### EnhanceGAN ★ 
**[Paper]** (MM 2018) Aesthetic-Driven Image Enhancement by Adversarial Learning <Br>
**[Author]** Yubin Deng, [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/index.html),	[Xiaoou Tang](https://www.ie.cuhk.edu.hk/people/xotang.shtml)  <Br>
**[[Project](http://personal.ie.cuhk.edu.hk/~dy015/ImageAesthetics/EnhanceGAN.html)]** **[[Torch-Code](https://github.com/dannysdeng/EnhanceGAN)]**<Br>
1) weakly supervised方法, 学习crop和色彩变换参数, 增强aesthetic quality

#### PPCN ☆
**[Paper]** (ECCVW 2018) Perception-Preserving Convolutional Networks for Image Enhancement on Smartphones <Br>
**[Author]** Zheng Hui, Xiumei Wang, Lirui Deng, [Xinbo Gao](http://see.xidian.edu.cn/faculty/xbgao/) <Br>
**[[TF-Code](https://github.com/Zheng222/PPCN)]**   <Br>
ECCV PIRM(Perceptual Image Restoration and Manipulation ) 2018竞赛, 一个快速图像增强方案

#### FEQE ☆
**[Paper]** (ECCVW 2018)  Fast and Efficient Image Quality Enhancement via Desubpixel Convolutional Neural Networks <Br>
**[Author]** [Thang Vu](https://thangvubk.github.io/), Cao V. Nguyen, Trung X. Pham, Tung M. Luu, and Chang D. Yoo  <Br>
**[[TF-Code](https://github.com/thangvubk/FEQE)]**   <Br>
使用pixel shuffle的实时图像增强网络

#### WESPE ★
**[Paper]** (CVPRW 2018) WESPE: Weakly Supervised Photo Enhancer for Digital Cameras <Br>
**[Author]** Andrey Ignatov, Nikolay Kobyshev, Radu Timofte , Kenneth Vanhoey, Luc Van Gool  <Br>
**[[Project](http://people.ee.ethz.ch/~ihnatova/index.html)]**   <Br>	

#### RSGUNet ★
**[Paper]** (ECCVW 2018) Range Scaling Global U-Net for Perceptual Image Enhancement on Mobile Devices <Br>
**[Author]** Jie Huang, Pengfei Zhu, Mingrui Geng, Jiewen Ran, Xingguang Zhou, Chen Xing, Pengfei Wan, Xiangyang Ji  <Br>
**[[TF-Code](https://github.com/MTlab/rsgunet_image_enhance)]**   <Br>
UNet + Global Pooling feature + 输入输出feature间的elementwise scaling
	
#### DPED ★★
**[Paper]** (ICCV 2017) DSLR-Quality Photos on Mobile Devices with Deep Convolutional Networks <Br>
**[Author]** Andrey Ignatov, Nikolay Kobyshev, Kenneth Vanhoey, Radu Timofte , Luc Van Gool  <Br>
**[[Code](http://people.ee.ethz.ch/~ihnatova/index.html)]**   <Br>
1) 从变换的角度出发, 学习一个从低质量图像到高质量图片的变换函数 
2) 变换部分采用残差快结构的CNN，定义了4个loss (color, texture, content, variance). color loss是图像进行高斯模糊后的均方差, texture loss是adversarial loss, content loss是perceptual loss, variance loss是图像梯度的模.
3) 提出了用于图像质量增强的数据集DPED, 包括iPhone, BlackBerry和Sony三种手机与Canon单反相机的图相对.

#### HDRNet ★★★
**[Paper]** (Siggraph 2017) Deep Bilateral Learning for Real-Time Image Enhancement <Br>
**[Author]** 	Michaël Gharbi, [Jiawen Chen](http://people.csail.mit.edu/jiawen/), [Jonathan T. Barron](https://jonbarron.info/),  [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Frédo Durand](http://people.csail.mit.edu/fredo/)  <Br>
**[[Project](https://groups.csail.mit.edu/graphics/hdrnet/)]**<Br>
1) 提出了一个实时图像增强网络, 速度快, 效果好. <Br>
2) 网络分为两个分支, 低分辨率分支提取特征, 学习每个像素的色彩映射参数; 高分辨率分支负责提取和保留细节信息. low res分支学到的映射参数通过类似于双线性差值的过程上采样到high res, 最后对high res图像做色彩映射并输出. <Br>
3) 学习映射参数部分, 采用bilateral grid的思路. 第三个维度被解释成8*12的网格, 意思是对8个灰度level做不同的色彩映射. 处理时选择哪个level的参数, 由high res分支生成的引导图决定. <Br> 

	
	
	
	
# Low-light Image Enhancement
#### LLFLOW
**[Paper]** (AAAI 2022 Oral) Low-Light Image Enhancement with Normalizing Flow <Br>
**[Author]**  [Yufei Wang](https://wyf0912.github.io/), [Renjie Wan](https://wanrenjie.github.io/), [Wenhan Yang](https://flyywh.github.io/), [Haoliang Li](https://hlli1991.github.io/), [Lap-pui Chau](https://personal.ntu.edu.sg/elpchau/), [Alex C. Kot](https://personal.ntu.edu.sg/eackot/index.html)     <Br>
**[[Project](https://wyf0912.github.io/LLFlow/)]** **[[Pytorch-Code](https://github.com/wyf0912/LLFlow)]** <Br>

#### Restoring Extremely Dark Images
**[Paper]** (CVPR 2021) Restoring Extremely Dark Images in Real Time  <Br>
**[Author]**  [Mohit Lamba](https://mohitlamba94.github.io/about-me/), [Kaushik Mitra](https://www.ee.iitm.ac.in/kmitra/) <Br>
**[[Code](https://github.com/MohitLamba94/Restoring-Extremely-Dark-Images-In-Real-Time)]** <Br>

####  Low-light Survey
**[Paper]** (TPAMI 2021) Low-light Image and Video Enhancement Using Deep Learning: A Survey <Br>
**[Author]** [Chongyi Li](https://li-chongyi.github.io/), Chunle Guo, Linghao Han, Jun Jiang, [Ming-Ming Cheng](https://mmcheng.net/cmm/), [Jinwei Gu](http://www.gujinwei.org/), [Chen Change Loy](https://www.mmlab-ntu.com/person/ccloy/)  <Br>
**[[Project](https://github.com/Li-Chongyi/Lighting-the-Darkness-in-the-Deep-Learning-Era-Open)]**<Br>

#### Zero-DCE ★★
**[Paper]** (CVPR 2020) Zero-Reference Deep Curve Estimation for Low-Light Image Enhancement <Br>
**[Author]** Chunle Guo, [Chongyi Li](https://li-chongyi.github.io/), Jichang Guo, [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/index.html), [Junhui Hou](https://sites.google.com/site/junhuihoushomepage/), [Sam Kwong](https://www.cs.cityu.edu.hk/~cssamk/research_group/index.html), [Runmin Cong](https://rmcong.github.io/)   <Br>
**[[Project](https://li-chongyi.github.io/Proj_Zero-DCE.html)]** **[[Pytorch-Code](https://github.com/Li-Chongyi/Zero-DCE)]** **[[TF-Code](https://github.com/tuvovan/Zero_DCE_TF)]**<Br>
1) 一篇挺有趣的论文, 把tone mapping看成pixel-wise的曲线预测问题, 设计了一个小型曲线估计网络, 并提出了几个无监督loss, 得到了不错的结果 <Br>
2) 一些局限性: 提出的一系列约束loss对于增强部分区域可能不太适用, 比如对夜景图片增强前景的同时保持夜空是暗的

#### Decomposition and Enhancement ★
**[Paper]** (CVPR 2020) Learning to Restore Low-Light Images via Decomposition-and-Enhancement <Br>
**[Author]** Ke Xu, [Xin Yang](http://faculty.dlut.edu.cn/yangxin/zh_CN/index.htm), Baocai Yin, [Rynson W.H. Lau](https://www.cs.cityu.edu.hk/~rynson/)   <Br>
在亮度增强的同时考虑去噪. 认为低频部分受噪声影响小(???)所以容易在低频部分进行增强. 低频部分增强后通过一个网络学习恢复高频部分. 设计了两个模块用于提取低频信息和扩大感受野.

#### DRBN ☆
**[Paper]** (CVPR 2020) From Fidelity to Perceptual Quality: A Semi-Supervised Approach for Low-Light Image Enhancement <Br>
**[Author]** [Wenhan Yang](https://flyywh.github.io/), Shiqi Wang, [Yuming Fang](https://sites.google.com/site/leofangyuming/), Yue Wang, Jiaying Liu   <Br>
**[[Pytorch-Code](https://github.com/flyywh/CVPR-2020-Semi-Low-Light)]** <Br>
分为有监督部分和无监督(GAN)两部分. 结构比较繁琐. 

#### EEMEFN ★
**[Paper]** (AAAI 2020) EEMEFN: Low-Light Image Enhancement via Edge-Enhanced Multi-Exposure Fusion Network <Br>
**[Author]** Minfeng Zhu, Pingbo Pan, [Wei Chen](http://www.cad.zju.edu.cn/home/chenwei/), Yi Yang   <Br>
大致浏览. 输入为raw, 设计了一个多分支网络, 分别处理不同曝光值得输入并将结果融合, 里面的参考曝光值不知道是怎么得到的. 另外还加入一个边缘增强网络, 方法是现成的. 

#### Self-supervised Image Enhancement Network
**[Paper]** (arXiv 2002) Self-supervised Image Enhancement Network: Training With Low Light Images Only <Br>
**[Author]** Yu Zhang, Xiaoguang Di, Bin Zhang, Chunhui Wang  <Br>
**[[TF-Code](https://github.com/hitzhangyu/Self-supervised-Image-Enhancement-Network-Training-With-Low-Light-Images-Only)]** <Br>	

#### Unsupervised Low-light Image Enhancement with Decoupled Networks ★
**[Paper]** (arXiv 2005) Unsupervised Real-world Low-light Image Enhancement with Decoupled Networks <Br>
**[Author]** [Wei Xiong](https://wxiong.me/publications/), Ding Liu, Xiaohui Shen, [Chen Fang](http://fangchen.org/), [Jiebo Luo](https://www.cs.rochester.edu/u/jluo/)  <Br>
无监督做亮度增强和去噪. 分为亮度增强和去噪两阶段, 亮度采用Retinex思想, 使用global和local的GAN做loss. 去噪部分提出构建Pseudo Triples的方法, 结合GAN去噪.
	
#### Deep Bilateral Retinex for Low-Light Image Enhancement
**[Paper]** (arXiv 2007) Deep Bilateral Retinex for Low-Light Image Enhancement <Br>
**[Author]** Jinxiu Liang, Yong Xu, [Yuhui Quan](https://csyhquan.github.io/), Jingwen Wang, [Haibin Ling](https://www3.cs.stonybrook.edu/~hling/), [Hui Ji](https://blog.nus.edu.sg/matjh/)  <Br>

#### Fast Enhancement for Non-Uniform Illumination ★★
**[Paper]** (MM 2020) Fast Enhancement for Non-Uniform Illumination Images using Light-weight CNNs <Br>
**[Author]** [Feifan Lv](https://lvfeifan.github.io/), Bo Liu, [Feng Lu](http://shi.buaa.edu.cn/lufeng/)  <Br>
1) 超轻量级网络(~5k参数), 同时成立过曝光和欠曝光问题, 效果不错
2) 用一个illumination net预测原图和1-原图的illumination, 用来解决retinex理论不能处理过曝的局限. 然后把欠曝光修复结果, 过曝修复结果和原图送到fusion net中预测三个分量的权重, 进行加权融合. 最后用一个restoration net去除噪声和artifacts

#### Integrating Semantic Segmentation and Retinex Model ★
**[Paper]** (MM 2020) Integrating Semantic Segmentation and Retinex Model for Low Light Image Enhancement <Br>
**[Author]** [Minhao Fan](https://xfw-go.github.io/), [Wenjing Wang](https://daooshee.github.io/website/), [Wenhan Yang](https://flyywh.github.io/), [Jiaying Liu](http://39.96.165.147/people/liujiaying.html)  <Br>
**[[Project](https://mm20-semanticreti.github.io/)]** <Br>
将分割特征与Retinex网络结合做亮度增强
	
#### DALE ★
**[Paper]** (BMVC 2020) DALE : Dark Region-Aware Low-light Image Enhancement  <Br>
**[Author]** Dokyeong Kwon, Guisik Kim, [Junseok Kwon](http://prof.cau.ac.kr/~jskwon/) <Br>
**[[Pytorch-Code](https://github.com/dokyeongK/DALE)]** <Br>
通过改变每个超像素的亮度生成了一个数据集, 用来训练一个attention网络. 感觉一般.
	
#### RRDNet
**[Paper]** (ICME 2020) Zero-Shot Restoration of Underexposed Images via Robust Retinex Decomposition <Br>
**[Author]** Anqi Zhu, [Lin Zhang](https://sse.tongji.edu.cn/linzhang/), [Ying Shen](https://sse.tongji.edu.cn/yingshen/), Yong Ma, Shengjie Zhao, Yicong Zhou <Br>
**[[Pytorch-Code](https://github.com/aaaaangel/RRDNet)]** <Br>

#### Low-Light Image Enhancement via a Deep Hybrid Network ☆
**[Paper]** (TIP 2019) Low-Light Image Enhancement via a Deep Hybrid Network <Br>
**[Author]** [Wenqi Ren](https://sites.google.com/site/renwenqi888/home), [Sifei Liu](https://www.sifeiliu.net/), [Lin Ma](http://forestlinma.com/), [Qianqian Xu](https://qianqianxu010.github.io/), [Xiangyu Xu](https://sites.google.com/view/xiangyuxu), [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en), Junping Du, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/)  <Br>
**[[Code](https://sites.google.com/site/renwenqi888/home)]**   <Br>
分为全局对比度增强和细节增强两支, 细节部分使用了RNN
	
#### Progressive Retinex
**[Paper]** (MM 2019) Progressive Retinex: Mutually Reinforced Illumination-Noise Perception Network for Low Light Image Enhancement<Br>
**[Author]**  Yang Wang, Yang  Cao Zheng-Jun Zha, [Jing Zhang](https://chaimi2013.github.io/), [Zhiwei  Xiong](http://staff.ustc.edu.cn/~zwxiong/), Wei  Zhang, Feng  Wu <Br>
	
#### KinD ★★
**[Paper]** (MM 2019) Kindling the Darkness: A Practical Low light Image Enhancer<Br>
**[Author]** Yonghua Zhang, Jiawan Zhang, [Xiaojie Guo](https://sites.google.com/view/xjguo) <Br>
**[[TF-Code-KinD](https://github.com/zhangyhuaee/KinD)]** **[[TF-Code-KinD++](https://github.com/zhangyhuaee/KinD_plus)]**<Br>
1) 采用类似Retinex的结构, 两个分支分别预测亮度分量和反射分量. 网络结构和loss可以参考. <Br>
2) 提出了一个小型的亮度adjustment net, 可以输入一个ratio, 控制增强程度, 比较有趣. <Br>
	
#### DeepUPE ★
**[Paper]** (CVPR 2019) Underexposed Photo Enhancement Using Deep Illumination Estimation<Br>
**[Author]** Ruixing Wang, [Qing Zhang](http://zhangqing-home.net/), [Chi-Wing Fu](https://www.cse.cuhk.edu.hk/~cwfu/), [Xiaoyong Shen](http://xiaoyongshen.me/), [Wei-Shi Zheng](https://sites.google.com/site/sunnyweishi/), [Jiaya Jia](http://jiaya.me/) <Br>
**[[TF-code](https://github.com/wangruixing/DeepUPE)]** <Br>
同样基于Retinex理论, 但网络只预测illumination map, 使用了reconstruction, color和smooth loss. 整个工程都建立在HDRNet的基础上. 用联合上采样的思路做tone mapping的思路感觉可以挖掘一下.

#### Learning digital camera pipeline for extreme low-light imaging
**[Paper]** (arXiv 1904) Learning digital camera pipeline for extreme low-light imaging <Br>
**[Author]**  Syed Waqas Zamir, [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Fahad Shahbaz Khan](https://sites.google.com/view/fahadkhans/home), Ling Shao <Br>

#### EnlightenGAN ★★
**[Paper]** (arXiv 1906) EnlightenGAN: Deep Light Enhancement without Paired Supervision <Br>
**[Author]** [Yifan Jiang](http://yifanjiang.net/), [Xinyu Gong](https://gongxinyuu.github.io/), Ding Liu, [Yu Cheng](https://sites.google.com/site/chengyu05), [Chen Fang](http://fangchen.org/), [Xiaohui Shen](https://xiaohuishen.github.io/), [Jianchao Yang](http://www.ifp.illinois.edu/~jyang29/), Pan Zhou, Zhangyang Wang  <Br>
**[[Pytorch-code](https://github.com/TAMU-VITA/EnlightenGAN)]** <Br>
基于GAN的非监督亮度增强方法, 效果不错 <Br>
	
#### Retinex-GAN ☆
**[Paper]** (arXiv 1906) Low-light Image Enhancement Algorithm Based on Retinex and Generative Adversarial Network <Br>
**[Author]** Yangming Shi, Xiaopo Wu, Ming Zhu  <Br>
RetinexNet+GAN
	
#### Attention-guided Low-light Image Enhancement ★☆
**[Paper]** (arXiv 1908) Attention Guided Low-light Image Enhancement with a Large Scale Low-light Simulation Dataset <Br>
**[Author]** [Feifan Lv](https://lvfeifan.github.io/), [Yu Li](http://yu-li.github.io/), [Feng Lu](http://shi.buaa.edu.cn/lufeng/)  <Br>
**[[Project](http://phi-ai.org/project/AgLLNet/default.htm)]**<Br>
1) 同时做tone mapping和去噪, 分为亮度attention map预测, noise map预测, 多尺度增强模块和refine模块四部分, 网络结构和loss可以参考 <Br>
2) 提出了一个生成低光照加噪声数据的流程.

#### Color-wise Attention Network ★
**[Paper]** (arXiv 1911) Color-wise Attention Network for Low-light Image Enhancement <Br>
**[Author]** [Yousef Atoum](http://faculty.yu.edu.jo/atoumyou/SitePages/Home.aspx), [Mao Ye](https://maoye.wordpress.com/), Liu Ren, [Ying Tai](https://tyshiwo.github.io/), [Xiaoming Liu](http://cvlab.cse.msu.edu/) <Br>
亮度和颜色通道分两只分别增强的方案, 其中color和point的attention部分没看懂

#### Exposure ★
**[Paper]** (SIGGRAPH 2018) Exposure: A White-Box Photo Post-Processing Framework <Br>
**[Author]** [Yuanming Hu](http://taichi.graphics/me/), [Hao He](http://people.csail.mit.edu/hehaodele/), Chenxi Xu, [Baoyuan Wang](https://sites.google.com/site/zjuwby/), Stephen Lin <Br>
**[[TF-Code](https://github.com/yuanming-hu/exposure)]** <Br> 
胡渊明大神在图像质量增强领域的一篇论文, 用增强学习对图像进行对比度, 曝光度, gamma等方面的校正. 由于实际部署的限制, 目前未对增强学习有所了解.
	
#### SICE 
**[Paper]** (TIP 2018) Learning a Deep Single Image Contrast Enhancer from Multi-Exposure Images <Br>
**[Author]** [Jianrui Cai](https://csjcai.github.io/), [Shuhang Gu](https://sites.google.com/site/shuhanggu/), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
**[[Caffe-Code](https://github.com/csjcai/SICE)]** <Br>
	
#### GLADNet ☆
**[Paper]** (FG 2018) GLADNet: Low-Light Enhancement Network with Global Awareness <Br>
**[Author]** [Wenjing Wang](https://daooshee.github.io/website/),[Chen Wei](https://weichen582.github.io/), [Wenhan Yang](https://flyywh.github.io/index.html), [Jiaying Liu](http://39.96.165.147/people/liujiaying.html) <Br>
**[[Project](https://daooshee.github.io/fgworkshop18Gladnet/)]**   **[[TF-Code](https://github.com/weichen582/GLADNet)]** <Br>
encoder-decoder + refine结构的网络
	
#### LightenNet
**[Paper]** (PRL 2018) LightenNet: A Convolutional Neural Network For Weakly Illuminated Image Enhancement <Br>
**[Author]** [Chongyi Li](https://li-chongyi.github.io/sub_publication.html), Jichang Guo, [Fatih Porikli](http://www.porikli.com/), Yanwei Pang <Br>
**[[Project](https://li-chongyi.github.io/proj_lowlight.html)]**  	

#### RetinexNet ★
**[Paper]** (BMVC 2018 Oral) Deep Retinex Decomposition for Low-Light Enhancement <Br>
**[Author]** [Chen Wei](https://weichen582.github.io/), [Wenjing Wang](https://daooshee.github.io/website/), [Wenhan Yang](https://flyywh.github.io/index.html), [Jiaying Liu](http://39.96.165.147/people/liujiaying.html)  <Br>
**[[Project](https://daooshee.github.io/BMVC2018website/)]**   **[[TF-Code](https://github.com/weichen582/RetinexNet)]** <Br>
基于retinex理论设计的网络, 后续一些工作基于这个思路展开, 但本文的效果一般
	
#### MBLLEN ★
**[Paper]** (BMVC 2018) MBLLEN: Low-light Image/Video Enhancement Using CNNs <Br>
**[Author]** [Feifan Lv](https://lvfeifan.github.io/), [Feng Lu](http://shi.buaa.edu.cn/lufeng/), Jianhua Wu, Chongsoon Lim <Br>
**[[Page](http://phi-ai.org/project/MBLLEN/default.htm)]**   **[[TF-Code](https://github.com/Lvfeifan/MBLLEN)]** <Br>
多分支亮度增强网络
	
#### Deep Photo Enhancer ★☆
**[Paper]** (CVPR 2018 Spotlight) Deep Photo Enhancer: Unpaired Learning for Image Enhancement from Photographs with GANs <Br>
**[Author]** [Yu-Sheng Chen](https://www.cmlab.csie.ntu.edu.tw/~nothinglo/), [Yu-Ching Wang](https://www.cmlab.csie.ntu.edu.tw/~urchinwang/), [Man-Hsin Kao](https://www.cmlab.csie.ntu.edu.tw/~cindy0711/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/) <Br>
**[[TF-Code](https://github.com/nothinglo/Deep-Photo-Enhancer)]** **[[TF-Code2](https://github.com/pnbao/deep-photo-enhance)]**<Br>
UNet + cycGAN, 无需paired样本的图像增强方法, 可以参考, 只是代码有一点点乱

#### Distort-and-Recover
**[Paper]** (CVPR 2018) Distort-and-recover: Color Enhancement Using Deep Reinforcement Learning <Br>
**[Author]** Jongchan Park, [Joon-Young Lee](https://joonyoung-cv.github.io/), [Donggeun Yoo](https://dgyoo.github.io/), In So Kweon <Br>
**[[TF-Code](https://github.com/Jongchan/DISTORT-AND-RECOVER-CVPR18)]**<Br>
	
#### DeepExposure
**[Paper]** (NIPS 2018) DeepExposure: Learning to Expose Photos with Asynchronously Reinforced Adversarial Learning <Br>
**[Author]** Runsheng Yu, Wenyu Liu, Yasen Zhang, Zhi Qu, [Deli Zhao](https://sites.google.com/site/zhaodeli/), Bo Zhang <Br>

#### LECARM
**[Paper]** (TCS 2018) LECARM: Low-Light Image Enhancement Using the Camera Response Model <Br>
**[Author]** Yurui Ren; [Zhenqiang Ying](https://baidut.github.io/about/); Thomas H. Li; Ge Li <Br>
(传统方法) 利用CRF和BTF做增强
	
#### MSR-net ★☆
**[Paper]** (arXiv 1711) MSR-net:Low-light Image Enhancement Using Deep Convolutional Network <Br>
**[Author]** Liang Shen, Zihan Yue, Fan Feng, Quan Chen, Shihao Liu, Jie Ma <Br>
用CNN做亮度增强较早的一篇, 个人觉得该网络结构可能未必效果很好, 但思路值得学习. 本文认为传统的MSR(multi scale Retinex)在实际应用中可以DoG的形式近似, 不同核的高斯函数可用若干个卷积stack代替. 提出的网络首先将低光照输入做不同程度的亮度调整并变换到log域, 之后再仿照MSR的形式用CNN对输入进行亮度增强, 最后是一个1x1的颜色恢复模块. 

#### Image-Contrast-Enhancement ★★
**[Paper]** (CAIP 2017) A New Image Contrast Enhancement Algorithm Using Exposure Fusion Framework <Br>
**[Author]** [Zhenqiang Ying](https://baidut.github.io/about/), Ge Li, Yurui Ren, Ronggang Wang, Wenmin Wang   <Br>
**[[Project](https://baidut.github.io/OpenCE/caip2017.html)]** **[[Matlab-Code](https://github.com/AndyHuang1995/Image-Contrast-Enhancement)]** **[[Python-Code](https://github.com/AndyHuang1995/Image-Contrast-Enhancement)]** <Br>
大致浏览, 利用原图和曝光增强后的图像融合, 提升亮度和对比度. 融合权值通过求解光照强度得到, 曝光增强图通过作者之前提出的相机响应校正模型得到.
	


