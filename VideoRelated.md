# Table of Contents
- [Video Super Resolution](#video-super-resolution)
- [Frame Interpolation](#frame-interpolation)
- [Video Enhancement & Restoration](#video-enhancement-and-restoration)
- [Video Stabilization](#video-stabilization)
- [Video Debluring](#video-debluring)
- [Video Deraining](#video-deraining)
- [Video Dehazing](#video-dehazing)
- [Video Matting](#video-matting)
- [Video Inpainting](#video-inpainting)
- [Video Synthesis](#video-synthesis)
- [Misc](#misc)


# Video Super Resolution
- **Learning Spatiotemporal Frequency-Transformer for Compressed Video Super-Resolution**  <Br>
Zhongwei Qiu, [Huan Yang(https://www.microsoft.com/en-us/research/people/huayan/publications/), Jianlong Fu, Dongmei Fu <Br>
[ECCV 2022] [[Pytorch-Code](https://github.com/researchmm/FTVSR)] <Br>
[**FTVSR**]

- **Towards Interpretable Video Super-Resolution via Alternating Optimization**  <Br>
[Jiezhang Cao](https://www.jiezhangcao.com/), [Jingyun Liang](https://jingyunliang.github.io/), [Kai Zhang](https://cszn.github.io/), [Wenguan Wang](http://homepage.hit.edu.cn/wangmengzuo), [Qin Wang](https://www.qin.ee/zh/), [Yulun Zhang](https://yulunzhang.com/), [Hao Tang](http://disi.unitn.it/~hao.tang/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html) <Br>
[ECCV 2022] [[Pytorch-Code](https://github.com/caojiezhang/DAVSR)] <Br>

- **AnimeSR: Learning Real-World Super-Resolution Models for Animation Videos**  <Br>
Yanze Wu, [Xintao Wang](https://xinntao.github.io/), Gen Li, Ying Shan <Br>
[arXiv 2206]  <Br>
[★☆] 提出了一个高清动画数据集. 提出了一个学习learnable basic operator的流程, 该算子可以加入到退化流程中生成更真实的LR样本.

- **Real-RawVSR: Real-World Raw Video Super-Resolution with a Benchmark Dataset**  <Br>
[Jiyang Yu](http://jiyang.fun/), Jingen Liu, [Liefeng Bo](https://research.cs.washington.edu/istc/lfb/), [Tao Mei](https://taomei.me/) <Br>
[ECCV 2022] [[Pytorch-Code](https://github.com/zmzhang1998/Real-RawVSR)] <Br>
[★☆] 收集了一个真实的HR/LR数据集, 通过beam-splitter和两个相机收集LR, HR, 用全局和局部的对齐将HR对齐到LR上.

- **Memory-Augmented Non-Local Attention for Video Super-Resolution**  <Br>
[Jiyang Yu](http://jiyang.fun/), Jingen Liu, [Liefeng Bo](https://research.cs.washington.edu/istc/lfb/), [Tao Mei](https://taomei.me/) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/jiy173/MANA)] <Br>

- **VideoINR: Learning Video Implicit Neural Representation for Continuous Space-Time Super-Resolution**  <Br>
[Zeyuan Chen](http://zeyuan-chen.com/), [Yinbo Chen](https://yinboc.github.io/), Jingwen Liu, Xingqian Xu, [Vidit Goel](https://vidit98.github.io/), Zhangyang Wang, [Humphrey Shi](https://www.humphreyshi.com/), [Xiaolong Wang](https://xiaolonw.github.io/) <Br>
[CVPR 2022] [[Project](http://zeyuan-chen.com/VideoINR/)] [[Pytorch-Code](https://github.com/Picsart-AI-Research/VideoINR-Continuous-Space-Time-Super-Resolution)] <Br>

- **Learning Trajectory-Aware Transformer for Video Super-Resolution** <Br>
Chengxu Liu, [Huan Yang](https://www.microsoft.com/en-us/research/people/huayan/), [Jianlong Fu](https://www.microsoft.com/en-us/research/people/jianf/), [Xueming Qian](http://smiles.xjtu.edu.cn/) <Br>
[CVPR 2022 Oral] [[Pytorch-Code](https://github.com/researchmm/TTVSR)] <Br>
[**TTVSR**]

- **Reference-based Video Super-Resolution Using Multi-Camera Video Triplets**  <Br>
[Junyong Lee](https://junyonglee.me/), Myeonghee Lee, [Sunghyun Cho](https://www.scho.pe.kr/), [Seungyong Lee](http://cg.postech.ac.kr/leesy/) <Br>
[CVPR 2022] [[Project](https://junyonglee.me/projects/RefVSR/)] [[Pytorch-Code](https://github.com/codeslake/RefVSR)] <Br>
	
- **Investigating Tradeoffs in Real-World Video Super-Resolution** <Br>
[Kelvin C.K. Chan](https://ckkelvinchan.github.io/), [Shangchen Zhou](https://shangchenzhou.com/), [Xiangyu Xu](https://sites.google.com/view/xiangyuxu), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
[CVPR 2022]  [[Pytorch-Code](https://github.com/ckkelvinchan/RealBasicVSR)] <Br>
[**RealBasicVSR**]

- **Real-Time Super-Resolution System of 4K-Video Based on Deep Learning** <Br>
Yanpeng Cao, Chengcheng Wang, Changjun Song, Yongming Tang, He Li <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/Thmen/EGVSR)] <Br>
[**EGVSR**] [★☆] 快速视频超分网络, 模型和loss参考了TecoGAN

- **Video Super-Resolution Transformer** <Br>
[Jiezhang Cao](https://www.jiezhangcao.com/), [Yawei Li](https://yaweili.bitbucket.io/), [Kai Zhang](https://cszn.github.io/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html) <Br>
[arXiv 2106] [[Pytorch-Code](https://github.com/caojiezhang/VSR-Transformer)] <Br>

- **BasicVSR++: Improving Video Super-Resolution with Enhanced Propagation and Alignment** <Br>
[Kelvin C.K. Chan](https://ckkelvinchan.github.io/), [Shangchen Zhou](https://shangchenzhou.com/), [Xintao Wang](https://xinntao.github.io/), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/open-mmlab/mmediting)] <Br>
[★] 在BasicVSR的基础上, 使用反复前向后向传播的结构和flow-guided deformable alignment, 提升了性能

- **DynaVSR: Dynamic Adaptive Blind VideoSuper-Resolution** <Br>
Suyoung Lee, [Myungsub Choi](https://myungsub.github.io/), [Kyoung Mu Lee](https://cv.snu.ac.kr/index.php/~kmlee/)   <Br>
[WACV 2021] [[Project](https://ckkelvinchan.github.io/projects/DCN/)] [[Pytorch-Code](https://github.com/ckkelvinchan/offset-fidelity-loss)] <Br>

- **Understanding Deformable Alignment in Video Super-Resolution** <Br>
[Kelvin C.K. Chan](https://ckkelvinchan.github.io/), [Xintao Wang](https://xinntao.github.io/), [Ke Yu](https://yuke93.github.io/), Chao Dong, [Chen Change Loy](https://www.mmlab-ntu.com/person/ccloy/)   <Br>
[AAAI 2021] [[Project](https://ckkelvinchan.github.io/projects/DCN/)] [[Pytorch-Code](https://github.com/ckkelvinchan/offset-fidelity-loss)] <Br>
[**DCN**] [★] 分析了可变形卷积对齐和flow-based对齐的相似性, 指出deformable alignment中offset的多样性对VSR这样的任务有优势. 另外, 提出了一个offset fidelity loss, 用光流约束offset的学习.

- **Omniscient Video Super-Resolution** <Br>
Peng Yi, Zhongyuan Wang, [Kui Jiang](https://github.com/kuijiang0802/kuijiang0802.github.io/blob/master/home.md), [Junjun Jiang](http://homepage.hit.edu.cn/jiangjunjun), Tao Lu, Xin Tian, [Jiayi Ma](https://sites.google.com/view/jiayima) <Br>
[ICCV 2021] [[Pytorch-Code](https://github.com/psychopa4/OVSR)]<Br>
[**OVSR**]

- **Deep Blind Video Super-resolution** <Br>
 [Jinshan Pan](https://jspan.github.io/), [Haoran Bai](https://csbhr.github.io/), Jiangxin Dong, Jiawei Zhang, Jinhui Tang <Br>
[ICCV 2021] [[Pytorch-Code](https://github.com/csbhr/Deep-Blind-VSR)]<Br>
	
- **COMISR:Compression-Informed Video Super-Resolution** <Br>
Yinxiao Li, [Pengchong Jin](https://research.google/people/PengchongJin/), [Feng Yang](https://sites.google.com/view/feng-yang), [Ce Liu](http://people.csail.mit.edu/celiu/), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/), [Peyman Milanfar](https://sites.google.com/view/milanfarhome/)   <Br>
[ICCV 2021] [[TF2-Code](https://github.com/google-research/google-research/tree/master/comisr)]<Br>

- **Space-Time Distillation for Video Super-Resolution** <Br>
Zeyu Xiao, [Xueyang Fu](https://xueyangfu.github.io/), Jie Huang, Zhen Cheng, Zhiwei Xiong <Br>
[CVPR 2021] <Br>
[**STD**] [★] 分为空间和时间蒸馏两部分. 空间蒸馏通过让S和T的空间attention map接近来训练. 时间蒸馏使用ConvLSTM提取时间特征, 监督该特征训练.

- **Video Rescaling Networks with Joint Optimization Strategies for Downscaling and Upscaling** <Br>
 [Yan-Cheng Huang](https://www.linkedin.com/in/hyancheng96),  [Yi-Hsin Chen](mailto:yhchen12101@gmail.com),  [Cheng-You Lu](https://johnnylu305.github.io), [Hui-Po Wang](https://a514514772.github.io), [Wen-Hsiao Peng](https://sites.google.com/g2.nctu.edu.tw/wpeng/cv), [Ching-Chun Huang](http://acm.cs.nctu.edu.tw/Home.aspx)   <Br>
[CVPR 2021] [[Project](https://ding3820.github.io/MIMO-VRN/)] [[Pytorch-Code](https://github.com/ding3820/MIMO-VRN)]<Br>
[**MIMO-VRN**]

- **BasicVSR: The Search for Essential Components in Video Super-Resolution and Beyond** <Br>
[Kelvin C.K. Chan](https://ckkelvinchan.github.io/), [Xintao Wang](https://xinntao.github.io/), [Ke Yu](https://yuke93.github.io/), [Chao Dong](https://scholar.google.com.hk/citations?user=OSDCB0UAAAAJ&hl=zh-CN), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
[CVPR 2021] [[Project](https://ckkelvinchan.github.io/projects/BasicVSR/)] [[Pytorch-Code](https://github.com/ckkelvinchan/BasicVSR-IconVSR)]<Br>
[★☆] 将视频超分分解为propagation, alignment, aggregation和upsampling四部分. 在此基础上设计了BasicVSR网络, 以及加入了两个新设计模块的IconVSR

- **Temporal Modulation Network for Controllable Space-Time Video Super-Resolution** <Br>
Gang Xu, [Jun Xu](https://csjunxu.github.io/), Zhen Li, Liang Wang, [Xing Sun](https://www.sunxing.org/), [Mingming Cheng](http://mmcheng.net/cmm/) <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/CS-GangXu/TMNet)]<Br>
[**TMNet**] [★] 使用一个时间调制模块, 根据不同的t, 控制deformable conv的插帧结果. 设计了一个feature fusion模块, refine局部运动, 使用双向可变形卷积BDConvLSTM refine全局运动.

- **Real-Time Super-Resolution System of 4K-Video Based on Deep Learning** <Br>
Yanpeng Cao, Chengcheng Wang, Changjun Song, Yongming Tang, He Li <Br>
[arXiv 2107] [[Pytorch-Code](https://github.com/Thmen/EGVSR)]<Br>
[**EGVSR**] [★☆] 基于TecoGAN, 设计了一个轻量级视频超分模型

- **Learning the Loss Functions in a Discriminative Space for Video Restoration** <Br>
[Younghyun Jo](https://yhjo09.github.io/), Jaeyeon Kang, Seoung Wug Oh, Seonghyeon Nam, Peter Vajda, [Seon Joo Kim](https://sites.google.com/view/seoungwugoh/) <Br>
[arXiv 2003] <Br>

- **ISR: Deep Joint Frame Interpolation and Super-Resolution with A Multi-scale Temporal Loss** <Br>
[Soo Ye Kim](https://sites.google.com/view/sooyekim),[Jihyong Oh](https://sites.google.com/view/ozbro/%ED%99%88), [Munchurl Kim](https://www.viclab.kaist.ac.kr/) <Br>
[AAAI 2020] [[TF-Code](https://github.com/JihyongOh/FISR)]<Br>
	
- **Space-Time-Aware Multi-Resolution Video Enhancement** <Br>
[Muhammad Haris](https://alterzero.github.io/), [Greg Shakhnarovich](https://ttic.uchicago.edu/~gregory/), [Norimichi Ukita](https://www.toyota-ti.ac.jp/Lab/Denshi/iim/ukita/)<Br>
[CVPR 2020] [[Project](https://alterzero.github.io/projects/STAR.html)] [[Pytorch-Code](https://github.com/alterzero/STARnet)]<Br>
[**STARnet**] [★★] 时空联合超分
	
- **TDAN: Temporally-Deformable Alignment Network for Video Super-Resolution** <Br>
[Yapeng Tian](https://yapengtian.org/), [Yulun Zhang](http://yulunzhang.com/), [Yun Fu](http://www1.ece.neu.edu/~yunfu/), [Chenliang Xu](https://www.cs.rochester.edu/~cxu22/)<Br>
[CVPR 2020] [[Pytorch-Code](https://github.com/YapengTian/TDAN-VSR-CVPR-2020)]<Br>
[**TDAN**] [★☆] 用deformable conv做VSR
	
- **Fast and Accurate One-Stage Space-Time Video Super-Resolution** <Br>
 [Xiaoyu Xiang](https://engineering.purdue.edu/people/xiaoyu.xiang.1), [Yapeng Tian](http://yapengtian.org/), [Yulun Zhang](http://yulunzhang.com/), [Yun Fu](http://www1.ece.neu.edu/~yunfu/), [Jan P. Allebach](https://engineering.purdue.edu/~allebach/), [Chenliang Xu](https://www.cs.rochester.edu/~cxu22/) <Br>
[CVPR 2020]  [[Pytorch-Code](https://github.com/Mukosame/Zooming-Slow-Mo-CVPR-2020)]<Br>
[**Zooming-Slow-M**] [★☆] 时空联合超分, 基于deformable卷积和ConvLSTM

- **STVUN: Deep Space-Time Video Upsampling Networks** <Br>
Jaeyeon Kang, [Younghyun Jo](https://yhjo09.github.io/), [Seoung Wug Oh](https://sites.google.com/view/seoungwugoh), [Peter Vajda](https://sites.google.com/site/vajdap/), [Seon Joo Kim](https://sites.google.com/site/seonjookim/) <Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/JaeYeonKang/STVUN-Pytorch)]<Br>	

- **Across Scales & Across Dimensions: Temporal Super-Resolution using Deep Internal Learning** <Br>
Liad Pollak Zuckerman, Eyal Naor, George Pisha, [Shai Bagon](https://www.weizmann.ac.il/math/bagon/), Michal Irani <Br>
[ECCV 2020] [[Project](http://www.wisdom.weizmann.ac.il/~vision/DeepTemporalSR/)] [[Pytorch-Code](https://github.com/eyalnaor/DeepTemporalSR)]<Br>	
[**DeepTemporalSR**]

- **MuCAN: Multi-Correspondence Aggregation Network for Video Super-Resolution** <Br>
Wenbo Li, [Xin Tao](http://www.xtao.website/), Taian Guo, [Lu Qi](http://luqi.info/), Jiangbo Lu, [Jiaya Jia](http://jiaya.me/) <Br>
[ECCV 2020] <Br>

- **Video Super-Resolution with Recurrent Structure-Detail Network** <Br>
Takashi Isobe, [Xu Jia](https://stephenjia.github.io/), [Shuhang Gu](https://sites.google.com/site/shuhanggu/), Songjiang Li, Shengjin Wang, Qi Tian<Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/junpan19/RSDN)]<Br>
[**RSDN**]

- **Recurrent Back-Projection Network for Video Super-Resolution** <Br>
[Muhammad Haris](https://alterzero.github.io/), [Greg Shakhnarovich](https://ttic.uchicago.edu/~gregory/), [Norimichi Ukita](https://www.toyota-ti.ac.jp/Lab/Denshi/iim/ukita/) <Br>
[ECCV 2020] [[Project](https://alterzero.github.io/projects/RBPN.html)] [[Pytorch-Code](https://github.com/alterzero/RBPN-PyTorch)]<Br>
[**RBPN**] [★☆] 视频超分, 使用DBPN中的back-projection结构利用前n帧信息完成对当前帧的空间超分.

- **Learning Temporal Coherence via Self-Supervision for GAN-based Video Generation** <Br>
[Mengyu Chu](https://people.mpi-inf.mpg.de/~mchu/), You Xie, Laura Leal-Taixe, [Nils Thuerey](https://ge.in.tum.de/) <Br>
[SIGGRAPH 2020] [[TF-Code](https://github.com/thunil/TecoGAN)]<Br>
[**TecoGAN**] [★★] 提出时空一致性的GAN和一个ping-pong loss保持long term时间一致性
	
- **Efficient Video Super-Resolution through Recurrent Latent Space Propagation** <Br>
Dario Fuoli, [Shuhang Gu](https://shuhanggu.github.io/), [Radu Timofte](https://people.ee.ethz.ch/~timofter/) <Br>
[ICCVW 2019] [[Pytorch-Code](https://github.com/dariofuoli/RLSP)]<Br>
[**RLSP**] [★] 用RNN做视频超分, 使用残差和pixel shuffle.
	
- **Deep Video Super-Resolution Network Using Dynamic Upsampling Filters Without Explicit Motion Compensation** <Br>
 [Younghyun Jo](https://yhjo09.github.io/), [Seoung Wug Oh](https://sites.google.com/view/seoungwugoh), Jaeyeon Kang, [Seon Joo Kim](https://sites.google.com/site/seonjookim/) <Br>
[CVPR 2018] [[Pytorch-Code](https://github.com/yhjo09/VSR-DUF0)]<Br>
[**DUF**]	
	
	
	
	
# Frame Interpolation
- **AMT: All-Pairs Multi-Field Transforms for Efficient Frame Interpolation** <Br>
[Zhen Li](https://paper99.github.io/), [Zuo-Liang Zhu](https://nk-cs-zzl.github.io/), Ling-Hao Han, [Qibin Hou](https://houqb.github.io/), Chun-Le Guo, [Ming-Ming Cheng](https://mmcheng.net/cmm/) <Br>
[CVPR 2023] [[Project](https://nk-cs-zzl.github.io/projects/amt/index.html)] [[Pytorch-Code](https://github.com/MCG-NKU/AMT)]<Br>

- **BiFormer: Learning Bilateral Motion Estimation via Bilateral Transformer for 4K Video Frame Interpolation** <Br>
Junheum Park, Jintae Kim, Chang-Su Kim<Br>
[CVPR 2023] [[Pytorch-Code](https://github.com/JunHeum/BiFormer)]<Br>

- **A Unified Pyramid Recurrent Network for Video Frame Interpolation** <Br>
Xin Jin, Longhai Wu, Jie Chen, Youxin Chen, Jayoon Koo, Cheul-hee Hahm <Br>
[CVPR 2023] [[Pytorch-Code](https://github.com/srcn-ivl/upr-net)]<Br>

- **Extracting Motion and Appearance via Inter-Frame Attention for Efficient Video Frame Interpolation** <Br>
Guozhen Zhang, Yuhan Zhu, Haonan Wang, Youxin Chen, [Gangshan Wu](http://mcg.nju.edu.cn/member/gswu/en/index.html), [Limin Wang](http://wanglimin.github.io/) <Br>
[CVPR 2023] [[Pytorch-Code](https://github.com/MCG-NJU/EMA-VFI)]<Br>
[**EMA-VFI**]

- **Beyond a Video Frame Interpolator: A Space Decoupled Learning Approach to Continuous Image Transition** <Br>
[Tao Yang](https://cg.cs.tsinghua.edu.cn/people/~tyang/), Peiran Ren, Xuansong Xie, Xiansheng Hua, [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
[arXiv 2203] [[Pytorch-Code](https://github.com/yangxy/sdl)]<Br>
[**SDL**]

- **FILM: Frame Interpolation for Large Motion** <Br>
Fitsum Reda, Janne Kontkanen, [Eric Tabellion](http://www.tabellion.org/et/), [Deqing Sun](https://deqings.github.io/), Caroline Pantofaru, [Brian Curless](https://homes.cs.washington.edu/~curless/) <Br>
[ECCV 2022] [[Project](https://film-net.github.io/)] [[TF2-Code](https://github.com/google-research/frame-interpolation)]<Br>
[★★] end-to-end的插帧网络, 使用类似PWCNet的多尺度flow预测结构, 特征提取部分使用共享权值对图像金字塔提特征, 首次使用gram matrix loss, 使生成帧更清晰. 网络结构很简单明了, 但效果很好, 训练和模型设计的细节应该是功不可没.

- **Enhancing Deformable Convolution based Video Frame Interpolation with Coarse-to-fine 3D CNN** <Br>
[Duolikun Danier](https://danielism97.github.io/), [Fan Zhang](https://fan-aaron-zhang.github.io/), [David Bull](https://david-bull.github.io/) <Br>
[arXiv 2202] [[Pytorch-Code](https://github.com/danielism97/EDC)]<Br>
[**EDC**]

- **A Subjective Quality Study for Video Frame Interpolation** <Br>
[Duolikun Danier](https://danielism97.github.io/), [Fan Zhang](https://fan-aaron-zhang.github.io/), [David Bull](https://david-bull.github.io/) <Br>
[arXiv 2202] [[Project](https://danielism97.github.io/BVI-VFI/)] <Br>
[**BVI-VFI**]

- **Splatting-based Synthesis for Video Frame Interpolation** <Br>
[Simon Niklaus](http://sniklaus.com/welcome), [Ping Hu](http://cs-people.bu.edu/pinghu/homepage.html), [Jiawen Chen](http://people.csail.mit.edu/jiawen/) <Br>
[arXiv 2201] <Br>

- **Deep Bayesian Video Frame Interpolation** <Br>
Zhiyang Yu, [Yu Zhang](https://zhangyulb.github.io/), Xujie Xiang, Dongqing Zou, Xijun Chen, [Jimmy S. Ren](http://www.jimmyren.com/) <Br>
[ECCV 2022] [[Pytorch-Code](https://github.com/Oceanlib/DBVI)]<Br>
[**DBVI**]

- **IFRNet: Intermediate Feature Refine Network for Efficient Frame Interpolation** <Br>
Lingtong Kong, [Boyuan Jiang](https://byjiang.com/), Donghao Luo, Wenqing Chu, Xiaoming Huang, [Ying Tai](https://tyshiwo.github.io/), Chengjie Wang, [Jie Yang](http://www.pami.sjtu.edu.cn/jieyang) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/ltkong218/IFRNet)]<Br

- **ST-MFNet: A Spatio-Temporal Multi-Flow Network for Frame Interpolation** <Br>
[Duolikun Danier](https://danielism97.github.io/), [Fan Zhang](https://fan-aaron-zhang.github.io/), [David Bull](https://david-bull.github.io/) <Br>
[CVPR 2022] [[Project](https://danielism97.github.io/ST-MFNet/)] [[Pytorch-Code](https://github.com/danielism97/st-mfnet)]<Br>
	
- **Real-time Spatial Temporal Transformer** <Br>
[Zhicheng Geng](https://zhichenggeng.com/), Luming Liang, [Tianyu Ding](https://www.tianyuding.com/), Ilya Zharkov <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/llmpass/RSTT)]<Br>
[**RSTT**]

- **Video Frame Interpolation Transformer** <Br>
Zhihao Shi, [Xiangyu Xu](https://sites.google.com/view/xiangyuxu), [Xiaohong Liu](https://jhc.sjtu.edu.cn/~xiaohongliu/), [Jun Chen](https://www.ece.mcmaster.ca/~junchen/), [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/zhshi0816/Video-Frame-Interpolation-Transformer)]<Br>
	
- **Many-to-many Splatting for Efficient Video Frame Interpolation** <Br>
[Ping Hu](http://cs-people.bu.edu/pinghu/homepage.html), [Simon Niklaus](https://sniklaus.com/welcome), [Stan Sclaroff](https://www.cs.bu.edu/fac/sclaroff/), [Kate Saenko](http://ai.bu.edu/ksaenko.html) <Br>
[CVPR 2022] [[Code](https://github.com/feinanshan/m2m_vfi)]<Br>
[**M2M**] [★★] 首先用off-the-shell model预测0->1/1->0的光流, 再通过motion refinement network预测N个光流图及置信度map, 最后利用N个光流进行forward warp并fuse结果. 使用Low-rank Feature Modulation加强光流的低秩约束.

- **DeMFI: Deep Joint Deblurring and Multi-Frame Interpolation with Flow-Guided Attentive Correlation and Recursive Boosting** <Br>
[Jihyong Oh](https://sites.google.com/view/ozbro/%ED%99%88), [Munchurl Kim](https://www.viclab.kaist.ac.kr/) <Br>
[arXiv 2111] [[Pytorch-Code](https://github.com/JihyongOh/DeMFI)]<Br>
	
- **EA-Net: Edge-Aware Network for Flow-based Video Frame Interpolation** <Br>
Bin Zhao, Xuelong Li <Br>
[arXiv 2105] <Br>
[★] 基于光流的插帧, 加入了edge信息

- **Asymmetric Bilateral Motion Estimation for Video Frame Interpolation** <Br>
Junheum Park, [Chul Lee](http://cilab.dongguk.edu/), [Chang-Su Kim](http://mcl.korea.ac.kr/) <Br>
[ICCV 2021] [[Pytorch-Code](https://github.com/junheum/abme)]<Br>
[**ABME**] [★] 先大致估计t->0, t->1的光流, 生成初始It, 再refine光流和生成帧

- **Revisiting Adaptive Convolutions for Video Frame Interpolation** <Br>
[Simon Niklaus](http://sniklaus.com/welcome), [Long Mai](http://mai-t-long.com/), [Oliver Wang](https://oliverwang.nfshost.com/) <Br>
[WACV 2021] [[Pytorch-Code](https://github.com/sniklaus/revisiting-sepconv)]<Br>
[**SepConv++**] [★] 使用adaptive conv做插帧, 在sepconv的基础上提出了一些trick. 要点为: 1.预测x和y方向的conv kernel; 2.在预测kernel时不padding; 3.输入两帧一起逐channel归一化到0均值单位方差; 4. 对kernel做norm; 5.使用VGG loss
	
- **XVFI: eXtreme Video Frame Interpolation** <Br>
Hyeonjun Sim, [Jihyong Oh](https://sites.google.com/view/ozbro/%ED%99%88), Munchurl Kim <Br>
[ICCV 2021 Oral] [[Pytorch-Code](https://github.com/JihyongOh/XVFI)]<Br>
[★★] 1. 提出了一个4K, 1000fps的插帧数据集; 2. 提出一个共享参数的多尺度插帧网络, 通过调整预测的scale级数, 处理不同分辨率和偏移.

- **FLAVR: Flow-Agnostic Video Representations for Fast Frame Interpolation** <Br>
[Tarun Kalluri](https://tarun005.github.io/), [Deepak Pathak](https://www.cs.cmu.edu/~dpathak/), [Manmohan Chandraker](http://cseweb.ucsd.edu/~mkchandraker/), [Du Tran](https://dutran.github.io/)    <Br>
[CVPR 2021] [[Project](https://tarun005.github.io/FLAVR/)] [[Pytorch-Code](https://github.com/tarun005/FLAVR)]<Br>
[★★] 首次提出用3D卷积做视频插帧, 结构为UNet, 输入为前后四帧, 输出为需要插的k-1帧

- **CDFI: Compression-Driven Network Design for Frame Interpolation** <Br>
[Tianyu Ding](https://www.tianyuding.com/), Luming Liang, [Zhihui Zhu](http://mysite.du.edu/~zzhu61/index.html), Ilya Zharkov    <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/tding1/CDFI)]<Br>
[★] 通过加入L1正则引入稀疏性, 然后将模型输入层数逐次减小, 得到压缩后的模型. 论文中表示压缩后的结构更合理, from scratch训练该网络就能得到与大模型相近的性能. 之后在小模型上加入了一些改进模块, 进一步提高了精度

- **Deep Animation Video Interpolation in the Wild** <Br>
Li Siyao, Shiyu Zhao, Weijiang Yu, Wenxiu Sun, [Dimitris N. Metaxas](https://www.cs.rutgers.edu/~dnm/), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/), [Ziwei Liu](https://liuziwei7.github.io/)    <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/lisiyao21/AnimeInterp/)]<Br>
[**AnimeInterp**] [★] 动画的插帧, 针对动画纹理平滑和位移大的特点, 设计了segment匹配模块和coarse-to-fine的光流匹配模块.

- **RIFE: Real-Time Intermediate Flow Estimation for Video Frame Interpolation** <Br>
[Zhewei Huang](https://github.com/hzwer), [Tianyuan Zhang](http://tianyuanzhang.com/), Wen Heng, [Boxin Shi](http://ci.idm.pku.edu.cn/), [Shuchang Zhou](https://zsc.github.io/) <Br>
[arXiv 2011] [[Pytorch-Code](https://github.com/hzwer/arXiv2020-RIFE)] [[Software](https://github.com/YiWeiHuang-stack/Squirrel-RIFE)]<Br>
[★★] 使用一个coarse-to-fine的网络IFNet预测f1,f2到t时刻的光流, 融合部分使用网络预测fusion map和residual. 为更好训练光流, 使用leakage distillation的方法, 先用一训练好的大网络预测中间光流的值.

- **Channel Attention Is All You Need for Video Frame Interpolation** <Br>
[Myungsub Choi](https://myungsub.github.io/), Heewon Kim, [Bohyung Han](https://cv.snu.ac.kr/index.php/~bhhan/), Ning Xu, [Kyoung Mu Lee](https://cv.snu.ac.kr/index.php/~kmlee/) <Br>
[AAAI 2020] [[Project](https://myungsub.github.io/CAIN/)] [[Pytorch-Code](https://github.com/myungsub/CAIN)]<Br>
[**CAIN**] [★★] 设计了一个pixelshuffle + attention residual block的网络, 无需光流估计和warp操作.

- **Video Frame Interpolation Via Residue Refinement** <Br>
Haopeng Li, Yuan Yuan, [Qi Wang](http://crabwq.github.io/#top) <Br>
[ICASSP  2020] [[Pytorch-Code](https://github.com/HopLee6/RRIN)]<Br>
[**RRIN**] [★] 残差和UNet结构预测光流, warp, refine

- **BMBC: Bilateral Motion Estimation with Bilateral Cost Volume for Video Interpolation** <Br>
Junheum Park, Keunsoo Ko, [Chul Lee](http://cilab.dongguk.edu/), [Chang-Su Kim](http://mcl.korea.ac.kr/) <Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/JunHeum/BMBC)]<Br>
[**BMBC**] [★] 基于光流的插帧, 提出了用中间光流值取得前后帧的feature组成bilateral cost volume

- **All at Once: Temporally Adaptive Multi-Frame Interpolation with Advanced Motion Modeling** <Br>
Zhixiang Chi, Rasoul Mohammadi Nasiri, Zheng Liu, [Juwei Lu](https://www.dsp.utoronto.ca/juwei/), Jin Tang, [Konstantinos N Plataniotis](https://www.comm.utoronto.ca/~kostas/) <Br>
[ECCV 2020] [[Project](https://chi-chi-zx.github.io/all-at-once/)] [[Code](https://github.com/chi-chi-zx/all-at-once)]<Br>
[★] 1.使用三次多项式对光流建模; 2.用temporal pyramidal形式, 有易到难逐次估计t1/t7->t2/t6->t3/t5->t4; 3. 估计光流时, 使用relaxed loss, 即允许估计的光流有小范围误差

- **Enhanced Quadratic Video Interpolation** <Br>
Yihao Liu, Liangbin Xie, Li Siyao, Wenxiu Sun, Yu Qiao, Chao Dong <Br>
[ECCVW 2020] [[Pytorch-Code](https://github.com/lyh-18/EQVI)]<Br>
[**EQVI**] [★] 1.用最小二乘计算quadratic光流; 2.用resnet18提取的contextual特征和原图一起预测残差; 3.对两个尺度的输入用相同网络处理, 并用一个fusion net预测map进行融合

- **Video Frame Interpolation without Temporal Priors** <Br>
 Youjian Zhang, [Chaoyue Wang](https://wang-chaoyue.github.io/), [Dacheng Tao](https://www.sydney.edu.au/engineering/about/our-people/academic-staff/dacheng-tao.html) <Br>
[NeurIPS 2020] [[Pytorch-Code](https://github.com/yjzhang96/UTI-VFI)]<Br>
[**UTI-VFI**] [★] 用残差网络先从模糊帧中预测清晰的起始和结束关键帧, 再用二次光流refine

- **Softmax Splatting for Video Frame Interpolation** <Br>
 [Simon Niklaus](http://sniklaus.com/welcome), [Feng Liu](http://web.cecs.pdx.edu/~fliu/) <Br>
[CVPR 2020] [[Pytorch-Code](https://github.com/sniklaus/softmax-splatting)]<Br>
[**SoftSplat**] [★☆] 使用前向光流warp的插帧, 大致浏览, 效果不错. 主要创新点为使用I0和I1_warp的亮度一致性作为权重Z, 并用一网络refine Z, 最后在融合时使用exp保证了尺度不变性(此处是从深度图作为Z来论述的).

- **Scene-Adaptive Video Frame Interpolation via Meta-Learning** <Br>
 [Myungsub Choi](https://myungsub.github.io/), Janghoon Choi, [Sungyong Baik](https://baiksung.github.io/), [Tae Hyun Kim](https://sites.google.com/site/lliger9/), [Kyoung Mu Lee](https://cv.snu.ac.kr/index.php/~kmlee/) <Br>
[CVPR 2020] [[Project](https://myungsub.github.io/meta-interpolation/)] [[Pytorch-Code](https://github.com/myungsub/meta-interpolation)]<Br>
[**Meta Interpolation**]

- **FeatureFlow: Robust Video Interpolation via Structure-to-Texture Generation** <Br>
Shurui Gui, [Chaoyue Wang](https://wang-chaoyue.github.io/), Qihua Chen, [Dacheng Tao](https://www.sydney.edu.au/engineering/about/our-people/academic-staff/dacheng-tao.html) <Br>
[CVPR 2020] [[Pytorch-Code](https://github.com/CM-BF/FeatureFlow)]<Br>
[★] 首先, 根据两帧输入图像和edge, 预测中间帧的structure图; 然后设计了一个texture compensator生成纹理细节. 网络用deformable conv做插帧和纹理补偿.

- **Blurry Video Frame Interpolation** <Br>
[Wang Shen](https://sites.google.com/view/wangshen94), [Wenbo Bao](https://sites.google.com/view/wenbobao/home), [Guangtao Zhai](https://faculty.sjtu.edu.cn/zhaiguangtao/en/index.htm), Li Chen, [Xiongkuo Min](https://sites.google.com/site/minxiongkuo/home), Zhiyong Gao<Br>
[CVPR 2020 Oral] [[Pytorch-Code](https://github.com/laomao0/BIN)]<Br>
[**BIN**] [★] 空间采用金字塔型结构, 逐层利用多帧信息, 为保证帧间一致性, 使用了ConvLSTM挖掘temporal关系

- **AdaCoF: Adaptive Collaboration of Flows for Video Frame Interpolation** <Br>
[Hyeongmin Lee](https://hyeongminlee.github.io/), [Taeoh Kim](https://taeoh-kim.github.io/), Tae-young Chung, Daehyun Pak, Yuseok Ban, Sangyoun Lee <Br>
[CVPR 2020] [[Pytorch-Code](https://github.com/HyeongminLEE/AdaCoF-pytorch)]<Br>
	
- **Deep Slow Motion Video Reconstruction with Hybrid Imaging System** <Br>
[Avinash Paliwal](http://people.tamu.edu/~avinashpaliwal/), [Nima Kalantari](https://people.engr.tamu.edu/nimak/index.html) <Br>
[TPAMI 2020] [[Project](https://people.engr.tamu.edu/nimak/Papers/ICCP2020_Slomo/index.html)] [[Pytorch-Code](https://github.com/avinashpaliwal/Deep-SloMo)]<Br>
[**Deep-SloMo**]

- **Robust Video Frame Interpolation With Exceptional Motion Map** <Br>
 Minho Park, [Hak Gu Kim](https://haku0331.wixsite.com/hakgukim), [Sangmin Lee](https://sites.google.com/view/sangmin-lee), [Yong Man Ro](http://ivylab.kaist.ac.kr/default/) <Br>
[TCSVT 2020] <Br>
	
- **ALANET: Adaptive Latent Attention Network for Joint Video Deblurring and Interpolation** <Br>
[Akash Gupta](https://akashagupta.com/), [Abhishek Aich](https://abhishekaich27.github.io/), [Amit K. Roy-Chowdhury](https://vcg.engr.ucr.edu/amit) <Br>
[MM 2020] [[Project](https://akashagupta.com/ALANET.html)] [[Code](https://github.com/agupt013/ALANET)]<Br>
[★] 用帧内和帧间attention做去模糊和插帧
	
- **Depth-Aware Video Frame Interpolation** <Br>
[Wenbo Bao](https://sites.google.com/view/wenbobao/home), [Wei-Sheng Lai](http://graduatestudents.ucmerced.edu/wlai24/), [Chao Ma](https://vision.sjtu.edu.cn/), Xiaoyun Zhang, Zhiyong Gao, [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/)  <Br>
[CVPR 2019] [[Project](https://sites.google.com/view/wenbobao/dain)] [[Pytorch-Code](https://github.com/baowenbo/DAIN)]<Br>
[**DAIN**] [★★☆]

- **Unsupervised Video Interpolation using Cycle Consistency** <Br>
Fitsum A. Reda, Deqing Sun, Aysegul Dundar, Mohammad Shoeybi, [Guilin Liu](https://liuguilin1225.github.io/), Kevin J. Shih, Andrew Tao, [Jan Kautz](http://jankautz.com/), [Bryan Catanzaro](http://catanzaro.name/)  <Br>
[ICCV 2019] [[Project](https://nv-adlr.github.io/publication/2019-UnsupervisedVideoInterpolation)] [[Pytorch-Code](https://github.com/NVIDIA/unsupervised-video-interpolation)]<Br>

- **IM-Net for High Resolution Video Frame Interpolationn** <Br>
Tomer Peleg, Pablo Szekely, Doron Sabo, [Omry Sendik](https://omrysendik.github.io/)  <Br>
[CVPR 2019] [[Project](https://sites.google.com/view/wenbobao/dain)] [[Pytorch-Code](https://github.com/baowenbo/DAIN)]<Br>
[★] 预测motion field vector(光流)和occlusion map做插帧

- **Quadratic video interpolation** <Br>
[Xiangyu Xu](https://sites.google.com/view/xiangyuxu), Siyao Li, Wenxiu Sun, Qian Yin, [Ming-Hsuan Yang](https://scholar.google.com/citations?user=p9-ohHsAAAAJ&hl=zh-CN&oi=sra)   <Br>
[NeurIPS 2019] [[Project](https://sites.google.com/view/xiangyuxu/qvi_nips19)] [[Pytorch-Code](https://github.com/xuxy09/QVI)]<Br>
[**QVI**] [★] 利用-1,0,1三帧的信息对光流进行二次插值

- **Deep Video Frame Interpolation using Cyclic Frame Generation** <Br>
[Yu-Lun Liu](http://www.cmlab.csie.ntu.edu.tw/~yulunliu/), [Yi-Tung Liao](http://www.cmlab.csie.ntu.edu.tw/~queenieliaw/), [Yen-Yu Lin](https://www.citi.sinica.edu.tw/pages/yylin/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/)   <Br>
[[Project](https://www.cmlab.csie.ntu.edu.tw/~yulunliu/CyclicGen)] [[TF-Code](https://github.com/alex04072000/CyclicGen)]<Br>
[**CyclicGen**] [★☆] 用2个预测帧预测输入帧, 作为consistency loss, 提高生成帧的质量. 另外提出了光流线性约束loss, 并将边缘信息加入到输入中

- **MEMC-Net: Motion Estimation and Motion Compensation Driven Neural Network for Video Interpolation and Enhancement** <Br>
[Wenbo Bao](https://sites.google.com/view/wenbobao/home), [Wei-Sheng Lai](http://graduatestudents.ucmerced.edu/wlai24/), Xiaoyun Zhang, Zhiyong Gao, [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/)    <Br>
[TPAMI 2019] [[Project](https://sites.google.com/view/wenbobao/memc-net)] [[Pytorch-Code](https://github.com/baowenbo/MEMC-Net)]<Br>
[★★] 提出一个自适应warping layer, 将warping中简单的bilinear操作改为学习的插值kernel与双线性核相结合的操作

- **Super SloMo: High Quality Estimation of Multiple Intermediate Frames for Video Interpolation** <Br>
[Huaizu Jiang](http://jianghz.me/), [Deqing Sun](https://deqings.github.io/), [Varun Jampani](https://varunjampani.github.io/), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/), [Erik Learned-Miller](https://people.cs.umass.edu/~elm/), [Jan Kautz](https://jankautz.com/)  <Br>
[CVPR 2018] [[Project](https://github.com/avinashpaliwal/Super-SloMo)] [[Pytorch-Code](http://jianghz.me/projects/superslomo/)]<Br>
[★☆] 视频插帧. 首先预测双向光流, 接下来在每个要插值的时刻t, 用一个网络refine光流并预测visibility map, 最后根据光流和visibility map插值生成t时刻图像.

- **Context-aware Synthesis for Video Frame Interpolation** <Br>
[Simon Niklaus](http://sniklaus.com/welcome), [Feng Liu](http://web.cecs.pdx.edu/~fliu/) <Br>
[CVPR 2018] [[Project](http://web.cecs.pdx.edu/~fliu/project/adaconv/)] <Br>
	
- **Video Frame Interpolation via Adaptive Separable Convolution** <Br>
[Simon Niklaus](http://sniklaus.com/welcome), Long Mai, [Feng Liu](http://web.cecs.pdx.edu/~fliu/) <Br>
[ICCV 2017] [[Project](http://web.cecs.pdx.edu/~fliu/project/sepconv/)] [[Pytorch-Code](https://github.com/sniklaus/sepconv-slomo)]<Br>
[**sepconv-slomo**]

- **Video Frame Interpolation via Adaptive Convolution** <Br>
[Simon Niklaus](http://sniklaus.com/welcome), Long Mai, [Feng Liu](http://web.cecs.pdx.edu/~fliu/) <Br>
[CVPR 2017] [[Project](http://web.cecs.pdx.edu/~fliu/project/adaconv/)] <Br>
[**adaconv-slomo**]
	
	
	
	
# Video Enhancement and Restoration
- **Recurrent Video Restoration Transformer with Guided Deformable Attention** <Br>
[Jingyun Liang](https://jingyunliang.github.io/), [Yuchen Fan](https://ychfan.github.io/), [Xiaoyu Xiang](https://engineering.purdue.edu/people/xiaoyu.xiang.1), Rakesh Ranjan, [Eddy Ilg](https://cvmp.cs.uni-saarland.de/), Simon Green, [Jiezhang Cao](https://www.jiezhangcao.com/), [Kai Zhang](https://cszn.github.io/), [Radu Timofte](http://people.ee.ethz.ch/~timofter/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html)  <Br>
[NeurlPS 2022] [[Pytorhc-Code](https://github.com/JingyunLiang/RVRT)] <Br>
[**RVRT**]

- **Context-Aware Video Reconstruction for Rolling Shutter Cameras** <Br>
[Bin Fan](https://gitcvfb.github.io/), [Yuchao Dai](http://npu-cvr.cn/), Zhiyuan Zhang, Qi Liu, Mingyi He <Br>
[CVPR 2022] [[Code](https://github.com/GitCVfb/CVR)] <Br>
[**CVR**]

- **Neural Global Shutter: Learn to Restore Video from a Rolling Shutter Camera with Global Reset Feature** <Br>
[Zhixiang Wang](https://lightchaserx.github.io/), Xiang Ji, Jia-Bin Huang, [Shin'ichi Satoh](http://www.satoh-lab.nii.ac.jp/), Xiao Zhou, Yinqiang Zheng <Br>
[CVPR 2022] [[Code](https://github.com/lightChaserX/neural-global-shutter)] <Br>

- **Bringing Old Films Back to Life** <Br>
[Ziyu Wan](http://raywzy.com/), [Bo Zhang](https://bo-zhang.me/), [Dongdong Chen](http://www.dongdongchen.bid/), [Jing Liao](https://liaojing.github.io/html/) <Br>
[CVPR 2022] [[Project](http://raywzy.com/Old_Film/)] <Br>

- **Revisiting Temporal Alignment for Video Restoration** <Br>
Kun Zhou, [Wenbo Li](https://fenglinglwb.github.io/), Liying Lu, Xiaoguang Han, [Jiangbo Lu](https://sites.google.com/site/jiangbolu/) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/redrock303/Revisiting-Temporal-Alignment-for-Video-Restoration)] <Br>

- **VRT: A Video Restoration Transformer** <Br>
[Jingyun Liang](https://jingyunliang.github.io/), [Jiezhang Cao](https://www.jiezhangcao.com/), [Yuchen Fan](https://ychfan.github.io/), [Kai Zhang](https://cszn.github.io/), Rakesh Ranjan, [Yawei Li](https://ofsoundof.github.io/), [Radu Timofte](http://people.ee.ethz.ch/~timofter/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html) <Br>
[arXiv 2201] [[Pytorch-Code](https://github.com/JingyunLiang/VRT)] <Br>
	
- **Learning Temporal Consistency for Low Light Video Enhancement from Single Images** <Br>
Fan Zhang, [Yu Li](https://yu-li.github.io/), [Shaodi You](https://youshaodi.github.io/), Ying Fu <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/zkawfanx/StableLLVE)]**
[★☆] 训练时, 对图像做分割并预测前景的随机光流, 计算warp后图像和原图像处理结果的consistency loss, 加强时间一致性, 另外在生成训练样本时, 加入了一些noise.

- **EDVR: Video Restoration with Enhanced Deformable Convolutional Networks** <Br>
 [Xintao Wang](https://xinntao.github.io/), [Kelvin C.K. Chan](https://ckkelvinchan.github.io/), [Ke Yu](https://yuke93.github.io/), Chao Dong, [Chen Change Loy](https://www.mmlab-ntu.com/person/ccloy/) <Br>
[CVPRW 2019] [[Project](https://xinntao.github.io/projects/EDVR)] [[Pytorch-Code](https://github.com/xinntao/EDVR)] <Br>

- **Learning to See Moving Objects in the Dark** <Br>
 Haiyang Jiang, Yinqiang Zheng <Br>
[ICCV 2019] [[TF-Code](https://github.com/MichaelHYJiang/Learning-to-See-Moving-Objects-in-the-Dark)] <Br>
[★★] 提供了一个暗光视频增强数据集, 通过设计camera system, 获取对齐的亮暗视频对. 设计一个基于3DUnet的网络.

- **Seeing Motion in the Dark** <Br>
[Chen Chen](http://cchen156.web.engr.illinois.edu/), [Qifeng Chen](http://cqf.io/), [Minh N. Do](http://minhdo.ece.illinois.edu/), [Vladlen Koltun](http://vladlen.info/) <Br>
[ICCV 2019] [[TF-Code](https://github.com/cchen156/Seeing-Motion-in-the-Dark)] <Br>
[★☆] 对一组静态的视频帧做亮度增强, 使用Deep Siamese Network, 增强帧间一致性.
	



# Video Stabilization
- **Deep Online Fused Video Stabilization** <Br>
 [Zhenmei Shi](http://pages.cs.wisc.edu/~zhmeishi/), [Fuhao Shi](http://fuhaoshi.com/), [Wei-Sheng Lai](http://graduatestudents.ucmerced.edu/wlai24/), [Chia-Kai Liang](http://chiakailiang.org/), [Yingyu Liang](http://pages.cs.wisc.edu/~yliang/) <Br>
[arXiv 2102] [[Project](https://zhmeishi.github.io/dvs/)] [[Pytorch-Code](https://github.com/googleinterns/deep-stabilization)] <Br>










# Video Debluring
- **Deep Discriminative Spatial and Temporal Network for Efficient Video Deblurring** <Br>
[Jinshan Pan](https://jspan.github.io/)], Boming Xu, Jiangxin Dong, Jianjun Ge, [Jinhui Tang](https://imag-njust.net/) <Br>
[CVPR 2023] [[Pytorch-Code](https://github.com/xuboming8/DSTNet)]<Br>
[**DSTNet**]

- **Multi-Scale Memory-Based Video Deblurring** <Br>
Bo Ji, [Angela Yao](https://www.comp.nus.edu.sg/~ayao/) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/jibo27/MemDeblur)]<Br>

- **DeFMO: Deblurring and Shape Recovery of Fast Moving Objects** <Br>
Denys Rozumnyi, Martin R. Oswald, Vittorio Ferrari, Jiri Matas, Marc Pollefeys<Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/rozumden/DeFMO)]<Br>
[★] 从单张模糊图像和背景图中恢复t张清晰的图像, 网络结构为一个encoder+t个renderers, 采用了几个loss分别用于处理目标外观, sharpness及空间一致性等.
	
- **ARVo: Learning All-Range Volumetric Correspondence for Video Deblurring** <Br>
Dongxu Li, Chenchen Xu, [Kaihao Zhang](https://zhangkaihao.github.io/), [Xin Yu](https://sites.google.com/view/xinyus-homepage/Home), [Yiran Zhong](https://yiranzhong.com/), [Wenqi Ren](https://sites.google.com/site/renwenqi888/home), [Hanna Suominen](https://researchers.anu.edu.au/researchers/suominen-h), Hongdong Li<Br>
[CVPR 2021] [[Project](https://baihaoran.xyz/projects/cdvd-tsp/index.html)] [[Pytorch-Code](https://github.com/csbhr/CDVD-TSP)]<Br>

- **Learning Event-Driven Video Deblurring and Interpolation** <Br>
Songnan Lin, [Jiawei Zhang](https://sites.google.com/site/zhjw1988), [Jinshan Pan](https://jspan.github.io/), Zhe Jiang, Dongqing Zou, Yongtian Wang, Jing Chen, [Jimmy Ren](http://www.jimmyren.com/) <Br>
[ECCV 2020] <Br>

- **Efficient Spatio-Temporal Recurrent Neural Network for Video Deblurring** <Br>
Zhihang Zhong, Ye Gao, Yinqiang Zheng, [Bo Zheng](http://www.bozheng-lab.com/) <Br>
[ECCV 2020 Spotlight] [[Pytorch-Code](https://github.com/zzh-tech/ESTRNN)]<Br>
[**ESTRNN**]

- **Cascaded Deep Video Deblurring Using Temporal Sharpness Prior** <Br>
[Jinshan Pan](https://jspan.github.io/), [Haoran Bai](https://baihaoran.xyz/about), Jinhui Tang<Br>
[CVPR 2020] [[Project](https://baihaoran.xyz/projects/cdvd-tsp/index.html)] [[Pytorch-Code](https://github.com/csbhr/CDVD-TSP)]<Br>
[**CDVD-TSP**] [★☆] 使用光流将先后帧warp到当前帧, 和一个新提出的sharpness prior进行concat, 送入网络进行处理. 通过级联(2阶段)的方式提高精度.

- **Spatio-Temporal Filter Adaptive Network for Video Deblurring** <Br>
[Shangchen Zhou](https://shangchenzhou.com/), [Jiawei Zhang](https://sites.google.com/site/zhjw1988), [Jinshan Pan](https://jspan.github.io/), [Haozhe Xie](https://haozhexie.com/about), [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), [Jimmy Ren](http://www.jimmyren.com/) <Br>
[ICCV 2019] [[Project](https://www.shangchenzhou.com/projects/stfan/)] [[Pytorch-Code](https://github.com/sczhou/STFAN)]<Br>
[**STFAN**]


# Video Deraining
- **Semi-supervised Video Deraining with Dynamical Rain Generator**  <Br>
Zongsheng Yue, [Jianwen Xie](http://www.stat.ucla.edu/~jxie/), Qian Zhao, [Deyu Meng](http://gr.xjtu.edu.cn/web/dymeng/1) <Br>	
[CVPR 2021] [[Pytorch-Code](https://github.com/zsyOAOA/S2VD)]<Br>
[**S2VD**]


# Video Dehazing
- **Learning to Restore Hazy Video: A New Real-World Dataset and A New Method** <Br>
[Xinyi Zhang](https://sites.cs.ucsb.edu/~xyzhang/), Hang Dong, [Jinshan Pan](https://jspan.github.io/), Chao Zhu, [Ying Tai](https://tyshiwo.github.io/), Chengjie Wang, Jilin Li, Feiyue Huang, Fei Wang <Br>
[CVPR 2021] <Br>


# Video Deflicker
- **Blind Video Deflickering by Neural Filtering with a Flawed Atlas** <Br>
[Chenyang Lei](https://chenyanglei.github.io/), [Xuanchi Ren](https://xuanchiren.com/), [Zhaoxiang Zhang](https://zhaoxiangzhang.net/), [Qifeng Chen](https://cqf.io/) <Br>
[CVPR 2023] [[Project](https://chenyanglei.github.io/deflicker/)] [[Pytorch-Code](https://github.com/ChenyangLEI/All-in-one-Deflicker)]<Br>


# Video Inpainting
- **The DEVIL is in the Details: A Diagnostic Evaluation Benchmark for Video Inpainting** <Br>
[Ryan Szeto](http://ryanszeto.com/), [Jason J. Corso](http://web.eecs.umich.edu/~jjcorso/) <Br>
[CVPR 2022] [[Code]](https://github.com/MichiganCOG/devil)]

- **Towards An End-to-End Framework for Flow-Guided Video Inpainting** <Br>
[Zhen Li](https://paper99.github.io/), Cheng-Ze Lu, Jianhua Qin, Chun-Le Guo, [Ming-Ming Cheng](http://mmcheng.net/cmm/) <Br>
[CVPR 2022] [[Pytorch-Code]](https://github.com/MCG-NKU/E2FGVI)]
[**E2FGVI**]

- **Internal Video Inpainting by Implicit Long-range Propagation** <Br>
[Hao Ouyang](https://ken-ouyang.github.io/), [Tengfei Wang](https://tengfei-wang.github.io/), [Qifeng Chen](https://cqf.io/publication.html) <Br>
[ICCV 2021] [[Project](https://tengfei-wang.github.io/Implicit-Internal-Video-Inpainting/index.html)] [[Pytorch-Code]](https://github.com/Tengfei-Wang/Implicit-Internal-Video-Inpainting)]
[**IIVI**]

- **Progressive Temporal Feature Alignment Network for Video Inpainting** <Br>
Xueyan Zou, [Linjie Yang](https://sites.google.com/site/linjieyang89/), Ding Liu, [Yong Jae Lee](https://web.cs.ucdavis.edu/~yjlee/) <Br>
[CVPR 2021] [[Pytorch-Code]](https://github.com/MaureenZOU/TSAM)]
[**TSAM**]

- **Short-Term and Long-Term Context Aggregation Network for Video Inpainting** <Br>
[Ang Li](https://angliunimelb.github.io/), [Shanshan Zhao](https://sshan-zhao.github.io/), [Xingjun Ma](http://xingjunma.com/), [Mingming Gong](https://mingming-gong.github.io/), [Jianzhong Qi](https://people.eng.unimelb.edu.au/jianzhongq/), [Rui Zhang](http://www.ruizhang.info/), [Dacheng Tao](https://www.sydney.edu.au/engineering/about/our-people/academic-staff/dacheng-tao.html), [Ramamohanarao Kotagirig](http://www.cloudbus.org/rao/) <Br>
[ECCV 2020] <Br>

- **Learning Joint Spatial-Temporal Transformations for Video Inpainting**  <Br>
[Yanhong Zeng](https://sites.google.com/view/1900zyh), [Jianlong Fu](https://jianlong-fu.github.io/), Hongyang Chao <Br>
[ECCV 2020] [[Pytorch-Code]](https://github.com/researchmm/STTN)]
[**STTN**]

- **DVI: Depth Guided Video Inpainting for Autonomous Driving** <Br>
Miao Liao, Feixiang Lu, Dingfu Zhou, [Sibo Zhang](https://sites.google.com/view/sibozhang/home), Wei Li, [Ruigang Yang](http://www.vis.uky.edu/~ryang/) <Br>
[ECCV 2020] [[Project]](https://sites.google.com/view/sibozhang/dvi)] [[Code]](https://github.com/sibozhang/Depth-Guided-Inpainting)]


	
# Video Matting
- **VMFormer: End-to-End Video Matting with Transformer** <Br>
[Jiachen Li](https://chrisjuniorli.github.io/), [Vidit Goel](https://vidit98.github.io/), Marianna Ohanyan, Shant Navasardyan, [Yunchao Wei](https://weiyc.github.io/), [Humphrey Shi](https://www.humphreyshi.com/) <Br>
[arXiv 2205] [[Project]](https://chrisjuniorli.github.io/project/VMFormer/)] [[Pytorch-Code]](https://github.com/SHI-Labs/VMFormer)]<Br>

- **One-Trimap Video Matting** <Br>
[Hongje Seong](https://hongje.github.io/), [Seoung Wug Oh](https://sites.google.com/view/seoungwugoh), [Brian Price](https://www.brianpricephd.com/), [Euntai Kim](https://cilab.yonsei.ac.kr/), [Joon-Young Lee](https://joonyoung-cv.github.io/) <Br>
[ECCV 2022] [[Pytorch-Code]](https://github.com/Hongje/OTVM)] <Br>
[**OTVM**]

- **Human Instance Matting via Mutual Guidance and Multi-Instance Refinement** <Br>
Yanan Sun, Chi-Keung Tang, Yu-Wing Tai <Br>
[CVPR 2022 Oral] [[Pytorch-Code]](https://github.com/nowsyn/InstMatt)] <Br>
[**InstMatt**]

- **MatteFormer: Transformer-Based Image Matting via Prior-Tokens** <Br>
GyuTae Park, SungJoon Son, JaeYoung Yoo, SeHo Kim, [Nojun Kwak](http://mipal.snu.ac.kr/) <Br>
[CVPR 2022] [[Pytorch-Code]](https://github.com/webtoon/matteformer)] <Br>

- **Robust High-Resolution Video Matting with Temporal Guidance** <Br>
Shanchuan Lin, Linjie Yang, Imran Saleemi, [Soumyadip Sengupta](https://homes.cs.washington.edu/~soumya91/) <Br>
[WACV 2022] [[Project]](https://peterl1n.github.io/RobustVideoMatting/#/)] [[Pytorch-Code]](https://github.com/PeterL1n/RobustVideoMatting)] <Br>
轻量级视频matting, 效果不错. 用ConvGRU利用时域信息, 用Deep guided filter处理大图  <Br>
[**RVM**] [★★]

- **Deep Video Matting via Spatio-Temporal Alignment and Aggregation** <Br>
[Yanan Sun](https://georgegu1997.github.io/), [Guanzhi Wang](https://cs.stanford.edu/~guanzhi/), Qiao Gu, [Chi-Keung Tang](http://www.cse.ust.hk/~cktang/), [Yu-Wing Tai](https://www.cse.ust.hk/admin/people/faculty/profile/yuwing) <Br>
[CVPR 2021] <Br>
[**DVM**]
	

# Video Demoireing
- **Video Demoireing with Relation-Based Temporal Consistency** <Br>
Peng Dai, Xin Yu, Lan Ma, Baoheng Zhang, Jia Li, [Wenbo Li](https://fenglinglwb.github.io/), Jiajun Shen, [Xiaojuan Qi](https://xjqi.github.io/) <Br>
[CVPR 2022] [[Project]](https://daipengwa.github.io/VDmoire_ProjectPage/)] [[Pytorch-Code]](https://github.com/CVMI-Lab/VideoDemoireing)] <Br>



# Video Synthesis
- **GAN-Supervised Dense Visual Alignment** <Br>
[William Peebles](https://www.wpeebles.com/), [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/), [Richard Zhang](http://richzhang.github.io/), [Antonio Torralba](https://groups.csail.mit.edu/vision/torralbalab/), [Alexei A. Efros](http://people.eecs.berkeley.edu/~efros/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/) <Br>
[CVPR 2022 Oral] [[Project]](https://www.wpeebles.com/gangealing)] [[Pytorch-Code]](https://github.com/wpeebles/gangealing)] <Br>

- **Thin-Plate Spline Motion Model for Image Animation** <Br>
Jian Zhao, Hui Zhang <Br>
[CVPR 2022] [[Pytorch-Code]](https://github.com/yoyo-nb/Thin-Plate-Spline-Motion-Model)] <Br>

- **Make It Move: Controllable Image-to-Video Generation with Text Descriptions** <Br>
Yaosi Hu, [Chong Luo](https://www.microsoft.com/en-us/research/people/cluo/?from=http%3A%2F%2Fresearch.microsoft.com%2Fen-us%2Fpeople%2Fcluo%2F), Zhenzhong Chen<Br>
[CVPR 2022] [[Pytorch-Code]](https://github.com/Youncy-Hu/MAGE)] <Br>
[**MAGE**]

- **StyleGAN-V: A Continuous Video Generator with the Price, Image Quality and Perks of StyleGAN2** <Br>
[Ivan Skorokhodov](https://universome.github.io/), [Sergey Tulyakov](http://www.stulyakov.com/), [Mohamed Elhoseiny](http://www.mohamed-elhoseiny.com/) <Br>
[CVPR 2022] [[Project]](https://universome.github.io/stylegan-v)] [[Pytorch-Code]](https://github.com/universome/stylegan-v)] <Br>

- **Playable Environments: Video Manipulation in Space and Time** <Br>
[Willi Menapace](https://www.willimenapace.com/), [Stéphane Lathuilière](https://stelat.eu/), [Aliaksandr Siarohin](https://github.com/AliaksandrSiarohin), [Christian Theobalt](https://www.mpg.de/16583907/informatics-theobalt), [Sergey Tulyakov](http://www.stulyakov.com/), [Vladislav Golyanik](https://people.mpi-inf.mpg.de/~golyanik/), [Elisa Ricci](http://elisaricci.eu/) <Br>
[CVPR 2022] [[Pytorch-Code]](https://github.com/willi-menapace/PlayableEnvironments)] <Br>

- **Show Me What and Tell Me How: Video Synthesis via Multimodal Conditioning** <Br>
[Ligong Han](https://phymhan.github.io/), [Jian Ren](https://alanspike.github.io/), Hsin-Ying Lee, [Francesco Barbieri](https://fvancesco.github.io/), [Kyle Olszewski](https://kyleolsz.github.io/), [Shervin Minaee](https://sites.google.com/site/shervinminaee/home) <Br>
[CVPR 2022] [[Project]](https://snap-research.github.io/MMVID/)] [[Pytorch-Code]](https://github.com/snap-research/MMVID)] <Br>
[**MMVID**]

- **Attribute Group Editing for Reliable Few-shot Image Generation** <Br>
Guanqi Ding, Xinzhe Han, Shuhui Wang, Shuzhe Wu, Xin Jin, Dandan Tu, Qingming Huang <Br>
[CVPR 2022] [[Pytorch-Code]](https://github.com/UniBester/AGE)] <Br>
[**AGE**]



# Misc
- **AutoTransition: Learning to Recommend Video Transition Effects** <Br>
Yaojie Shen, Libo Zhang, Kai Xu, [Xiaojie Jin](https://airobotai.github.io/jinxiaojie/) <Br>
[ECCV 2022] [字节跳动] [[Pytorch-Code]](https://github.com/AcherStyx/AutoTransition)] <Br>
自动生成剪辑

- **ClothFormer: Taming Video Virtual Try-on in All Module** <Br>
Jianbin Jiang, Tan Wang, He Yan, Junhui Liu <Br>
[CVPR 2022 Oral] [[Project](https://cloth-former.github.io/)] [[Pytorch-Code]](https://github.com/luxiangju-PersonAI/ClothFormer)] <Br>

- **Single-frame Regularization for Temporally Stable CNNs** <Br>
[Gabriel Eilertsen](https://liu.se/en/employee/gabei62), [Rafał K. Mantiuk](https://www.cl.cam.ac.uk/~rkm38/), [Jonas Unger](https://weber.itn.liu.se/~jonun/web/Home.php) <Br>
[CVPR 2019] <Br>
[★☆] 提出增强视频帧间稳定性的一些正则loss, 包括Stability regularization(加入高斯噪声), Transform invariance regularization(几何变换), Sparse Jacobian regularization(梯度一致loss).

- **Blind Video Temporal Consistency** <Br>
[Nicolas Bonneel](https://perso.liris.cnrs.fr/nicolas.bonneel/), [James Tompkin](https://jamestompkin.com/), [Kalyan Sunkavalli](http://www.kalyans.org/), [Deqing Sun](https://deqings.github.io/), [Sylvain Paris](http://people.csail.mit.edu/sparis/), [Hanspeter Pfister](https://vcg.seas.harvard.edu/)  <Br>
[TOG 2015] [[Project](https://perso.liris.cnrs.fr/nicolas.bonneel/consistency/)] <Br>
[★] 内容和时域一致联合最小化, 适用于各种处理算子
