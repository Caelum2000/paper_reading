### Adapting Neural Networks for the Estimation of Treatment Effects
1. 核心的insight在于 Theorem 2.1。就是说ATE可以用propensity score进行condition。所以，这启发我们预训练一个propensity score的NN，然后用这个NN的中间特征作为condition去估计ATE
2. 具体的网络结构见Fig.1
3. 使用了一系列正则化方法，来自于非参数估计的trick，主要是保证估计的稳定等