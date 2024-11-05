## Low-Cost High-Power Membership Inference Attacks
1. 主要是研究MIA(Membership inference attack)问题，就是确定数据x是否用于训练了某个模型
2. 提出了一个指标LR, 见Eq.2. 是指定数据x和随机选取的数据z是否用于训练该模型的概率比值。要是LR高于某个阈值，则认为x用于训练模型
3. 问题：如何计算Eq.2中的$Pr(\theta|x)$