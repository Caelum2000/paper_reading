## Title: LIPSCHITZ SINGULARITIES IN DIFFUSION MODELS
1. 经过一系列推导发现DDPM在t接近0的时候 Lipschitz constant很大，这会导致网络不光滑，不稳定
2. Lipschitz constant就是 $|f(x)-f(y)| \leq L |x-y|$中的L
3. 提出一种方法解决t=0附近L大的问题。就是把t=0附近分成几小段，然后对段内的t round到边界上。这样L在段内就是0 ($\frac{\epsilon(t_1)-\epsilon(t_2)}{\delta t}$)
4. 问题：这种方法是否会损失本来DDPM的性能，这和把time step减小有什么区别吗