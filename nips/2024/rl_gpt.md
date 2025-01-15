## RL-GPT: Integrating Reinforcement Learning and Code-as-policy
1. 使GPT是否要进行RL过程，RL过程的action是GPT写的代码
2. 需要一个额外的critic（也就是policynet?）
3. 整体没仔细看，放waiting list


## review
1. 有两个agent, slow agent和fast agent
2. slow agent负责把一个任务拆分成子任务，并决定每一个子任务是通过fast agent编写代码还是通过RL的policy net来生成动作
3. 有一个critic还对fast agent进行反馈，使fast agent不断refine