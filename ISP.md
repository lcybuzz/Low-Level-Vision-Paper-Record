# Table of Contents
- [ISP](#isp)
- [AWB](#awb)
- [Misc](#misc)


## ISP
- **Transform your Smartphone into a DSLR Camera: Learning the ISP in the Wild** <Br>
Ardhendu Shekhar Tripathi, [Martin Danelljan](https://martin-danelljan.github.io/), Samarth Shukla, [Radu Timofte](http://people.ee.ethz.ch/~timofter/), [Luc Van Gool](https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html) <Br>
[ECCV 2022] [[Code](https://github.com/4rdhendu/TransformPhone2DSLR)] <Br>

- **RAWtoBit: A Fully End-to-end Camera ISP Network** <Br>
Wooseok Jeong, [Seung-Won Jung](https://sites.google.com/view/deepiplab/) <Br>
[ECCV 2022] <Br>

- **Day-to-Night Image Synthesis for Training Nighttime Neural ISPs** <Br>
[Abhijith Punnappurath](https://abhijithpunnappurath.github.io/), [Abdullah Abuolaim](https://sites.google.com/view/abdullah-abuolaim/), [Abdelrahman Abdelhamed](https://abdokamel.github.io/), Alex Levinshtein, [Michael S. Brown](https://www.eecs.yorku.ca/~mbrown/) <Br>
[CVPR 2022 Oral] [[Pytorch-Code](https://github.com/SamsungLabs/day-to-night)] <Br>

- **Abandoning the Bayer-Filter to See in the Dark** <Br>
[Xingbo Dong](https://xingbod.github.io/), Wanyan Xu, Zhihui Miao, Lan Ma, Chao Zhang, Jiewen Yang, [Zhe Jin](https://sites.google.com/site/jinzhe/home?authuser=0), [Andrew Beng Jin Teoh](https://sites.google.com/site/multimediasecuritylab/Home), Jiajun Shen <Br>
[CVPR 2022] [[Pytorch-Code](https://github.com/TCL-AILab/Abandon_Bayer-Filter_See_in_the_Dark)] <Br>
[★] 从bayer raw预测一个mono. 采集了一个bayer和mono配对的数据集.

- **Model-Based Image Signal Processors via Learnable Dictionaries** <Br>
[Marcos V. Conde](https://mv-lab.github.io/), [Steven McDonagh](https://smcdonagh.github.io/), Matteo Maggioni, [Aleš Leonardis](https://www.cs.bham.ac.uk/~leonarda/), [Eduardo Pérez-Pellitero](http://perezpellitero.github.io/) <Br>
[AAAI 2022 Oral] [[Project](https://mv-lab.github.io/model-isp22/)] <Br>
[**Model ISP**] [★★] 对ISP过程做了较详细的拆分, 每一步尽量做到可逆, end-to-end训练和推理

- **Mobile Computational Photography: A Tour** <Br>
[Mauricio Delbracio](https://mdelbra.github.io/), Damien Kelly, [Michael S. Brown](https://www.eecs.yorku.ca/~mbrown/), [Peyman Milanfar](https://sites.google.com/view/milanfarhome/) <Br>
[arXiv 2102] <Br>
[★★★] 很好的一篇ISP综述

- **Learning RAW-to-sRGB Mappings with Inaccurately Aligned Supervision** <Br>
Zhilu Zhang, Haolin Wang, Ming Liu, Ruohao Wang, [Jiawei Zhang](https://sites.google.com/site/zhjw1988), [Wangmeng Zuo](http://homepage.hit.edu.cn/wangmengzuo) <Br>
[ICCV 2021] [[Project](https://github.com/cszhilu1998/RAW-to-sRGB)] <Br>
  
- **ReconfigISP: Reconfigurable Camera Image Processing Pipeline** <Br>
Ke Yu, Zexian Li, Yue Peng, [Chen Change Loy](https://www.mmlab-ntu.com/person/ccloy/), [Jinwei Gu](http://www.gujinwei.org/) <Br>
[ICCV 2021] [[Project](https://www.mmlab-ntu.com/project/reconfigisp/)] <Br>

- **End-to-end High Dynamic Range Camera Pipeline Optimization** <Br>
[Yazhou Xing](https://yzxing87.github.io/), Zian Qian, [Qifeng Chen](https://cqf.io/) <Br>
[CVPR 2021] [[Project](https://yzxing87.github.io/InvISP/index.html)] [[Pytorch-Code](https://github.com/yzxing87/Invertible-ISP)] <Br>
[★] 将ISP参数与下游任务一同优化

- **Invertible Image Signal Processing** <Br>
Nicolas Robidoux, Luis E. Garcia Capel, Dong-eun Seo, Avinash Sharma, Federico Ariza, Felix Heide <Br>
[CVPR 2021] [[Project](https://light.princeton.edu/publication/hdr_isp_opt/)] <Br>
  
- **Neural Camera Simulators** <Br>
Hao Ouyang, Zifan Shi, [Chenyang Lei](https://chenyanglei.github.io/), Ka Lung Law, [Qifeng Chen](https://cqf.io/) <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/ken-ouyang/neural_image_simulator)]<Br>
[★] 提出了一个controllable raw图像生成流程, 通过控制曝光时间, ISO, 噪声level和aperture, 控制生成图像的亮度, blur, 噪声等属性
  
- **Learning sRGB-to-Raw-RGB De-rendering with Content-Aware Metadata** <Br>
[Seonghyeon Nam](http://snam.ml/), [Abhijith Punnappurath](https://abhijithpunnappurath.github.io/), [Marcus A. Brubaker](https://mbrubake.github.io/), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
[CVPR 2021] <Br>
**SRGB->RAW**
  
- **CycleISP: Real Image Restoration via Improved Data Synthesis** <Br>
[Syed Waqas Zamir](https://scholar.google.es/citations?user=WNGPkVQAAAAJ&hl=en), [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Munawar Hayat](https://scholar.google.com/citations?user=Mx8MbWYAAAAJ&hl=en), [Fahad Shahbaz Khan](https://scholar.google.es/citations?user=zvaeYnUAAAAJ&hl=en), [Ming-Hsuan Yang](https://scholar.google.com/citations?user=p9-ohHsAAAAJ&hl=en), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en)<Br>
[CVPR 2020 Oral] [[Pytorch-Code](https://github.com/swz30/CycleISP)]  <Br>
[★] 提出了一个从sRGB到RAW相互转换的网络, 在Raw图像上注入高斯噪声用于生成RGB噪声样本.
  
- **Replacing Mobile Camera ISP with a Single Deep Learning Model** <Br>
Andrey Ignatov, Luc Van Gool, Radu Timofte  <Br>
[CVPR 2020] [[Code](https://github.com/aiff22/pynet)] <Br>
[**PyNet**] [★] 1) 提出了一个端到端的深度学习网络, 用以代替现有的ISP处理流程. 2) 提出了一个华为P20 RAW 和Canon 5D的RAW-RGB图像对, 用以训练ISP模型. 3) 提出的算法与自带的ISP流程相比, 色彩上有一定提升, 但没有明显优势, 且存在晕影. 另外速度也是个问题. 因此对于用一个DL模型代替ISP流程的方案可行性还是有待确认. <Br>

- **Rethinking Learning-based Demosaicing, Denoising, and Super-Resolution Pipeline**  <Br>
[Guocheng Qian](https://www.gcqian.com/), [Jinjin Gu](http://www.jasongt.com/), [Jimmy Ren](http://www.jimmyren.com/), [Chao Dong](http://xpixel.group/2010/01/20/chaodong.html), Furong Zhao, Juan Lin <Br>
[ICCP 2022] [[Pytorch-Code](https://github.com/guochengqian/TENet)] <Br>
[**TENet**] [★] 1. 使用具有pixel shift技术的相机收集了一可以做demoasic的数据集, 避免了用普通RGB数据做真值时内置demoasic过程带来的误差. 2. 提出了一端到端的demosaic, 去噪和超分的网络, 采用residual + dense block的形式, 没什么特别的

- **End-to-End Learning for Joint Image Demosaicing, Denoising and Super-Resolution**  <Br>
Wenzhu Xing, [Karen Egiazarian](https://www.tuni.fi/en/karen-eguiazarian) <Br>
[CVPR 2021] [[Pytorch-Code](https://github.com/xingwz/End-to-End-JDNDMSR)] <Br>
[★] 一个网络联合做demosaic, 去噪和超分, 退化很简单, 没在真实数据上实验.

- **Generating Training Data for Denoising Real RGB Images via Camera Pipeline Simulation**  <Br>
[Ronnachai Jaroensri](http://people.csail.mit.edu/tiam/), Camille Biscarrat, [Miika Aittala](https://people.csail.mit.edu/miika/), [Frédo Durand](https://people.csail.mit.edu/fredo/) <Br>
[arXiv 1904] [[Project](http://people.csail.mit.edu/tiam/camera_sim/)] [[Pytorch-Code](https://github.com/12dmodel/camera_sim)] <Br>
[★★] 提出了一个模拟isp流程, 使用多种demoasic, denoise, tone mapping算法, 从raw生成rgb, 用于去噪. 可以学习它的pipeline和算法.

- **DeepISP: Learning End-to-End Image Processing Pipeline** <Br>
[Eli Schwartz](https://elischwartz.github.io/publications/), [Raja Giryes](http://web.eng.tau.ac.il/~raja/), [Alex M. Bronstein](https://bron.cs.technion.ac.il/) <Br>
[TIP 2018] <Br>
[☆] 大致浏览, 一个end-to-end的网络, 分为保持分辨率的low level部分和逐层下采样的high level部分. 使用了conv+relu, conv+tanh, 直连三个分支并行的设计, 比较少见

- **Learning to See in the Dark** <Br>
[Chen Chen](http://cchen156.web.engr.illinois.edu/), [Qifeng Chen](https://cqf.io/), [Jia Xu](http://pages.cs.wisc.edu/~jiaxu/), [Vladlen Koltun](http://vladlen.info/)  <Br>
[CVPR 2018] [[Project](http://cchen156.web.engr.illinois.edu/SID.html)] [[TF-Code](https://github.com/cchen156/Learning-to-See-in-the-Dark)] <Br>
[★★] 1) 提出了SID数据集, 包括RGB和Raw数据. 2) 提出了一个end-to-end的isp网络, 以RAW和增益信息为输入, 输入RGB图像, 代替传统ISP流程

- **Reconfiguring the Imaging Pipeline for Computer Vision** <Br>
[Mark Buckler](http://www.markbuckler.com/), [Suren Jayasuriya](http://www.andrew.cmu.edu/user/sjayasur/website.html), [Adrian Sampson](http://www.cs.cornell.edu/~asampson/)  <Br>
[ICCV 2017] [[Project](https://capra.cs.cornell.edu/research/visionmode/)] [[Code1](https://github.com/cucapra/approx-vision)] [[Code2](https://github.com/mbuckler/ReversiblePipeline)] <Br>
[★★] 1) 针对计算机视觉任务(而不是photography)简化ISP流程. 提出只有demosaicing和gamma校正是CV任务中必需的, 并据此设计了系统. 2) 系统包括3个步骤: reduced resolution readout, subsampling to produce RGB images, lower-precision logarithmic ADC configuration. 能将总体能耗降低约75% 3) 公布了一套用于模拟imaging pipeline及其逆过程的工具CRIP

- **Learning the image processing pipeline** <Br>
Haomiao Jiang, Qiyuan Tian, [Joyce Farrell](https://web.stanford.edu/group/scien/cgi-bin/farrell/), [Brian Wandell](https://web.stanford.edu/group/vista/cgi-bin/wandell/)  <Br>
[TIP 2017] <Br>
[**L3**] [★] 将RAW到sRGB的转换用局部相信滤波器完成, 类似于RAISR.
  
- **A Software Platform for Manipulating the Camera Imaging Pipeline**  <Br>
[Hakki Can Karaimer](https://karaimer.github.io/), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
[CVPR 2016] [[Project](https://karaimer.github.io/camera-pipeline/)]  <Br> 
  
 
  

# AWB
- **Cross-Camera Convolutional Color Constancy** <Br>
[Mahmoud Afifi](https://sites.google.com/corp/view/mafifi), [Jonathan T. Barron](https://jonbarron.info/), [Chloe LeGendre](http://www.chloelegendre.com/), [Yun-Ta Tsai](https://research.google/people/105312/), [Francois Bleibel](https://www.linkedin.com/in/fbleibel/)  <Br>
[ICCV 2021] [[Pytorch-Code](https://github.com/mahmoudnafifi/C5)] <Br>
[**C5**]

- **A Multi-Hypothesis Approach to Color Constancy for improved Automatic White Balance** <Br>
[Daniel Hernandez-Juarez](https://danihernandez.eu/), [Sarah Parisot](https://parisots.github.io/), [Benjamin Busam](http://campar.in.tum.de/Main/BenjaminBusam), Ales Leonardis, [Gregory Slabaugh](http://www.gregslabaugh.net/), Steven McDonagh <Br>
[CVPR 2020] [[Project](http://cvil.eecs.yorku.ca/projects/public_html/sRGB_WB_correction/index.html)] <Br>
[★☆] 粗读, 用贝叶斯思想处理AWB问题. 首先用K-Means选取n个candidates, 再用一个小型CNN预测似然概率(即当前图像是来自于该光照的可能性), 最后的预测光照结果为n个似然概率取softmax后的加权求和.
  
- **Deep White-Balance Editing** <Br>
[Mahmoud Afifi](https://sites.google.com/view/mafifi/home), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/)<Br>
[CVPR 2020 Oral] [[Pytorch & Matlab-Code](https://github.com/mahmoudnafifi/Deep_White_Balance)] <Br>
[★☆] 1) 1个encoder, 3个decoder, 分别预测正确, 白炽灯, 室外场景的白平衡结果. 最后可根据三个结果插值出用户需要的色温. 2) 为在device上进行快速推理, 在小图上预测, 然后在小图上通过优化的方法闭式求解输入输出的全局色彩映射函数, 再将该函数用到全图上

- **Sensor-Independent illumination estimation for DNN Models** <Br>
[Mahmoud Afifi](https://sites.google.com/view/mafifi/home), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
[arXiv 1912] [[Matlab-Code](https://github.com/mahmoudnafifi/SIIE)] <Br>
[**SIIE**] [★☆]

- **When Color Constancy Goes Wrong: Correcting Improperly White-Balanced Images** <Br>
[Mahmoud Afifi](https://sites.google.com/view/mafifi/home), [Brian Price](https://www.brianpricephd.com/), [Scott Cohen](https://research.adobe.com/person/scott-cohen/), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
[CVPR 2019] [[Project](http://cvil.eecs.yorku.ca/projects/public_html/sRGB_WB_correction/index.html)] [[Code](https://github.com/mahmoudnafifi/WB_sRGB)] [[Blog](http://www.noahlab.com.hk/#/news/5ee70c18a0c07a1a3855452d)] <Br>
  
- **Improving Color Reproduction Accuracy on Cameras** <Br>
[Hakki Can Karaimer](https://karaimer.github.io/), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
[CVPR 2018] [[Project](https://karaimer.github.io/camera-color/)] <Br> 

- **Convolutional color constancy** <Br>
[Jonathan T. Barron](https://jonbarron.info/) <Br>
[ICCV 2015] <Br> 
[★★]




# Misc
- **Improving Color Reproduction Accuracy on Cameras** <Br>
[Thomas Eboli](https://teboli.github.io/), [Jean-Michel Morel](https://sites.google.com/site/jeanmichelmorelcmlaenscachan/), [Gabriele Facciolo](http://dev.ipol.im/~facciolo/) <Br>
[ECCV 2022] [[Project](https://teboli.github.io/fast_optical.html)] [[Pytorch-Code](https://github.com/teboli/fast_two_stage_psf_correction)] <Br> 

