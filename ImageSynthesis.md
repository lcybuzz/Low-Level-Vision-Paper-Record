# Table of Contents
- [Image Synthesis](#image-synthesis)
- [Image Translation](#image-translation)


# Image Synthesis
### Progressive Growing of GANs ★★☆
**[Paper]** (ICLR 2018) Progressive Growing of GANs for Improved Quality, Stability, and Variation <Br>
**[Author]** [Tero Karras](https://research.nvidia.com/person/tero-karras), [Timo Aila](https://research.nvidia.com/person/timo-aila), [Samuli Laine](https://users.aalto.fi/~laines9/), [Jaakko Lehtinen](https://users.aalto.fi/~lehtinj7/)   <Br>
**[[Pytorch-Code](https://github.com/tkarras/progressive_growing_of_gans)]** <Br>
提出了一个渐进式训练GAN的方案, 可以实现大分辨率图像的生成(1024x1024人脸), 并提出了一些训练的技巧. 代码Star非常多, 可以学习一下 <Br>

### BigGAN 
**[Paper]**  (ICLR 2019) Large Scale GAN Training for High Fidelity Natural Image Synthesis <Br>
**[Author]** Andrew Brock, [Jeff Donahue](https://jeffdonahue.com/), Karen Simonyan <Br>
**[[Pytorch-Code](https://github.com/ajbrock/BigGAN-PyTorch)]**  <Br>
	
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

### StyleGAN ★★
**[Paper]**  (CVPR 2019) A Style-Based Generator Architecture for Generative Adversarial Networks <Br>
**[Author]** Tero Karras, [Samuli Laine](https://users.aalto.fi/~laines9/), [Timo Aila](https://users.aalto.fi/~ailat1/) <Br>
**[[TF-Code](https://github.com/NVlabs/stylegan)]**  <Br>
 通过若干FC层得到中间向量, 使用AdaIn的形式将中间向量作用在生成器上

### StyleGAN2 
**[Paper]**  (CVPR 2020) Analyzing and Improving the Image Quality of StyleGAN <Br>
**[Author]** Tero Karras,[Samuli Laine](https://users.aalto.fi/~laines9/), Miika Aittala, Janne Hellsten, Jaakko Lehtinen, [Timo Aila](https://users.aalto.fi/~ailat1/) <Br>
**[[TF-Code](https://github.com/NVlabs/stylegan2)]**  <Br>

  
### Image2StyleGAN 
**[Paper]**  (ICCV 2019) Image2StyleGAN: How to Embed Images Into the StyleGAN Latent Space? <Br>
**[Author]** Rameen Abdal, Yipeng Qin, Peter Wonka <Br>
**[[TF-Code](https://github.com/NVlabs/stylegan)]**  <Br>

### SEAN ★
**[Paper]** (CVPR 2020 Oral) SEAN: Image Synthesis with Semantic Region-Adaptive Normalization <Br>
**[Author]** Peihao Zhu, Rameen Abdal, [Yipeng Qin](https://www.cardiff.ac.uk/people/view/1508897-qin-yipeng), [Peter Wonka](http://peterwonka.net/)    <Br>
**[[Project](https://zpdesu.github.io/SEAN/)]** **[[PyTorch-Code](https://github.com/ZPdesu/SEAN)]**<Br>
与SPADE类似, 不过提取了每个语义类别的style信息, 并与语义mask一起, 通过AdaIN的形式控制生成器的activation


# Image Translation
### StarGAN 
**[Paper]**  (CVPR 2018 Oral) StarGAN: Unified Generative Adversarial Networks for Multi-Domain Image-to-Image Translation <Br>
**[Author]** [Yunjey Choi](https://yunjey.github.io/), [Minje Choi](http://www.minjechoi.com/), Munyoung Kim, Jung-Woo Ha, [Sunghun Kim](http://home.cse.ust.hk/~hunkim/), [Jaegul Choo](https://sites.google.com/site/jaegulchoo/) <Br>
**[[Pytorch-Code](https://github.com/yunjey/stargan)]**   <Br>

### StarGAN v2
**[Paper]** (CVPR 2020) StarGAN v2: Diverse Image Synthesis for Multiple Domains <Br>
**[Author]** [Yunjey Choi](https://yunjey.github.io/), [Youngjung Uh](https://sites.google.com/site/youngjunguh), Jaejun Yoo, Jung-Woo Ha<Br>
**[[Pytorch-Code](https://github.com/clovaai/stargan-v2)]**<Br>
