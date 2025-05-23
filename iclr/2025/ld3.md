### LEARNING TO DISCRETIZE DENOISING DIFFUSION ODES
1. 对diffusion需要的time step进行加速
2. 还是teacher, student的蒸馏。蒸馏的目标之一是选择student的最优时间步，而teacher的time step很高
3. 提出了一个soft的蒸馏loss，更容易训练
4. 是否可以和大脑中学习-推理的不同速度进行结合？