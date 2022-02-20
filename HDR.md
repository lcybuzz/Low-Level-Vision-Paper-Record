
# Table of Contents
  - [HDR](#hdr)
  - [Tone Mapping](#tone-mapping)

    
# HDR
## Multi-frame HDR
### DL Methods
#### ADNet
**[Paper]** (CVPR2021) ADNet: Attention-guided Deformable Convolutional Network for High Dynamic Range Imaging <Br>
**[Author]** Zhen Liu, Wenjie Lin, Xinpeng Li, Qing Rao, Ting Jiang, Mingyan Han, Haoqiang Fan, [Jian Sun](http://www.jiansun.org/), [Shuaicheng Liu](http://www.liushuaicheng.org/) <Br>
**[[Pytorch-Code](https://github.com/liuzhen03/ADNet)]**<Br>

#### AHDRNet ★★
**[Paper]** (CVPR 2019) Attention-guided Network for Ghost-free High Dynamic Range Imaging <Br>
**[Author]** [Qingsen Yan](https://qingsenyangit.github.io/), [Dong Gong](https://donggong1.github.io/), [Qinfeng Shi](https://cs.adelaide.edu.au/~javen/), [Anton van den Hengel](https://cs.adelaide.edu.au/~hengel/), [Chunhua Shen](https://cshen.github.io/), [Ian Reid](https://cs.adelaide.edu.au/~ianr/), Yanning Zhang <Br>
**[[Project](https://qingsenyangit.github.io/project/ahdr/)]** **[[Pytorch-Code](https://github.com/qingsenyangit/AHDRNet)]**<Br>
**多帧HDR**.基于空间attention的多帧HDR, 网络使用dilated residual dense blocks, 预测残差, loss使用μ-law压缩的L1 loss. 结构简洁, 效果不错.

#### Deep High Dynamic Range Imaging of Dynamic Scenes
**[Paper]** (Siggraph 2017) Deep High Dynamic Range Imaging of Dynamic Scenes <Br>
**[Author]** [Nima Khademi Kalantari](https://people.engr.tamu.edu/nimak/index.html), [Ravi Ramamoorthi](https://cseweb.ucsd.edu//~ravir/) <Br>
**[[Project](https://cseweb.ucsd.edu//~viscomp/projects/SIG17HDR/)]** <Br>
	

### Traditional Methods
####  Noise-Optimal Capture
**[Paper]** (CVPR 2010) Noise-Optimal Capture for High Dynamic Range Photography <Br>
**[Author]** [Samuel W. Hasinoff](http://people.csail.mit.edu/hasinoff/), [Frédo Durand](http://people.csail.mit.edu/fredo/), [William T. Freeman](http://billf.mit.edu/)  <Br>
**[[Project](http://people.csail.mit.edu/hasinoff/hdrnoise/)]** <Br>

#### Recovering High Dynamic Range Radiance Maps from Photographs
**[Paper]** (TOG 2008) Recovering High Dynamic Range Radiance Maps from Photographs <Br>
**[Author]** [Paul Debevec](http://www.pauldebevec.com/), [Jitendra Malik](https://people.eecs.berkeley.edu/~malik/)<Br>
**[[Project](http://www.pauldebevec.com/Research/HDR/)]** <Br>

#### Exposure Fusion
**[Paper]** (PG 2007) Exposure Fusion <Br>
**[Author]** [Tom Mertens](http://www.mericam.net/), [Jan Kautz](https://jankautz.com/), Frank Van Reeth<Br>

#### High Dynamic Range Imaging ★
**[Paper]** (CIC 2001) High Dynamic Range Imaging <Br>
**[Author]** Greg Ward  <Br>
讲了color rendering的pipeline, 包括: 怎么估计真实场景目标的光强, 转换到颜色空间的近似表示, 将信息记录为HDR格式, tone mapping以在设备上显示等
	
#### SVE ★
**[Paper]** (CVPR 2000) High Dynamic Range Imaging: Spatially Varying Pixel Exposures <Br>
**[Author]** [Shree K. Nayar](http://www.cs.columbia.edu/~nayar/), Tomoo Mitsunaga  <Br>
提出一个基于硬件的HDR图像生成方法. 在相机传感器前放置一个optical mask, mask上有不同exposure的pattern, 利用邻域不同曝光的像素值, 恢复目标像素值, 动态范围可大致扩展到Emax/Emin倍.



## Single-frame HDR
### DL Methods
#### HDRUNet ★
**[Paper]** (CVPRW 2021) HDRUNet: Single Image HDR Reconstruction with Denoising and Dequantization <Br>
**[Author]** Xiangyu Chen, Yihao Liu, Zhengwen Zhang, [Yu Qiao](http://mmlab.siat.ac.cn/), [Chao Dong](http://xpixel.group/) <Br>
**[[Pytorch-Code](https://github.com/chxy95/HDRUNet)]**<Br>
**单帧HDR**.base网络为UNet, 还有一个weight net和一个由SFT组成的condition net. loss用tanh L1.

#### *Single-Image HDR Reconstruction by Learning to Reverse the Camera Pipeline* ★
**[Paper]** (CVPR 2020) Single-Image HDR Reconstruction by Learning to Reverse the Camera Pipeline <Br>
**[Author]** [Yu-Lun Liu](http://www.cmlab.csie.ntu.edu.tw/~yulunliu/), [Wei-Sheng Lai](https://www.wslai.net/), [Yu-Sheng Chen](https://www.cmlab.csie.ntu.edu.tw/~nothinglo/), Yi-Lung Kao, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/) <Br>
**[[Project](https://www.cmlab.csie.ntu.edu.tw/~yulunliu/SingleHDR)]** **[[TF-Code](https://github.com/alex04072000/SingleHDR)]**<Br>
**单帧HDR**.用几个CNN模拟ISP中HDR到LDR的映射过程, 完成HDR. 关键是定义每个部分的训练目标和数据, 这部分没细看.

#### UnModNet
**[Paper]** (NeruIPS 2020) UnModNet: Learning to Unwrap a Modulo Image for High Dynamic Range Imaging <Br>
**[Author]**  Chu Zhou, Hang Zhao, Jin Han, [Chang Xu](http://changxu.xyz/), Chao Xu, Tiejun Huang, [Boxin Shi](http://ci.idm.pku.edu.cn/Publication.htm) <Br>
**[[Project](https://www.cmlab.csie.ntu.edu.tw/~yulunliu/SingleHDR)]** **[[TF-Code](https://github.com/alex04072000/SingleHDR)]**<Br>

#### ExpandNet
**[Paper]** (EG 2018) ExpandNet: A Deep Convolutional Neural Network for High Dynamic Range Expansion from Low Dynamic Range Content <Br>
**[Author]** 	Demetris Marnerides, [Thomas Bashford-Rogers](http://thomasbashfordrogers.com/), [Jonathan Hatchett](https://hatchett.co.uk/), [Kurt Debattista](https://warwick.ac.uk/fac/sci/wmg/people/profile/?wmgid=518)  <Br>
**[[Pytorch-Code](https://github.com/dmarnerides/hdr-expandnet)]** **[[Unofficial-TF-Code](https://github.com/echolijinghui/ExpandNet)]**<Br>

#### *Image Correction via Deep Reciprocating HDR Transformation*
**[Paper]** (CVPR 2018) Image Correction via Deep Reciprocating HDR Transformation <Br>
**[Author]** [Xin Yang](http://faculty.dlut.edu.cn/yangxin/zh_CN/index.htm), Ke Xu, [Yibing Song](https://ybsong00.github.io/), Qiang Zhang, Xiaopeng Wei, [Rynson Lau](https://www.cs.cityu.edu.hk/~rynson/)  <Br>
**[[Project](https://ybsong00.github.io/cvpr18_imgcorrect/index.html)]** **[[TF-Code](https://github.com/ybsong00/DRHT)]**<Br>

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
## Traditional Methods
#### High Dynamic Range Video ★★
**[Paper]** (TOG 2003) High Dynamic Range Video <Br>
**[Author]** [Sing Bing Kang](http://www.singbingkang.com/), [Matthew Uyttendaele](https://research.facebook.com/people/uyttendaele-matt/), [Simon Winder](http://simonwinder.com/), [Richard Szeliski](http://szeliski.org/RichardSzeliski.htm)  <Br>
提出了一个视频HDR pipeline. 1.根据场景亮度, 设置相邻帧的曝光值; 2.将相邻帧处理到相同亮度, 做运动检测和warping. 对于当前帧saturate的部分, 使用前后两帧之间的光流估计到当前帧的光流并做warp, 没有saturate的部分, 利用前后帧到当前帧的光流直接warp, 并用一些策略fuse; 3.将HDR的radiance map通过tone mapping转换为能显示的LDR视频, 使用前后若干帧统计平均log域亮度, 做全局scale, 局部只根据当前帧scale
	

	
# Tone Mapping
## Traditional Methods
#### Photographic tone reproduction for digital images ★★
**[Paper]** (TOG 2002) Photographic tone reproduction for digital images  <Br>
**[Author]** [Erik Reinhard](http://erikreinhard.com/), Michael Stark, [Peter Shirley](https://www.petershirley.com/), [James Ferwerda](https://jamesferwerda.com/) <Br>
1. 在log域计算平均照度, 并用其对全图进行scale; 2. 自适应dodging-and-burning, 实现局部tone mapping
