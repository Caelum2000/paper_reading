### Inferring deterministic causal relations
1. 本文提出的背景是，我们有时候没法确定哪个是cause，哪个是effect。因此有了ANM模型，能确定的判断DAG的方向
2. 本文的论点是，即使不add noise, 也就是SCM的映射是一个确定函数的情况下，也能确定cause和effect的方向。
3. 假设是cause和mechanism是independ的，也就是原因和因果机制（如物理定律）相互没关系。
4. Fig.1展示了大致的思路，当cause X为uniform，mechanism f()的斜会影响effect p(Y)的分布。因此effect和f不是独立的。
5. Fig.1对于cause的假设可以推广，不一定是均匀分布。