# Graph Learning:Principles,Challenges,and Open Directions.
## 来源：ICML2024 tutorial.
## website: https://icml2024graphs.ameyavelingker.com/

### 早期研究：学习图上节点的emdedding，该embedding表示图结构
1. random walk 方法

### MPNN
1. 思想：聚集节点，更新。以最后更新完的节点进行下游任务
2. GCN: 利用Lapalce矩阵
3. GraphSAGE: 随机选取相邻节点的MPNN
4. GAT: 利用attention确定聚集时相邻节点的权重

### Graph的数学工具
1. 主要是谱图理论的东西
2. Laplace特征向量
3. Cheeger consatnt: 最小割
4. 有效电导和Commute Time

### Graph transformer系列
1. 和MPNN不同，这种是利用transformer的全局特性（和GAT不一样，GAT还是MPNN）
2. 各种魔改位置编码: Spectral Attention Network(SAN)，Graphformer
3. 稀疏transformer解决大型图，小于O(N^2)：Exphormer
4. 将graph-transformer 和 MPNN结合：GraphGPS


### GNN的可表达性
1. 围绕MPNN能否突破 WL test展开
2. 突破WL方法: 增加特征，打破对称性。（Graph Substructure Networks）
3. 突破WL方法：更改传统MPNN，例如GAT，Directional Graph Networks 
4. 突破WL方法：采用高阶的例如基于k-WL的MPNN，这样能突破1-WL

### 泛化性
1. 这部分没仔细看，涉及机器学习理论


### Under-reaching
1. 就是网络“看不到”离得比较远的节点的关系
2. solution: 增加层数

### over-smoothing (OSM)
1. 各个节点学习到的feature或embedding都几乎一样，差别比较小。过度平滑
2. 有研究从random walk的stationary distribution角度解释了这个问题，但没有仔细看
3. 还有从GNN结构角度研究这个问题的，也没仔细看
4. solution：没仔细看

### over-squashing (OSQ)
1. 就是随着MPNN层数的增加，一次聚合涉及的节点指数上升
2. Solution: graph rewiring
   1. Spitial: 找到bottleneck
   2. Spectral: 根据Laplace特征值，没太看懂
   3. 增加virtual node

### OSM & OSQ的trade off
1. 没仔细看，意思大概是这两者可能此消彼长

