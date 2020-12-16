# Table of Contents
- [Face Restoration](#face-restoration)
- [Face SuperResolution](#face-superresolution)

# Face Restoration
### ASFFNet
**[Paper]** (CVPR 2020 Oral) Enhanced Blind Face Restoration With Multi-Exemplar Images and Adaptive Spatial Feature Fusion  <Br>
**[Author]** [Xiaoming Li](https://csxmli2016.github.io/), Wenyu Li, [Dongwei Ren](https://csdwren.github.io/), Hongzhi Zhang, Meng Wang, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo) <Br>
**[[Code](https://github.com/csxmli2016/ASFFNet)]** <Br>
	

# Face SuperResolution
### *Face Super-resolution Guided by Facial Component Heatmaps* ★
**[Paper]** (ECCV 2018) Face Super-resolution Guided by Facial Component Heatmaps <Br>
**[Author]** [Xin Yu](https://sites.google.com/view/xinyus-homepage/Home), [Basura Fernando](https://basurafernando.github.io/), [Bernard Ghanem](http://www.bernardghanem.com/), [Fatih Porikli](http://www.porikli.com/), [Richard Hartley](http://users.cecs.anu.edu.au/~hartley/) <Br>
结合人脸关键点的heapmap信息做人脸超分
	
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

### *Face Super-Resolution Guided by 3D Facial Priors*
**[Paper]**  (ECCV 2020) Face Super-Resolution Guided by 3D Facial Priors <Br>
**[Author]** Xiaobin Hu, [Wenqi Ren](https://sites.google.com/site/renwenqi888/home), John LaMaster, [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en), [Xiaoming Li](https://csxmli2016.github.io/), Zechao Li, Bjoern Menze, Wei Liu <Br>

### DFDNet ★★
**[Paper]** (ECCV 2020) Blind Face Restoration via Deep Multi-scale Component Dictionaries <Br>
**[Author]** [Xiaoming Li](https://csxmli2016.github.io/), [Chaofeng Chen](https://chaofengc.github.io/), [Shangchen Zhou](https://shangchenzhou.com/), Xianhui Lin, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), [Lei Zhang](https://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
**[[Pytorch-Code](https://github.com/csxmli2016/DFDNet)]** <Br>
