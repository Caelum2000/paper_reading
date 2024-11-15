## DiJiang: Efficient Large Language Models through Compact Kernelization
1. 利用修改attention kernel的方法降低transformer的时间复杂度
2. 具体方法如Eq.4,将softmax修改成了kernel function。但我不太理解为什么会降低复杂度