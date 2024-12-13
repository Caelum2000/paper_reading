## SAPG: Split and Aggregate Policy Gradients
1. 目前的on-policy的RL难以并行
2. 提出一种能并行的on-policy RL，并行地学习各个环境的policy，然后聚合
3. 复习RL后再看，放waiting list


### review
1. 推到PPO,TRPO, 搞清楚为什么用优势函数方差小
2. 本文主要是解决batch size增大对PPO不起作用的问题
3. 解决方法是把一个大batch size切分，然后每个块有一个policy，这些policy的超参数不同，得到的采样轨迹也不同。然后将policy进行聚合
4. 用到了off-policy 的PPO算法，各个policy可以access其他块的采样数据