## Probabilistic Inference in Language Models via Twisted Sequential Monte Carlo
1. 利用序列蒙特卡洛解释LLM中RHLF等问题？
2. 没太看懂
3. 是best paper，因此放到waiting list


### review
1. 本文使用了序列蒙特卡洛，就是类似序列的重要性采样的方法
2. 要解决什么问题：对指令reward下，对pretrained LLM进行采样，可以使用SMC
3. 将SMC过程参数化，并作为可以训练的NN，见Eq.9
4. Eq.21怎么对sigma采样没说太清楚