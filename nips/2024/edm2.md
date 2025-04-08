## Guiding a Diffusion Model with a Bad Version of Itself
1. 与guidance相关，提出用同样模型生成的质量不好的图片来进行guidance。不用classifier-free 的null condition
2. 放waiting list

### review
1. 分析了clasifier-free guidance (CFG) 为什么不仅能让生成符合类别，还能让图像质量更好。作者的解释是在不加条件生成的时候需要考虑到所有类别，是一个更广的分布，因此对denoiser的要求更高
2. 提出用weaker的denoiser来guid新的denoiser，具体方法类似CFG，就是把输入empty condition换成weaker denoiser