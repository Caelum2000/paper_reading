## Title: BATCHED LOW-RANK ADAPTATION OF FOUNDATION MODELS
1. LoRA是针对某个特定任务进行finetune，现在像对一个batch里不同任务进行推理‘
2. 问题在于LoRA无法并行训练多个任务
3. 本文提出一种并行的，类似LoRA的方法，可以实现多任务并行推理
4. 关键点在于Eq.2,3,4,5. 把LoRA的delta W相加变成了eletment-wise multi。这样可以写成并行的Eq.6
5. 还是比较巧妙。可以把eletment wise multi变成乘以(1+delta W). 虽然在full expressive下是等价的，但也许有了残差连接效果更好
6. 未开源，5的想法无法验证