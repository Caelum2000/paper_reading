### Fast Sampling of Diffusion Models via Operator Learning
1. 通过FNO将噪声$x_T$映射为具有时间轨迹的$x_{0:T}$，从而完成一步采样，当然这样也许不叫diffusion？
2. 网络结构前面有一个Lift层，将$x_T$加上时间维度
3. loss就是简单的MSE