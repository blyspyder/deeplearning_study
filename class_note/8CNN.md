## cnn整个网络

![image-20200618160126251](8CNN.assets/image-20200618160126251.png)

- ### convolution

  - **黑白图片**		![image-20200618155241364](8CNN.assets/image-20200618155241364.png)

  多少filter就会出现多少结果

  - **彩色图片**

  ​	![image-20200618155436517](8CNN.assets/image-20200618155436517.png)

  每个filter考虑不同颜色的channel

  - #### filter理解

    ![image-20200618155913898](8CNN.assets/image-20200618155913898.png)

    - 每个filter相当于一个neural
    - 每个neural只关注部分weight
    - neural共享权重

- Max Pooling

  ![image-20200618160507756](8CNN.assets/image-20200618160507756.png)

  四个中选择最大一个保留

  ![image-20200618160537371](8CNN.assets/image-20200618160537371.png)

- CNN - Max pooling之后图像缩小

  ![image-20200618160649797](8CNN.assets/image-20200618160649797.png)

  每次卷积池化后都得到一个更小的image。

 ## 如何分析cnn 

  

  