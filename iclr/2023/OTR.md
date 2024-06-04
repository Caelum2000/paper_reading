## Title: Optimal Transport for Offline Imitation Learning
1. 模仿学习的两种范式：行为克隆，逆强化学习。本文是逆强化学习，就是从特定MDP轨迹求reaward再用于offline RL.
2. 用OT最优传输，来对MDP求reward. 在求reward的时候需要一个expert demo（就是expert的MDP）。所以是模仿学习
3. 具体方法是通过OT来求未知的reward. 通过MDP和expert的相似度来求reward
4. 问题: 用OT的motivation是什么 