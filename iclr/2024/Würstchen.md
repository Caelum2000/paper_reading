## Title: Würstchen: An Efficient Architecture for Large-Scale Text-to-Image Diffusion Models
1. 更高效的T2I diffusion, 训练的GPU hour, 数据量都有提升
2. 有三个stage: 
   1. stage 1: 训练一个有更高缩放因子的LDM，可以加入text信息
   2. stage 2: 利用stage 1的LDM生成的latent作 condition, 然后生成VQ-GAN的code. 也是一个LDM
   3. stage 3: VQ-GAN将stage 2 的code解码
3. 参数量比stabel diffusion大，因为需要3个stages
4. inference时间比stable diffusion. 因为仅在stage 1需要较大的time step. stage 2的time step很小
5. 开源