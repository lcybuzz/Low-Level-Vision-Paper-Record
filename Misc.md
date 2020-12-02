# Table of Contents
- [De-raining](#de-raining)
- [Image Demoireing](#image-demoireing)
- [Style-Transfer (Archived)](#style-transfer)
- [Image Synthesis (Archived)](#image-synthesis)


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
	
### *Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs*
**[Paper]** (NeurIPS 2020) Self-Adaptively Learning to Demoiré from Focused and Defocused Image Pairs  <Br>
**[Author]** [Lin Liu](http://home.ustc.edu.cn/~ll0825/#home), [Shanxin Yuan](https://shanxinyuan.github.io/), Jianzhuang Liu, Liping Bao, Gregory Slabaugh, Qi Tian <Br>
**[[Project](http://home.ustc.edu.cn/~ll0825/project_FDNet.html)]** <Br>



# Style-Transfer
### *Bilateral Style Transfer* ★★
**[Paper]**  (ECCV 2020) Joint Bilateral Learning for Real-time Universal Photorealistic Style Transfer  <Br>
**[Author]** [Xide Xia](https://xidexia.github.io/), Meng Zhang, [Tianfan Xue](http://people.csail.mit.edu/tfxue/), Zheng Sun, Hui Fang, [Brian Kulis](http://people.bu.edu/bkulis/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/) <Br>
基于HDRNet的实时风格迁移, 创新点尽管不是很多, 但是工作很有价值

  
  
# Image Synthesis
### Dynamic-Net ★☆
**[Paper]** (ICCV 2017) Dynamic-Net: Tuning the Objective Without Re-training for Synthesis Tasks <Br>
**[Author]** [Qifeng Chen](https://cqf.io/),	Jia Xu,	[Vladlen Koltun](http://vladlen.info/)  <Br>
**[[Project](https://cgm.technion.ac.il/Computer-Graphics-Multimedia/Software/DynamicNet/)]** **[[PyTorch-Code](https://github.com/AlonShoshan10/dynamic_net)]**<Br>
先以Objective 0训练主干网络, 之后固定主干网络以Objective 1训练tuning block. 测试时手动指定插值系数, 达到在O0和O1之间的输出效果. 论文思路和实现都很简单, 分析论述方式值得学习
	
