## Less is More: on the Over-Globalizing Problem in Graph Transformers
1. 提出了graph transformer所具有的over globaling问题，就是会过多的考虑全局结构和较远的点
2. 将graph利用聚类算法拆分然后放transformer。transformer中有inter-cluster和intra-cluster的交互
3. 用GCN+graph transformer进行collaborative training。这里collaborative看起来像model ensemble，有作弊的嫌疑