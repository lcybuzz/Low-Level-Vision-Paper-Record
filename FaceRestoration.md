# Table of Contents
- [Face Restoration](#face-restoration)
- [Face SuperResolution](#face-superresolution)

# Face Restoration
### *Deep semantic face deblurring*
**[Paper]** (CVPR 2018) Deep semantic face deblurring <Br>
**[Author]** [Ziyi Shen](https://sites.google.com/site/ziyishenmi/), [Wei-Sheng Lai](https://www.wslai.net/) , Tingfa Xu, [Jan Kautz](https://jankautz.com/), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/)  <Br>
**[[Project](https://sites.google.com/site/ziyishenmi/cvpr18_face_deblur)]** **[[Matlab-Code](https://github.com/joanshen0508/Deep-Semantic-Face-Deblurring)]** <Br>

### GFRNet
**[Paper]** (CVPR 2018) Learning Warped Guidance for Blind Face Restoration <Br>
**[Author]** [Xiaoming Li](https://csxmli2016.github.io/), Ming Liu, Yuting Ye, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), [Liang Lin](http://www.linliang.net/), Ruigang Yang <Br>
**[[Torch-Code](https://github.com/csxmli2016/GFRNet)]** <Br>
	
### ASFFNet ★
**[Paper]** (CVPR 2020 Oral) Enhanced Blind Face Restoration With Multi-Exemplar Images and Adaptive Spatial Feature Fusion  <Br>
**[Author]** [Xiaoming Li](https://csxmli2016.github.io/), Wenyu Li, [Dongwei Ren](https://csdwren.github.io/), Hongzhi Zhang, Meng Wang, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo) <Br>
**[[Code](https://github.com/csxmli2016/ASFFNet)]** <Br>
**(基于同一张脸的exemplar做恢复)** 通过关键点从数张同一人的examplar图像中选出最相思的图像, 使用moving least-square和AdaIn进行空间和亮度的对齐, 提出了ASFF模块通过预测attention map将引导图和LR图的特征融合

### HiFaceGAN ★☆
**[Paper]** (MM 2020) HiFaceGAN: Face Renovation via Collaborative Suppression and Replenishment <Br>
**[Author]** [Lingbo Yang](https://lotayou.github.io/), Chang Liu, Pan Wang, Shanshe Wang, Peiran Ren, Siwei Ma, Wen Gao <Br>
**[[Project](https://lotayou.github.io/projects/face_renov.html)]** **[[Pytorch-Code](https://github.com/Lotayou/Face-Renovation)]**  <Br>
通过不同提取不同尺度的语义信息作为指导, 实现人脸修复, 对真实照片效果良好.

# Face SuperResolution
### Attention-FH
**[Paper]** (CVPR 2017) Attention-Aware Face Hallucination via Deep Reinforcement Learning <Br>
**[Author]** Qingxing Cao, [Liang Lin](http://www.linliang.net/), [Yukai Shi](https://ykshi.github.io/), [Xiaodan Liang](https://lemondan.github.io/), [Guanbin Li](http://guanbinli.com/) <Br>
**[[Torch-Code](https://github.com/ykshi/facehallucination)]** <Br>

### *Learning to Super-resolve Blurry Face and Text Images*
**[Paper]** (ICCV 2017) Learning to Super-resolve Blurry Face and Text Images <Br>
**[Author]** [Xiangyu Xu](https://sites.google.com/view/xiangyuxu), [Deqing Sun](https://deqings.github.io/), [Jinshan Pan](https://jspan.github.io/), Yujin Zhang, [Hanspeter Pfister](https://vcg.seas.harvard.edu/), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Project](https://sites.google.com/view/xiangyuxu/deblursr_iccv17)]** <Br>
	
### FSRNet ★
**[Paper]** (CVPR 2018) FSRNet: End-to-End Learning Face Super-Resolution with Facial Priors <Br>
**[Author]** Yu Chen, [Ying Tai](https://tyshiwo.github.io/), [Xiaoming Liu](http://cvlab.cse.msu.edu/), [Chunhua Shen](https://cshen.github.io/index.html), Jian Yang <Br>
**[[Torch-Code](https://github.com/tyshiwo/FSRNet)]** <Br>
一个分支预测lanmark和分割结果, 辅助人脸超分
	
### *Face Super-resolution Guided by Facial Component Heatmaps* ★
**[Paper]** (ECCV 2018) Face Super-resolution Guided by Facial Component Heatmaps <Br>
**[Author]** [Xin Yu](https://sites.google.com/view/xinyus-homepage/Home), [Basura Fernando](https://basurafernando.github.io/), [Bernard Ghanem](http://www.bernardghanem.com/), [Fatih Porikli](http://www.porikli.com/), [Richard Hartley](http://users.cecs.anu.edu.au/~hartley/) <Br>
结合人脸关键点的heapmap信息做人脸超分

### Progressive Face Super-Resolution ★☆
**[Paper]** (BMVC 2019) Progressive Face Super-Resolution via Attention to Facial Landmark <Br>
**[Author]** Deokyun Kim, Minseon Kim, Gihyun Kwon, Dae-Shik Kim <Br>
**[[Pytorch-Code](https://github.com/DeokyunKim/Progressive-Face-Super-Resolution)]** <Br>
一个结构简洁的渐进式人脸超分网络, 使用了额外的关键点检测网络作为计算loss的attention.
	
### GWAInet ★
**[Paper]** (CVPRW 2019) Exemplar Guided Face Image Super-Resolution without Facial Landmarks <Br>
**[Author]** Berk Dogan, [Shuhang Gu](https://shuhanggu.github.io/), [Radu Timofte](https://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/Maclory/Deep-Iterative-Collaboration)]** <Br>
用一张相同人的照片作为引导图, 将引导图通过一个可学习的warp net与输入图像对齐, 之后将原图和warped guidance经过一个网络生成超分结果. 使用了GAN loss, VGG loss以及identity loss等.
	
### Deep-Iterative-Collaboration ★
**[Paper]** (CVPR 2020) Deep Face Super-Resolution with Iterative Collaboration between Attentive Recovery and Landmark Estimation  <Br>
**[Author]** Cheng Ma, Zhenyu Jiang, [Yongming Rao](https://raoyongming.github.io/), Jiwen Lu, Jie Zhou <Br>
**[[Pytorch-Code](https://github.com/Maclory/Deep-Iterative-Collaboration)]** <Br>
迭代训练人脸超分和关键点网络, 并利用两个任务的信息, 相互优化

### Ear for Face Super-Resolution
**[Paper]**  (CVPR 2020) Learning to Have an Ear for Face Super-Resolution <Br>
**[Author]** [Givi Meishvili](https://gmeishvili.github.io/), [Simon Jenni](https://sjenni.github.io/), [Paolo Favaro](https://www.cvg.unibe.ch/people/favaro)  <Br>
**[[Project](https://gmeishvili.github.io/ear_for_face_super_resolution/index.html)]**

### *Face Super-Resolution Guided by 3D Facial Priors*
**[Paper]**  (ECCV 2020) Face Super-Resolution Guided by 3D Facial Priors <Br>
**[Author]** Xiaobin Hu, [Wenqi Ren](https://sites.google.com/site/renwenqi888/home), John LaMaster, [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en), [Xiaoming Li](https://csxmli2016.github.io/), Zechao Li, Bjoern Menze, Wei Liu <Br>

### DFDNet ★★
**[Paper]** (ECCV 2020) Blind Face Restoration via Deep Multi-scale Component Dictionaries <Br>
**[Author]** [Xiaoming Li](https://csxmli2016.github.io/), [Chaofeng Chen](https://chaofengc.github.io/), [Shangchen Zhou](https://shangchenzhou.com/), Xianhui Lin, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), [Lei Zhang](https://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
**[[Pytorch-Code](https://github.com/csxmli2016/DFDNet)]** <Br>
**(构建字典, 匹配最近邻特征)** 对眼睛鼻子嘴建立字典, inference时通过匹配最相似的feature找到相似的高清特征并做替换. 字典通过VGG网络提特征和聚类实现. 实测对五官的增强效果不错, 不过对于头发皮肤等部分效果不明显.
