# HDR


#### *Single-Image HDR Reconstruction by Learning to Reverse the Camera Pipeline* ★
**[Paper]** (CVPR 2020) Single-Image HDR Reconstruction by Learning to Reverse the Camera Pipeline <Br>
**[Author]** [Yu-Lun Liu](http://www.cmlab.csie.ntu.edu.tw/~yulunliu/), [Wei-Sheng Lai](https://www.wslai.net/), [Yu-Sheng Chen](https://www.cmlab.csie.ntu.edu.tw/~nothinglo/), Yi-Lung Kao, [Ming-Hsuan Yang](https://faculty.ucmerced.edu/mhyang/), [Yung-Yu Chuang](https://www.csie.ntu.edu.tw/~cyy/), [Jia-Bin Huang](https://filebox.ece.vt.edu/~jbhuang/) <Br>
**[[Project](https://www.cmlab.csie.ntu.edu.tw/~yulunliu/SingleHDR)]** **[[TF-Code](https://github.com/alex04072000/SingleHDR)]**<Br>
用几个CNN模拟ISP中HDR到LDR的映射过程, 完成HDR. 关键是定义每个部分的训练目标和数据, 这部分没细看.

#### UnModNet
**[Paper]** (NeruIPS 2020) UnModNet: Learning to Unwrap a Modulo Image for High Dynamic Range Imaging <Br>
**[Author]**  Chu Zhou, Hang Zhao, Jin Han, [Chang Xu](http://changxu.xyz/), Chao Xu, Tiejun Huang, [Boxin Shi](http://ci.idm.pku.edu.cn/Publication.htm) <Br>
**[[Project](https://www.cmlab.csie.ntu.edu.tw/~yulunliu/SingleHDR)]** **[[TF-Code](https://github.com/alex04072000/SingleHDR)]**<Br>

#### ExpandNet
**[Paper]** (EG 2018) ExpandNet: A Deep Convolutional Neural Network for High Dynamic Range Expansion from Low Dynamic Range Content <Br>
**[Author]** 	Demetris Marnerides, [Thomas Bashford-Rogers](http://thomasbashfordrogers.com/), [Jonathan Hatchett](https://hatchett.co.uk/), [Kurt Debattista](https://warwick.ac.uk/fac/sci/wmg/people/profile/?wmgid=518)  <Br>
**[[Pytorch-Code](https://github.com/dmarnerides/hdr-expandnet)]** **[[Unofficial-TF-Code](https://github.com/echolijinghui/ExpandNet)]**<Br>

#### *Image Correction via Deep Reciprocating HDR Transformation*
**[Paper]** (CVPR 2018) Image Correction via Deep Reciprocating HDR Transformation <Br>
**[Author]** [Xin Yang](http://faculty.dlut.edu.cn/yangxin/zh_CN/index.htm), Ke Xu, [Yibing Song](https://ybsong00.github.io/), Qiang Zhang, Xiaopeng Wei, [Rynson Lau](https://www.cs.cityu.edu.hk/~rynson/)  <Br>
**[[Project](https://ybsong00.github.io/cvpr18_imgcorrect/index.html)]** **[[TF-Code](https://github.com/ybsong00/DRHT)]**<Br>
	
#### HDRCNN ★
**[Paper]** (Siggraph Asia 2017) HDR image reconstruction from a single exposure using deep CNNs <Br>
**[Author]** [Gabriel Eilertsen](http://vcl.itn.liu.se/members/gabriel-eilertsen), [Joel Kronander](http://vcl.itn.liu.se/members/joel-kronander), [Gyorgy Denes](https://www.cl.cam.ac.uk/~gd355/), [Rafał K. Mantiuk](https://www.cl.cam.ac.uk/~rkm38/), [Jonas Unger](http://webstaff.itn.liu.se/~jonun/web/Home.php) <Br>
**[[Page](http://hdrv.org/hdrcnn/)]** **[[TF-Code](https://github.com/gabrieleilertsen/hdrcnn)]** <Br>
	粗读, 较早将CNN用于HDR的一篇paper, 网络结构比较老, 但提出了两个可能有趣的点: 1) 将输入转换到log域训练更符合人眼视觉特性; 2) 高光部分采用输入和输出线性加权的方式, 修复过曝光, 并避免形成带状伪影. <Br>
	
#### DrTMO
**[Paper]** (Siggraph Asia 2017) Deep Reverse Tone Mapping <Br>
**[Author]** [Yuki Endo](http://www.npal.cs.tsukuba.ac.jp/~endo/index_en.html), [Yoshihiro Kanamori](http://kanamori.cs.tsukuba.ac.jp/index.html), [Jun Mitani](http://mitani.cs.tsukuba.ac.jp/en/)  <Br>
**[[Project](http://www.npal.cs.tsukuba.ac.jp/~endo/projects/DrTMO/)]** **[[Unofficial-Pytorch-Code](https://github.com/shleecs/DrTMO_unofficial_pytorch)]**<Br>
	
