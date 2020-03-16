# Personal repository under construction.

# Table of Contents
- [Restoration](#restoration)
	- [DL Restoration](#dl-restoration)
	- [Traditional Restoration](#traditional-restoration)
- [Image Enhancement](#image-enhancement)
- [Denoising](#denoising)
	- [DL Denoising](#dl-denoising)
	- [Traditional Denoising](#traditional-denoising)
- [Debluring](#debluring)
	- [DL debluring](#dl-debluring)
	- [Traditional debluring](#traditional-debluring)
- [General](#general)
	- [General DL Methods](#general-dl-methods)
	- [General Traditional Methods](#general-traditional-methods)	
- [Using Raw](#using-raw)
- [Dataset](#dataset)
- [Useful Resources](#useful-resources)

# Restoration
## DL Restoration

### Multi-scale-CNN-Dehazing ☆
**[Paper]**  (CVPR 2018) Single Image Dehazing via Multi-Scale Convolutional Neural Networks <Br>
**[Author]** [Wenqi Ren](https://sites.google.com/site/renwenqi888/), [Si Liu](http://www.colalab.org/people), Hua Zhang, [Jinshan Pan](https://sites.google.com/site/jspanhomepage/), [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Project](https://sites.google.com/site/renwenqi888/research/dehazing/mscnndehazing)]** **[[Matlab-Code](https://github.com/rwenqi/Multi-scale-CNN-Dehazing)]**  **[[Unofficial-TF-Code](https://github.com/dishank-b/MSCNN-Dehazing-Tensorflow)]**<Br>
大致浏览, 一个多尺度去雾网络, coarse尺度预测transmission map, fine尺度预测去雾图像, 用深度图生成transmmision map训练 <Br>
	
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


	
### GCANet
**[Paper]** (WACV 2019) Gated Context Aggregation Network for Image Dehazing and Deraining <Br>
**[Author]** [Dongdong Chen](http://www.dongdongchen.bid/), Mingming He, [Qingnan Fan](https://fqnchina.github.io/)  <Br>
**[[Code](https://github.com/cddlyf/GCANet)]**  <Br>
	
## Traditional Restoration
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
	
# Image Enhancement

### DPED ★
**[Paper]** (ICCV 2017) DSLR-Quality Photos on Mobile Devices with Deep Convolutional Networks <Br>
**[Author]** Andrey Ignatov, Nikolay Kobyshev, Kenneth Vanhoey, Radu Timofte , Luc Van Gool  <Br>
**[[Code](http://people.ee.ethz.ch/~ihnatova/index.html)]**   <Br>
1) 从变换的角度出发, 学习一个从低质量图像到高质量图片的变换函数 
2) 变换部分采用残差快结构的CNN，定义了4个loss (color, texture, content, variance). color loss是图像进行高斯模糊后的均方差, texture loss是adversarial loss, content loss是perceptual loss, variance loss是图像梯度的模.
3) 提出了用于图像质量增强的数据集DPED, 包括iPhone, BlackBerry和Sony三种手机与Canon单反相机的图相对.

### WESPE ★
**[Paper]** (arXiv 1709) WESPE: Weakly Supervised Photo Enhancer for Digital Cameras <Br>
**[Author]** Andrey Ignatov, Nikolay Kobyshev, Radu Timofte , Kenneth Vanhoey, Luc Van Gool  <Br>
**[[Project](http://people.ee.ethz.ch/~ihnatova/index.html)]**   <Br>
1) 弱监督, 训练时无需成对的低质量图像和高质量图像. 用两个adversarial losses (color和texture)保证将低质量图像变换到高质量图像所在的域
2) 定义一content loss保证增强后的图像与输入图像的content consistency. 注意此处是将增强后的图像backward map到输入空间, 在输入空间定义的perceptual loss
3) 定义一total variation (TV)保证输出的平滑 
4) 本文的思路及loss的设计来自DPED
  
### EnhanceGAN ★ 
**[Paper]** (arXiv 1707) Aesthetic-Driven Image Enhancement by Adversarial Learning <Br>
**[Author]** 	Yubin Deng, [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/index.html),	[Xiaoou Tang](https://www.ie.cuhk.edu.hk/people/xotang.shtml)  <Br>
1) weakly supervised方法, 学习crop和色彩变换参数, 增强aesthetic quality



# Denoising
## DL Denoising

### RIDNet ★☆
**[Paper]** (ICCV 2019 Oral) Real image denoising with feature attention<Br>
**[Author]** [Saeed Anwar](https://saeed-anwar.github.io/), Nick Barnes<Br>
**[[Code](https://github.com/saeed-anwar/RIDNet)]**  <Br>
1) 提出了一个端到端的去噪网络, 基于channel attention和skip connection. 在真是图像上测试效果不错, 速度一般. <Br>
2) 作为一篇Oral来说感觉创新点和理论论述都一般, 也没有解释为什么提出的网络对真是图像去噪效果好. <Br>
3) 如果需要, 参考网络流程图和代码即可. <Br>
	
### Unprocessing Images for Learned Raw Denoising ★☆
**[Paper]** (CVPR 2019) Unprocessing Images for Learned Raw Denoising<Br>
**[Author]** [Tim Brooks](https://www.timothybrooks.com/tech/), [Ben Mildenhall](https://people.eecs.berkeley.edu/~bmild/), [Tianfan Xue](http://people.csail.mit.edu/tfxue/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/), [Dillon Sharlet](http://dsharlet.com/), [Jonathan T. Barron](https://jonbarron.info/)<Br>
**[[Code](https://www.timothybrooks.com/tech/unprocessing/)]**  <Br>
1) 提出了一个通过unprocess ISP流程而生成更真实去噪样本的框架, 可以用任意图像生成真实的训练样本, 以提高模型性能. <Br>
2) 对于sRGB图像, 根据ISP流程, 将其逐步逆运算位raw image, 在此基础上加的噪声更符合真实噪声.<Br>
3) 推断时, 要先把sRGB转换为raw image, 再经过网络处理, 最后再进行正向的ISP恢复为sRGB. <Br>
4) ISP流程的推断对每个品牌型号的相机都有所不同, 模拟其过程感觉还是有难度的. <Br>
	
### CBDNet ★☆
**[Paper]** (CVPR 2019) Toward Convolutional Blind Denoising of Real Photographs<Br>
**[Author]** Shi Guo, Zifei Yan, Kai Zhang, Wangmeng Zuo, Lei Zhang, [Jonathan T. Barron](https://jonbarron.info/)<Br>
**[[Code](https://github.com/GuoShi28/CBDNet)]**  <Br>
1) 大致浏览. 采用一个FCN估计噪声level, 噪声level map与输入concat然后输入一类似U-Net的网络去噪. <Br>
2) 可以学习其网络和训练细节. <Br>
	
## Traditional Denoising

# Debluring
## DL Debluring
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
	
### DeblurGAN-v2 ★☆
**[Paper]** (ICCV 2019) DeblurGAN-v2: Deblurring (Orders-of-Magnitude) Faster and Better <Br>
**[Author]** Orest Kupyn, Tetiana Martyniuk, Junru Wu, Zhangyang Wang<Br>
**[[Pytorch-Code](https://github.com/TAMU-VITA/DeblurGANv2)]**  <Br>
	
## Traditional Debluring

# General
## General DL Methods
 
### Fast Image Processing ★★
**[Paper]** (ICCV 2017) Fast Image Processing with Fully-Convolutional Networks <Br>
**[Author]** [Qifeng Chen](https://cqf.io/),	Jia Xu,	[Vladlen Koltun](http://vladlen.info/)  <Br>
**[[Project](https://cqf.io/ImageProcessing/)]** <Br>
较早用CNN做图像滤波增强的paper之一, 使用了dilation conv提取全局信息. <Br>
	
### HDRNet ★★	
**[Paper]** (Siggraph 2017) Deep Bilateral Learning for Real-Time Image Enhancement <Br>
**[Author]** 	Michaël Gharbi, [Jiawen Chen](http://people.csail.mit.edu/jiawen/), [Jonathan T. Barron](https://jonbarron.info/),  [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Frédo Durand](http://people.csail.mit.edu/fredo/)  <Br>
**[[Project](https://groups.csail.mit.edu/graphics/hdrnet/)]**<Br>
1) 提出了一个实时图像增强网络, 速度快, 效果好. <Br>
2) 网络分为两个分支, 低分辨率分支提取特征, 学习每个像素的色彩映射参数; 高分辨率分支负责提取和保留细节信息. low res分支学到的映射参数通过类似于双线性差值的过程上采样到high res, 最后对high res图像做色彩映射并输出. <Br>
3) 学习映射参数部分, 采用bilateral grid的思路. 第三个维度被解释成8*12的网格, 意思是对8个灰度level做不同的色彩映射. 处理时选择哪个level的参数, 由high res分支生成的引导图决定. <Br>

###  Trainable Guided Filter ★★ 
**[Paper]** (CVPR 2018) Fast End-to-End Trainable Guided Filter <Br>
**[Author]**  [Huikai Wu](http://wuhuikai.me/), [Shuai Zheng](https://kylezheng.org/), [Junge Zhang](http://www.escience.cn/people/JungeZHANG/index.html), [Kaiqi Huang](http://www.cbsr.ia.ac.cn/users/kqhuang/) <Br>
**[[Code](https://github.com/wuhuikai/DeepGuidedFilter)]**<Br>
1) 可训练的引导滤波, 用于联合上采样. 可用于各种像素级的增强任务中. <Br>
2) 同时提供了用TensorFlow实现的原始guided filter, 赞！<Br>
	
### ***Perception-Distortion Tradeoff* ★★**
**[Paper]** (CVPR 2018) The Perception-Distortion Tradeoff <Br>
**[Authors]** [Yochai Blau](https://yochai.webgr.technion.ac.il/), [Tomer Michaeli](https://tomer.net.technion.ac.il/) <Br>
1) 大致浏览, 提出在image restoration中, perception和distortion存在tradeoff. 对不同的loss这种tradedoff的严重程度不同, 如perceptual loss与MSE loss相比能在perception和distortion直接取得更好的平衡. <Br>
2) 很多理论都还没看, 日后如果研究这一方向, 可以仔细读一下. <Br>
	
### **Decouple Learning**
**[Paper]** (ECCV 2018) Decouple Learning for Parameterized Image Operators <Br>
**[Authors]** Qingnan Fan, Dongdong Chen, Lu Yuan, Gang Hua, Nenghai Yu, Baoquan Chen <Br>
**[[Code](https://github.com/fqnchina/DecoupleLearning)]** <Br>

### **Contextual Loss ★★**
**[Paper]** (ECCV 2018 Oral) The Contextual Loss for Image Transformation with Non-Aligned Data <Br>
**[Authors]** [Roey Mechrez](https://cgm.technion.ac.il/people/Roey/), Itamar Talmi, Firas Shama, [Lihi Zelnik-Manor](https://lihi.net.technion.ac.il/) <Br>
**[[Project](http://cgm.technion.ac.il/Computer-Graphics-Multimedia/Software/Contextual/)]** **[[Code](https://github.com/roimehrez/contextualLoss)]**<Br>
提出了一个处理非对齐数据的loss, 利用特征(用VGG19获得)的距离定义两像素特征点的相似度, 并在此基础上定义loss, 以解决输入和真值在空间上不对齐的问题. <Br>
	
### SVLRM ★
**[Paper]** (CVPR 2019) Spatially Variant Linear Representation Models for Joint Filtering <Br>
**[Author]** 	[Jinshan Pan](https://sites.google.com/site/jspanhomepage/), Jiangxin Dong, [Jimmy S. Ren](http://www.jimmyren.com/), [Liang Lin](http://www.linliang.net/), Jinhui Tang, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Project](https://sites.google.com/site/jspanhomepage/)]** <Br>
大致浏览, 用CNN预测guided filter中的系数A和b. <Br>


	
## General Traditional Methods

### Guided Image Filtering ★★★ 
**[Paper]** (ECCV 2010) Guided Image Filtering  <Br>
**[Author]**  [Kaiming He](http://kaiminghe.com/index.html), [Jian Sun](http://www.jiansun.org/), [Xiaoou Tang](http://www.ie.cuhk.edu.hk/people/xotang.shtml) <Br>
**[[Project](http://kaiminghe.com/eccv10/)]** **[[TF/Pytorch-Code](https://github.com/wuhuikai/DeepGuidedFilter/tree/master/GuidedFilteringLayer)]**  <Br>
大名鼎鼎的引导滤波, 可用在去噪, 融合, 联合上采样, matting, 图像增强等多种任务中. 速度快, 效果好. <Br>
	
### Local Laplacian Filters ★★
**[Paper]** (SIGGRAPH 2011) Local Laplacian Filters: Edge-aware Image Processing with a Laplacian Pyramid  <Br>
**[Author]**  [Sylvain Paris](http://people.csail.mit.edu/sparis/), [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Jan Kautz](http://jankautz.com/)<Br>
**[[Project](http://people.csail.mit.edu/sparis/publi/2011/siggraph/)]** **[[Code1](https://github.com/psalvaggio/local_laplacian_filters)]** **[[Code2](https://github.com/hassenkassim/LocalLaplace)]** <Br>
用拉普拉斯金字塔做图像增强, tone mapping等. <Br>

### Misalignment-Robust Joint Filter ★☆
**[Paper]** (ICCV 2017) Misalignment-Robust Joint Filter for Cross-Modal Image Pairs <Br>
**[Author]**  Takashi Shibata, [Masayuki Tanaka](http://www.ok.sc.e.titech.ac.jp/~mtanaka/publication2017.html), [Masatoshi Okutomi](http://www.ok.sc.e.titech.ac.jp/mem/mxo/okutomi.html) <Br>
1) 提出一种适用于不对齐多模数据的联合滤波方法, 可结合引导滤波等优良滤波算法, 在非对齐不同源数据上达到很好的滤波效果. <Br>
2) 算法的思路其实就是计算cost volume并对其进行加权求和. 其最好版本的大体思路为: 将引导图上下左右位移组成k个移位引导图, 1.计算target和k个引导图的距离(NCC等)组成cost volume. 2.从cost volume计算weight volume, 并通过最小化能量函数的方法对其进行优化. 3.用k个移位引导图分别对target进行滤波.4.用weight volume对k个滤波输出进行加权平均, 生成最后的输出. <Br>
3) 从paper中看, 该方法对非对齐的多模数据滤波效果不错, 可以在设计DL方案时作为参考. <Br>
4) 算法的局限: 1.weight volume优化的步骤过于耗时; 2. cost volume的准确性仍依赖于距离的计算准则, 现有的例如NCC等策略也不能完美解决多模数据的相似性度量问题.<Br>

# Using Raw
###  *Super-Resolution with Raw Images*
**[Paper]**  (CVPR 2019) Towards Real Scene Super-Resolution with Raw Images  <Br>
**[Author]** [Xiangyu Xu](https://sites.google.com/view/xiangyuxu/%E9%A6%96%E9%A1%B5), Yongrui Ma, [Wenxiu Sun](http://wenxiusun.com/) <Br>
**[[Project](https://sites.google.com/view/xiangyuxu/rawsr_cvpr19)]** <Br>
大致浏览, 利用Raw做细节恢复, 用RGB做Color校正.<Br> 

###  TENet ★
**[Paper]**  (arXiv 1905) Trinity of Pixel Enhancement: a Joint Solution for Demosaicking, Denoising and Super-Resolution  <Br>
**[Author]** [Guocheng Qian](https://www.gcqian.com/), [Jinjin Gu](http://www.jasongt.com/), [Jimmy Ren](http://www.jimmyren.com/), [Chao Dong](http://xpixel.group/2010/01/20/chaodong.html), Furong Zhao, Juan Lin <Br>
**[[Pytorch-Code](https://github.com/guochengqian/TENet)]** <Br>
1. 使用具有pixel shift技术的相机收集了一可以做demoasic的数据集, 避免了用普通RGB数据做真值时内置demoasic过程带来的误差
2. 提出了一端到端的demosaic, 去噪和超分的网络, 采用residual + dense block的形式, 没什么特别的

# Dataset
## Real Image Denoising
[DnD](https://noise.visinf.tu-darmstadt.de/) <Br>
[SIDD](https://www.eecs.yorku.ca/~kamel/sidd/) <Br>

[PolyU](https://github.com/csjunxu/PolyU-Real-World-Noisy-Images-Dataset) <Br>
[Renoir](http://ani.stat.fsu.edu/~abarbu/Renoir.html) <Br>
[CC](http://snam.ml/research/ccnoise) <Br>
[SID](http://cchen156.web.engr.illinois.edu/SID.html) <Br>
[kodak_color](http://r0k.us/graphics/kodak/) <Br>
[NoiseClinicImages](http://demo.ipol.im/demo/125/input_select?044_solvay_1927.x=63&044_solvay_1927.y=68) <Br>

# Useful Resources
https://paperswithcode.com/task/image-denoising?page=2 

https://github.com/wenbihan/reproducible-image-denoising-state-of-the-art


