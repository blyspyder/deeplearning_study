## Policy Gradient

- #### policy of actor

  ![image-20200624142244185](Policy Gradient.assets/image-20200624142244185.png)

  - pixels：输入
  - DNN：agent
  - actor输出
  
- #### actor，env，reward

  ![image-20200624142922335](Policy Gradient.assets/image-20200624142922335.png)

- #### policy gradient

  ![image-20200624143125798](Policy Gradient.assets/image-20200624143125798.png)

  

  - 更新参数

    ![image-20200624144047410](Policy Gradient.assets/image-20200624144047410.png)

    需要收集多组<state,action>

  - 实际部署

    ![image-20200624144420229](Policy Gradient.assets/image-20200624144420229.png)

    - add a Baseline

      ![image-20200624144759578](Policy Gradient.assets/image-20200624144759578.png)

      **解决所有R都为正的问题**

    - Assign Suitable Credit

      