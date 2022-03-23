
# Table of Contents
  - [HDR](#hdr)
    - [Multi-Frame HDR](#multi-frame-hdr)
    - [Single-Frame HDR](#single-frame-hdr)
    - [Video HDR](#video-hdr)
  - [Tone Mapping](#tone-mapping)
  - [Datasets](#datasets)

    
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
	
#### NHDRRNet
**[Paper]** (TIP 2020) Deep HDR Imaging via A Non-Local Network ★ <Br>
**[Author]** [Qingsen Yan](https://qingsenyangit.github.io/), Lei Zhang, [Yu Liu](https://sites.google.com/site/yuliuunilau/home), Yu Zhu, Jinqiu Sun, [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), Yanning Zhang <Br>
**[[Keras-Code](https://github.com/tuvovan/NHDRRNet)]**<Br>
UNet + non-local + 并行不同kernel的卷积分支

#### AHDRNet ★★
**[Paper]** (CVPR 2019) Attention-guided Network for Ghost-free High Dynamic Range Imaging <Br>
**[Author]** [Qingsen Yan](https://qingsenyangit.github.io/), [Dong Gong](https://donggong1.github.io/), [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), [Anton van den Hengel](https://cs.adelaide.edu.au/~hengel/), [Chunhua Shen](https://cshen.github.io/), [Ian Reid](https://cs.adelaide.edu.au/~ianr/), Yanning Zhang <Br>
**[[Project](https://qingsenyangit.github.io/project/ahdr/)]** **[[Pytorch-Code](https://github.com/qingsenyangit/AHDRNet)]**<Br>
**多帧HDR**.基于空间attention的多帧HDR, 网络使用dilated residual dense blocks, 预测残差, loss使用μ-law压缩的L1 loss. 结构简洁, 效果不错.

#### Multi-scale Dense Networks for Deep High Dynamic Range Imaging
**[Paper]** (WACV 2019) Multi-scale Dense Networks for Deep High Dynamic Range Imaging <Br>
**[Author]** [Qingsen Yan](https://qingsenyangit.github.io/), [Dong Gong](https://donggong1.github.io/), Pingping Zhang, [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), Jinqiu Sun, [Ian Reid](https://cs.adelaide.edu.au/~ianr/), Yanning Zhang <Br>

#### Deep Multi-Stage Learning for HDR With Large Object Motions ☆
**[Paper]** (ICCP 2019) Deep Multi-Stage Learning for HDR With Large Object Motions <Br>
**[Author]** Green Rosh K S, Anmol Biswas Mandakinee, Singh Patel, B H Pawan Prasad<Br>

#### DeepHDR
**[Paper]** (ECCV 2018) Deep High Dynamic Range Imaging with Laxingrge Foreground Motions <Br>
**[Author]** [Shangzhe Wu](https://elliottwu.com/), [Jiarui Xu](https://jerryxu.net/), [Yu-Wing Tai](https://www.cse.ust.hk/admin/people/faculty/profile/yuwing), Chi-Keung Tang <Br>
**[[Project](https://elliottwu.com/projects/hdr/)]** **[[TF-Code](https://github.com/elliottwu/DeepHDR)]**<Br>
	
#### Deep High Dynamic Range Imaging of Dynamic Scenes ★☆
**[Paper]** (Siggraph 2017) Deep High Dynamic Range Imaging of Dynamic Scenes <Br>
**[Author]** [Nima Khademi Kalantari](https://people.engr.tamu.edu/nimak/index.html), [Ravi Ramamoorthi](https://cseweb.ucsd.edu//~ravir/) <Br>
**[[Project](https://cseweb.ucsd.edu//~viscomp/projects/SIG17HDR/)]** <Br>
较早使用CNN做多帧HDR的一篇论文, 提出了Kalantari数据集



### Traditional Methods
####  Noise-Optimal Capture
**[Paper]** (CVPR 2010) Noise-Optimal Capture for High Dynamic Range Photography ★☆ <Br>
**[Author]** [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Frédo Durand](http://people.csail.mit.edu/fredo/), [William T. Freeman](http://billf.mit.edu/)  <Br>
**[[Project](http://people.csail.mit.edu/hasinoff/hdrnoise/)]** <Br>
从成像的物理过程出发, 推导出最大化SNR下限和最短拍摄时间的拍摄参数设置. 文中对噪声建模和ISO与SNR关系的论述比较清晰, 值得学习.

#### Recovering High Dynamic Range Radiance Maps from Photographs
**[Paper]** (TOG 2008) Recovering High Dynamic Range Radiance Maps from Photographs <Br>
**[Author]** [Paul Debevec](http://www.pauldebevec.com/), [Jitendra Malik](https://people.eecs.berkeley.edu/~malik/)<Br>
**[[Project](http://www.pauldebevec.com/Research/HDR/)]** <Br>

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



## Single-Frame HDR
### DL Methods
#### HDRUNet ★
**[Paper]** (CVPRW 2021) HDRUNet: Single Image HDR Reconstruction with Denoising and Dequantization <Br>
**[Author]** Xiangyu Chen, Yihao Liu, Zhengwen Zhang, [Yu Qiao](http://mmlab.siat.ac.cn/), [Chao Dong](http://xpixel.group/) <Br>
**[[Pytorch-Code](https://github.com/chxy95/HDRUNet)]**<Br>
**单帧HDR**.base网络为UNet, 还有一个weight net和一个由SFT组成的condition net. loss用tanh L1.

#### End-to-End Differentiable Learning to HDR Image Synthesis for Multi-exposure Images
**[Paper]** (AAAI 2021) End-to-End Differentiable Learning to HDR Image Synthesis for Multi-exposure Images <Br>
**[Author]** Jung Hee Kim, Siyeong Lee, [Suk-Ju Kang](http://vds.sogang.ac.kr/) <Br>

#### Single-Image HDR Reconstruction by Learning to Reverse the Camera Pipeline ★
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

#### FHDR
**[Paper]** (Global SIP 2019) FHDR: HDR Image Reconstruction from a SingleLDR Image using Feedback Network <Br>
**[Author]** Zeeshan Khan, Mukul Khanna, Shanmuganathan Raman  <Br>
**[[Pytorch-Code](https://github.com/mukulkhanna/fhdr)]**<Br>

#### ExpandNet
**[Paper]** (EG 2018) ExpandNet: A Deep Convolutional Neural Network for High Dynamic Range Expansion from Low Dynamic Range Content <Br>
**[Author]** 	Demetris Marnerides, [Thomas Bashford-Rogers](http://thomasbashfordrogers.com/), [Jonathan Hatchett](https://hatchett.co.uk/), [Kurt Debattista](https://warwick.ac.uk/fac/sci/wmg/people/profile/?wmgid=518)  <Br>
**[[Pytorch-Code](https://github.com/dmarnerides/hdr-expandnet)]** **[[Unofficial-TF-Code](https://github.com/echolijinghui/ExpandNet)]**<Br>

#### Image Correction via Deep Reciprocating HDR Transformation
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
**[[Project](http://hdrv.org/hdrcnn/)]** **[[TF-Code](https://github.com/gabrieleilertsen/hdrcnn)]** <Br>
**单帧HDR**. 粗读, 较早将CNN用于HDR的一篇paper, 网络结构比较老, 但提出了两个可能有趣的点: 1) 将输入转换到log域训练更符合人眼视觉特性; 2) 高光部分采用输入和输出线性加权的方式, 修复过曝光, 并避免形成带状伪影. <Br>

#### DrTMO
**[Paper]** (Siggraph Asia 2017) Deep Reverse Tone Mapping <Br>
**[Author]** [Yuki Endo](http://www.npal.cs.tsukuba.ac.jp/~endo/index_en.html), [Yoshihiro Kanamori](http://kanamori.cs.tsukuba.ac.jp/index.html), [Jun Mitani](http://mitani.cs.tsukuba.ac.jp/en/)  <Br>
**[[Project](http://www.npal.cs.tsukuba.ac.jp/~endo/projects/DrTMO/)]** **[[Unofficial-Pytorch-Code](https://github.com/shleecs/DrTMO_unofficial_pytorch)]**<Br>
	

## Video HDR
#### DeepHDRVideo ★
**[Paper]** (ICCV 2021) HDR Video Reconstruction: A Coarse-to-fine Network and A Real-world Benchmark Dataset <Br>
**[Author]** [Guanying Chen](https://guanyingc.github.io/), [Chaofeng Chen](http://chaofengc.github.io/), [Shi Guo](https://scholar.google.com/citations?user=5hsEmuQAAAAJ&hl=en), [Zhetong Liang](https://scholar.google.com/citations?user=fCnuU9YAAAAJ&hl=en), [Kwan-Yee K. Wong](http://i.cs.hku.hk/~kykwong/), [Lei Zhang](https://www4.comp.polyu.edu.hk/~cslzhang/)  <Br>
**[[Project](https://guanyingc.github.io/DeepHDRVideo/)]** **[[Pytorch-Code](https://github.com/guanyingc/DeepHDRVideo)]**  <Br>
给定5张不同EV值的视频帧, 采用coarse to fine的方式生成hdr图像.

#### Deep HDR Video from Sequences with Alternating Exposures ★
**[Paper]** (Eurographics 2019) Deep HDR Video from Sequences with Alternating Exposures <Br>
**[Author]** [Nima Khademi Kalantari](https://people.engr.tamu.edu/nimak/index.html), [Ravi Ramamoorthi](https://cseweb.ucsd.edu/~ravir/)  <Br>
光流对齐加融合, 提出了一个从HDR视频生成样本的流程可以研究下


	
# Tone Mapping
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





# Datasets
[Kalantari Dataset](https://cseweb.ucsd.edu/~viscomp/projects/SIG17HDR/)
	
[Jan Fröhlich](https://www.hdm-stuttgart.de/vmlab/hdm-hdr-2014/)
	
[Sumsung Synthetic](https://github.com/nadir-zeeshan/sensor-realistic-synthetic-data)

