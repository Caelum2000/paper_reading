## Title: PRE-TRAINING GOAL-BASED MODELS FOR SAMPLE-EFFICIENT REINFORCEMENT LEARNING
1. 具有层次的RL，一个high level policy生成goal state， 然后一个low level policy根据 goal state 生成轨迹
2. 本文主要是通过一个pretrained goal prior 来指导 high level 的policy（通过最小化KL）.
3. goal prior是什么原理，怎么实现的? 看related work之前的论文
4. 本文通过对goal states进行聚类来仅仅采样聚类中心的state，所谓sample efficient