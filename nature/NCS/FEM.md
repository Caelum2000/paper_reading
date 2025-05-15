## Free-Energy Machine for Combinatorial Optimization
1. 利用variational free energy(VFE)和SGD来解决组合优化问题(如SAT, MaxCut)
2. VFE是根据mean field 和 boltzmann distribution的KL散度导出来的
3. 本文SGD优化的objective 就是VFE，并将能量设计成组合优化问题得出解最小的形式
4. 问题：为什么优化VFE，换句话说优化mean field 和 boltzmann distribution的KL散度会最小化能量？不应该minimizing mean field分布和boltzmann distribution之间的差异吗？
5. 答：注意Eq.3，当 $\beta \rightarrow \inf$ 或 $T \rightarrow 0$的时候，等价于对平均场求能量的均值，这时候既会拉近平均场和boltzmann的距离，又会最小化能量，这也是为啥将这个KL散度成为“变分自由能”