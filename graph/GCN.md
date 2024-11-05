## SEMI-SUPERVISED CLASSIFICATION WITH GRAPH CONVOLUTIONAL NETWORKS
1. 属于消息传递网络，通过聚合各个node的特征得到下一级node的特征
2. 采用了图上傅里叶变化来引入卷积，利用切比雪夫多项式来拟合卷积核（这只能是一种理论解释）
3. 最后得到的形式如Eq.2所示，前面的Laplace矩阵可以理解为将特征与相邻节点之间进行“平均”