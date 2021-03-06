# Proximal-Dehaze-Net-CPU

CPU based Matlab code for ECCV 2018 paper "[Proximal Dehaze-Net: A Prior Learning-Based Deep Network for Single Image Dehazing](http://openaccess.thecvf.com/content_ECCV_2018/papers/Dong_Yang_Proximal_Dehaze-Net_A_ECCV_2018_paper.pdf)". There is only test code right now and we will release the training code soon.

### Installation

The code is based on [MatConvNet](http://www.vlfeat.org/matconvnet/) package. You may need to first run the setup codes to run the demo

```matlab
vl_compilenn
```

### Demo

Simply run demo.m will give an example of our dehazing methods. 

There are 3 trained models:

1. "net-ours-s1.mat": 1-stage network trained on our own dataset
2. "net-reside-s1.mat": 1-stage network trained on RESIDE dataset
3. "net-reside-s2.mat": 2-stage network trained on RESIDE dataset

These models are evaluated respectively by function `cnn_ours_eval`, `cnn_reside_s1_eval` and `cnn_s2_eval`.

The code is tested on Ubuntu 16.04 with Matlab R2018a. It should work well on other operating systems like Windows. And for any problem on compiling MatConvNet package, please refer to http://www.vlfeat.org/matconvnet/ or contact me at: yangdong2010@stu.xjtu.edu.cn.

If a GPU device is available, it is recommended to use the GPU version of our dehazing network: https://github.com/legendongary/Proximal-Dehaze-Net-GPU.

### Update

Supplementary material is added: https://github.com/legendongary/Proximal-Dehaze-Net-GPU/blob/master/supplementary-material.pdf