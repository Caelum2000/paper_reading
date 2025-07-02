### TRANSFUSION: PREDICT THE NEXT TOKEN AND DIFFUSE IMAGES WITH ONE MULTI-MODAL MODEL
1. 设计了一种transformer的ppipeline，使其既能进行next-token-pred，又有ddpm去噪的能力。。
2. 其实还是transformer+AR的范式，只不过next token pred能够生成图片的latent, 见Fig.1
3. 改进了mask, 图片部分的mask不加，，见Fig.4