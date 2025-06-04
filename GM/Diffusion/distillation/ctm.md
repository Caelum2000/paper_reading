### CONSISTENCY TRAJECTORY MODELS: LEARNING PROBABILITY FLOW ODE TRAJECTORY OF DIFFUSION
1. 基于consistency model进行改进，可以在任意两个时间步之间跳步
2. 有一些参数化方式来保证前后两个时间步相等的时候，增量等于0（见G(),g()）
3. 使用了一些辅助loss，例如DSM, GAN等
4. 提出了gamma采样，就是类似来回采样
5. 开源，cifar-10训练需要 4*V100