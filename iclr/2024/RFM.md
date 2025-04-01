## Title: FLOW MATCHING ON GENERAL GEOMETRIES
1. 和黎曼几何以及flow model有关，PML推导玩flow再看
2. 在黎曼流形上的概率分布train flow模型
3. flow的论文（对应nips2024的tutorial）：Flow Matching Guide and Code


### review
1. 在流形上进行flow matching
2. 标准的flow matching 是用直线的连线作为vector field, 黎曼流形就是一般用测地线
3. 本文argue 测地线不容易计算，所以用一种叫做谱分解得到的“半径”
4. 现在的问题是：为什么要在流形上进行“生成”？之前有riemannian diffusion就是在riemannian manifold上进行生成, 看上去貌似是生成地图上的数据，这个motivation有点奇怪，因为流形可以嵌入R^n