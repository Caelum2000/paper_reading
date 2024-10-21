## Title: Model Tells You What to Discard: Adaptive KV Cache Compression for LLMs
1. compress KV cache 来减少计算资源
2. 不同的attention head有不同的compress 策略
3. 具体怎么选择策略是通过策略组合和枚举
4. 具体怎么实现compress写的不清楚，这部分可以看代码