## Title: GENERALIZATION IN DIFFUSION MODELS ARISES FROM GEOMETRY-ADAPTIVE HARMONIC REPRESENTATIONS
1. 分析了DDPM泛化性的问题。就是仅学习数据集的一个子集是否真正学习到了data分布，而不是过拟合记住了图片。
2. 发现有泛化能力
3. 作者假设这种泛化能力是由于DNN的inductive bias导致的
4. 对DNN的Jacobi进行特征值分解，分析了特征值，发现特征向量符合geometry-adaptive harmonic bases. 这是调和分析的东西
5. 用实验验证了DNN的Jacobi特征值很可能符合geometry-adaptive harmonic bases。 但没有给出具体形式