Face Restoration and Super-Resolution and other related topics. **Archived**

# Table of Contents
- [Face Restoration](#face-restoration)
- [Face SuperResolution](#face-superresolution)
- [Face Manipulation](#face-manipulation)
- [Others](#others)


# Face Restoration
- **VQFR: Blind Face Restoration with Vector-Quantized Dictionary and Parallel Decoder**  <Br>
[Yuchao Gu](https://ycgu.site/), [Xintao Wang](https://xinntao.github.io/), [Liangbin Xie](https://liangbinxie.github.io/), [Chao Dong](http://xpixel.group/]), Gen Li, Ying Shan, [Ming-Ming Cheng](https://mmcheng.net/cmm/) <Br>
[ECCV 2022 Oral] [[Project](https://ycgu.site/projects/vqfr/)] [[Pytorch-Code](https://github.com/TencentARC/VQFR)] <Br>

- **RestoreFormer: High-Quality Blind Face Restoration from Undegraded Key-Value Pairs**  <Br>
Zhouxia Wang, [Jiawei Zhang](https://sites.google.com/site/zhjw1988), [Runjian Chen](https://www.rjchen.site/), Wenping Wang, [Ping Luo](http://luoping.me/) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/wzhouxiff/RestoreFormer)] <Br>

- **Progressive Semantic-Aware Style Transformation for Blind Face Restoration** <Br>
[Chaofeng Chen](https://chaofengc.github.io), [Xiaoming Li](https://csxmli2016.github.io/), [Lingbo Yang](https://lotayou.github.io), [Xianhui Lin](https://dblp.org/pid/147/7708.html), [Lei Zhang](https://www4.comp.polyu.edu.hk/~cslzhang/), [Kwan-Yee K. Wong](https://i.cs.hku.hk/~kykwong/) <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/chaofengc/PSFRGAN)]  <Br>
[★] 用人脸图像和人脸解析结果预测scale和bias, 整体和SPADE的思路十分相似. 实测效果貌似不如HiFaceGAN.
	
- **GFP-GAN: Towards Real-World Blind Face Restoration with Generative Facial Prior**  <Br>
[Xintao Wang](https://xinntao.github.io/), [Yu Li](https://yu-li.github.io/), Honglun Zhang, Ying Shan <Br>
[CVPR 2021] [[Project](https://xinntao.github.io/projects/gfpgan)]  <Br>
[★] 用预训练的人脸GAN网络提取的特征作为先验, 一个UNet型网络作为degradation removal模块, 从该模块中提取空间特征, 并用SFT的思想结合到先验特征上. 对五官分别使用了判别器.

- **Blind Face Restoration via Deep Multi-scale Component Dictionaries** <Br>
[Xiaoming Li](https://csxmli2016.github.io/), [Chaofeng Chen](https://chaofengc.github.io/), [Shangchen Zhou](https://shangchenzhou.com/), Xianhui Lin, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), [Lei Zhang](https://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/csxmli2016/DFDNet)] <Br>
[★★] **(构建字典, 匹配最近邻特征)** 对眼睛鼻子嘴建立字典, inference时通过匹配最相似的feature找到相似的高清特征并做替换. 字典通过VGG网络提特征和聚类实现. 实测对五官的增强效果不错, 不过对于头发皮肤等部分效果不明显.

- **Enhanced Blind Face Restoration With Multi-Exemplar Images and Adaptive Spatial Feature Fusion**  <Br>
[Xiaoming Li](https://csxmli2016.github.io/), Wenyu Li, [Dongwei Ren](https://csdwren.github.io/), Hongzhi Zhang, Meng Wang, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo) <Br>
[CVPR 2020 Oral] [[Code](https://github.com/csxmli2016/ASFFNet)] <Br>
[★] **(基于同一张脸的exemplar做恢复)** 通过关键点从数张同一人的examplar图像中选出最相思的图像, 使用moving least-square和AdaIn进行空间和亮度的对齐, 提出了ASFF模块通过预测attention map将引导图和LR图的特征融合

- **HiFaceGAN: Face Renovation via Collaborative Suppression and Replenishment** <Br>
[Lingbo Yang](https://lotayou.github.io/), Chang Liu, Pan Wang, Shanshe Wang, Peiran Ren, Siwei Ma, Wen Gao <Br>
[MM 2020] [[Project](https://lotayou.github.io/projects/face_renov.html)] [[Pytorch-Code](https://github.com/Lotayou/Face-Renovation)]  <Br>
[★☆] 通过不同提取不同尺度的语义信息作为指导, 实现人脸修复, 对真实照片效果也还可以.

- **(CVPR 2018) Deep semantic face deblurring** <Br>
[Ziyi Shen](https://sites.google.com/site/ziyishenmi/), [Wei-Sheng Lai](https://www.wslai.net/) , Tingfa Xu, [Jan Kautz](https://jankautz.com/), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/)  <Br>
[CVPR 2018] [[Project](https://sites.google.com/site/ziyishenmi/cvpr18_face_deblur)] [[Matlab-Code](https://github.com/joanshen0508/Deep-Semantic-Face-Deblurring)] <Br>
[★] 用一个人脸解析网络得到五官mask, 再把mask与输入结合, 分64和128两个分辨率尺度做deblur

- **Learning Warped Guidance for Blind Face Restoration** <Br>
[Xiaoming Li](https://csxmli2016.github.io/), Ming Liu, Yuting Ye, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), [Liang Lin](http://www.linliang.net/), Ruigang Yang <Br>
[CVPR 2018] [[Torch-Code](https://github.com/csxmli2016/GFRNet)] <Br>
[★] **(基于同一张脸的exemplar做恢复)** 设计了WrapNet做对齐和RecNet做修复. WrapNet以exemplar和LR做输入, 关键点距离作为loss. RecNet接受LR和对齐后的exemplar, 使用全局和局部的gan loss以及VGG loss

- **Deep face deblurring** <Br>
Grigorios Chrysos, [Stefanos Zafeiriou](https://wp.doc.ic.ac.uk/szafeiri/)  <Br>
[CVPRW 2017] <Br>
[☆]



# Face SuperResolution

- **Deep Face Super-Resolution with Iterative Collaboration between Attentive Recovery and Landmark Estimation**  <Br>
Cheng Ma, Zhenyu Jiang, [Yongming Rao](https://raoyongming.github.io/), Jiwen Lu, Jie Zhou <Br>
[CVPR 2020] [[Pytorch-Code](https://github.com/Maclory/Deep-Iterative-Collaboration)] <Br>
[★] 迭代训练人脸超分和关键点网络, 并利用两个任务的信息, 相互优化

- **Learning to Have an Ear for Face Super-Resolution** <Br>
[Givi Meishvili](https://gmeishvili.github.io/), [Simon Jenni](https://sjenni.github.io/), [Paolo Favaro](https://www.cvg.unibe.ch/people/favaro)  <Br>
[CVPR 2020] [[Project](https://gmeishvili.github.io/ear_for_face_super_resolution/index.html)] <Br>

- **Face Super-Resolution Guided by 3D Facial Priors** <Br>
Xiaobin Hu, [Wenqi Ren](https://sites.google.com/site/renwenqi888/home), John LaMaster, [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en), [Xiaoming Li](https://csxmli2016.github.io/), Zechao Li, Bjoern Menze, Wei Liu <Br>
[ECCV 2020] <Br>

- **Component Attention Guided Face Super-Resolution Network: CAGFace** <Br>
Ratheesh Kalarot, [Tao Li](https://tao.li/), [Fatih Porikli](http://porikli.com/) <Br>
[WACV 2020] [[Pytorch-Code](https://github.com/SeungyounShin/CAGFace)] <Br>
[★] 利用人脸解析mask作为attention map的两阶段人脸超分
    
- **Progressive Face Super-Resolution via Attention to Facial Landmark** <Br>
Deokyun Kim, Minseon Kim, Gihyun Kwon, Dae-Shik Kim <Br>
[BMVC 2019] [[Pytorch-Code](https://github.com/DeokyunKim/Progressive-Face-Super-Resolution)] <Br>
[★☆] 一个结构简洁的渐进式人脸超分网络, 使用了额外的关键点检测网络作为计算loss的attention.
	
- **Exemplar Guided Face Image Super-Resolution without Facial Landmarks** <Br>
Berk Dogan, [Shuhang Gu](https://shuhanggu.github.io/), [Radu Timofte](https://people.ee.ethz.ch/~timofter/) <Br>
[CVPRW 2019] [[Pytorch-Code](https://github.com/Maclory/Deep-Iterative-Collaboration)] <Br>
[★] 用一张相同人的照片作为引导图, 将引导图通过一个可学习的warp net与输入图像对齐, 之后将原图和warped guidance经过一个网络生成超分结果. 使用了GAN loss, VGG loss以及identity loss等.

- **FSRNet: End-to-End Learning Face Super-Resolution with Facial Priors** <Br>
Yu Chen, [Ying Tai](https://tyshiwo.github.io/), [Xiaoming Liu](http://cvlab.cse.msu.edu/), [Chunhua Shen](https://cshen.github.io/index.html), Jian Yang <Br>
[CVPR 2018] [[Torch-Code](https://github.com/tyshiwo/FSRNet)] <Br>
[★] 一个分支预测lanmark和分割结果, 辅助人脸超分

- **Super-FAN: Integrated facial landmark localization and super-resolution of real-world low resolution faces in arbitrary poses with GANs** <Br>
[Adrian Bulat](https://www.adrianbulat.com/), [Georgios Tzimiropoulos](http://www.cs.nott.ac.uk/~pszyt/) <Br>
[CVPR 2018] [[Pytorch-Code](https://github.com/jzijin/Super-FAN)] <Br>
[★] 同时做SR和关键点检测

- **To learn image super-resolution, use a GAN to learn how to do image degradation first** <Br>
[Adrian Bulat](https://www.adrianbulat.com/), [Jing Yang](https://www.nottingham.ac.uk/pharmacy/people/jing.yang), [Georgios Tzimiropoulos](http://www.cs.nott.ac.uk/~pszyt/) <Br>
[ECCV 2018] [[Pytorch-Code](https://github.com/jingyang2017/Face-and-Image-super-resolution)] <Br>
[★] 先用GAN预测一个降质网络, 估计真实LR数据, 再训练超分模型
	
- **Face Super-resolution Guided by Facial Component Heatmaps** <Br>
[Xin Yu](https://sites.google.com/view/xinyus-homepage/Home), [Basura Fernando](https://basurafernando.github.io/), [Bernard Ghanem](http://www.bernardghanem.com/), [Fatih Porikli](http://www.porikli.com/), [Richard Hartley](http://users.cecs.anu.edu.au/~hartley/) <Br>
[ECCV 2018] <Br>
[★] 结合人脸关键点的heapmap信息做人脸超分

- **Attention-Aware Face Hallucination via Deep Reinforcement Learning** <Br>
Qingxing Cao, [Liang Lin](http://www.linliang.net/), [Yukai Shi](https://ykshi.github.io/), [Xiaodan Liang](https://lemondan.github.io/), [Guanbin Li](http://guanbinli.com/) <Br>
[CVPR 2017] [[Torch-Code](https://github.com/ykshi/facehallucination)] <Br>

- **Learning to Super-resolve Blurry Face and Text Images** <Br>
[Xiangyu Xu](https://sites.google.com/view/xiangyuxu), [Deqing Sun](https://deqings.github.io/), [Jinshan Pan](https://jspan.github.io/), Yujin Zhang, [Hanspeter Pfister](https://vcg.seas.harvard.edu/), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
[ICCV 2017] [[Project](https://sites.google.com/view/xiangyuxu/deblursr_iccv17)] <Br>





# Face Manipulation

- **TransEditor: Transformer-Based Dual-Space GAN for Highly Controllable Facial Editing** <Br>
[Yanbo Xu](https://github.com/BillyXYB), [Yueqin Yin](https://github.com/yinyueqin), [Liming Jiang](https://liming-jiang.com/), [Qianyi Wu](https://qianyiwu.github.io/), [Chengyao Zheng](https://github.com/daili0015), [Chen Change Loy](https://www.mmlab-ntu.com/person/ccloy/), [Bo Dai](http://daibo.info/), [Wayne Wu](https://wywu.github.io/)  <Br>
[CVPR 2022] [[Project](https://billyxyb.github.io/TransEditor/)] [[Pytorch-Code](https://github.com/BillyXYB/TransEditor)]  <Br>

- **MaskGAN: Towards Diverse and Interactive Facial Image Manipulation** <Br>
[Cheng-Han Lee](https://steven413d.github.io/), [Ziwei Liu](https://liuziwei7.github.io/), Lingyun Wu, [Ping Luo](http://luoping.me/) <Br>
[CVPR 2020] [[Pytorch-Code & Dataset](https://github.com/switchablenorms/CelebAMask-HQ)] <Br>
[★] 大致浏览, 基于语义的人脸操作. 提供了CelebAmask-HQ数据集

- **Interpreting the Latent Space of GANs for Semantic Face Editing**  <Br>
[Yujun Shen](http://shenyujun.github.io), [Jinjin Gu](http://www.jasongt.com), [Xiaoou Tang](http://www.ie.cuhk.edu.hk/people/xotang.shtml), [Bolei Zhou](http://bzhou.ie.cuhk.edu.hk) <Br>
[CVPR 2020]  [[Project](https://genforce.github.io/interfacegan/)] [[Pytorch-Code](https://github.com/genforce/interfacegan)] <Br>
[**InterFaceGAN**]

- **MichiGAN: Multi-Input-Conditioned Hair Image Generation for Portrait Editing** <Br>
Zhentao Tan, [Menglei Chai](https://mlchai.com/), [Dongdong Chen](http://www.dongdongchen.bid/), [Jing Liao](https://liaojing.github.io/html/index.html), [Qi Chu](https://scholar.google.com/citations?user=JZjOMdsAAAAJ&hl=en), Lu Yuan, [Sergey Tulyakov](http://www.stulyakov.com/), [Nenghai Yu](https://scholar.google.com/citations?user=7620QAMAAAAJ&hl=zh-CN)  <Br>
[SIGGRAPH 2020] [[Pytorch-Code](https://github.com/tzt101/MichiGAN)] <Br>
[★] 

- **AttGAN: Facial Attribute Editing by Only Changing What You Want**  <Br>
Zhenliang He, Wangmeng Zuo, Meina Kan, Shiguang Shan, Xilin Chen <Br>
[TIP 2019] [[TF-Code](https://github.com/LynnHo/AttGAN-Tensorflow)] <Br>




	
# Others

- **HairCLIP: Design Your Hair by Text and Reference Image** <Br>
Tianyi Wei, [Dongdong Chen](http://www.dongdongchen.bid/), Wenbo Zhou, [Jing Liao](https://liaojing.github.io/html/index.html), Zhentao Tan, Lu Yuan, Weiming Zhang, Nenghai Yu  <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/wty-ustc/HairCLIP)]  <Br>

- **Intuitive, Interactive Beard and Hair Synthesis With Generative Models** <Br>
[Kyle Olszewski](http://kyleolszewski.com), [Duygu Ceylan](http://www.duygu-ceylan.com), [Jun Xing](https://junxnui.github.io/), [Jose Echevarria](http://www.jiechevarria.com/), [Zhili Chen](http://www.zhilichen.com/), [Weikai Chen](http://chenweikai.github.io/),  [Hao Li](http://hao-li.com)**   <Br>
[CVPR 2020 Oral] [[Project](https://kyleolsz.github.io/HairGen/) <Br>
[**HairGen**] [★] 交互式脸部毛发生成, 结构为两个UNet
	
- **FabSoften: Face Beautification via Dynamic Skin Smoothing, Guided Feathering, and Texture Restoration** <Br>
Sudha Velusamy, Rishubh Parihar, Raviprasad Kini, Aniket Rege   <Br>
[CVPRW 2020] <Br>
[**HairGen**] [☆] 提出了一个人脸美化的流程, 速度应该不会快

