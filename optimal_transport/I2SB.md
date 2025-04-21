### I2SB: Image-to-Image Schrodinger Bridge
1. 从schrodinger桥的角度解决任意两个分布之间的“演化”过程
2. 最后弄成了一个类似diffsuion的形式，是在一对(X1,X0)之间来进行插值，然后加噪声，最终的分布不是gaussian
3. 有一些理论的部分不太清楚比如为什么prop3.2能在$p(x_0)$和$p_b(x_1|x_0)$之间传输，貌似是在两个delta分布之间传输，或者这是一种denoise score matching 类似的东西