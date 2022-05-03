# Table of Contents
- [Image Super Resolution](#super-resolution)
- [Datasets](#datasets)
- [Resources](#resources)

#  Image Super Resolution
#### NAFNet
**[Paper]**  (arXiv 2204) Simple Baselines for Image Restoration<Br>
**[Author]** Liangyu Chen, Xiaojie Chu, Xiangyu Zhang, [Jian Sun](http://www.jiansun.org/) <Br>
**[[Pytorch-Code](https://github.com/megvii-research/NAFNet/)]**   <Br>

#### RCAN-it
**[Paper]** (arXiv 2201) Revisiting RCAN: Improved Training for Image Super-Resolution <Br>
**[Author]** Zudi Lin, Prateek Garg, Atmadeep Banerjee, [Salma Abdel Magid](https://sites.google.com/view/salma-abdelmagid/), [Deqing Sun](https://deqings.github.io/), [Yulun Zhang](http://yulunzhang.com/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html), [Donglai Wei](https://donglaiw.github.io/), [Hanspeter Pfister](https://vcg.seas.harvard.edu/people) <Br>
**[[Pytorch-Code](https://github.com/zudi-lin/rcan-it)]**   <Br>

#### ARM-Net
**[Paper]** (CVPR 2022) ARM: Any-Time Super-Resolution Method <Br>
**[Author]** Bohong Chen, [Mingbao Lin](https://lmbxmu.github.io/), Kekai Sheng, Mengdan Zhang, Peixian Chen, [Ke Li](https://keli-61.github.io/), Liujuan Cao, [Rongrong Ji](https://mac.xmu.edu.cn/rrji_en/) <Br>
**[[Pytorch-Code](https://github.com/chenbong/ARM-Net)]**   <Br>
		
#### DPT
**[Paper]** (AAAI 2022) Detail-Preserving Transformer for Light Field Image Super-Resolution <Br>
**[Author]** Shunzhou Wang, [Tianfei Zhou](https://www.tfzhou.com/), Yao Lu, Huijun Di <Br>
**[[Pytorch-Code](https://github.com/BITszwang/DPT)]**   <Br>
	
#### Real-ESRGAN
**[Paper]**  (arXiv 2107) Real-ESRGAN: Training Real-World Blind Super-Resolution with Pure Synthetic Data <Br>
**[Author]** [Xintao Wang](https://xinntao.github.io/), Liangbie Xie, Chao Dong, Ying Shan <Br>
**[[Pytorch-Code](https://github.com/xinntao/Real-ESRGAN)]**   <Br>
	
#### GhostSR ★☆
**[Paper]**  (arXiv 2101) GhostSR: Learning Ghost Features for Efficient Image Super-Resolution <Br>
**[Author]** Ying Nie, Kai Han, Zhenhua Liu, An Xiao, Yiping Deng, Chunjing Xu, Yunhe Wang <Br>
(**轻量级超分**) 使用pixel shift的思想做超分
	
#### SplitSR ★☆
**[Paper]**  (arXiv 2101) SplitSR: An End-to-End Approach to Super-Resolution on Mobile Devices <Br>
**[Author]** [Xin Liu](https://homes.cs.washington.edu/~xliu0/), Yuang Li, [Josh Fromm](https://jwfromm.com/), [Yuntao Wang](http://pi.cs.tsinghua.edu.cn/lab/people/YuntaoWang/), [Ziheng Jiang](https://www.ziheng.org/), [Alex Mariakakis](https://mariakakis.github.io/), Shwetak Patel <Br>
**[[Unofficial-Pytorch-Code](https://github.com/deepconsc/SplitSR)]**  <Br>
(**轻量级超分**) 提出了一个轻量级residual block结构: SplitSRBlock

#### ECBSR ★☆
**[Paper]**  (MM 2021 Oral) About Edge-oriented Convolution Block for Real-time Super Resolution on Mobile Devices <Br>
**[Author]** Xindong Zhang, [Hui Zeng](https://huizeng.github.io/), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
**[[Pytorch-Code](https://github.com/xindongzhang/ECBSR)]**  <Br>
重参数化, 并行卷积模块+sobel/laplacian算子

#### Deep Reparametrization
**[Paper]** (ICCV 2021 Oral) Deep Reparametrization of Multi-Frame Super-Resolution and Denoising<Br>
**[Author]** [Goutam Bhat](https://goutamgmb.github.io/), [Martin Danelljan](https://martin-danelljan.github.io/), [Fisher Yu](https://www.yf.io/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html), [Radu Timofte](http://people.ee.ethz.ch/~timofter/) <Br>

#### BSRGAN
**[Paper]** (ICCV 2021) Designing a Practical Degradation Model for Deep Blind Image Super-Resolution <Br>
**[Author]** [Kai Zhang](https://cszn.github.io/), Jingyun Liang, [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html), [Radu Timofte](http://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/cszn/BSRGAN)]**    <Br>
	
#### MANet
**[Paper]** (ICCV 2021) Mutual Affine Network for Spatially Variant Kernel Estimation in Blind Image Super-Resolution <Br>
**[Author]** Jingyun Liang, Guolei Sun, [Kai Zhang](https://cszn.github.io/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html), [Radu Timofte](http://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/JingyunLiang/MANet)]**    <Br>
	
#### HCFlow
**[Paper]** (ICCV 2021) Hierarchical Conditional Flow: A Unified Framework for Image Super-Resolution and Image Rescaling <Br>
**[Author]** Jingyun Liang, Andreas Lugmayr, [Kai Zhang](https://cszn.github.io/), [Martin Danelljan](https://martin-danelljan.github.io/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html), [Radu Timofte](http://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/JingyunLiang/HCFlow)]**    <Br>

#### DCSR
**[Paper]** (ICCV 2021 Oral) Dual-Camera Super-Resolution with Aligned Attention Modules <Br>
**[Author]** [Tengfei Wang](https://tengfei-wang.github.io/), [Jiaxin Xie](https://jiaxinxie97.github.io/Jiaxin-Xie/), [Wenxiu Sun](http://wenxiusun.com/), [Qiong Yan](http://yan-qiong.com/), [Qifeng Chen](https://cqf.io/) <Br>
**[[Project](https://longguangwang.github.io/Project/ArbSR/)]** **[[Pytorch-Code](https://github.com/LongguangWang/ArbSR)]**    <Br>

#### ArbSR
**[Paper]** (ICCV 2021) Learning A Single Network for Scale-Arbitrary Super-Resolution <Br>
**[Author]** [Longguang Wang](https://longguangwang.github.io/), [Yingqian Wang](https://yingqianwang.github.io/), Zaiping Lin, Jungang Yang, Wei An, [Yulan Guo](http://yulanguo.me/) <Br>
**[[Project](https://longguangwang.github.io/Project/ArbSR/)]** **[[Pytorch-Code](https://github.com/LongguangWang/ArbSR)]**    <Br>

#### sr-uncertainty
**[Paper]** (CVPR 2021) Fast Bayesian Uncertainty Estimation and reduction of Batch Normalized Single Image Super-Resolution Network <Br>
**[Author]** [Aupendu Kar](https://aupendu.github.io/), [Prabir Kumar Biswas](http://www.ecdept.iitkgp.ac.in/Eece/facultydetails/ece-pkb) <Br>
**[[Project](https://aupendu.github.io/sr-uncertainty)]** **[[Pytorch-Code](https://github.com/aupendu/sr-uncertainty)]**    <Br>
	
#### BURSTSR
**[Paper]** (CVPR 2021) Deep Burst Super-Resolution <Br>
**[Author]** [Goutam Bhat](https://goutamgmb.github.io/), [Martin Danelljan](https://martin-danelljan.github.io/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html), [Radu Timofte](https://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/goutamgmb/NTIRE21_BURSTSR)]**   <Br>
	
#### DASR
**[Paper]** (CVPR 2021) Unsupervised Real-World Image Super Resolution via Domain-Distance Aware Training <Br>
**[Author]** Yunxuan Wei, [Shuhang Gu](https://shuhanggu.github.io/), [Yawei Li](https://ofsoundof.github.io/), Longcun Jin <Br>
**[[Pytorch-Code](https://github.com/ShuhangGu/DASR)]**   <Br>
	
#### Non-Local-Sparse-Attention
**[Paper]** (CVPR 2021) Image Super-Resolution With Non-Local Sparse Attention <Br>
**[Author]** [Yiqun Mei](https://yiqunmei.net/), [Yuchen Fan](https://ychfan.github.io/), [Yuqian Zhou](https://yzhouas.github.io/) <Br>
**[[Pytorch-Code](https://github.com/HarukiYqM/Non-Local-Sparse-Attention)]**   <Br>
	
#### KOALAnet
**[Paper]** (CVPR 2021) KOALAnet: Blind Super-Resolution using Kernel-Oriented Adaptive Local Adjustment <Br>
**[Author]** [Soo Ye Kim](https://sites.google.com/view/sooyekim), [Hyeonjun Sim](https://sites.google.com/view/hjsim), [Munchurl Kim]https://www.viclab.kaist.ac.kr/) <Br>
**[[Pytorch-Code](https://github.com/hjSim/KOALAnet)]**   <Br>
	
#### AdaTarget ★
**[Paper]** (CVPR 2021) Tackling the Ill-Posedness of Super-Resolution through Adaptive Target Generation <Br>
**[Author]** [Younghyun Jo](https://yhjo09.github.io/), [Seoung Wug Oh], [Peter Vajda](https://sites.google.com/site/vajdap/), [Seon Joo Kim](https://sites.google.com/site/seonjookim/) <Br>
**[[Pytorch-Code](https://github.com/yhjo09/AdaTarget)]**   <Br>
认为在SR任务中, HR和LR位置并不是完全对应的, 因此设计了一个ART模块, 对GT patch进行仿射变换, 使LR和HRpair更加匹配

#### Single Pair Cross-Modality
**[Paper]** (CVPR 2021) Single Pair Cross-Modality Super Resolution <Br>
**[Author]** Guy Shacht, Dov Danon, Sharon Fogel, Daniel Cohen-Or <Br>
	
#### SR-LUT
**[Paper]** (CVPR 2021) Practical Single-Image Super-Resolution Using Look-Up Table <Br>
**[Author]** [Younghyun Jo](https://yhjo09.github.io/), [Seon Joo Kim](https://sites.google.com/site/seonjookim/) <Br>
**[[Pytorch-Code](https://github.com/yhjo09/SR-LUT)]**   <Br>

#### SRFlow-DA
**[Paper]** (CVPRW 2021) SRFlow-DA: Super-Resolution Using Normalizing Flow with Deep Convolutional Block <Br>
**[Author]** [Younghyun Jo](https://yhjo09.github.io/), [Sejong Yang](https://yangspace.co.kr/), [Seon Joo Kim](https://sites.google.com/site/seonjookim/) <Br>
**[[Pytorch-Code](https://github.com/yhjo09/SRFlow-DA)]**   <Br>
	
#### SRWarp
**[Paper]** (CVPR 2021) SRWarp: Generalized Image Super-Resolution under Arbitrary Transformation <Br>
**[Author]** [Sanghyun Son](https://cv.snu.ac.kr/), [Kyoung Mu Lee](https://cv.snu.ac.kr/index.php/~kmlee/) <Br>
**[[Pytorch-Code](https://github.com/sanghyun-son/srwarp)]**   <Br>

#### LAM
**[Paper]** (CVPR 2021) Interpreting Super-Resolution Networks with Local Attribution Maps <Br>
**[Author]** [Jinjin Gu](http://www.jasongt.com/), [Chao Dong](https://xpixel.group/index.html)   <Br>
**[[Project](https://x-lowlevel-vision.github.io/lam.html)]**   <Br>

#### FKP
**[Paper]** (CVPR 2021) Flow-based Kernel Prior with Application to Blind Super-Resolution <Br>
**[Author]** Jingyun Liang, [Kai Zhang](https://cszn.github.io/), [Shuhang Gu](https://sites.google.com/site/shuhanggu/), [Luc Van Gool](www.vision.ee.ethz.ch/members/get_member.cgi?lang=en&id=1), [Radu Timofte](http://people.ee.ethz.ch/~timofter/)   <Br>
**[[Pytorch-Code](https://github.com/JingyunLiang/FKP)]**   <Br>

#### MASA-SR 
**[Paper]** (CVPR 2021) MASA-SR: Matching Acceleration and Spatial Adaptation for Reference-Based Image Super-Resolution <Br>
**[Author]** Liying Lu, Wenbo Li, [Xin Tao](http://www.xtao.website/), Jiangbo Lu, [Jiaya Jia](https://jiaya.me/)   <Br>
**[[Pytorch-Code](https://github.com/dvlab-research/MASA-SR)]**   <Br>

#### GLEAN 
**[Paper]** (CVPR 2021 Oral) GLEAN: Generative Latent Bank for Large-Factor Image Super-Resolution <Br>
**[Author]** [Kelvin C.K. Chan](https://ckkelvinchan.github.io/), [Xintao Wang](https://xinntao.github.io/), [Xiangyu Xu](https://sites.google.com/view/xiangyuxu/), [Jinwei Gu](https://www.gujinwei.org/), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/)   <Br>
**[[Project](https://ckkelvinchan.github.io/projects/GLEAN/)]**   <Br>

#### LIIF 
**[Paper]** (CVPR 2021 Oral) Learning Continuous Image Representation with Local Implicit Image Function <Br>
**[Author]** [Yinbo Chen](https://yinboc.github.io/), [Sifei Liu](https://www.sifeiliu.net/), [Xiaolong Wang](https://xiaolonw.github.io/)  <Br>
**[[Project](https://yinboc.github.io/liif/)]** **[[Pytorch-Code](https://github.com/yinboc/liif)]**  <Br>

#### LAU-Net 
**[Paper]** (CVPR 2021) LAU-Net: Latitude Adaptive Upscaling Network for Omnidirectional Image Super-resolution <Br>
**[Author]** [Yinbo Chen](https://yinboc.github.io/), [Sifei Liu](https://www.sifeiliu.net/), [Xiaolong Wang](https://xiaolonw.github.io/)  <Br>
**[[Pytorch-Code](https://github.com/wangh-allen/LAU-Net)]**  <Br>

#### Cross-MPI
**[Paper]**  (CVPR 2021) Cross-MPI: Cross-scale Stereo for Image Super-Resolution using Multiplane Images <Br>
**[Author]** Yuemei Zhou, Gaochang Wu, Ying Fu, Kun Li, [Yebin Liu](http://www.liuyebin.com/) <Br>
**[[Project](http://www.liuyebin.com/crossMPI/crossMPI.html)]**  <Br>

#### ClassSR
**[Paper]**  (CVPR 2021) ClassSR: A General Framework to Accelerate Super-Resolution Networks by Data Characteristic <Br>
**[Author]** Xiangtao Kong, [Hengyuan Zhao](https://github.com/zhaohengyuan1), [Yu Qiao](https://scholar.google.com/citations?user=gFtI-8QAAAAJ&hl=zh-CN), Chao Dong <Br>
**[[Pytorch-Code](https://github.com/Xiangtaokong/ClassSR)]**  <Br>

#### SMSR
**[Paper]**  (CVPR 2021) Exploring Sparsity in Image Super-Resolution for Efficient Inference <Br>
**[Author]** [Longguang Wang](https://longguangwang.github.io/), Xiaoyu Dong, [Yingqian Wang](https://yingqianwang.github.io/), Xinyi Ying, Zaiping Lin, Wei An, [Yulan Guo](http://yulanguo.me/)  <Br>
**[[Pytorch-Code](https://github.com/LongguangWang/SMSR)]**  <Br>

#### DASR
**[Paper]**  (CVPR 2021) Unsupervised Degradation Representation Learning for Blind Super-Resolution <Br>
**[Author]** [Longguang Wang](https://longguangwang.github.io/), [Yingqian Wang](https://yingqianwang.github.io/), Xiaoyu Dong, Qingyu Xu, Jungang Yang, Wei An, [Yulan Guo](http://yulanguo.me/) <Br>
**[[Pytorch-Code](https://github.com/LongguangWang/DASR)]**  <Br>

#### C2-Matching
**[Paper]**  (CVPR 2021) Robust Reference-based Super-Resolution via C²-Matching <Br>
**[Author]** [Yuming Jiang](https://yumingj.github.io/), [Kelvin C.K. Chan](https://ckkelvinchan.github.io/), [Xintao Wang](https://xinntao.github.io/), [Chen Change Loy](https://www.mmlab-ntu.com/person/ccloy/), [Ziwei Liu](https://liuziwei7.github.io/) <Br>
**[[Project](https://yumingj.github.io/projects/C2_matching)]**  **[[Pytorch-Code](https://github.com/yumingj/C2-Matching)]**  <Br>

#### AdderSR ★
**[Paper]**  (CVPR 2021) AdderSR: Towards Energy Efficient Image Super-Resolution <Br>
**[Author]** Dehua Song, Yunhe Wang, Hanting Chen, [Chang Xu](http://changxu.xyz/), Chunjing Xu, Dacheng Tao <Br>
使用加法做SR
	
#### Data-Free Knowledge Distillation For Image Super-Resolution
**[Paper]**  (CVPR 2021) Data-Free Knowledge Distillation For Image Super-Resolution <Br>
**[Author]** Yiman Zhang, Hanting Chen, Xinghao Chen, Yiping Deng, Chunjing Xu, [Yunhe Wang](https://www.wangyunhe.site/) <Br>
	
#### AMNet
**[Paper]** (CVPR 2021) Learning the Non-Differentiable Optimization for Blind Super-Resolution <Br>
**[Author]** Zheng Hui, Jie Li, Xiumei Wang, [Xinbo Gao](https://see.xidian.edu.cn/faculty/xbgao/) <Br>

#### FCA ★
**[Paper]**  (AAAI 2021) Frequency Consistent Adaptation for RealWorld Super Resolution <Br>
**[Author]** Xiaozhong Ji, Guangpin Tao, Yun Cao, [Ying Tai](https://tyshiwo.github.io/), Tong Lu, Chengjie Wang, Jilin Li, Feiyue Huang <Br>
	
#### MAFFSRN ★☆
**[Paper]**  (arXiv 2008) Ultra Lightweight Image Super-Resolution with Multi-Attention Layers <Br>
**[Author]** Abdul Muqeet, Jiwon Hwang, Subin Yang, Jung Heum Kang, Yongwoo Kim, Sung-Ho Bae<Br>
**[[Code](https://github.com/AbdulMoqeet/MAFFSRN)]** <Br>
轻量级超分网络


#### RFDN ★☆
**[Paper]**  (arXiv 2009) Residual Feature Distillation Network for Lightweight Image Super-Resolution <Br>
**[Author]** Jie Liu, Jie Tang, Gangshan Wu<Br>
**[[Pytorch-Code](https://github.com/njulj/RFDN)]** <Br>
AIM2020-ESR冠军方案, 基于IDN提出了几点改善.


#### A2F ★
**[Paper]**  (ACCV 2020) Lightweight Single-Image Super-Resolution Network with Attentive Auxiliary Feature Learning <Br>
**[Author]** [Xuehui Wang,](http://wangxuehui.site)   [Qing Wang,](https://cv.wangxuehui.site/SR/)  [Yuzhi Zhao,](https://cv.wangxuehui.site/SR/)  [Junchi Yan,](https://cv.wangxuehui.site/SR/) [Lei Fan,](https://cv.wangxuehui.site/SR/)  [Long Chen]( <Br>
**[[Project](https://cv.wangxuehui.site/SR/)]**  <Br>
(**轻量级超分**) 使用attention和dense connection思想

#### loss functions for extreme super-resolution
**[Paper]** (CVPRW 2020) Investigating loss functions for extreme super-resolution <Br>
**[Author]**  [Younghyun Jo](https://yhjo09.github.io/), [Sejong Yang](https://yangspace.co.kr/), [Seon Joo Kim](https://sites.google.com/site/seonjookim/) <Br>
**[[Pytorch-Code](https://github.com/kingsj0405/ciplab-NTIRE-2020)]** <Br>
	
#### DRN ★
**[Paper]** (CVPR 2020) Closed-loop Matters: Dual Regression Networks for Single Image Super-Resolution <Br>
**[Author]**  [Yong Guo](http://www.guoyongcs.com/), Jian Chen, [Jingdong Wang](https://jingdongwang2017.github.io/), Qi Chen, [Jiezhang Cao](https://www.jiezhangcao.com/), Zeshuai Deng, [Yanwu Xu](https://xuyanwu.github.io/), [Mingkui Tan](https://tanmingkui.github.io/)<Br>
**[[Pytorch-Code](https://github.com/guoyongcs/DRN)]** <Br>
训练时引入HR->LR的映射, 对LR图像进行额外的约束. 大致浏览.
 
#### USRNet ★
**[Paper]** (CVPR 2020) Deep Unfolding Network for Image Super-Resolution <Br>
**[Author]** [Kai Zhang](https://cszn.github.io/), [Luc Van Gool](https://vision.ee.ethz.ch/people-details.OTAyMzM=.TGlzdC8zMjQ4LC0xOTcxNDY1MTc4.html), [Radu Timofte](http://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/cszn/USRNet)]** <Br>
大致浏览, 通过变量分解迭代求解, 一部分用FFT直接求解, 一部分用网络训练.

#### RFANet ★
**[Paper]** (CVPR 2020) Residual Feature Aggregation Network for Image Super-resolution <Br>
**[Author]** Jie Liu, Wenjie Zhang, Yuting Tang, Jie Tang, Gangshan Wu <Br>
**[[Code](https://github.com/njulj/RFANet)]** <Br>
设计了一个残差聚合和attention模块
	
#### Cross Scale Non Local Attention ★☆
**[Paper]** (CVPR 2020) Image Super-Resolution with Cross-Scale Non-Local Attention and Exhaustive Self-Exemplars Mining <Br>
**[Author]** [Yiqun Mei](http://yiqunm2.web.illinois.edu/), [Yuchen Fan](https://ychfan.github.io/), [Yuqian Zhou](https://yzhouas.github.io/), Lichao Huang, [Thomas S. Huang](https://ifp-uiuc.github.io/), [Humphrey Shi](https://www.humphreyshi.com/) <Br>
**[[Pytorch-Code](https://github.com/SHI-Labs/Cross-Scale-Non-Local-Attention)]** <Br>
设计了LR到降采样LR的attention, 挖掘不同尺度下的non-local相似性

#### TTSR ★★
**[Paper]** (CVPR 2020) TTSR: Learning Texture Transformer Network for Image Super-Resolution <Br>
**[Author]** Fuzhi Yang, Huan Yang, Jianlong Fu, Hongtao Lu, Baining Guo <Br>
**[[Pytorch-Code](https://github.com/researchmm/TTSR)]** <Br>
使用transformer从参考图像获取纹理信息
	
#### *Unpaired Image Super-Resolution using Pseudo-Supervision* ★
**[Paper]** (CVPR 2020) Unpaired Image Super-Resolution using Pseudo-Supervision <Br>
**[Author]** Shunta Maeda <Br>
大致浏览, 类似CycleGAN的结构

#### SPSR ★
**[Paper]** (CVPR 2020) Structure-Preserving Super Resolution with Gradient Guidance  <Br>
**[Author]** Cheng Ma, [Yongming Rao](https://raoyongming.github.io/), Yean Cheng, Ce Chen, [Jiwen Lu](http://ivg.au.tsinghua.edu.cn/Jiwen_Lu/), Jie Zhou <Br>
**[[Pytorch-Code](https://github.com/Maclory/SPSR)]** <Br>
在常规超分分支外加入一个gradient分支

#### PULSE ★★
**[Paper]** (CVPR 2020) PULSE: Self-Supervised Photo Upsampling via Latent Space Exploration of Generative Models  <Br>
**[Author]** [Sachit Menon](https://sachit-menon.github.io/), Alexandru Damian, Shijia Hu, Nikhil Ravi, [Cynthia Rudin](https://users.cs.duke.edu/~cynthia/home.html) <Br>
**[[Pytorch-Code](https://github.com/adamian98/pulse)]** <Br>
**(无监督SR)** 通过在LR空间优化latent vector使生成的HR图像符合LR图像的内容. 思路很有意思.
	
#### Correction Filter
**[Paper]** (CVPR 2020 Oral) Correction Filter for Single Image Super-Resolution: Robustifying Off-the-Shelf Deep Super-Resolvers  <Br>
**[Author]** Shady Abu Hussein, [Tom Tirer](https://tirertom.wixsite.com/homepage), [Raja Giryes](http://web.eng.tau.ac.il/~raja/) <Br>
**[[Pytorch-Code](https://github.com/shadyabh/Correction-Filter)]** <Br>
	
#### MZSR
**[Paper]** (CVPR 2020) Meta-Transfer Learning for Zero-Shot Super-Resolution <Br>
**[Author]** Jae Woong Soh, Sunwoo Cho, Nam Ik Cho <Br>
**[[TF-Code](https://github.com/JWSoh/MZSR)]** <Br>
	
#### CutBlur ★
**[Paper]** (CVPR 2020) Rethinking Data Augmentation for Image Super-resolution: A Comprehensive Analysis and a New Strategy <Br>
**[Author]** Jaejun Yoo, [Namhyuk Ahn](https://nmhkahn.github.io/), [Kyung-Ah Sohn](https://sites.google.com/site/kasohn/home) <Br>
**[[Pytorch-Code](https://github.com/clovaai/cutblur)]** <Br>
(**数据增强方法**) 提出随机置换HR和LR中某一区域, 使网络能够判断哪些区域需要增强, 对过度锐化方面貌似有所改善
	
#### CARB ★☆
**[Paper]**  (CVPRW 2020) Guided Frequency Separation Network for Real-World Super-Resolution <Br>
**[Author]** Yuanbo Zhou, Wei Deng, Tong Tong, Qinquan Gao<Br>
**[[Pytorch-Code](https://github.com/fzuzyb/2020NTIRE-Guided-Frequency-Separation-Network-for-RWSR)]** <Br>
使用一套基于GAN的无监督方案生成真实LR图像对, 在该方案中提出了所谓颜色引导生成器网络, 用于产生AdaIn中的参数. 
	
#### REAL-SR ★★
**[Paper]** (CVPRW 2020) Real-World Super-Resolution via Kernel Estimation and Noise Injection <Br>
**[Author]** Xiaozhong Ji，Yun Cao， [Ying Tai](https://tyshiwo.github.io/)， Chengjie Wang，Jilin Li，Feiyue Huang<Br>
**[[Pytorch-Code](https://github.com/Tencent/Real-SR)]** <Br>
设计了一个退化图像的流程, 通过随机模糊核和注入噪声, 生成接近于真实的样本, 在NTIRE 2020超分竞赛中取得了第一名, 并且在真实数据上表现良好


#### TPSR ★
**[Paper]**  (ECCV 2020) Journey towards tiny perceptual superresolution <Br>
**[Author]** Royson Lee, Łukasz Dudziak, Mohamed Abdelfattah, Stylianos I. Venieris, Hyeji Kim, Hongkai Wen, Nicholas D. Lane <Br>
(**NAS, Mobile SR**)
	
#### MoreMNAS ★
**[Paper]**  (ECCV 2020) Multi-objective reinforced evolution in mobile neural architecture search <Br>
**[Author]** Xiangxiang Chu, Bo Zhang, Ruijun Xu, Hailong Ma <Br>
(**NAS, Mobile SR**)
	
#### CDC
**[Paper]**  (ECCV 2020) Component Divide-and-Conquer for Real-World Image Super-Resolution <Br>
**[Author]** Pengxu Wei, Ziwei Xie, Hannan Lu, Zongyuan Zhan, [Qixiang Ye](http://people.ucas.ac.cn/~qxye?language=en), [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), Liang Lin Lin<Br>
**[[Pytorch-Code](https://github.com/xiezw5/Component-Divide-and-Conquer-for-Real-World-Image-Super-Resolution)]** <Br>
	
#### SRFlow
**[Paper]**  (ECCV 2020) Learning the Super-Resolution Space with Normalizing Flow <Br>
**[Author]** Andreas Lugmayr, [Martin Danelljan](https://martin-danelljan.github.io/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html), [Radu Timofte](https://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/andreas128/SRFlow)]** <Br>	

#### HAN
**[Paper]**  (ECCV 2020) Single Image Super-Resolution via a Holistic Attention Network <Br>
**[Author]** Ben Niu, Weilei Wen, [Wenqi Ren](https://sites.google.com/site/renwenqi888/home), Xiangde Zhang, Lianping Yang, Shuzhen Wang, Kaihao Zhang, Xiaochun Cao, Haifeng Shen <Br>
**[[Pytorch-Code](https://github.com/wwlCape/HAN)]** <Br>	
	
#### SFM
**[Paper]**  (ECCV 2020) Stochastic Frequency Masking to Improve Super-Resolution and Denoising Networks <Br>
**[Author]** [Majed El Helou](https://majedelhelou.github.io/), Ruofan Zhou, Sabine Süsstrunk <Br>
**[[Pytorch-Code](https://github.com/majedelhelou/SFM)]** <Br>	
	
#### VarSR
**[Paper]**  (ECCV 2020) VarSR: Variational Super-Resolution Network for Very Low Resolution Images <Br>
**[Author]** Sangeek Hyun, Jae-Pil Heo <Br>

#### PISR
**[Paper]**  (ECCV 2020) Learning with Privileged Information for Efficient Image Super-Resolution <Br>
**[Author]** Junghyup Lee, Dohyung Kim, [Wonkyung Lee](https://cv.wonkyunglee.io/), [Bumbsub Ham](https://bsham.github.io/) <Br>
**[[Project](https://cvlab.yonsei.ac.kr/projects/PISR/)]** <Br> **[[Pytorch-Code](https://github.com/cvlab-yonsei/PISR)]** <Br>	

#### *Efficient Super Resolution Using Binarized Neural Network*
**[Paper]**  (ECCV 2020) Efficient Super Resolution Using Binarized Neural Network <Br>
**[Author]** Yinglan Ma, Hongyu Xiong, Zhe Hu, Lizhuang Ma <Br>
	
#### *Towards Content-independent Multi-Reference Super-Resolution: Adaptive Pattern Matching and Feature Aggregation*
**[Paper]**  (ECCV 2020) Towards Content-independent Multi-Reference Super-Resolution: Adaptive Pattern Matching and Feature Aggregation <Br>
**[Author]** Xu Yan, Weibing Zhao, Kun Yuan, Ruimao Zhang, [Zhen Li](https://mypage.cuhk.edu.cn/academics/lizhen/), Shuguang Cui <Br>

 #### *Zero-Shot Image Super-Resolution with Depth Guided Internal Degradation Learning*
**[Paper]** (ECCV 2020) Zero-Shot Image Super-Resolution with Depth Guided Internal Degradation Learning <Br>
**[Author]** Xi Cheng, Zhenyong Fu, Jian Yang <Br>

#### MLSR
**[Paper]** (ECCV 2020) Fast Adaptation to Super-Resolution Networks via Meta-Learning <Br>
**[Author]** Xi Cheng, Zhenyong Fu, Jian Yang <Br>
**[[TF-Code](https://github.com/parkseobin/MLSR)]** <Br>
 
#### LatticeNet ★
**[Paper]** (ECCV 2020) LatticeNet: Towards Lightweight Image Super-Resolution with Lattice Block <Br>
**[Author]** Xiaotong Luo, Yuan Xie, [Yulun Zhang](http://yulunzhang.com/), [Yanyun Qu](http://quyanyun.xmu.edu.cn/), Cuihua Li, Yun Fu  <Br>
(**轻量级超分**)
	
#### LAPAR ★☆
**[Paper]** (NIPS 2020) Linearly-Assembled Pixel-Adaptive Regression Network for Single Image Super-resolution and Beyond <Br>
**[Author]** Wenbo Li, Kun Zhou, [Lu Qi](http://luqi.info/), Nianjuan Jiang, Jiangbo Lu, [Jiaya Jia](https://jiaya.me/) <Br>
**[[Pytorch-Code](https://github.com/Jia-Research-Lab/Simple-SR)]** <Br>
预先定义L个滤波器, 滤波器是不同方向的高斯核和DoG核, 对LR进行bicubic插值, 用一个网络预测滤波器的系数.

#### IGNN
**[Paper]** (NIPS 2020) Cross-Scale Internal Graph Neural Network for Image Super-Resolution <Br>
**[Author]** [Shangchen Zhou](https://shangchenzhou.com/), [Jiawei Zhang](https://sites.google.com/site/zhjw1988), [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/)<Br>
**[[Pytorch-Code](https://github.com/sczhou/IGNN)]** <Br>

#### DAN
**[Paper]** (NIPS 2020) Unfolding the Alternating Optimization for Blind Super Resolution <Br>
**[Author]** Zhengxiong Luo, [Yan Huang](https://yanrockhuang.github.io/), Shang Li, Liang Wang, Tieniu Tan<Br>
**[[Pytorch-Code](https://github.com/greatlog/DAN)]** <Br>

#### Zoom to Learn, Learn to Zoom ★★
**[Paper]**  (CVPR 2019) Zoom to Learn, Learn to Zoom  <Br>
**[Author]** [Xuaner Zhang](https://ceciliavision.github.io/), [Qifeng Chen](https://cqf.io/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html), [Vladlen Koltun](http://vladlen.info/) <Br>
**[[Project](https://ceciliavision.github.io/project-pages/zoom.html)]** **[[TF-Code](https://github.com/ceciliavision/zoom-learn-zoom)]** <Br>
提出了考虑空间距离的bilateral contextual loss. 提出了一个由光学zoom图像对组成的raw超分数据集

####  *Super-Resolution with Raw Images* ★
**[Paper]**  (CVPR 2019) Towards Real Scene Super-Resolution with Raw Images  <Br>
**[Author]** [Xiangyu Xu](https://sites.google.com/view/xiangyuxu/%E9%A6%96%E9%A1%B5), Yongrui Ma, [Wenxiu Sun](http://wenxiusun.com/) <Br>
**[[Project](https://sites.google.com/view/xiangyuxu/rawsr_cvpr19)]** <Br>
大致浏览, 利用Raw做细节恢复, 用RGB做Color校正.<Br> 
	
#### SFTMD ★
**[Paper]**  (CVPR 2019) Blind Super-Resolution with Iterative Kernel Correction <Br>
**[Author]** [Jinjin Gu](http://www.jasongt.com/), Hannan Lu, [Wangmeng Zuo](http://www.jasongt.com/projectpages/IKC.html), Chao Dong<Br>
**[[Project](http://www.jasongt.com/projectpages/IKC.html)]** <Br>
1) 粗读, 提出一个基于深度学习的交替预测blur kernel和预测超分结果的模型, 对给定的blur有很好的效果 <Br>
2) 文中提出的预测blur kernel并用其辅助超分的思路很有意思, 但对真实图像而言无法获得真实的blur kernel用于训练, 另外论文似乎假设一张图像只有一种blur kernel, 感觉不太合理  <Br>
	
#### CameraSR ★
**[Paper]**  (CVPR 2019) Camera Lens Super-Resolution <Br>
**[Author]** Chang Chen, Zhiwei Xiong, Xinmei Tian, Zheng-Jun Zha, Feng Wu<Br>
**[[Code & Data](https://github.com/ngchc/CameraSR)]** <Br>
文章认为普通的插值退化不能模拟由于焦距-FOV变化带来的退化 (其实这是一个无论从分析上还是工程中都很明显的事实...). 最重要的贡献是提出了一个真实DSLR和手机的数据集, 但是在生成单反数据集时, 貌似没有考虑焦距变化带来的景深变化.
	
#### DPSR ★★
**[Paper]**  (CVPR 2019) Deep Plug-and-Play Super-Resolution for Arbitrary Blur Kernels <Br>
**[Author]** [Kai Zhang](https://cszn.github.io/), [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
**[[Pytorch-Code](https://github.com/cszn/DPSR)]** **[[Pytorch-IR-Toolbox](https://github.com/cszn/KAIR)]** <Br>
1. 把HR到LR的退化解释成bicubic降采样+非盲blur kernel退化+加性高斯白噪声的过程. 
2. 将求解过程用HQS变量分裂法分解为去模糊和超分+去噪两步, 第一步在频谱域求闭式解, 避免了模糊现象; 第二步可以使用现有的SR方法, 只需额外加入一噪声level. 采用迭代的形式交替求解.
3. 非盲kernel这个先验其实挺强的, 而且只在生成的数据集上做了实验. 但是实际效果来看, 在真实图像上的效果的确很不错.

#### SRNTT ★
**[Paper]**  (CVPR 2019) Image Super-Resolution by Neural Texture Transfer <Br>
**[Author]** [Zhifei Zhang](http://web.eecs.utk.edu/~zzhang61/), [Zhaowen Wang](https://research.adobe.com/person/zhaowen-wang/), [Zhe Lin](https://research.adobe.com/person/zhe-lin/), [Hairong Qi](http://web.eecs.utk.edu/~hqi/) <Br>
**[[Project](https://zzutk.github.io/SRNTT-Project-Page/)]** **[[TF-Code](https://github.com/ZZUTK/SRNTT)]** <Br>
(**借助参考图的超分**) 选出参考图中与当前patch最相近的patch, 再与LR一起处理
	
#### KernelGAN ★★
**[Paper]**  (NIPS 2019 Oral) Blind Super-Resolution Kernel Estimation using an Internal-GAN <Br>
**[Author]** Sefi Bell-Kligler, [Assaf Shocher](http://www.wisdom.weizmann.ac.il/~/assafsho/), [Michal Irani](https://www.weizmann.ac.il/math/irani/) <Br>
**[[Project](http://www.wisdom.weizmann.ac.il/~vision/kernelgan/)]** **[[Pytorch-Code](https://github.com/sefibk/KernelGAN)]**  <Br>
无监督预测降质核并进行超分的方法. 使用若干个现象卷积层的GAN预测降质kernel, 训练的的GAN可以合成一个kernel, 作为该图形的降质核, 网络训练采用LSGAN和若干正则项构成. 预测的模糊核作为ZSSR的降质核, 再无监督地预测超分结果

	
#### ESRGAN
**[Paper]**  (ECCV 2018 workshop) Enhanced Super-Resolution Generative Adversarial Networks <Br>
**[Author]** Xintao Wang, [Ke Yu](https://yuke93.github.io/), Shixiang Wu, [Jinjin Gu](https://www.jasongt.com/), Yihao Liu, Chao Dong, [Yu Qiao](http://mmlab.siat.ac.cn/yuqiao/), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[[Pytorch-Code](https://github.com/xinntao/ESRGAN)]**  <Br>
	
#### *Super-resolution using a GAN to degradate* ★★
**[Paper]**  (ECCV 2018) To learn image super-resolution, use a GAN to learn how to do image degradation first <Br>
**[Author]** [Adrian Bulat](https://www.adrianbulat.com/), [Jing Yang](https://jingyang2017.github.io/), [Georgios Tzimiropoulos](http://www.cs.nott.ac.uk/~pszyt/) <Br>
**[[Pytorch-Code](https://github.com/jingyang2017/Face-and-Image-super-resolution)]**  <Br>
(**使用GAN的无监督学习降质**)
	
#### CARN ★☆
**[Paper]**  (ECCV 2018) Fast, Accurate, and Lightweight Super-Resolution with Cascading Residual Network <Br>
**[Author]** [Namhyuk Ahn](https://nmhkahn.github.io/), Byungkon Kang, [Kyung-Ah Sohn](https://sites.google.com/site/kasohn/home) <Br>
**[[Pytorch-Code](https://github.com/nmhkahn/CARN-pytorch)]**  <Br>
(**轻量级超分**) 在block内部使用group conv和skip connection, 使用全局和局部的跳连. 在低分辨率上处理, 用PixelShuffle上采样.

#### RCAN ★☆
**[Paper]**  (ECCV 2018) Image Super-Resolution Using Very Deep Residual Channel Attention Networks <Br>
**[Author]** [Yulun Zhang](http://yulunzhang.com/), [Kunpeng Li](https://kunpengli1994.github.io/), [Kai Li](http://kailigo.github.io/), [Lichen Wang](https://sites.google.com/site/lichenwang123/), [Bineng Zhong](https://scholar.google.de/citations?user=hvRBydsAAAAJ&hl=en), [Yun Fu](http://www1.ece.neu.edu/~yunfu/)  <Br>
**[[Pytorch-Code](https://github.com/yulunzhang/RCAN)]**  <Br>
residual + 通道attention
	
#### ZSSR ★☆
**[Paper]**  (CVPR 2018) "Zero Shot" Super-Resolution using Deep Internal Learning <Br>
**[Author]** [Assaf Shocher](http://www.wisdom.weizmann.ac.il/~/assafsho/), [Nadav Cohen](http://www.cohennadav.com/), [Michal Irani](https://www.weizmann.ac.il/math/irani/) <Br>
**[[Project](http://www.wisdom.weizmann.ac.il/~vision/zssr/)]** **[[Pytorch-Code](https://github.com/assafshocher/ZSSR)]**  <Br>
DL Zero shot超分较早的一篇, 使用LR内部patch将采样后作为训练输入, 对应的LR patch作为输出, 训练网络. 网络收敛后用来预测LR图像的超分结果.
 
#### DBPN ★★
**[Paper]**  (CVPR 2018) Deep Back-Projection Networks For Super-Resolution <Br>
**[Author]** [Muhammad Haris](https://alterzero.github.io/), [Greg Shakhnarovich](https://ttic.uchicago.edu/~gregory/), [Norimichi Ukita](https://www.toyota-ti.ac.jp/Lab/Denshi/iim/ukita/) <Br>
**[[Project](https://alterzero.github.io/projects/DBPN.html)]**  <Br>
提出在神经网络中引入back-projection思想, 引入HR到LR的反馈信息. 这个思路或许可以用在其他形式的网络中, 替代加或乘的特征融合方式.
	
#### SFTGAN ★★
**[Paper]**  (CVPR 2018) Recovering Realistic Texture in Image Super-resolution by Deep Spatial Feature Transform <Br>
**[Author]** Xintao Wang, [Ke Yu](https://yuke93.github.io/), Chao Dong, [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[[Pytorch-Code](https://github.com/xinntao/SFTGAN)]**  <Br>
**(结合语义的超分)** 从分割图中提取特征作为超分网络feature的scale和shift
	
#### RDN ★☆
**[Paper]**  (CVPR 2018) Residual Dense Network for Image Super-Resolution <Br>
**[Author]** [Yulun Zhang](http://yulunzhang.com/), [Yapeng Tian](http://yapengtian.org/), [Yu Kong](http://www1.ece.neu.edu/~yukong/), [Bineng Zhong](https://scholar.google.de/citations?user=hvRBydsAAAAJ&hl=en), [Yun Fu](http://www1.ece.neu.edu/~yunfu/)  <Br>
**[[Pytorch-Code](https://github.com/lizhengwei1992/ResidualDenseNetwork-Pytorch)]**  <Br>
提出Residual Dense Block(RDB)

#### SRGAN
**[Paper]**  (CVPR 2017) Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network<Br>
**[Author]** [Christian Ledig](http://www.christianledig.com/), [Lucas Theis](http://theis.io/), [Ferenc Huszar](https://www.inference.vc/about/), Jose Caballero, Andrew Cunningham, Alejandro Acosta, Andrew Aitken, [Alykhan Tejani](http://alykhantejani.github.io/), Johannes Totz, Zehan Wang, Wenzhe Shi <Br>
**[[TF-Code](https://github.com/brade31919/SRGAN-tensorflow)]**  <Br>

#### FSRCNN  ★☆
**[Paper]**  (ECCV 2016) Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network <Br>
**[Author]** Chao Dong, [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/), [Xiaoou Tang](https://www.ie.cuhk.edu.hk/people/xotang.shtml) <Br>
**[[Project](http://mmlab.ie.cuhk.edu.hk/projects/FSRCNN.html)]**  <Br>
SRCNN的加速版本, 在小分辨率上处理，用deconv升分辨率.
	

  

# Datasets
[DIV2k](https://data.vision.ee.ethz.ch/cvl/DIV2K/)  <Br>


# Resources
[[超分论文整理1](https://github.com/ChaofWang/Awesome-Super-Resolution)]

[[图像/视频超分论文整理2](https://github.com/HymEric/latest-development-of-ISR-VSR)]

[[图像/视频超分方法TF复现](https://github.com/LoSealL/VideoSuperResolution)]
