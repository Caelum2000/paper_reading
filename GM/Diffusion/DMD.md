## One-step Diffusion with Distribution Matching Distillation
1. 将步数较多的diffusion蒸馏为一步生成器
2. 方法是优化KL散度，见Eq.1
3. 为什么score需要用denoiser来计算，不能直接用噪声代替？答：人工噪声是$p(x_t|x_0)$的score，我们需要的是$p(x_t)$的score，所以$p_{real}$需要用pretrained denoiser, 而$p_{fake}$需要另外训练一个denoiser
4. 注意$p_{fake}$的$x_0$应该是one step generator生成的分布，而$p_{real}(x_0)$应该是真实的分布(这也是pretrained denoiser的训练方法)