### DSPO: DIRECT SCORE PREFERENCE OPTIMIZATION FOR DIFFUSION MODEL ALIGNMENT
1. diffusion进行价值观对齐，DPO的diffusion版本
2. 利用类似classifier-guidance类似的condition条件，将loss写成eq.10. 然后再用preference(Eq.4)+DPO最优条件(Eq.6)得到最终Eq.12,13的loss
3. 对比Eq.8和Eq.13, 一个需要优化denoising参数，一个需要对r求x_t的梯度