## Neural Collapse Meets Differential Privacy: Curious Behaviors of NoisyGD with Near-perfect Representation Learning
1. 预训练和差分隐私相关，放waiting list


### review
1. 是基于NoisySGD的工作，NoisySGD需要根据模型参数的维数来加噪声，但发现pretrained model不需要知道维数
2. 相关工作表明，pretrained model最后一层会neural collapse，就是一种特殊的特征模式，和参数的维数无关
3. 数学细节较多，没仔细看