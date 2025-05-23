### DISCRETIZATION-INVARIANCE? ON THE DISCRETIZATION MISMATCH ERRORS IN NEURAL OPERATORS
1. 主要是针对neural operator 的 discretization-invariance的问题
2. 提出先用一个lift把不同的input形状统一到相同维度的latent space，然后再用一个proj层把latent space 投影到output维度
3. lift和proj是通过DFT实现给定维度输出的