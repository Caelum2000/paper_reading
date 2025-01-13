## DenoiseRep: Denoising Model for Representation Learning
1. 利用DDPM denoise的过程来进行分类
2. 方法是先通过forward的网络来获取特征，再使用denoise的方法来获取特征。然后融合这两个参数