### LVSM: A Large View Synthesis Model with Minimal 3D Inductive Bias
1. 大规模view生成
2. 之前view生成大多是基于3d表示的方法，，例如NeRF，GaussianSplatting等，然后在特定view render.
3. 本论文指出上述方法有inductive bias的限制，，因此采用transformer+pos condition的方法生成不同view，，没有explict 3d representation的过程.
4. 所谓消除 inductive bias 就是把3d表示模型换成transformer大力出奇迹