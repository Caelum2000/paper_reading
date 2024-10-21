## Title: Predictive auxiliary objectives in deep RL mimic learning in the brain
1. 探索predictive loss对RL特征表示的影响和提升
2. 具体是用一个网络去根据$s_t,a_t$预测$\hat{s}_{t+1}$. 然后用loss对其真实的$s_{t+1}$和预测的$\hat{s}_{t+1}$
3. 文章指出，这种预测loss和hippocampus有关。这个预测模块可以解释为hippocampus, 根据$s_t$产生$a_t$的policy net可以看作纹状体
4. 实验结果肯定是加了predictive loss的好。