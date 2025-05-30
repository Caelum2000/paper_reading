### ACCELERATING DIFFUSION SAMPLING WITH CLASSIFIER-BASED FEATURE DISTILLATION
1. 基于progressive distillation进行修改
2. 把对齐student和teacher中间去噪的MSE改为了对齐一个分类器特征，见Eq.4
3. 同时注重了该分类器上的IS指标，见Eq.5, Eq.6. 这有点硬凑IS的意思
4. 代码中提供了progressive distill的cifar-10实现