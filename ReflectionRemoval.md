# Reflection Removal


### perceptual-reflection-removal ★☆
**[Paper]** (CVPR 2018) Single Image Reflection Removal with Perceptual Losses <Br>
**[Author]** [Xuaner Zhang](https://people.eecs.berkeley.edu/~cecilia77/), [Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html), [Qifeng Chen](https://cqf.io/) <Br>
**[[Project](https://people.eecs.berkeley.edu/~cecilia77/project-pages/reflection.html)]** **[[TF-Code](https://github.com/ceciliavision/perceptual-reflection-removal)]**<Br>
VGG19的多层特征作为hypercolumn与图像串联作为输入, 一个网络同时预测transmission和reflection, 使用pixel, VGG和GAN loss, 另外提出了一个gradient exclusion loss. 


### ERRNet ★
**[Paper]** (CVPR 2019) Single Image Reflection Removal Exploiting Misaligned Training Data and Network Enhancements <Br>
**[Author]** [Kaixuan Wei](https://kxwei.net/), [Jiaolong Yang](http://jlyang.org/), [Ying Fu](https://ying-fu.github.io/), [David Wipf](http://www.davidwipf.com/), Hua Huang <Br>
**[[Pytorch-Code](https://github.com/Vandermode/ERRNet)]** **[[Pytorch-Code](https://github.com/Vandermode/ERRNet)]**<Br>
也用了VGG19的特征串联作为输入, 采用了PSP模块和channel-wise attention模块. 使用pixel loss, VGG loss, GAN loss, 另外提出了一个利用非对齐数据训练的方法, 貌似就是用VGG的高层特征计算距离, 效果上看不如contextual loss.  
