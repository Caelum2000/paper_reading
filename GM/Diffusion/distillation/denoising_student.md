### Knowledge Distillation in Iterative Generative Models for Improved Sampling Speed
1. 对DDPM进行蒸馏，将多步的denoising过程蒸馏为一步
2. loss见Eq.10, Eq.11. 就是一个非常简单的MSE