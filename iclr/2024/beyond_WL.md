## Title: BEYOND WEISFEILER-LEHMAN: A QUANTITATIVE FRAMEWORK FOR GNN EXPRESSIVENESS
1. 关于测量GNN表示能力的。利用的是同胚的方法
2. 没有学过GNN，先没看
3. GNN的course: stanford cs 224W


### review
1. 指出1-WL test的局限性
2. 提出一种基于图同态的度量GNN的表示能力的方法
3. 具体方法是对每一个GNN算法找到一个图集合，通过该算法能够得到该图集合F和所有图的同态关系（通过GNN算法得到的feature来计算），见def 3.1
4. 对一些常见的GNN，如MPNN，Subgraph GNN 通过一个叫NED（见def 3.3）来度量F之间的关系