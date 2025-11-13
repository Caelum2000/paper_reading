### Causal Effect Inference with Deep Latent-Variable Models
1. 使用类似VAE的方法采样Fig.1中的图，并将其用于ITE估计，见Theorem 1
2. 主要的思想见Fig.2，具有一个inference network和model network。对应VAE的encoder和decoder。然后利用ELBO作为loss。
3. inference net用于推理，输入真实x的分布。model net用于生成，z具有先验分布。