## Title: A Free Lunch From ANN: Towards Efﬁcient, Accurate Spiking Neural Networks Calibration
1. 利用soft-reset LIF。问题：怎么将softrest LIF变成spike
2. 提出了clip loss 和 floor loss. 问题：Eq.10 中clip里面也是spike，但需要的是ann的激活和spike的对比，因此这样是否合理
3. 通过对clip & floor loss的分析，发现膜电位阈值很重要。因此通过一个MSE和SG调整阈值
4. 同样的方法，通过MSE调整W,b等