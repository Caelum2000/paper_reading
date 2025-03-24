## Discrete Diffusion Modeling by Estimating the Ratios of the Data Distribution
1. 基于DDPM生成离散数据的，可以打过GPT2
2. 开源
3. 具体方法是基于score matching推导的，没仔细看，放waiting list


### review
1. 需要先看看Eq.2 Eq.3是怎么来的，以及score是怎么推导出来的
2. 前序论文：SCORE-BASED CONTINUOUS-TIME DISCRETE DIFFUSION MODELS。在下面论文的基础上，不用ELBO，用score matching
3. 前序论文：A Continuous Time Framework for Discrete Denoising Models. 用连续时间的CTMC解决离散diffusion的问题，使用的是ELBO。之前的工作没用连续时间的模型
4. 能否使用SNN做一个离散diffusion，然后生成生物脉冲