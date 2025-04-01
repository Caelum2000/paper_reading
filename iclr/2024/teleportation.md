## Title: IMPROVING CONVERGENCE AND GENERALIZATION USING PARAMETER SYMMETRIES
1. 利用teleportation增强收敛速度和泛化能力，属于optim和ML theory范围
2. teleportation是找到另一组参数，使其与当前参数loss一致。可以理解为parameter空间的loss等势面
3. 数学以及细节没有细看，用空看一下，有点意思
4. data和parameter是否存在dual的关系，从而导致低曲率的最低点generalization好

### review
1. 之前有一系列的工作
2. 可以和meta-learning结合，通过teleportation初始化网络参数
3. 好像说teleportation可以找到泛化更好的点
4. 需要看李群的知识，正在看