#  Dehazing

### DehazeNet ☆
**[Paper]**  (TIP 2016) DehazeNet: An End-to-End System for Single Image Haze Removal <Br>
**[Author]** [Bolun Cai](https://caibolun.github.io/), Xiangmin Xu, Kui Jia, Chunmei Qing, Dacheng Tao, Lingke Zeng <Br>
**[[Project](http://caibolun.github.io/DehazeNet/)]** **[[Matlab-Code](https://github.com/caibolun/DehazeNet)]**<Br>
端到端预测透射率map

### AOD-NET ★
**[Paper]**  (ICCV 2017) AOD-NET：An All-in-One Network for Dehazing and Beyond<Br>
**[Author]** [Boyi Li](https://sites.google.com/site/boyilics/home), Xiulian Peng, [Zhangyang Wang](https://www.atlaswang.com/), Jizheng Xu, Dan Feng <Br>
**[[Project](https://sites.google.com/site/boyilics/website-builder/project-page)]**  **[[Pytorch&Caffe-Code](https://github.com/Boyiliee/AOD-Net)]** <Br>
轻量级去雾网络, 通过预测一个变量, 直接输出清晰的RGB图像

### DCPDN ★
**[Paper]**  (CVPR 2018) Densely Connected Pyramid Dehazing Network<Br>
**[Author]** [He Zhang](https://sites.google.com/site/hezhangsprinter), [Vishal M. Patel](https://engineering.jhu.edu/vpatel36/sciencex_teams/vishalpatel/) <Br>
**[[Pytorch-Code](https://github.com/hezhangsprinter/DCPDN)]**<Br>
两分支网络, transmission map通过类似dense-net的网络预测, 大气光照假设是一全局常量并通过一UNet预测, 两分支结果经大气散射模型公式的计算, 恢复清晰RGB. 使用了L2, VGG loss, gradient loss和GAN loss.
	
### Multi-scale-CNN-Dehazing ☆
**[Paper]**  (CVPR 2018) Single Image Dehazing via Multi-Scale Convolutional Neural Networks <Br>
**[Author]** [Wenqi Ren](https://sites.google.com/site/renwenqi888/), [Si Liu](http://www.colalab.org/people), Hua Zhang, [Jinshan Pan](https://sites.google.com/site/jspanhomepage/), [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en), [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Project](https://sites.google.com/site/renwenqi888/research/dehazing/mscnndehazing)]** **[[Matlab-Code](https://github.com/rwenqi/Multi-scale-CNN-Dehazing)]**  **[[Unofficial-TF-Code](https://github.com/dishank-b/MSCNN-Dehazing-Tensorflow)]**<Br>
大致浏览, 一个多尺度去雾网络, coarse尺度预测transmission map, fine尺度预测去雾图像, 用深度图生成transmmision map训练 <Br>

### GFN
**[Paper]**  (CVPR 2018) Gated Fusion Network for Single Image Dehazing <Br>
**[Author]** [Wenqi Ren](https://sites.google.com/site/renwenqi888/), [Lin Ma](http://forestlinma.com/), [Jiawei Zhang](https://sites.google.com/site/zhjw1988), [Jinshan Pan](https://sites.google.com/site/jspanhomepage/), [Xiaochun Cao](http://people.ucas.ac.cn/~0022382?language=en),  Wei Liu, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Project](https://sites.google.com/site/renwenqi888/research/dehazing/gfn)]** **[[MatCaffe-Code](https://github.com/rwenqi/GFN-dehazing)]**  <Br>

### MSBDN-DFF ★☆
**[Paper]**  (CVPR 2020) Multi-Scale Boosted Dehazing Network with Dense Feature Fusion <Br>
**[Author]**  [Hang Dong](https://sites.google.com/view/hdong/%E9%A6%96%E9%A1%B5), [Jinshan Pan](https://jspan.github.io/), [Zhe Hu](https://zjuela.github.io/), Xiang Lei, [Xinyi Zhang](http://xinyizhang.tech/), Fei Wang, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/) <Br>
**[[Pytorch-Code](https://github.com/BookerDeWitt/MSBDN-DFF)]**  <Br>
粗读, Unet结合超分中的Deep Back-Projection, 有时间可以研究一下反投影的原理和代码


### DA_dahazing ★☆
**[Paper]**  (CVPR 2020) Domain Adaptation for Image Dehazing <Br>
**[Author]**  Yuanjie Shao, [Lerenhan Li](https://sites.google.com/view/lerenhanli/homepage), [Wenqi Ren](https://sites.google.com/site/renwenqi888/), [Changxin Gao](https://sites.google.com/site/changxingao), Nong Sang<Br>
**[[Pytorch-Code](https://github.com/HUSTSYJ/DA_dahazing)]**  <Br>
粗读, 提出了一个生成数据集训练的网络迁移到真实图像去雾中的框架, 使用两个变换网络和GAN完成Syn和Real数据间的相互迁移.
								     
