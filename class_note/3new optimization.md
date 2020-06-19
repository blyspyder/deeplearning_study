## New Optimizers for Deep Learning

### what is optimization acout

​		![image-20200616155704590](3new optimization.assets/image-20200616155704590.png)

### on-line VS Off-line

- off-line

![image-20200616155752988](3new optimization.assets/image-20200616155752988.png)

​	已知所有训练资料

- on-line

  ![image-20200616155852498](3new optimization.assets/image-20200616155852498.png)

  每次只知道一对

### SGD

​	![image-20200616160134660](3new optimization.assets/image-20200616160134660.png)

### SGDM

​	![image-20200616160202534](3new optimization.assets/image-20200616160202534.png)

 增加向量v，movement计算时需要使用过去的movement。作用：**添加过去累加项，确保当L趋近于0时，仍然能够保持移动**。如图例子

​	![image-20200616160405518](3new optimization.assets/image-20200616160405518.png)

### Adagrade

 		![image-20200616160503174](3new optimization.assets/image-20200616160503174.png)

   添加一个分母为过去梯度和。避免下降过大导致跳过最低点。因为梯度一直累加，可能导致学习率过小。

### RMSProp

​		![image-20200616160615988](3new optimization.assets/image-20200616160615988.png)

类似adagrade和movement求和。

- 防止梯度过大导致停止。
- 不能处理梯度为0位置

### Adam

​	![image-20200616161043054](3new optimization.assets/image-20200616161043054.png)

### 有点

- SGDM：最终收敛较低

- Adam：收敛速度快

- SWATS

  **结合SGDM和Adam**训练过程中切换

  ![image-20200616161623545](3new optimization.assets/image-20200616161623545.png)

- 