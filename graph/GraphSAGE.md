## Inductive Representation Learning on Large Graphs
1. 在每一次迭代，随机选取邻接节点，然后通过一个aggregate将他们在这次迭代的特征聚合。然后和本节点的特征concat，经过线性变化得到下一次迭代的特征
2. Alg.1写的很清楚inference的过程
3. infernce过程中的参数需要学习，是通过无监督的相邻节点特征相似，不相邻节点的特征不相似的loss实现的（Eq.1）