### DENOISING DIFFUSION IMPLICIT MODELS
1. 指出为了得到Eq.4中的margin PDF，不一定使用DDPM中markovian的diffusion过程。
2. 只需要按Eq.6和Eq.7中进行分解就可以得到Eq.4的形式。注意Eq.7中的$\sigma_t$是一个自由变量，可以设置成任意值
3. 将Eq.7中的$\sigma_t$设置为0，即可得到当$t>1$时的确定性的过程。
4. 怎么理解这个确定性过程？可以认为当t=1时加了噪声，但在$t>1$时将噪声进行push forward, 从而得出Eq.4
5. 基于以上论述，可以得出一个加速采样策略，就是仅在几步设置$\sigma_t \neq 0$, 其他时间步不需要denoise，只需要确定的映射（即通过NN学习x_0）