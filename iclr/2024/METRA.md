## Title: METRA: SCALABLE UNSUPERVISED RL WITH METRIC-AWARE ABSTRACTION
1. 解决unsupervise RL 问题。对于unsupervised RL, 了解比较少。根据文中介绍，类似让agent 自己探索env
2. 通过一个隐变量z，使其与状态空间S相连，从而改进policy net。 应该之前是有类似的工作，可以看看
3. 本文提出之前的工作在处理z和S的关系的时候，是用的KL散度的方法，这不是一个好的metric，不利于梯度下降。本文采用Wasserstein metric(1-Wasserstein)改进objective
4. 提出了一系列的简化
5. 问题：引入z的意义是什么。从objective来看，仅是增强了z和S的相关性？需要看一下之前unsupervised RL的论文