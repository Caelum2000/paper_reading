## FINETUNING TEXT-TO-IMAGE DIFFUSION MODELS FOR FAIRNESS
1. 微调SD的工作
2. 目的是为了增强SD的公平性，比如没有性别，人种，年龄等歧视
3. 设计了一种loss，通过一个分类器，能将生成图片的分布拉向目标分布。利用的是最优传输
4. 改进了SD的直接微调方法，去掉了梯度中的一些项以保证梯度小方差
5. 使用的微调方法是直接微调，开销较大，有开源
6. related work里有一些SD微调的调研