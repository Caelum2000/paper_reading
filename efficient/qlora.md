## QLORA: Efficient Finetuning of Quantized LLMs
1. 先量化，然后再对量化的模型Lora微调
2. 量化使用了一种新的数据类型: NormalFloat4. 4-bit的根据正态分布的分位数进行量化映射。即4-bit中不同的数值代表N(0,1)中不同分位数的点
3. 为什么normalfloat好？因为假设权重是正态分布的，更多的权重可能在mean附近，因此用分布的分位数能够使4个bit的数字出现的更均匀，在权重分布更多的区间用更多的数字去切分。否则可能只使用几个bit，其他bit用不到。
4. 在计算时需要将normalfloat反量化为BF16