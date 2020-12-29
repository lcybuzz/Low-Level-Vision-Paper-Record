# ISP
ISP及其内部模块相关论文

## ISP
### *Reconfiguring the Imaging Pipeline* ★★ 
**[Paper]** (ICCV 2017) Reconfiguring the Imaging Pipeline for Computer Vision <Br>
**[Author]**   [Mark Buckler](http://www.markbuckler.com/), [Suren Jayasuriya](http://www.andrew.cmu.edu/user/sjayasur/website.html), [Adrian Sampson](http://www.cs.cornell.edu/~asampson/)  <Br>
**[[Project](https://capra.cs.cornell.edu/research/visionmode/)]** **[[Code1](https://github.com/cucapra/approx-vision)]** **[[Code2](https://github.com/mbuckler/ReversiblePipeline)]** <Br>
1) 针对计算机视觉任务(而不是photography)简化ISP流程. 提出只有demosaicing和gamma校正是CV任务中必需的, 并据此设计了系统.
2) 系统包括3个步骤: reduced resolution readout, subsampling to produce RGB images, lower-precision logarithmic ADC configuration. 能将总体能耗降低约75%
3) 公布了一套用于模拟imaging pipeline及其逆过程的工具CRIP
  

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

### PyNet ★
**[Paper]** (arXiv 2002) Replacing Mobile Camera ISP with a Single Deep Learning Model <Br>
**[Author]**   Andrey Ignatov, Luc Van Gool, Radu Timofte  <Br>
**[[Code](https://github.com/aiff22/pynet)]**<Br>
1) 提出了一个端到端的深度学习网络, 用以代替现有的ISP处理流程. <Br>
2) 提出了一个华为P20 RAW 和Canon 5D的RAW-RGB图像对, 用以训练ISP模型.<Br>
3) 提出的算法与自带的ISP流程相比, 色彩上有一定提升, 但没有明显优势, 且存在晕影. 另外速度也是个问题. 因此对于用一个DL模型代替ISP流程的方案可行性还是有待确认. <Br>



## AWB

### WB_sRGB
**[Paper]** (CVPR 2019) When Color Constancy Goes Wrong: Correcting Improperly White-Balanced Images <Br>
**[Author]** [Mahmoud Afifi](https://sites.google.com/view/mafifi/home), [Brian Price](https://www.brianpricephd.com/), [Scott Cohen](https://research.adobe.com/person/scott-cohen/), [Michael S. Brown](http://www.cse.yorku.ca/~mbrown/) <Br>
**[[Project](http://cvil.eecs.yorku.ca/projects/public_html/sRGB_WB_correction/index.html)]** **[[Code](https://github.com/mahmoudnafifi/WB_sRGB)]** **[[Blog](http://www.noahlab.com.hk/#/news/5ee70c18a0c07a1a3855452d)]**<Br>
  
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
