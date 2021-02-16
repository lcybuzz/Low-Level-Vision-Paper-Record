# Table of Contents
- [Super Resolution](#super-resolution)
- [Video Super Resolution](#video-super-restoration)

#  Super Resolution
### SRGAN
**[Paper]**  (CVPR 2017) Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network<Br>
**[Author]** [Christian Ledig](http://www.christianledig.com/), [Lucas Theis](http://theis.io/), [Ferenc Huszar](https://www.inference.vc/about/), Jose Caballero, Andrew Cunningham, Alejandro Acosta, Andrew Aitken, [Alykhan Tejani](http://alykhantejani.github.io/), Johannes Totz, Zehan Wang, Wenzhe Shi <Br>
**[[TF-Code](https://github.com/brade31919/SRGAN-tensorflow)]**  <Br>
	
### ESRGAN
**[Paper]**  (ECCV 2018 workshop) Enhanced Super-Resolution Generative Adversarial Networks <Br>
**[Author]** Xintao Wang, [Ke Yu](https://yuke93.github.io/), Shixiang Wu, [Jinjin Gu](https://www.jasongt.com/), Yihao Liu, Chao Dong, [Yu Qiao](http://mmlab.siat.ac.cn/yuqiao/), [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[[Pytorch-Code](https://github.com/xinntao/ESRGAN)]**  <Br>
	
### *Super-resolution using a GAN to degradate* ★★
**[Paper]**  (ECCV 2018) To learn image super-resolution, use a GAN to learn how to do image degradation first <Br>
**[Author]** [Adrian Bulat](https://www.adrianbulat.com/), [Jing Yang](https://jingyang2017.github.io/), [Georgios Tzimiropoulos](http://www.cs.nott.ac.uk/~pszyt/) <Br>
**[[Pytorch-Code](https://github.com/jingyang2017/Face-and-Image-super-resolution)]**  <Br>
(**使用GAN的无监督学习降质**)
	
### ZSSR ★☆
**[Paper]**  (CVPR 2018) "Zero Shot" Super-Resolution using Deep Internal Learning <Br>
**[Author]** [Assaf Shocher](http://www.wisdom.weizmann.ac.il/~/assafsho/), [Nadav Cohen](http://www.cohennadav.com/), [Michal Irani](https://www.weizmann.ac.il/math/irani/) <Br>
**[[Project](http://www.wisdom.weizmann.ac.il/~vision/zssr/)]** **[[Pytorch-Code](https://github.com/assafshocher/ZSSR)]**  <Br>
DL Zero shot超分较早的一篇, 使用LR内部patch将采样后作为训练输入, 对应的LR patch作为输出, 训练网络. 网络收敛后用来预测LR图像的超分结果.
 
### DBPN ★★
**[Paper]**  (CVPR 2018) Deep Back-Projection Networks For Super-Resolution <Br>
**[Author]** [Muhammad Haris](https://alterzero.github.io/), [Greg Shakhnarovich](https://ttic.uchicago.edu/~gregory/), [Norimichi Ukita](https://www.toyota-ti.ac.jp/Lab/Denshi/iim/ukita/) <Br>
**[[Project](https://alterzero.github.io/projects/DBPN.html)]**  <Br>
提出在神经网络中引入back-projection思想, 引入HR到LR的反馈信息. 这个思路或许可以用在其他形式的网络中, 替代加或乘的特征融合方式.
	
### SFTGAN ★★
**[Paper]**  (CVPR 2018) Recovering Realistic Texture in Image Super-resolution by Deep Spatial Feature Transform <Br>
**[Author]** Xintao Wang, [Ke Yu](https://yuke93.github.io/), Chao Dong, [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/) <Br>
**[[Pytorch-Code](https://github.com/xinntao/SFTGAN)]**  <Br>
**(结合语义的超分)** 从分割图中提取特征作为超分网络feature的scale和shift
  
###  *Super-Resolution with Raw Images* ★
**[Paper]**  (CVPR 2019) Towards Real Scene Super-Resolution with Raw Images  <Br>
**[Author]** [Xiangyu Xu](https://sites.google.com/view/xiangyuxu/%E9%A6%96%E9%A1%B5), Yongrui Ma, [Wenxiu Sun](http://wenxiusun.com/) <Br>
**[[Project](https://sites.google.com/view/xiangyuxu/rawsr_cvpr19)]** <Br>
大致浏览, 利用Raw做细节恢复, 用RGB做Color校正.<Br> 
	
### SFTMD ★
**[Paper]**  (CVPR 2019) Blind Super-Resolution with Iterative Kernel Correction <Br>
**[Author]** [Jinjin Gu](http://www.jasongt.com/), Hannan Lu, [Wangmeng Zuo](http://www.jasongt.com/projectpages/IKC.html), Chao Dong<Br>
**[[Project](http://www.jasongt.com/projectpages/IKC.html)]** <Br>
1) 粗读, 提出一个基于深度学习的交替预测blur kernel和预测超分结果的模型, 对给定的blur有很好的效果 <Br>
2) 文中提出的预测blur kernel并用其辅助超分的思路很有意思, 但对真实图像而言无法获得真实的blur kernel用于训练, 另外论文似乎假设一张图像只有一种blur kernel, 感觉不太合理  <Br>
	
### CameraSR ★
**[Paper]**  (CVPR 2019) Camera Lens Super-Resolution <Br>
**[Author]** Chang Chen, Zhiwei Xiong, Xinmei Tian, Zheng-Jun Zha, Feng Wu<Br>
**[[Code & Data](https://github.com/ngchc/CameraSR)]** <Br>
文章认为普通的插值退化不能模拟由于焦距-FOV变化带来的退化 (其实这是一个无论从分析上还是工程中都很明显的事实...). 最重要的贡献是提出了一个真实DSLR和手机的数据集, 但是在生成单反数据集时, 貌似没有考虑焦距变化带来的景深变化.
	
### DPSR ★★
**[Paper]**  (CVPR 2019) Deep Plug-and-Play Super-Resolution for Arbitrary Blur Kernels <Br>
**[Author]** [Kai Zhang](https://cszn.github.io/), [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
**[[Pytorch-Code](https://github.com/cszn/DPSR)]** **[[Pytorch-IR-Toolbox](https://github.com/cszn/KAIR)]** <Br>
1. 把HR到LR的退化解释成bicubic降采样+非盲blur kernel退化+加性高斯白噪声的过程. 
2. 将求解过程用HQS变量分裂法分解为去模糊和超分+去噪两步, 第一步在频谱域求闭式解, 避免了模糊现象; 第二步可以使用现有的SR方法, 只需额外加入一噪声level. 采用迭代的形式交替求解.
3. 非盲kernel这个先验其实挺强的, 而且只在生成的数据集上做了实验. 但是实际效果来看, 在真实图像上的效果的确很不错.

### KernelGAN ★★
**[Paper]**  (NIPS 2019 Oral) Blind Super-Resolution Kernel Estimation using an Internal-GAN <Br>
**[Author]** Sefi Bell-Kligler, [Assaf Shocher](http://www.wisdom.weizmann.ac.il/~/assafsho/), [Michal Irani](https://www.weizmann.ac.il/math/irani/) <Br>
**[[Project](http://www.wisdom.weizmann.ac.il/~vision/kernelgan/)]** **[[Pytorch-Code](https://github.com/sefibk/KernelGAN)]**  <Br>
无监督预测降质核并进行超分的方法. 使用若干个现象卷积层的GAN预测降质kernel, 训练的的GAN可以合成一个kernel, 作为该图形的降质核, 网络训练采用LSGAN和若干正则项构成. 预测的模糊核作为ZSSR的降质核, 再无监督地预测炒粉结果

### DRN ★
**[Paper]** (CVPR 2020) Closed-loop Matters: Dual Regression Networks for Single Image Super-Resolution <Br>
**[Author]**  [Yong Guo](http://www.guoyongcs.com/), Jian Chen, [Jingdong Wang](https://jingdongwang2017.github.io/), Qi Chen, [Jiezhang Cao](https://www.jiezhangcao.com/), Zeshuai Deng, [Yanwu Xu](https://xuyanwu.github.io/), [Mingkui Tan](https://tanmingkui.github.io/)<Br>
**[[Pytorch-Code](https://github.com/guoyongcs/DRN)]** <Br>
训练时引入HR->LR的映射, 对LR图像进行额外的约束. 大致浏览.
 
### USRNet ★
**[Paper]** (CVPR 2020) Deep Unfolding Network for Image Super-Resolution <Br>
**[Author]** [Kai Zhang](https://cszn.github.io/), [Luc Van Gool](https://vision.ee.ethz.ch/people-details.OTAyMzM=.TGlzdC8zMjQ4LC0xOTcxNDY1MTc4.html), [Radu Timofte](http://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/cszn/USRNet)]** <Br>
大致浏览, 通过变量分解迭代求解, 一部分用FFT直接求解, 一部分用网络训练.

### RFANet ★
**[Paper]** (CVPR 2020) Residual Feature Aggregation Network for Image Super-resolution <Br>
**[Author]** Jie Liu, Wenjie Zhang, Yuting Tang, Jie Tang, Gangshan Wu <Br>
**[[Code](https://github.com/njulj/RFANet)]** <Br>
设计了一个残差聚合和attention模块
	
### Cross Scale Non Local Attention ★☆
**[Paper]** (CVPR 2020) Image Super-Resolution with Cross-Scale Non-Local Attention and Exhaustive Self-Exemplars Mining <Br>
**[Author]** [Yiqun Mei](http://yiqunm2.web.illinois.edu/), [Yuchen Fan](https://ychfan.github.io/), [Yuqian Zhou](https://yzhouas.github.io/), Lichao Huang, [Thomas S. Huang](https://ifp-uiuc.github.io/), [Humphrey Shi](https://www.humphreyshi.com/) <Br>
**[[Pytorch-Code](https://github.com/SHI-Labs/Cross-Scale-Non-Local-Attention)]** <Br>
设计了LR到降采样LR的attention, 挖掘不同尺度下的non-local相似性

### TTSR ★★
**[Paper]** (CVPR 2020) TTSR: Learning Texture Transformer Network for Image Super-Resolution <Br>
**[Author]** Fuzhi Yang, Huan Yang, Jianlong Fu, Hongtao Lu, Baining Guo <Br>
**[[Pytorch-Code](https://github.com/researchmm/TTSR)]** <Br>
使用transformer从参考图像获取纹理信息
	
### *Unpaired Image Super-Resolution using Pseudo-Supervision* ★
**[Paper]** (CVPR 2020) Unpaired Image Super-Resolution using Pseudo-Supervision <Br>
**[Author]** Shunta Maeda <Br>
大致浏览, 类似CycleGAN的结构

### SPSR ★
**[Paper]** (CVPR 2020) Structure-Preserving Super Resolution with Gradient Guidance  <Br>
**[Author]** Cheng Ma, [Yongming Rao](https://raoyongming.github.io/), Yean Cheng, Ce Chen, [Jiwen Lu](http://ivg.au.tsinghua.edu.cn/Jiwen_Lu/), Jie Zhou <Br>
**[[Pytorch-Code](https://github.com/Maclory/SPSR)]** <Br>
在常规超分分支外加入一个gradient分支

### PULSE
**[Paper]** (CVPR 2020) PULSE: Self-Supervised Photo Upsampling via Latent Space Exploration of Generative Models  <Br>
**[Author]** [Sachit Menon](https://sachit-menon.github.io/), Alexandru Damian, Shijia Hu, Nikhil Ravi, [Cynthia Rudin](https://users.cs.duke.edu/~cynthia/home.html) <Br>
**[[Pytorch-Code](https://github.com/adamian98/pulse)]** <Br>
	
### Correction Filter
**[Paper]** (CVPR 2020 Oral) Correction Filter for Single Image Super-Resolution: Robustifying Off-the-Shelf Deep Super-Resolvers  <Br>
**[Author]** Shady Abu Hussein, [Tom Tirer](https://tirertom.wixsite.com/homepage), [Raja Giryes](http://web.eng.tau.ac.il/~raja/) <Br>
**[[Pytorch-Code](https://github.com/shadyabh/Correction-Filter)]** <Br>
	
### MZSR
**[Paper]** (CVPR 2020) Meta-Transfer Learning for Zero-Shot Super-Resolution <Br>
**[Author]** Jae Woong Soh, Sunwoo Cho, Nam Ik Cho <Br>
**[[TF-Code](https://github.com/JWSoh/MZSR)]** <Br>
	
### CutBlur
**[Paper]** (CVPR 2020) Rethinking Data Augmentation for Image Super-resolution: A Comprehensive Analysis and a New Strategy <Br>
**[Author]* Jaejun Yoo, [Namhyuk Ahn](https://nmhkahn.github.io/), [Kyung-Ah Sohn](https://sites.google.com/site/kasohn/home) <Br>
**[[Pytorch-Code](https://github.com/clovaai/cutblur)]** <Br>
	
### CARB ★☆
**[Paper]**  (CVPRW 2020) Guided Frequency Separation Network for Real-World Super-Resolution <Br>
**[Author]** Yuanbo Zhou, Wei Deng, Tong Tong, Qinquan Gao<Br>
**[[Pytorch-Code](https://github.com/fzuzyb/2020NTIRE-Guided-Frequency-Separation-Network-for-RWSR)]** <Br>
使用一套基于GAN的无监督方案生成真实LR图像对, 在该方案中提出了所谓颜色引导生成器网络, 用于产生AdaIn中的参数. 
	
### REAL-SR ★★
**[Paper]** (CVPRW 2020) Real-World Super-Resolution via Kernel Estimation and Noise Injection <Br>
**[Author]** Xiaozhong Ji，Yun Cao， [Ying Tai](https://tyshiwo.github.io/)， Chengjie Wang，Jilin Li，Feiyue Huang<Br>
**[[Pytorch-Code](https://github.com/Tencent/Real-SR)]** <Br>
设计了一个退化图像的流程, 通过随机模糊核和注入噪声, 生成接近于真实的样本, 在NTIRE 2020超分竞赛中取得了第一名, 并且在真实数据上表现良好

### MAFFSRN ★☆
**[Paper]**  (arXiv 2008) Ultra Lightweight Image Super-Resolution with Multi-Attention Layers <Br>
**[Author]** Abdul Muqeet, Jiwon Hwang, Subin Yang, Jung Heum Kang, Yongwoo Kim, Sung-Ho Bae<Br>
**[[Code](https://github.com/AbdulMoqeet/MAFFSRN)]** <Br>
轻量级超分网络, 在AIM 2020上取得了不错的成绩, 结构可学习
	
### RFDN ★☆
**[Paper]**  (arXiv 2009) Residual Feature Distillation Network for Lightweight Image Super-Resolution <Br>
**[Author]** Jie Liu, Jie Tang, Gangshan Wu<Br>
**[[Pytorch-Code](https://github.com/njulj/RFDN)]** <Br>
AIM2020-ESR冠军方案, 基于IDN提出了几点改善.

### CDC
**[Paper]**  (ECCV 2020) Component Divide-and-Conquer for Real-World Image Super-Resolution <Br>
**[Author]** Pengxu Wei, Ziwei Xie, Hannan Lu, Zongyuan Zhan, [Qixiang Ye](http://people.ucas.ac.cn/~qxye?language=en), [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo), Liang Lin Lin<Br>
**[[Pytorch-Code](https://github.com/xiezw5/Component-Divide-and-Conquer-for-Real-World-Image-Super-Resolution)]** <Br>
	
### SRFlow
**[Paper]**  (ECCV 2020) Learning the Super-Resolution Space with Normalizing Flow <Br>
**[Author]** Andreas Lugmayr, [Martin Danelljan](https://martin-danelljan.github.io/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html), [Radu Timofte](https://people.ee.ethz.ch/~timofter/) <Br>
**[[Pytorch-Code](https://github.com/andreas128/SRFlow)]** <Br>	

### HAN
**[Paper]**  (ECCV 2020) Single Image Super-Resolution via a Holistic Attention Network <Br>
**[Author]** Ben Niu, Weilei Wen, [Wenqi Ren](https://sites.google.com/site/renwenqi888/home), Xiangde Zhang, Lianping Yang, Shuzhen Wang, Kaihao Zhang, Xiaochun Cao, Haifeng Shen <Br>
**[[Pytorch-Code](https://github.com/wwlCape/HAN)]** <Br>	
	
### SFM
**[Paper]**  (ECCV 2020) Stochastic Frequency Masking to Improve Super-Resolution and Denoising Networks <Br>
**[Author]** [Majed El Helou](https://majedelhelou.github.io/), Ruofan Zhou, Sabine Süsstrunk <Br>
**[[Pytorch-Code](https://github.com/majedelhelou/SFM)]** <Br>	
	
### VarSR
**[Paper]**  (ECCV 2020) VarSR: Variational Super-Resolution Network for Very Low Resolution Images <Br>
**[Author]** Sangeek Hyun, Jae-Pil Heo <Br>

### PISR
**[Paper]**  (ECCV 2020) Learning with Privileged Information for Efficient Image Super-Resolution <Br>
**[Author]** Junghyup Lee, Dohyung Kim, [Wonkyung Lee](https://cv.wonkyunglee.io/), [Bumbsub Ham](https://bsham.github.io/) <Br>
**[[Project](https://cvlab.yonsei.ac.kr/projects/PISR/)]** <Br> **[[Pytorch-Code](https://github.com/cvlab-yonsei/PISR)]** <Br>	

### *Efficient Super Resolution Using Binarized Neural Network*
**[Paper]**  (ECCV 2020) Efficient Super Resolution Using Binarized Neural Network <Br>
**[Author]** Yinglan Ma, Hongyu Xiong, Zhe Hu, Lizhuang Ma <Br>
	
### *Towards Content-independent Multi-Reference Super-Resolution: Adaptive Pattern Matching and Feature Aggregation*
**[Paper]**  (ECCV 2020) Towards Content-independent Multi-Reference Super-Resolution: Adaptive Pattern Matching and Feature Aggregation <Br>
**[Author]** Xu Yan, Weibing Zhao, Kun Yuan, Ruimao Zhang, [Zhen Li](https://mypage.cuhk.edu.cn/academics/lizhen/), Shuguang Cui <Br>

 ### *Zero-Shot Image Super-Resolution with Depth Guided Internal Degradation Learning*
**[Paper]** (ECCV 2020) Zero-Shot Image Super-Resolution with Depth Guided Internal Degradation Learning <Br>
**[Author]** Xi Cheng, Zhenyong Fu, Jian Yang <Br>

### MLSR
**[Paper]** (ECCV 2020) Fast Adaptation to Super-Resolution Networks via Meta-Learning <Br>
**[Author]** Xi Cheng, Zhenyong Fu, Jian Yang <Br>
**[[TF-Code](https://github.com/parkseobin/MLSR)]** <Br>
  
	

# Video Super Resolution
### STARnet
**[Paper]**  (CVPR 2020) Space-Time-Aware Multi-Resolution Video Enhancement <Br>
**[Author]** [Muhammad Haris](https://alterzero.github.io/), [Greg Shakhnarovich](https://ttic.uchicago.edu/~gregory/), [Norimichi Ukita](https://www.toyota-ti.ac.jp/Lab/Denshi/iim/ukita/)<Br>
**[[Pytorch-Code](https://github.com/alterzero/STARnet)]** <Br>
	
### DeepTemporalSR
**[Paper]**  (ECCV 2020) Across Scales & Across Dimensions: Temporal Super-Resolution using Deep Internal Learning <Br>
**[Author]** Liad Pollak Zuckerman, Eyal Naor, George Pisha, [Shai Bagon](https://www.weizmann.ac.il/math/bagon/), Michal Irani <Br>
**[[Project](http://www.wisdom.weizmann.ac.il/~vision/DeepTemporalSR/)]** <Br> **[[Pytorch-Code](https://github.com/eyalnaor/DeepTemporalSR)]** <Br>	

### MuCAN
**[Paper]**  (ECCV 2020) MuCAN: Multi-Correspondence Aggregation Network for Video Super-Resolution <Br>
**[Author]** Wenbo Li, [Xin Tao](http://www.xtao.website/), Taian Guo, [Lu Qi](http://luqi.info/), Jiangbo Lu, [Jiaya Jia](http://jiaya.me/) <Br>

### RSDN
**[Paper]**  (ECCV 2020) Video Super-Resolution with Recurrent Structure-Detail Network <Br>
**[Author]** Takashi Isobe, [Xu Jia](https://stephenjia.github.io/), [Shuhang Gu](https://sites.google.com/site/shuhanggu/), Songjiang Li, Shengjin Wang, Qi Tian<Br>



