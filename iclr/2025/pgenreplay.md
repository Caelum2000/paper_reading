### PRIORITIZED GENERATIVE REPLAY
1. 主要是针对RL的replay buffer进行改进
2. 通过生成模型conditional diffsuion来生成replay buffer的内容，并使用guidance来进行指导生成的需要replay的experience拉向对RL有用的环境动作对
3. 讲了memeory 的故事，naive replay buffer可以是短时的记忆，generative replay buffer是经过皮层之后的长期记忆
4. 放waiting list "relevant"部分