# Personal repository under construction.

# Table of Contents
- [Denoising](#denoising)
	- [DL Methods](#dl-methods)
	- [Traditional Methods](#general-traditional-methods)
 - ★★★ <Br>
 - ★★ <Br>
 - ★ <Br>
	
# [Useful Resources](#useful-resources)
	
# Denoising
## DL Methods

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
	
## Traditional Methods

## Useful Resources
https://paperswithcode.com/task/image-denoising?page=2 
https://github.com/wenbihan/reproducible-image-denoising-state-of-the-art
