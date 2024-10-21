## Title: Diffusion Models already have a Semantic Latent Space

1. 通过修改unet bottleneck的特征h，从而使已经pretrain好的diffusion editable。例如让图片微笑（利用CLIP实现）.
2. 非对称地进行修改。只修改预测到的x0，不修改加噪声的方向。具体见Eq(6). 因为文章证明对称地修改效果不好（当然这个证明比较weak）
3. 文章介绍了一些其他的修改方法，可以看看
4. 对h的修改有较好的性质