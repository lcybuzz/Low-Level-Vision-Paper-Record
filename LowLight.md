# Low Light

# Table of Contents
  - [DL Methods](#dl-methods)
  - [Traditional Methods](#traditional-methods)	
  - [Useful Resources](#useful-resources)
    

## DL Methods

## Deep Learning

### MSR-net ★☆
**[Paper]** (arXiv 1711) MSR-net:Low-light Image Enhancement Using Deep Convolutional Network <Br>
**[Author]** Liang Shen, Zihan Yue, Fan Feng, Quan Chen, Shihao Liu, Jie Ma <Br>
用CNN做亮度增强较早的一篇, 个人觉得该网络结构可能未必效果很好, 但思路值得学习. 本文认为传统的MSR(multi scale Retinex)在实际应用中可以DoG的形式近似, 不同核的高斯函数可用若干个卷积stack代替. 提出的网络首先将低光照输入做不同程度的亮度调整并变换到log域, 之后再仿照MSR的形式用CNN对输入进行亮度增强, 最后是一个1x1的颜色恢复模块. 


### Exposure ★
**[Paper]** (SIGGRAPH 2018) Exposure: A White-Box Photo Post-Processing Framework <Br>
**[Author]** [Yuanming Hu](http://taichi.graphics/me/), [Hao He](http://people.csail.mit.edu/hehaodele/), Chenxi Xu, [Baoyuan Wang](https://sites.google.com/site/zjuwby/), Stephen Lin <Br>
**[[TF-Code](https://github.com/yuanming-hu/exposure)]** <Br> 
胡渊明大神在图像质量增强领域的一篇论文, 用增强学习对图像进行对比度, 曝光度, gamma等方面的校正. 由于实际部署的限制, 目前未对增强学习有所了解.
	
	

### SICE 
**[Paper]** (TIP 2018) Learning a Deep Single Image Contrast Enhancer from Multi-Exposure Images <Br>
**[Author]** [Jianrui Cai](https://csjcai.github.io/), [Shuhang Gu](https://sites.google.com/site/shuhanggu/), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
**[[Caffe-Code](https://github.com/csjcai/SICE)]** <Br>
	
### GLADNet ☆
**[Paper]** (FG 2018) GLADNet: Low-Light Enhancement Network with Global Awareness <Br>
**[Author]** [Wenjing Wang](https://daooshee.github.io/website/),[Chen Wei](https://weichen582.github.io/), [Wenhan Yang](https://flyywh.github.io/index.html), [Jiaying Liu](http://39.96.165.147/people/liujiaying.html) <Br>
**[[Project](https://daooshee.github.io/fgworkshop18Gladnet/)]**   **[[TF-Code](https://github.com/weichen582/GLADNet)]** <Br>
encoder-decoder + refine结构的网络
	
### LightenNet
**[Paper]** (PRL 2018) LightenNet: A Convolutional Neural Network For Weakly Illuminated Image Enhancement <Br>
**[Author]** [Chongyi Li](https://li-chongyi.github.io/sub_publication.html), Jichang Guo, [Fatih Porikli](http://www.porikli.com/), Yanwei Pang <Br>
**[[Project](https://li-chongyi.github.io/proj_lowlight.html)]**  	

### RetinexNet ★
**[Paper]** (BMVC 2018 Oral) Deep Retinex Decomposition for Low-Light Enhancement <Br>
**[Author]** [Chen Wei](https://weichen582.github.io/), [Wenjing Wang](https://daooshee.github.io/website/), [Wenhan Yang](https://flyywh.github.io/index.html), [Jiaying Liu](http://39.96.165.147/people/liujiaying.html)  <Br>
**[[Project](https://daooshee.github.io/BMVC2018website/)]**   **[[TF-Code](https://github.com/weichen582/RetinexNet)]** <Br>
基于retinex理论设计的网络, 后续一些工作基于这个思路展开, 但本文的效果一般
	
### MBLLEN ★
**[Paper]** (BMVC 2018) MBLLEN: Low-light Image/Video Enhancement Using CNNs <Br>
**[Author]** [Feifan Lv](https://lvfeifan.github.io/), [Feng Lu](http://shi.buaa.edu.cn/lufeng/), Jianhua Wu, Chongsoon Lim <Br>
**[[Page](http://phi-ai.org/project/MBLLEN/default.htm)]**   **[[TF-Code](https://github.com/Lvfeifan/MBLLEN)]** <Br>
多分支亮度增强网络
	
### Deep Photo Enhancer ★☆
**[Paper]** (CVPR 2018 Spotlight) Deep Photo Enhancer: Unpaired Learning for Image Enhancement from Photographs with GANs <Br>
**[Author]** [Yu-Sheng Chen](https://www.cmlab.csie.ntu.edu.tw/~nothinglo/), [Yu-Ching Wang](https://www.cmlab.csie.ntu.edu.tw/~urchinwang/), [Man-Hsin Kao](https://www.cmlab.csie.ntu.edu.tw/~cindy0711/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/) <Br>
**[[TF-Code](https://github.com/nothinglo/Deep-Photo-Enhancer)]** **[[TF-Code2](https://github.com/pnbao/deep-photo-enhance)]**<Br>
UNet + cycGAN, 无需paired样本的图像增强方法, 可以参考, 只是代码有一点点乱

### Distort-and-Recover
**[Paper]** (CVPR 2018) Distort-and-recover: Color Enhancement Using Deep Reinforcement Learning <Br>
**[Author]** Jongchan Park, [Joon-Young Lee](https://joonyoung-cv.github.io/), [Donggeun Yoo](https://dgyoo.github.io/), In So Kweon <Br>
**[[TF-Code](https://github.com/Jongchan/DISTORT-AND-RECOVER-CVPR18)]**<Br>
	
### DeepExposure
**[Paper]** (NIPS 2018) DeepExposure: Learning to Expose Photos with Asynchronously Reinforced Adversarial Learning <Br>
**[Author]** Runsheng Yu, Wenyu Liu, Yasen Zhang, Zhi Qu, [Deli Zhao](https://sites.google.com/site/zhaodeli/), Bo Zhang <Br>

### Progressive Retinex
**[Paper]** (MM 2019) Progressive Retinex: Mutually Reinforced Illumination-Noise Perception Network for Low Light Image Enhancement<Br>
**[Author]**  Yang Wang, Yang  Cao Zheng-Jun Zha, [Jing Zhang](https://chaimi2013.github.io/), [Zhiwei  Xiong](http://staff.ustc.edu.cn/~zwxiong/), Wei  Zhang, Feng  Wu <Br>
	
### KinD ★★
**[Paper]** (MM 2019) Kindling the Darkness: A Practical Low light Image Enhancer<Br>
**[Author]** Yonghua Zhang, Jiawan Zhang, [Xiaojie Guo](https://sites.google.com/view/xjguo) <Br>
**[[TF-Code-KinD](https://github.com/zhangyhuaee/KinD)]** **[[TF-Code-KinD++](https://github.com/zhangyhuaee/KinD_plus)]**<Br>
1) 采用类似Retinex的结构, 两个分支分别预测亮度分量和反射分量. 网络结构和loss可以参考. <Br>
2) 提出了一个小型的亮度adjustment net, 可以输入一个ratio, 控制增强程度, 比较有趣. <Br>
	
### DeepUPE ★
**[Paper]** (CVPR 2019) Underexposed Photo Enhancement Using Deep Illumination Estimation<Br>
**[Author]** Ruixing Wang, [Qing Zhang](http://zhangqing-home.net/), [Chi-Wing Fu](https://www.cse.cuhk.edu.hk/~cwfu/), [Xiaoyong Shen](http://xiaoyongshen.me/), [Wei-Shi Zheng](https://sites.google.com/site/sunnyweishi/), [Jiaya Jia](http://jiaya.me/) <Br>
**[[TF-code](https://github.com/wangruixing/DeepUPE)]** <Br>
同样基于Retinex理论, 但网络只预测illumination map, 使用了reconstruction, color和smooth loss. 整个工程都建立在HDRNet的基础上. 用联合上采样的思路做tone mapping的思路感觉可以挖掘一下.


### *Learning digital camera pipeline for extreme low-light imaging*
**[Paper]** (arXiv 1904) Learning digital camera pipeline for extreme low-light imaging <Br>
**[Author]**  Syed Waqas Zamir, [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Fahad Shahbaz Khan](https://sites.google.com/view/fahadkhans/home), Ling Shao <Br>


### EnlightenGAN ★★
**[Paper]** (arXiv 1906) EnlightenGAN: Deep Light Enhancement without Paired Supervision <Br>
**[Author]** [Yifan Jiang](http://yifanjiang.net/), [Xinyu Gong](https://gongxinyuu.github.io/), Ding Liu, [Yu Cheng](https://sites.google.com/site/chengyu05), [Chen Fang](http://fangchen.org/), [Xiaohui Shen](https://xiaohuishen.github.io/), [Jianchao Yang](http://www.ifp.illinois.edu/~jyang29/), Pan Zhou, Zhangyang Wang  <Br>
**[[Pytorch-code](https://github.com/TAMU-VITA/EnlightenGAN)]** <Br>
基于GAN的非监督亮度增强方法, 效果不错 <Br>
	
### Retinex-GAN ☆
**[Paper]** (arXiv 1906) Low-light Image Enhancement Algorithm Based on Retinex and Generative Adversarial Network <Br>
**[Author]** Yangming Shi, Xiaopo Wu, Ming Zhu  <Br>
RetinexNet+GAN
	
### Attention-guided Low-light Image Enhancement ★☆
**[Paper]** (arXiv 1908) Attention Guided Low-light Image Enhancement with a Large Scale Low-light Simulation Dataset <Br>
**[Author]** [Feifan Lv](https://lvfeifan.github.io/), [Yu Li](http://yu-li.github.io/), [Feng Lu](http://shi.buaa.edu.cn/lufeng/)  <Br>
**[[Project](http://phi-ai.org/project/AgLLNet/default.htm)]**<Br>
1) 同时做tone mapping和去噪, 分为亮度attention map预测, noise map预测, 多尺度增强模块和refine模块四部分, 网络结构和loss可以参考 <Br>
2) 提出了一个生成低光照加噪声数据的流程.

### Color-wise Attention Network for Low-light Image Enhancement ★
**[Paper]** (arXiv 1911) Color-wise Attention Network for Low-light Image Enhancement <Br>
**[Author]** [Yousef Atoum](http://faculty.yu.edu.jo/atoumyou/SitePages/Home.aspx), [Mao Ye](https://maoye.wordpress.com/), Liu Ren, [Ying Tai](https://tyshiwo.github.io/), [Xiaoming Liu](http://cvlab.cse.msu.edu/) <Br>
亮度和颜色通道分两只分别增强的方案, 其中color和point的attention部分没看懂

### Zero-DCE ★★
**[Paper]** (CVPR 2020) Zero-Reference Deep Curve Estimation for Low-Light Image Enhancement <Br>
**[Author]** Chunle Guo, [Chongyi Li](https://li-chongyi.github.io/), Jichang Guo, [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/index.html), [Junhui Hou](https://sites.google.com/site/junhuihoushomepage/), [Sam Kwong](https://www.cs.cityu.edu.hk/~cssamk/research_group/index.html), [Runmin Cong](https://rmcong.github.io/)   <Br>
**[[Project](https://li-chongyi.github.io/Proj_Zero-DCE.html)]** **[[Pytorch-Code](https://github.com/Li-Chongyi/Zero-DCE)]** **[[TF-Code](https://github.com/tuvovan/Zero_DCE_TF)]**<Br>
1) 一篇挺有趣的论文, 把tone mapping看成pixel-wise的曲线预测问题, 设计了一个小型曲线估计网络, 并提出了几个无监督loss, 得到了不错的结果 <Br>
2) 一些局限性: 提出的一系列约束loss对于增强部分区域可能不太适用, 比如对夜景图片增强前景的同时保持夜空是暗的

### *Decomposition-and-Enhancement* ★
**[Paper]** (CVPR 2020) Learning to Restore Low-Light Images via Decomposition-and-Enhancement <Br>
**[Author]** Ke Xu, [Xin Yang](http://faculty.dlut.edu.cn/yangxin/zh_CN/index.htm), Baocai Yin, [Rynson W.H. Lau](https://www.cs.cityu.edu.hk/~rynson/)   <Br>
在亮度增强的同时考虑去噪. 认为低频部分受噪声影响小(???)所以容易在低频部分进行增强. 低频部分增强后通过一个网络学习恢复高频部分. 设计了两个模块用于提取低频信息和扩大感受野.

	
### Learning to Correct Overexposed and Underexposed Photos ★☆
**[Paper]** (arXiv 2003) Learning to Correct Overexposed and Underexposed Photos <Br>
**[Author]** [Mahmoud Afifi](https://sites.google.com/view/mafifi), [Konstantinos G. Derpanis](https://www.cs.ryerson.ca/kosta/), [Björn Ommer](https://hci.iwr.uni-heidelberg.de/Staff/bommer),  [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/)   <Br>
**[[Code](https://github.com/mahmoudnafifi/Exposure_Correction)]** <Br>
粗读, coarse-to-fine增强的策略, 并在每个level加入相应的拉普拉斯金字塔层作为细节信息. 使用L1和GAN loss. 效果不错. <Br>
	
	
### DRBN ☆
**[Paper]** (CVPR 2020) From Fidelity to Perceptual Quality: A Semi-Supervised Approach for Low-Light Image Enhancement <Br>
**[Author]** [Wenhan Yang](https://flyywh.github.io/), Shiqi Wang, [Yuming Fang](https://sites.google.com/site/leofangyuming/), Yue Wang, Jiaying Liu   <Br>
分为有监督部分和无监督(GAN)两部分. 结构比较繁琐. 


### EEMEFN★
**[Paper]** (AAAI 2020) EEMEFN: Low-Light Image Enhancement via Edge-Enhanced Multi-Exposure Fusion Network <Br>
**[Author]** Minfeng Zhu, Pingbo Pan, [Wei Chen](http://www.cad.zju.edu.cn/home/chenwei/), Yi Yang   <Br>
大致浏览. 输入为raw, 设计了一个多分支网络, 分别处理不同曝光值得输入并将结果融合, 里面的参考曝光值不知道是怎么得到的. 另外还加入一个边缘增强网络, 方法是现成的. 

### *Self-supervised Image Enhancement Network: Training With Low Light Images Only*
**[Paper]** (arXiv 2002) Self-supervised Image Enhancement Network: Training With Low Light Images Only <Br>
**[Author]** Yu Zhang, Xiaoguang Di, Bin Zhang, Chunhui Wang  <Br>
**[[TF-Code](https://github.com/hitzhangyu/Self-supervised-Image-Enhancement-Network-Training-With-Low-Light-Images-Only)]** <Br>	

### *Unsupervised Real-world Low-light Image Enhancement with Decoupled Networks* ★
**[Paper]** (arXiv 2005) Unsupervised Real-world Low-light Image Enhancement with Decoupled Networks <Br>
**[Author]** [Wei Xiong](https://wxiong.me/publications/), Ding Liu, Xiaohui Shen, [Chen Fang](http://fangchen.org/), [Jiebo Luo](https://www.cs.rochester.edu/u/jluo/)  <Br>
无监督做亮度增强和去噪. 分为亮度增强和去噪两阶段, 亮度采用Retinex思想, 使用global和local的GAN做loss. 去噪部分提出构建Pseudo Triples的方法, 结合GAN去噪.
	
### Deep Bilateral Retinex for Low-Light Image Enhancement
**[Paper]** (arXiv 2007) Deep Bilateral Retinex for Low-Light Image Enhancement <Br>
**[Author]** Jinxiu Liang, Yong Xu, [Yuhui Quan](https://csyhquan.github.io/), Jingwen Wang, [Haibin Ling](https://www3.cs.stonybrook.edu/~hling/), [Hui Ji](https://blog.nus.edu.sg/matjh/)  <Br>

### *Fast Enhancement for Non-Uniform Illumination* ★★
**[Paper]** (MM 2020) Fast Enhancement for Non-Uniform Illumination Images using Light-weight CNNs <Br>
**[Author]** [Feifan Lv](https://lvfeifan.github.io/), Bo Liu, [Feng Lu](http://shi.buaa.edu.cn/lufeng/)  <Br>
1) 超轻量级网络(~5k参数), 同时成立过曝光和欠曝光问题, 效果不错
2) 用一个illumination net预测原图和1-原图的illumination, 用来解决retinex理论不能处理过曝的局限. 然后把欠曝光修复结果, 过曝修复结果和原图送到fusion net中预测三个分量的权重, 进行加权融合. 最后用一个restoration net去除噪声和artifacts

### *Integrating Semantic Segmentation and Retinex Model* ★
**[Paper]** (MM 2020) Integrating Semantic Segmentation and Retinex Model for Low Light Image Enhancement <Br>
**[Author]** [Minhao Fan](https://xfw-go.github.io/), [Wenjing Wang](https://daooshee.github.io/website/), [Wenhan Yang](https://flyywh.github.io/), [Jiaying Liu](http://39.96.165.147/people/liujiaying.html)  <Br>
**[[Project](https://mm20-semanticreti.github.io/)]** <Br>
将分割特征与Retinex网络结合做亮度增强

## Traditional Methods

### *Image-Contrast-Enhancement* ★★
**[Paper]** (CAIP2017) A New Image Contrast Enhancement Algorithm Using Exposure Fusion Framework <Br>
**[Author]** [Zhenqiang Ying](https://baidut.github.io/about/), Ge Li, Yurui Ren, Ronggang Wang, Wenmin Wang   <Br>
**[[Project](https://baidut.github.io/OpenCE/caip2017.html)]** **[[Matlab-Code](https://github.com/AndyHuang1995/Image-Contrast-Enhancement)]** **[[Python-Code](https://github.com/AndyHuang1995/Image-Contrast-Enhancement)]** <Br>
大致浏览, 利用原图和曝光增强后的图像融合, 提升亮度和对比度. 融合权值通过求解光照强度得到, 曝光增强图通过作者之前提出的相机响应校正模型得到.
	


# Useful Resources
[各种对比度增强算法代码 Matlab] https://github.com/baidut/OpenCE
