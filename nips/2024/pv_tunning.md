## PV-Tuning: Beyond Straight-Through Estimation for Extreme LLM Compression
1. 研究的是LLM的量化
2. 指出之前基于STE的量化方法可能是sub-optimal的
3. 具体的前序工作忘了，放waiting list   


### review
1. 使用两步P-tuning 和 V-tuning来迭代优化已经量化的网络
2. P-tuning是优化一个codebook,也就量化后值的选择集，例如NF4就就有2^4可以选择
3. V-tuning是优化对于一个参数选择codebook或选择集中的哪些值, 见Alg.1 Alg.2
4. V-tuning可以使用梯度近似, 近似的推导有点意思