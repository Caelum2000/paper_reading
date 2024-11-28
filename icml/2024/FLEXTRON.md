## FLEXTRON: Many-in-One Flexible Large Language Model
1. 根据设备不同动态调整模型大小，可以调整子结构大小适应不同环境，见Fig.1
2. 训练的时候需要综合各个子结构的loss，见Eq.5。 子结构是随机选择的
3. 训练了一个surrogate model来确定选择哪些子结构，见Fig.3