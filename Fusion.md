# Image Fusion


### Digital Photography with Flash and No-Flash Image Pairs ★★
**[Paper]** (SIGGRAPH 2004) Digital Photography with Flash and No-Flash Image Pairs<Br>
**[Author]** Georg Petschnigg, [Maneesh Agrawala](http://vis.berkeley.edu/~maneesh/), [Hugues Hoppe](http://hhoppe.com/), [Richard Szeliski](http://szeliski.org/RichardSzeliski.htm), Michael Cohen, Kentaro Toyama <Br>
**[[Project](http://hhoppe.com/proj/flash/)]** **[[Code](https://github.com/pranaygupta36/DIP_PROJECT_REPO)]**<Br>
提出了一个融合Flash和Non-Flash照片的流程, 包括双边滤波, 联合双边滤波, detail提取和detail transfer. 可用于去躁, 白平衡, 去红眼, 调整flash强度等多种图像增强应用中. <Br>
	
### *BJND* ★☆
**[Paper]** (Optics express 2017) Enhancement of low light level images using color-plus-mono dual camera <Br>
**[Author]**   [Yong Ju Jung](https://sites.google.com/site/coolyjjung/)<Br>
1) 提出了一个融合Mono和Color图像的流程, 包括直方图匹配, 配准, Color+Color和Color+Mono的引导滤波, BJND-aware merge和detail trainsfer几个步骤. <Br>
2) 大致流程与 Digital Photography with Flash and No-Flash Image Pairs 这篇paper类似, 创新点是提出用BJND引导detail transfer. BJND即binocular just-noticeable-difference, 是根据人眼视觉系统的特性提出的. 具体方法中有很多参数和细节. <Br>
	
### *Stereo Matching with Color and Monochrome Cameras in Low-light Conditions* ★
**[Paper]** (CVPR 2016) Stereo Matching with Color and Monochrome Cameras in Low-light Conditions <Br>
**[Author]**   [Hae-Gon Jeon](https://sites.google.com/site/hgjeoncv/), [Joon-Young Lee](https://joonyoung-cv.github.io/), [Sunghoon Im](https://sunghoonim.github.io/), [Hyowon Ha](https://sites.google.com/site/hyowoncv/), [In So Kweon](https://scholar.google.com/citations?user=XA8EOlEAAAAJ&hl=zh-CN&oi=ao) <Br>
  
### Deep Convolutional Network for Colorization in Monochrome-Color Dual-Lens System ★
**[Paper]** (AAAI 2019) Learning a Deep Convolutional Network for Colorization in Monochrome-Color Dual-Lens System <Br>
**[Author]**  Xuan Dong, Weixin Li, Xiaojie Wang, Yunhong Wang <Br>
1) 提出了一个Mono和Color图像融合的网络, 将融合看做对Mono图像的上色问题. 未开源, 非轻量级. <Br>
2) 分为rough和fine两部分, 首先将color图像在x方向加权求和作为rough result, 其中权值是使用3D卷积预测的weight volume; 接下来再用rough result和mono图像作为输入进行refine. <Br>

### Stereoscopic Dark Flash ★
**[Paper]** (Siggraph 2017) DStereoscopic Dark Flash for Low-light Photography <Br>
**[Author]** Jian Wang, Tianfan Xue, [Jonathan T. Barron](https://jonbarron.info/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/)<Br>
1) 大致浏览, 提出了一个RGB和NIR-NUV双相机成像方案, 以增强低光照条件下的图像质量. <Br>
2) 分为registration, 基于scalemap的融合, 基于HDRNet的tone correction三部分. <Br>

### Exposure Fusion ★★
**[Paper]** (Pacific Graphics 2007) Exposure Fusion <Br>
**[Author]** [Tom Mertens](http://www.mericam.net/)，[Jan Kautz](http://jankautz.com/)，Frank Van Reeth <Br>
**[[Code](https://github.com/Mericam/exposure-fusion)]**   <Br>
1) 提出了一个融合exposure bracketing图像的经典方案, 可以直接融合图像序列而无需现将其转换为HDR图像再tone mapping. <Br>
2) 使用三个指标确定每张图像的权重图, 三个指标为对比度, 饱和度和well-exposureness, 最后的权重为三个指标相乘.<Br>
3) 为消除直接逐像素融合产生的seam, 将图像和权重图分别计算分解为拉普拉斯和高斯金字塔, 在每个level做融合.
