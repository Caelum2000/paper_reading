### MOE++: ACCELERATING MIXTURE-OF-EXPERTS METHODS WITH ZERO-COMPUTATION EXPERTS
1. 对moe进行加速，，设计了一些trivial expert, 比如只输出0，直接copy输入等等，不需要计算。。见method
2. 设计了平衡负载的loss，，就是比如zero expert计算的快，，就让他router分配的概率大一点