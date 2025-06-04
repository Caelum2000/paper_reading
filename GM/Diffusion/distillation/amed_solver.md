### Fast ODE-based Sampling for Diffusion Models in Around 5 Steps
1. 主要是针对已经训练好的diffusion，然后选择更少的时间步去求解微分方程
2. motivation是基于 mean value theorem. 相邻时间步之间有关系Eq.7, 因此根据mean-vlaue可以写成Eq.8. 因此只要学到中间的一个时间步$s_n$和scale factor $c_n$就可以。scale factor是为了适应不同的步长，类似学习率
3. 开源，但是是基于solver的加速方式，因此训练开销低，但要思考怎么加入snn