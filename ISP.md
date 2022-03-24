# ISP
ISP及其内部模块相关论文

## ISP
### Model ISP ★★
**[Paper]**  (AAAI 2022 Oral) Model-Based Image Signal Processors via Learnable Dictionaries <Br>
**[Author]** [Marcos V. Conde](https://mv-lab.github.io/), [Steven McDonagh](https://smcdonagh.github.io/), Matteo Maggioni, [Aleš Leonardis](https://www.cs.bham.ac.uk/~leonarda/), [Eduardo Pérez-Pellitero](http://perezpellitero.github.io/) <Br>
**[[Project](https://mv-lab.github.io/model-isp22/)]** <Br>
 对ISP过程做了较详细的拆分, 每一步尽量做到可逆, end-to-end训练和推理
  
### Mobile Computational Photography: A Tour ★★★
**[Paper]**  (arXiv 2102) Mobile Computational Photography: A Tour <Br>
**[Author]** [Mauricio Delbracio](https://mdelbra.github.io/), Damien Kelly, [Michael S. Brown](https://mdelbra.github.io/), [Peyman Milanfar](https://sites.google.com/view/milanfarhome/) <Br>
很好的一篇ISP综述

### Invertible ISP
**[Paper]**  (CVPR 2021) Invertible Image Signal Processing <Br>
**[Author]** [Yazhou Xing](https://yzxing87.github.io/), Zian Qian, [Qifeng Chen](https://cqf.io/) <Br>
**[[Project](https://yzxing87.github.io/InvISP/index.html)]**, **[[Pytorch-Code](https://github.com/yzxing87/Invertible-ISP)]** <Br>
  
### Neural Camera Simulators ★
**[Paper]**  (CVPR 2021) Neural Camera Simulators <Br>
**[Author]** Hao Ouyang, Zifan Shi, [Chenyang Lei](https://chenyanglei.github.io/), Ka Lung Law, [Qifeng Chen](https://cqf.io/) <Br>
提出了一个controllable raw图像生成流程, 通过控制曝光时间, ISO, 噪声level和aperture, 控制生成图像的亮度, blur, 噪声等属性
  
##### CycleISP ★
**[Paper]** (CVPR 2020 Oral) CycleISP: Real Image Restoration via Improved Data Synthesis <Br>
**[Author]** [Syed Waqas Zamir](https://scholar.google.es/citations?user=WNGPkVQAAAAJ&hl=en), [Aditya Arora](https://adityac8.github.io/), [Salman Khan](https://salman-h-khan.github.io/), [Munawar Hayat](https://scholar.google.com/citations?user=Mx8MbWYAAAAJ&hl=en), [Fahad Shahbaz Khan](https://scholar.google.es/citations?user=zvaeYnUAAAAJ&hl=en), [Ming-Hsuan Yang](https://scholar.google.com/citations?user=p9-ohHsAAAAJ&hl=en), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=en)<Br>
**[[Pytorch-Code](https://github.com/swz30/CycleISP)]**  <Br>
提出了一个从sRGB到RAW相互转换的网络, 在Raw图像上注入高斯噪声用于生成RGB噪声样本.
  
### PyNet ★
**[Paper]** (CVPR 2020) Replacing Mobile Camera ISP with a Single Deep Learning Model <Br>
**[Author]**   Andrey Ignatov, Luc Van Gool, Radu Timofte  <Br>
**[[Code](https://github.com/aiff22/pynet)]**<Br>
1) 提出了一个端到端的深度学习网络, 用以代替现有的ISP处理流程. <Br>
2) 提出了一个华为P20 RAW 和Canon 5D的RAW-RGB图像对, 用以训练ISP模型.<Br>
3) 提出的算法与自带的ISP流程相比, 色彩上有一定提升, 但没有明显优势, 且存在晕影. 另外速度也是个问题. 因此对于用一个DL模型代替ISP流程的方案可行性还是有待确认. <Br>

###  TENet ★
**[Paper]**  (arXiv 1905) Trinity of Pixel Enhancement: a Joint Solution for Demosaicking, Denoising and Super-Resolution  <Br>
**[Author]** [Guocheng Qian](https://www.gcqian.com/), [Jinjin Gu](http://www.jasongt.com/), [Jimmy Ren](http://www.jimmyren.com/), [Chao Dong](http://xpixel.group/2010/01/20/chaodong.html), Furong Zhao, Juan Lin <Br>
**[[Pytorch-Code](https://github.com/guochengqian/TENet)]** <Br>
1. 使用具有pixel shift技术的相机收集了一可以做demoasic的数据集, 避免了用普通RGB数据做真值时内置demoasic过程带来的误差
2. 提出了一端到端的demosaic, 去噪和超分的网络, 采用residual + dense block的形式, 没什么特别的

### DeepISP ☆
**[Paper]** (TIP 2018) DeepISP: Learning End-to-End Image Processing Pipeline <Br>
**[Author]** [Eli Schwartz](https://elischwartz.github.io/publications/), [Raja Giryes](http://web.eng.tau.ac.il/~raja/),  [Alex M. Bronstein](https://bron.cs.technion.ac.il/) <Br>
大致浏览, 一个end-to-end的网络, 分为保持分辨率的low level部分和逐层下采样的high level部分. 使用了conv+relu, conv+tanh, 直连三个分支并行的设计, 比较少见

### Learning to See in the Dark ★★
**[Paper]** (CVPR 2018) Learning to See in the Dark <Br>
**[Author]** [Chen Chen](http://cchen156.web.engr.illinois.edu/), [Qifeng Chen](https://cqf.io/), [Jia Xu](http://pages.cs.wisc.edu/~jiaxu/), [Vladlen Koltun](http://vladlen.info/)  <Br>
**[[Project](http://cchen156.web.engr.illinois.edu/SID.html)]** **[[TF-Code](https://github.com/cchen156/Learning-to-See-in-the-Dark)]**<Br>
1) 提出了SID数据集, 包括RGB和Raw数据 <Br>
2) 提出了一个end-to-end的isp网络, 以RAW和增益信息为输入, 输入RGB图像, 代替传统ISP流程

### *Reconfiguring the Imaging Pipeline* ★★ 
**[Paper]** (ICCV 2017) Reconfiguring the Imaging Pipeline for Computer Vision <Br>
**[Author]**   [Mark Buckler](http://www.markbuckler.com/), [Suren Jayasuriya](http://www.andrew.cmu.edu/user/sjayasur/website.html), [Adrian Sampson](http://www.cs.cornell.edu/~asampson/)  <Br>
**[[Project](https://capra.cs.cornell.edu/research/visionmode/)]** **[[Code1](https://github.com/cucapra/approx-vision)]** **[[Code2](https://github.com/mbuckler/ReversiblePipeline)]** <Br>
1) 针对计算机视觉任务(而不是photography)简化ISP流程. 提出只有demosaicing和gamma校正是CV任务中必需的, 并据此设计了系统.
2) 系统包括3个步骤: reduced resolution readout, subsampling to produce RGB images, lower-precision logarithmic ADC configuration. 能将总体能耗降低约75%
3) 公布了一套用于模拟imaging pipeline及其逆过程的工具CRIP

### L3
**[Paper]** (TIP 2017) Learning the image processing pipeline <Br>
**[Author]** Haomiao Jiang, Qiyuan Tian, [Joyce Farrell](https://web.stanford.edu/group/scien/cgi-bin/farrell/), [Brian Wandell](https://web.stanford.edu/group/vista/cgi-bin/wandell/)  <Br>
将RAW到sRGB的转换用局部相信滤波器完成, 类似于RAISR.
  
### *A Software Platform for Manipulating the Camera Imaging Pipeline *
**[Paper]** (CVPR 2016) A Software Platform for Manipulating the Camera Imaging Pipeline  <Br>
**[Author]** [Hakki Can Karaimer](https://karaimer.github.io/), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
**[[Project](https://karaimer.github.io/camera-pipeline/)]** <Br> 
  
 
  

## AWB
### C5
**[Paper]** (ICCV 2021) Cross-Camera Convolutional Color Constancy <Br>
**[Author]** [Mahmoud Afifi](https://sites.google.com/corp/view/mafifi), [Jonathan T. Barron](https://jonbarron.info/), [Chloe LeGendre](http://www.chloelegendre.com/), [Yun-Ta Tsai](https://research.google/people/105312/), [Francois Bleibel](https://www.linkedin.com/in/fbleibel/)  <Br>

### *Multi-Hypothesis CC* ★☆
**[Paper]** (CVPR 2020) A Multi-Hypothesis Approach to Color Constancy for improved Automatic White Balance <Br>
**[Author]** [Daniel Hernandez-Juarez](https://danihernandez.eu/), [Sarah Parisot](https://parisots.github.io/), [Benjamin Busam](http://campar.in.tum.de/Main/BenjaminBusam), Ales Leonardis, [Gregory Slabaugh](http://www.gregslabaugh.net/), Steven McDonagh <Br>
**[[Project](http://cvil.eecs.yorku.ca/projects/public_html/sRGB_WB_correction/index.html)]**<Br>
  粗读, 用贝叶斯思想处理AWB问题. 首先用K-Means选取n个candidates, 再用一个小型CNN预测似然概率(即当前图像是来自于该光照的可能性), 最后的预测光照结果为n个似然概率取softmax后的加权求和.
  
### Deep White-Balance Editing ★☆
**[Paper]** (CVPR 2020 Oral) Deep White-Balance Editing <Br>
**[Author]** [Mahmoud Afifi](https://sites.google.com/view/mafifi/home), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/)<Br>
**[[PYtorch & Matlab-Code](https://github.com/mahmoudnafifi/Deep_White_Balance)]**<Br>
1) 1个encoder, 3个decoder, 分别预测正确, 白炽灯, 室外场景的白平衡结果. 最后可根据三个结果插值出用户需要的色温
2) 为在device上进行快速推理, 在小图上预测, 然后在小图上通过优化的方法闭式求解输入输出的全局色彩映射函数, 再将该函数用到全图上

### WB_sRGB
**[Paper]** (CVPR 2019) When Color Constancy Goes Wrong: Correcting Improperly White-Balanced Images <Br>
**[Author]** [Mahmoud Afifi](https://sites.google.com/view/mafifi/home), [Brian Price](https://www.brianpricephd.com/), [Scott Cohen](https://research.adobe.com/person/scott-cohen/), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
**[[Project](http://cvil.eecs.yorku.ca/projects/public_html/sRGB_WB_correction/index.html)]** **[[Code](https://github.com/mahmoudnafifi/WB_sRGB)]** **[[Blog](http://www.noahlab.com.hk/#/news/5ee70c18a0c07a1a3855452d)]**<Br>
  
### *Improving Color Reproduction Accuracy on Cameras*
**[Paper]** (CVPR 2018) Improving Color Reproduction Accuracy on Cameras <Br>
**[Author]** [Hakki Can Karaimer](https://karaimer.github.io/), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
**[[Project](https://karaimer.github.io/camera-color/)]** <Br> 
