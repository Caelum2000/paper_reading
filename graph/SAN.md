## Rethinking Graph Transformers with Spectral Attention
1. 利用transformer处理图数据
2. 主要是研究怎么给graph的node embedding 进行位置编码。
3. 位置编码的方法是利用Laplace的特征值和特征向量，然后每个node的embedding加上对应位置的特征向量。然后这只是初始化，这个positional embedding还需要学习
4. Fig.1; Fig.4画的比较清楚
5. 问题：用Laplace特征向量初始化真的有效吗？因为后面需要学习才能得到positional embedding。如果网络足够强也许不需要Laplace? 但是Laplace没法使网络提前知道位置信息的bias。。。