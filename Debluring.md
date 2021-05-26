# Debluring 
# Table of Contents
- [Image Debluring](#image-debluring)
- [Video Debluring](#video-debluring)

## Image Debluring	
### *Deblurring by Realistic Blurring*
**[Paper]** (CVPR 2020) Deblurring by Realistic Blurring <Br>
**[Author]** [Kaihao Zhang](https://sites.google.com/view/kaihaozhang), [Wenhan Luo](https://sites.google.com/site/whluoimperial/), Yiran Zhong, [Lin Ma](http://forestlinma.com/), Bjorn Stenger, Wei Liu, [Hongdong Li](http://users.cecs.anu.edu.au/~hongdong/)<Br>

### *Event-Based Motion Deblurring*
**[Paper]** (CVPR 2020) Learning Event-Based Motion Deblurring <Br>
**[Author]** Zhe Jiang, [Yu Zhang](https://zhangyulb.github.io/), Dongqing Zou, [Jimmy Ren](http://www.jimmyren.com/), Jiancheng Lv, Yebin Liu<Br>

### *Deblurring Using Spatially Variant Deconvolution*
**[Paper]** (CVPR 2020) Efficient Dynamic Scene Deblurring Using Spatially Variant Deconvolution Network With Optical Flow Guided Training <Br>
**[Author]** Yuan Yuan, Wei Su, Dandan Ma<Br>

### *Adaptive Motion Deblurring*
**[Paper]** (CVPR 2020) Spatially-Attentive Patch-Hierarchical Network for Adaptive Motion Deblurring <Br>
**[Author]** Maitreya Suin, Kuldeep Purohit, A. N. Rajagopalan<Br>
	
### *Variational-EM-Based Deblurring*
**[Paper]** (CVPR 2020) Variational-EM-Based Deep Learning for Noise-Blind Image Deblurring <Br>
**[Author]** Yuesong Nan, Yuhui Quan, Hui Ji<Br>
	
### *Deblurring Using Analysis-Synthesis Networks Pair*
**[Paper]** (CVPR 2020) Deblurring Using Analysis-Synthesis Networks Pair<Br>
**[Author]** Adam Kaufman, Raanan Fattal<Br>

### *Deep Learning for Handling Kernel/model Uncertainty in Image Deconvolution*
**[Paper]** (CVPR 2020) Deep Learning for Handling Kernel/model Uncertainty in Image Deconvolution<Br>
**[Author]** Yuesong Nan, Hui Ji<Br>
	
### *Bad Weather Removal using Architectural Search*
**[Paper]** (CVPR 2020) All in One Bad Weather Removal using Architectural Search<Br>
**[Author]** Ruoteng Li, Robby T. Tan, Loong-Fah Cheong<Br>

### DeblurGAN-v2 ★☆
**[Paper]** (ICCV 2019) DeblurGAN-v2: Deblurring (Orders-of-Magnitude) Faster and Better <Br>
**[Author]** Orest Kupyn, Tetiana Martyniuk, Junru Wu, Zhangyang Wang<Br>
**[[Pytorch-Code](https://github.com/TAMU-VITA/DeblurGANv2)]**  <Br>
DeblurGAN基础上的改进, 把生成网络换成了FPN, 设计了新的loss, 效果更快更好了

### DeepGyro ★
**[Paper]** (WACV 2019) Gyroscope-Aided Motion Deblurring with Deep Network <Br>
**[Author]** Janne Mustaniemi, Juho Kannala, Simo Särkkä, Jiri Matas, Janne Heikkilä<Br>
结合陀螺仪作为先验deblur. 从陀螺仪和图像拍摄信息生成训练集的方法可以参考. <Br>
	
### Dr-Net ★☆
**[Paper]** (CVPR 2019) Douglas-Rachford Networks: Learning Both the Image Prior and Data Fidelity Terms for Blind Image Deconvolution <Br>
**[Author]** Raied Aljadaany, [Dipan K. Pal](https://dkpal.github.io/), [Marios Savvides](https://www.cmu-biometrics.org/)<Br>
1) 基于Douglas-Rachford迭代优化求解blind deconvolution的思路(不懂), 提出了一个由简单conv和连接操作组成的Dr Block, 将其嵌入普通卷积网络中, 用L2和GAN loss训练, 取得了不错的效果. <Br>
2) 网络细节没看, 可以借鉴其模块设计
	
### DMPHN ☆
**[Paper]** (CVPR 2019) Deep Stacked Multi-patch Hierarchical Network for Image Deblurring <Br>
**[Author]** [Hongguang Zhang](https://hongguangzhang.github.io/), [Yuchao Dai](http://users.cecs.anu.edu.au/~yuchao/), [Hongdong Li](http://users.cecs.anu.edu.au/~hongdong/), [Piotr Koniusz](http://users.cecs.anu.edu.au/~koniusz/)<Br>
**[[Pytorch-Code](https://github.com/HongguangZhang/DMPHN-cvpr19-master)]** <Br>
从spatial pyramid matching的角度出发, 提出了一个分patch的逐层融合处理的网络, 参数少速度快. 但个人仍不理解这种分patch的做法对CNN来说到底有什么意义. 

### HA-Deblur ★☆
**[Paper]** (ICCV 2019) Human-Aware Motion Deblurring <Br>
**[Author]** [Ziyi Shen](https://sites.google.com/site/ziyishenmi/), [Wenguan Wang](https://sites.google.com/view/wenguanwang/), [Xiankai Lu](https://sites.google.com/site/xiankailu111/), Jianbin Shen, [Haibin Ling](https://www3.cs.stonybrook.edu/~hling/), Tingfa Xu, [Ling Shao](http://www.inceptioniai.org/)<Br>
**[[Project](https://sites.google.com/site/ziyishenmi/ha_deblur)]**  **[[HIDE Dataset](https://github.com/joanshen0508/HA_deblur)]** <Br>
1. 提出了HIDE数据集, 主要关注对人体的deblur <Br>
2. 提出了一个多分支deblur网络, 根据human-aware子网络预测前背景生成weight map, 将多分枝信息融合处理后输出 <Br>	
	
### ED-DSRN ☆
**[Paper]** (ICASSP 2018) A Deep Encoder-Decoder Network For Joint Deblurring and Super-Resolution <Br>
**[Author]** Xinyi Zhang, Fei Wang, Hang Dong, Yu Guo  <Br>
**[[Project](http://xinyizhang.tech/icassp2018/)]**  <Br>
大致浏览, 一个端到端的同时deblur和超分网络 <Br>
	

### GFN ★☆
**[Paper]** (BMVC 2018) Gated Fusion Network for Joint Image Deblurring and Super-Resolution <Br>
**[Author]** Xinyi Zhang, Hang Dong, [Zhe Hu](https://zjuela.github.io/), [Wei-Sheng Lai](http://graduatestudents.ucmerced.edu/wlai24/), Fei Wang, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/_)<Br>
**[[Project](http://xinyizhang.tech/bmvc2018/)]** **[[Pytorch-Code](https://github.com/jacquelinelala/GFN)]** <Br>
1) 提出了一个同时做deblur和超分的网络. 网络有两个分支, 一个encoder-decoder结构做deblur, 一个不降分辨率做SR, 用一个几层卷积组成的gate模块选择特征. <Br>
2) 思路简单, 可以尝试.<Br>
	
### DeblurGAN ★★
**[Paper]** (CVPR 2018) DeblurGAN: Blind Motion Deblurring Using Conditional Adversarial Networks <Br>
**[Author]** Orest Kupyn, Volodymyr Budzan, Mykola Mykhailych, Dmytro Mishkin, Jiří Matas<Br>
**[[Pytorch-Code](https://github.com/KupynOrest/DeblurGAN)]** **[[Unofficial-TF-Code1](https://github.com/LeeDoYup/DeblurGAN-tf)]** **[[Unofficial-TF-Code2](https://github.com/dongheehand/DeblurGAN-tf)]**<Br>
1) 用GAN做deblur的一篇典型文章, 效果不错.<Br>
2) 生成网络结构简单, 采用残差形式. <Br>
3) 提出了生成blur数据的方法, 可以参考一下. <Br>
	
### Deep Multi-scale Deblur ★☆
**[Paper]** (CVPR 2017 Spotlight) Deep Multi-scale Convolutional Neural Network for Dynamic Scene Deblurring <Br>
**[Author]** [Seungjun Nah](https://seungjunnah.github.io/), [Tae Hyun Kim](https://sites.google.com/site/lliger9/), [Kyoung Mu Lee](https://cv.snu.ac.kr/index.php/~kmlee/)  <Br>
**[[Code](https://github.com/SeungjunNah/DeepDeblur_release)]**  <Br>
1) 提出了GOPRO单张图像deblur数据集 <Br>
2) 提出了一个多尺度输入的去噪网络	
	
	

## Video Debluring
### CDVD-TSP
**[Paper]** (CVPR 2020) Cascaded Deep Video Deblurring Using Temporal Sharpness Prior <Br>
**[Author]** [Jinshan Pan](https://jspan.github.io/), [Haoran Bai](https://baihaoran.xyz/about), Jinhui Tang<Br>
**[[Project](https://baihaoran.xyz/projects/cdvd-tsp/index.html)]**  **[[Pytorch-Code](https://github.com/csbhr/CDVD-TSP)]** <Br>
