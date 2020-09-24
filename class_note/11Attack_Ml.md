#### Attack network

![image-20200807174619093](/home/bly/.config/Typora/typora-user-images/image-20200807174619093.png)

原图像中加入一部分噪声

- **没有目标的攻击**

  ![image-20200807174908164](/home/bly/.config/Typora/typora-user-images/image-20200807174908164.png)

  加入一定噪声后输出y与真实y相差越远越好

- **有目标攻击**

  ![image-20200807175234329](/home/bly/.config/Typora/typora-user-images/image-20200807175234329.png)

  离错误目标越接近越好

- **限制**

  加噪后图片和原图越接近越好，设置原图与加噪后图限制

  - 距离计算方法

    ![image-20200807180022784](/home/bly/.config/Typora/typora-user-images/image-20200807180022784.png)

    当每个像素都进行轻微改变和对其中一个像素改变较大两种方式

    

- **攻击实现方式**

  ![image-20200807180851255](/home/bly/.config/Typora/typora-user-images/image-20200807180851255.png)

  - **修正方式**

    ![image-20200807181040617](/home/bly/.config/Typora/typora-user-images/image-20200807181040617.png)

    找到距离最近点替换

- FGSM

  ![image-20200807220301076](/home/bly/.config/Typora/typora-user-images/image-20200807220301076.png)

  


#### 黑盒攻击

![image-20200807220822518](/home/bly/.config/Typora/typora-user-images/image-20200807220822518.png)

使用相同训练数据集训练神经网络，攻击重新训练出的网络，使用攻击的样本攻击黒盒网络



#### 防御

- **被动防御**

  不修改模型

  ![image-20200807224410091](/home/bly/.config/Typora/typora-user-images/image-20200807224410091.png)

  filter：**平滑化**

  - **feature squzue**

    ![image-20200807224818942](/home/bly/.config/Typora/typora-user-images/image-20200807224818942.png)
    
  - ![image-20200807224929600](/home/bly/.config/Typora/typora-user-images/image-20200807224929600.png)

- **主动防御**

  
  
  

