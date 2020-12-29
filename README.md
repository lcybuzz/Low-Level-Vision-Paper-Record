# Personal repository under construction.

# Table of Contents
- <a href='Enhancement & Restoration.md'> Enhancement & Restoration </a>
- <a href='LowLight.md'> Low Light </a>
- <a href='Denoising.md'> Denoising </a>
- <a href='SuperResolution.md'> Super Resolution </a>
- <a href='FaceRestoration.md'> Face Restoration </a>
- <a href='HDR.md'> HDR </a>
- <a href='UsingRaw.md'> Using Raw </a>
- <a href='ISP.md'> ISP </a>
- <a href='Industry.md'> Industry</a>
- <a href='General.md'> General </a>
- <a href='Few-Shot.md'> Few-Shot</a>
- <a href='Misc.md'> Misc </a>
- <a href='Dehazing.md'> Dehazing (Archived) </a>
- <a href='Debluring.md'> Debluring (Archived) </a>
- <a href='Fusion.md'> Fusion (Archived) </a>
- [Dataset](#dataset)
- [Useful Resources](#useful-resources)

	


# Dataset
## Image Enhancement
[MIT-Adobe FiveK Dataset](https://data.csail.mit.edu/graphics/fivek/) 单反相机拍摄的raw图像 + 5个人工retouch的tiff图, 共5k张 <Br>
[DPED](http://people.ee.ethz.ch/~ihnatova/) 手机相机和单反相机增强数据集, 使用sift做对齐, 包括来自三种手机和Canon单反的超过15k张图像对 <Br>


## Low Light
[SID](http://vladlen.info/publications/learning-see-dark/)  <Br>
[ExDark](https://github.com/cs-chan/Exclusively-Dark-Image-Dataset) <Br>
[CID](https://github.com/505030475/ExtremeLowLight) <Br>
[VV](https://sites.google.com/site/vonikakis/datasets)  <Br>
[LOL](https://daooshee.github.io/BMVC2018website/)  <Br>
[LIME](http://cs.tju.edu.cn/orgs/vision/~xguo/LIME.htm)  <Br>
[RENOIR](http://adrianbarburesearch.blogspot.com/p/renoir-dataset.html) <Br>
[ExDARK](https://github.com/cs-chan/Exclusively-Dark-Image-Dataset) <Br>
[SICE](https://github.com/csjcai/SICE) <Br>
[The Extended Yale Face Database B](http://vision.ucsd.edu/~iskwak/ExtYaleDatabase/ExtYaleB.html) <Br>


## Super Resolution
[DIV2k](https://data.vision.ee.ethz.ch/cvl/DIV2K/)  <Br>

## Face Super Resolution
[CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) 人脸属性数据集, 超过200k张图像, 5个关键点, 40个属性 <Br>
[CelebAMask-HQ](https://github.com/switchablenorms/CelebAMask-HQ) 3w张人脸解析数据集, 包括19个facial components <Br>
[Flickr-Faces-HQ Dataset (FFHQ)](https://github.com/NVlabs/ffhq-dataset) <Br>
	

## Real Image Denoising
[DnD](https://noise.visinf.tu-darmstadt.de/) <Br>
[SIDD](https://www.eecs.yorku.ca/~kamel/sidd/) <Br>

[PolyU](https://github.com/csjunxu/PolyU-Real-World-Noisy-Images-Dataset) <Br>
[Renoir](http://ani.stat.fsu.edu/~abarbu/Renoir.html) <Br>
[CC](http://snam.ml/research/ccnoise) <Br>
[SID](http://cchen156.web.engr.illinois.edu/SID.html) <Br>
[kodak_color](http://r0k.us/graphics/kodak/) <Br>
[NoiseClinicImages](http://demo.ipol.im/demo/125/input_select?044_solvay_1927.x=63&044_solvay_1927.y=68) <Br>
	
## Signle Image Deblurring
[HIDE](https://github.com/joanshen0508/HA_deblur) motion deblur <Br>
[GOPRO](https://github.com/SeungjunNah/DeepDeblur_release) motion deblur <Br>

## Reflection Removal
[SIR](https://sir2data.github.io/) <Br>

## AWB
[GehlerShi](https://www2.cs.sfu.ca/~colour/data/shi_gehler/) <Br>
[CUBE+](https://ipg.fer.hr/ipg/resources/color_constancy) <Br>


# Useful Resources
[[ECCV 2020图像重建方向](https://zhuanlan.zhihu.com/p/180551773)]

[[CVPR 2020论文集合](https://github.com/extreme-assistant/CVPR2020-Paper-Code-Interpretation)]

[[低光照论文整理1](https://github.com/cxtalk/You-Can-See-Clearly-Now)] [[低光照论文整理2](https://github.com/Elin24/Awesome-Low-Light-Enhancement)]

[[超分论文整理](https://github.com/it-hao/Super-Resolution)]

[[去噪论文整理](https://paperswithcode.com/task/image-denoising?page=2)] [[去噪论文with codes](https://github.com/wenbihan/reproducible-image-denoising-state-of-the-art)]

[[Deblurring](https://github.com/subeeshvasu/Awesome-Deblurring)]

[[去雾](https://github.com/cxtalk/DehazeZoo)]

[[传统图像处理算法实现](https://github.com/BBuf/Image-processing-algorithm)]

[[一些基于C++的对比度增强算法实现](https://github.com/dengyueyun666/Image-Contrast-Enhancement)]

[[传统图像质量增强的系列blog-1](https://www.cnblogs.com/Imageshop/category/535367.html)] [[传统图像质量增强的系列blog-2](https://blog.csdn.net/maozefa/article/list/1)]

[[ISP介绍blog](https://blog.csdn.net/qq_42261630/article/details/102918149)]

[[数据集](https://github.com/daooshee/Image-Processing-Datasets)]

[[移动端AI benchmark](http://ai-benchmark.com/index.html#title)]

# Competition
**[CVPR NTIRE]** New Trends in Image Restoration and Enhancement Challenges, 图像超分辨率、图像去噪、去模糊、去摩尔纹、重建、去雾 <Br>
**[CVPR LPCVC]** Low Power Computer Vision Challenge, 低功耗计算机视觉、目标检测、图像分类 <Br>
**[ECCV AIM]** Advances in Image Manipulation workshop and challenges <Br>
**[ECCV PIRM]** Perceptual Image Restoration and Manipulation, 貌似只有18, 19两届 <Br>

# To See
[CVPR 2020 GAN in 图像恢复论文盘点] https://blog.csdn.net/lgzlgz3102/article/details/106799006/
