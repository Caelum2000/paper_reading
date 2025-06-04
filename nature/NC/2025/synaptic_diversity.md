### Concept transfer of synaptic diversity from biological to artificial neural networks
1. 主要研究突触多样性对神经网络的影响，研究方法是对ANN进行各种与突触相关的生物启发的改进
2. 主要是提出了三种突触启发的方式: Fuzzy learning rates (FL)，Weight rejuvenation (WR)，Weight splitting (WS)
3. FL的实现方式是给不同weight的学习率加一个随机值
4. WR的实现方式是，如果weight太小，那么重新初始化weight为随机值
5. WS的实现方式是，对一个输入通过lateral的n个weight，分别过了act func后再相加
6. 上面argue的方式其实是一种一如随机性的方式，也许可以用在SNN neural operator，放relevant
7. 开源