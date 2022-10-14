
# Denoising
- [Image Denoising](#image-denoising)
- [Raw Denoising](#raw-denoising)
- [Video Denoising](#video-denoising)
- [Signal Processing Based](#signal-processing-based)



# Image Denoising

- **Fast and High-quality Image Denoising via Malleable Convolutions** <Br>
[Yifan Jiang](https://yifanjiang.net/), [Bartlomiej Wronski](https://bartwronski.com/), [Ben Mildenhall](https://bmild.github.io/), [Jonathan Barron](https://jonbarron.info/), Zhangyang Wang, [Tianfan Xue](https://people.csail.mit.edu/tfxue/) <Br>
[ECCV 2022] [[Project](https://yifanjiang.net/MalleConv.html)] <Br>

- **CVF-SID: Cyclic multi-Variate Function for Self-Supervised Image Denoising by Disentangling Noise from Image** <Br>
Reyhaneh Neshatavar, [Mohsen Yavartanoo](https://myavartanoo.github.io/), [Sanghyun Son](https://cv.snu.ac.kr/), [Kyoung Mu Lee](https://cv.snu.ac.kr/index.php/~kmlee/) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/Reyhanehne/CVF-SID_PyTorch)] <Br>

- **AP-BSN: Self-Supervised Denoising for Real-World Images via Asymmetric PD and Blind-Spot Network** <Br>
Wooseok Lee, [Sanghyun Son](https://cv.snu.ac.kr/), [Kyoung Mu Lee](https://cv.snu.ac.kr/index.php/~kmlee/) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/wooseoklee4/AP-BSN)] <Br>

- **Blind2Unblind: Self-Supervised Image Denoising with Visible Blind Spots** <Br>
Zejin Wang, Jiazheng Liu, Guoqing Li, Hua Han <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/demonsjin/Blind2Unblind)] <Br>

- **IDR: Self-Supervised Image Denoising via Iterative Data Refinement** <Br>
[Yi Zhang](https://zhangyi-3.github.io/), Dasong Li, Ka Lung Law, [Xiaogang Wang](http://www.ee.cuhk.edu.hk/~xgwang/), [Hongwei Qin](https://scholar.google.com/citations?user=ZGM7HfgAAAAJ&hl=en), [Hongsheng Li](https://www.ee.cuhk.edu.hk/~hsli/) <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/zhangyi-3/IDR)] <Br>

- **Practical Blind Denoising via Swin-Conv-UNet and Data Synthesis** <Br>
[Kai Zhang](https://cszn.github.io/), [Yawei Li](https://ofsoundof.github.io/), [Jingyun Liang](https://jingyunliang.github.io/), [Jiezhang Cao](https://www.jiezhangcao.com/), [Yulun Zhang](http://yulunzhang.com/), Hao Tang, [Radu Timofte](http://people.ee.ethz.ch/~timofter/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html) <Br>
[arXiv 2003] [[Pytorch-Code](https://github.com/cszn/SCUNet)] <Br>
[**SCUNet**]
	
- **FBI-Denoiser: Fast Blind Image Denoiser for Poisson-Gaussian Noise** <Br>
Jaeseok Byun, [Sungmin Cha](https://sites.google.com/view/sungmin-cha/), [Taesup Moon](https://mindlab-snu.github.io/) <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/csm9493/FBI-Denoiser)]  <Br>
	
- **Invertible Denoising Network: A Light Solution for Real Noise Removal** <Br>
Yang Liu, Zhenyue Qin, [Saeed Anwar](https://saeed-anwar.github.io/), [Pan Ji](https://sites.google.com/view/panji530), [Dongwoo Kim](http://dongwookim-ml.github.io/), [Sabrina Caldwell](https://thephotographicalist.wordpress.com/), [Tom Gedeon](http://users.cecs.anu.edu.au/~Tom.Gedeon/) <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/Yang-Liu1082/InvDN)]  <Br>

- **Deep Denoising of Flash and No-Flash Pairs for Photography in Low-Light Environments** <Br>
[Zhihao Xia](https://www.cse.wustl.edu/~zhihao.xia/), Michaël Gharbi, [Federico Perazzi](https://fperazzi.github.io/), [Kalyan Sunkavalli](https://www.kalyans.org/), [Ayan Chakrabarti](https://projects.ayanc.org/) <Br>
[CVPR 2021] [[TF-Code](https://www.cse.wustl.edu/~zhihao.xia/deepfnf/)]  <Br>
[**deepfnf**] [★] 基于"Basis Prediction Networks for Effective Burst Denoising with Large Kernels"设计网络, 另外有一个scale map, 用于从flash image中得到高频细节, 乘到滤波后的non flash图像中.

- **NBNet: Noise Basis Learning for Image Denoising with Subspace Projection** <Br>
Shen Cheng, [Yuzhi Wang](https://bigeagle.me/about/), [Haibin Huang](https://brotherhuang.github.io/), Donghao Liu, Haoqiang Fan, [Shuaicheng Liu](http://www.liushuaicheng.org/) <Br>
[CVPR 2021] [[Code](https://github.com/megvii-research/NBNet)]  <Br>
[★] UNet结构, 利用decoder产生的高层特征预测basis及投影矩阵, 用于将低层特征投影已达到降噪目的.

- **Neighbor2Neighbor: Self-Supervised Denoising from Single Noisy Images** <Br>
[Tao Huang](https://taohuang2018.github.io/), Songjiang Li, [Xu Jia](https://stephenjia.github.io/), [Huchuan Lu](http://ice.dlut.edu.cn/lu/index.html), Jianzhuang Liu<Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/TaoHuang2018/Neighbor2Neighbor)]  <Br>

- **Beyond Joint Demosaicking and Denoising**  <Br>
[SMA Sharif](https://smasharif.info/), Rizwan Ali Naqvi, Mithun Biswas) <Br>
[CVPRW 2021] [[Pytorch-Code](https://github.com/sharif-apu/BJDD_CVPR21)]  <Br>
[**BJDD**]

- **CycleISP: Real Image Restoration via Improved Data Synthesis** <Br>
[Syed Waqas Zamir](https://scholar.google.es/citations?user=WNGPkVQAAAAJ&hl=en), [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Munawar Hayat](https://scholar.google.com/citations?user=Mx8MbWYAAAAJ&hl=en), [Fahad Shahbaz Khan](https://scholar.google.es/citations?user=zvaeYnUAAAAJ&hl=en), [Ming-Hsuan Yang](https://scholar.google.com/citations?user=p9-ohHsAAAAJ&hl=en), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en)<Br>
[CVPR 2021 Oral] [[Pytorch-Code](https://github.com/swz30/CycleISP)]  <Br>
[★] 提出了一个从sRGB到RAW相互转换的网络, 在Raw图像上注入高斯噪声用于生成RGB噪声样本.

- **Self2Self With Dropout: Learning Self-Supervised Denoising From Single Image**  <Br>
[Yuhui Quan](https://csyhquan.github.io/), Mingqin Chen, Tongyao Pang, Hui Ji<Br>
[CVPR 2021] [[TF-Code](https://github.com/scut-mingqinchen/self2self)] <Br>

- **Transfer Learning from Synthetic to Real-Noise Denoising with Adaptive Instance Normalization**  <Br>
Yoonsik Kim, Jae Woong Soh, Gu Yong Park, Nam Ik Cho<Br>
[CVPR 2020] [[TF-Code](https://github.com/scut-mingqinchen/self2self)]  <Br>
[**AINDNet**]

- **Memory-Efficient Hierarchical Neural Architecture Search for Image Denoising** <Br>
Haokui Zhang, Ying Li, Hao Chen, [Chunhua Shen](https://cshen.github.io/)<Br>
[CVPR 2020] <Br>

- **Unpaired Learning of Deep Image Denoising**  <Br>
Xiaohe Wu, Ming Liu, Yue Cao, [Dongwei Ren](https://csdwren.github.io/), [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo) <Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/XHWXD/DBSN/)] <Br>
[**DBSN**]

- **Reconstructing the Noise Variance Manifold for Image Denoising** <Br>
Ioannis Marras, Grigorios G. Chrysos, Ioannis Alexiou, [Gregory Slabaugh](http://www.gregslabaugh.net/), [Stefanos Zafeiriou](https://wp.doc.ic.ac.uk/szafeiri/) <Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/XHWXD/DBSN/)]  <Br>

- **Burst Denoising via Temporally Shifted Wavelet Transforms** <Br>
Xuejian Rong, Denis Demandolx, Kevin Matzen, Priyam Chatterjee, Yingli Tian<Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/XHWXD/DBSN/)]  <Br>
	
- **Burst Denoising via Temporally Shifted Wavelet Transforms**  <Br>
[Majed El Helou](https://majedelhelou.github.io/), Ruofan Zhou, Sabine Süsstrunk <Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/majedelhelou/SFM)] <Br>
[**SFM**]

- **BLearning Graph-Convolutional Representations for Point Cloud Denoising** <Br>
Francesca Pistilli, Giulia Fracastoro, [Diego Valsesia](https://ipl.polito.it/people/valsesia/, [Enrico Magli](https://ipl.polito.it/people/enrico-magli/) <Br>
[ECCV 2020] [[TF-Code](https://github.com/diegovalsesia/GPDNet)]  <Br>
[**GPDNet**]

- **Spatial Hierarchy Aware Residual Pyramid Network for Time-of-Flight Depth Denoising** <Br>
Guanting Dong, Yueyi Zhang, [Zhiwei Xiong](http://staff.ustc.edu.cn/~zwxiong/) <Br>
[ECCV 2020] [[TF-Code](https://github.com/ashesknight/tof-mpi-remove)]  <Br>
	
- **A Decoupled Learning Scheme for Real-world Burst Denoising from Raw Images** <Br>
Zhetong Liang, Shi Guo, Hong Gu, Huaqi Zhang, [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/) <Br>
[ECCV 2020] <Br>

- **Robust and On-the-fly Dataset Denoising for Image Classification** <Br>
[Jiaming Song](http://tsong.me/), [Lunjia Hu](https://sites.google.com/stanford.edu/lunjia), Michael Auli, [Yann Dauphin](https://www.dauphin.io/), [Tengyu Ma](http://ai.stanford.edu/~tengyuma/) <Br>
[ECCV 2020] <Br>
 
- **Spatial-Adaptive Network for Single Image Denoising** <Br>
Meng Chang, Qi Li, Huajun Feng, Zhihai Xu <Br>
[ECCV 2020] [[Pytorch-Code](https://github.com/JimmyChame/SADNet)]  <Br>
[**SADNet**]

- **Noise2Same: Optimizing A Self-Supervised Bound for Image Denoising** <Br>
Yaochen Xie, [Zhengyang Wang](https://zhengyang-wang.github.io/), [Shuiwang Ji](http://people.tamu.edu/~sji/) <Br>
[NIPS 2020] [[TF-Code](https://github.com/divelab/Noise2Same)]  <Br>	

- **Patch2Self: Denoising Diffusion MRI with Self-Supervised Learning** <Br>
Shreyas Fadnavis, Joshua Batson, Eleftherios Garyfallidis  <Br>
[NIPS 2020] [[Code](https://github.com/ShreyasFadnavis/patch2self)]  <Br>
	
- **Real image denoising with feature attention** <Br>
[Saeed Anwar](https://saeed-anwar.github.io/), Nick Barnes <Br>
[ICCV 2019 Oral] [[Code](https://github.com/cszn/IRCNN)]  <Br>
[**RIDNet**] [★☆] 1) 提出了一个端到端的去噪网络, 基于channel attention和skip connection. 在真是图像上测试效果不错, 速度一般. 2) 作为一篇Oral来说感觉创新点和理论论述都一般, 也没有解释为什么提出的网络对真是图像去噪效果好. 3) 如果需要, 参考网络流程图和代码即可. <Br>
	
- **Toward Convolutional Blind Denoising of Real Photographs** <Br>
Shi Guo, Zifei Yan, Kai Zhang, Wangmeng Zuo, Lei Zhang, [Jonathan T. Barron](https://jonbarron.info/)<Br>
[CVPR 2019] [[Code](https://github.com/GuoShi28/CBDNet)]  <Br>
[**CBDNet**] [★☆] 1) 大致浏览. 采用一个FCN估计噪声level, 噪声level map与输入concat然后输入一类似U-Net的网络去噪. 2) 可以学习其网络和训练细节. <Br>

- **FC-AIDE: Fully Convolutional Adaptive Image Denoiser** <Br>
[Sungmin cha](https://sites.google.com/view/sungmin-cha/), [Taesup Moon](https://mindlab-skku.github.io/)<Br>
[CVPR 2019] [[TF-Code](https://github.com/csm9493/FC-AIDE-Keras)]  <Br>

- **FOCNet: A Fractional Optimal Control Network for Image Denoising** <Br>
Xixi Jia, Sanyang Liu, Xiangchu Feng, [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
[CVPR 2019] [[Matlab-Code](https://github.com/hsijiaxidian/FOCNet)]  <Br>

- **Variational Denoising Network: Toward Blind Noise Modeling and Removal** <Br>
Zongsheng Yue, [Hongwei Yong](https://sites.google.com/view/yonghongwei-homepage/%E9%A6%96%E9%A1%B5), Qian Zhao, [Deyu Meng](http://gr.xjtu.edu.cn/web/dymeng), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
[NeurIPS 2019] [[Pytorch-Code](https://github.com/zsyOAOA/VDNet)]  <Br>
[**VDNet**]

- **High-Quality Self-Supervised Deep Image Denoising** <Br>
[Samuli Laine](https://users.aalto.fi/~laines9/), [Tero Karras](https://research.nvidia.com/person/tero-karras), [Jaakko Lehtinen](https://users.aalto.fi/~lehtinj7/), [Timo Aila](https://users.aalto.fi/~ailat1/)<Br>
[NeurIPS 2019] [[TF-Code](https://github.com/NVlabs/selfsupervised-denoising)]  <Br>

- **Learning Deep CNN Denoiser Prior for Image Restoration** <Br>
[Kai Zhang](https://github.com/cszn), [Wangmeng Zuo](https://github.com/cszn), [Shuhang Gu](https://sites.google.com/site/shuhanggu/), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
[CVPR 2017] [[Matlab-Code](https://github.com/cszn/IRCNN)]  <Br>
[**IRCNN**] [★] 大致浏览, 提出了一个结构简单的CNN去噪器, 可以为基于模型的优化方法提供有效的prior, 还可以用于求解其它图像恢复的逆问题
	


	
# Raw Denoising
- **Learnability Enhancement for Low-light Raw Denoising: Where Paired Real Data Meets Noise Modeling** <Br>
Hansen Feng, [Lizhi Wang](https://wang-lizhi.github.io/), Yuzhi Wang, Hua Huang <Br>
[MM 2022] [[Pytorch-Code](https://github.com/megvii-research/PMN)] <Br>
[**PMN**]

- **Efficient Burst Raw Denoising with Variance Stabilization and Multi-frequency Denoising Network** <Br>
[Dasong Li](https://dasongli1.github.io/), [Yi Zhang](https://zhangyi-3.github.io/), Ka Lung Law, [Xiaogang Wang](http://www.ee.cuhk.edu.hk/~xgwang/), [Hongwei Qin](http://qinhongwei.com/academic/), [Hongsheng Li](https://www.ee.cuhk.edu.hk/~hsli/) <Br>
[IJCV 2022]  <Br>
[★★] 1) 提出将输入进行变换, 从Poisson-Gaussian distribution变换到与gain和信号强度无关的固定方差高斯分布; 2) 提出了一个轻量级的上/下采样去噪网络, 序列化地处理N个输入帧, 使网络能在端侧运行; 3) 对齐部分使用block-matching和homography flow, 在4级金字塔上corase-to-fine进行; 4) 从实验结果上看, 提出的变换与直接concat噪声map和k-sigma方法相比, 指标稍高一点, 可视化结果细节保留更多.

- **A Physics-based Noise Formation Model for Extreme Low-light Raw Denoising** <Br>
[Kaixuan Wei](https://kxwei.net/), [Ying Fu](https://ying-fu.github.io/), [Jiaolong Yang](http://jlyang.org/), Hua Huang<Br>
[CVPR 2020 Oral] [[Pytorch-Code & Dataset](https://github.com/Vandermode/ELD)]  <Br>
[**ELD**] [★★] 较为全面的分析了相机噪声来源, 并据此提出了一个高度模拟真实的噪声生成模型.

- **Basis Prediction Networks for Effective Burst Denoising with Large Kernels** <Br>
[Zhihao Xia](https://www.cse.wustl.edu/~zhihao.xia/), [Federico Perazzi](https://fperazzi.github.io/), [Michael Gharbi](https://www.mgharbi.com/), Kalyan Sunkavalli, [Ayan Chakrabarti](https://projects.ayanc.org/) <Br>
[CVPR 2020] [[Project](https://www.cse.wustl.edu/~zhihao.xia/bpn/)]  <Br>	
[**BPN**]

- **Practical Deep Raw Image Denoising on Mobile Devices** <Br>
Yuzhi Wang, [Haibin Huang](https://brotherhuang.github.io/), Qin Xu, Jiaming Liu, Yiqun Liu, [Jue Wang](https://www.juew.org/)<Br>
[ECCV 2020 Spotlight] [[Pytorch-Code](https://github.com/MegEngine/PMRID)] <Br>
[**PMRID**] [★★] 分析了噪声来源, 提出用k-sigma变换消除iso对噪声水平的影响, 并提出了标定相机噪声参数的方法.

- **Unprocessing Images for Learned Raw Denoising** <Br>
[Tim Brooks](https://www.timothybrooks.com/tech/), [Ben Mildenhall](https://people.eecs.berkeley.edu/~bmild/), [Tianfan Xue](http://people.csail.mit.edu/tfxue/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/), [Dillon Sharlet](http://dsharlet.com/), [Jonathan T. Barron](https://jonbarron.info/)<Br>
[CVPR 2019] [[TF-Code](https://www.timothybrooks.com/tech/unprocessing/)]  <Br>
[★☆] 1) 提出了一个通过unprocess ISP流程而生成更真实去噪样本的框架, 可以用任意图像生成真实的训练样本, 以提高模型性能. 2) 对于sRGB图像, 根据ISP流程, 将其逐步逆运算位raw image, 在此基础上加的噪声更符合真实噪声. 3) 推断时, 要先把sRGB转换为raw image, 再经过网络处理, 最后再进行正向的ISP恢复为sRGB. <Br>

- **Burst Denoising with Kernel Prediction Networks** <Br>
[Ben Mildenhall](https://bmild.github.io/), [Jonathan T. Barron](https://jonbarron.info/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/), Dillon Sharlet, [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html), Robert Carroll <Br>
[CVPR 2018 Oral] [[Project](https://bmild.github.io/kpn/index.html)] [[TF-Code](https://github.com/google/burst-denoising)] [[Unofficial-Pytorch-Code](https://github.com/z-bingo/kernel-prediction-networks-PyTorch)] <Br>
[**KPN**] [★★] 1) 提出了一个从普通RGB通过逆ISP, 加噪等流程生成raw burst denoise数据对的流程 (KPN数据集); 2) 提出将输入与噪声map(标准差)一起输入网络, 改善了性能; 3) 提出了一个预测kernel的网络, 对每个位置预测若然个去噪核, 并集成得到去噪结果.



# Video Denoising
- **Dancing under the stars: video denoising in starlight** <Br>
[Kristina Monakhova](https://kristinamonakhova.com/), [Stephan R. Richter](http://www.stephanrichter.org/), [Laura Waller](https://laurawaller.com/), [Vladlen Koltun](http://vladlen.info/) <Br>
[CVPR 2022 Oral] [[Project](http://kristinamonakhova.com/starlight_denoising/)] [[Pytorch-Code](https://github.com/monakhova/starlight_denoising/)] <Br>
	
- **Patch Craft: Video Denoising by Deep Modeling and Patch Matching** <Br>
Gregory Vaksman, [Michael Elad](https://elad.cs.technion.ac.il/), [Peyman Milanfar](https://sites.google.com/view/milanfarhome/) <Br>
[ICCV 2021] [[Pytorch-Code](https://github.com/grishavak/PaCNet-denoiser)] <Br>
[**PaCNet**] [★] 大致浏览. 在前后帧提取相似patch作为网络输入, 后面加了一个时域滤波网络保证时间一致性, 可能速度会很慢?
	
- **Efficient Multi-Stage Video Denoising with Recurrent Spatio-Temporal Fusion** <Br>
Matteo Maggioni, Yibin Huang, Cheng Li, Shuai Xiao, Zhongqian Fu, Fenglong Song <Br>
[CVPR 2021] [[Unofficial-Pytorch-Code](https://github.com/Baymax-chen/EMVD)] <Br>	
[**EMVD**] [★★] 轻量级视频去噪, 效果与复杂模型效果相当. 首先用线性变换将raw图像在颜色-亮度和频率上分解; 第二步利用前一帧去噪结果与当前帧融合, 初步去噪; 第三步对初步去噪的图像再次进行去噪; 第四步将两次去噪的结果结合进行refine. 融合和refine是通过预测fusion map完成的.
	
- **FastDVDnet: A Very Fast Deep Video Denoising algorithm** <Br>
Matias Tassano, Julie Delon, Thomas Veit<Br>
[CVPR 2020] [[Pytorch-Code](https://delon.wp.imt.fr/)] <Br>	

- **Supervised Raw Video Denoising With a Benchmark Dataset on Dynamic Scenes** <Br>
 Huanjing Yue, Cong Cao, Lei Liao, Ronghe Chu, Jingyu Yang<Br>
[CVPR 2020] [[Pytorch-Code](https://github.com/cao-cong/RViDeNet)] <Br>	
[**RViDeNet**] [★★] 提出了CRVD dataset, 用于Raw去噪.



# Signal Processing Based

- **Practical Signal-Dependent Noise Parameter Estimation From a Single Noisy Image** <Br>
[Xinhao Liu](https://sites.google.com/site/liuxinhao0535/), Masayuki Tanaka, [Masatoshi Okutomi](http://www.ok.sc.e.titech.ac.jp/mem/mxo/okutomi.html) <Br>
[TIP 2014] <Br>
[★★] 将噪声模型建模为异方差高斯分布, 并通过小波和最小二乘求得噪声参数, 并分析了clipping对噪声建模的影响.

- **Practical Poissonian-Gaussian Noise Modeling and Fitting for Single-Image Raw-Data** <Br>
[Alessandro Foi](https://webpages.tuni.fi/foi/), Mejdi Trimeche, [Vladimir Katkovnik](https://webpages.tuni.fi/lasip/), [Karen Egiazarian](https://www.tuni.fi/en/karen-eguiazarian) <Br>
[TIP 2008] <Br>
[★★] 统计方差和均值, 从单张图像种拟合出噪声参数