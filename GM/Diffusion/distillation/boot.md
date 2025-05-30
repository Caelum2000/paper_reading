### BOOT: Data-free Distillation of Denoising Diffusion Models with Bootstrapping
1. 给定$x_T$,和t, 直接一步生成$x_t$
2. 使用的是类似consistency model的对微观的连续性的对齐方法(Eq.7)。然后对齐了边界条件(Eq.9)
3. 代码开源，但是又删了