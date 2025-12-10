### The Causal-Neural Connection: Expressiveness, Learnability, and Inference
1. 提出了一种与SCM对应的神经网络模型NCM，大概就是用神经网络的计算图代表SCM的generation process
2. 通过训练NCM实现causal identification问题，就是给定DAG的情况下计算intervention等
3. loss分为两个部分，第一部分是对observed data distribution的matching。第二部分是是对intervention distribution的maximize/minimize
4. 如果interventional distribution优化得到的max和min差距过大，则认为基于现在的DAG是不能identification的，有unobserved cofounder
5. 有很多数学细节，没仔细check

### reveiw
1. 为什么不能直接学习do(t)的分布，而忽略unobserved variable(如backdoor)？正如condition生成。（可能的答案：没有do(t)的样本）
2. 结合Partial Identification of Treatment Effects with Implicit Generative Models（UATD）
3. NCM是怎么实现最大最小优化的，在优化过程中是否使用了类似UATD的遍历可能的SCM?