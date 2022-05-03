
# Denoising
- [Image Denoising](#image-denoising)
- [Raw Denoising](#raw-denoising)
- [Burst Denoising](#burst-denoising)
- [Datasets](#datasets)
- [Resources](#resources)


# Image Denoising
##### SCUNet
**[Paper]** (arXiv 2003) Practical Blind Denoising via Swin-Conv-UNet and Data Synthesis <Br>
**[Author]** [Kai Zhang](https://cszn.github.io/), [Yawei Li](https://ofsoundof.github.io/), [Jingyun Liang](https://jingyunliang.github.io/), [Jiezhang Cao](https://www.jiezhangcao.com/), [Yulun Zhang](http://yulunzhang.com/), Hao Tang, [Radu Timofte](http://people.ee.ethz.ch/~timofter/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html) <Br>
**[[Pytorch-Code](https://github.com/cszn/SCUNet)]**  <Br>
	
##### FBI-Denoiser
**[Paper]** (CVPR 2021) FBI-Denoiser: Fast Blind Image Denoiser for Poisson-Gaussian Noise <Br>
**[Author]** Jaeseok Byun, [Sungmin Cha](https://sites.google.com/view/sungmin-cha/), [Taesup Moon](https://mindlab-snu.github.io/) <Br>
**[[Pytorch-Code](https://github.com/csm9493/FBI-Denoiser)]**  <Br>
	
##### Invertible Image Denoising
**[Paper]** (CVPR 2021) Invertible Denoising Network: A Light Solution for Real Noise Removal <Br>
**[Author]** Yang Liu, Zhenyue Qin, [Saeed Anwar](https://saeed-anwar.github.io/), [Pan Ji](https://sites.google.com/view/panji530), [Dongwoo Kim](http://dongwookim-ml.github.io/), [Sabrina Caldwell](https://thephotographicalist.wordpress.com/), [Tom Gedeon](http://users.cecs.anu.edu.au/~Tom.Gedeon/) <Br>
**[[Pytorch-Code](https://github.com/Yang-Liu1082/InvDN)]**  <Br>

##### deepfnf ★
**[Paper]** (CVPR 2021) Deep Denoising of Flash and No-Flash Pairs for Photography in Low-Light Environments <Br>
**[Author]** [Zhihao Xia](https://www.cse.wustl.edu/~zhihao.xia/), Michaël Gharbi, [Federico Perazzi](https://fperazzi.github.io/), [Kalyan Sunkavalli](https://www.kalyans.org/), [Ayan Chakrabarti](https://projects.ayanc.org/) <Br>
**[[TF-Code](https://www.cse.wustl.edu/~zhihao.xia/deepfnf/)]**  <Br>
基于"Basis Prediction Networks for Effective Burst Denoising with Large Kernels"设计网络, 另外有一个scale map, 用于从flash image中得到高频细节, 乘到滤波后的non flash图像中.

##### NBNet ★
**[Paper]** (CVPR 2021) NBNet: Noise Basis Learning for Image Denoising with Subspace Projection <Br>
**[Author]** Shen Cheng, [Yuzhi Wang](https://bigeagle.me/about/), [Haibin Huang](https://brotherhuang.github.io/), Donghao Liu, Haoqiang Fan, [Shuaicheng Liu](http://www.liushuaicheng.org/) <Br>
**[[Code](https://github.com/megvii-research/NBNet)]**  <Br>
UNet结构, 利用decoder产生的高层特征预测basis及投影矩阵, 用于将低层特征投影已达到降噪目的.

##### Neighbor2Neighbor
**[Paper]** (CVPR 2021) Neighbor2Neighbor: Self-Supervised Denoising from Single Noisy Images <Br>
**[Author]** [Tao Huang](https://taohuang2018.github.io/), Songjiang Li, [Xu Jia](https://stephenjia.github.io/), [Huchuan Lu](http://ice.dlut.edu.cn/lu/index.html), Jianzhuang Liu<Br>
**[[Pytorch-Code](https://github.com/TaoHuang2018/Neighbor2Neighbor)]**  <Br>

##### BJDD
**[Paper]** (CVPRW 2021) Beyond Joint Demosaicking and Denoising  <Br>
**[Author]** [SMA Sharif](https://smasharif.info/), Rizwan Ali Naqvi, Mithun Biswas) <Br>
**[[Pytorch-Code](https://github.com/sharif-apu/BJDD_CVPR21)]**  <Br>

##### CycleISP ★
**[Paper]** (CVPR 2020 Oral) CycleISP: Real Image Restoration via Improved Data Synthesis <Br>
**[Author]** [Syed Waqas Zamir](https://scholar.google.es/citations?user=WNGPkVQAAAAJ&hl=en), [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Munawar Hayat](https://scholar.google.com/citations?user=Mx8MbWYAAAAJ&hl=en), [Fahad Shahbaz Khan](https://scholar.google.es/citations?user=zvaeYnUAAAAJ&hl=en), [Ming-Hsuan Yang](https://scholar.google.com/citations?user=p9-ohHsAAAAJ&hl=en), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en)<Br>
**[[Pytorch-Code](https://github.com/swz30/CycleISP)]**  <Br>
提出了一个从sRGB到RAW相互转换的网络, 在Raw图像上注入高斯噪声用于生成RGB噪声样本.

##### Self2Self
**[Paper]** (CVPR 2020) Self2Self With Dropout: Learning Self-Supervised Denoising From Single Image <Br>
**[Author]** [Yuhui Quan](https://csyhquan.github.io/), Mingqin Chen, Tongyao Pang, Hui Ji<Br>
**[[TF-Code](https://github.com/scut-mingqinchen/self2self)]**  <Br>

##### AINDNet
**[Paper]** (CVPR 2020) Transfer Learning from Synthetic to Real-Noise Denoising with Adaptive Instance Normalization  <Br>
**[Author]** Yoonsik Kim, Jae Woong Soh, Gu Yong Park, Nam Ik Cho<Br>
**[[TF-Code](https://github.com/scut-mingqinchen/self2self)]**  <Br>

##### *Memory-Efficient Hierarchical Neural Architecture Search for Image Denoising*
**[Paper]** (CVPR 2020) Memory-Efficient Hierarchical Neural Architecture Search for Image Denoising <Br>
**[Author]** Haokui Zhang, Ying Li, Hao Chen, [Chunhua Shen](https://cshen.github.io/)<Br>

##### DBSN
**[Paper]** (ECCV 2020) Unpaired Learning of Deep Image Denoising <Br>
**[Author]** Xiaohe Wu, Ming Liu, Yue Cao, [Dongwei Ren](https://csdwren.github.io/), [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo) <Br>
**[[Pytorch-Code](https://github.com/XHWXD/DBSN/)]**  <Br>
	
##### *Reconstructing the Noise Variance Manifold for Image Denoising*
**[Paper]** (ECCV 2020) Reconstructing the Noise Variance Manifold for Image Denoising <Br>
**[Author]** Ioannis Marras, Grigorios G. Chrysos, Ioannis Alexiou, [Gregory Slabaugh](http://www.gregslabaugh.net/), [Stefanos Zafeiriou](https://wp.doc.ic.ac.uk/szafeiri/) <Br>
**[[Pytorch-Code](https://github.com/XHWXD/DBSN/)]**  <Br>

##### *Burst Denoising via Temporally Shifted Wavelet Transforms*
**[Paper]** (ECCV 2020) Burst Denoising via Temporally Shifted Wavelet Transforms <Br>
**[Author]** Xuejian Rong, Denis Demandolx, Kevin Matzen, Priyam Chatterjee, Yingli Tian<Br>
**[[Pytorch-Code](https://github.com/XHWXD/DBSN/)]**  <Br>
	
##### SFM
**[Paper]** (ECCV 2020) Burst Denoising via Temporally Shifted Wavelet Transforms <Br>
**[Author]** [Majed El Helou](https://majedelhelou.github.io/), Ruofan Zhou, Sabine Süsstrunk <Br>
**[[Pytorch-Code](https://github.com/majedelhelou/SFM)]**  <Br>

##### GPDNet
**[Paper]** (ECCV 2020) BLearning Graph-Convolutional Representations for Point Cloud Denoising <Br>
**[Author]** Francesca Pistilli, Giulia Fracastoro, [Diego Valsesia](https://ipl.polito.it/people/valsesia/, [Enrico Magli](https://ipl.polito.it/people/enrico-magli/) <Br>
**[[TF-Code](https://github.com/diegovalsesia/GPDNet)]**  <Br>

##### *Spatial Hierarchy Aware Residual Pyramid Network for Time-of-Flight Depth Denoising*
**[Paper]** (ECCV 2020) Spatial Hierarchy Aware Residual Pyramid Network for Time-of-Flight Depth Denoising <Br>
**[Author]** Guanting Dong, Yueyi Zhang, [Zhiwei Xiong](http://staff.ustc.edu.cn/~zwxiong/) <Br>
**[[TF-Code](https://github.com/ashesknight/tof-mpi-remove)]**  <Br>
	
##### *A Decoupled Learning Scheme for Real-world Burst Denoising from Raw Images*
**[Paper]** (ECCV 2020) A Decoupled Learning Scheme for Real-world Burst Denoising from Raw Images <Br>
**[Author]** Zhetong Liang, Shi Guo, Hong Gu, Huaqi Zhang, [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/) <Br>

##### *Robust and On-the-fly Dataset Denoising for Image Classification*
**[Paper]** (ECCV 2020) Robust and On-the-fly Dataset Denoising for Image Classification <Br>
**[Author]** [Jiaming Song](http://tsong.me/), [Lunjia Hu](https://sites.google.com/stanford.edu/lunjia), Michael Auli, [Yann Dauphin](https://www.dauphin.io/), [Tengyu Ma](http://ai.stanford.edu/~tengyuma/) <Br>

##### SADNet
**[Paper]** (ECCV 2020) Spatial-Adaptive Network for Single Image Denoising <Br>
**[Author]** Meng Chang, Qi Li, Huajun Feng, Zhihai Xu <Br>
**[[Pytorch-Code](https://github.com/JimmyChame/SADNet)]**  <Br>
	
##### Noise2Same
**[Paper]** (NIPS 2020) Noise2Same: Optimizing A Self-Supervised Bound for Image Denoising <Br>
**[Author]** Yaochen Xie, [Zhengyang Wang](https://zhengyang-wang.github.io/), [Shuiwang Ji](http://people.tamu.edu/~sji/) <Br>
**[[TF-Code](https://github.com/divelab/Noise2Same)]**  <Br>	

##### Patch2Self
**[Paper]** (NIPS 2020) Patch2Self: Denoising Diffusion MRI with Self-Supervised Learning <Br>
**[Author]**  Shreyas Fadnavis, Joshua Batson, Eleftherios Garyfallidis  <Br>
**[[Code](https://github.com/ShreyasFadnavis/patch2self)]**  <Br>
	
##### RIDNet ★☆
**[Paper]** (ICCV 2019 Oral) Real image denoising with feature attention<Br>
**[Author]** [Saeed Anwar](https://saeed-anwar.github.io/), Nick Barnes<Br>
**[[Code](https://github.com/cszn/IRCNN)]**  <Br>
1) 提出了一个端到端的去噪网络, 基于channel attention和skip connection. 在真是图像上测试效果不错, 速度一般. <Br>
2) 作为一篇Oral来说感觉创新点和理论论述都一般, 也没有解释为什么提出的网络对真是图像去噪效果好. <Br>
3) 如果需要, 参考网络流程图和代码即可. <Br>
	
##### Unprocessing Images for Learned Raw Denoising ★☆
**[Paper]** (CVPR 2019) Unprocessing Images for Learned Raw Denoising<Br>
**[Author]** [Tim Brooks](https://www.timothybrooks.com/tech/), [Ben Mildenhall](https://people.eecs.berkeley.edu/~bmild/), [Tianfan Xue](http://people.csail.mit.edu/tfxue/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/), [Dillon Sharlet](http://dsharlet.com/), [Jonathan T. Barron](https://jonbarron.info/)<Br>
**[[Code](https://www.timothybrooks.com/tech/unprocessing/)]**  <Br>
1) 提出了一个通过unprocess ISP流程而生成更真实去噪样本的框架, 可以用任意图像生成真实的训练样本, 以提高模型性能. <Br>
2) 对于sRGB图像, 根据ISP流程, 将其逐步逆运算位raw image, 在此基础上加的噪声更符合真实噪声.<Br>
3) 推断时, 要先把sRGB转换为raw image, 再经过网络处理, 最后再进行正向的ISP恢复为sRGB. <Br>
4) ISP流程的推断对每个品牌型号的相机都有所不同, 模拟其过程感觉还是有难度的. <Br>
	
##### CBDNet ★☆
**[Paper]** (CVPR 2019) Toward Convolutional Blind Denoising of Real Photographs<Br>
**[Author]** Shi Guo, Zifei Yan, Kai Zhang, Wangmeng Zuo, Lei Zhang, [Jonathan T. Barron](https://jonbarron.info/)<Br>
**[[Code](https://github.com/GuoShi28/CBDNet)]**  <Br>
1) 大致浏览. 采用一个FCN估计噪声level, 噪声level map与输入concat然后输入一类似U-Net的网络去噪. <Br>
2) 可以学习其网络和训练细节. <Br>

##### FC-AIDE
**[Paper]** (CVPR 2019) FC-AIDE: Fully Convolutional Adaptive Image Denoiser<Br>
**[Author]** [Sungmin cha](https://sites.google.com/view/sungmin-cha/), [Taesup Moon](https://mindlab-skku.github.io/)<Br>
**[[TF-Code](https://github.com/csm9493/FC-AIDE-Keras)]**  <Br>

##### FOCNet
**[Paper]** (CVPR 2019) FOCNet: A Fractional Optimal Control Network for Image Denoising<Br>
**[Author]** Xixi Jia, Sanyang Liu, Xiangchu Feng, [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
**[[Matlab-Code](https://github.com/hsijiaxidian/FOCNet)]**  <Br>

##### VDNet
**[Paper]** (NeurIPS 2019) Variational Denoising Network: Toward Blind Noise Modeling and Removal<Br>
**[Author]** Zongsheng Yue, [Hongwei Yong](https://sites.google.com/view/yonghongwei-homepage/%E9%A6%96%E9%A1%B5), Qian Zhao, [Deyu Meng](http://gr.xjtu.edu.cn/web/dymeng), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
**[[Pytorch-Code](https://github.com/zsyOAOA/VDNet)]**  <Br>
	
##### *selfsupervised-denoising*
**[Paper]** (NeurIPS 2019) High-Quality Self-Supervised Deep Image Denoising <Br>
**[Author]** [Samuli Laine](https://users.aalto.fi/~laines9/), [Tero Karras](https://research.nvidia.com/person/tero-karras), [Jaakko Lehtinen](https://users.aalto.fi/~lehtinj7/), [Timo Aila](https://users.aalto.fi/~ailat1/)<Br>
**[[TF-Code](https://github.com/NVlabs/selfsupervised-denoising)]**  <Br>

##### IRCNN ★
**[Paper]** (CVPR 2017) Learning Deep CNN Denoiser Prior for Image Restoration<Br>
**[Author]** [Kai Zhang](https://github.com/cszn), [Wangmeng Zuo](https://github.com/cszn), [Shuhang Gu](https://sites.google.com/site/shuhanggu/), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
**[[Matlab-Code](https://github.com/cszn/IRCNN)]**  <Br>
大致浏览, 提出了一个结构简单的CNN去噪器, 可以为基于模型的优化方法提供有效的prior, 还可以用于求解其它图像恢复的逆问题
	


	
# Raw Denoising
##### ELD ★★
**[Paper]** (CVPR 2020 Oral) A Physics-based Noise Formation Model for Extreme Low-light Raw Denoising<Br>
**[Author]** [Kaixuan Wei](https://kxwei.net/), [Ying Fu](https://ying-fu.github.io/), [Jiaolong Yang](http://jlyang.org/), Hua Huang<Br>
**[[Pytorch-Code & Dataset](https://github.com/Vandermode/ELD)]**  <Br>
较为全面的分析了相机噪声来源, 并据此提出了一个高度模拟真实的噪声生成模型. 有趣的论文, 目前没有做基于Raw的处理, 故没有深入研究.

##### BPN
**[Paper]** (CVPR 2020) Basis Prediction Networks for Effective Burst Denoising with Large Kernels <Br>
**[Author]** [Zhihao Xia](https://www.cse.wustl.edu/~zhihao.xia/), [Federico Perazzi](https://fperazzi.github.io/), [Michael Gharbi](https://www.mgharbi.com/), Kalyan Sunkavalli, [Ayan Chakrabarti](https://projects.ayanc.org/) <Br>
**[[Project](https://www.cse.wustl.edu/~zhihao.xia/bpn/)]**  <Br>	
##### *Practical Deep Raw Image Denoising on Mobile Devices*
**[Paper]** (ECCV 2020 Spotlight) Practical Deep Raw Image Denoising on Mobile Devices <Br>
**[Author]** Yuzhi Wang, [Haibin Huang](https://brotherhuang.github.io/), Qin Xu, Jiaming Liu, Yiqun Liu, [Jue Wang](https://www.juew.org/)<Br>
	
## Burst Denoising
##### *Burst Denoising with Kernel Prediction Networks*
**[Paper]** (CVPR 2018 Oral) Burst Denoising with Kernel Prediction Networks <Br>
**[Author]** [Ben Mildenhall](https://bmild.github.io/), [Jonathan T. Barron](https://jonbarron.info/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/), Dillon Sharlet, [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html), Robert Carroll <Br>
**[[Project](https://bmild.github.io/kpn/index.html)]**  **[[TF-Code](https://github.com/google/burst-denoising)]** **[[Unofficial-Pytorch-Code](https://github.com/z-bingo/kernel-prediction-networks-PyTorch)]** <Br>


	
	
	
# Datasets
## Real Image Denoising
[DnD](https://noise.visinf.tu-darmstadt.de/) <Br>
[SIDD](https://www.eecs.yorku.ca/~kamel/sidd/) <Br>

[PolyU](https://github.com/csjunxu/PolyU-Real-World-Noisy-Images-Dataset) <Br>
[Renoir](http://ani.stat.fsu.edu/~abarbu/Renoir.html) <Br>
[CC](http://snam.ml/research/ccnoise) <Br>
[SID](http://cchen156.web.engr.illinois.edu/SID.html) <Br>
[kodak_color](http://r0k.us/graphics/kodak/) <Br>
[NoiseClinicImages](http://demo.ipol.im/demo/125/input_select?044_solvay_1927.x=63&044_solvay_1927.y=68) <Br>


# Resources
[[去噪论文整理](https://paperswithcode.com/task/image-denoising?page=2)]  <Br>

[[去噪论文with codes](https://github.com/wenbihan/reproducible-image-denoising-state-of-the-art)]  <Br>
