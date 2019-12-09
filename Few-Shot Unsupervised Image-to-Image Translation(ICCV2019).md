# Few-Shot Unsupervised Image-to-Image Translation(ICCV2019)

***paper*** ： https://arxiv.org/pdf/1905.01723.pdf

***code*** ：https://github.com/NVlabs/FUNIT



### 问题定义：能够生成训练过程中没见过的风格的图片，仅在测试过程中给出少量目标域的图片。



![image-20191203185721539](/home/chenshen/.config/Typora/typora-user-images/image-20191203185721539.png)

<center>图1 训练过程只输入一张 content image和 class images， 而在测试阶段，class images换成从没见过的 Target class</center>

![image-20191203200138277](/home/chenshen/.config/Typora/typora-user-images/image-20191203200138277.png)

![image-20191203200158880](/home/chenshen/.config/Typora/typora-user-images/image-20191203200158880.png)

![image-20191203200236689](/home/chenshen/.config/Typora/typora-user-images/image-20191203200236689.png)

*<u>GAN的损失，是对于每一类都是一个二分类的GAN损失</u>*

![image-20191203200343128](/home/chenshen/.config/Typora/typora-user-images/image-20191203200343128.png)

![image-20191203200356131](/home/chenshen/.config/Typora/typora-user-images/image-20191203200356131.png)

### 效果

![image-20191203200645222](/home/chenshen/.config/Typora/typora-user-images/image-20191203200645222.png)







