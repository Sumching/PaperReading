# Latent Filter Scaling for Multimodal Unsupervised Image-to-Image Translation(CVPR2019)

### 目的：解决一张source域图片转换到多张target域图片

### 贡献：认为自己质量和多样性多达到SOTA，且十分简单

![image-20191211193427659](/home/chenshen/.config/Typora/typora-user-images/image-20191211193427659.png)

<center>图1, 通过一些因子乘上不同的featuremap，实现风格多样性目的</center>

### 如何证明z学到的是风格特征，固定一个z，改变不同的输入图片，输出的是同一种风格的图片。

![image-20191211195238659](/home/chenshen/.config/Typora/typora-user-images/image-20191211195238659.png)

### 在mapping从z到scalar上，选择tanh会质量比较好，选择leakyrelu变化更多，这是因为tanh bounded了scalar的幅度，导致乘到filters上就比较小。

### 全链接网络不使用bias也会导致图片变化更多，作者认为目标域的风格的平均点会被bias学到。



## 评估

### 数据集： winter to summer, edges to shoes, labels to facades.

### 评测方法：qulity（忽略） 和 *diversity*  Learned Perceptual Image Patch Similarity (LPIPS)



