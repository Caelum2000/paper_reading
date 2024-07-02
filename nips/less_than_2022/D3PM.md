## Title: Structured Denoising Diffusion Models in Discrete State-Spaces
1. 用于建模离散分布的DDPM
2. 提出了一系列方法，怎么给离散的分布加噪声。包括均匀转移矩阵，mask等
3. 由于分布是离散的$p_{\theta}(x_{t-1}|x_{t})$可以通过$\sum_{x_0} q(x_{t-1}|x_{t},x_0) p_{\theta}(x_{0}|x_{t})$得到。但是对于连续的DDPM，这是intractable的