## DREAM TO CONTROL: LEARNING BEHAVIORS BY LATENT IMAGINATION
## Mastering Atari with Discrete World Models
## Mastering Diverse Domains through World Models

1. dreamer系列，构建一个recurrent的世界模型RSSM，然后通过对世界模型采样来自我想象，推演动作轨迹的reward
2. RSSM的loss是信息瓶颈推导出来的，见dreamerV1
3. dreamerV2中是把隐变量表示成了vq-vae的codebook的形式
4. dreamerV3好像是多了一些trick，并且拓展了任务的范围