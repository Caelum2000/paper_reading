## Offline Actor-Critic Reinforcement Learning Scales to Large Models
1. 提出了能够scale的 offline Actor-Critic的方法，打过了Behavior Clone
2. 方法好像介于传统方法和Behavior Clone 之间
3. 没仔细研究，放waiting list

### review
1. 本文研究离线强化学习，就是agent不与环境交互，根据其他policy的轨迹更新自己的policy （和模仿学习有什么区别）
2. offline RL 有NIPS2020 tutorial

1. 通过解析的求得最优的offline策略来得到目标policy, 见Eq.2, 其中用现在的Q来估计最优策略对应的Q
2. 设计Eq.3的loss来优化。可以分别理解每一项
3. 设计了可以scale的基于attention的Q和pi网络