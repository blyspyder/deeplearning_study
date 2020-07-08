## RNN

#### application

- slot filling

  ![image-20200704100254676](9RNN.assets/image-20200704100254676.png)

  

- 词向量化

  - one-hot编码

  - beyond one-hot

    ![image-20200704100548998](9RNN.assets/image-20200704100548998.png)

- nerual network做词划分工作的问题

  ![image-20200704100731957](9RNN.assets/image-20200704100731957.png)

  - 解决方法：使得神经网络有记忆性。



#### RNN

- example

  提前制定内存中的起始值，只有weight，没有bias

  ![image-20200704101219802](9RNN.assets/image-20200704101219802.png)

  **输入第二组参数后更新内存中的内容**

  ![image-20200704101339262](9RNN.assets/image-20200704101339262.png)

  

- **rnn解决slot filling**

  - 使用一个隐藏层

    ![image-20200704101612748](9RNN.assets/image-20200704101612748.png)

  - 使用深度神经网络

    ![image-20200704101822003](9RNN.assets/image-20200704101822003.png)

    

- **rnn变形**

  - 双向循环

    ![image-20200704102057154](9RNN.assets/image-20200704102057154.png)

    - 既可以学到从句首到句尾的上下文关系同时有可以学到从句尾到句首的关系

### LSTM

![image-20200704102650436](9RNN.assets/image-20200704102650436.png)

- 4个输入得到一个输出
- 输入门：决定是否存入到memory中
- 输出门：决定是否memory中的记忆是否能用
- forget门：决定memory什么时候忘记记忆

![image-20200704103228072](9RNN.assets/image-20200704103228072.png)

- **LSTM - Example**

  ![image-20200704103442408](9RNN.assets/image-20200704103442408.png)

  ![image-20200704103957654](9RNN.assets/image-20200704103957654.png)

  - **每一个门的权重和偏执都通过梯度下降方式学到**

  - **每个cell都是是一个nerual network**

  - LSTM需要的参数量会是一般的网络的4倍

    ![image-20200704104852477](9RNN.assets/image-20200704104852477.png)

    **x经过4个不同transform得到4个向量**

  - **图对应运算**

    ![image-20200704105048587](9RNN.assets/image-20200704105048587.png)

  - **多个cell运算**

    ![image-20200704105119884](9RNN.assets/image-20200704105119884.png)

  - **LSTM实际运算**

    ![image-20200704105154536](9RNN.assets/image-20200704105154536.png)

    - 真正LSTM进行transform之前同时考虑输入变量x，上一轮cell中的值，上一轮隐藏层的输出，将三个值同时考虑输入到transform中。