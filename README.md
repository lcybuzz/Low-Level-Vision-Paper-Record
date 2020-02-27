# Personal repository under construction.

# Table of Contents
- [Restoration](#restoration)
	- [DL Restoration](#dl-restoration)
	- [Traditional Restoration](#traditional-restoration)
	- Rank
		- ★★★ <Br>
		- ★★ <Br>
		- ★ <Br>
		  [DuRN]
- [Denoising](#denoising)
	- [DL Denoising](#dl-denoising)
	- [Traditional Denoising](#traditional-denoising)
	- Rank
		- ★★★ <Br>
		- ★★ <Br>
		- ★ <Br>
		  [RIDNet], [Unprocessing Images for Learned Raw Denoising]
- [Dataset](#dataset)
- [Useful Resources](#useful-resources)

# Restoration
## DL Restoration
### DuRN ★☆
**[Paper]** Dual Residual Networks Leveraging the Potential of Paired Operations for Image Restoration<Br>
**[Year]** CVPR 2019 <Br>
**[Author]** Xing Liu, Masanori Suganuma, Zhun Sun, Takayuki Okatani<Br>
**[Pages]** https://github.com/saeed-anwar/RIDNet <Br>
**[Description]** <Br>
1) 文章提出, 许多图像复原任务都由一些成对的模块组成, 比如去噪里的大kernel和小kernel, 超分里的下采样和上采样. 本文在residual connection的基础上, 进一步给每个模块内部的操作直接加入residual connection, 增加了组合数. <Br>
2) 在去噪, 去模糊, 去雾等任务中都取得了不错的效果. <Br>
	
## Traditional Restoration


# Denoising
## DL Denoising

### RIDNet ★☆
**[Paper]** Real image denoising with feature attention<Br>
**[Year]** ICCV 2019 Oral <Br>
**[Author]** [Saeed Anwar](https://saeed-anwar.github.io/), Nick Barnes<Br>
**[Pages]** https://github.com/saeed-anwar/RIDNet <Br>
**[Description]** <Br>
1) 提出了一个端到端的去噪网络, 基于channel attention和skip connection. 在真是图像上测试效果不错, 速度一般. <Br>
2) 作为一篇Oral来说感觉创新点和理论论述都一般, 也没有解释为什么提出的网络对真是图像去噪效果好. <Br>
3) 如果需要, 参考网络流程图和代码即可. <Br>
	
### Unprocessing Images for Learned Raw Denoising ★☆
**[Paper]** Unprocessing Images for Learned Raw Denoising<Br>
**[Year]** CVPR 2019 <Br>
**[Author]** [Tim Brooks](https://www.timothybrooks.com/tech/), [Ben Mildenhall](https://people.eecs.berkeley.edu/~bmild/), [Tianfan Xue](http://people.csail.mit.edu/tfxue/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/), [Dillon Sharlet](http://dsharlet.com/), [Jonathan T. Barron](https://jonbarron.info/)<Br>
**[Pages]** https://www.timothybrooks.com/tech/unprocessing/ <Br>
**[Description]** <Br>
1) 提出了一个通过unprocess ISP流程而生成更真实去噪样本的框架, 可以用任意图像生成真实的训练样本, 以提高模型性能. <Br>
2) 对于sRGB图像, 根据ISP流程, 将其逐步逆运算位raw image, 在此基础上加的噪声更符合真实噪声.<Br>
3) 推断时, 要先把sRGB转换为raw image, 再经过网络处理, 最后再进行正向的ISP恢复为sRGB. <Br>
4) ISP流程的推断对每个品牌型号的相机都有所不同, 模拟其过程感觉还是有难度的. <Br>
	
## Traditional Denoising

# Dataset
## Real Image Denoising
[DnD](https://noise.visinf.tu-darmstadt.de/) <Br>
[SIDD](https://www.eecs.yorku.ca/~kamel/sidd/) <Br>

[PolyU](https://github.com/csjunxu/PolyU-Real-World-Noisy-Images-Dataset) <Br>
[Renoir](http://ani.stat.fsu.edu/~abarbu/Renoir.html) <Br>
[CC](http://snam.ml/research/ccnoise) <Br>
[SID](http://cchen156.web.engr.illinois.edu/SID.html) <Br>
[kodak_color](http://r0k.us/graphics/kodak/) <Br>
[NoiseClinicImages](http://demo.ipol.im/demo/125/input_select?044_solvay_1927.x=63&044_solvay_1927.y=68) <Br>

# Useful Resources
https://paperswithcode.com/task/image-denoising?page=2 

https://github.com/wenbihan/reproducible-image-denoising-state-of-the-art


