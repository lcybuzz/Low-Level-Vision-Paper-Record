# Table of Contents
- [Image Synthesis](#image-synthesis)


# Image Synthesis
### Progressive Growing of GANs ★★☆
**[Paper]** (ICLR 2018) Progressive Growing of GANs for Improved Quality, Stability, and Variation <Br>
**[Author]** [Tero Karras](https://research.nvidia.com/person/tero-karras), [Timo Aila](https://research.nvidia.com/person/timo-aila), [Samuli Laine](https://users.aalto.fi/~laines9/), [Jaakko Lehtinen](https://users.aalto.fi/~lehtinj7/)   <Br>
**[[Pytorch-Code](https://github.com/tkarras/progressive_growing_of_gans)]** <Br>
提出了一个渐进式训练GAN的方案, 可以实现大分辨率图像的生成(1024x1024人脸), 并提出了一些训练的技巧. 代码Star非常多, 可以学习一下 <Br>

### Dynamic-Net ★☆
**[Paper]** (ICCV 2019) Dynamic-Net: Tuning the Objective Without Re-training for Synthesis Tasks <Br>
**[Author]** Alon Shoshan, [Roey Mechrez](https://roimehrez.github.io/), [Lihi Zelnik-Manor](https://webee.technion.ac.il/~lihi/)  <Br>
**[[Project](https://cgm.technion.ac.il/Computer-Graphics-Multimedia/Software/DynamicNet/)]** **[[PyTorch-Code](https://github.com/AlonShoshan10/dynamic_net)]**<Br>
先以Objective 0训练主干网络, 之后固定主干网络以Objective 1训练tuning block. 测试时手动指定插值系数, 达到在O0和O1之间的输出效果. 论文思路和实现都很简单, 分析论述方式值得学习
	
### SPADE ★★
**[Paper]** (CVPR 2019 Oral) Semantic Image Synthesis with Spatially-Adaptive Normalization <Br>
**[Author]** [Taesung Park](https://taesung.me/), [Ming-Yu Liu](http://mingyuliu.net/), [Ting-Chun Wang](https://tcwang0509.github.io/), [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/)     <Br>
**[[Project](https://nvlabs.github.io/SPADE/)]** **[[PyTorch-Code](https://github.com/NVlabs/SPADE)]**<Br>
提出一个与AdaIN结构相似的SPADE模块, 用于将语义信息嵌入到生成模型中
	
### SEAN ★
**[Paper]** (CVPR 2020 Oral) SEAN: Image Synthesis with Semantic Region-Adaptive Normalization <Br>
**[Author]** Peihao Zhu, Rameen Abdal, [Yipeng Qin](https://www.cardiff.ac.uk/people/view/1508897-qin-yipeng), [Peter Wonka](http://peterwonka.net/)    <Br>
**[[Project](https://zpdesu.github.io/SEAN/)]** **[[PyTorch-Code](https://github.com/ZPdesu/SEAN)]**<Br>
与SPADE类似, 不过提取了每个语义类别的style信息, 并与语义mask一起, 通过AdaIN的形式控制生成器的activation
