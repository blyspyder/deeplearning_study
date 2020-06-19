## Logistic Regression

- 概念

  ![image-20200617145653035](5.assets/image-20200617145653035.png)

  得到目标值为某一个分类的概率。使用sigmoid Function之后输出都为0，1之间
  
- function 好坏

  ![image-20200617150556495](5.assets/image-20200617150556495.png)

  交叉熵计算损失。

- 逻辑回归和线性回归比较

  ![image-20200617151459795](5.assets/image-20200617151459795.png)

- cross entropy 和 square error

  ![image-20200617152011822](5.assets/image-20200617152011822.png)

  分类问题时cross entropy距离目标越远则微分越大。

- 多分类原理

  ![image-20200617154150240](5.assets/image-20200617154150240.png)

  输出和为1，强化其中较大的值。
     - **多分类案例**

       ![image-20200617154714604](5.assets/image-20200617154714604.png)

- 特征转换后逻辑回归

  ![image-20200617155215646](5.assets/image-20200617155215646.png)

  使用两个逻辑回归首先进行特征转换，特征转换后在使用一个逻辑回归得到分类结果。

- 类神经网络

  ![image-20200617155511186](5.assets/image-20200617155511186.png)

​      多个逻辑回归相连