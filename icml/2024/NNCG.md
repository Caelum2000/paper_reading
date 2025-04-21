## Challenges in Training PINNs: A Loss Landscape Perspective
1. 分析了PINN训练中的困难
2. 提出了一种新优化器NNCG
3. 放waiting list


### review
1. 指出了PINN训练中的问题，指出Hessian出现了较大的特征值（提示曲率较大，ill conditioned）
2. 通过分析指出是loss中的PDE residual项导致了大曲率
3. 提出了一些优化方法解决这个问题，这部分具体没看