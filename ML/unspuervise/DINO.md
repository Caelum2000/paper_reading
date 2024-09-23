## Emerging Properties in Self-Supervised Vision Transformers
1. ViT对比学习+蒸馏
2. 蒸馏的student是正常梯度更新的网络。teacher是EMA的student，没有梯度，相当于model ensemble
3. 对比学习的方法是令student 和 teacher输出的不同view同一个所指的feature一致
4. KNN分类acc高， CLS token能学到特征