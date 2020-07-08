
# Denoising
## DL Denoising

### IRCNN ★
**[Paper]** (CVPR 2017) Learning Deep CNN Denoiser Prior for Image Restoration<Br>
**[Author]** [Kai Zhang](https://github.com/cszn), [Wangmeng Zuo](https://github.com/cszn), [Shuhang Gu](https://sites.google.com/site/shuhanggu/), [Lei Zhang](http://www4.comp.polyu.edu.hk/~cslzhang/)<Br>
**[[Matlab-Code](https://github.com/cszn/IRCNN)]**  <Br>
大致浏览, 提出了一个结构简单的CNN去噪器, 可以为基于模型的优化方法提供有效的prior, 还可以用于求解其它图像恢复的逆问题
	
### RIDNet ★☆
**[Paper]** (ICCV 2019 Oral) Real image denoising with feature attention<Br>
**[Author]** [Saeed Anwar](https://saeed-anwar.github.io/), Nick Barnes<Br>
**[[Code](https://github.com/cszn/IRCNN)]**  <Br>
1) 提出了一个端到端的去噪网络, 基于channel attention和skip connection. 在真是图像上测试效果不错, 速度一般. <Br>
2) 作为一篇Oral来说感觉创新点和理论论述都一般, 也没有解释为什么提出的网络对真是图像去噪效果好. <Br>
3) 如果需要, 参考网络流程图和代码即可. <Br>
	
### Unprocessing Images for Learned Raw Denoising ★☆
**[Paper]** (CVPR 2019) Unprocessing Images for Learned Raw Denoising<Br>
**[Author]** [Tim Brooks](https://www.timothybrooks.com/tech/), [Ben Mildenhall](https://people.eecs.berkeley.edu/~bmild/), [Tianfan Xue](http://people.csail.mit.edu/tfxue/), [Jiawen Chen](http://people.csail.mit.edu/jiawen/), [Dillon Sharlet](http://dsharlet.com/), [Jonathan T. Barron](https://jonbarron.info/)<Br>
**[[Code](https://www.timothybrooks.com/tech/unprocessing/)]**  <Br>
1) 提出了一个通过unprocess ISP流程而生成更真实去噪样本的框架, 可以用任意图像生成真实的训练样本, 以提高模型性能. <Br>
2) 对于sRGB图像, 根据ISP流程, 将其逐步逆运算位raw image, 在此基础上加的噪声更符合真实噪声.<Br>
3) 推断时, 要先把sRGB转换为raw image, 再经过网络处理, 最后再进行正向的ISP恢复为sRGB. <Br>
4) ISP流程的推断对每个品牌型号的相机都有所不同, 模拟其过程感觉还是有难度的. <Br>
	
### CBDNet ★☆
**[Paper]** (CVPR 2019) Toward Convolutional Blind Denoising of Real Photographs<Br>
**[Author]** Shi Guo, Zifei Yan, Kai Zhang, Wangmeng Zuo, Lei Zhang, [Jonathan T. Barron](https://jonbarron.info/)<Br>
**[[Code](https://github.com/GuoShi28/CBDNet)]**  <Br>
1) 大致浏览. 采用一个FCN估计噪声level, 噪声level map与输入concat然后输入一类似U-Net的网络去噪. <Br>
2) 可以学习其网络和训练细节. <Br>

### SGN ★
**[Paper]** (ICCV 2019) Self-Guided Network for Fast Image Denoising<Br>
**[Author]** Shuhang Gu, Yawei Li, [Luc Van Gool](https://ee.ethz.ch/the-department/people-a-z/person-detail.html?persid=90233), [Radu Timofte](https://people.ee.ethz.ch/~timofter/)<Br>
**[[Pytorch-Code](https://github.com/zhaoyuzhi/Self-Guided-Network-for-Fast-Image-Denoising)]**  <Br>
pixel shuffle + 多尺度聚合的轻量级网络, 只在高斯噪声上实验了一下
