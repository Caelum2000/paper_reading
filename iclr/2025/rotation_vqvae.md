### RESTRUCTURING VECTOR QUANTIZATION WITH THE ROTATION TRICK
1. 指出vanilla VQ-VAE的梯度估计方式存在误差，方式是直接将quant后的code(decoder)的grad直接传到quant前的(encoder). 相当于quant函数的Jacobi是单位矩阵
2. 这个工作主要是让jacobi不是单位矩阵，定义了一种基于旋转的方式，见Sec.4.1。很大程度是受Vqvae quant梯度写法的启发，代码中会写成```q=e-detach(e-q) ```，他这个就是把这个改了
3. 感觉可解释性有待探讨，因为在q的一个邻域的e，梯度应该是相同的（都属于q）。但如果e变化量很大，那jacobi应该有一个阶跃？
4. 放relevant, 梯度的修正是否可以和类脑机制结合？