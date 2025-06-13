### LATENT BAYESIAN OPTIMIZATION VIA AUTOREGRESSIVE NORMALIZING FLOWS
1. 主要是解决latent bayesian optimization的问题. LBO主要是把信息压缩到隐空间，然后进行bayes，以解决维数问题。但会有重建误差
2. 本文主要是采用normalizing flow去构建一个VAE，用可逆的方式解决上述问题
3. 不太了解bayesian optimization的问题和语境, 放waiting list