## DREAMGAUSSIAN: GENERATIVE GAUSSIAN SPLATTING FOR EFFICIENT 3D CONTENT CREATION
1. DreamFusion的后继工作，将其中的NeRF换成了GaussianSplatting
2. 采用了DreamFusion著名的SDS loss
3. 对纹理细节做了优化，方法是通过输入图片的纹理和经过StableDiffusion refine后的纹理的MSE对GS的参数进行优化
4. 训练速度很快，可以作为下一个工作的baseline