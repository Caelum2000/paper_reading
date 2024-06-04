## Title: Deterministic training of generative autoencoders using invertible layers
1. Flow model，类似VAE的结构，但不是VAE
2. 相比于VAE可以不优化ELBO，直接优化NLL，因为这是NF模型
3. 巧妙定义了残差分布，使encoder可逆
4. in practice, 又定义了一个网络扩展输入特征空间，详细见 Sec 3.2 