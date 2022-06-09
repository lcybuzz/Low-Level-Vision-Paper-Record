
# Table of Contents
  - [HDR](#hdr)
    - [Multi-Frame HDR](#multi-frame-hdr)
    - [Single-Frame HDR](#single-frame-hdr)
    - [Video HDR](#video-hdr)
    - [New Sensor HDR](#new-sensor-hdr)
  - [Tone Mapping](#tone-mapping)
  - [CRF](#crf)
  - [Datasets](#datasets)
  - [Resources](#resources)

    
# HDR
## Multi-Frame HDR
### DL Methods
#### FlexHDR ★
**[Paper]** (arXiv 2201) FlexHDR: Modelling Alignment and Exposure Uncertainties for Flexible HDR Imaging <Br>
**[Author]** [Sibi Catley-Chandar](https://sib1.github.io/), [Thomas Tanay](https://thomas-tanay.github.io/about/), Lucas Vandroux, [Aleš Leonardis](https://www.cs.bham.ac.uk/~leonarda/), [Gregory Slabaugh](http://eecs.qmul.ac.uk/profiles/slabaughgreg.html), [Eduardo Pérez-Pellitero](https://perezpellitero.github.io/) <Br>
对输入的每一张LDR, 根据亮度和光流准确度预测map, 并用它们预测spatial attention map. 每张LDR的分支通过feature的max pooling操作交换信息.
	
#### ADNet ★
**[Paper]** (CVPR 2021) ADNet: Attention-guided Deformable Convolutional Network for High Dynamic Range Imaging <Br>
**[Author]** Zhen Liu, Wenjie Lin, Xinpeng Li, Qing Rao, Ting Jiang, Mingyan Han, Haoqiang Fan, [Jian Sun](http://www.jiansun.org/), [Shuaicheng Liu](http://www.liushuaicheng.org/) <Br>
**[[Pytorch-Code](https://github.com/liuzhen03/ADNet)]**<Br>
spatial attention + deformable conv

#### HDR-GAN ★
**[Paper]** (TIP 2021) HDR-GAN: HDR Image Reconstruction from Multi-Exposed LDR Images with Large Motions <Br>
**[Author]** Yuzhen Niu, Jianbin Wu, Wenxi Liu, Wenzhong Guo, Rynson W.H. Lau <Br>
**[[TF-Code](https://github.com/nonu116/HDR-GAN)]**<Br>
多尺度网络 + GAN

#### CF-Net ★
**[Paper]** (TIP 2021) Deep Coupled Feedback Network for Joint Exposure Fusion and Image Super-Resolution <Br>
**[Author]** Xin Deng, Yutong Zhang, Mai Xu, [Shuhang Gu](https://shuhanggu.github.io/), Yiping Duan <Br>
**[[Pytorch-Code](https://github.com/ytZhang99/CF-Net)]**<Br>
2张图像曝光融合+超分, 分成两支, 在处理中引入对方信息.
	
#### GCHDRNet ★☆
**[Paper]** (Neurocomputing 2021) Towards Accurate HDR Imaging with Learning Generator Constraints <Br>
**[Author]** [Qingsen Yan](https://qingsenyangit.github.io/), Bo Wang, [Lei Zhang](https://sites.google.com/site/leizhanghyperspectral/home), Jingyu Zhang, Zheng You, [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), Yanning Zhang <Br>
提出用3个LDR subnetwork将生成的HDR变换为LDR, 并对3个LDR计算loss, 目的是使网络更关注于有distortion的区域. 可以尝试下该思路.
	
#### NHDRRNet ★
**[Paper]** (TIP 2020) Deep HDR Imaging via A Non-Local Network  <Br>
**[Author]** [Qingsen Yan](https://qingsenyangit.github.io/), [Lei Zhang](https://sites.google.com/site/leizhanghyperspectral/home), [Yu Liu](https://sites.google.com/site/yuliuunilau/home), Yu Zhu, Jinqiu Sun, [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), Yanning Zhang <Br>
**[[Keras-Code](https://github.com/tuvovan/NHDRRNet)]**<Br>
UNet + non-local + 并行不同kernel的卷积分支

#### MEFNet ★
**[Paper]** (TIP 2020) Deep Guided Learning for Fast Multi-Exposure Image Fusion <Br>
**[Author]** [Kede Ma](https://kedema.org/), [Zhengfang Duanmu](https://ece.uwaterloo.ca/~zduanmu/), Hanwei Zhu, [Yuming Fang](http://sim.jxufe.cn/JDMKL/ymfang.html), [Zhou Wang](https://ece.uwaterloo.ca/~z70wang/) <Br>
**[[Pytorch-Code](https://github.com/makedede/MEFNet)]**<Br>
**无监督MEF**
	
#### Towards Practical and Efficient High-Resolution HDR Deghosting with CNN ★★
**[Paper]** (ECCV 2020) Towards Practical and Efficient High-Resolution HDR Deghosting with CNN <Br>
**[Author]** [K Ram Prabhakar](https://sites.google.com/view/kramprabhakar/), S Agrawal, [D K Singh](https://durgesh93.github.io/), B Ashwath, [R. V. Babu](http://cds.iisc.ac.in/faculty/venky/) <Br>
将计算量大的光流对齐和融合网络部分在小图处理, 用BGU上采用, BGU所需的guided map通过对三帧的加权求和得到, weight通过小图预测并上采样得到. 距离实际移动端落地还有距离, 不过思路比较新奇.

#### LSD2 ★
**[Paper]** (BMVC 2020) LSD_2 - Joint denoising and deblurring of short and long exposure images with CNNs <Br>
**[Author]** Janne Mustaniemi, [Juho Kannala](https://users.aalto.fi/~kannalj1/), [Jiri Matas](https://cmp.felk.cvut.cz/~matas/), [Simo Särkkä](https://users.aalto.fi/~ssarkka/), Janne Heikkilä <Br>
**[[Keras-Code](https://github.com/jannemus/LSD2)]**<Br>
short/long曝光融合, 用一个UNet同时实现denoise和deblur. 从RGB图像中通过模拟过曝, blur, 加噪等生成short/long数据.

#### Ganfuse ★
**[Paper]** (NCA 2020) Ganfuse: a novel multi-exposure image fusion method based on generative adversarial networks <Br>
**[Author]** Zhiguang Yang, Youping Chen, Zhuliang Le, Yong Ma  <Br>
提出了GAN loss及gradient loss, 非监督MEF
	
#### AHDRNet ★★
**[Paper]** (CVPR 2019) Attention-guided Network for Ghost-free High Dynamic Range Imaging <Br>
**[Author]** [Qingsen Yan](https://qingsenyangit.github.io/), [Dong Gong](https://donggong1.github.io/), [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), [Anton van den Hengel](https://cs.adelaide.edu.au/~hengel/), [Chunhua Shen](https://cshen.github.io/), [Ian Reid](https://cs.adelaide.edu.au/~ianr/), Yanning Zhang <Br>
**[[Project](https://qingsenyangit.github.io/project/ahdr/)]** **[[Pytorch-Code](https://github.com/qingsenyangit/AHDRNet)]**<Br>
**多帧HDR**.基于空间attention的多帧HDR, 网络使用dilated residual dense blocks, 预测残差, loss使用μ-law压缩的L1 loss. 结构简洁, 效果不错.

#### Multi-scale Dense UNet for HDR ★
**[Paper]** (WACV 2019) Multi-scale Dense Networks for Deep High Dynamic Range Imaging <Br>
**[Author]** [Qingsen Yan](https://qingsenyangit.github.io/), [Dong Gong](https://donggong1.github.io/), Pingping Zhang, [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), Jinqiu Sun, [Ian Reid](https://cs.adelaide.edu.au/~ianr/), Yanning Zhang <Br>

#### Deep Multi-Stage Learning for HDR With Large Object Motions ☆
**[Paper]** (ICCP 2019) Deep Multi-Stage Learning for HDR With Large Object Motions <Br>
**[Author]** Green Rosh K S, Anmol Biswas Mandakinee, Singh Patel, B H Pawan Prasad<Br>

#### Scalable Deghosting Exposure Fusion ★
**[Paper]** (ICCP 2019) A Fast, Scalable, and Reliable Deghosting Method for Extreme Exposure Fusion <Br>
**[Author]** [K Ram Prabhakar](https://sites.google.com/view/kramprabhakar/), Rajat Arora, Adhitya Swaminathan, Kunal Pratap Singh, [R. Venkatesh Babu](http://cds.iisc.ac.in/faculty/venky/) <Br>
**[[TF-Code](https://github.com/rajat95/Deep-Deghosting-HDR)]** <Br>
对任意个输入提特征并进行feature aggregation, 使网络能处理任意输入. 提出了一个HDR数据集

#### DeepHDR ★★
**[Paper]** (ECCV 2018) Deep High Dynamic Range Imaging with Large Foreground Motions <Br>
**[Author]** [Shangzhe Wu](https://elliottwu.com/), [Jiarui Xu](https://jerryxu.net/), [Yu-Wing Tai](https://www.cse.ust.hk/admin/people/faculty/profile/yuwing), Chi-Keung Tang <Br>
**[[Project](https://elliottwu.com/projects/hdr/)]** **[[TF-Code](https://github.com/elliottwu/DeepHDR)]**<Br>
3个encoder, 1个decoder, loss和预处理与'Deep High Dynamic Range Imaging of Dynamic Scenes'相似
	
#### Deep High Dynamic Range Imaging of Dynamic Scenes ★★★
**[Paper]** (TOG 2017) Deep High Dynamic Range Imaging of Dynamic Scenes <Br>
**[Author]** [Nima Khademi Kalantari](https://people.engr.tamu.edu/nimak/index.html), [Ravi Ramamoorthi](https://cseweb.ucsd.edu//~ravir/) <Br>
**[[Project](https://cseweb.ucsd.edu//~viscomp/projects/SIG17HDR/)]** <Br>
较早使用CNN做多帧HDR的一篇论文, 提出了Kalantari数据集, 其中的3张图像预处理流程, 算法整体思路, 以及使用mu-law计算loss等内容被之后很多论文借鉴

#### DeepFuse ★
**[Paper]** (ICCV 2017) DeepFuse:A Deep Unsupervised Approach for Exposure Fusion with Extreme Exposure Image Pairs <Br>
**[Author]** [K Ram Prabhakar](https://sites.google.com/view/kramprabhakar/home), V Sai Srikar, [R. Venkatesh Babu](http://cds.iisc.ac.in/faculty/venky/) <Br>
**[[Theano-Code](https://github.com/KRamPrabhakar/DeepFuse)]** **[[Unofficial-Pytorch-Code](https://github.com/SunnerLi/DeepFuse.pytorch)]**<Br>


### Traditional Methods
####  Noise-Optimal Capture ★★☆
**[Paper]** (CVPR 2010) Noise-Optimal Capture for High Dynamic Range Photography  <Br>
**[Author]** [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Frédo Durand](http://people.csail.mit.edu/fredo/), [William T. Freeman](http://billf.mit.edu/)  <Br>
**[[Project](http://people.csail.mit.edu/hasinoff/hdrnoise/)]** <Br>
从成像的物理过程出发, 推导出最大化SNR下限和最短拍摄时间的拍摄参数设置. 文中对噪声建模和ISO与SNR关系的论述比较清晰, 值得学习. 没有考虑多帧间的motion.

#### Fusing Multiple Raw Images and Tone Reproduction ★☆
**[Paper]** (TCE 2008) High Dynamic Range Imaging by Fusing Multiple Raw Images and Tone Reproduction <Br>
**[Author]** [Wen-Chung Kao](https://scholar.lib.ntnu.edu.tw/en/persons/wen-chung-kao) <Br>
提出了一个针对静止场景的多张raw融合并tone mapping的pipeline, 可以学习
	
#### Exposure Fusion
**[Paper]** (PG 2007) Exposure Fusion <Br>
**[Author]** [Tom Mertens](http://www.mericam.net/), [Jan Kautz](https://jankautz.com/), Frank Van Reeth<Br>

#### High Dynamic Range Video ★★
**[Paper]** (TOG 2003) High Dynamic Range Video <Br>
**[Author]** [Sing Bing Kang](http://www.singbingkang.com/), [Matthew Uyttendaele](https://research.facebook.com/people/uyttendaele-matt/), [Simon Winder](http://simonwinder.com/), [Richard Szeliski](http://szeliski.org/RichardSzeliski.htm)  <Br>
提出了一个视频HDR pipeline. 1.根据场景亮度, 设置相邻帧的曝光值; 2.将相邻帧处理到相同亮度, 做运动检测和warping. 对于当前帧saturate的部分, 使用前后两帧之间的光流估计到当前帧的光流并做warp, 没有saturate的部分, 利用前后帧到当前帧的光流直接warp, 并用一些策略fuse; 3.将HDR的radiance map通过tone mapping转换为能显示的LDR视频, 使用前后若干帧统计平均log域亮度, 做全局scale, 局部只根据当前帧scale
	
#### High Dynamic Range Imaging ★
**[Paper]** (CIC 2001) High Dynamic Range Imaging <Br>
**[Author]** Greg Ward  <Br>
讲了color rendering的pipeline, 包括: 怎么估计真实场景目标的光强, 转换到颜色空间的近似表示, 将信息记录为HDR格式, tone mapping以在设备上显示等
	
#### SVE ★
**[Paper]** (CVPR 2000) High Dynamic Range Imaging: Spatially Varying Pixel Exposures <Br>
**[Author]** [Shree K. Nayar](http://www.cs.columbia.edu/~nayar/), Tomoo Mitsunaga  <Br>
提出一个基于硬件的HDR图像生成方法. 在相机传感器前放置一个optical mask, mask上有不同exposure的pattern, 利用邻域不同曝光的像素值, 恢复目标像素值, 动态范围可大致扩展到Emax/Emin倍.
 
#### Recovering High Dynamic Range Radiance Maps from Photographs ★★★
**[Paper]** (SIGGRAPH 97) Recovering High Dynamic Range Radiance Maps from Photographs <Br>
**[Author]** [Paul Debevec](http://www.pauldebevec.com/), [Jitendra Malik](https://people.eecs.berkeley.edu/~malik/)<Br>
**[[Project](http://www.pauldebevec.com/Research/HDR/)]** <Br>
经典的多曝光HDR算法, 不考虑motion, 主要包括通过最优化求CRF和融合生成HDR两部分.
	

## Single-Frame HDR
### DL Methods
#### HDRUNet ★
**[Paper]** (CVPRW 2021) HDRUNet: Single Image HDR Reconstruction with Denoising and Dequantization <Br>
**[Author]** Xiangyu Chen, Yihao Liu, Zhengwen Zhang, [Yu Qiao](http://mmlab.siat.ac.cn/), [Chao Dong](http://xpixel.group/) <Br>
**[[Pytorch-Code](https://github.com/chxy95/HDRUNet)]**<Br>
**单帧HDR**.base网络为UNet, 还有一个weight net和一个由SFT组成的condition net. loss用tanh L1.

#### DiffHDRsyn
**[Paper]** (AAAI 2021) End-to-End Differentiable Learning to HDR Image Synthesis for Multi-exposure Images <Br>
**[Author]** Jung Hee Kim, Siyeong Lee, [Suk-Ju Kang](http://vds.sogang.ac.kr/) <Br>
**[[Pytorch-Code](https://github.com/JungHeeKim29/DiffHDRsyn)]**
	
#### HDR by Learning to Reverse the Camera Pipeline ★★
**[Paper]** (CVPR 2020) Single-Image HDR Reconstruction by Learning to Reverse the Camera Pipeline <Br>
**[Author]** [Yu-Lun Liu](http://www.cmlab.csie.ntu.edu.tw/~yulunliu/), [Wei-Sheng Lai](https://www.wslai.net/), [Yu-Sheng Chen](https://www.cmlab.csie.ntu.edu.tw/~nothinglo/), Yi-Lung Kao, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/) <Br>
**[[Project](https://www.cmlab.csie.ntu.edu.tw/~yulunliu/SingleHDR)]** **[[TF-Code](https://github.com/alex04072000/SingleHDR)]**<Br>
**单帧HDR**.用几个CNN模拟ISP中HDR到LDR的映射过程, 完成HDR. 关键是定义每个部分的训练目标和数据, 这部分没细看.

#### UnModNet
**[Paper]** (NeruIPS 2020) UnModNet: Learning to Unwrap a Modulo Image for High Dynamic Range Imaging <Br>
**[Author]**  Chu Zhou, Hang Zhao, Jin Han, [Chang Xu](http://changxu.xyz/), Chao Xu, Tiejun Huang, [Boxin Shi](http://ci.idm.pku.edu.cn/Publication.htm) <Br>
**[[Project](https://www.cmlab.csie.ntu.edu.tw/~yulunliu/SingleHDR)]** **[[TF-Code](https://github.com/alex04072000/SingleHDR)]**<Br>

#### Deep-HdrReconstruction
**[Paper]** (SIGGRAPH 2020) Single Image HDR Reconstruction Using a CNN with Masked Features and Perceptual Loss <Br>
**[Author]** [Marcel Santana Santos](https://marcelsan.github.io/), Tsang Ing Ren, [Nima Khademi Kalantari](https://people.engr.tamu.edu/nimak/index.html)  <Br>
**[[Pytorch-Code](https://github.com/marcelsan/Deep-HdrReconstruction)]**<Br>

#### JSI-GAN ★
**[Paper]** (AAAI 2020) JSI-GAN: GAN-Based Joint Super-Resolution and Inverse Tone-Mapping with Pixel-Wise Task-Specific Filters for UHD HDR Video  <Br>
**[Author]** [Soo Ye Kim](https://sites.google.com/view/sooyekim), [Jihyong Oh](https://sites.google.com/view/ozbro/%ED%99%88), [Munchurl Kim](https://www.viclab.kaist.ac.kr/) <Br>
**[[TF-Code](https://github.com/JihyongOh/JSI-GAN)]**<Br>
adaptive conv, GAN loss

#### Learning to generate multi-exposure stacks with cycle consistency ★
**[Paper]** (TMM 2020) Learning to generate multi-exposure stacks with cycle consistency for high dynamic range imaging <Br>
**[Author]** Siyeong Lee, Gwon Hwan An, [Suk-Ju Kang](http://vds.sogang.ac.kr/)   <Br>
训练一个stop-up和一个stop-down网络, 可以对任意ev的输入改变其亮度. 反复运行两个网络, 可以得到多个不同ev的图像, 用于生成HDR图像. 使用了cycle consitency loss.

#### Deep-SR-ITM ★
**[Paper]** (ICCV 2019) Deep sr-itm: Joint learning of super-resolution and inverse tone-mapping for 4k uhd hdr applications  <Br>
**[Author]** [Soo Ye Kim](https://sites.google.com/view/sooyekim), [Jihyong Oh](https://sites.google.com/view/ozbro/%ED%99%88), [Munchurl Kim](https://www.viclab.kaist.ac.kr/)  <Br>
**[[MatConvNet-Code](https://github.com/sooyekim/Deep-SR-ITM)]**<Br>
将输入分解为detail和base分别处理

#### iTM-Net ☆
**[Paper]** (Global SIP 2019) iTM-Net: Deep Inverse Tone Mapping Using Novel Loss Function Considering Tone Mapping Operator <Br>
**[Author]** [Yuma Kinoshita](https://sites.google.com/view/kinoshita-yuma-en/), [Hitoshi Kiya](http://www-isys.sd.tmu.ac.jp/members-2/kiya/)  <Br>
在非线性空间计算loss

#### FHDR
**[Paper]** (Global SIP 2019) FHDR: HDR Image Reconstruction from a SingleLDR Image using Feedback Network <Br>
**[Author]** Zeeshan Khan, Mukul Khanna, Shanmuganathan Raman  <Br>
**[[Pytorch-Code](https://github.com/mukulkhanna/fhdr)]**<Br>

#### Joint High Dynamic Range Imaging and Super-Resolution from a Single Image ★
**[Paper]** (IEEE Access 2019) Joint High Dynamic Range Imaging and Super-Resolution from a Single Image <Br>
**[Author]** Jae Woong Soh, Jae Sung Park, Nam Ik Cho  <Br>
**[[TF-Code](https://github.com/JWSoh/HDRI-SR)]**<Br>
Retinex分解辐illuminance和reflectance, 对反射分量用CNN处理

#### High Dynamic Range and Super-Resolution Imaging from a Single Image ★☆
**[Paper]** (IEEE Access 2018) High Dynamic Range and Super-Resolution Imaging from a Single Image <Br>
**[Author]** Jae Woong Soh, Jae Sung Park, Nam Ik Cho  <Br>
Retinex分解辐illuminance和reflectance, 对辐照度和反射分量分别处理. HDR部分有一些较经验话的设置, 可以参考
	
#### ExpandNet
**[Paper]** (EG 2018) ExpandNet: A Deep Convolutional Neural Network for High Dynamic Range Expansion from Low Dynamic Range Content <Br>
**[Author]** 	Demetris Marnerides, [Thomas Bashford-Rogers](http://thomasbashfordrogers.com/), [Jonathan Hatchett](https://hatchett.co.uk/), [Kurt Debattista](https://warwick.ac.uk/fac/sci/wmg/people/profile/?wmgid=518)  <Br>
**[[Pytorch-Code](https://github.com/dmarnerides/hdr-expandnet)]** **[[Unofficial-TF-Code](https://github.com/echolijinghui/ExpandNet)]**<Br>

#### DRHT
**[Paper]** (CVPR 2018) Image Correction via Deep Reciprocating HDR Transformation <Br>
**[Author]** [Xin Yang](http://faculty.dlut.edu.cn/yangxin/zh_CN/index.htm), Ke Xu, [Yibing Song](https://ybsong00.github.io/), Qiang Zhang, Xiaopeng Wei, [Rynson Lau](https://www.cs.cityu.edu.hk/~rynson/)  <Br>
**[[Project](https://ybsong00.github.io/cvpr18_imgcorrect/index.html)]** **[[TF-Code](https://github.com/ybsong00/DRHT)]**<Br>

#### Deep recursive hdri
**[Paper]** (ECCV 2018) Deep recursive hdri: Inverse tone mapping using generative adversarial networks <Br>
**[Author]** Siyeong Lee, Gwon Hwan An, Suk-Ju Kang  <Br>
**[[Pytorch-Code](https://github.com/Siyeong-Lee/Deep_Recursive_HDRI)]**<Br>

#### Deep Chain HDRI
**[Paper]** (Access 2018) Deep Chain HDRI: Reconstructing a High Dynamic Range Image from a Single Low Dynamic Range Image <Br>
**[Author]** Siyeong Lee, Gwon Hwan An, Suk-ju Kang  <Br>
**[[Project](https://siyeong-lee.github.io/hdr_vds_dataset/)]** <Br>

#### HDRCNN ★
**[Paper]** (Siggraph Asia 2017) HDR image reconstruction from a single exposure using deep CNNs <Br>
**[Author]** [Gabriel Eilertsen](http://vcl.itn.liu.se/members/gabriel-eilertsen), [Joel Kronander](http://vcl.itn.liu.se/members/joel-kronander), [Gyorgy Denes](https://www.cl.cam.ac.uk/~gd355/), [Rafał K. Mantiuk](https://www.cl.cam.ac.uk/~rkm38/), [Jonas Unger](http://webstaff.itn.liu.se/~jonun/web/Home.php) <Br>
**[[Project](https://weber.itn.liu.se/~gabei62/hdrcnn/)]** **[[TF-Code](https://github.com/gabrieleilertsen/hdrcnn)]** <Br>
**单帧HDR**. 粗读, 较早将CNN用于HDR的一篇paper, 网络结构比较老, 但提出了两个可能有趣的点: 1) 将输入转换到log域训练更符合人眼视觉特性; 2) 高光部分采用输入和输出线性加权的方式, 修复过曝光, 并避免形成带状伪影. <Br>

#### DrTMO
**[Paper]** (Siggraph Asia 2017) Deep Reverse Tone Mapping <Br>
**[Author]** [Yuki Endo](http://www.npal.cs.tsukuba.ac.jp/~endo/index_en.html), [Yoshihiro Kanamori](http://kanamori.cs.tsukuba.ac.jp/index.html), [Jun Mitani](http://mitani.cs.tsukuba.ac.jp/en/)  <Br>
**[[Project](http://www.npal.cs.tsukuba.ac.jp/~endo/projects/DrTMO/)]** **[[Unofficial-Pytorch-Code](https://github.com/shleecs/DrTMO_unofficial_pytorch)]**<Br>
	

## Video HDR
#### Video HDR with Tri-Exposure Quad-Bayer Sensors
**[Paper]** (arXiv 2103) HDR Video Reconstruction with Tri-Exposure Quad-Bayer Sensors<Br>
**[Author]** Yitong Jiang, [Inchang Choi](http://www.inchangchoi.info/), Jun Jiang, [Jinwei Gu](http://www.gujinwei.org/)  <Br>
	
#### DeepHDRVideo ★★
**[Paper]** (ICCV 2021) HDR Video Reconstruction: A Coarse-to-fine Network and A Real-world Benchmark Dataset <Br>
**[Author]** [Guanying Chen](https://guanyingc.github.io/), [Chaofeng Chen](http://chaofengc.github.io/), [Shi Guo](https://scholar.google.com/citations?user=5hsEmuQAAAAJ&hl=en), [Zhetong Liang](https://scholar.google.com/citations?user=fCnuU9YAAAAJ&hl=en), [Kwan-Yee K. Wong](http://i.cs.hku.hk/~kykwong/), [Lei Zhang](https://www4.comp.polyu.edu.hk/~cslzhang/)  <Br>
**[[Project](https://guanyingc.github.io/DeepHDRVideo/)]** **[[Pytorch-Code](https://github.com/guanyingc/DeepHDRVideo)]**  <Br>
给定5张不同EV值的视频帧, 采用coarse to fine的方式生成hdr图像, 网络较复杂. 另外提出了一个HDR数据集, 生成数据的方法可以借鉴.

#### Deep HDR Video from Sequences with Alternating Exposures ★
**[Paper]** (Eurographics 2019) Deep HDR Video from Sequences with Alternating Exposures <Br>
**[Author]** [Nima Khademi Kalantari](https://people.engr.tamu.edu/nimak/index.html), [Ravi Ramamoorthi](https://cseweb.ucsd.edu/~ravir/)  <Br>
光流对齐加融合, 提出了一个从HDR视频生成样本的流程可以研究下

	
## New Sensor HDR
#### HDR Video Reconstruction with Tri-Exposure Quad-Bayer Sensors  ★★
**[Paper]** (arXiv 2103) HDR Video Reconstruction with Tri-Exposure Quad-Bayer Sensors <Br>
**[Author]** Yitong Jiang, [Inchang Choi](http://www.inchangchoi.info/), Jun Jiang, [Jinwei Gu](http://www.gujinwei.org/) <Br>
**Tri-Exposure Quad-Bayer Sensor video HDR**. 提出了一个包括HDR fusion, 时域去噪, 超分三个模块的pipeline.
	
#### Hdr denoising and deblurring by learning spatio-temporal distortion models  ★★
**[Paper]** (arXiv 2012) Hdr denoising and deblurring by learning spatio-temporal distortion models  <Br>
**[Author]** Uğur Çoğalan, [Mojtaba Bemana](https://people.mpi-inf.mpg.de/~mbemana/), [Karol Myszkowski](https://people.mpi-inf.mpg.de/~karol/), [Hans-Peter Seidel](https://people.mpi-inf.mpg.de/~hpseidel/), [Tobias Ritschel](http://www.homepages.ucl.ac.uk/~ucactri/) <Br>
Dual-exposure HDR, 奇数列短曝光, 偶数列长曝光. 网络采用UNet. 提出了一个生成数据的流程.
	
#### Deep joint deinterlacing and denoising for single shot dual-iso hdr reconstruction ★★
**[Paper]** (TIP 2020) Deep joint deinterlacing and denoising for single shot dual-iso hdr reconstruction <Br>
**[Author]** Ugur Cogalan, [Ahmet Oguz Akyuz](https://user.ceng.metu.edu.tr/~akyuz/index.html)  <Br>
**[[Code & Dataset](https://user.ceng.metu.edu.tr/~akyuz/publications.html)]**<Br>	
Dual-ISO HDR. 两个网络分别处理low/high图像. 通过分析噪声, 提出了一个生成Dual-ISO数据集的方法

	
# Tone Mapping
## DL Methods
#### Unpaired Learning for High Dynamic Range Image Tone Mapping ★☆
**[Paper]** (ICCV 2021) Unpaired Learning for High Dynamic Range Image Tone Mapping  <Br>
**[Author]** Yael Vinker, Inbar Huberman-Spiegelglas, [Raanan Fattal](https://www.cs.huji.ac.il/w~raananf/) <Br>
基于GAN的无监督tone mapping, 使用LSGAN loss和patch相关系数loss, 输入做了自适应的log压缩预处理, 压缩参数通过最小化与自然LDR直方图交叉熵得到.
	
#### DeepTMO ★
**[Paper]** (TIP 2019) Deep Tone Mapping Operator for High Dynamic Range Images  <Br>
**[Author]** Aakanksha Rana, Praveer Singh, [Giuseppe Valenzise](https://l2s.centralesupelec.fr/u/valenzise-giuseppe/), [Frederic Dufaux](https://l2s.centralesupelec.fr/u/dufaux-frederic/), [Nikos Komodakis](https://www.csd.uoc.gr/~komod/), Aljosa Smolic <Br>
 **[[PYtorch-Code]([https://github.com/csjunxu/L1-L0-Tone-mapping](https://github.com/Aakanksha-Rana/DeepTMO))]** 	<Br>
较早用CNN做tone mapping的论文, 使用了two-scale结构, loss使用LSGAN loss, 判别器feature matching loss和vgg loss

## Traditional Methods

#### ℓ1-ℓ0 Layer Decomposition ★
**[Paper]** (CVPR 2018) A Hybrid ℓ1-ℓ0 Layer Decomposition Model for Tone Mapping  <Br>
**[Author]** Zhetong Liang, [Jun Xu](https://csjunxu.github.io/), [David Zhang](http://www4.comp.polyu.edu.hk/~csdzhang/), Zisheng Cao, [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
 **[[Code](https://github.com/csjunxu/L1-L0-Tone-mapping)]** 	<Br>
l1约束base layer, l0约束detail layer
	
#### Photographic tone reproduction for digital images ★★
**[Paper]** (TOG 2002) Photographic tone reproduction for digital images  <Br>
**[Author]** [Erik Reinhard](http://erikreinhard.com/), Michael Stark, [Peter Shirley](https://www.petershirley.com/), [James Ferwerda](https://jamesferwerda.com/) <Br>
1. 在log域计算平均照度, 并用其对全图进行scale; 2. 自适应dodging-and-burning, 实现局部tone mapping

	
# CRF
## DL Methods
#### CRF-net ★★
**[Paper]** (CVMP 2017) CRF-net: Single Image Radiometric Calibration using CNNs  <Br>
**[Author]** Han Li, [Pieter Peers](https://www.cs.wm.edu/~ppeers/) <Br>
较少的用DL做CRF预测的paper, 效果有限, 但思路被一些方法借鉴, 如"HDR by Learning to Reverse the Camera Pipeline"
	
## Traditional Methods



# Datasets
[Kalantari Dataset](https://cseweb.ucsd.edu/~viscomp/projects/SIG17HDR/)
	
[Jan Fröhlich](https://www.hdm-stuttgart.de/vmlab/hdm-hdr-2014/)
	
[Sumsung Synthetic](https://github.com/nadir-zeeshan/sensor-realistic-synthetic-data)


# Resources
[HDR Deghosting Paper List](https://github.com/JimmyChame/The-State-of-the-Art-in-HDR-Deghosting)

[HDR Toolbox (Matlab/Octave)](https://github.com/banterle/HDR_Toolbox)
