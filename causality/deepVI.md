### Deep IV: A Flexible Approach for Counterfactual Prediction
1. 用于反事实预测。所谓反事实预测，就是在给出一个条件概率分布的情况下（事实），进行干预（反事实）。然后预测此类情况下对输出的影响。
2. Eq(1)是正常的SCM，Eq(2)是反事实的分布
3. 因为我们不可能在显示中去进行干预，只能通过观测到的数据进行预测。因此观测到的是Eq(3)而不是Eq(2)的“干预分布”。Eq(3)和Eq(2)之间的gap，如Eq(4)所示
4. 解决3中gap的方法是引入一个"instrument variable(IV)", IV的要求是仅对treatment variable产生影响，如Fig.1
5. 对于VI，有Eq(5)的关系。因此可以先学习$F(p|x,z)$, 再通过蒙特卡洛学习h(p,x)。见Sec.3中的first/second stage