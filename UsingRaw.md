# Using Raw

###  TENet ★
**[Paper]**  (arXiv 1905) Trinity of Pixel Enhancement: a Joint Solution for Demosaicking, Denoising and Super-Resolution  <Br>
**[Author]** [Guocheng Qian](https://www.gcqian.com/), [Jinjin Gu](http://www.jasongt.com/), [Jimmy Ren](http://www.jimmyren.com/), [Chao Dong](http://xpixel.group/2010/01/20/chaodong.html), Furong Zhao, Juan Lin <Br>
**[[Pytorch-Code](https://github.com/guochengqian/TENet)]** <Br>
1. 使用具有pixel shift技术的相机收集了一可以做demoasic的数据集, 避免了用普通RGB数据做真值时内置demoasic过程带来的误差
2. 提出了一端到端的demosaic, 去噪和超分的网络, 采用residual + dense block的形式, 没什么特别的
