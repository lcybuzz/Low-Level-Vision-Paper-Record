# Table of Contents
- [Reflection Removal](#reflection-removal)
- [De-raining](#de-raining)
- [Image Demoireing](#image-demoireing)
- [Style-Transfer (Archived)](#style-transfer)

# Reflection Removal
### perceptual-reflection-removal ★☆
**[Paper]** (CVPR 2018) Single Image Reflection Removal with Perceptual Losses <Br>
**[Author]** [Xuaner Zhang](https://people.eecs.berkeley.edu/~cecilia77/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html), [Qifeng Chen](https://cqf.io/) <Br>
**[[Project](https://people.eecs.berkeley.edu/~cecilia77/project-pages/reflection.html)]** **[[TF-Code](https://github.com/ceciliavision/perceptual-reflection-removal)]**<Br>
VGG19的多层特征作为hypercolumn与图像串联作为输入, 一个网络同时预测transmission和reflection, 使用pixel, VGG和GAN loss, 另外提出了一个gradient exclusion loss. 

### ERRNet ★
**[Paper]** (CVPR 2019) Single Image Reflection Removal Exploiting Misaligned Training Data and Network Enhancements <Br>
**[Author]** [Kaixuan Wei](https://kxwei.net/), [Jiaolong Yang](http://jlyang.org/), [Ying Fu](https://ying-fu.github.io/), [David Wipf](http://www.davidwipf.com/), Hua Huang <Br>
**[[Pytorch-Code](https://github.com/Vandermode/ERRNet)]** **[[Pytorch-Code](https://github.com/Vandermode/ERRNet)]**<Br>
也用了VGG19的特征串联作为输入, 采用了PSP模块和channel-wise attention模块. 使用pixel loss, VGG loss, GAN loss, 另外提出了一个利用非对齐数据训练的方法, 貌似就是用VGG的高层特征计算距离, 效果上看不如contextual loss.  



# De-raining
### DID-MDN ★☆
**[Paper]**  (CVPR 2018) Density-aware Single Image De-raining using a Multi-stream Dense Network<Br>
**[Author]** [He Zhang](https://sites.google.com/site/hezhangsprinter), [Vishal M. Patel](https://engineering.jhu.edu/vpatel36/sciencex_teams/vishalpatel/) <Br>
**[[Pytorch-Code](https://github.com/hezhangsprinter/DID-MDN)]**<Br>
基于dense connection的双分支去雨网络, 一个分支预测一个雨稠密程度的类别标签(大中小), 一个采用残差预测结构, 并结合稠密程度label, 预测去雨图像, 经过一个refinement网络输出. 加入一个预测程度的分支的策略, 在图像增强恢复任务中还是比较值得尝试的.

### Syn2Real ★★
**[Paper]**  (CVPR 2020) Syn2Real Transfer Learning for Image Deraining using Gaussian Processes<Br>
**[Author]** [Rajeev Yasarla](https://sites.google.com/view/rajeevyasarla/home), [Vishwanath A. Sindagi](https://www.vishwanathsindagi.com/), [Vishal M. Patel](https://engineering.jhu.edu/ece/faculty/vishal-m-patel/) <Br>
**[[Pytorch-Code](https://github.com/rajeevyasarla/Syn2Real)]**<Br>
使用高斯过程计算无标签真实数据的unsupervised loss. 从paper的实验效果来看有不错的效果, 值得一试

### MSPFN
**[Paper]**  (CVPR 2020) Multi-Scale Progressive Fusion Network for Single Image Deraining <Br>
**[Author]** [Kui Jiang](https://github.com/kuihua/kuijiang.github.io/blob/master/home.md), Zhongyuan Wang, Peng Yi, [Chen Chen](https://webpages.uncc.edu/cchen62/), Baojin Huang, Yimin Luo, [Jiayi Ma](https://sites.google.com/site/jiayima2013/), [Junjun Jiang](https://jiangjunjun.wordpress.com/) <Br>
**[[TF-Code](https://github.com/kuihua/MSPFN)]**<Br>
	
### DRD-Net
**[Paper]**  (CVPR 2020) Detail-recovery Image Deraining via Context Aggregation Networks <Br>
**[Author]** Sen Deng, Mingqiang Wei, Jun Wang, Yidan Feng, Luming Liang, Haoran Xie, Fu Lee Wang, Meng Wang <Br>
**[[TF-Code](hhttps://github.com/Dengsgithub/DRD-Net)]**<Br>
	
  

# Image Demoireing
### Learnbale_Bandpass_Filter ★
**[Paper]**  (CVPR 2020) Image Demoireing with Learnable Bandpass Filters  <Br>
**[Author]** Bolun Zheng, [Shanxin Yuan](https://sites.google.com/site/shanxinyuan/), [Gregory Slabaugh](http://www.gregslabaugh.net/), [Ales Leonardis](https://www.cs.bham.ac.uk/~leonarda/) <Br>
**[[TF-Code](https://github.com/zhenngbolun/Learnbale_Bandpass_Filter)]** <Br>
在DCT变换后的频谱域做摩尔纹提取, 分为3个scale提取不同尺度的摩尔纹. 对带通去取摩尔纹的推导部分没看懂. <Br>

### JDD
**[Paper]**  (CVPR 2020) Joint Demosaicing and Denoising With Self Guidance  <Br>
**[Author]** [Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), [Xu Jia](https://stephenjia.github.io/), Jianzhuang Liu, Qi Tian <Br>

### *Wavelet-Based Dual-Branch Networkfor Image Demoireing*
**[Paper]** (ECCV 2020) Wavelet-Based Dual-Branch Networkfor Image Demoireing  <Br>
**[Author]**[Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), Jianzhuang Liu, [Shanxin Yuan](https://shanxinyuan.github.io/), [Gregory Slabaugh](http://www.gregslabaugh.net/), [Ales Leonardis](https://www.cs.bham.ac.uk/~leonarda/), Wengang Zhou, Qi Tian <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>
	
### FHDe²Net
**[Paper]** (ECCV 2020) FHDe²Net: Full High Definition Demoireing Network <Br>
**[Author]** Bin He, Ce Wang, [Boxin Shi](http://ci.idm.pku.edu.cn/), Ling-Yu Duan <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>
	
### *Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs*
**[Paper]** (NeurIPS 2020) Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs  <Br>
**[Author]** [Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), [Shanxin Yuan](https://shanxinyuan.github.io/), Jianzhuang Liu, Liping Bao, Gregory Slabaugh, Qi Tian <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>



# Style-Transfer
### *Bilateral Style Transfer* ★★
**[Paper]**  (ECCV 2020) Joint Bilateral Learning for Real-time Universal Photorealistic Style Transfer  <Br>
**[Author]** [Xide Xia](https://xidexia.github.io/), Meng Zhang, [Tianfan Xue](http://people.csail.mit.edu/tfxue/), Zheng Sun, Hui Fang, [Brian Kulis](http://people.bu.edu/bkulis/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/) <Br>
基于HDRNet的实时风格迁移, 创新点尽管不是很多, 但是工作很有价值

  
  
