## ICML 2024 tutorial: Neural Operator
1. neural opeartor learning 主要是关注输入一个函数，然后输出一个函数。区别于传统深度学习输入一个向量，输出一个向量
2. 输入neural opeartor的函数因为不能是获取在各个定义域的值（否则就会输入无限维），因此输入的本质还是一个向量。但我们希望输出的函数能在定义域各个点采样
3. 如何做到2? 可以用核函数的观点，见ppt，也可以用fourier transform的观点，见ppt的文献
4. 可以和PINN结合，使输出的函数满足特定ODE或条件
5. 有generative neural operator(ppt最后)，生成一个函数（或任意分辨率的图片），以后可以结合类似的工作？