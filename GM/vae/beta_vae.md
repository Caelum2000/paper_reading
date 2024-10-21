## Title: β-VAE: LEARNING BASIC VISUAL CONCEPTS WITH A CONSTRAINED VARIATIONAL FRAMEWORK
1. 在VAE的ELBO的KL项加了一个系数beta
2. 该系数beta可以控制latent variable的disentangle, 也就是使z的不同元素控制不同的概念。为什么：因为KL让后验的z和先验的iid假设更类似。
3. 在disentangle和图像质量方面有一个负相关的关系。为什么：KL约束越强，z越受限制，所以会影响质量