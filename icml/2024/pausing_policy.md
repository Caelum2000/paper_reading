## Pausing Policy Learning in Non-stationary Reinforcement Learning
1. 关注的是real-time强化学习，就是针对随时间变化的env来调整policy
2. 适当停止policy的更新可以获得更好的效果
3. 没仔细看，放到waiting list


### review
1. 需要看看related work的文章
2. 主要解决实时变化的状态转移函数以及reward, 见Sec.3
3. 提出适当暂停策略，就是不是一直持续的更新policy