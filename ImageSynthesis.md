# Table of Contents
- [Image Synthesis](#image-synthesis)
- [Image Translation](#image-translation)
- [Image Manipulation](#image-manipulation)
- [Style Transfer](#style-transfer)


# Image Synthesis
#### Anycost GAN
**[Paper]**  (CVPR 2021) Anycost GANs for Interactive Image Synthesis and Editing <Br>
**[Author]** [Ji Lin](http://linji.me/), [Richard Zhang](https://richzhang.github.io/), Frieder Ganz, [Song Han](https://songhan.mit.edu/), [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/)  <Br>
**[[Project](https://hanlab.mit.edu/projects/anycost-gan/)]**  **[[Pytorch-Code](https://github.com/mit-han-lab/anycost-gan)]**  <Br>
	
#### GH-Feat
**[Paper]**  (CVPR 2021 Oral) Generative Hierarchical Features from Synthesizing Images <Br>
**[Author]** [Yinghao Xu](https://justimyhxu.github.io/academic.html), [Yujun Shen](http://shenyujun.github.io/), [Jiapeng Zhu](https://zhujiapeng.github.io/), [Ceyuan Yang](http://ceyuan.me/), [Bolei Zhou](http://bzhou.ie.cuhk.edu.hk) <Br>
**[[Project](https://genforce.github.io/ghfeat/)]** **[[TF-Code](https://github.com/genforce/ghfeat)]**  <Br>

#### SEAN ★
**[Paper]** (CVPR 2020 Oral) SEAN: Image Synthesis with Semantic Region-Adaptive Normalization <Br>
**[Author]** Peihao Zhu, Rameen Abdal, [Yipeng Qin](https://www.cardiff.ac.uk/people/view/1508897-qin-yipeng), [Peter Wonka](http://peterwonka.net/)    <Br>
**[[Project](https://zpdesu.github.io/SEAN/)]** **[[PyTorch-Code](https://github.com/ZPdesu/SEAN)]**<Br>
与SPADE类似, 不过提取了每个语义类别的style信息, 并与语义mask一起, 通过AdaIN的形式控制生成器的activation

#### UNet GAN ★
**[Paper]** (CVPR 2020) A U-Net Based Discriminator for Generative Adversarial Networks <Br>
**[Author]** Edgar Sch ̈onfeld, [Bernt Schiele](https://www.mpi-inf.mpg.de/departments/computer-vision-and-machine-learning/people/bernt-schiele) <Br>
**[[PyTorch-Code](https://github.com/boschresearch/unetgan)]**<Br>
采用UNet形式的判别器, 可以用CutMix等数据增强策略

#### *Semantic Pyramid for Image Generation* ★☆
**[Paper]** (CVPR 2020 Oral)  Semantic Pyramid for Image Generation  <Br>
**[Author]** [Assaf Shocher](http://www.wisdom.weizmann.ac.il/~/assafsho/), Yossi Gandelsman, Inbar Mosseri, Michal Yarom, [Michal Irani](https://www.weizmann.ac.il/math/irani/), [William T. Freeman](https://billf.mit.edu/), [Tali Dekel](http://people.csail.mit.edu/talidekel/) <Br>
**[[Project](https://semantic-pyramid.github.io/)]**<Br>
提出一个通用的图像生成框架, 将预训练的多尺度特征融合进生成网络中, 实现对不同语义层次图像内容的生成控制, 融合时使用mask选择特定区域的生成. 论文思路简单清晰, 适用于多种任务
	
#### *Few-shot Image Generation with Elastic Weight Consolidation*
**[Paper]** (NeurIPS 2020)  Few-shot Image Generation with Elastic Weight Consolidation  <Br>
**[Author]** [Yijun Li](https://yijunmaverick.github.io/), [Richard Zhang](https://richzhang.github.io/), [Jingwan Lu](https://research.adobe.com/person/jingwan-lu/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/) <Br>
**[[Project](https://yijunmaverick.github.io/publications/ewc/)]**<Br>
	
#### StyleGAN2 ★☆
**[Paper]**  (CVPR 2020) Analyzing and Improving the Image Quality of StyleGAN <Br>
**[Author]** Tero Karras, [Samuli Laine](https://users.aalto.fi/~laines9/), Miika Aittala, Janne Hellsten, Jaakko Lehtinen, [Timo Aila](https://users.aalto.fi/~ailat1/) <Br>
**[[TF-Code](https://github.com/NVlabs/stylegan2)]**  <Br>
对StyleGAN做了一些改进, 如去掉减均值操作
	
#### StyleGAN2-ADA
**[Paper]**  (arXiv 2006) Training Generative Adversarial Networks with Limited Data <Br>
**[Author]** Tero Karras, Miika Aittala, Janne Hellsten, [Samuli Laine](https://users.aalto.fi/~laines9/), [Jaakko Lehtinen](https://users.aalto.fi/~lehtinj7/), [Timo Aila](https://users.aalto.fi/~ailat1/) <Br>
**[[TF-Code](https://github.com/NVlabs/stylegan2-ada)]** **[[Pytorch-Code](https://github.com/NVlabs/stylegan2-ada-pytorch)]**  <Br>


#### CC-FPSE ★
**[Paper]**  (NIPS 2019) Learning to Predict Layout-to-image Conditional Convolutions for Semantic Image Synthesis <Br>
**[Author]** [Xihui Liu](https://xh-liu.github.io), [Guojun Yin](https://gjyin91.github.io/), [Jing Shao](https://amandajshao.github.io/), [Xiaogang Wang](https://www.ee.cuhk.edu.hk/~xgwang/), [Hongsheng Li](https://www.ee.cuhk.edu.hk/~hsli/) <Br>
**[[Pytorch-Code](https://github.com/xh-liu/CC-FPSE)]**  <Br>
使用分割图通过一个网络预测每个pixel我的卷积参数, 虽然使用的depthwise卷积, 但参数量仍然非常庞大, 所以生成的图像较小.
	
#### BigGAN ★☆
**[Paper]**  (ICLR 2019) Large Scale GAN Training for High Fidelity Natural Image Synthesis <Br>
**[Author]** Andrew Brock, [Jeff Donahue](https://jeffdonahue.com/), Karen Simonyan <Br>
**[[Pytorch-Code](https://github.com/ajbrock/BigGAN-PyTorch)]**  <Br>
加大网络复杂度和训练batch size, 另外使用了截断等一些trick, 大幅提升了生成效果
	
#### SinGAN
**[Paper]**  (ICCV 2019 Best Paper Award) SinGAN: Learning a generative model from a single natural image <Br>
**[Author]** [Tamar Rott Shaham](https://tamarott.github.io/), [Tali Dekel](people.csail.mit.edu/talidekel/), [Tomer Michaeli](https://tomer.net.technion.ac.il/) <Br>
**[[Project](https://tamarott.github.io/SinGAN.htm)]** **[[Pytorch-Code](https://github.com/tamarott/SinGAN)]**  <Br>

#### Dynamic-Net ★☆
**[Paper]** (ICCV 2019) Dynamic-Net: Tuning the Objective Without Re-training for Synthesis Tasks <Br>
**[Author]** Alon Shoshan, [Roey Mechrez](https://roimehrez.github.io/), [Lihi Zelnik-Manor](https://webee.technion.ac.il/~lihi/)  <Br>
**[[Project](https://cgm.technion.ac.il/Computer-Graphics-Multimedia/Software/DynamicNet/)]** **[[PyTorch-Code](https://github.com/AlonShoshan10/dynamic_net)]**<Br>
先以Objective 0训练主干网络, 之后固定主干网络以Objective 1训练tuning block. 测试时手动指定插值系数, 达到在O0和O1之间的输出效果. 论文思路和实现都很简单, 分析论述方式值得学习
	
#### SPADE ★★
**[Paper]** (CVPR 2019 Oral) Semantic Image Synthesis with Spatially-Adaptive Normalization <Br>
**[Author]** [Taesung Park](https://taesung.me/), [Ming-Yu Liu](http://mingyuliu.net/), [Ting-Chun Wang](https://tcwang0509.github.io/), [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/)     <Br>
**[[Project](https://nvlabs.github.io/SPADE/)]** **[[PyTorch-Code](https://github.com/NVlabs/SPADE)]**<Br>
提出一个与AdaIN结构相似的SPADE模块, 用于将语义信息嵌入到生成模型中

#### StyleGAN ★★☆
**[Paper]**  (CVPR 2019) A Style-Based Generator Architecture for Generative Adversarial Networks <Br>
**[Author]** Tero Karras, [Samuli Laine](https://users.aalto.fi/~laines9/), [Timo Aila](https://users.aalto.fi/~ailat1/) <Br>
**[[TF-Code](https://github.com/NVlabs/stylegan)]**  <Br>
 通过若干FC层得到中间向量, 使用AdaIn的形式将中间向量作用在生成器上

#### layout2im
**[Paper]**  (CVPR 2019 Oral) Image Generation From Layout <Br>
**[Author]** [Bo Zhao](https://www.zhaobo.me/), [Lili Meng](https://lilimeng1103.wixsite.com/research-site), Weidong Yin, [Leonid Sigal](https://www.cs.ubc.ca/~lsigal/) <Br>
**[[Pytorch-Code](https://github.com/zhaobozb/layout2im)]**  <Br>

#### PhotographicImageSynthesis
**[Paper]** (CVPR 2018) Progressive Growing of GANs for Improved Quality, Stability, and Variation <Br>
**[Author]** [Qifeng Chen](https://cqf.io/), [Vladlen Koltun](http://vladlen.info/)   <Br>
**[[Project](https://cqf.io/ImageSynthesis/)]**  **[[TF-Code](https://github.com/CQFIO/PhotographicImageSynthesis)]** <Br>

#### pix2pixHD ★☆
**[Paper]** (CVPR 2018) High-Resolution Image Synthesis and Semantic Manipulation with Conditional GANs <Br>
**[Author]** [Ting-Chun Wang](https://tcwang0509.github.io/), [Ming-Yu Liu](http://mingyuliu.net/), [Jun-Yan Zhu](http://people.eecs.berkeley.edu/~junyanz/), Andrew Tao, [Jan Kautz](http://jankautz.com/), [Bryan Catanzaro](http://catanzaro.name/) <Br>
**[[Project](https://tcwang0509.github.io/pix2pixHD/)]**  **[[Pytorch-Code](https://github.com/NVIDIA/pix2pixHD)]** <Br>
生成2048 x 1024的高清图像, 提出了一个local到global的多尺度生成器结构, 使用多尺度的判别器, 提出使用判别器的中间层feature相似度作为一个loss
	
#### Progressive Growing of GANs ★★☆
**[Paper]** (ICLR 2018) Progressive Growing of GANs for Improved Quality, Stability, and Variation <Br>
**[Author]** [Tero Karras](https://research.nvidia.com/person/tero-karras), [Timo Aila](https://research.nvidia.com/person/timo-aila), [Samuli Laine](https://users.aalto.fi/~laines9/), [Jaakko Lehtinen](https://users.aalto.fi/~lehtinj7/)   <Br>
**[[Pytorch-Code](https://github.com/tkarras/progressive_growing_of_gans)]** <Br>

	


	
	
# Image Translation
#### LPTN
**[Paper]**  (CVPR 2021) High-Resolution Photorealistic Image Translation in Real-Time: A Laplacian Pyramid Translation Network <Br>
**[Author]** [Tamar Rott Shaham](https://tamarott.github.io/), [Michaël Gharbi](http://www.mgharbi.com/), [Richard Zhang](http://richzhang.github.io/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/), [Tomer Michaeli](https://tomer.net.technion.ac.il/)  <Br>
**[[Pytorch-Code](https://github.com/csjliang/LPTN)]**  <Br>

#### ASAPNet ★★
**[Paper]**  (CVPR 2021) Spatially-Adaptive Pixelwise Networks for Fast Image Translation <Br>
**[Author]** [Tamar Rott Shaham](https://tamarott.github.io/), [Michaël Gharbi](http://www.mgharbi.com/), [Richard Zhang](http://richzhang.github.io/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/), [Tomer Michaeli](https://tomer.net.technion.ac.il/)  <Br>
**[[Project](https://tamarott.github.io/ASAPNet_web/)]**  <Br>
(**快速图像生成**) 在小分辨率(降32倍)上预测每个pixel的MLP映射系数, 将位置信息编码为不同频率的sin, cosine信息, 提升了生成图像的细节. 论文很有实际意义, 值得学习. 

#### *Few-shot Image Generation*
**[Paper]**  (CVPR 2021) Spatially-Adaptive Pixelwise Networks for Fast Image Translation <Br>
**[Author]** [Utkarsh Ojha](https://utkarshojha.github.io/) , [Yijun Li](https://yijunmaverick.github.io/), [Jingwan Lu](https://research.adobe.com/person/jingwan-lu/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/), [Yong Jae Lee](https://web.cs.ucdavis.edu/~yjlee/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/), [Richard Zhang](https://richzhang.github.io/)  <Br>
**[[Project](https://utkarshojha.github.io/few-shot-gan-adaptation/)]**  **[[Pytorch-Code](https://github.com/utkarshojha/few-shot-gan-adaptation)]**  <Br>
	
#### TrGAN
**[Paper]**  (arXiv 2103) Unsupervised Image Transformation Learning via Generative Adversarial Networks <Br>
**[Author]** [Kaiwen Zha](http://kaiwenzha.github.io),  [Yujun Shen](http://shenyujun.github.io),  [Bolei Zhou](http://bzhou.ie.cuhk.edu.hk/)  <Br>
**[[Project](https://genforce.github.io/trgan/)]**  <Br>
	
#### COCO-FUNIT
**[Paper]**  (ECCV 2020) COCO-FUNIT: Few-Shot Unsupervised Image Translation with a Content Conditioned Style Encoder <Br>
**[Author]** [Kuniaki Saito](http://ai.bu.edu/ksaenko.html), [Kate Saenko](http://cs-people.bu.edu/keisaito/), [Ming-Yu Liu](http://mingyuliu.net/) <Br>
**[[Pytorch-Code](https://github.com/nvlabs/imaginaire)]**  <Br>

#### CUT
**[Paper]**  (ECCV 2020) Contrastive Learning for Unpaired Image-to-Image Translation <Br>
**[Author]** [Taesung Park](https://taesung.me/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/), [Richard Zhang](https://richzhang.github.io/),  [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/) <Br>
**[[Project](http://taesung.me/ContrastiveUnpairedTranslation/)]** **[[Pytorch-Code](https://github.com/taesungp/contrastive-unpaired-translation)]**  <Br>

#### DeepI2I
**[Paper]**  (NeurIPS 2020) DeepI2I: Enabling Deep Hierarchical Image-to-Image Translation by Transferring from GANs <Br>
**[Author]** [Yaxing Wang](https://yaxingwang.github.io//), [Lu Yu](https://yulu0724.github.io/), [Joost van de Weijer](http://www.cvc.uab.es/LAMP/joost/) <Br>
**[[Pytorch-Code](https://github.com/yaxingwang/DeepI2I)]**  <Br>
	
#### mbu-content-tansfer
**[Paper]**  (ICLR 2020) Mask Based Unsupervised Content Transfer <Br>
**[Author]** Ron Mokady, [Sagie Benaim](https://sagiebenaim.github.io/), [Lior Wolf](http://www.cs.tau.ac.il/~wolf/), [Amit Bermano](https://www.cs.tau.ac.il/~amberman/) <Br>
**[[Pytorch-Code](https://github.com/rmokady/mbu-content-tansfer)]**  <Br>

#### STGAN 
**[Paper]**  (CVPR 2019) STGAN: A Unified Selective Transfer Network for Arbitrary Image Attribute Editing  <Br>
**[Author]** Ming Liu, Yukang Ding, Min Xia, Xiao Liu, Errui Ding, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), Shilei Wen <Br>
**[[Pytorch-Code](https://github.com/csmliu/STGAN)]**   <Br>
	
#### RelGAN 
**[Paper]**  (ICLR 2019) RelGAN: Multi-Domain Image-to-Image Translation via Relative Attributes <Br>
**[Author]** Po-Wei Wu, Yu-Jing Lin, Che-Han Chang, Edward Y. Chang, Shih-Wei Liao <Br>
**[[Pytorch-Code](https://github.com/elvisyjlin/RelGAN-PyTorch)]**   <Br>
	
#### ContentDisentanglement 
**[Paper]**  (ICLR 2019) Emerging Disentanglement in Auto-Encoder Based Unsupervised Image Content Transfer <Br>
**[Author]** [Ori Press](https://oripress.com/), [Tomer Galanti](https://www.tau.ac.il/~tomerga2/), [Sagie Benaim](https://sagiebenaim.github.io/), [Lior Wolf](http://www.cs.tau.ac.il/~wolf/) <Br>
**[[Pytorch-Code](https://github.com/oripress/ContentDisentanglement)]**   <Br>

#### StarGAN v2
**[Paper]** (CVPR 2020) StarGAN v2: Diverse Image Synthesis for Multiple Domains <Br>
**[Author]** [Yunjey Choi](https://yunjey.github.io/), [Youngjung Uh](https://sites.google.com/site/youngjunguh), Jaejun Yoo, Jung-Woo Ha<Br>
**[[Pytorch-Code](https://github.com/clovaai/stargan-v2)]**<Br>

#### StarGAN 
**[Paper]**  (CVPR 2018 Oral) StarGAN: Unified Generative Adversarial Networks for Multi-Domain Image-to-Image Translation <Br>
**[Author]** [Yunjey Choi](https://yunjey.github.io/), [Minje Choi](http://www.minjechoi.com/), Munyoung Kim, Jung-Woo Ha, [Sunghun Kim](http://home.cse.ust.hk/~hunkim/), [Jaegul Choo](https://sites.google.com/site/jaegulchoo/) <Br>
**[[Pytorch-Code](https://github.com/yunjey/stargan)]**   <Br>

#### MUNIT
**[Paper]**  (ECCV 2018) Multimodal Unsupervised Image-to-image Translation <Br>
**[Author]** [Xun Huang](http://www.cs.cornell.edu/~xhuang/), [Ming-Yu Liu](http://mingyuliu.net/), [Serge Belongie](https://vision.cornell.edu/se3/), [Jan Kautz](https://jankautz.com/) <Br>
**[[Pytorch-Code](https://github.com/NVlabs/MUNIT)]**  <Br>

#### DRIT++
**[Paper]**  (IJCV 2020) DRIT++: Diverse Image-to-Image Translation via Disentangled Representations <Br>
**[Author]** [Hsin-Ying Lee](http://vllab.ucmerced.edu/hylee/), [Hung-Yu Tseng](https://sites.google.com/site/hytseng0509/), [Qi Mao](https://sites.google.com/view/qi-mao/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/), [Yu-Ding Lu](https://jonlu0602.github.io/), [Maneesh Kumar Singh](https://scholar.google.com/citations?user=hdQhiFgAAAAJ), [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/)  <Br>
**[[Pytorch-Code](https://github.com/HsinYingLee/DRIT)]**  <Br>

#### DRIT
**[Paper]**  (ECCV 2018 Oral) Diverse Image-to-Image Translation via Disentangled Representations <Br>
**[Author]** [Hsin-Ying Lee](http://vllab.ucmerced.edu/hylee/), [Hung-Yu Tseng](https://sites.google.com/site/hytseng0509/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/), [Maneesh Kumar Singh](https://scholar.google.com/citations?user=hdQhiFgAAAAJ), [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/) <Br>

#### pix2pix ★★☆
**[Paper]**  (CVPR 2017) Image-to-Image Translation with Conditional Adversarial Nets<Br>
**[Author]**  [Phillip Isola](http://web.mit.edu/phillipi/), [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/), [Tinghui Zhou](https://people.eecs.berkeley.edu/~tinghuiz/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/) <Br>
**[[Project](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)]**  <Br>
使用patchGAN的图像迁移的经典方法
	
#### CycleGAN ★★★
**[Paper]**  (ICCV 2017) Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks<Br>
**[Author]** [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/), [Taesung Park](https://taesung.me/), [Phillip Isola](http://web.mit.edu/phillipi/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/) <Br>
**[[Project](https://junyanz.github.io/CycleGAN/)]**  <Br>
无监督图像迁移

#### BicycleGAN
**[Paper]**  (NIPS 2017) Toward Multimodal Image-to-Image Translation <Br>
**[Author]** [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/), [Richard Zhang](http://richzhang.github.io/), [Deepak Pathak](https://www.cs.cmu.edu/~dpathak/), [Trevor Darrell](https://people.eecs.berkeley.edu/~trevor/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/), [Oliver Wang](http://www.oliverwang.info/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/) <Br>
**[[Pytorch-Code](https://github.com/junyanz/BicycleGAN)]**  <Br>
	
#### UNIT
**[Paper]**  (NIPS 2017) Unsupervised image-to-image translation networks <Br>
**[Author]** [Ming-Yu Liu](http://mingyuliu.net/), [Thomas Breuel](http://www.tmbdev.org/), [Jan Kautz](https://jankautz.com/) <Br>
**[[Pytorch-Code](https://github.com/nvlabs/imaginaire)]**  <Br>
	


	
	

# Image Manipulation
#### DeFLOCNet
**[Paper]**  (CVPR 2021) DeFLOCNet: Deep Image Editing via Flexible Low-level Controls <Br>
**[Author]** [Hongyu Liu](https://github.com/KumapowerLIU/DeFLOCNet#jump1), [Ziyu Wan](http://raywzy.com/), [Wei Huang](https://github.com/KumapowerLIU/DeFLOCNet#jump1), [Yibing Song](https://ybsong00.github.io/), [Xintong Han](http://users.umiacs.umd.edu/~xintong/) , [Jing Liao](https://liaojing.github.io/html/), [Bin Jiang](https://github.com/KumapowerLIU/DeFLOCNet#jump1), [Wei Liu](https://scholar.google.com/citations?user=AjxoEpIAAAAJ&hl=zh-CN)  <Br>
**[[Pytorch-Code](https://github.com/KumapowerLIU/DeFLOCNet)]**  <Br>
	
#### HiSD ★★
**[Paper]**  (CVPR 2021 Oral) HiSD: Image-to-image Translation via Hierarchical Style Disentanglement <Br>
**[Author]** Xinyang Li, Shengchuan Zhang, Jie Hu, Liujuan Cao, [Xiaopeng Hong](https://hongxiaopeng.com/), [Xudong Mao](https://xudongmao.github.io/), Feiyue Huang, Yongjian Wu, [Rongrong Ji](https://mac.xmu.edu.cn/rrji_en/)  <Br>
**[[Pytorch-Code](https://github.com/imlixinyang/HiSD)]**  <Br>
大致浏览, 可将人脸各属性解耦, 并实现准确控制. 将CelebA的属性信息进一步划分为相互独立的tags(如刘海, 眼镜)和互斥的attributes(如黑发和棕发),并为每个tag和attribute分别构造模块. 论文整体思路很清晰, 代码也很友好, 可以仔细研究一下.
	
#### SeFa
**[Paper]**  (CVPR 2021 Oral) Closed-Form Factorization of Latent Semantics in GANs <Br>
**[Author]** [Yujun Shen](https://shenyujun.github.io/), [Bolei Zhou](http://bzhou.ie.cuhk.edu.hk/) <Br>
**[[Project](https://genforce.github.io/sefa/)]** **[[Pytorch-Code](https://github.com/genforce/sefa)]**  <Br>

#### IDInvert
**[Paper]**  (ECCV 2020) IDInvert：In-Domain GAN Inversion for Real Image Editing <Br>
**[Author]** [Jiapeng Zhu](https://zhujiapeng.github.io/), [Yujun Shen](https://shenyujun.github.io/), [Deli Zhao](https://sites.google.com/site/zhaodeli/), [Bolei Zhou](http://bzhou.ie.cuhk.edu.hk/) <Br>
**[[Project](https://genforce.github.io/idinvert/)]** **[[TF-Code](https://github.com/genforce/idinvert)]**  <Br>
	
#### Faster StyleGAN Embedding ★
**[Paper]**  (arXiv 2007) Collaborative Learning for Faster StyleGAN Embedding <Br>
**[Author]** Shanyan Guan, [Ying Tai](https://tyshiwo.github.io/), Bingbing Ni, [Feida Zhu](https://zhufeida.github.io/), Feiyue Huang, Xiaokang Yang<Br>
(**latent code embedding**) 

#### Image2StyleGAN ★☆
**[Paper]**  (ICCV 2019) Image2StyleGAN: How to Embed Images Into the StyleGAN Latent Space? <Br>
**[Author]** Rameen Abdal, Yipeng Qin, Peter Wonka <Br>
**[[TF-Code](https://github.com/NVlabs/stylegan)]**  <Br>
(**latent code embedding**) 



# Style Transfer
#### SWAG
**[Paper]**  (CVPR 2021 Oral) Rethinking and Improving the Robustness of Image Style Transfer <Br>
**[Author]** [Pei Wang](http://www.svcl.ucsd.edu/~peiwang), [Yijun Li](https://yijunmaverick.github.io/), [Nuno Vasconcelos](http://www.svcl.ucsd.edu/~nuno) <Br>
**[[Pytorch-Code](https://github.com/peiwang062/swag)]**  <Br>

#### *Bilateral Style Transfer* ★★
**[Paper]**  (ECCV 2020) Joint Bilateral Learning for Real-time Universal Photorealistic Style Transfer  <Br>
**[Author]** [Xide Xia](https://xidexia.github.io/), Meng Zhang, [Tianfan Xue](http://people.csail.mit.edu/tfxue/), Zheng Sun, Hui Fang, [Brian Kulis](http://people.bu.edu/bkulis/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/) <Br>
基于HDRNet的实时风格迁移, 创新点尽管不是很多, 但是工作很有价值
