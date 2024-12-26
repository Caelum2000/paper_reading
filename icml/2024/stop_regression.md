## Stop Regressing: Training Value Functions via Classification for Scalable Deep RL
1. 作者说目前value-based RL中 value func都是基于regression学习的
2. 为什么是基于Regression，可能需要复习一下RL基础
3. 该研究认为改成基于classification的 value学习更好
4. 放到waiting list

## review
1. 用cross-entropy代替需要计算td_error的RL方法，以此来学习Q值
2. 需要将目标值改为一个分布，这样才能计算KL散度
3. 需要将要学习的Q值离散化，转化为分类问题