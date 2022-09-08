# Table of Contents
- [Image Synthesis](#image-synthesis)
- [Image Translation](#image-translation)
- [Image Manipulation](#image-manipulation)
- [Style Transfer](#style-transfer)


# Image Synthesis
- **Multimodal Image Synthesis and Editing: A Survey** <Br>
[Fangneng Zhan](https://fnzhan.com/), [Yingchen Yu](https://yingchen001.github.io/), [Rongliang Wu](https://scholar.google.com.sg/citations?user=SZkh3iAAAAAJ&hl=en), [Jiahui Zhang](https://scholar.google.com/citations?user=DXpYbWkAAAAJ&hl=zh-CN), [Shijian Lu](https://scholar.google.com.sg/citations?user=uYmK-A0AAAAJ&hl=en), [Lingjie Liu](https://lingjie0206.github.io/), [Adam Kortylewsk](https://generativevision.mpi-inf.mpg.de/), [Christian Theobalt](https://people.mpi-inf.mpg.de/~theobalt/), [Eric Xing](http://www.cs.cmu.edu/~epxing/) <Br>
[arXiv 2112] [[Project](https://github.com/fnzhan/MISE)] 

- **NeRF in the Dark: High Dynamic Range View Synthesis from Noisy Raw Images** <Br>
[Ben Mildenhall](https://bmild.github.io/), [Peter Hedman](https://www.phogzone.com/), [Ricardo Martin-Brualla](http://ricardomartinbrualla.com/), [Pratul Srinivasan](https://pratulsrinivasan.github.io/), [Jonathan Barron](https://jonbarron.info/) <Br>
[CVPR 2022 Oral] [[Project](https://bmild.github.io/rawnerf/)] [[TF-Code](https://github.com/google-research/multinerf)]  

- **Im2Vec Synthesizing Vector Graphics without Vector Supervision** <Br>
[Sheng-Yu Wang](https://peterwang512.github.io/), [David Bau](https://people.csail.mit.edu/davidbau/home/), [Jun-Yan Zhu](https://cs.cmu.edu/~junyanz)  <Br>
[ICCV 2021] [[Project](https://peterwang512.github.io/GANSketching/)] [[Pytorch-Code](https://github.com/PeterWang512/GANSketching)]  <Br>
	
- **Im2Vec Synthesizing Vector Graphics without Vector Supervision** <Br>
[Pradyumna Reddy](https://preddy5.github.io/), [Michael Gharbi](http://www.mgharbi.com/), [Michal Lukac](https://research.adobe.com/person/michal-lukac/), [Niloy J. Mitra](http://www0.cs.ucl.ac.uk/staff/n.mitra/)  <Br>
[CVPR 2021 Oral] [[Project](http://geometry.cs.ucl.ac.uk/projects/2021/im2vec/)] [[Pytorch-Code](https://github.com/preddy5/Im2Vec)]  <Br>
	
- **Image Generators with Conditionally-Independent Pixel Synthesis** <Br>
Ivan Anokhin, Kirill Demochkin, Taras Khakhulin, Gleb Sterkin, [Victor Lempitsky](http://sites.skoltech.ru/compvision/members/vilem/), Denis Korzhenkov  <Br>
[CVPR 2021 Oral] [[Pytorch-Code](https://github.com/saic-mdal/CIPS)]  <Br>
[**CIPS**]

- **Anycost GANs for Interactive Image Synthesis and Editing** <Br>
[Ji Lin](http://linji.me/), [Richard Zhang](https://richzhang.github.io/), Frieder Ganz, [Song Han](https://songhan.mit.edu/), [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/)  <Br>
[CVPR 2021] [[Project](https://hanlab.mit.edu/projects/anycost-gan/)] [[Pytorch-Code](https://github.com/mit-han-lab/anycost-gan)]  <Br>
	
- **Generative Hierarchical Features from Synthesizing Images** <Br>
[Yinghao Xu](https://justimyhxu.github.io/academic.html), [Yujun Shen](http://shenyujun.github.io/), [Jiapeng Zhu](https://zhujiapeng.github.io/), [Ceyuan Yang](http://ceyuan.me/), [Bolei Zhou](http://bzhou.ie.cuhk.edu.hk) <Br>
[CVPR 2021 Oral] [[Project](https://genforce.github.io/ghfeat/)] [[TF-Code](https://github.com/genforce/ghfeat)]  <Br>
[**GH-Feat**]

- **SEAN: Image Synthesis with Semantic Region-Adaptive Normalization** <Br>
Peihao Zhu, Rameen Abdal, [Yipeng Qin](https://www.cardiff.ac.uk/people/view/1508897-qin-yipeng), [Peter Wonka](http://peterwonka.net/)    <Br>
[CVPR 2020 Oral] [[Project](https://zpdesu.github.io/SEAN/)] [[PyTorch-Code](https://github.com/ZPdesu/SEAN)]<Br>
[★] 与SPADE类似, 不过提取了每个语义类别的style信息, 并与语义mask一起, 通过AdaIN的形式控制生成器的activation

- **A U-Net Based Discriminator for Generative Adversarial Networks** <Br>
Edgar Sch ̈onfeld, [Bernt Schiele](https://www.mpi-inf.mpg.de/departments/computer-vision-and-machine-learning/people/bernt-schiele) <Br>
[CVPR 2020] [[PyTorch-Code](https://github.com/boschresearch/unetgan)] <Br>
[★] 采用UNet形式的判别器, 可以用CutMix等数据增强策略

- **Semantic Pyramid for Image Generation**  <Br>
[Assaf Shocher](http://www.wisdom.weizmann.ac.il/~/assafsho/), Yossi Gandelsman, Inbar Mosseri, Michal Yarom, [Michal Irani](https://www.weizmann.ac.il/math/irani/), [William T. Freeman](https://billf.mit.edu/), [Tali Dekel](http://people.csail.mit.edu/talidekel/) <Br>
[CVPR 2020 Oral] [[Project](https://semantic-pyramid.github.io/)] <Br>
[★☆] 提出一个通用的图像生成框架, 将预训练的多尺度特征融合进生成网络中, 实现对不同语义层次图像内容的生成控制, 融合时使用mask选择特定区域的生成. 论文思路简单清晰, 适用于多种任务
	
- **Few-shot Image Generation with Elastic Weight Consolidation**  <Br>
[Yijun Li](https://yijunmaverick.github.io/), [Richard Zhang](https://richzhang.github.io/), [Jingwan Lu](https://research.adobe.com/person/jingwan-lu/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/) <Br>
[NeurIPS 2020] [[Project](https://yijunmaverick.github.io/publications/ewc/)] <Br>
	
- **Analyzing and Improving the Image Quality of StyleGAN** <Br>
Tero Karras, [Samuli Laine](https://users.aalto.fi/~laines9/), Miika Aittala, Janne Hellsten, Jaakko Lehtinen, [Timo Aila](https://users.aalto.fi/~ailat1/) <Br>
[CVPR 2020] [[TF-Code](https://github.com/NVlabs/stylegan2)]  <Br>
[★☆] 对StyleGAN做了一些改进, 如去掉减均值操作
	
- **Training Generative Adversarial Networks with Limited Data** <Br>
Tero Karras, Miika Aittala, Janne Hellsten, [Samuli Laine](https://users.aalto.fi/~laines9/), [Jaakko Lehtinen](https://users.aalto.fi/~lehtinj7/), [Timo Aila](https://users.aalto.fi/~ailat1/) <Br>
[arXiv 2006] [[TF-Code](https://github.com/NVlabs/stylegan2-ada)] [[Pytorch-Code](https://github.com/NVlabs/stylegan2-ada-pytorch)]  <Br>
[**StyleGAN2-ADA**]

- **Learning to Predict Layout-to-image Conditional Convolutions for Semantic Image Synthesis** <Br>
[Xihui Liu](https://xh-liu.github.io), [Guojun Yin](https://gjyin91.github.io/), [Jing Shao](https://amandajshao.github.io/), [Xiaogang Wang](https://www.ee.cuhk.edu.hk/~xgwang/), [Hongsheng Li](https://www.ee.cuhk.edu.hk/~hsli/) <Br>
[NIPS 2019] [[Pytorch-Code](https://github.com/xh-liu/CC-FPSE)]  <Br>
[**CC-FPSE**] [★] 使用分割图通过一个网络预测每个pixel我的卷积参数, 虽然使用的depthwise卷积, 但参数量仍然非常庞大, 所以生成的图像较小.
	
- **Large Scale GAN Training for High Fidelity Natural Image Synthesis** <Br>
Andrew Brock, [Jeff Donahue](https://jeffdonahue.com/), Karen Simonyan <Br>
[ICLR 2019] [[Pytorch-Code](https://github.com/ajbrock/BigGAN-PyTorch)]  <Br>
[**BigGAN**] [★☆] 加大网络复杂度和训练batch size, 另外使用了截断等一些trick, 大幅提升了生成效果
	
- **SinGAN: Learning a generative model from a single natural image** <Br>
[Tamar Rott Shaham](https://tamarott.github.io/), [Tali Dekel](people.csail.mit.edu/talidekel/), [Tomer Michaeli](https://tomer.net.technion.ac.il/) <Br>
[ICCV 2019 Best Paper] [[Project](https://tamarott.github.io/SinGAN.htm)] [[Pytorch-Code](https://github.com/tamarott/SinGAN)]  <Br>

- **Dynamic-Net: Tuning the Objective Without Re-training for Synthesis Tasks** <Br>
Alon Shoshan, [Roey Mechrez](https://roimehrez.github.io/), [Lihi Zelnik-Manor](https://webee.technion.ac.il/~lihi/)  <Br>
[ICCV 2019] [[Project](https://cgm.technion.ac.il/Computer-Graphics-Multimedia/Software/DynamicNet/)] [[PyTorch-Code](https://github.com/AlonShoshan10/dynamic_net)] <Br>
[★☆] 先以Objective 0训练主干网络, 之后固定主干网络以Objective 1训练tuning block. 测试时手动指定插值系数, 达到在O0和O1之间的输出效果. 论文思路和实现都很简单, 分析论述方式值得学习
	
- **Semantic Image Synthesis with Spatially-Adaptive Normalization** <Br>
[Taesung Park](https://taesung.me/), [Ming-Yu Liu](http://mingyuliu.net/), [Ting-Chun Wang](https://tcwang0509.github.io/), [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/)     <Br>
[CVPR 2019 Oral] [[Project](https://nvlabs.github.io/SPADE/)] [[PyTorch-Code](https://github.com/NVlabs/SPADE)]<Br>
[**SPADE**] [★★] 提出一个与AdaIN结构相似的SPADE模块, 用于将语义信息嵌入到生成模型中

- **A Style-Based Generator Architecture for Generative Adversarial Networks** <Br>
Tero Karras, [Samuli Laine](https://users.aalto.fi/~laines9/), [Timo Aila](https://users.aalto.fi/~ailat1/) <Br>
[CVPR 2019] [[TF-Code](https://github.com/NVlabs/stylegan)]  <Br>
[**StyleGAN**] [★★☆] 通过若干FC层得到中间向量, 使用AdaIn的形式将中间向量作用在生成器上

- **Image Generation From Layout** <Br>
[Bo Zhao](https://www.zhaobo.me/), [Lili Meng](https://lilimeng1103.wixsite.com/research-site), Weidong Yin, [Leonid Sigal](https://www.cs.ubc.ca/~lsigal/) <Br>
[CVPR 2019 Oral] [[Pytorch-Code](https://github.com/zhaobozb/layout2im)]  <Br>

- **Progressive Growing of GANs for Improved Quality, Stability, and Variation** <Br>
[Qifeng Chen](https://cqf.io/), [Vladlen Koltun](http://vladlen.info/)   <Br>
[CVPR 2018] [[Project](https://cqf.io/ImageSynthesis/)] [[TF-Code](https://github.com/CQFIO/PhotographicImageSynthesis)] <Br>

- **High-Resolution Image Synthesis and Semantic Manipulation with Conditional GANs** <Br>
[Ting-Chun Wang](https://tcwang0509.github.io/), [Ming-Yu Liu](http://mingyuliu.net/), [Jun-Yan Zhu](http://people.eecs.berkeley.edu/~junyanz/), Andrew Tao, [Jan Kautz](http://jankautz.com/), [Bryan Catanzaro](http://catanzaro.name/) <Br>
[CVPR 2018] [[Project](https://tcwang0509.github.io/pix2pixHD/)] [[Pytorch-Code](https://github.com/NVIDIA/pix2pixHD)] <Br>
[**pix2pixHD**] [★☆] 生成2048 x 1024的高清图像, 提出了一个local到global的多尺度生成器结构, 使用多尺度的判别器, 提出使用判别器的中间层feature相似度作为一个loss
	
- **Progressive Growing of GANs for Improved Quality, Stability, and Variation** <Br>
[Tero Karras](https://research.nvidia.com/person/tero-karras), [Timo Aila](https://research.nvidia.com/person/timo-aila), [Samuli Laine](https://users.aalto.fi/~laines9/), [Jaakko Lehtinen](https://users.aalto.fi/~lehtinj7/)   <Br>
[ICLR 2018] [[Pytorch-Code](https://github.com/tkarras/progressive_growing_of_gans)] <Br>
[★★☆]
	


	
	
# Image Translation
- **AgileGAN: Stylizing Portraits by Inversion-Consistent Transfer Learning** <Br>
[Guoxian Song](https://guoxiansong.github.io/homepage/index.html), [Linjie Luo](http://linjieluo.com/), [Jing Liu](https://www.jingliu.net/), [Wan-Chun Ma](https://en.wikipedia.org/wiki/Alex_Ma), [Chunpong Lai](https://guoxiansong.github.io/homepage/index.html), [Chuanxia Zheng](https://www.chuanxiaz.com/), [Tat-Jen Cham](https://www.ntu.edu.sg/home/astjcham/)   <Br>
[SIGGRAPH 2021] [[Project](https://guoxiansong.github.io/homepage/agilegan.html)]  <Br>

- **The Spatially-Correlative Loss for Various Image Translation Tasks** <Br>
[Chuanxia Zheng](https://lyndonzheng.github.io/), [Tat-Jen Cham](https://personal.ntu.edu.sg/astjcham/), [Jianfei Cai](https://jianfei-cai.github.io/)    <Br>
[CVPR 2021] [[Project](http://www.chuanxiaz.com/publication/flsesim/)] [[Pytorch-Code](https://github.com/lyndonzheng/F-LSeSim)]  <Br>

- **Unpaired Image-to-Image Translation via Latent Energy Transport** <Br>
[Yang Zhao](https://sites.google.com/view/zhao-yang/), Jianwen Xie, Ping Li  <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/YangNaruto/latent-energy-transport)]  <Br>

- **CoCosNet v2: Full-Resolution Correspondence Learning for Image Translation** <Br>
[Xingran Zhou](http://xingranzh.github.io/), [Bo Zhang](https://bo-zhang.me/), [Ting Zhang](https://www.microsoft.com/en-us/research/people/tinzhan/), [Pan Zhang](https://panzhang0212.github.io/), [Jianmin Bao](https://jianminbao.github.io/), [Dong Chen](https://www.microsoft.com/en-us/research/people/doch/), [Zhongfei Zhang](https://www.cs.binghamton.edu/~zhongfei/), [Fang Wen](https://www.microsoft.com/en-us/research/people/fangwen/)   <Br>
[CVPR 2021 Oral] [[Pytorch-Code](https://github.com/microsoft/CoCosNet-v2)]  <Br>

- **High-Resolution Photorealistic Image Translation in Real-Time: A Laplacian Pyramid Translation Network** <Br>
[Tamar Rott Shaham](https://tamarott.github.io/), [Michaël Gharbi](http://www.mgharbi.com/), [Richard Zhang](http://richzhang.github.io/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/), [Tomer Michaeli](https://tomer.net.technion.ac.il/)  <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/csjliang/LPTN)]  <Br>
[**LPTN**]

- **Spatially-Adaptive Pixelwise Networks for Fast Image Translation** <Br>
[Tamar Rott Shaham](https://tamarott.github.io/), [Michaël Gharbi](http://www.mgharbi.com/), [Richard Zhang](http://richzhang.github.io/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/), [Tomer Michaeli](https://tomer.net.technion.ac.il/)  <Br>
[[Project](https://tamarott.github.io/ASAPNet_web/)]  <Br>
[**ASAPNet**] [★★] (**快速图像生成**) 在小分辨率(降32倍)上预测每个pixel的MLP映射系数, 将位置信息编码为不同频率的sin, cosine信息, 提升了生成图像的细节. 论文很有实际意义, 值得学习. 

- **Few-shot Image Generation via Cross-domain Correspondence** <Br>
[Utkarsh Ojha](https://utkarshojha.github.io/) , [Yijun Li](https://yijunmaverick.github.io/), [Jingwan Lu](https://research.adobe.com/person/jingwan-lu/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/), [Yong Jae Lee](https://web.cs.ucdavis.edu/~yjlee/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/), [Richard Zhang](https://richzhang.github.io/)  <Br>
[CVPR 2021] [[Project](https://utkarshojha.github.io/few-shot-gan-adaptation/)]  [[Pytorch-Code](https://github.com/utkarshojha/few-shot-gan-adaptation)]  <Br>
	
- **Unsupervised Image Transformation Learning via Generative Adversarial Networks** <Br>
[Kaiwen Zha](http://kaiwenzha.github.io),  [Yujun Shen](http://shenyujun.github.io),  [Bolei Zhou](http://bzhou.ie.cuhk.edu.hk/)  <Br>
[arXiv 2103] [[Project](https://genforce.github.io/trgan/)]  <Br>
[**TrGAN**]

- **COCO-FUNIT: Few-Shot Unsupervised Image Translation with a Content Conditioned Style Encoder** <Br>
[Kuniaki Saito](http://ai.bu.edu/ksaenko.html), [Kate Saenko](http://cs-people.bu.edu/keisaito/), [Ming-Yu Liu](http://mingyuliu.net/) <Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/nvlabs/imaginaire)]  <Br>

- **Contrastive Learning for Unpaired Image-to-Image Translation** <Br>
[Taesung Park](https://taesung.me/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/), [Richard Zhang](https://richzhang.github.io/),  [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/) <Br>
[ECCV 2020] [[Project](http://taesung.me/ContrastiveUnpairedTranslation/)] [[Pytorch-Code](https://github.com/taesungp/contrastive-unpaired-translation)]  <Br>
[**CUT**]

- **DeepI2I: Enabling Deep Hierarchical Image-to-Image Translation by Transferring from GANs** <Br>
[Yaxing Wang](https://yaxingwang.github.io//), [Lu Yu](https://yulu0724.github.io/), [Joost van de Weijer](http://www.cvc.uab.es/LAMP/joost/) <Br>
[NeurIPS 2020] [[Pytorch-Code](https://github.com/yaxingwang/DeepI2I)]  <Br>
	
- **Mask Based Unsupervised Content Transfer** <Br>
Ron Mokady, [Sagie Benaim](https://sagiebenaim.github.io/), [Lior Wolf](http://www.cs.tau.ac.il/~wolf/), [Amit Bermano](https://www.cs.tau.ac.il/~amberman/) <Br>
[ICLR 2020] [[Pytorch-Code](https://github.com/rmokady/mbu-content-tansfer)]  <Br>

- **STGAN: A Unified Selective Transfer Network for Arbitrary Image Attribute Editing**  <Br>
Ming Liu, Yukang Ding, Min Xia, Xiao Liu, Errui Ding, [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), Shilei Wen <Br>
[CVPR 2019] [[Pytorch-Code](https://github.com/csmliu/STGAN)]   <Br>
	
- **RelGAN: Multi-Domain Image-to-Image Translation via Relative Attributes** <Br>
Po-Wei Wu, Yu-Jing Lin, Che-Han Chang, Edward Y. Chang, Shih-Wei Liao <Br>
[[Pytorch-Code](https://github.com/elvisyjlin/RelGAN-PyTorch)]   <Br>
	
- **Emerging Disentanglement in Auto-Encoder Based Unsupervised Image Content Transfer** <Br>
[Ori Press](https://oripress.com/), [Tomer Galanti](https://www.tau.ac.il/~tomerga2/), [Sagie Benaim](https://sagiebenaim.github.io/), [Lior Wolf](http://www.cs.tau.ac.il/~wolf/) <Br>
[ICLR 2019] [[Pytorch-Code](https://github.com/oripress/ContentDisentanglement)]   <Br>

- **StarGAN v2: Diverse Image Synthesis for Multiple Domains** <Br>
[Yunjey Choi](https://yunjey.github.io/), [Youngjung Uh](https://sites.google.com/site/youngjunguh), Jaejun Yoo, Jung-Woo Ha<Br>
[CVPR 2020] [[Pytorch-Code](https://github.com/clovaai/stargan-v2)]<Br>

- **StarGAN: Unified Generative Adversarial Networks for Multi-Domain Image-to-Image Translation** <Br>
[Yunjey Choi](https://yunjey.github.io/), [Minje Choi](http://www.minjechoi.com/), Munyoung Kim, Jung-Woo Ha, [Sunghun Kim](http://home.cse.ust.hk/~hunkim/), [Jaegul Choo](https://sites.google.com/site/jaegulchoo/) <Br>
[CVPR 2018 Oral] [[Pytorch-Code](https://github.com/yunjey/stargan)]   <Br>

- **Multimodal Unsupervised Image-to-image Translation** <Br>
[Xun Huang](http://www.cs.cornell.edu/~xhuang/), [Ming-Yu Liu](http://mingyuliu.net/), [Serge Belongie](https://vision.cornell.edu/se3/), [Jan Kautz](https://jankautz.com/) <Br>
[ECCV 2018] [[Pytorch-Code](https://github.com/NVlabs/MUNIT)]  <Br>
[**MUNIT**]

- **DRIT++: Diverse Image-to-Image Translation via Disentangled Representations** <Br>
[Hsin-Ying Lee](http://vllab.ucmerced.edu/hylee/), [Hung-Yu Tseng](https://sites.google.com/site/hytseng0509/), [Qi Mao](https://sites.google.com/view/qi-mao/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/), [Yu-Ding Lu](https://jonlu0602.github.io/), [Maneesh Kumar Singh](https://scholar.google.com/citations?user=hdQhiFgAAAAJ), [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/)  <Br>
[IJCV 2020] [[Pytorch-Code](https://github.com/HsinYingLee/DRIT)]  <Br>

- **Diverse Image-to-Image Translation via Disentangled Representations** <Br>
[Hsin-Ying Lee](http://vllab.ucmerced.edu/hylee/), [Hung-Yu Tseng](https://sites.google.com/site/hytseng0509/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/), [Maneesh Kumar Singh](https://scholar.google.com/citations?user=hdQhiFgAAAAJ), [Ming-Hsuan Yang](http://faculty.ucmerced.edu/mhyang/) <Br>
[ECCV 2018 Oral] <Br>
[**DRIT**]

- **Image-to-Image Translation with Conditional Adversarial Nets** <Br>
 [Phillip Isola](http://web.mit.edu/phillipi/), [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/), [Tinghui Zhou](https://people.eecs.berkeley.edu/~tinghuiz/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/) <Br>
[CVPR 2017] [[Project](https://github.com/junyanz/pytorch-CycleGAN-and-pix2pix)]  <Br>
[**pix2pix**] [★★☆] 使用patchGAN的图像迁移的经典方法
	
- **Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks** <Br>
[Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/), [Taesung Park](https://taesung.me/), [Phillip Isola](http://web.mit.edu/phillipi/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/) <Br>
[ICCV 2017] [[Project](https://junyanz.github.io/CycleGAN/)]  <Br>
[**CycleGAN**] [★★★] 无监督图像迁移

- **Toward Multimodal Image-to-Image Translation** <Br>
[Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/), [Richard Zhang](http://richzhang.github.io/), [Deepak Pathak](https://www.cs.cmu.edu/~dpathak/), [Trevor Darrell](https://people.eecs.berkeley.edu/~trevor/), [Alexei A. Efros](https://people.eecs.berkeley.edu/~efros/), [Oliver Wang](http://www.oliverwang.info/), [Eli Shechtman](https://research.adobe.com/person/eli-shechtman/) <Br>
[NIPS 2017] [[Pytorch-Code](https://github.com/junyanz/BicycleGAN)]  <Br>
[**BicycleGAN**]

- **Unsupervised image-to-image translation networks** <Br>
[Ming-Yu Liu](http://mingyuliu.net/), [Thomas Breuel](http://www.tmbdev.org/), [Jan Kautz](https://jankautz.com/) <Br>
[NIPS 2017] [[Pytorch-Code](https://github.com/nvlabs/imaginaire)]  <Br>
[**UNIT**]


	
	

# Image Manipulation
- **HyperStyle: StyleGAN Inversion with HyperNetworks for Real Image Editing** <Br>
[Yuval Alaluf](https://yuval-alaluf.github.io/), Omer Tov, [Ron Mokady](https://rmokady.github.io/), [Rinon Gal](https://rinongal.github.io/), [Amit H. Bermano](https://www.cs.tau.ac.il/~amberman/)  <Br>
[CVPR 2021] [[Project](https://yuval-alaluf.github.io/hyperstyle/)] [[Pytorch-Code](https://github.com/yuval-alaluf/hyperstyle)]  <Br>

- **High-Fidelity GAN Inversion for Image Attribute Editing** <Br>
[Tengfei Wang](https://tengfei-wang.github.io/), [Yong Zhang](https://yzhang2016.github.io/yongnorriszhang.github.io/), [Yanbo Fan](https://sites.google.com/site/yanbofan0124/), Jue Wang, [Qifeng Chen](https://cqf.io/)  <Br>
[CVPR 2021] [[Project](https://tengfei-wang.github.io/HFGI/)] [[Pytorch-Code](https://github.com/Tengfei-Wang/HFGI)]  <Br>
[**HFGI**]

- **HairCLIP: Design Your Hair by Text and Reference Image** <Br>
Tianyi Wei, [Dongdong Chen](http://www.dongdongchen.bid/), Wenbo Zhou, [Jing Liao](https://liaojing.github.io/html/index.html), Zhentao Tan, Lu Yuan, Weiming Zhang, Nenghai Yu  <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/wty-ustc/HairCLIP)]  <Br>

- **Blended Diffusion for Text-driven Editing of Natural Images** <Br>
[Omri Avrahami](https://omriavrahami.com/), [Dani Lischinski](https://www.cs.huji.ac.il/~danix/), [Ohad Fried](https://www.ohadf.com/)  <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/omriav/blended-diffusion)]  <Br>

- **Style Transformer for Image Inversion and Editing** <Br>
Xueqi Hu, Qiusheng Huang, Zhengyi Shi, Siyuan Li, [Changxin Gao](https://sites.google.com/site/changxingao), Li Sun, Qingli Li  <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/sapphire497/style-transformer)]  <Br>

- **DeFLOCNet: Deep Image Editing via Flexible Low-level Controls** <Br>
[Hongyu Liu](https://github.com/KumapowerLIU/DeFLOCNet#jump1), [Ziyu Wan](http://raywzy.com/), [Wei Huang](https://github.com/KumapowerLIU/DeFLOCNet#jump1), [Yibing Song](https://ybsong00.github.io/), [Xintong Han](http://users.umiacs.umd.edu/~xintong/) , [Jing Liao](https://liaojing.github.io/html/), [Bin Jiang](https://github.com/KumapowerLIU/DeFLOCNet#jump1), [Wei Liu](https://scholar.google.com/citations?user=AjxoEpIAAAAJ&hl=zh-CN)  <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/KumapowerLIU/DeFLOCNet)]  <Br>
	
- **HiSD: Image-to-image Translation via Hierarchical Style Disentanglement** <Br>
Xinyang Li, Shengchuan Zhang, Jie Hu, Liujuan Cao, [Xiaopeng Hong](https://hongxiaopeng.com/), [Xudong Mao](https://xudongmao.github.io/), Feiyue Huang, Yongjian Wu, [Rongrong Ji](https://mac.xmu.edu.cn/rrji_en/)  <Br>
[CVPR 2021 Oral] [[Pytorch-Code](https://github.com/imlixinyang/HiSD)]  <Br>
[★★] 大致浏览, 可将人脸各属性解耦, 并实现准确控制. 将CelebA的属性信息进一步划分为相互独立的tags(如刘海, 眼镜)和互斥的attributes(如黑发和棕发),并为每个tag和attribute分别构造模块. 论文整体思路很清晰, 代码也很友好, 可以仔细研究一下.
	
- **Closed-Form Factorization of Latent Semantics in GANs** <Br>
[Yujun Shen](https://shenyujun.github.io/), [Bolei Zhou](http://bzhou.ie.cuhk.edu.hk/) <Br>
[CVPR 2021 Oral] [[Project](https://genforce.github.io/sefa/)] [[Pytorch-Code](https://github.com/genforce/sefa)]  <Br>
[**SeFa**]

- **IDInvert：In-Domain GAN Inversion for Real Image Editing** <Br>
[Jiapeng Zhu](https://zhujiapeng.github.io/), [Yujun Shen](https://shenyujun.github.io/), [Deli Zhao](https://sites.google.com/site/zhaodeli/), [Bolei Zhou](http://bzhou.ie.cuhk.edu.hk/) <Br>
[ECCV 2020] [[Project](https://genforce.github.io/idinvert/)] [[TF-Code](https://github.com/genforce/idinvert)]  <Br>
	
- **Collaborative Learning for Faster StyleGAN Embedding** <Br>
Shanyan Guan, [Ying Tai](https://tyshiwo.github.io/), Bingbing Ni, [Feida Zhu](https://zhufeida.github.io/), Feiyue Huang, Xiaokang Yang<Br>
[arXiv 2007] <Br>
[★] (**latent code embedding**) 

- **mage2StyleGAN: How to Embed Images Into the StyleGAN Latent Space?** <Br>
Rameen Abdal, Yipeng Qin, Peter Wonka <Br>
[ICCV 2019] [[TF-Code](https://github.com/NVlabs/stylegan)]  <Br>
[★☆] (**latent code embedding**) 



# Style Transfer
- **Pastiche Master: Exemplar-Based High-Resolution Portrait Style Transfer** <Br>
[Shuai Yang](https://williamyang1991.github.io/), [Liming Jiang](https://liming-jiang.com/), [Ziwei Liu](https://liuziwei7.github.io/), [Chen Change Loy](https://www.mmlab-ntu.com/person/ccloy/) <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/williamyang1991/DualStyleGAN)]  <Br>
[**DualStyleGAN**]

- **Industrial Style Transfer with Large-scale Geometric Warping and Content Preservation** <Br>
Jinchao Yang, Fei Guo, Shuo Chen, [Jun Li](https://sites.google.com/view/junlineu/), [Jian Yang](http://www.patternrecognition.cn/~jian/)  <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/jcyang98/InST)]  <Br>
[**InST**]

- **Exact Feature Distribution Matching for Arbitrary Style Transfer and Domain Generalization** <Br>
Yabin Zhang, Minghan Li, Ruihuang Li, Kui Jia, Lei Zhang <Br>
[CVPR 2021 Oral] [[Pytorch-Code](https://github.com/YBZh/EFDM)]  <Br>

- **Style-ERD: Responsive and Coherent Online Motion Style Transfer** <Br>
[Tianxin Tao](https://tianxintao.github.io/), Xiaohang Zhan, Zhongquan Chen, [Michiel van de Panne](https://www.cs.ubc.ca/~van/) <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/tianxintao/Online-Motion-Style-Transfer)]  <Br>

- **CLIPstyler:Image Style Transfer with a Single Text Condition** <Br>
[Gihyun Kwon](https://sites.google.com/view/gihyunkwon), Jong Chul Ye <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/cyclomon/CLIPstyler)]  <Br>

- **Rethinking and Improving the Robustness of Image Style Transfer** <Br>
[Pei Wang](http://www.svcl.ucsd.edu/~peiwang), [Yijun Li](https://yijunmaverick.github.io/), [Nuno Vasconcelos](http://www.svcl.ucsd.edu/~nuno) <Br>
[CVPR 2021 Oral] [[Pytorch-Code](https://github.com/peiwang062/swag)]  <Br>
[**SWAG**] [★] 实验说明resnet等网络使用的shotcut结构会产生大激活值和小的层间entropy, 不利于基于gram矩阵的loss计算. 因此提出了用softmax平滑激活值, 再用来计算loss.

- **Joint Bilateral Learning for Real-time Universal Photorealistic Style Transfer**  <Br>
[Xide Xia](https://xidexia.github.io/), Meng Zhang, [Tianfan Xue](http://people.csail.mit.edu/tfxue/), Zheng Sun, Hui Fang, [Brian Kulis](http://people.bu.edu/bkulis/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/) <Br>
[ECCV 2020] <Br>
[★★] 基于HDRNet的实时风格迁移, 创新点尽管不是很多, 但是工作很有价值
