## Scale Equivariant Graph Metanetworks
1. 基于GNN的hypernetwork，用于提取神经网络权重代表的信息
2. 放waiting list


### review
1. 通过GNN来处理神经网络的工作
2. 指出神经网络不仅有置换的对称性，还有scaling 对称性
3. 所谓scaling对称性是指在不同层之间乘额外矩阵可能导致最后输出不变，见Eq.3
4. 针对以上两种对称性设计网络，具体怎么设计的没仔细看