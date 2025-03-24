## Title: Amortizing intractable inference in large language models
1. 利用GFlowNet fintune LLm， LLM相当于policy(agent)
2. 有些细节不太清楚，也没有示意图之类的
3. Sec.2 中展示了用GflowNet fintune的LLM有生成uniform distribution数字的能力，但PPO的效果很差，有没有什么定量解释
4. amortizing在哪里，有什么意义 
5. 没太看懂insight, 结合openreview再看一下


### review
1. Gflownet 的 loss来自于 Learning GFlowNets from partial episodes for improved convergence and stability。 可能需要看一下
2. 为什么叫 amortizing, 可以看一下 Amortized Variational Inference: When and Why?
3. 对于CoT,一般有x->z->y.那么R(z) 是怎么来的
4. 根据Learning GFlowNets from partial episodes for improved convergence and stability, 使用的loss是Subtrajectory balance, 有一个forward和backward prob. idea类似Detailed balance(见该文章related work)