## Do Transformers Really Perform Bad for Graph Representation?
1. transformer处理图数据的工作
2. 主要贡献还是设计将位置信息加入transformer，从而让transformer知道node在什么位置
3. 贡献1是将positioal embedding加入了根据node的degree计算重要性的部分，见Eq.5
4. 贡献2是在attention计算中加了相邻两个节点的最短路信息，见Eq.6