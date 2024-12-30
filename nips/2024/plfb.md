## Policy Learning from Tutorial Books via Understanding, Rehearsing and Introspecting
1. 通过书本的文本信息使agent做 offline RL
2. 分为三个stage，
   1. 第一个stage是提出textbook的文本为伪代码。
   2. 第二个是根据state生成action,然后retrival第一步的伪代码库，得到reward的next state (因为他假设textbook有env信息)
   3. 第三stage是收集上面的数据，然后进行offline RL
3. offline 算法是 conservative Q-learning
4. 本质上是将textbook的信息和知识，变成MDP的轨迹对，然后offline RL