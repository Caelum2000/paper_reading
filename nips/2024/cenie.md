## Improving Environment Novelty Quantification for Effective Unsupervised Environment Design
1. 研究Unsupervised Environment Design (UED)问题
2. 不知道干什么的，放waiting list

## review
1. 通过一个GMM学习一个概率模型，来判断student的 state,action 对是否是小概率的
2. 如果state,action对是小概率的，那么认为teacher的env是novel的
3. 这种teacher-student的方式没太见过，还需调研