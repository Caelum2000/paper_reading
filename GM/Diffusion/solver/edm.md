### Elucidating the Design Space of Diffusion-Based Generative Models
1. 若$p(x_t|x_o)=N(x_t|s(t)x_0,s^2(t) \sigma^2(t) I)$, 则根据diffusion SDE的确定性的反向ODE，有Eq.2，当设置$s(t)=1$,则有Eq.1,这种情况下就是Variance explode. 
2. 该工作的主要贡献在于Alg.1，把Diffusion SMLD的过程看作类似梯度下降，并用Heun方法
3. 普通的梯度下降方法是Eluer, 使用了插值是Heun，Heun类似二阶 Runge–Kutta方法。
4. $\sigma(t)=1, s(t)=1$(类似variance explode)的反向SDE采样见Alg.2