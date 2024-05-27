title: DIFFUSION POSTERIOR SAMPLING FOR GENERAL NOISY INVERSE PROBLEMS 

1. 解决了所谓 inverse problem 的 score function 的问题。即 $\nabla_{x_t} \log P(y|x_t)$
2. 这个问题其实在guidance里讨论了，但是本文是解决ill-posed的inverse problem, 即仅能知道$P(y|x_0)$ 的确定形式，对于$P(y|x_t)$, 无法知道形式
3. 问题：guidance 和 inverse problem 是两条线吗？两者之间的关系在相互的论文中没有提到
4. 解决方法是 用$\nabla_{x_t} \log P(y|\hat{x_0})$估计$\nabla_{x_t} \log P(y|x_t)$, $\hat{x_0}$ is a function of $x_t$
5. 具体的数学细节还没有check, 等着check一下