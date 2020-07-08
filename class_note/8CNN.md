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
  
  2*2 image深度和filter数量相同，经过卷集池化后得到更小的图片。

- whole cnn

  ![image-20200629202712036](8CNN.assets/image-20200629202712036.png)

- flatten

  将矩阵数据换乘一个向量后输入全连接层。



## applicatino

- playing go

  ![image-20200629213556582](8CNN.assets/image-20200629213556582.png)

- speech

  ![image-20200629214505379](8CNN.assets/image-20200629214505379.png)

  声谱图能够分析得到所说内容。

  使用cnn尽心个图像识别，识别得到对应声音。

  cnn的filter应该在cnn的频率方面平移判定不同音表示，

 ## 如何分析cnn 



  

  