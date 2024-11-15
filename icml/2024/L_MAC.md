## Listenable Maps for Audio Classifiers
1. 研究目标是找到找到梅林谱的一个mask，标记重要的区域，类GradCam的效果
2. 方法是将classifier的中间特征输入decoder，然后decoder学习到mask。然后使加了mask的input再次输入classifier，优化Eq.1 & Eq.2