
# Table of Contents
  - [HDR](#hdr)
    - [Multi-Frame HDR](#multi-frame-hdr)
    - [Single-Frame HDR](#single-frame-hdr)
    - [Video HDR](#video-hdr)
    - [New Sensor HDR](#new-sensor-hdr)
    - [Traditional Methods](#traditional-methods)
  - [Tone Mapping](#tone-mapping)
  - [CRF](#crf)
  - [Datasets](#datasets)
  - [Resources](#resources)

    
# HDR
## Multi-Frame HDR
- **Inverting the Imaging Process by Learning an Implicit Camera Model** <Br>
[Xin Huang](https://xhuangcv.github.io/), [Qi Zhang](https://qzhang-cv.github.io/), Ying Feng, [Hongdong Li](https://users.cecs.anu.edu.au/~hongdong/), [Qing Wang](https://teacher.nwpu.edu.cn/qwang.html) <Br>
[CVPR 2023] [[Pytorch-Code](https://github.com/xhuangcv/neucam)] <Br>

- **Joint HDR Denoising and Fusion: A Real-World Mobile HDR Image Dataset** <Br>
Shuaizheng Liu, Xindong Zhang, Lingchen Sun, Zhetong Liang, [Hui Zeng](https://huizeng.github.io/), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
[CVPR 2023] [[Code](https://github.com/shuaizhengliu/Joint-HDRDN)] <Br>
[oppo]

- **TransMEF: A Transformer-Based Multi-Exposure Image Fusion Framework via Self-Supervised Multi-Task Learning** <Br>
[Linhao Qu])https://linhao-qu.github.io/, Shaolei Liu, Manning Wang, Zhijian Song <Br>
[AAAI 2022] [[Pytorch-Code](https://github.com/miccaiif/TransMEF)] <Br>

- **Gamma-Enhanced Spatial Attention Network for Efficient High Dynamic Range Imaging** <Br>
Zhen Liu, Yinglong Wang, Bing Zeng, [Shuaicheng Liu](http://www.liushuaicheng.org/) <Br>
[ECCV 2022] [[Pytorch-Code](https://github.com/megvii-research/HDR-Transformer)] <Br>

- **DRHDR: A Dual Branch Residual Network for Multi-Bracket High Dynamic Range Imaging** <Br>
Juan Marín-Vega, Michael Sloth, Peter Schneider-Kamp, Richard Röttger <Br>
[CVPRW 2022] <Br>
[★] NTIRE22

- **Gamma-Enhanced Spatial Attention Network for Efficient High Dynamic Range Imaging** <Br>
Fangya Li, Ruipeng Gang, Chenghua Li, Jinjing Li, Sai Ma, Chenming Liu, Yizhen Cao <Br>
[CVPRW 2022] <Br>
[★] NTIRE22

- **A Lightweight Network for High Dynamic Range Imaging** <Br>
[Qingsen Yan](https://qingsenyangit.github.io/), Song Zhang, Weiye Chen, Yuhang Liu, Zhen Zhang, Yanning Zhang, [Javen Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), [Dong Gong](https://donggong1.github.io/) <Br>
[CVPRW 2022] <Br>
[★☆] NTIRE22. Spatial attention + dual attention提取特征. Encoder-decoder结构做融合. 使用了Depthwise Conv和ghost block. 计算量小, 效果不错(Rank 4 in Track 1).

- **Bidirectional Motion Estimation With Cyclic Cost Volume for High Dynamic Range Imaging** <Br>
[An Gia Vien](https://viengiaan.github.io/), Seonghyun Park, Truong Thanh Nhat Mai, Gahyeon Kim, [Chul Lee](http://cilab.dongguk.edu/) <Br>
[CVPRW 2022] <Br>
[★] NTIRE22

- **Attention-Guided Progressive Neural Texture Fusion for High Dynamic Range Image Restoration** <Br>
Jie Chen, Zaifeng Yang, [Tsz Nam Chan](https://www.comp.hkbu.edu.hk/~edisonchan/), Hui Li, [Junhui Hou](https://sites.google.com/site/junhuihoushomepage/), Lap-Pui Chau <Br>
[TIP 2022] <Br>
[★] 设计了一个基于vgg特征的匹配模块, 从short中找到medium的过曝内容并通过替换特征的方式加以填补

- **FlexHDR: Modelling Alignment and Exposure Uncertainties for Flexible HDR Imaging** <Br>
[Sibi Catley-Chandar](https://sib1.github.io/), [Thomas Tanay](https://thomas-tanay.github.io/about/), Lucas Vandroux, [Aleš Leonardis](https://www.cs.bham.ac.uk/~leonarda/), [Gregory Slabaugh](http://eecs.qmul.ac.uk/profiles/slabaughgreg.html), [Eduardo Pérez-Pellitero](https://perezpellitero.github.io/) <Br>
[arXiv 2201] <Br>
[★] 对输入的每一张LDR, 根据亮度和光流准确度预测map, 并用它们预测spatial attention map. 每张LDR的分支通过feature的max pooling操作交换信息. 

- **Labeled from Unlabeled: Exploiting Unlabeled Data for Few-shot Deep HDR Deghosting** <Br>
[K. Ram Prabhakar](https://sites.google.com/view/kramprabhakar/), Gowtham Senthil, Susmit Agrawal, [R. Venkatesh Babu](http://cds.iisc.ac.in/faculty/venky/), [Rama Krishna Sai S Gorthi](https://sites.google.com/site/gorthisaisubrahmanyam/) <Br>
[CVPR 2021] [[TF-Code](https://github.com/Susmit-A/FSHDR)] <Br>
[★★] **Few Shot HDR**. 用少数Labeled数据(L), 较多的Static数据(S)和大量的Unlabeled数据(U), 训练HDR网络.
	
- **ADNet: Attention-guided Deformable Convolutional Network for High Dynamic Range Imaging** <Br>
Zhen Liu, Wenjie Lin, Xinpeng Li, Qing Rao, Ting Jiang, Mingyan Han, Haoqiang Fan, [Jian Sun](http://www.jiansun.org/), [Shuaicheng Liu](http://www.liushuaicheng.org/) <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/liuzhen03/ADNet)]<Br>
[★] spatial attention + deformable conv

- **A Two-Stage Deep Network for High Dynamic Range Image Reconstruction** <Br>
S M A Sharif, [Rizwan Ali Naqvi](https://sites.google.com/view/drrizwanalinaqvi/home), Mithun Biswas, Sungjun Kim <Br>
[CVPRW 2021] [[Pytorch-Code](https://github.com/sharif-apu/twostageHDR_NTIRE21)] <Br>
[★]

- **MetaHDR: Model-Agnostic Meta-Learning for HDR Image Reconstruction** <Br>
[Edwin Pan](https://edwin-pan.github.io/), Anthony Vento <Br>
[arXiv 2103] [[Pytorch-Code](https://github.com/edwin-pan/MetaHDR)] <Br>

- **HDR-GAN: HDR Image Reconstruction from Multi-Exposed LDR Images with Large Motions** <Br>
Yuzhen Niu, Jianbin Wu, Wenxi Liu, Wenzhong Guo, Rynson W.H. Lau <Br>
[TIP 2021] [[TF-Code](https://github.com/nonu116/HDR-GAN)]<Br>
[★] multi-scale network + GAN

- **Deep Coupled Feedback Network for Joint Exposure Fusion and Image Super-Resolution** <Br>
Xin Deng, Yutong Zhang, Mai Xu, [Shuhang Gu](https://shuhanggu.github.io/), Yiping Duan <Br>
[TIP 2021] [[Pytorch-Code](https://github.com/ytZhang99/CF-Net)] <Br>
[**CF-Net**] [★] 2张图像曝光融合+超分, 分成两支, 在处理中引入对方信息.
	
- **Towards Accurate HDR Imaging with Learning Generator Constraints** <Br>
[Qingsen Yan](https://qingsenyangit.github.io/), Bo Wang, [Lei Zhang](https://sites.google.com/site/leizhanghyperspectral/home), Jingyu Zhang, Zheng You, [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), Yanning Zhang <Br>
[Neurocomputing 2021] <Br>
[**GCHDRNet**] [★☆] 提出用3个LDR subnetwork将生成的HDR变换为LDR, 并对3个LDR计算loss, 目的是使网络更关注于有distortion的区域. 可以尝试下该思路.
	
- **Deep HDR Imaging via A Non-Local Network**  <Br>
[Qingsen Yan](https://qingsenyangit.github.io/), [Lei Zhang](https://sites.google.com/site/leizhanghyperspectral/home), [Yu Liu](https://sites.google.com/site/yuliuunilau/home), Yu Zhu, Jinqiu Sun, [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), Yanning Zhang <Br>
[TIP 2020] [[Keras-Code](https://github.com/tuvovan/NHDRRNet)] <Br>
[**NHDRRNet**] [★] UNet + non-local + 并行不同kernel的卷积分支

- **Deep Guided Learning for Fast Multi-Exposure Image Fusion** <Br>
[Kede Ma](https://kedema.org/), [Zhengfang Duanmu](https://ece.uwaterloo.ca/~zduanmu/), Hanwei Zhu, [Yuming Fang](http://sim.jxufe.cn/JDMKL/ymfang.html), [Zhou Wang](https://ece.uwaterloo.ca/~z70wang/) <Br>
[TIP 2020] [[Pytorch-Code](https://github.com/makedede/MEFNet)]<Br>
[**MEFNet**] [★] **无监督MEF** 小图预测融合权重, guided filter上采样作用到全图
	
- **Towards Practical and Efficient High-Resolution HDR Deghosting with CNN** <Br>
[K Ram Prabhakar](https://sites.google.com/view/kramprabhakar/), S Agrawal, [D K Singh](https://durgesh93.github.io/), B Ashwath, [R. V. Babu](http://cds.iisc.ac.in/faculty/venky/) <Br>
[ECCV 2020] <Br>
[★★] 将计算量大的光流对齐和融合网络部分在小图处理, 用BGU上采用, BGU所需的guided map通过对三帧的加权求和得到, weight通过小图预测并上采样得到. 距离实际移动端落地还有距离, 不过思路比较新奇.

- **Exposure-Structure Blending Network for High Dynamic Range Imaging of Dynamic Scenes** <Br>
Sang-Hoon Lee, Haesoo Chung, Nam Ik Cho <Br>
[Access 2020] <Br>
[★☆] S/M/L三帧HDR. 先预测L和S在结构上对齐到M的结果, 再将三张图像concat送入merge网络. 使用Kalantari数据集, 自己生成了对齐网络需要的GT(通过改变M帧的曝光得到)

- **LSD_2 - Joint denoising and deblurring of short and long exposure images with CNNs** <Br>
Janne Mustaniemi, [Juho Kannala](https://users.aalto.fi/~kannalj1/), [Jiri Matas](https://cmp.felk.cvut.cz/~matas/), [Simo Särkkä](https://users.aalto.fi/~ssarkka/), Janne Heikkilä <Br>
[BMVC 2020] [[Keras-Code](https://github.com/jannemus/LSD2)]<Br>
[★] short/long曝光融合, 用一个UNet同时实现denoise和deblur. 从RGB图像中通过模拟过曝, blur, 加噪等生成short/long数据.

- **Ganfuse: a novel multi-exposure image fusion method based on generative adversarial networks** <Br>
Zhiguang Yang, Youping Chen, Zhuliang Le, Yong Ma  <Br>
[NCA 2020] <Br>
[★] 提出了GAN loss及gradient loss, **非监督MEF**.

- **Robust High Dynamic Range (HDR) Imaging with Complex Motion and Parallax** <Br>
Zhiyuan Pu, Peiyao Guo, [M. Salman Asif](https://intra.ece.ucr.edu/~sasif/), [Zhan Ma](https://vision.nju.edu.cn/main.htm) <Br>
[ACCV 2020] <Br>

- **Deep Exposure Fusion with Deghosting via Homography Estimation and Attention Learning** <Br>
Sheng-Yeh Chen [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/) <Br>
[ICASSP 2020] <Br>
[★★] S/L两曝光MEF. 首先预测homography参数, 将L全局对齐到S, homography网络使用median threshold bitmap(MTB)作为额外的输入, 预测的是四个顶点的位移(参考Deep image homography estimation). 再通过attention, 修正局部鬼影. 最后融合. 使用了vgg loss + LSGAN loss.

- **Attention-mask dense merger (attendance)deep hdr for ghost removal** <Br>
Kareem Metwaly, Vishal Monga  <Br>
[ICASSP 2020] <Br>
[**AttenDense**] [★] 用 Spectral Angle Mapper(SAM, 其实就是两个pixel的角度) 计算三张图的运动区域mask, 用该mask得出一个loss的weight map, 使网络更关注运动区域

- **Pyramid Inter-Attention for High Dynamic Range Imaging** <Br>
Sungil Choi, [Jaehoon Cho](https://jhcho90.github.io/), Wonil Song, Jihwan Choe, Jisung Yoo, [Kwanghoon Sohn](http://diml.yonsei.ac.kr/)  <Br>
[Sensors 2020] <Br>

- **Attention-guided Network for Ghost-free High Dynamic Range Imaging** <Br>
[Qingsen Yan](https://qingsenyangit.github.io/), [Dong Gong](https://donggong1.github.io/), [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), [Anton van den Hengel](https://cs.adelaide.edu.au/~hengel/), [Chunhua Shen](https://cshen.github.io/), [Ian Reid](https://cs.adelaide.edu.au/~ianr/), Yanning Zhang <Br>
[CVPR 2019] [[Project](https://qingsenyangit.github.io/project/ahdr/)] [[Pytorch-Code](https://github.com/qingsenyangit/AHDRNet)]<Br>
[**AHDRNet**] [★★] **多帧HDR**. 基于空间attention的多帧HDR, 网络使用dilated residual dense blocks, 预测残差, loss使用μ-law压缩的L1 loss. 结构简洁, 效果不错.

- **Multi-scale Dense Networks for Deep High Dynamic Range Imaging** <Br>
[Qingsen Yan](https://qingsenyangit.github.io/), [Dong Gong](https://donggong1.github.io/), Pingping Zhang, [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), Jinqiu Sun, [Ian Reid](https://cs.adelaide.edu.au/~ianr/), Yanning Zhang <Br>
[WACV 2019]  <Br>
[★] 

- **Deep Multi-Stage Learning for HDR With Large Object Motions** <Br>
Green Rosh K S, Anmol Biswas Mandakinee, Singh Patel, B H Pawan Prasad <Br>
[ICCP 2019]  <Br>
[★☆] S/M/L三帧HDR. 先预测用两个AlignNet得到L和S在结构上对齐到M的结果, 再用MergeNet融合三帧结果. AlignNet的训练数据生成方法可以参考.

- **A Fast, Scalable, and Reliable Deghosting Method for Extreme Exposure Fusion** <Br>
[K Ram Prabhakar](https://sites.google.com/view/kramprabhakar/), Rajat Arora, Adhitya Swaminathan, Kunal Pratap Singh, [R. Venkatesh Babu](http://cds.iisc.ac.in/faculty/venky/) <Br>
[ICCP 2019] [[TF-Code](https://github.com/rajat95/Deep-Deghosting-HDR)] <Br>
[★] 对任意个输入提特征并进行feature aggregation, 使网络能处理任意输入. 提出了一个HDR数据集

- **Deep High Dynamic Range Imaging with Large Foreground Motions** <Br>
[Shangzhe Wu](https://elliottwu.com/), [Jiarui Xu](https://jerryxu.net/), [Yu-Wing Tai](https://www.cse.ust.hk/admin/people/faculty/profile/yuwing), Chi-Keung Tang <Br>
[ECCV 2018] [[Project](https://elliottwu.com/projects/hdr/)] [[TF-Code](https://github.com/elliottwu/DeepHDR)] <Br>
[**DeepHDR**] [★★] 3个encoder, 1个decoder, loss和预处理与'Deep High Dynamic Range Imaging of Dynamic Scenes'相似
	
- **Deep High Dynamic Range Imaging of Dynamic Scenes** <Br>
[Nima Khademi Kalantari](https://people.engr.tamu.edu/nimak/index.html), [Ravi Ramamoorthi](https://cseweb.ucsd.edu//~ravir/) <Br>
[TOG 2017] [[Project](https://cseweb.ucsd.edu//~viscomp/projects/SIG17HDR/)] <Br>
[★★★] 较早使用CNN做多帧HDR的一篇论文, 提出了Kalantari数据集, 其中的3张图像预处理流程, 算法整体思路, 以及使用mu-law计算loss等内容被之后很多论文借鉴

- **DeepFuse:A Deep Unsupervised Approach for Exposure Fusion with Extreme Exposure Image Pairs** <Br>
[K Ram Prabhakar](https://sites.google.com/view/kramprabhakar/home), V Sai Srikar, [R. Venkatesh Babu](http://cds.iisc.ac.in/faculty/venky/) <Br>
[ICCV 2017] [[Theano-Code](https://github.com/KRamPrabhakar/DeepFuse)] [[Unofficial-Pytorch-Code](https://github.com/SunnerLi/DeepFuse.pytorch)]<Br>
[★★]


## Single-Frame HDR
- **Learning a Practical SDR-to-HDRTV Up-conversion using New Dataset and Degradation Models** <Br>
Cheng Guo, Leidong Fan, Ziyu Xue, Xiuhua Jiang <Br>
[CVPR 2023] [[Pytorch-Code](https://github.com/AndreGuo/HDRTVDM)] <Br>

- **SDRTV-to-HDRTV via Hierarchical Dynamic Context Feature Mapping** <Br>
Gang He, Kepeng Xu, Li Xu, Chang Wu, Ming Sun, Xing Wen, Yu-Wing Tai <Br>
[MM 2022] [快手] [[Pytorch-Code](https://github.com/chxy95/HDRTVNet)] <Br>

- **Unsupervised HDR Imaging: What Can Be Learned from a Single 8-bit Video?** <Br>
Francesco Banterle, Demetris Marnerides, Kurt Debattista, Thomas Bashford-Rogers <Br>
[arXiv 2202] [[Pytorch-Code](https://github.com/chxy95/HDRTVNet)] <Br>
[★] 手动设置ev, 生成high, 最后生成high/base的scale map, 预测时以base为输入, 预测scale map和low

- **A New Journey from SDRTV to HDRTV** <Br>
Xiangyu Chen, Zhengwen Zhang, [Jimmy S. Ren](http://www.jimmyren.com/), Lynhoo Tian, [Yu Qiao](http://mmlab.siat.ac.cn/), [Chao Dong](http://xpixel.group/)  <Br>
[ICCV 2021] [[Pytorch-Code](https://github.com/chxy95/HDRTVNet)] <Br>
[**HDRTVNet**]

- **HDRUNet: Single Image HDR Reconstruction with Denoising and Dequantization** <Br>
Xiangyu Chen, Yihao Liu, Zhengwen Zhang, [Yu Qiao](http://mmlab.siat.ac.cn/), [Chao Dong](http://xpixel.group/) <Br>
[CVPRW 2021] [[Pytorch-Code](https://github.com/chxy95/HDRUNet)]<Br>
[★] base网络为UNet, 还有一个weight net和一个由SFT组成的condition net. loss用tanh L1.

- **End-to-End Differentiable Learning to HDR Image Synthesis for Multi-exposure Images** <Br>
Jung Hee Kim, Siyeong Lee, [Suk-Ju Kang](http://vds.sogang.ac.kr/) <Br>
[AAAI 2021] [[Pytorch-Code](https://github.com/JungHeeKim29/DiffHDRsyn)] <Br>
	
- **Single-Image HDR Reconstruction by Learning to Reverse the Camera Pipeline** <Br>
[Yu-Lun Liu](http://www.cmlab.csie.ntu.edu.tw/~yulunliu/), [Wei-Sheng Lai](https://www.wslai.net/), [Yu-Sheng Chen](https://www.cmlab.csie.ntu.edu.tw/~nothinglo/), Yi-Lung Kao, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/) <Br>
[CVPR 2020] [[Project](https://www.cmlab.csie.ntu.edu.tw/~yulunliu/SingleHDR)] [[TF-Code](https://github.com/alex04072000/SingleHDR)]<Br>
[★★] 用几个CNN模拟ISP中HDR到LDR的映射过程, 完成HDR. 关键是定义每个部分的训练目标和数据, 这部分没细看.

- **UnModNet: Learning to Unwrap a Modulo Image for High Dynamic Range Imaging** <Br>
Chu Zhou, Hang Zhao, Jin Han, [Chang Xu](http://changxu.xyz/), Chao Xu, Tiejun Huang, [Boxin Shi](http://ci.idm.pku.edu.cn/Publication.htm) <Br>
[NeruIPS 2020] [[Project](https://www.cmlab.csie.ntu.edu.tw/~yulunliu/SingleHDR)] [[TF-Code](https://github.com/alex04072000/SingleHDR)] <Br>

- **Single Image HDR Reconstruction Using a CNN with Masked Features and Perceptual Loss** <Br>
[Marcel Santana Santos](https://marcelsan.github.io/), Tsang Ing Ren, [Nima Khademi Kalantari](https://people.engr.tamu.edu/nimak/index.html)  <Br>
[SIGGRAPH 2020] [[Pytorch-Code](https://github.com/marcelsan/Deep-HdrReconstruction)]<Br>

- **JSI-GAN: GAN-Based Joint Super-Resolution and Inverse Tone-Mapping with Pixel-Wise Task-Specific Filters for UHD HDR Video**  <Br>
[Soo Ye Kim](https://sites.google.com/view/sooyekim), [Jihyong Oh](https://sites.google.com/view/ozbro/%ED%99%88), [Munchurl Kim](https://www.viclab.kaist.ac.kr/) <Br>
[AAAI 2020] [[TF-Code](https://github.com/JihyongOh/JSI-GAN)] <Br>
[★] adaptive conv, GAN loss

- **Learning to generate multi-exposure stacks with cycle consistency for high dynamic range imaging** <Br>
Siyeong Lee, Gwon Hwan An, [Suk-Ju Kang](http://vds.sogang.ac.kr/)   <Br>
[TMM 2020] <Br>
[★] 训练一个stop-up和一个stop-down网络, 可以对任意ev的输入改变其亮度. 反复运行两个网络, 可以得到多个不同ev的图像, 用于生成HDR图像. 使用了cycle consitency loss.

- **Deep sr-itm: Joint learning of super-resolution and inverse tone-mapping for 4k uhd hdr applications**  <Br>
[Soo Ye Kim](https://sites.google.com/view/sooyekim), [Jihyong Oh](https://sites.google.com/view/ozbro/%ED%99%88), [Munchurl Kim](https://www.viclab.kaist.ac.kr/)  <Br>
[ICCV 2019] [[MatConvNet-Code](https://github.com/sooyekim/Deep-SR-ITM)]<Br>
[★] 将输入分解为detail和base分别处理

- **iTM-Net: Deep Inverse Tone Mapping Using Novel Loss Function Considering Tone Mapping Operator** <Br>
[Yuma Kinoshita](https://sites.google.com/view/kinoshita-yuma-en/), [Hitoshi Kiya](http://www-isys.sd.tmu.ac.jp/members-2/kiya/)  <Br>
[Global SIP 2019] <Br>
[☆] 在非线性空间计算loss

- **FHDR: HDR Image Reconstruction from a SingleLDR Image using Feedback Network** <Br>
Zeeshan Khan, Mukul Khanna, Shanmuganathan Raman  <Br>
[Global SIP 2019] [[Pytorch-Code](https://github.com/mukulkhanna/fhdr)]<Br>

- **Joint High Dynamic Range Imaging and Super-Resolution from a Single Image** <Br>
Jae Woong Soh, Jae Sung Park, Nam Ik Cho  <Br>
[IEEE Access 2019] [[TF-Code](https://github.com/JWSoh/HDRI-SR)] <Br>
[★] Retinex分解辐illuminance和reflectance, 对反射分量用CNN处理

- **High Dynamic Range and Super-Resolution Imaging from a Single Image** <Br>
Jae Woong Soh, Jae Sung Park, Nam Ik Cho  <Br>
[IEEE Access 2019] <Br>
[★☆] Retinex分解辐illuminance和reflectance, 对辐照度和反射分量分别处理. HDR部分有一些较经验话的设置, 可以参考
	
- **ExpandNet: A Deep Convolutional Neural Network for High Dynamic Range Expansion from Low Dynamic Range Content** <Br>
Demetris Marnerides, [Thomas Bashford-Rogers](http://thomasbashfordrogers.com/), [Jonathan Hatchett](https://hatchett.co.uk/), [Kurt Debattista](https://warwick.ac.uk/fac/sci/wmg/people/profile/?wmgid=518)  <Br>
[EG 2018] [[Pytorch-Code](https://github.com/dmarnerides/hdr-expandnet)] [[Unofficial-TF-Code](https://github.com/echolijinghui/ExpandNet)] <Br>

- **Image Correction via Deep Reciprocating HDR Transformation** <Br>
[Xin Yang](http://faculty.dlut.edu.cn/yangxin/zh_CN/index.htm), Ke Xu, [Yibing Song](https://ybsong00.github.io/), Qiang Zhang, Xiaopeng Wei, [Rynson Lau](https://www.cs.cityu.edu.hk/~rynson/)  <Br>
[CVPR 2018] [[Project](https://ybsong00.github.io/cvpr18_imgcorrect/index.html)] [[TF-Code](https://github.com/ybsong00/DRHT)] <Br>
[**DRHT**] <Br>

- **Deep recursive hdri: Inverse tone mapping using generative adversarial networks** <Br>
Siyeong Lee, Gwon Hwan An, Suk-Ju Kang  <Br>
[ECCV 2018] [[Pytorch-Code](https://github.com/Siyeong-Lee/Deep_Recursive_HDRI)]<Br>

- **Deep Chain HDRI: Reconstructing a High Dynamic Range Image from a Single Low Dynamic Range Image** <Br>
Siyeong Lee, Gwon Hwan An, Suk-ju Kang  <Br>
[Access 2018] [[Project](https://siyeong-lee.github.io/hdr_vds_dataset/)] <Br>

- **HDR image reconstruction from a single exposure using deep CNNs** <Br>
[Gabriel Eilertsen](http://vcl.itn.liu.se/members/gabriel-eilertsen), [Joel Kronander](http://vcl.itn.liu.se/members/joel-kronander), [Gyorgy Denes](https://www.cl.cam.ac.uk/~gd355/), [Rafał K. Mantiuk](https://www.cl.cam.ac.uk/~rkm38/), [Jonas Unger](http://webstaff.itn.liu.se/~jonun/web/Home.php) <Br>
[Siggraph Asia 2017] [[Project](https://weber.itn.liu.se/~gabei62/hdrcnn/)] [[TF-Code](https://github.com/gabrieleilertsen/hdrcnn)] <Br>
[**HDRCNN**] [★] 粗读, 较早将CNN用于HDR的一篇paper, 网络结构比较老, 但提出了两个可能有趣的点: 1) 将输入转换到log域训练更符合人眼视觉特性; 2) 高光部分采用输入和输出线性加权的方式, 修复过曝光, 并避免形成带状伪影. <Br>

- **Deep Reverse Tone Mapping** <Br>
[Yuki Endo](http://www.npal.cs.tsukuba.ac.jp/~endo/index_en.html), [Yoshihiro Kanamori](http://kanamori.cs.tsukuba.ac.jp/index.html), [Jun Mitani](http://mitani.cs.tsukuba.ac.jp/en/)  <Br>
[Siggraph Asia 2017] [[Project](http://www.npal.cs.tsukuba.ac.jp/~endo/projects/DrTMO/)] [[Unofficial-Pytorch-Code](https://github.com/shleecs/DrTMO_unofficial_pytorch)] <Br>
[**DrTMO**]

## Video HDR
- **HDR Video Reconstruction with Tri-Exposure Quad-Bayer Sensors** <Br>
Yitong Jiang, [Inchang Choi](http://www.inchangchoi.info/), Jun Jiang, [Jinwei Gu](http://www.gujinwei.org/)  <Br>
[arXiv 2103] <Br>
	
- **HDR Video Reconstruction: A Coarse-to-fine Network and A Real-world Benchmark Dataset** <Br>
[Guanying Chen](https://guanyingc.github.io/), [Chaofeng Chen](http://chaofengc.github.io/), [Shi Guo](https://scholar.google.com/citations?user=5hsEmuQAAAAJ&hl=en), [Zhetong Liang](https://scholar.google.com/citations?user=fCnuU9YAAAAJ&hl=en), [Kwan-Yee K. Wong](http://i.cs.hku.hk/~kykwong/), [Lei Zhang](https://www4.comp.polyu.edu.hk/~cslzhang/)  <Br>
[ICCV 2021] [[Project](https://guanyingc.github.io/DeepHDRVideo/)] [[Pytorch-Code](https://github.com/guanyingc/DeepHDRVideo)] <Br>
[**DeepHDRVideo**] [★★] 给定5张不同EV值的视频帧, 采用coarse to fine的方式生成hdr图像, 网络较复杂. 另外提出了一个HDR数据集, 生成数据的方法可以借鉴.

- **Deep HDR Video from Sequences with Alternating Exposures** <Br>
[Nima Khademi Kalantari](https://people.engr.tamu.edu/nimak/index.html), [Ravi Ramamoorthi](https://cseweb.ucsd.edu/~ravir/)  <Br>
[Eurographics 2019] <Br>
[★] 光流对齐加融合, 提出了一个从HDR视频生成样本的流程可以研究下

	
## New Sensor HDR
- **HDR Video Reconstruction with Tri-Exposure Quad-Bayer Sensors** <Br>
Yitong Jiang, [Inchang Choi](http://www.inchangchoi.info/), Jun Jiang, [Jinwei Gu](http://www.gujinwei.org/) <Br>
[arXiv 2103] <Br>
[★★] **Tri-Exposure Quad-Bayer Sensor video HDR**. 提出了一个包括HDR fusion, 时域去噪, 超分三个模块的pipeline.
	
- **Hdr denoising and deblurring by learning spatio-temporal distortion models**  <Br>
Uğur Çoğalan, [Mojtaba Bemana](https://people.mpi-inf.mpg.de/~mbemana/), [Karol Myszkowski](https://people.mpi-inf.mpg.de/~karol/), [Hans-Peter Seidel](https://people.mpi-inf.mpg.de/~hpseidel/), [Tobias Ritschel](http://www.homepages.ucl.ac.uk/~ucactri/) <Br>
[arXiv 2012] <Br>
[★★] **Dual-exposure HDR**, 奇数列短曝光, 偶数列长曝光. 网络采用UNet. 提出了一个生成数据的流程.
	
- **Deep joint deinterlacing and denoising for single shot dual-iso hdr reconstruction** <Br>
Ugur Cogalan, [Ahmet Oguz Akyuz](https://user.ceng.metu.edu.tr/~akyuz/index.html)  <Br>
[TIP 2020] [[Code & Dataset](https://user.ceng.metu.edu.tr/~akyuz/publications.html)]<Br>	
[★★] **Dual-ISO HDR**. 两个网络分别处理low/high图像. 通过分析噪声, 提出了一个生成Dual-ISO数据集的方法

- **High Dynamic Range Imaging: Spatially Varying Pixel Exposures** <Br>
[Shree K. Nayar](http://www.cs.columbia.edu/~nayar/), Tomoo Mitsunaga  <Br>
[CVPR 2000] <Br>
[**SVE**] [★] 提出一个基于硬件的HDR图像生成方法. 在相机传感器前放置一个optical mask, mask上有不同exposure的pattern, 利用邻域不同曝光的像素值, 恢复目标像素值, 动态范围可大致扩展到Emax/Emin倍.


## Traditional Methods
- **High Dynamic Range and Super-Resolution From Raw Image Bursts**  <Br>
[Bruno Lecouat](https://bruno-31.github.io/), [Thomas Eboli](https://teboli.github.io/), [Jean Ponce](https://www.di.ens.fr/~ponce/), [Julien Mairal](https://lear.inrialpes.fr/people/mairal/)  <Br>
[SIGGRAPH 2022] <Br>

- **Auto Complementary Exposure Control for High Dynamic Range Video Capturing** <Br>
Bing Han, Xiu Jia, [Rui Song](https://web.xidian.edu.cn/songrui/), Feng Ran, Peng Rao <Br>
[Access 2021]<Br> 
[★☆] 提出了一个确定长短曝最佳曝光参数的pipeline. 1) 文中分析发现, 使图像(块)熵最大的曝光时间就是该图像最佳曝光时间, 并用高斯分布模拟熵随时间变化的分布(μ即为最大熵的曝光时间); 2) 拍摄若干张不同曝光的图像, 将图像分成patch, 统计每个patch在每个曝光时间的熵, 计算高斯分布的μ和σ, 用GMM建模, 将patch分类为过曝, 正常, 欠曝三类. 经过EM迭代, 可得到每个patch的类别, 以及S/M/L三个曝光的μ(即为该曝光情况下对应的最优曝光时间).

- **Exposure bracketing via automatic exposure selection**  <Br>
Reza Pourreza-Shahri, [Nasser Kehtarnavaz](https://personal.utdallas.edu/~kehtar/)  <Br>
[ICIP 2015]
[★] [**MEF**, **AEC**] 根据当前帧的亮度直方图, 聚类成over, normal, short三类, 调整曝光时间, 使t+1时刻三帧的中间灰度(127)正好对应三类的聚类中心.

- **Fast exposure time decision in multi-exposure HDR imaging**  <Br>
Yongjie Piao, Guang Jin  <Br>
[SPIE 2012]
[★] [**AEC**] 根据当前帧中值确定medium曝光, 再把medium帧的最小和最大场景亮度对应到short和long的图像中值上, 以此确定三帧的曝光参数.

- **Noise-Optimal Capture for High Dynamic Range Photography**  <Br>
[Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Frédo Durand](http://people.csail.mit.edu/fredo/), [William T. Freeman](http://billf.mit.edu/)  <Br>
[CVPR 2010] [[Project](http://people.csail.mit.edu/hasinoff/hdrnoise/)] <Br>
[★★☆] 从成像的物理过程出发, 推导出最大化SNR下限和最短拍摄时间的拍摄参数设置. 文中对噪声建模和ISO与SNR关系的论述比较清晰, 值得学习. 没有考虑多帧间的motion.

- **High Dynamic Range Imaging by Fusing Multiple Raw Images and Tone Reproduction** <Br>
[Wen-Chung Kao](https://scholar.lib.ntnu.edu.tw/en/persons/wen-chung-kao) <Br>
[TCE 2008] <Br>
[★☆] 提出了一个针对静止场景的多张raw融合并tone mapping的pipeline, 可以学习
	
- **Exposure Fusion** <Br>
[Tom Mertens](http://www.mericam.net/), [Jan Kautz](https://jankautz.com/), Frank Van Reeth<Br>
[PG 2007] [[Project](https://mericam.github.io/exposure_fusion/index.html)] <Br>
[★★★] [**MEF**] contrast, saturation, well-exposedness三个加权得到weight map. 将图像用拉普拉斯金字塔分解, weight用高斯金字塔分解, 在多个尺度融合.

- **High Dynamic Range Video** <Br>
[Sing Bing Kang](http://www.singbingkang.com/), [Matthew Uyttendaele](https://research.facebook.com/people/uyttendaele-matt/), [Simon Winder](http://simonwinder.com/), [Richard Szeliski](http://szeliski.org/RichardSzeliski.htm)  <Br>
[TOG 2003] <Br>
[★★] 提出了一个视频HDR pipeline. 1.根据场景亮度, 设置相邻帧的曝光值; 2.将相邻帧处理到相同亮度, 做运动检测和warping. 对于当前帧saturate的部分, 使用前后两帧之间的光流估计到当前帧的光流并做warp, 没有saturate的部分, 利用前后帧到当前帧的光流直接warp, 并用一些策略fuse; 3.将HDR的radiance map通过tone mapping转换为能显示的LDR视频, 使用前后若干帧统计平均log域亮度, 做全局scale, 局部只根据当前帧scale

- **Fast, Robust Image Registration for Compositing High Dynamic Range Photographs from Hand-Held Exposures** <Br>
Greg Ward  <Br>
[JGT 2003] <Br>
[★★] MTB算法

- **High Dynamic Range Imaging** <Br>
Greg Ward  <Br>
[CIC 2001] <Br>
[★] 讲了color rendering的pipeline, 包括: 怎么估计真实场景目标的光强, 转换到颜色空间的近似表示, 将信息记录为HDR格式, tone mapping以在设备上显示等

- **Dynamic range improvement through multiple exposures** <Br>
Mark A Robertson, Sean Borman, Robert L Stevenson  <Br>
[ICIP 1999] <Br>
[★★]

- **Recovering High Dynamic Range Radiance Maps from Photographs** <Br>
[Paul Debevec](http://www.pauldebevec.com/), [Jitendra Malik](https://people.eecs.berkeley.edu/~malik/)<Br>
[SIGGRAPH 1997] [[Project](http://www.pauldebevec.com/Research/HDR/)] <Br>
[★★★] 经典的多曝光HDR算法, 不考虑motion, 主要包括通过最优化求CRF和融合生成HDR两部分. CRF计算部分不显式建模, 而是求radiance和像素值间的查找表, 加入一些平滑约束, 求解得到.
	


# Tone Mapping
## DL Methods
- **Unpaired Learning for High Dynamic Range Image Tone Mapping**  <Br>
Yael Vinker, Inbar Huberman-Spiegelglas, [Raanan Fattal](https://www.cs.huji.ac.il/w~raananf/) <Br>
[ICCV 2021] <Br>
[★☆] 基于GAN的无监督tone mapping, 使用LSGAN loss和patch相关系数loss, 输入做了自适应的log压缩预处理, 压缩参数通过最小化与自然LDR直方图交叉熵得到.
	
- **Deep Tone Mapping Operator for High Dynamic Range Images**  <Br>
Aakanksha Rana, Praveer Singh, [Giuseppe Valenzise](https://l2s.centralesupelec.fr/u/valenzise-giuseppe/), [Frederic Dufaux](https://l2s.centralesupelec.fr/u/dufaux-frederic/), [Nikos Komodakis](https://www.csd.uoc.gr/~komod/), Aljosa Smolic <Br>
[TIP 2019] [[PYtorch-Code](https://github.com/Aakanksha-Rana/DeepTMO)]	<Br>
[**DeepTMO**] [★] 较早用CNN做tone mapping的论文, 使用了two-scale结构, loss使用LSGAN loss, 判别器feature matching loss和vgg loss


## Traditional Methods
- **A Hybrid ℓ1-ℓ0 Layer Decomposition Model for Tone Mapping** <Br>
Zhetong Liang, [Jun Xu](https://csjunxu.github.io/), [David Zhang](http://www4.comp.polyu.edu.hk/~csdzhang/), Zisheng Cao, [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
[CVPR 2018] [[Code](https://github.com/csjunxu/L1-L0-Tone-mapping)]	<Br>
[★] l1约束base layer, l0约束detail layer

- **Adaptive Local Tone Mapping Based on Retinex for High Dynamic Range Images** <Br>
H Ahn, B Keum, D Kim, HS Lee <Br>
[ICCE 2013] [[Code](https://github.com/csjunxu/L1-L0-Tone-mapping)]	<Br>

- **Local Laplacian Filters: Edge-aware Image Processing with a Laplacian Pyramid**  <Br>
[Sylvain Paris](http://people.csail.mit.edu/sparis/), [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Jan Kautz](https://jankautz.com/) <Br>
[SIGGRAPH 2011] [[Project](http://people.csail.mit.edu/sparis/publi/2011/siggraph/)] <Br>
**Related** [[Fast Local Laplacian Filters]](http://imagine.enpc.fr/~aubrym/projects/llf/index.html)  <Br>
[**LLF**] [★★★] 著名的LLF, 可用于多个任务, tone mapping中用的也很多.

- **Tone-mapping high dynamic range images by novel histogram adjustment**  <Br>
Jiang Duan, Marco Bressan, Chris Dance, [Guoping Qiu](http://www.cs.nott.ac.uk/~pszqiu/)  <Br>
[PR 2010] <Br>
[**HALEQ**] [**ALHA**] [★★☆]

- **Fast Bilateral Filtering for the Display of High-Dynamic-Range Images**  <Br>
[Frédo Durand](https://people.csail.mit.edu/fredo/), [Julie Dorsey](https://graphics.cs.yale.edu/people/julie-dorsey) <Br>
[TOG 2002]  <Br>
[★★☆] 使用fast双边滤波, 分离base和detail, base做压缩, detail不懂, 再将压缩后的base和detail融合, 即为输出

- **Photographic tone reproduction for digital images**  <Br>
[Erik Reinhard](http://erikreinhard.com/), Michael Stark, [Peter Shirley](https://www.petershirley.com/), [James Ferwerda](https://jamesferwerda.com/) <Br>
[TOG 2002]  <Br>
[**Reinhard tone mapping**] [★★☆] 1. 在log域计算平均照度, 并用其对全图进行scale; 2. 自适应dodging-and-burning, 实现局部tone mapping

	
# CRF
## DL Methods
- **CRF-net: Single Image Radiometric Calibration using CNNs**  <Br>
Han Li, [Pieter Peers](https://www.cs.wm.edu/~ppeers/) <Br>
[CVMP 2017] <Br>
[★★] 较少的用DL做CRF预测的paper, 效果有限, 但思路被一些方法借鉴, 如"HDR by Learning to Reverse the Camera Pipeline"
	
## Traditional Methods
- **Radiometric Self Calibration**  <Br>
Tomoo Mitsunaga, [Shree K. Nayar](http://www.cs.columbia.edu/~nayar/) <Br>
[CVPR 1999] <Br>
[★★★] 预测CRF的经典方法. 将CRF建模为一个n次多项式. 在exposure ratio不能精确得到(认为相机给出的光圈, shutter speed等参数不能精确地反映曝光量)的情况下, 通过迭代优化的方式求多项式系数和ratio.
	


# Datasets

## Multi-frame HDR
### With Motion
| Name      | Link                                                                    | Download | With GT | Size |                                                          |
| --------- | ----------------------------------------------------------------------- | -------- | ------- | ---- | -------------------------------------------------------- |
| Kalantari | [Project](https://cseweb.ucsd.edu//~viscomp/projects/SIG17HDR/)         | Yes      | Yes     | 89   | S/M/L 3-frame. Real Scene. Canon EOS-5D Mark III camera. |
| Prabhakar | [Project](https://val.cds.iisc.ac.in/HDR/ICCP19/)                       | Yes      | Yes     | 582  |                                                          |
| NTIRE22   | [Project](https://codalab.lisn.upsaclay.fr/competitions/1514)           | Yes      | Yes     |      |                                                          |
| Tursun    | [Project](https://user.ceng.metu.edu.tr/~akyuz/files/eg2016/index.html) | Yes      | No      |      |                                                          |
| Sumsung Synthetic    | [Project](https://github.com/nadir-zeeshan/sensor-realistic-synthetic-data) | Yes      | Yes      |      |                                                          |


### Without Motion
| Name  | Link                                         | Download | With GT | Size |                                                           |
| ----- | -------------------------------------------- | -------- | ------- | ---- | --------------------------------------------------------- |
| SICE  | [Project](https://github.com/csjcai/SICE)    | Yes      | Yes     | 589  | MEF数据集. 用多个相机收集室内外静止场景的多曝光样本, 用13种MEF和HDR方法处理, 挑出最好的作为GT. |
| HDRPS | [Project](http://markfairchild.org/HDR.html) | Yes      | No      | 106  |                                                           |


## Single-frame HDR
| Name        | Link                                                      | Download        | With GT | Size |                                        |
| ----------- | --------------------------------------------------------- | --------------- | ------- | ---- | -------------------------------------- |
| Liu         | [Project](https://alex04072000.github.io/SingleHDR)       | Yes             | Yes     |      | HDR-SYNTH dataset +  HDR-REAL dataset: |
| Eilertsen   | [Project](https://weber.itn.liu.se/~gabei62/hdrcnn/)      | Yes (Test only) | Yes     | 96   | Degrade HDRs to get LDRs               |
| VDS dataset | [Project](https://siyeong-lee.github.io/hdr_vds_dataset/) | Yes             | Yes     | 96   | Degrade HDRs to get LDRs               |


## Video HDR
| Name        | Link                                                           | Download | With GT | Size        |                                           |
| ----------- | -------------------------------------------------------------- | -------- | ------- | ----------- | ----------------------------------------- |
| Chen        | [Project](https://guanyingc.github.io/DeepHDRVideo/)           | Yes      | Yes     |             | S/M/L 3-frame LDR + HDR. Sythetic + real. |
| Kalantari13 | [Project](https://web.ece.ucsb.edu/~psen/PaperPages/HDRVideo/) | Yes      | Yes     | 2 sequences | S/M/L 3-frame LDR + HDR. Real scenes.     |


## HDR videos and images
| Name      | Link                                                                                                        | Download | Size         |                                                            |
| --------- | ----------------------------------------------------------------------------------------------------------- | -------- | ------------ | ---------------------------------------------------------- |
| HdM       | [Project](https://www.hdm-stuttgart.de/vmlab/hdm-hdr-2014/) | Yes      | 33 sequences | 包括室内室外不同光源场景, 视频质量较高. 缺点是场景数量有限, 由于mirror会有flare等artifact. |
| Boitard   | [Project](https://people.ece.ubc.ca/rboitard/)                                                              | Yes      | 7 sequences  |                                                            |
| MPI       | [Project](https://resources.mpi-inf.mpg.de/hdr/video/)                                                      | Yes      | 2 sequences  | IMS Chips HDR Camera                                       |
| DML-HDR   | [Project](http://dml.ece.ubc.ca/data/DML-HDR/)                                                              | Yes      | 5 sequences  | RED SCARLET–X HDR Camera                                   |
| Liu       | [Project](http://hdrv.org/)                                                                                 | No       | 10 sequences | Website unaccessble. Can download from Chen dataset        |
| HDR Haven | [Project](https://polyhaven.com/hdris)                                                                      | Yes      | 537          |                                                            |
| Ward      | [Project](http://www.anyhere.com/gward/hdrenc/pages/originals.html)                                         | Yes      | 33           |                                                            |
| Funt      | [Project](https://www2.cs.sfu.ca/~colour/data/funt_hdr/#DATA)                                               | Yes      | 105          |                                                            |
| HDR-Eye   | [Project](https://www.epfl.ch/labs/mmspg/downloads/hdr-eye/)                                                | Failed   | 46           |                                                            |


# Resources
- [HDR Deghosting Paper List](https://github.com/JimmyChame/The-State-of-the-Art-in-HDR-Deghosting)
- [HDR Toolbox (Matlab/Octave)](https://github.com/banterle/HDR_Toolbox)
