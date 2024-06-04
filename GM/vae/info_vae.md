## Title: InfoVAE: Information Maximizing Variational Autoencoders
1. 指出了VAE的ELBO的KL项可能会使x,z独立，从而出现collapse, 见Eq(1)
2. 将VAE的ELBO的KL项删除，得到AE-loss，见Eq(2). 这个loss可以表示成和互信息相关的形式，也就是说优化$L_{AE}$等价于增大x,z的互信息
3. 提出了一些其他的散度，这样可以祖先采样，即p(z)的先验符合某个分布。同时，可以不损失互信息。(proposition 2)
4. 问题：新提出的散度会不会导致第1条的问题？让x,z无关。