## PRISE: LLM-Style Sequence Compression for Learning Temporal Action Abstractions in Control
1. 解决temporal action abstraction的问题
2. 没看出和连续学习的关系，没太看懂
3. 放到waiting lis  t


### review
1. 类似VQ-VAE, 只不过是将连续时间的动作序列用离散的codebook表示
2. 将连续动作离散化，有利于与基于分类的autoregressive模型对接，例如输入离散的语言，输出由codebook解码的连续动作 