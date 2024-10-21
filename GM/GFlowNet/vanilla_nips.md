## Title: Flow Network based Generative Models for Non-Iterative Diverse Candidate Generation
1. 将RL里的reward 看作能量，想要通过逐步采样最大化这个能量。RL和生成模型结合的工作
2. reward只给最终想要的states，其他state reward=0
3. 把MDP过程看成一个DAG，然后reward看作“汇”（流入），在DAG每条路径上有flow，每个节点满足流出等于流入. 满足 Eq.4
4. 根据flow的大小标准化后采样(proposition 2)
5. 优化的算法和loss和RL 中的 temporal difference 类似，就是让flow在DAG的分布满足Eq.4的稳定方程. 见Eq.11 Eq.12
6. 在下游任务是具体怎么设计的，还得看一下其他论文