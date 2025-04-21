## Parameterized Physics-informed Neural Networks for Parameterized PDEs
1. 提出一种新的PINN
2. 解决PDE的问题
3. 放waiting list


### review
1. 提出将PDE中的参数输入一个encoder，学到一个参数的latent feature, 然后再将其输入PINN
2. 这样的motivation主要是原始PINN中可能没有PDE的参数的信息。另外，这样便于微调