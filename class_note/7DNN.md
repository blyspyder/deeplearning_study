## DNN

使用network为了将目标函数变为非线性

- 激活函数

  - RELU

    ![image-20200618135930282](7DNN.assets/image-20200618135930282.png)

  0点处不可微分。

  - ReLU-variant

    ![image-20200618140144037](7DNN.assets/image-20200618140144037.png)

- Maxout

  Relu时Maxout的一个特殊例子。自动寻找激活函数

  ![image-20200618140442814](7DNN.assets/image-20200618140442814.png)

  可以决定多个element为一个组，例子中为两个element为一个组。

  假设z2为0，则maxout为RELU

  ![image-20200618140759423](7DNN.assets/image-20200618140759423.png)

  假设z2不为0：

  ![image-20200618140850128](7DNN.assets/image-20200618140850128.png)

- 训练Maxout

  **由于存在max函数因此不能微分**

  ![image-20200618141041656](7DNN.assets/image-20200618141041656.png)

  没有接上的部分可以除去。

  ![image-20200618141105392](7DNN.assets/image-20200618141105392.png)

  - 如何处理没有训练到的权重值

    每次给定不同输入x，每次选定z不同，因此所有都会训练到

- Moment优化器

  ![image-20200618152239256](7DNN.assets/image-20200618152239256.png)

  

- Dropout

  ![image-20200618152757178](7DNN.assets/image-20200618152757178.png)

  ![image-20200618152809283](7DNN.assets/image-20200618152809283.png)

  

  不同trainset通过不同model得到的结果平均。

  ![image-20200618153043856](7DNN.assets/image-20200618153043856.png)

  

