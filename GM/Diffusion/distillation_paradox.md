### The paradox of diffusion distillation
1. 指出diffusion为什么不能一步走很长？因为本质是基于狼之丸动力学的采样，是基于score的。而该过程与SGD类似，score只是一个梯度。（因此一些optimization的方法可以adopt到diffusion, 例如动量，二阶方法等）
2. 为什么要在每一步加噪声：解释1是为了更新方向的随机性。也可以从denosing score matching的角度去解释？