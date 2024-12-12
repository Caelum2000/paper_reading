## Offline Actor-Critic Reinforcement Learning Scales to Large Models
1. 提出了能够scale的 offline Actor-Critic的方法，打过了Behavior Clone
2. 方法好像介于传统方法和Behavior Clone 之间
3. 没仔细研究，放waiting list

### review
1. 本文研究离线强化学习，就是agent不与环境交互，根据其他policy的轨迹更新自己的policy （和模仿学习有什么区别）
2. offline RL 有NIPS2020 tutorial