## Title: Robust agents learn causal world models
1. 因果推理和RL相关
2. 没看懂，需要学一下前置知识，可以参考文中的PRELIMINARIES
3. causal infer 的 course: https://www.bradyneal.com/causal-inference-course. 这个课程有对应的textbook，视频啰嗦可以看书
4. https://aaai23causalinference.github.io/ AAAI2023的tutorial


### review
1. 主要是证明了如果agent能对各种data shift下的env都能得到optimal policy. 那么可以由agent构建一个环境隐变量，决策变量和效用函数之间的causal model
2. 看了一个简单的证明过程