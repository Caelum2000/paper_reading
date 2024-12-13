## CONTINUAL PRE-TRAINING OF LANGUAGE MODELS
1. 使llm增量的学习新内容，不需要获取前面任务的数据
2. 方法是计算模型参数对任务的重要性，然后加权地计算梯度
3. 用了激活对齐，见Eq.7