### LARP: TOKENIZING VIDEOS WITH A LEARNED AUTOREGRESSIVE GENERATIVE PRIOR
1. 研究内容是video版的vq-vae
2. 创新点主要有两个：一是使用了holistic token，，二是设计了一个autoregressive prior（（AR-prior））
3. 所谓holistic token是指把video 进行patch embedding后，，后面再加几个learnable prompt, 感觉只是加了可学习的参数。。使输入vq-vae的embedding都有相同的postfix
4. AR-prior是指，，在训练vq-vae的时候同时训练一个transformer-AR, 这样能在用AR采用的时候，，codebook更符合AR的inductive bias.