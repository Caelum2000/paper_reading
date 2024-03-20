1. 由RHLF设计的rewrad function 推出该reward下最优的policy (这一步推导很有意思)
2. 将上述policy带入prefernece的模型，比如 Bradley-Terry model 得到一个2分类问题，将rl问题转换为分类问题
3. 对DPO进行了理论分析，证明了
    - 每一个reward的等价类都有一个代表函数。(theorem 1)
    - 一个等价类内的reward诱导同样的preference objective (lemma 1)
    - 一个等价类内的rewrad的RHLF reward 确定同样的最优policy (lemma 2)
4. 分析了原有RLHF基于actor-critic算法（如PPO）不稳定的原因,**这一部分没看懂**