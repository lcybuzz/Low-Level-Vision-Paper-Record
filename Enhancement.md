# Image Enhancement



### DPED ★★
**[Paper]** (ICCV 2017) DSLR-Quality Photos on Mobile Devices with Deep Convolutional Networks <Br>
**[Author]** Andrey Ignatov, Nikolay Kobyshev, Kenneth Vanhoey, Radu Timofte , Luc Van Gool  <Br>
**[[Code](http://people.ee.ethz.ch/~ihnatova/index.html)]**   <Br>
1) 从变换的角度出发, 学习一个从低质量图像到高质量图片的变换函数 
2) 变换部分采用残差快结构的CNN，定义了4个loss (color, texture, content, variance). color loss是图像进行高斯模糊后的均方差, texture loss是adversarial loss, content loss是perceptual loss, variance loss是图像梯度的模.
3) 提出了用于图像质量增强的数据集DPED, 包括iPhone, BlackBerry和Sony三种手机与Canon单反相机的图相对.
 
	
### HDRNet ★★
**[Paper]** (Siggraph 2017) Deep Bilateral Learning for Real-Time Image Enhancement <Br>
**[Author]** 	Michaël Gharbi, [Jiawen Chen](http://people.csail.mit.edu/jiawen/), [Jonathan T. Barron](https://jonbarron.info/),  [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Frédo Durand](http://people.csail.mit.edu/fredo/)  <Br>
**[[Project](https://groups.csail.mit.edu/graphics/hdrnet/)]**<Br>
1) 提出了一个实时图像增强网络, 速度快, 效果好. <Br>
2) 网络分为两个分支, 低分辨率分支提取特征, 学习每个像素的色彩映射参数; 高分辨率分支负责提取和保留细节信息. low res分支学到的映射参数通过类似于双线性差值的过程上采样到high res, 最后对high res图像做色彩映射并输出. <Br>
3) 学习映射参数部分, 采用bilateral grid的思路. 第三个维度被解释成8*12的网格, 意思是对8个灰度level做不同的色彩映射. 处理时选择哪个level的参数, 由high res分支生成的引导图决定. <Br> 
 
### EnhanceGAN ★ 
**[Paper]** (arXiv 1707) Aesthetic-Driven Image Enhancement by Adversarial Learning <Br>
**[Author]** 	Yubin Deng, [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/index.html),	[Xiaoou Tang](https://www.ie.cuhk.edu.hk/people/xotang.shtml)  <Br>
1) weakly supervised方法, 学习crop和色彩变换参数, 增强aesthetic quality

### FEQE ☆
**[Paper]** (ECCVW 2018)  Fast and Efficient Image Quality Enhancement via Desubpixel Convolutional Neural Networks, <Br>
**[Author]** [Thang Vu](https://thangvubk.github.io/), Cao V. Nguyen, Trung X. Pham, Tung M. Luu, and Chang D. Yoo  <Br>
**[[TF-Code](https://github.com/thangvubk/FEQE)]**   <Br>
使用pixel shuffle的实时图像增强网络


### WESPE ★
**[Paper]** (CVPRW 2018) WESPE: Weakly Supervised Photo Enhancer for Digital Cameras <Br>
**[Author]** Andrey Ignatov, Nikolay Kobyshev, Radu Timofte , Kenneth Vanhoey, Luc Van Gool  <Br>
**[[Project](http://people.ee.ethz.ch/~ihnatova/index.html)]**   <Br>
	
	
### RSGUNet ★
**[Paper]** (ECCVW 2018) Range Scaling Global U-Net for Perceptual Image Enhancement on Mobile Devices <Br>
**[Author]** Jie Huang, Pengfei Zhu, Mingrui Geng, Jiewen Ran, Xingguang Zhou, Chen Xing, Pengfei Wan, Xiangyang Ji  <Br>
**[[TF-Code](https://github.com/MTlab/rsgunet_image_enhance)]**   <Br>
UNet + Global Pooling feature + 输入输出feature间的elementwise scaling

### FUnIE-GAN ★
**[Paper]** (RAL 2020) Fast Underwater Image Enhancement for Improved Visual Perception <Br>
**[Author]** [Md Jahidul Islam](https://xahidbuffon.github.io/), [Youya Xia](https://www.xiayouya.com/), [Junaed Sattar](https://junaedsattar.cs.umn.edu/)  <Br>
**[[Code](https://github.com/xahidbuffon/FUnIE-GAN)]**   <Br>
encoder-decoder结构, 使用了几个目标函数从各方面增强图像视觉质量. 提出了一个水下图像数据集.
	

### *Content-preserving Tone Adjustment* ★☆
**[Paper]** (CVPRW 2019) Content-preserving Tone Adjustment for Image Enhancement <Br>
**[Author]** [Simone Bianco](http://www.ivl.disco.unimib.it/people/simone-bianco/), [Claudio Cusano](http://www.ivl.disco.unimib.it/people/claudio-cusano/), [Flavio Piccoli](http://www.ivl.disco.unimib.it/people/flavio-piccoli/), [Raimondo Schettini](http://www.ivl.disco.unimib.it/people/raimondo-schettini/)  <Br>
**[[PyTorch-Code](https://github.com/dros1986/content-preserving-tone-adjustment-for-image-enhancement)]**   <Br>
有点类似HRDNet, 在小分辨率预测输入值的分段映射系数, 在原图上增强. 速度快, 应该有较强的实用性.

### DeepLPF ★☆
**[Paper]** (CVPR 2020) DeepLPF: Deep Local Parametric Filters for Image Enhancement <Br>
**[Author]** [Sean Moran](http://www.seanjmoran.com/), Pierre Marza, [Steven McDonagh], Sarah Parisot, [Gregory Slabaugh](http://gregslabaugh.net/)  <Br>
**[[PyTorch-Code](https://github.com/huawei-noah/noah-research/tree/071a49fb8f0975192dcc919a18f9a082093122e6/DeepLPF)]**   <Br>
1) 华为欧洲实验室的文章, 把lightroom等修图软件中的brugh, graduated filters, radial filters工具用CNN模拟出来. 分为三个分支, 一个分支预测pixelwise的增强, 两个分支分别预测两种fiter的参数. 
2) 个人觉得预测的filter仍然不太够local. 不过论文的思路挺有意思.
