## SCALABLE LANGUAGE MODEL WITH GENERALIZED CONTINUAL LEARNING
1. 利用LoRA作LLM的continual learning
2. 对不同task的LoRA增量进行knn，然后找出中心，利用中心的LoRA增量加权更新
3. 加权的权重是利用对task的分布得到vector然后计算相似性得到的