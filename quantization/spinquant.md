### SPINQUANT: LLM QUANTIZATION WITH LEARNED ROTATIONS
1. 基于quarot的思想，通过正交矩阵选择weight/act来消除outlier
2. 本文的贡献在于，使正交矩阵可以学习和优化，而不是随机的。学习方法基于之前的工作：Caley SGD。