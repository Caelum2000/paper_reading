### Balls-and-Bins Sampling for DP-SGD
1. 首先指出了三种不同的对batch进行采样的方式：Deterministic，Shuffle，Poisson
2. DP-SGD可以视为将batch后的数据进行变换，因此batch的方式比较重要。
3. 之前的工作发现possion才有privacy保证，但possion采样不够简单
4. 本文主要提出一种简单且有privacy保证的采样方式