# Personal repository under construction.

# Table of Contents
- <a href='ImageRestoration.md'> Image Restoration </a>
- <a href='ImageEnhancement.md'> Image Enhancement </a>
- <a href='Denoising.md'> Image & Video Denoising </a>
- <a href='SuperResolution.md'> Image Super Resolution </a>
- <a href='HDR.md'> HDR </a>
- <a href='ISP.md'> ISP </a>
- <a href='VideoRelated.md'> Video Related </a>
- <a href='Industry.md'> Industry</a>
- <a href='General.md'> General </a>
- <a href='FewShot.md'> Few Shot</a>
- <a href='Misc.md'> Misc </a>
- <a href='FaceRelated.md'> Face Related (archived) </a>
- <a href='ImageSynthesis.md'> Image Synthesis (archived)</a>




# Datasets
## Image datasets

- [[图像处理任务数据集](https://github.com/daooshee/Image-Processing-Datasets)]

- Image Enhancement
    - [MIT-Adobe FiveK Dataset](https://data.csail.mit.edu/graphics/fivek/) 单反相机拍摄的raw图像 + 5个人工retouch的tiff图, 共5k张 <Br>
    - [DPED](http://people.ee.ethz.ch/~ihnatova/) 手机相机和单反相机增强数据集, 使用sift做对齐, 包括来自三种手机和Canon单反的超过15k张图像对 <Br>

- Low Light
    - [SID](http://vladlen.info/publications/learning-see-dark/)  <Br>
    - [ExDark](https://github.com/cs-chan/Exclusively-Dark-Image-Dataset) <Br>

    - [CID](https://github.com/505030475/ExtremeLowLight) <Br>
    - [VV](https://sites.google.com/site/vonikakis/datasets)  <Br>
    - [LOL](https://daooshee.github.io/BMVC2018website/)  <Br>
    - [LIME](http://cs.tju.edu.cn/orgs/vision/~xguo/LIME.htm)  <Br>
    - [RENOIR](http://adrianbarburesearch.blogspot.com/p/renoir-dataset.html)
    - [ExDARK](https://github.com/cs-chan/Exclusively-Dark-Image-Dataset) <Br>
    - [SICE](https://github.com/csjcai/SICE) <Br>
    - [The Extended Yale Face Database B](http://vision.ucsd.edu/~iskwak/ExtYaleDatabase/ExtYaleB.html) <Br>

- Super Resolution
    - [DIV2k](https://data.vision.ee.ethz.ch/cvl/DIV2K/)  NTIRE17 (800 train and 100 validation) <Br>
    - [Flicker2K](https://github.com/limbee/NTIRE2017)  NTIRE17 (2650 2K分辨率) <Br>
    - [Urban100](https://github.com/jbhuang0604/SelfExSR) <Br>

- Real Image Denoising
    - [DnD](https://noise.visinf.tu-darmstadt.de/)  <Br>
    - [SIDD](https://www.eecs.yorku.ca/~kamel/sidd/) <Br>
    - [PolyU](https://github.com/csjunxu/PolyU-Real-World-Noisy-Images-Dataset) <Br>
    - [Renoir](http://ani.stat.fsu.edu/~abarbu/Renoir.html) <Br>
    - [CC](http://snam.ml/research/ccnoise) <Br>
    - [SID](http://cchen156.web.engr.illinois.edu/SID.html) <Br>
    - [kodak_color](http://r0k.us/graphics/kodak/) <Br>
    - [NoiseClinicImages](http://demo.ipol.im/demo/125/input_select?044_solvay_1927.x=63&044_solvay_1927.y=68) <Br>

- Real Video Denoising
    - [CRVD dataset](https://github.com/cao-cong/RViDeNet) Raw视频去噪数据集. 11个室内场景, 5个ISO.  <Br>

- Deblurring
    - [HIDE](https://github.com/joanshen0508/HA_deblur) image motion deblur <Br>
    - [GOPRO](https://github.com/SeungjunNah/DeepDeblur_release) image motion deblur, 240fps, 1280x720 <Br>
    - [Deep Video Deblurring(Adobe240fps)](http://www.cs.ubc.ca/labs/imager/tr/2017/DeepVideoDeblurring/#dataset) video deblur <Br>
    - [REDS](https://seungjunnah.github.io/Datasets/reds) 视频去模糊, 视频超分, 120fps, 1280x720<Br>
    - [BSD](https://github.com/zzh-tech/ESTRNN) real-world video deblur <Br>

- Face Redrawing
    - [CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) 人脸属性数据集, 超过200k张图像, 5个关键点, 40个属性 <Br>
    - [CelebAMask-HQ](https://github.com/switchablenorms/CelebAMask-HQ) 3w张人脸解析数据集, 包括19个facial components <Br>
    - [Flickr-Faces-HQ Dataset (FFHQ)](https://github.com/NVlabs/ffhq-dataset) <Br>
    - [PPR10K](https://github.com/csjliang/PPR10K) <Br>

- Reflection Removal
    - [SIR](https://sir2data.github.io/) <Br>

- AWB
    - [GehlerShi](https://www2.cs.sfu.ca/~colour/data/shi_gehler/) <Br>
    - [CUBE+](https://ipg.fer.hr/ipg/resources/color_constancy) <Br>

- Demosaicing releated
    - [MIT moire](https://groups.csail.mit.edu/graphics/demosaicnet/dataset.html) <Br>
    - [McMaster](https://groups.csail.mit.edu/graphics/demosaicnet/dataset.html) 18张RGB, 500x500, 一般用于测试 <Br>
    - [Kodak](https://r0k.us/graphics/kodak/) 24张真全彩色RGB图像, 768x512, 一般用于测试<Br>

## Video datasets
- [Vimeo-90k](http://toflow.csail.mit.edu/) 超分, 插帧,  30fps  <Br>
- [Middlebury](https://vision.middlebury.edu/flow/) 光流估计, 视频插帧 <Br>
- [UCF101](https://www.crcv.ucf.edu/data/UCF101.php) 视频动作识别  <Br>
- [X4K1000FPS](https://github.com/JihyongOh/XVFI) 4k分辨率,1000fps <Br>
- [DAVIS](https://davischallenge.org/index.html) 视频分割, 1080p, 24fps <Br>







# Competitions
- **[CVPR NTIRE]** New Trends in Image Restoration and Enhancement Challenges, 图像超分辨率、图像去噪、去模糊、去摩尔纹、重建、去雾 <Br>
- **[MAI]** Mobile AI Workshop (CVPR workshop). <Br>
- **[CVPR LPCVC]** Low Power Computer Vision Challenge, 低功耗计算机视觉、目标检测、图像分类 <Br>
- **[ECCV AIM]** Advances in Image Manipulation workshop and challenges <Br>
- **[ECCV PIRM]** Perceptual Image Restoration and Manipulation, 貌似只有18, 19两届 <Br>



# Resources
## Paper collection
- Conference paper collection
    - [[CVPR 2023](https://github.com/extreme-assistant/CVPR2023-Paper-Code-Interpretation/blob/master/CVPR2023.md)] 
    [[CVPR 2023](https://github.com/amusi/CVPR2023-Papers-with-Code)] 
    [[CVPR 2022](https://github.com/extreme-assistant/CVPR2022-Paper-Code-Interpretation)] 
    [[CVPR 2022](https://github.com/amusi/CVPR2022-Papers-with-Code)] 
    [[CVPR 2021](https://github.com/52CV/CVPR-2021-Papers)] 
    [[CVPR 2020](https://github.com/extreme-assistant/CVPR2020-Paper-Code-Interpretation)]
    - [[ECCV 2022](https://github.com/extreme-assistant/ECCV2022-Paper-Code-Interpretation)]
    - [[ICCV 2021](https://github.com/extreme-assistant/ICCV2021-Paper-Code-Interpretation/blob/master/ICCV2021.md)] 

- Low level vision conference paper collection
    - [[CVPR 2023](https://github.com/DarrenPan/Awesome-CVPR2023-Low-Level-Vision)]  
    [[CVPR 2022](https://github.com/DarrenPan/CVPR2022-Low-Level-Vision)] 
    [[CVPR 2021/2020](https://github.com/Kobaayyy/Awesome-CVPR2021-CVPR2020-Low-Level-Vision/blob/master/CVPR2021.md)]
    - [[ECCV 2022](https://github.com/DarrenPan/Awesome-ECCV2022-Low-Level-Vision)] 
    [[ECCV 2020](https://zhuanlan.zhihu.com/p/180551773)]
    - [[ICCV 2023](https://github.com/DarrenPan/Awesome-ICCV2023-Low-Level-Vision)] 
    - [[ICCV 2021](https://github.com/Kobaayyy/Awesome-ICCV2021-Low-Level-Vision)] 

- Paper collection on low-level tasks
    - [[超分论文整理1](https://github.com/ChaofWang/Awesome-Super-Resolution)] [[图像/视频超分论文整理2](https://github.com/HymEric/latest-development-of-ISR-VSR)] [[图像/视频超分方法TF复现](https://github.com/LoSealL/VideoSuperResolution)]

    - [[VideoSuperResolution](https://github.com/LoSealL/VideoSuperResolution)] A collection of state-of-the-art video or single-image super-resolution architectures, reimplemented in TF

    - Low light enhancement [[Project 1](https://github.com/dawnlh/awesome-low-light-image-enhancement)] [[Project 2](https://github.com/cxtalk/You-Can-See-Clearly-Now)] [[Project 3](https://github.com/Elin24/Awesome-Low-Light-Enhancement)]
    - [[image-to-image translation](https://github.com/weihaox/awesome-image-translation)]

    - [[Deblurring](https://github.com/subeeshvasu/Awesome-Deblurring)]
    - [[SimDeblur](https://github.com/ljzycmd/SimDeblur)] 多个deep-learning based图像和视频去模糊Pytorch代码实现

    - [[Denoising with codes](https://github.com/wenbihan/reproducible-image-denoising-state-of-the-art)]

    - [[Awesome Face Restoratio](https://github.com/TaoWangzj/Awesome-Face-Restoration)]

## Codes
- [[各种对比度增强算法代码 Matlab](https://github.com/baidut/OpenCE)]
- [[一些基于C++的对比度增强算法实现](https://github.com/dengyueyun666/Image-Contrast-Enhancement)]

## 博客/专栏/资讯
- [[传统图像质量增强的系列blog-1](https://www.cnblogs.com/Imageshop/category/535367.html)]
- [[传统图像质量增强的系列blog-2](https://blog.csdn.net/maozefa/article/list/1)]
- [[图像处理相关](https://blog.csdn.net/aoman_hao/category_9353856.html?spm=1001.2014.3001.5482)]
- [无法抗拒的图像技术](https://www.zhihu.com/column/sining)
- [All in Camera](https://www.zhihu.com/column/allincamera)
- [Color Image Processing](https://www.zhihu.com/column/ColorImageProcessing)
- [计算摄影学](https://www.zhihu.com/column/hawkcp)

- [AIWalker](https://www.zhihu.com/column/c_1252624169897562112)
- [GiantPandaCV](https://www.zhihu.com/column/giantpandacv)
- [极市平台](https://www.zhihu.com/column/c_1027917842385129473)
- [CVer](https://www.zhihu.com/column/c_172507674)

## Misc
- [[Mobile AI benchmark](http://ai-benchmark.com/index.html#title)]

- [[Waifu2x-Extension-GUI](https://github.com/AaronFeng753/Waifu2x-Extension-GUI)] Image & GIF & Video Super-Resolution and Video Frame Interpolation using DNNs

- [[Photons to Photos](https://www.photonstophotos.net/index.htm)]

- [[Colour Science for Python]](https://github.com/colour-science/colour)

- [[数据增强albumentations]](https://github.com/albumentations-team/albumentations)

- [[RawTherapee]](https://github.com/Beep6581/RawTherapee)