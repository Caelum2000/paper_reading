## Title: Smoothquant: Accurate and efficient post-training quantization for large language models
1. weight 和 activation 的最大值和scale不一样，通过Eq.3 Eq.4将weight和activation的scale变换成一致的，从而增加量化精度
2. 变换是对每个channel进行的，当确保activation不是离群点的时候，就会导致weight的对应channel趋向离群点，因此需要alpha参数进行权衡