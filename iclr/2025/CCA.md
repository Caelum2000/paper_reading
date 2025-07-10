### TOWARD GUIDANCE-FREE AR VISUAL GENERATION VIA CONDITION CONTRASTIVE ALIGNMENT
1. 将classifer-free guidance的思想用到了自回归的图像生成模型上
2. 将CFG解释为训练一个constrative 的NCE loss. 见Eq.7和Theorem 3.1
3. 最后使用NCE训练原模型，，见Eq.11. 这个loss实质上是利用正确condition和错误condition作为正负样本对。然后对比学习训练模型，，因此能增强condition generation的效果.