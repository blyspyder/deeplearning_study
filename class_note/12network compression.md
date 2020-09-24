**移动设备运算资源有限，不能使用较深网络，本文主要讲解缩小模型方法**

#### Network Pruning

![image-20200807230044551](/home/bly/Document/deeplearning_study/class_note/12network compression.assets/image-20200807230044551.png) 

- **pruning weigth**

  ![image-20200808132705472](/home/bly/Document/deeplearning_study/class_note/12network compression.assets/image-20200808132705472.png)

  - 1. 训练一个较大network
    2. 取出大network中影响较大参数组成小网络
    3. 使用大网络对应节点参数初始化西哦呵网络
    4.  使用相同数据集训练该较小网络

  - 问题

    网络不规则，导致现实中不能使用GPU加速。

- **purning neuron**

  ![image-20200808133606104](/home/bly/Document/deeplearning_study/class_note/12network compression.assets/image-20200808133606104.png)

  将网络中前后连接的weight都断开

  

#### 知识蒸馏

![image-20200808134542932](/home/bly/Document/deeplearning_study/class_note/12network compression.assets/image-20200808134542932.png)

- 较小网络学习大网络模仿模型输出

- 效果较好原因

  **不仅告诉学生网络该图片是1，而且告诉该网络1和7比较相近** 



#### Parameter Quantization

- 使用更少的bit表示一个数值

- **weight clustering**

  ![image-20200808142404330](/home/bly/Document/deeplearning_study/class_note/12network compression.assets/image-20200808142404330.png)

  先将weight进行聚类，聚类后使用一个值表示聚类中的所有数值

  **较常出现的weight使用较短编码表示**

- **binary connect**



#### 调整网络架构设计 

- 网络架构调整

  ![image-20200808154155121](/home/bly/Document/deeplearning_study/class_note/12network compression.assets/image-20200808154155121.png)

  

  

- 标准卷积

  ![image-20200808154256086](/home/bly/Document/deeplearning_study/class_note/12network compression.assets/image-20200808154256086.png)

  72个参数

- 修改后的卷积

  ![image-20200808154449537](/home/bly/Document/deeplearning_study/class_note/12network compression.assets/image-20200808154449537.png)

  总共使用26个参数

#### Dynamic compution

- 训练多分类

- 隐藏层分类

  根据网络中间层决定结果

  ![image-20200808160246064](/home/bly/Document/deeplearning_study/class_note/12network compression.assets/image-20200808160246064.png)

