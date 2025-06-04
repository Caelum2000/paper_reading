### One-step Diffusion with Distribution Matching Distillation
1. obejctive为优化student生成的fake分布和真实数据分布的KL散度
2. KL散度的梯度里面有score function, 因此用一个pretrained diffuion来计算real pdf的score, 用一个待学习的diffusion来计算student生成的fake score
3. 这个待学习用来计算fake score的diffusion，的loss是和student一步生成的图片对齐。（这样类似EM算法，是否会造成不稳定问题？）
4. 需要一个额外的regression loss, 就是使student生成和真实图片对齐，仅用上述KL散度方法可能不work。
5. 没开源，但DMD-2开了