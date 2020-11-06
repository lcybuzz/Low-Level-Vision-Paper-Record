# General

# Table of Contents
  - [General DL Methods](#general-dl-methods)
  - [General Traditional Methods](#general-traditional-methods)	
    
    

## General DL Methods

### *Deep Joint Image Filtering*
**[Paper]** Deep Joint Image Filtering <Br>
**[Year]** ECCV 2016 <Br>
**[Author]** [Yijun Li](https://yijunmaverick.github.io/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/), [Narendra Ahuja](http://vision.ai.illinois.edu/ahuja.html), [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/) <Br>
**[Pages]** <Br>
http://vllab1.ucmerced.edu/~yli62/DJF_residual/ <Br>
https://github.com/Yijunmaverick/DeepJointFilter <Br>
**[Description]** <Br>
	
### *Learning Recursive Filters for Low-Level Vision via a Hybrid Neural Network*
**[Paper]** Learning Recursive Filters for Low-Level Vision via a Hybrid Neural Network <Br>
**[Year]** ECCV 2016 Oral<Br>
**[Author]**   		[Sifei Liu](https://www.sifeiliu.net/), [Jinshan Pan](http://vllab1.ucmerced.edu/~jinshan/), [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/) <Br>
**[Pages]** <Br>
https://www.sifeiliu.net/linear-rnn <Br>
https://github.com/Liusifei/caffe-lowlevel <Br>
**[Description]** <Br>
 
### Fast Image Processing ★★
**[Paper]** (ICCV 2017) Fast Image Processing with Fully-Convolutional Networks <Br>
**[Author]** [Qifeng Chen](https://cqf.io/),	Jia Xu,	[Vladlen Koltun](http://vladlen.info/)  <Br>
**[[Project](https://cqf.io/ImageProcessing/)]** <Br>
较早用CNN做图像滤波增强的paper之一, 使用了dilation conv提取全局信息. <Br>

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
	
### DecoupleLearning ★
**[Paper]**  (ECCV 2018) Decouple Learning for Parameterized Image Operators <Br>
**[Author]** [Qingnan Fan](https://fqnchina.github.io/), [Dongdong Chen](http://www.dongdongchen.bid/), [Lu Yuan](https://www.microsoft.com/en-us/research/people/luyuan/), [Gang Hua](http://www.ganghua.org/), [Nenghai Yu](http://staff.ustc.edu.cn/~ynh/), Baoquan Chen  <Br>
**[[PyTorch-Code](https://github.com/fqnchina/DecoupleLearning)]**  <Br>
粗读, 貌似是给不同任务设定一个parameter, 用网络以parameter为输入预测每层的weight, 这个weight作为instance norm的weight对每层做归一化.

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


### DNI ★☆
**[Paper]** (CVPR 2019) Deep Network Interpolation <Br>
**[Author]** [Xintao Wang](https://xinntao.github.io/), [Ke Yu](https://yuke93.github.io/), [Chao Dong](http://xpixel.group/2010/01/20/chaodong.html), [Xiaoou Tang](), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[[Project](https://xinntao.github.io/projects/DNI)]** <Br>
大致浏览, 通过对filter插值取得两个或多个任务间过渡的效果. 为保证两个filter直接有强相关性，用一个模型作为另一个模型的pretrain model.

### SGN 
**[Paper]** (ICCV 2019) Self-Guided Network for Fast Image Denoising <Br>
**[Author]** [Shuhang Gu](https://sites.google.com/site/shuhanggu/), Yawei Li, Luc Van Gool, [Radu Timofte](http://people.ee.ethz.ch/~timofter/)  <Br>
**[[Pytorch-Code](https://github.com/ShuhangGu/SGN_ICCV2019)]** <Br>

### MTLU ★
**[Paper]** (ICCV 2019) Fast Image Restoration with Multi-bin Trainable Linear Units <Br>
**[Author]** [Shuhang Gu](https://sites.google.com/site/shuhanggu/), Wen Li, Luc Van Gool, [Radu Timofte](http://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/ShuhangGu/MTLU_ICCV2019)]** <Br>
	
	
### CIE XYZ Net ★
**[Paper]** (arXiv 2006) CIE XYZ Net: Unprocessing Images for Low-Level Computer Vision Tasks <Br>
**[Author]** [Mahmoud Afifi](https://sites.google.com/view/mafifi), [Abdelrahman Abdelhamed](https://www.eecs.yorku.ca/~kamel/), [Abdullah Abuolaim](https://sites.google.com/view/abdullah-abuolaim/), [Abhijith Punnappurath](https://abhijithpunnappurath.github.io/), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/)<Br>
**[[Matlab & Pytorch-Code](https://github.com/mahmoudnafifi/CIE_XYZ_NET)]** <Br>	
使用CNN, 把sRGB变换到设备无关的CIE XYZ空间, 在此scene-referred空间中进行去噪增强等处理, 再用一CNN变换回sRGB空间
	
### Invertible Image Rescaling ★★
**[Paper]** (ECCV 2020) Invertible Image Rescaling <Br>
**[Author]** Mingqing Xiao, Shuxin Zheng, [Chang Liu](https://changliu00.github.io/), Yaolong Wang, Di He, Guolin Ke, Jiang Bian, [Zhouchen Lin](https://zhouchenlin.github.io/), [Tie-Yan Liu](https://www.microsoft.com/en-us/research/people/tyliu/?from=http%3A%2F%2Fresearch.microsoft.com%2Fusers%2Ftyliu)<Br>
**[[Pytorch-Code](https://github.com/pkuxmq/Invertible-Image-Rescaling)]** <Br>	
提出一个基于小波和可逆神经网络(INN)的图像降采样恢复方法. 


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
用拉普拉斯金字塔做图像增强, tone mapping等. 为更好地保持边缘, 对高斯金字塔的每个像素做映射, 根据其与原分辨率对应像素的差值, 将其分为边缘和细节两种case, 对细节进行非线性增强, 对边缘进行线性的对比度增强. <Br>

### Misalignment-Robust Joint Filter ★☆
**[Paper]** (ICCV 2017) Misalignment-Robust Joint Filter for Cross-Modal Image Pairs <Br>
**[Author]**  Takashi Shibata, [Masayuki Tanaka](http://www.ok.sc.e.titech.ac.jp/~mtanaka/publication2017.html), [Masatoshi Okutomi](http://www.ok.sc.e.titech.ac.jp/mem/mxo/okutomi.html) <Br>
1) 提出一种适用于不对齐多模数据的联合滤波方法, 可结合引导滤波等优良滤波算法, 在非对齐不同源数据上达到很好的滤波效果. <Br>
2) 算法的思路其实就是计算cost volume并对其进行加权求和. 其最好版本的大体思路为: 将引导图上下左右位移组成k个移位引导图, 1.计算target和k个引导图的距离(NCC等)组成cost volume. 2.从cost volume计算weight volume, 并通过最小化能量函数的方法对其进行优化. 3.用k个移位引导图分别对target进行滤波.4.用weight volume对k个滤波输出进行加权平均, 生成最后的输出. <Br>
3) 从paper中看, 该方法对非对齐的多模数据滤波效果不错, 可以在设计DL方案时作为参考. <Br>
4) 算法的局限: 1.weight volume优化的步骤过于耗时; 2. cost volume的准确性仍依赖于距离的计算准则, 现有的例如NCC等策略也不能完美解决多模数据的相似性度量问题.<Br>


### Fast bilateral filtering for the display of high-dynamic-range images
**[Paper]** (SIGGRAPH 2002) Fast bilateral filtering for the display of high-dynamic-range images <Br>
**[Author]** [Frédo Durand](http://people.csail.mit.edu/fredo/), Julie Dorsey  <Br>
**[[Project](http://people.csail.mit.edu/fredo/PUBLI/Siggraph2002/)]** **[[Code](http://people.csail.mit.edu/sparis/bf/#code)]**

### *A Fast Approximation of the Bilateral Filter using a Signal Processing Approach* ★★
**[Paper]** (ECCV 2006) A Fast Approximation of the Bilateral Filter using a Signal Processing Approach <Br>
**[Author]** [Sylvain Paris](http://people.csail.mit.edu/sparis/), [Frédo Durand](http://people.csail.mit.edu/fredo/)  <Br>
**[[Code](http://people.csail.mit.edu/sparis/bf/#code)]** **[[A Good Blog](https://niecongchong.github.io/2019/08/28/%E5%A2%9E%E7%BB%B4%E5%9E%8B%E5%BF%AB%E9%80%9F%E5%8F%8C%E8%BE%B9%E6%BB%A4%E6%B3%A2/)]**    <Br>
Bilateral filter的一种加速方法. 将2D图像的灰度值作为一个新的维度, 将原来的非线性滤波操作转化为3D空间中的线性卷积. 并且, 高斯卷积属于低通操作, 因此可以把3D网络做下采样而不损失精度, 在小分辨上进行3D卷积, 速度大大提升.


### Bilateral Grid ★★
**[Paper]** (SIGGRAPH 2007) Real-time edge-aware image processing with the bilateral grid <Br>
**[Author]** [Jiawen Chen](https://people.csail.mit.edu/jiawen/), [Sylvain Paris](http://people.csail.mit.edu/sparis/), [Frédo Durand](http://people.csail.mit.edu/fredo/)  <Br>
**[[Project](http://groups.csail.mit.edu/graphics/bilagrid/)]** <Br>
将转换到3D空间的思路离散化, 网格化, 提出bilateral grid这种数据结构. 优化了代码, 在GPU上达到实时. 在多种任务上有良好表现.
	
### JBU
**[Paper]** (SIGGRAPH 2007) Joint Bilateral Upsampling <Br>
**[Author]**  [Johannes Kopf](http://johanneskopf.de/), Michael F. Cohen, [Dani Lischinski](https://www.cs.huji.ac.il/~danix/), Matt Uyttendaele <Br>
**[[Project](http://johanneskopf.de/publications/jbu/)]**
	
### BGU
**[Paper]** (SIGGRAPH 2016 Asia) Bilateral Guided Upsampling <Br>
**[Author]** [Jiawen Chen](https://people.csail.mit.edu/jiawen/), Andrew Adams, [Neal Wadhwa](https://nealwadhwa.com/), [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/) <Br>
**[[Matlab-Code](https://github.com/google/bgu)]** <Br>

	

