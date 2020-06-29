## Q-learning

#### Critic

- ![image-20200625195319499](Q-learning.assets/image-20200625195319499.png)

  衡量actor好坏，需要给定状态s和/pi

  相同actor，不同策略获得奖励不同

- estimate

  - **MC-based**

   ![image-20200625195631403](Q-learning.assets/image-20200625195631403.png)

  - **TD-Based**

    ![image-20200625195856577](Q-learning.assets/image-20200625195856577.png)

  - Q-function

    ![image-20200625200603500](Q-learning.assets/image-20200625200603500.png)

    固定状态下固定动作得到的奖励。

  - Q-Learning

    ![image-20200625201059498](Q-learning.assets/image-20200625201059498.png)

#### Target Network

​		![image-20200625201759720](Q-learning.assets/image-20200625201759720.png)

​	训练updata网络多次后，在更新fixed的参数（参数复制）

#### Replay Buffer

![image-20200625202615370](Q-learning.assets/image-20200625202615370.png)

- replay buffer：减少与环境互动的次数

#### Double DQN

![image-20200625203219480](Q-learning.assets/image-20200625203219480.png)

![image-20200625203615683](Q-learning.assets/image-20200625203615683.png)、

#### Dueling DQN

![image-20200625203741252](Q-learning.assets/image-20200625203741252.png)

改动network架构。

#### Noisy Net

![image-20200625204851757](Q-learning.assets/image-20200625204851757.png)

#### Distributional Q-function

![image-20200625205432243](Q-learning.assets/image-20200625205432243.png)

输出分布情况。

#### Q-Leraning for Continuous Actions

![image-20200627142132905](Q-learning.assets/image-20200627142132905.png)

![image-20200627142425525](Q-learning.assets/image-20200627142425525.png)

